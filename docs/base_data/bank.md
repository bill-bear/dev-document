# 银行

**简要描述：**

- 这里只包含烈熊数据中使用到的银行。

**请求URL：**
- `/base_data/v1/bank`

**请求方式：**
- GET

**参数：**
- 同[参数规定](http://doc.liexiong.cc/#/rule/param)

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
    "data":[
        {
            "create_time":"2016-06-22 09:23:15.105000",
            "id":8,
            "logo_url":"https://qnpic.billbear.cn/icon_guangfa.png",
            "name":"广发银行",
            "name_en":null,
            "status":1,
            "update_time":"2016-09-21 10:12:41.282000"
        },
        {
            "create_time":"2016-06-22 09:23:15.111000",
            "id":12,
            "logo_url":"https://qnpic.billbear.cn/icon_pingan.png",
            "name":"平安银行",
            "name_en":null,
            "status":1,
            "update_time":"2016-09-21 10:12:41.279999"
        },
        .....
    ]
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|name |string   |名称  |
|name_en |string   |英文名称  |
|logo_url |string   |logo地址  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|

