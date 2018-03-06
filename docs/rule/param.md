# 参数规定

### Query string格式要求

除了每个接口自定义的参数之外，请求URL参数中应该包含该的以下参数：

**参数格式：**

```
url?sync_time=1474861722907617&random_str=h5qgq9on&count=100&token=AuPIMicoJZ2PknHwFxHil6zDKyiX2hn9qk5c4GA6kENz4saTTiGvEoq4wlYXP7WX
```

**说明： **

|参数名|必选|类型|说明|
|:----    |:---|:----- |-----   |
|sync_time |是  |string |上次请求获取到的时间戳（具体查看[协议规则](http://doc.liexiong.cc/#/rule/token) ）  |
|random_str     |是  |string | 8位随机字符串    |
|count     |否  |int | 请求的数量    |
|token     |是  |string | 请求凭证   |


*** sync_time(时间戳)： ***

16 位的 Unix 时间戳（微妙级），用来表示当前已经同步的位置。

Python 示例

```python
    import time
    t = int(time.time() * 1000000)
```

*** random_str: ***

- 随机字符串，用来表示请求的唯一性，

*** count: ***
- 请求数量，非必选项，1-1000,默认是100。

*** token:***
- 请求的合法性凭证，需要通过[token接口](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8D%8F%E8%AE%AE%E8%A7%84%E5%88%99)获得。