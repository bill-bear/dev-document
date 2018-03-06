# 货币

**简要描述：**

- 包含全部货币（ALL），以及一些主要货币（人民币、美元、日元、）
- 如果一个新的货币没有罗列出来，就通过有没有（ALL）来判断。

**请求URL：**
- `/base_data/v1/currency`

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
            "code":"CNY",
            "create_time":"2016-06-22 09:23:15.127000",
            "id":2,
            "name":"人民币",
            "status":1,
            "symbol":null,
            "update_time":"2016-07-12 09:54:12.344000"
        },
        {
            "code":"ALL",
            "create_time":"2016-06-22 09:23:15.117000",
            "id":1,
            "name":"全币种",
            "status":1,
            "symbol":null,
            "update_time":"2016-07-12 09:54:12.339999"
        },
        .....
    ]
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----  |
|id |int   |对象唯一标示  |
|name |string   |名称  |
|code |string   |编码  |
|symbol |string   |符号  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
