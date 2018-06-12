# 地区

**简要描述：**

- 地区分为4个界别，分别是洲、国、省、市；
- 地区的数据应该在2000条左右，考虑到上下级关系，最好能够同步一次同步过去，以免出现id找不到的情况。

**请求URL：**
- `/base_data/v1/zone`

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
            "create_time":"2016-07-27 10:27:00.332999",
            "id":100,
			"mongo_id": '57981bf30926a858b31257ee',
            "name":"委内瑞拉",
            "name_en":"Venezuela",
            "parent_id":5,
            "parent_name":"南美洲",
            "status":1,
            "update_time":"2016-07-27 10:27:00.332999",
            "zone_type":2
        },
        {
            "create_time":"2016-07-27 10:27:00.328000",
            "id":99,
			"mongo_id": '57981bf30926a858b31257ee',
            "name":"孟加拉",
            "name_en":"Bangladesh",
            "parent_id":1,
            "parent_name":"亚洲",
            "status":1,
            "update_time":"2016-07-27 10:27:00.328000",
            "zone_type":2
        },
        .....
    ]
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|mongo_id | string | 也是对象唯一标示，活动商户地区用这个关联|
|name |string   |名称  |
|name_en |string   |英文名称  |
|parent_id |string   |父级的id  |
|parent_name|string|父级的名称|
|zone_type|string|地区的界别|
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|

**zone_type解释**

|级别|说明|
|:-- |:-- |
|1|洲（亚洲、欧洲等）|
|2|国家（中国、美国等）|
|3|省（安徽、江苏等）|
|4|城市（合肥、安庆、黄山等）|
|5|县级市，区（昆山市，徐汇区等）|

