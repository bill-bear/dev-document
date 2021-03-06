# 活动分类

**简要描述：**

- 活动标签接口。

**请求URL：**
- `/base_data/v1/act_tag`

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
            "id": 283,
            "level": 3,
            "name": "超市",
            "name_en": "",
            "parent_id": 222,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.395000"
        },
        {
            "create_time": "2017-05-22 10:21:55.390000",
            "id": 282,
            "level": 3,
            "name": "商场",
            "name_en": "",
            "parent_id": 222,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.390000"
        },
        {
            "create_time": "2017-05-22 10:21:55.384000",
            "id": 281,
            "level": 3,
            "name": "其他运动健身",
            "name_en": "",
            "parent_id": 221,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.384000"
        },
        {
            "create_time": "2017-05-22 10:21:55.379000",
            "id": 280,
            "level": 3,
            "name": "健身房",
            "name_en": "",
            "parent_id": 221,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.379000"
        },
        {
            "create_time": "2017-05-22 10:21:55.373000",
            "id": 279,
            "level": 3,
            "name": "网球",
            "name_en": "",
            "parent_id": 221,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.373000"
        },
        {
            "create_time": "2017-05-22 10:21:55.367000",
            "id": 278,
            "level": 3,
            "name": "游泳",
            "name_en": "",
            "parent_id": 221,
            "status": 1,
            "update_time": "2017-05-22 10:21:55.367000"
        },
        .....
    ]
}
```

**返回参数说明：** 
 
|参数名|类型|说明|
|:-----  |:-----|-----|
|id |int   |对象唯一标识  |
|name |string   |活动标签|
|name_en |string   |活动标签英文 |
|level |int   |标签等级  |
|parent_id|int| 父级标签|
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|



