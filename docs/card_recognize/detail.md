*卡片详细

**简要描述：**

- 返回卡片的详细信息

**请求URL：**
- `/api/v3/detail/card`

**请求方式：**
- GET

**参数：**
```json
 {
      "random_str": "h5qgq9on",
      "token": "AuPIMicoJZ2PknHwFxHil6zDKyiX2hn9qk5c4GA6kENz4saTTiGvEoq4wlYXP7WX",
      "first_code": "52885600",   # 必须是8位，如不足8位，后面补0
      "last_code": "1234",
      'card_id': '88',
	  'order_by': "update_time",          # update_time按更新时间排序 act_yield按活动收益率排序
  }
```

 **返回示例**

```json
{
    "data": {
        "card_benefit": [
            {
				"id": 1650,
                "original_url": "http://www.icbc.com.cn/ICBC/%E7%89%A1%E4%B8%B9%E5%8D%A1/%E7%99%BD%E9%87%91%E5%8D%A1/%E8%87%B3%E5%B0%8A%E5%95%86%E5%8A%A1%E7%A4%BC%E9%81%87.htm",
                "title": "工行牡丹 MasterCard 白金卡全球机场贵宾室服务",
                "tags": [
                    {
                        "name": "航空礼遇"
                    }
                ],
                "content": "· 持有我行前期配发 PP 卡的客户可继续享受 PP 卡全球机场贵宾室服务。我行已对PP卡机场贵宾厅增值服务进行调整，详询白金卡贵宾专线 4000095588 \n"
            },
            {
			    "id": 1652,
                "original_url": "http://www.icbc.com.cn/ICBC/%E7%89%A1%E4%B8%B9%E5%8D%A1/%E7%99%BD%E9%87%91%E5%8D%A1/%E8%BD%BB%E6%9D%BE%E5%93%81%E5%91%B3%E4%BA%BA%E7%94%9F.htm",
                "title": "工行牡丹/尊尚/百夫长白金卡女性俱乐部",
                "tags": [
                    {
                        "name": "其他"
                    }
                ],
                "content": "· 为您提供覆盖北京、上海、广州、深圳四个大型城市的女性俱乐部服务。俱乐部以“女性健康、身心幸福”作为服务核心，为有文化、有品位且志趣相投的女性提供一个休闲场所与精神驿站\n"
            },
            {
			    "id": 1653,
                "original_url": "http://www.icbc.com.cn/ICBC/%E7%89%A1%E4%B8%B9%E5%8D%A1/%E7%99%BD%E9%87%91%E5%8D%A1/%E8%87%B3%E5%B0%8A%E5%95%86%E5%8A%A1%E7%A4%BC%E9%81%87.htm",
                "title": "工行白金卡机场/高铁贵宾厅服务礼遇",
                "tags": [
                    {
                        "name": "航空礼遇"
                    }
                ],
                "content": "· 中国工商银行为工银白金信用卡客户提供机场和高铁贵宾厅服务，只要出示您的白金卡，就可以免费使用我行指定的机场和高铁自有贵宾厅，使您的旅途倍添尊贵与舒适\n"
            },
        ],
        "annual_fee": {
            "annual_fee_currency": {
                "id": 2,
                "code": "CNY",
                "name": "人民币"
            },
            "annual_fee": 2000,
            "annual_fee_rule": "",
            "annual_fee_free": 0
        },
        "img_url": "http://www.icbc.com.cn/ICBC/html/card/newcard/images/ky/1872mh-158.gif",
        "name": "工行牡丹万事达1872联名卡（白金卡）",
        "bank": {
            "id": 8,
            "name": "工商银行"
        },
        "id": 88,
		"act_ids": [
            9520,
            24229,
            32593,
            32600,
            33396,
		},
        "card_org": [
            {
                "id": 2,
                "name": "万事达"
            },
            {
                "id": 1,
                "name": "银联"
            }
        ],
        "level": {
            "id": 4,
            "name_en": "Platinum",
            "name": "白金卡"
        },
        "annual_fee_rule": "",
        "currency": [
            {
                "id": 1,
                "code": "ALL",
                "name": "全币种"
            },
            {
                "id": 2,
                "code": "CNY",
                "name": "人民币"
            },
            {
                "id": 3,
                "code": "USD",
                "name": "美元"
            },
            {
                "id": 4,
                "code": "EUR",
                "name": "欧元"
            },
            {
                "id": 5,
                "code": "JPY",
                "name": "日元"
            },
            {
                "id": 6,
                "code": "HKD",
                "name": "港币"
            },
            {
                "id": 7,
                "code": "GBP",
                "name": "英镑"
            },
            {
                "id": 8,
                "code": "CHF",
                "name": "瑞士法郎"
            },
            {
                "id": 9,
                "code": "AUD",
                "name": "澳元"
            },
            {
                "id": 10,
                "code": "NZD",
                "name": "新西兰元"
            },
            {
                "id": 11,
                "code": "SGD",
                "name": "新加坡币"
            },
            {
                "id": 12,
                "code": "CAD",
                "name": "加元"
            },
            {
                "id": 13,
                "code": "THB",
                "name": "泰铢"
            }
        ],
		"point_rule": [
            {
                "input_unit": "THB",
                "input_value": "5",
                "output_unit": "积分 ",
                "output_value": "2",
                "tag": "标准"
            },
            {
                "input_unit": "CNY",
                "input_value": "1",
                "output_unit": "积分",
                "output_value": "2",
                "tag": "标准"
            },
            {
                "description": "当申请分期付款时，在原有积分基础上，将再获额外 1 倍积分",
                "input_unit": "CNY",
                "input_value": "1",
                "output_value": "4",
                "tag": "多倍"
            }
        ],
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
    "status": "200",
    "msg": "success"
}


```

 **返回参数说明** 


|参数名|类型|说明|
|:----|:----- |-----   |
|id |string |唯一标示|
|name |string |名称   |
|level  |dict | 卡级别    |
|img_url |string | 图片地址    |
|currency  |list |货币 |
|card_org|list|卡组织|
|annual_fee|dict|年费|
|bank|dict|银行|
|card_benefit |list|非刷卡权益（指办卡就能有的权益）|
|act_ids|list|卡片能够参加的活动id列表|
|point_rule|list|积分规则 |
|interest_free_period | string | 免息期 |
|min_repayment_description | string | 最低还款额|
|hotlines| list | 信用卡热线|