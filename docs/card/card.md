# 卡片信息
    
**简要描述：** 

- 信用卡卡片数据同步接口

**请求URL：** 
- ` /base_data/v1/card `
  
**请求方式：**
- GET

**参数：**
- 同[参数规定](http://doc.liexiong.cc/#/rule/param)


**返回示例：**

```json
 {
    "data": [
        {
            "annual_fee": 200,
            "annual_fee_currency": {
                "code": "CNY",
                "id": 2,
                "name": "人民币"
            },
            "annual_fee_free": 1,
            "annual_fee_rule": "首年免年费，刷卡 5 次免次年年费",
            "apply_url": null,
            "attached_card_limit": 0,
            "bank": {
                "id": 18,
                "name": "农业银行"
            }
            "card_orgs": [
                {
                    "id": 3,
                    "name": "VISA-银联"
                }
            ],
            "create_time": "2016-07-12 16:37:29.230000",
            "currency": [
                {
                    "code": "CNY",
                    "id": 2,
                    "name": "人民币"
                },
                {
                    "code": "USD",
                    "id": 3,
                    "name": "美元"
                }
            ],
            "id": 548,
            "img_url": "https://qnpic.billbear.cn/FpAyqIt2E-kyIkWKzzKpmaebXGrd",
            "is_hot": 1,
            "is_primary": 1,
            "level": {
                "id": 11,
                "name": "金卡"
            },
            "name": "农行 VISA 浙江都市网联名卡（金卡）",
            "point_rule": [
                {
                    "input_unit": "CNY",
                    "input_value": "1",
                    "output_unit": "积分",
                    "output_value": "1",
                    "tag": "标准"
                },
                {
                    "input_unit": "USD",
                    "input_value": "1",
                    "output_unit": "积分",
                    "output_value": "6",
                    "tag": "标准"
                }
            ],
            "issue_zones": [
                597
            ],
			"issue_zones_name": [
                "长春"
            ],
            "point_validity_description": "信用卡有效积分可以继续累积直至销户",
            "status": 1,
            "tags": [
                {
                    "children": [
                        {
                            "id": "5769e8830926a83c3b8553dd",
                            "level": 2,
                            "name": "女性"
                        },
                        {
                            "id": "5769e8830926a83c3b8553de",
                            "level": 2,
                            "name": "DIY"
                        },
                        {
                            "id": "5769e8830926a83c3b8553df",
                            "level": 2,
                            "name": "地方"
                        },
                        {
                            "id": "5769e8830926a83c3b8553e0",
                            "level": 2,
                            "name": "其他"
                        }
                    ],
                    "id": 149,
                    "level": 1,
                    "name": "特殊卡"
                },
                {
                    "id": 160,
                    "level": 2,
                    "name": "地方"
                },
                {
                    "name": "浙江"
                }
            ],
            "update_time": "2017-03-14 17:49:56.463000",
			"interest_free_period": "50",
			"min_repayment_description": "10%(刷卡金额+取现金额)+100%（当期分期金额+上期最低还款额未还金额+超额使用款项+费用利息）",
			"hotlines": [
				{
					"description": "境内服务电话",
					"phone": "400-820-5555"
				},
				{
					"description": "境外服务电话",
					"phone": "+86-4008205555"
				}
			],
        },
        {
            "annual_fee": 200,
            "annual_fee_currency": {
                "code": "CNY",
                "id": 2,
                "name": "人民币"
            },
            "annual_fee_free": 1,
            "annual_fee_rule": "首年免年费，刷卡消费满 5 次或以上免次年年费",
            "apply_url": "http://www.abchina.com/cn/CreditCard/ApplyCard/cardinfo/201601/t20160128_827529.htm",
            "attached_card_limit": -1,
            "bank": {
                "id": 18,
                "name": "农业银行"
            },
            "bin_code": [
                "40411700"
            ],
            "card_orgs": [
                {
                    "id": 3,
                    "name": "VISA-银联"
                }
            ],
            "create_time": "2016-10-11 11:45:58.698000",
            "currency": [
                {
                    "code": "CNY",
                    "id": 2,
                    "name": "人民币"
                },
                {
                    "code": "USD",
                    "id": 3,
                    "name": "美元"
                }
            ],
            "id": 2516,
            "img_url": "https://qnpic.billbear.cn/FokvIg673o4yh82MrzN7gWfTrrfC",
            "is_hot": 1,
            "is_primary": 1,
            "level": {
                "id": 11,
                "name": "金卡"
            },
            "name": "农行 VISA 浙江都市网联名卡（金卡）",
            "point_rule": [
                {
                    "input_unit": "CNY",
                    "input_value": "1",
                    "output_unit": "积分",
                    "output_value": "1",
                    "tag": "标准"
                }
            ],
            "issue_zones": [
                597
            ],
			"issue_zones_name": [
                "长春"
            ],
            "point_validity_description": "永久有效",
            "status": 1,
            "tags": [
                {
                    "children": [
                        {
                            "id": "5769e8830926a83c3b8553d3",
                            "level": 2,
                            "name": "航空"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d4",
                            "level": 2,
                            "name": "酒店"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d5",
                            "level": 2,
                            "name": "百货"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d6",
                            "level": 2,
                            "name": "超市"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d7",
                            "level": 2,
                            "name": "校园"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d8",
                            "level": 2,
                            "name": "网络"
                        },
                        {
                            "id": "5769e8830926a83c3b8553d9",
                            "level": 2,
                            "name": "公司"
                        }
                    ],
                    "id": 147,
                    "level": 1,
                    "name": "联名卡"
                },
                {
                    "id": 155,
                    "level": 2,
                    "name": "网络"
                },
                {
                    "name": "浙江都市网"
                }
            ],
            "update_time": "2017-03-09 10:14:15.393000",
			"interest_free_period": "50",
			"min_repayment_description": "10%(刷卡金额+取现金额)+100%（当期分期金额+上期最低还款额未还金额+超额使用款项+费用利息）",
			"hotlines": [
				{
					"description": "境内服务电话",
					"phone": "400-820-5555"
				},
				{
					"description": "境外服务电话",
					"phone": "+86-4008205555"
				}
			],
        }
    ],
    "msg": "success",
    "status": "200",
    "sync_time": "1489484996463000"
}

```

 **返回参数说明** 

|参数名|类型|说明|
|:-----  |:-----|-----                           |
| id  | int | 卡片唯一标识 |
|annual_fee |int   | 年费金额 |
|annual_fee_currency |dict   | 年费货币 |
|annual_fee_rule  |string  | 年费描述 |
|annual_fee_free_rule | json | 年费规则 |
|apply_url  | string | 申卡链接 |
|attached_card_limit  | int | 附属卡数量 |
|bank  | dict | 银行 |
|card_orgs  | list | 卡组织 |
|currency  | list | 货币 |
|img_url  | string | 卡图片 |
|is_hot  | int | 是否热门卡 |
|is_primary  | int | 是否主卡 |
|level  |dict  |卡级别  |
|name  |string  |名称  |
|point_rule  |list  |积分规则  |
|point_validity_description  | string | 积分有效期 |
|interest_free_period | string | 免息期 |
|min_repayment_description | string | 最低还款额|
|hotlines| list | 信用卡热线|
|tags | json |  卡分类 |
|issue_zones|list|发卡城市id，id对应到地区表 |
|issue_zones_name|list|发卡城市名称 |
|status|int|状态（1：正常，0：无效）|
|create_time|string|创建时间|
|update_time|string|更新时间|


**年费规则：**

```
"annuel_fee_free_rules" : [
		{
			"time_type" : 0,
			"rules" : [
				{
					"free_type" : 2
				}
			]
		}
	],
```

|参数名|类型|说明|
|:-----  |:-----|-----                           |
|time_type  | int | 0所有时间 1首年 2次年及以后 |
|free_type |int   | 1终身免 2全免 3不免 4满次免 5满额免 6积分抵金额 7积分抵部分 |
