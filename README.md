# 功能流程图

## aps 功能

> APS门户主页 [ https://fengnuanxiang.com/](https://fengnuanxiang.com/)   👈👈👈👈  
> APS操作平台 [ https://aps.fengnuanxiang.com/](https://aps.fengnuanxiang.com/)  👈👈👈👈  
> 如有疑问或需求,请联系  (微信: rpcjmeter ,备注: APS) (QQ: 2363745556)  👈👈👈👈  

### 使用范围

```
 商品制造复杂的工厂单位:    五金、注塑、涂装、机械、汽配、组装等行业，
```

### 功能介绍:

> 实现商品管理,工作日历,工作班次, 工段, 工位,状态, 车间, 工艺路径, 销售特征, 工程特征,零件, 预测生产, 订单, 排产, 排程, 零件等功能
>
>> 工作日历,工作班次: 可以设置工厂在一年内的工作时间, 并选择每天上班周期(工作时间影响预生产计划, 工作班次影
> > 响零件的使用量)
> > 工艺路径: 可以设置整条生产工艺路线, 设置每个车间到由N个工段, N个工位以及其耗时时间 (工位绑定零件可预测零件使用量)
> > 预测生产: 可以按销售特征比例及需要生产等数量, 生成每种销售特征需要生产等数量 (由总数到每种销售特征个数)
> > (预)生产计划: 可以把发布的预生成计划,按当前工作日历的配置时间,平均分配到某一周中( 由月度生产到天生产),并查询零件使用情况
> > 订单: 从创建订单到订单完成,以及发送大屏用户手中所有状态监控 (订单信息维护)
> > 排产:  按工厂产能, 配置限制, 订单基本信息等纬度判断订单应该在那一天上线生产(按计划预排每个订单的状态的大概日期)
> > 排程:  按车间排产顺序, 基于每个时间段的产能限制, 安排商品生产顺序 (定于每个商品的生产时间)
>>

|     模块      | 列表  | 增加  | 删除  | 修改  | 详情  | 其他       | 需求   |
|:-----------:|:---:|-----|-----|-----|-----|----------|:-----|
|    商品管理     |  ✅  | ✅   | ✅   | ✅   | ✅️  |          |      |
|    工段管理     |  ✅  | ✅   | ✅   | ✅   | ✅️  |          |      |
|    工位管理     |  ✅  | ✅   | ✅   | ✅   | ✅️  |          |      |
|    状态管理     |  ✅  | ✅   | ✅   | ✅   | ✅️  |          |      |
|    车间管理     |  ✅  | ✅   | ✅️  | ✅️  | ✅   |          |      |
|   工艺路径管理    | ✅️  | ✅️️ | ✅️️ | ✅️️ | ✅️️ |          |      |
|   销售特征管理    | ️ ✅ | ✅️  | ✅️  | ✅   | ✅️  |          |      |
|  商品销售特征绑定   | ✅️  | ✅️  | ✅️  | ✅️  | ✅️  |          |      |
|   工程特征组管理   |  ✅  | ✅️  | ✅️  | ✅️  | ✅️  |          |      |
|   销售转工程管理   |  ✅  | ✅️  | ❌️  | ✅   | ✅️  |          |      |
|    零件管理     | ✅️  | ✅️  | ✅️  | ✅️  | ✅️  |          |      |
|    预测管理     | ✅️  | ✅️  | ✅️  | ✅️  | ✅️  | 上传,发布    | 版本对比 |
|   预测管理主版本   | ✅️  | ✅️️ | ✅️️ | ✅️️ | ✅️  |          | 版本对比 |
|  (预)周生产计划   | ✅️  | ✅️️ | ✅️️ | ✅️️ | ✅️  | 发布, 零件使用 |      |
| (预)周生产计划主版本 | ✅️  | ✅️️ | ✅️️ | ✅️️ | ✅️  |          |      |
|    订单管理     | ✅️️ | ✅️️ | ❌️  | ❌️  | ❌️  |          | 报表   |
|   工厂产能管理    |  ✅  | ✅   | ❌️️ | ✅️️ | ✅️️ |          |      |
|   销售产能管理    |  ✅  | ✅️  | ❌️  | ✅️️ | ✅️️ |          |      |
|   商品产能管理    | ✅️️ | ✅️️ | ❌️  | ✅️️ | ✅️️ |          |      |
|    排产管理     | ✅️  | ✅️️ | ✅️️ | ✅️️ | ✅️️ | 零件使用量    |      |
|    滚动预测     | ⌛️  | ⌛️  | ⌛️  | ⌛️  | ⌛️  |          |      |
|    零件使用     | ⌛️  | ⌛️  | ⌛️  | ⌛️  | ⌛️  |          |      |

[流程图](./doc/md/aps.md)
[页面展示](doc%2Fmd%2Faps-page.md)

---

## 盘点

### 使用范围

```
     需要定时盘点固定资产等单位: 如固定盘点办公用品等,能贴就能盘点
```

### 功能介绍:

> 实现从工厂管理, 楼层管理, 房间管理, 资产管理, 资产盘点,盘点报表等功能
>
>> 资产盘点: 生成相应的资产二维码, 用户可以扫码该二维码进行资产盘点, 可以生成并下载盘点报表
>>

|  模块  | 列表 | 增加 | 删除 | 修改 | 详情 | 其他              | 需求      |
|:----:|:--:|----|----|----|----|-----------------|:--------|
| 楼层管理 | ✅  | ✅  | ✅  | ✅  | ✅  | 批量创建            |         |
| 房间管理 | ✅  | ✅  | ✅  | ✅  | ✅  | 批量创建            |         |
| 资产管理 | ✅  | ✅  | ✅  | ✅  | ✅  | 资产禁用,批量创建,生成二维码 | 增加资产使用人 |
| 盘点管理 | ✅  | ✅  | ✅  | ✅  | ✅  | 扫码盘点,下载         | 盘点快照    |

[流程图](./doc/md/propertyCheck.md)
[页面展示](./doc%2Fmd%2Fpro-page.md)
-----------------------------------------------------------------------

## 进存销

### 使用范围

```
    需要商品管理的单位: 如中小型超市, 需要了解从商品采购,录入,成本管理等行业
```

### 功能介绍:

> 实现商品录入, 订单管理, 商品盘点,采购计划单生成, 采购单生成等功能
>
>> 自动盘点: 可以每天设置商品盘点时间, 当不足商品预警数量时, 自动生产采购计划
> > 采购计划: 选择采购计划, 生成相应的采购单, 并发送供应商
>>

|  模块   | 列表 | 增加 | 删除 | 修改 | 详情 | 其他              | 需求             |
|:-----:|:--:|----|----|----|----|-----------------|:---------------|
| 商品管理  | ✅  | ✅  | ✅  | ✅  | ❌  | 生成条形码,库存预警,每日盘点 | 销售数据           |
| 订单管理  | ✅  | ✅  | ❌  | ❌  | ✅  |                 |                |
| 财务管理  | ⌛️ | ⌛️ | ⌛️ | ⌛️ | ⌛️ |                 | 收支统计,财务分析,财务报告 |
| 供应商管理 | ✅  | ✅  | ✅  | ✅  | ✅  |                 |                |
| 采购计划  | ✅  | ✅  | ✅  | ✅  | ✅  |                 |                |
| 采购订单  | ✅  | ✅  | ✅  | ❌  | ✅️ | 驳回,预览           |                |
| 入库管理  | ⌛️ | ⌛️ | ⌛️ | ⌛️ | ⌛️ |                 |                |

[流程图](./doc/md/jcx.md)
[页面展示](doc%2Fmd%2Fjcx-page.md)

---

# 各系统页面展示

[各系统页面展示](./doc/md/page-show.md)

# 系统功能概览

> 图示:
>
>> ❌: 不实现
> > ⌛️: 待实现功能
> > ✅: 已实现
>>

## 基础功能

|  模块  | 列表 | 增加 | 删除 | 修改 | 详情 | 其他          | 需求 |
|:----:|:--:|----|----|----|----|-------------|:---|
| 用户管理 | ✅  | ✅  | ✅  | ✅  | ✅  | 登录,登出       |    |
| 租户管理 | ✅  | ✅  | ✅  | ✅  | ✅  |             |    |
| 消息中心 | ✅  | ❌  | ❌  | ❌  | ✅  | 已读          |    |
| H3接口 | ❌  | ❌  | ❌  | ❌  | ❌  | H3 API接口已接入 |    |
| 工厂管理 | ✅  | ✅  | ✅  | ✅  | ✅  |             |    |
| 文件管理 | ✅  | ✅  | ✅  | ⌛️ | ✅  |             |    |
| 日历管理 | ✅  | ✅️ | ✅️ | ✅  | ✅️ |             |    |
| 排班管理 | ✅️ | ✅️ | ✅️ | ✅️ | ✅️ |             |    |

# 技术栈

## 后端

| 组建名称                 | 依赖版本         | 说明                 |
|----------------------|--------------|--------------------|
| JDK                  | jdk 17       | Jdk最低版本            |
| Spring Boot          | 3.2.0        | springboot版本       |
| mybatis-plus         | 3.5.3.1      | mybatisplus版本      |
| mybatis-plus-join    | 1.4.8.1      | mybatisplus-join版本 |
| ~~sqlite-jdbc~~      | ~~3.45.1.0~~ | ~~sqlite驱动版本~~     |
| mysql-connector-java | 8.0          | mysql驱动版本          |
| lombok               | 1.18.22 | lombok版本 |
| uber-h3              | 4.1.1 | 经纬度转code码 |
| hutool               | 5.8.0 | 常用工具库 |
| org.kie              | 7.14.0.Final | 规则引擎 |
| fastjson2            | 2.0.46 | json 插件 |
| ortools-java         | 9.9.3963 | 计算插件 |

# 数据库

| 组建名称        | 依赖版本     | 说明         | 备注         |
|-------------|----------|------------|------------|
| mysql       | 8.0      | mysql驱动版本  | 支持mysql版本  |

## 前端

| 组建名称           | 依赖版本    | 说明                  |
|----------------|---------|---------------------|
| ruoyi          | 3.8.6   | vue版本               |
| qrcodejs       | 1.0.0   | 条形码生成               |
| qrcodejs2      | 0.0.2   | 二维码生成,必须在https下才能使用 |
| @zxing/library | ^0.20.0 | 二维码扫描               |
