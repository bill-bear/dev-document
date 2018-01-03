# 权益信息
   
**简要描述：** 

- 卡片权益接口

**请求URL：** 
- ` /base_data/v1/card_benefit `
  
**请求方式：**
- GET

**参数：**
- 同[参数规定](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8F%82%E6%95%B0%E8%A7%84%E5%AE%9A)


**返回示例：**

```json 
{
    "data": [
        {
            "bank": {
                "id": 15,
                "name": "中信银行"
            },
            "card_org": {},
            "content": "##### 活动\n· 积分换钢蹦：当月计积分交易（含取现）达 800 元累积 1 京东钢镚\n\n",
            "create_time": "2016-08-30 14:29:10.709000",
            "id": 438,
            "original_url": "http://creditcard.ecitic.com/shenqing/jingdong/index.shtml?netId=ECCXBKNX",
            "status": 0,
            "subject": {
                "name": "bank",
                "type": 1
            },
            "tags": [
                {
                    "name": "卡片专享"
                }
            ],
            "title": "中信京东白条联名卡享积分换钢蹦",
            "update_time": "2016-12-14 15:21:15.355000",
			"benefit_type": 1,
			"zone_include": [15, 71],
			"zone_exclude": [],
			"zone_include_description": "华东地区",
			"zone_include_description": "",
			"start_date":"2016-04-06",
			"end_date":"2020-06-29",
			"available_time_ranges": [
				{
					"end_time": 86400,
					"day": 1493222400.0,
					"start_time": 0,
					"weekday": null,
					"range_type": 3
				}
			],
			"unavailable_time_ranges": [
				{
					"end_time": 86400,
					"day": 1493136000.0,
					"start_time": 0,
					"weekday": null,
					"range_type": 3
				}
			],
			"instruction" : "- 关注微信民生信用卡，在汽车服务里选加油卡兑换",
			"usage_count_unlimited" : 0,
			"repay_description" : "淘宝",
        },
        {
            "bank": {
                "id": 17,
                "name": "上海银行"
            },
            "card_org": {},
            "content": "##### 活动\n· 「不限商户，不限商品」的消费分期付\n· 在消费额度内消费金额满 1000 元以上，可申请分期付款\n\n",
            "create_time": "2016-12-12 15:58:21.505000",
            "id": 1554,
            "original_url": "http://www.cardbaobao.com/card/cardinfo/shanghaiyinhangxinyongka_1449.shtml#tsgn_2",
            "status": 0,
            "subject": {
                "name": "bank",
                "type": 1
            },
            "tags": [],
            "title": "分期自由",
            "update_time": "2016-12-12 17:53:36.921000",
			"benefit_type": 2,
			"zone_include": [75, 76],
			"zone_exclude": [],
			"zone_include_description": "华东地区",
			"zone_include_description": "",
			"start_date":"2016-04-06",
			"end_date":"2018-06-29",
			"available_time_ranges": [],
			"unavailable_time_ranges": [],
			"instruction" : "- 关注微信民生信用卡，在汽车服务里选加油卡兑换",
			"usage_count_unlimited" : 0,
			"repay_description" : "淘宝",
        }
    ],
    "msg": "success",
    "status": "200",
    "sync_time": "1481700075355000"
}
```

**返回参数说明：** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|id |int   |对象唯一标示  |
|bank | dict | 银行|
|card_org |dict   |卡组织  |
|content |string   |权益内容，markdown格式  |
|original_url |string   | 原文链接  |
|subject|dict|区分是银行权益还是卡组织权益|
|tags|list|标签|
|title | string | 标题 |
|benefit_type | int | 权益类型 1 线上 2 线下 3 两者 |
|zone_include | list | 参与地区 |
|zone_exclude | list | 不参与地区 |
|zone_include_description | string | 参与地区备注  |
|zone_exclude_description | string | 不参与地区备注 |
|start_date|string|开始日期|
|end_date|string|结束日期|
|available_time_ranges|list | 可用时间(详细见下文说明) |
|unavailable_time_ranges|list | 不可用时间(详细见下文说明) |
|instruction|string| 使用说明 |
|usage_count_unlimited | int | 是否不限次数 1是 0否 |
|repay_description | 回报描述 |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|


**可用与不可用时间：**

|参数名|类型|说明|
|:-----  |:-----|-----|
| day |timestamp|日期|
|start_time|int|开始时间(秒)|
|end_time|int|结束时间(秒)|
|weekday|int | 星期， 0是星期一，6为星期日|
|range_type|int|1 每一天 2 星期 3 特殊日期 |

比如：available_time_ranges: [{
	"end_time": 86400,
	"day": 1493222400.0,
	"start_time": 0,
	"weekday": null,
	"range_type": 3
}]
表示就2017年4月27日这一天0点到24点可用

