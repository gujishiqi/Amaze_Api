### 企业高管信息

---

#### 接口描述

* 根据企业的ID获取企业的工商注册信息

#### 请求URL

* /api/company/basic

#### 请求方式

* GET

#### 请求参数

| 参数名 | 必填 | 数据类型 | 说明 |
| :--- | :--- | :--- | :--- |
| id | 是 | String | 企业ID |

#### 返回数据示例

```
{
  "code": 100,
  "company": {
    "id": "59903e4b17322c8434661784",
    "name": "银亿房地产股份有限公司",
    "registry": "甘肃省工商行政管理局",
    "operatingStatus": "存续（在营、开业、在册）",
    "legalRepresentative": "熊续强",
    "registeredCapital": "305843.0395万元人民币",
    "establishmentDate": "1998-08-31",
    "unifiedSocialCreditCode": null,
    "businessScope": null,
    "address": null,
    "phone": null,
    "province": "甘肃省",
    "city": "兰州市",
    "county": "城关区",
    "code": "000981",
    "shortName": " 银亿股份 ",
    "time": "2000-06-22",
    "exchange": "深市主板",
    "number": "5000"
  }
}
```

#### 返回数据说明

| 参数名称 | 数据类型 | 说明 |
| --- | --- | --- |
| code | Long | 参照[全局返回代码](/数据词典.md) |
| company | Object | 参照[企业信息](/shu-ju-ci-dian/qi-ye-xin-xi.md) |

#### 备注

* 如果\`code\`股票代码字段不为空，则说明该公司为上市公司



