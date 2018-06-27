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
            "name_en": "",
            "parent_id": 379,
            "parent_name": "杭州",
            "zone_type": 5,
            "mongo_id": "5979b0090926a83a9102f0e8",
            "name": "下城区",
            "id": 3306,
            "adcode": "330103",
            "update_time": "2018-06-27 10:46:26.859000",
            "citycode": "0571",
            "create_time": "2017-07-27 17:19:05.380000",
            "status": 1
        },
        {
            "name_en": "",
            "parent_id": 379,
            "parent_name": "杭州",
            "zone_type": 5,
            "mongo_id": "5979b0090926a83a9102f0e7",
            "name": "上城区",
            "id": 3305,
            "adcode": "330102",
            "update_time": "2018-06-27 10:46:26.850000",
            "citycode": "0571",
            "create_time": "2017-07-27 17:19:05.370000",
            "status": 1
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
|adcode | string|高德区域编码 |
|citycode | string | 高德城市编码|
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

