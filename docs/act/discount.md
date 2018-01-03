# 活动优惠类型

**简要描述：**

- 活动优惠类型接口。

**请求URL：**
- `/base_data/v2/act_discount`

**请求方式：**
- GET

**参数：**

- 同[参数规定](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8F%82%E6%95%B0%E8%A7%84%E5%AE%9A)

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
    "data":[
         {
            "create_time": "2017-05-22 10:21:55.395000",
            "id": 18,
            "name": "打折",
            "name_en": "discount",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.395000"
        },
        {
            "create_time": "2017-05-22 10:21:55.390000",
            "id": 20,
            "name": "兑换",
            "name_en": "exchange",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.390000"
        },
        {
            "create_time": "2017-05-22 10:21:55.384000",
            "id": 22,
            "name": "享券",
            "name_en": "free_coupon",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.384000"
        }
    ]
}
```

**返回参数说明：** 
 
|参数名|类型|说明|
|:-----  |:-----|-----|
|id |int   |对象唯一标识  |
|name |string   |活动标签|
|name_en |string   |活动标签英文 |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|



