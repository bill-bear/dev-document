# 卡片和活动关系
   
**简要描述：** 

- 卡片和活动关联关系接口

**请求URL：** 
- ` /base_data/v1/act_card_ref `
  
**请求方式：**
- GET

**参数：**
- 同[参数规定](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8F%82%E6%95%B0%E8%A7%84%E5%AE%9A)

**返回示例：**

```json 
{
    "data": [
        {
            "act_id": 24428,
            "card_id": 1967,
            "create_time": "2016-08-05 15:46:55.725000",
            "id": 2,
            "status": 1,
            "update_time": "2017-04-07 11:07:01.281889"
        },
        {
            "act_id": 24428,
            "card_id": 2286,
            "create_time": "2016-08-05 15:46:55.725000",
            "id": 1,
            "status": 1,
            "update_time": "2017-04-07 11:07:01.281844"
        }
    ],
    "msg": "success",
    "status": "200",
    "sync_time": "1491534421281889"
}
```

**返回参数说明：** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|card_id | int | 卡片id|
|act_id |int   |活动id  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|




