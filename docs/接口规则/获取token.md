# 获取token

**简要描述：**

- 获取token接口

**请求URL：**
- `/core/v1/token `

**请求方式：**
- POST

**参数：**
```json
  {
    "access_key": 'ta3gzb9lovq424zrgzkl0o13jqc4f7yd',
    "sign": "9DAF21F50797DCBC9B643B7B306188C0"，
    "time": '1499767733.013236'
  }
```

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|access_key |是  |string |烈熊提供的access_key   |
|sign |是  |string |签名 |
|time |是  |float |当前时间的，Unix时间戳 |

 **返回示例**

```json
  {
    "expires_in": 20317,
    "access_token": "AuPIMicoJZ2PknHwFxHil6zDKyiX2hn9qk5c4GA6kENz4saTTiGvEoq4wlYXP7WX"
  }
```

 **返回参数说明**

|参数名|类型|说明|
|:-----  |:-----|-----|
|expires_in |int   |返回的token的剩余有效期（最大86400秒）  |
|access_token  |string   |token  |

## 签名计算方法 ##
1. 将需要加密的非空参数值的参数按照参数名ASCII码从小到大排序（字典序），使用键值对的格式（即key1:value1&key2:value2…）拼接成字符串stringA。
2. 在stringA后面拼接上“&secret_key={sk}”
3. 对字符串进行md5求值。

Python示例：
```python
import hashlib

params = {
    "access_key": ‘ta3gzb9lovq424zrgzkl0o13jqc4f7yd’,
    "time": '1499767733.013236'
}
secret_key = 'wud1sfd3mrdmygs1z5l8bk4glo9v9qlz'
string_a = '&'.join(['{}:{}'.format(k, params[k]) for k in sorted(params.keys()) if params[k] and k != 'sign'])
print(string_a) # access_key:20317&time:1477535149

string_sign_temp = "{}&secret_key={}".format(string_a, secret_key)
print(string_sign_temp)  # access_key:20317&time:1477535149&secret_key=123456789

hlb = hashlib.md5()
hlb.update(string_sign_temp.encode('utf-8'))
md5 = hlb.hexdigest().upper()
print(md5)  # 9DAF21F50797DCBC9B643B7B306188C0
```

## Python Demo ##
```python
import json
import requests

data = {
    'access_key': "syd43yni3fde3h46vz70pl8ns4orbt5s",
    'sign': "56069FDBBC05D360E77759459F2477C8",
    'time': 1502033319
}

resp = requests.request('POST', 'http://openapi-test.billbear.cn/core/v1/token',
                  headers={'Content-Type': 'application/json', }, data=json.dumps(data))
resp_obj = json.loads(resp.text)
print(resp_obj)

# 返回： {'access_token': '61FCu7Y92WeHWpeQutt9Dz5k7Tnp6WFO5uPx4bgpCJU4XTobi08zRAjWRJenQ9nt', 'expires_in': 84762}
```

## Java Demo ##
```java
package com.billbear.common.web.util;

import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStream;
import java.io.InputStreamReader;
import java.io.OutputStream;
import java.io.StringWriter;
import java.net.HttpURLConnection;
import java.net.URL;
import java.security.SecureRandom;

import javax.net.ssl.HostnameVerifier;
import javax.net.ssl.HttpsURLConnection;
import javax.net.ssl.KeyManager;
import javax.net.ssl.SSLContext;
import javax.net.ssl.SSLSession;

public class HttpInvokeUtil
{
  public static final String DEFAULT_CHARSET = "UTF-8";

  private HttpInvokeUtil()
  {
    throw new UnsupportedOperationException();
  }

  public static String doPost(String url, String params, int connectTimeout, int readTimeout)
    throws Exception
  {
    return doPost(url, params, "UTF-8", connectTimeout, readTimeout);
  }

  public static String doPost(String url, String param, String charset, int connectTimeout, int readTimeout)
    throws Exception
  {
	String ctype = "application/json";
    byte[] content = new String(param).getBytes();
    return doPost(url, ctype, content, connectTimeout, readTimeout);
  }

  public static String doPost(String url, String ctype, byte[] content, int connectTimeout, int readTimeout)
    throws IOException
  {
    HttpURLConnection conn = null;
    OutputStream out = null;
    String rsp = null;
    try
    {
      conn = getConnection(new URL(url), "POST", ctype);

      conn.setConnectTimeout(connectTimeout);
      conn.setReadTimeout(readTimeout);
      out = conn.getOutputStream();
      out.write(content);
      rsp = getResponseAsString(conn);
    }
    finally
    {
      if (out != null) {
        out.close();
      }
      if (conn != null) {
        conn.disconnect();
      }
    }
    return rsp;
  }

  private static HttpURLConnection getConnection(URL url, String method, String ctype)
    throws IOException
  {
    HttpURLConnection conn = null;
    if ("https".equals(url.getProtocol()))
    {
      SSLContext ctx = null;
      try
      {
        ctx = SSLContext.getInstance("TLS");
        ctx.init(new KeyManager[0], new DefaultTrustManager[] { new DefaultTrustManager() }, new SecureRandom());
      }
      catch (Exception e)
      {
        throw new IOException(e);
      }
      HttpsURLConnection connHttps = (HttpsURLConnection)url.openConnection();
      connHttps.setSSLSocketFactory(ctx.getSocketFactory());
      connHttps.setHostnameVerifier(new HostnameVerifier()
      {
        public boolean verify(String hostname, SSLSession session)
        {
          return true;
        }
      });
      conn = connHttps;
    }
    else
    {
      conn = (HttpURLConnection)url.openConnection();
    }
    conn.setRequestMethod(method);
    conn.setDoInput(true);
    conn.setDoOutput(true);
    conn.setRequestProperty("cache-control", "no-cache");
    conn.setRequestProperty("Content-Type", ctype);
    conn.setRequestProperty("postman-token", "1483499d-f0d6-19a3-65d6-f7624d571a15");
    return conn;
  }

  public static void main(String[] args) throws Exception {

	  String param="{\"access_key\": \"qrguetfa58mtsgnmhfbbm8er4j40h8g1\",\"sign\": \"6A01C17F3F4C48B161D798BF7E927F76\",\"time\": 1506993752}";

	  System.out.println(HttpInvokeUtil.doPost("https://openapi.billbear.cn/core/v1/token", param, 100000, 100000));
  }

  protected static String getResponseAsString(HttpURLConnection conn)
    throws IOException
  {
    String charset = getResponseCharset(conn.getContentType());
    InputStream es = conn.getErrorStream();
    if (es == null) {
      return getStreamAsString(conn.getInputStream(), charset);
    }
    String msg = getStreamAsString(es, charset);
    if (StringUtil.isEmpty(msg)) {
      throw new IOException(conn.getResponseCode() + ":" + conn.getResponseMessage());
    }
    throw new IOException(msg);
  }

  private static String getStreamAsString(InputStream stream, String charset)
    throws IOException
  {
    try
    {
      BufferedReader reader = new BufferedReader(new InputStreamReader(stream, charset));
      StringWriter writer = new StringWriter();

      char[] chars = new char['?'];
      int count = 0;
      while ((count = reader.read(chars)) > 0) {
        writer.write(chars, 0, count);
      }
      return writer.toString();
    }
    finally
    {
      if (stream != null) {
        stream.close();
      }
    }
  }

  private static String getResponseCharset(String ctype)
  {
    String charset = "UTF-8";
    if (!StringUtil.isEmpty(ctype))
    {
      String[] params = ctype.split(";");
      for (String param : params)
      {
        param = param.trim();
        if (param.startsWith("charset"))
        {
          String[] pair = param.split("=", 2);
          if ((pair.length != 2) ||
            (StringUtil.isEmpty(pair[1]))) {
            break;
          }
          charset = pair[1].trim(); break;
        }
      }
    }
    return charset;
  }

}




// DefaultTrustManager.java

package com.billbear.common.web.util;

import java.security.cert.CertificateException;
import java.security.cert.X509Certificate;
import javax.net.ssl.X509TrustManager;

public class DefaultTrustManager
  implements X509TrustManager
{
  public X509Certificate[] getAcceptedIssuers()
  {
    return null;
  }

  public void checkClientTrusted(X509Certificate[] chain, String authType)
    throws CertificateException
  {}

  public void checkServerTrusted(X509Certificate[] chain, String authType)
    throws CertificateException
  {}
}
```

 **备注**

- token的最大有效期是86400秒（24\*60\*60）,当请求生成一个token之后，在token没有失效之前，继续请求token，token不变，但是返回的token剩余有效期会相应的变小。
