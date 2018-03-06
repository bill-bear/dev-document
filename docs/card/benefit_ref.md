# 卡片和权益关系
   
**简要描述：** 

- 卡片和权益关联关系接口

**请求URL：** 
- ` /base_data/v1/card_benefit_ref `
  
**请求方式：**
- GET

**参数：**
- 同[参数规定](http://doc.liexiong.cc/#/rule/param)


**返回示例：**

```json 
{
    "data": [
        {
            "benefit_id": 2,
            "card_id": 1380,
            "create_time": "2016-07-07 12:14:18.849000",
            "id": 2,
            "status": 1,
            "update_time": "2016-07-12 09:54:12.256000"
        },
        {
            "benefit_id": 1,
            "card_id": 1380,
            "create_time": "2016-07-07 12:04:38.913000",
            "id": 1,
            "status": 1,
            "update_time": "2016-07-12 09:54:12.251000"
        }
    ],
    "msg": "success",
    "status": "200",
    "sync_time": "1468288452256000"
}
```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|card_id | int | 卡片id|
|benefit_id |int   |权益id  |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|




