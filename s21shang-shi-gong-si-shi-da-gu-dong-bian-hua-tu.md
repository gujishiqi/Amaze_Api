### 上市公司十大股东变化图

---

#### 接口描述

* 根据上市公司的股票代码获取上市公司十大股东变化数据

#### 请求URL

* /api/stock/chart

#### 请求方式

* GET

#### 请求参数

| 参数名 | 必填 | 数据类型 | 说明 |
| :--- | :--- | :--- | :--- |
| code | 是 | String | 股票代码 |

#### 返回数据示例

```
{
  "code": 100,
  "timeList": [
    "2017-02-06",
    "2017-03-31",
    "2017-07-28"
  ],
  "nodes": [
    {
      "id": 0,
      "name": "银亿房地产股份有限公司",
      "type": "企业"
    },
    {
      "id": 1,
      "name": "宁波银亿控股有限公司",
      "type": "企业"
    },
    {
      "id": 2,
      "name": "熊基凯",
      "type": "个人"
    },
    {
      "id": 3,
      "name": "西藏银亿投资管理有限公司",
      "type": "企业"
    },
    {
      "id": 4,
      "name": "鲁国华",
      "type": "个人"
    },
    {
      "id": 5,
      "name": "孔永林",
      "type": "个人"
    },
    {
      "id": 6,
      "name": "蒋伟平",
      "type": "个人"
    },
    {
      "id": 7,
      "name": "周株军",
      "type": "个人"
    },
    {
      "id": 8,
      "name": "姚佳洪",
      "type": "个人"
    },
    {
      "id": 9,
      "name": "华福证券-兴业银行-兴发稳增-银亿股份1号集合资产管理计划",
      "type": "企业"
    },
    {
      "id": 10,
      "name": "华宝信托有限责任公司-单一类资金信托R2007ZX111",
      "type": "企业"
    }
  ],
  "edges": [
    {
      "source": 1,
      "target": 0,
      "relation": "31.190"
    },
    {
      "source": 2,
      "target": 0,
      "relation": "24.520"
    },
    {
      "source": 3,
      "target": 0,
      "relation": "15.740"
    },
    {
      "source": 4,
      "target": 0,
      "relation": "3.830"
    },
    {
      "source": 5,
      "target": 0,
      "relation": "3.730"
    },
    {
      "source": 6,
      "target": 0,
      "relation": "3.240"
    },
    {
      "source": 7,
      "target": 0,
      "relation": "2.750"
    },
    {
      "source": 8,
      "target": 0,
      "relation": "1.770"
    },
    {
      "source": 9,
      "target": 0,
      "relation": "0.950"
    },
    {
      "source": 10,
      "target": 0,
      "relation": "0.410"
    }
  ]
}
```

#### 返回数据说明

| 参数名称 | 数据类型 | 说明 |
| --- | --- | --- |
| code | Long | 参照[全局返回代码](/数据词典.md) |
| timeList | Object | 时间节点集合 |
| nodes | Object | 节点 |
| edges | Object | 边 |

#### 备注

* 当请求参数`time`为空时，返回最近一个时间节点的投资关系图谱数据



