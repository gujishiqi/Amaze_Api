### 企业涉税信息数量列表

---

#### 接口描述

* 根据企业名称获取企业的各个涉税主题的涉税信息数量

#### 请求URL

* /api/company/eventsNum

#### 请求方式

* GET

#### 请求参数

| 参数名 | 必填 | 数据类型 | 说明 |
| :--- | :--- | :--- | :--- |
| name | 是 | String | 企业名称 |

#### 返回数据示例

```
{
  "code": 100,
  "eventsNum": [
    {
      "type": "投资收购",
      "themes": [
        {
          "name": "资产评估",
          "themeCode": "ZCPG",
          "num": 1
        },
        {
          "name": "股权转让",
          "themeCode": "GQZR",
          "num": 1
        }
      ]
    },
    {
      "type": "工程采购",
      "themes": [
        {
          "name": "政采采购",
          "themeCode": "ZFCG",
          "num": 12
        },
        {
          "name": "工程招标",
          "themeCode": "GCZB",
          "num": 1
        }
      ]
    }
  ]
}
```

#### 返回数据说明

| 参数名称 | 数据类型 | 说明 |
| --- | --- | --- |
| code | Long | 参照[全局返回代码](/数据词典.md) |
| eventsNum | Object | 企业涉税信息数量 |
| type | String | 涉税主题所属类别 |
| name | String | 涉税主题名称 |
| themeCode | String | 涉税主题代码 |
| num | Long | 涉税数据数量 |



