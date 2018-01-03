# 活动信息

**简要描述：**

- 活动有较多的属性，而且各个银行的活动差异较大，这里提供了尽可能详细的信息。

**请求URL：**
- `/base_data/v2/act`

**请求方式：**
- GET

**参数：**

|参数名|类型|说明|
|:-----  |:-----|-----|
|display_style |string   |html和markdown两者之一，默认为markdown  |

其他同[参数规定](http://doc.liexiong.cc/#/%E6%8E%A5%E5%8F%A3%E8%A7%84%E5%88%99/%E5%8F%82%E6%95%B0%E8%A7%84%E5%AE%9A)

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
    "data":[
        {
            "banks":[
                {
                    "id":14,
                    "name":"招商银行"
                }
            ],
            "card_orgs":[],      # 主体是银行，则卡组织字段为空，反之亦然
            "category":[
                {
                    "id":51,
                    "name":"火锅",
                    "name_en":"hotpot"
                },
                {
                    "id":53,
                    "name":"冷饮",
                    "name_en":"cold_drink"
                },
                {
                    "id":55,
                    "name":"其他美食",
                    "name_en":"other_food"
                },
                {
                    "id":50,
                    "name":"自助餐",
                    "name_en":"buffet"
                }
            ],
            "content":"##### 活动内容 1. 即日起至2016年6月29日每周三招行卡至掌上生活享50元购花千锅价值100元代金券1张。 1. 每位客户最多购买1张。 ##### 注意事项 - 凭代金券验证码至上海花千锅大宁国际店验证后使用，一经验证使用不可退款。 - 5折券可与招行天天享美食代金券一起使用。 - 仅支持周三购买，且仅限每周三使用。 - 仅限堂食自助餐，不提供外带。",
            "create_time":"2016-06-06 14:41:01.000000",
            "discount":[
                {
                    "id":18,
                    "name":"打折",
                    "name_en":"discount"
                }
            ],
            "end_date":"2016-06-29",
            "id":100,
            "original_title":"",
            "original_url":"http://market.cmbchina.com/ccard/5zqxms/index.html",
            "big_img_url":"https://qnpic.billbear.cn/images/act/57551837?imageMogr2/crop/!749.0013315579228x399.46737683089214a0a0/thumbnail/!100p",
            "start_date":"2016-04-06",
            "status":1,
            "subject":{
                "name":"bank",
                "type":1
            },
            "title":"招行卡周三50元购大宁国际花千锅100元代金券",
            "update_time":"2016-06-21 15:56:36.048000",
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
			"zone_include": [
                685,
            ]
			"zone_exclude": [
                237,
            ]，
			"subject_description": "VISA 信用卡持卡人",
			"act_type": 1,
			"participate_info" : {
                "way" : "到门店报名，然后在app注册",
                "requirements" : [
                    "拥有浦发银行信用卡",
                    "开通网上支付"
                ],
                "note" : "注意必须要先报名，才可享受优惠",
                "quota" : "20",
                "need_reserve" : true,
                "reserve_description" : "app预约",
                "need_apply" : true,
                "apply_description" : "app报名"
            },
            "period_usage_limits" : [
                {
                    "period_type" : 3,
                    "usage_count" : 10,
                    "usage_count_unlimited" : false
                },
                {
                    "period_type" : 5,
                    "usage_count" : 1,
                    "usage_count_unlimited" : false
                },
            ],
            "pay_brands": [1,4,8],
            "pay_forms": [3,6]
        },
        {
            "banks":[
                {
                    "id":14,
                    "name":"招商银行"
                }
            ],
            "card_orgs":[
            ],
            "category":[
                {
                    "id":55,
                    "name":"其他美食",
                    "name_en":"other_food"
                },
                {
                    "id":50,
                    "name":"自助餐",
                    "name_en":"buffet"
                }
            ],
            "content":"##### 活动内容 1. 即日起至2016年6月29日每周三上午10点招行卡至掌上生活享50元购新石器烤肉价值100元代金券1张。 1. 每位客户仅限抢购2张。 ##### 注意事项 - 抢兑商品是否成功购买以收到验证码为准，是否使用以商户验证核实为准。 - 本券仅限堂食，不提供外带、打包服务，酒水饮料等问题请致电商家咨询，以商家反馈为准。 - 可累计使用。 - 不兑现，不找零，不与其他优惠同享。",
            "create_time":"2016-06-06 13:25:39.000000",
            "discount":[
                {
                    "id":18,
                    "name":"打折",
                    "name_en":"discount"
                }
            ],
            "end_date":"2016-06-29",
            "id":99,
            "original_title":"",
            "original_url":"http://market.cmbchina.com/ccard/5zqxms/index.html",
            "start_date":"2016-06-01",
            "status":1,
            "subject":{
                "name":"bank",
                "type":1
            },
            "title":"招行卡周三50元购新石器烤肉100元代金券",
            "update_time":"2016-06-21 15:56:36.046999",
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
			"zone_include": [
                685
            ],
			"zone_exclude": [
               237
            ],
			"subject_description": "VISA 信用卡持卡人",
			"act_type": 2,
			"participate_info" : {
                "way" : "到门店报名，然后在app注册",
                "requirements" : [
                    "拥有浦发银行信用卡",
                    "开通网上支付"
                ],
                "note" : "注意必须要先报名，才可享受优惠",
                "quota" : "20",
                "need_reserve" : true,
                "reserve_description" : "app预约",
                "need_apply" : true,
                "apply_description" : "app报名"
            },
            "period_usage_limits" : [
                {
                    "period_type" : 3,
                    "usage_count" : 10,
                    "usage_count_unlimited" : false
                },
                {
                    "period_type" : 5,
                    "usage_count" : 1,
                    "usage_count_unlimited" : false
                },
            ],
            "pay_brands": [1,4,8],
            "pay_forms": [3,6]
        },
        .....
    ]
}
```

**返回参数说明：** 
 
|参数名|类型|说明|
|:-----  |:-----|-----|
|id |int   |对象唯一标识  |
|title |string   |活动标题（编辑之后的标题，信息更加明确）|
|original_title |string   |原始标题 |
|content |string   |活动内容，markdown格式  |
|original_url|string| 活动原文链接|
|big_img_url|string|大图标地址|
|subject|string|活动主体（活动是银行还是卡组织发起的）|
|bank|list|参与的银行|
|card_orgs|list|参与的卡组织|
|start_date|string|活动开始日期|
|end_date|string|活动结束日期|
|category | list |活动分类|
|discount | list |活动的优惠类型（例如：打折、立减、兑换）|
|pay_form|list|支付方式（例如：POS刷卡、ApplePay）|
|pay_brand | list | 活动支付渠道（美团支付、京东支付等）|
|available_time_ranges|list | 可用时间(详细见下文说明) |
|unavailable_time_ranges|list | 不可用时间(详细见下文说明) |
|display_tags|list | 特殊标签 |
|zone_include|list|参与地区|
|zone_exclude|list|不参与地区|
|subject_description|string |参与对象（活动对象）|
|act_type|int| 1线上  2线下 3 两者|
|participate_info | json | 参与信息（包括是否需预约、是否需报名、活动名额、活动前置条件等）|
|period_usage_limits | json | 周期 |
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

**参与信息：**

```json
"participate_info" : {
		"way" : "到门店报名，然后在app注册",
		"requirements" : [
			"拥有浦发银行信用卡",
			"开通网上支付"
		],
		"note" : "注意必须要先报名，才可享受优惠",
		"quota" : "20",
		"need_reserve" : true,
		"reserve_description" : "app预约",
		"need_apply" : true,
		"apply_description" : "app报名"
	},
```

|参数名|类型|说明|
|:-----  |:-----|-----|
|way |string|参与方式|
|requirements|list| 参与前置条件|
|note|string|注意事项|
|quota|int | 活动名额|
|need_reserve|bool|是否需要预约 |
|reserve_description | string | 预约说明 |
|need_apply | bool | 是否需要报名 |
|apply_description | string | 报名说明 |


**周期：**

```json
"period_usage_limits" : [
		{
			"period_type" : 3,
			"usage_count" : 10,
			"usage_count_unlimited" : false
		},
		{
			"period_type" : 5,
			"usage_count" : 1,
			"usage_count_unlimited" : false
		},
	],
# 这个表示每月限额10次，其中每日限1次
```

|参数名|类型|说明|
|:-----  |:-----|-----|
|period_type |int|周期类型 1 每年 2 每季 3 每月 4 每周 5 每日 6 每半年|
|usage_count| int | 使用次数 |
|usage_count_unlimited|bool| 是否不限次数|
