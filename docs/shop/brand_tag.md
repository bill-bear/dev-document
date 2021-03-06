# 品牌标签

**简要描述：**

- 品牌标签接口。

**请求URL：**
- `/base_data/v2/brand_category`

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
            "create_time": "2017-05-22 10:21:55.395000",
            "id": 339,
            "name": "电影院",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.395000"
        },
        {
            "create_time": "2017-05-22 10:21:55.390000",
            "id": 175,
            "name": "餐饮",
            "status": 1,
            "update_time": "2017-05-22 10:21:55.390000"
        },
        {
            "create_time": "2017-05-22 10:21:55.384000",
            "id": 162,
            "name": "酒店",
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
|name |string   |门店品牌标签|
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|



