# Superstore_Analysis_Report
本项目对 Superstore 2015–2018 年销售数据进行了系统的数据分析，包括数据清洗、特征工程、品类分析、客户细分、区域表现、时间趋势、产品贡献度等维度，最终形成业务洞察与战略建议。


---

##  1. 项目背景

本项目基于 Superstore 的历史订单数据，从业务视角出发进行探索性数据分析（EDA），目标是：

- 了解 GMV 的主要驱动力  
- 找到高价值客户和高价值产品  
- 识别最重要的区域市场  
- 分析销售趋势与季节性  
- 为业务策略提供数据支持  

---

##  2. 数据清洗与预处理

主要步骤：

- 缺失值检查（Postal Code 存在 11 条缺失，不影响核心分析）
- 重复值检查（无重复订单记录）
- 日期字段转换为 datetime
- 新增 `YearMonth` 字段用于时间序列分析
- 分类字段（Category、Segment 等）格式化

最终数据质量良好，可以直接用于业务分析。

---

##  3. 分析结果（关键发现）

###  3.1 Category（品类）表现
- **Technology** GMV 最高（核心增长引擎）  
- Furniture 次之  
- Office Supplies 最低  

➡ 高客单价设备是业务核心驱动力。

---

### 3.2 Sub-Category（子类）表现

Top 5 GMV 子类：

1. Phones  
2. Chairs  
3. Storage  
4. Tables  
5. Binders  

Bottom 5 子类：

- Fasteners  
- Labels  
- Envelopes  
- Art  
- Supplies  

➡ GMV 贡献高度集中，库存策略可进一步优化。

---

### 3.3 Segment（客户类型）

- **Consumer：50.8%（主要 GMV 来源）**  
- Corporate 次之  
- Home Office 占比小  

➡ Consumer 营销要继续保持；企业客户更具扩展价值。

---

### 3.4 Region（区域表现）

- **West：约 710k（第一名）**  
- **East：约 670k（第二名）**  
- Central & South 较弱  

➡ West 与 East 需继续投入，South 是潜力区域。

---

###  3.5 时间趋势（GMV）

- 2015–2018 整体呈上升趋势  
- **Q4（10–12月）为旺季**  
- **Q1 为低谷**  
- 2018-12 创历史新高（≈120k）

➡ 典型季节性零售模式，备货需前置。

---

###  3.6 Top10 产品

GMV Top10 产品多数为：

- 高客单价打印设备  
- 远程会议设备  
- 办公家具  


第一名 GMV：

- **Canon imageCLASS 2200 Advanced Copier：≈61,600**

➡ 明星产品对总 GMV 贡献巨大，必须重点保障供应链。

---

##  4. 业务洞察与建议

- 加强 Technology 类的库存和供应链管理  
- 针对 Consumer 和企业客户做差异化营销  
- 强化 West/East 的广告预算投入  
- 扩展 South 区域渠道布局  
- Q3 提前备货以应对 Q4 旺季  
- 优先保障 Top10 产品供给，提高复购率  

---

## 🛠 5. 使用方法（运行项目）

### 克隆项目：
```bash
git clone https://github.com/tony1921/Superstore_Analysis_Report/blob/main/%E7%94%B5%E5%95%86%E9%A1%B9%E7%9B%AE%E5%88%86%E6%9E%90.ipynb
