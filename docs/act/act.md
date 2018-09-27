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

其他同[参数规定](http://doc.liexiong.cc/#/rule/param)

**返回示例：**

```json
{
    "msg":"success",
    "status":"200",
    "sync_time":"1469586420332999",
    "data":[
        {
            "zone_exclude": [],
            "receive_description": "",
            "usage_scene": [],
            "subject_description": "招商银行信用卡持卡人",
            "banks": [
                {
                    "name": "招商银行",
                    "id": 11
                }
            ],
            "card_orgs": [],
            "act_type": 1,
            "end_date": "2018-07-25",
            "available_time_ranges": [
                {
                    "day": null,
                    "weekday": 2,
                    "range_type": 2,
                    "start_time": 36000,
                    "end_time": 86100
                }
            ],
            "title": "小大董 50 元购 100 元代金券",
            "id": 399702,
            "category": [
                {
                    "name_en": "",
                    "name": "中餐",
                    "id": 316
                }
            ],
            "display_tags": [],
            "original_url": "https://piao.o2o.cmbchina.com/shopwindow/weixinProductDetail?cityNo=10&productNo=9918062803721",
            "zone_include": [
                "北京"
            ],
            "special_weekdays": [],
            "act_area": null,
            "small_img_url": null,
            "payment": [
                {
                    "name_en": "",
                    "name": "网银快捷支付",
                    "id": 169
                }
            ],
            "create_time": "2018-07-01 09:03:35.319000",
            "update_time": "2018-07-16 09:55:53.570000",
            "money_limit": null,
            "subject": {
                "name": "bank",
                "type": 1
            },
            "content": "##### 参与方式\n- 通过「掌上生活 APP」购劵\n- 至「小大董」使用\n\n##### 活动内容\n- 活动期间，招商银行信用卡持卡人**每周三上午 10:00** 至招行「掌上生活 APP」50 元购「小大董」100 元代金券\n\n##### 注意事项\n- 仅限周三使用\n- 可与招商银行常规优惠券叠加使用\n- 不与商户其他优惠同享\n- 有效期内限购买 1 张\n- 具体使用细则请以银行和门店公告为准\n\n",
            "big_img_url": "https://qnpic.billbear.cn/Fs1P6xchqJwyYvGTpUNhHZROcgpl",
            "quota": "数量有限，先到先得",
            "is_hot": 0,
            "discount": [
                {
                    "name_en": "free_coupon",
                    "name": "享券",
                    "id": 22
                }
            ],
            "special_dates": [],
            "unavailable_time_ranges": [],
            "status": 1,
            "start_date": "2018-07-04",
            "zone_include_id": [
                567
            ],
            "original_title": "(周三5折）小大董100元代金券",
            "zone_exclude_id": []
        },
        {
            "zone_exclude": [],
            "receive_description": "",
            "usage_scene": [],
            "subject_description": "招商银行信用卡持卡人",
            "banks": [
                {
                    "name": "招商银行",
                    "id": 11
                }
            ],
            "card_orgs": [],
            "act_type": 1,
            "end_date": "2018-12-31",
            "available_time_ranges": [
                {
                    "day": null,
                    "weekday": 2,
                    "range_type": 2,
                    "start_time": 36000,
                    "end_time": 79200
                }
            ],
            "title": "韩宫宴 50 元购 100 元代金券",
            "id": 396297,
            "category": [
                {
                    "name_en": "barbecue",
                    "name": "烧烤",
                    "id": 196
                }
            ],
            "display_tags": [],
            "original_url": "https://piao.o2o.cmbchina.com/shopwindow/weixinProductDetail?cityNo=572&productNo=9918062701041",
            "zone_include": [
                "湖州"
            ],
            "special_weekdays": [],
            "act_area": null,
            "small_img_url": null,
            "payment": [
                {
                    "name_en": "",
                    "name": "网银快捷支付",
                    "id": 169
                }
            ],
            "create_time": "2018-07-07 09:44:20.371000",
            "update_time": "2018-07-16 09:55:45.259000",
            "money_limit": null,
            "subject": {
                "name": "bank",
                "type": 1
            },
            "content": "##### 参与方式\n- 通过「掌上生活 APP」购劵\n- 至「韩宫宴」使用\n\n##### 活动内容\n- 活动期间，招商银行信用卡持卡人**每周三上午 10:00** 至招行「掌上生活 APP」50 元购「韩宫宴」100 元代金券\n\n##### 注意事项\n- 仅限周三使用\n- 有效期内限购买 20 张\n- 单笔订单限购 1 张\n- 具体使用细则请以银行和门店公告为准\n\n",
            "big_img_url": "https://qnpic.billbear.cn/FlvfTBZw7OwlVGRjXCWuQ2m5Sal6",
            "quota": "数量有限，先到先得",
            "is_hot": 0,
            "discount": [
                {
                    "name_en": "free_coupon",
                    "name": "享券",
                    "id": 22
                }
            ],
            "special_dates": [],
            "unavailable_time_ranges": [],
            "status": 1,
            "start_date": "2018-07-01",
            "zone_include_id": [
                607
            ],
            "original_title": "（周三5折）韩宫宴100元代金券",
            "zone_exclude_id": []
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
|subject|dict|活动主体（活动是银行还是卡组织发起的）|
|bank|list|参与的银行|
|card_orgs|list|参与的卡组织|
|start_date|string|活动开始日期|
|end_date|string|活动结束日期|
|category | list |活动分类|
|discount | list |活动的优惠类型（例如：打折、立减、兑换）|
|pay_forms|list|支付方式（例如：POS刷卡、ApplePay）|
|pay_brands | list | 活动支付渠道（美团支付、京东支付等）|
|available_time_ranges|list | 可用时间(详细见下文说明) |
|unavailable_time_ranges|list | 不可用时间(详细见下文说明) |
|display_tags|list | 特殊标签 |
|zone_include|list|参与地区|
|zone_exclude|list|不参与地区|
|zone_include_id|list|参与地区id, 对应地区表id|
|zone_exclude_id|list|不参与地区id|
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
|way |string|参与方式（刷呗上叫参与流程）|
|requirements|list| 参与前置条件|
|note|string|注意事项|
|quota|string | 活动名额|
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
