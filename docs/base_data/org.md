# 卡组织

**简要描述：**

- 主流的6个卡组织。
- 一些卡是有多个卡组织发行的，比如银联-VISA信用卡，这些数据数作为特殊卡组织存在的。

**请求URL：**
- `/base_data/v1/card_org`

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
            "create_time":"2016-06-22 09:23:15.153000",
            "id":6,
            "logo_url":"https://qnpic.billbear.cn/DINERSCLUB@2x.png",
            "name":"大莱",
            "name_en":"DinersClub",
            "short_name":null,
            "status":1,
            "update_time":"2016-09-21 11:11:53.315999"
        },
        {
            "create_time":"2016-06-22 09:23:15.151999",
            "id":5,
            "logo_url":"https://qnpic.billbear.cn/AMERICANEXPRESS@2x.png",
            "name":"运通",
            "name_en":"AmericanExpress",
            "short_name":null,
            "status":1,
            "update_time":"2016-09-21 11:11:38.043999"
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
|name_en |string   |英文名称|
|logo_url|string|logo地址|
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
