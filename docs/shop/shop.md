# 商户

**简要描述：**

- 当前对象依赖品牌信息
- 烈熊尽可能保证这里信息的严谨性，但是由于商户信息的特殊性，很难做到百分百准确，比如商户电话，商户随时都可能调整电话信息。

**请求URL：**
- `/base_data/v1/shop`

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
            "address":"香洲区碧海路1号星程酒店",
            "brand":{
                "id":21851,
                "name":"星程酒店"
            },
            "city":{
                "id":671,
                "name":"珠海"
            },
            "coordinate":{
                "latitude":22.269779,
                "longitude":113.579789
            },
            "create_time":"2016-08-23 09:37:59.901000",
            "id":2,
            "name":"星程酒店-中餐厅",
            "status":1,
            "tags":[
                "住宿服务",
                "宾馆酒店",
                "经济型连锁酒店"
            ],
            "tel":[
                "0756-2121666"
            ],
            "update_time":"2016-05-23 13:20:53.000000"
        },
        {
            "address":"徐汇区虹桥镇虹梅路2071号远中产业园四期1号楼2f-2102",
            "brand":{
                "id":null,
                "name":null
            },
            "city":{
                "id":685,
				"mongo_id": '57981bf30926a858b31257ee',
                "name":"上海"
            },
            "coordinate":{
                "latitude":31.171715,
                "longitude":121.393356
            },
            "create_time":"2016-08-23 09:37:59.071000",
            "id":1,
            "name":"上海烈熊网络",
            "status":1,
            "tags":[
                "高端网络服务",
                "顶级互联网公司",
            ],
            "tel":[

            ],
            "update_time":"2016-05-23 10:55:35.000000"
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
|address|string|地址|
|brand |dict   |品牌  |
|city |dict   |城市  |
|coordinate|dict|坐标|
|tags| list|标签|
|tel|list|电话|
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|
