# 品牌

**简要描述：**

- 品牌作为商户的主要属性之一，单独记录可以有效避免数据的冗余。

**请求URL：**
- `/base_data/v1/brand`

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
            "create_time":"2016-08-05 15:20:07.760999",
            "id":6,
            "logo_url":"https://qnpic.billbear.cn/images/amap/575d5254?imageMogr2/crop/!200x200a0a0/thumbnail/!100p",
            "name":"德克士",
            "status":1,
            "update_time":"2016-08-05 15:20:07.760999"
        },
        {
            "create_time":"2016-08-05 15:20:13.071000",
            "id":36,
            "logo_url":"https://qnpic.billbear.cn/images/amap/575cbb9d?imageMogr2/crop/!196x196a0a0/thumbnail/!102p",
            "name":"中石油",
            "status":1,
            "update_time":"2016-08-05 15:20:13.071000"
        },
        .....
    ]
}
```

**返回参数说明：** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|name |string   |名称  |
|logo_url |string   |logo地址  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
