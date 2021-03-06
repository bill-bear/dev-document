# 卡级别

**简要描述：**

- 不同卡组织的不同卡级。

**请求URL：**
- `/base_data/v1/card_level`

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
            "card_org":{
                "id":2,
                "name":"万事达"
            },
            "create_time":"2016-06-22 09:23:15.161999",
            "id":2,
            "name":"金卡",
            "name_en":"Gold",
            "status":1,
            "update_time":"2016-07-12 09:54:12.089999"
        },
        {
            "card_org":{
                "id":2,
                "name":"万事达"
            },
            "create_time":"2016-06-22 09:23:15.155999",
            "id":1,
            "name":"普卡",
            "name_en":"Classic",
            "status":1,
            "update_time":"2016-07-12 09:54:12.086999"
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
|card_org |对象   |卡组织信息  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
