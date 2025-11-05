# pep-27.github.io

# Pillar 2 大纲
---
# 

## 🎯 一、我们要解决的商业问题是什么（Pillar 2核心）

### **问题定义：**

> 当前的 Gies Sustainability Dashboard 只是在“展示数据”，还没有真正变成一个能驱动决策的“智能工具”。

也就是说：

* 现在的仪表板 **告诉你“有什么”**（多少篇论文、哪个SDG占比高）；
* 但不能 **告诉你“所以怎样”**（哪些领域最具投资价值、哪些教授该合作、哪些研究能吸引捐赠人）。

### **商业问题的本质：**

> 如何把分散的学术研究数据，转化为**能直接支撑战略、合作与投资决策的 actionable insights（可执行洞察）**。

### **三个关键痛点：**

1. **信息孤岛**
   研究分布在不同学院、不同主题下，缺少“横向连接”的智能分析（谁在做相似的事、哪些SDG被忽视）。

2. **缺少决策信号**
   领导层看不到投资回报或潜在增长点，无法做出资源再分配或战略聚焦。

3. **故事缺乏数据支撑**
   对外讲述（捐赠人、政府、企业）需要定量证据和影响故事，而仪表板目前只有静态计数。

---

## 🧭 二、为什么这样设计整个分析流程（Phase 1–7）

整个方案的核心思路是：**让数据从“描述性” → “诊断性” → “预测性” → “行动性”**。
也就是：

> 从 *What Happened* → *Why It Happened* → *What Will Happen* → *What Should We Do Now*。

---

### **Phase 1 — 建立指标语言（KPI 体系）**

**目的：**
把不同用户的决策需求（领导、教师、捐赠人）转化为可以计算的指标。

**为什么要先做：**
因为没有“共同指标语言”，数据分析就无从服务决策。
这一步让所有决策都能落到数值维度上，如：

> “我们要提升 SDG-7 的投资效率 20%” 就能变成一个可追踪指标。

---

### **Phase 2 — 数据建模（Insight Data Model）**

**目的：**
把原始研究数据（论文、专利、课程、项目等）重构成“能计算洞察的结构化表”。

**为什么这样做：**
仪表盘不是仓库，而是“推理引擎”。
每一个指标（Impact Score、White Space、Collab Bridge）都需要可复用的事实表与桥表。
这一阶段确保分析可以跨学院、跨SDG无缝进行。

---

### **Phase 3 — 洞察引擎（Insight Engines）**

**目的：**
把指标转化为**对不同角色有意义的决策结论**。

**为什么分三类：**

* 领导 → 要看到“强项/短板/ROI”；
* 教师 → 要找到“合作机会”；
* 捐赠人 → 要读到“影响故事”。

这三类洞察形成了“决策三角”：

> 战略投资 → 学术合作 → 外部讲述
> 共同强化 UIUC 的社会影响力。

---

### **Phase 4 — 预测与行动（Predictive & Next Best Action）**

**目的：**
让系统从被动报告变成主动推荐。

**为什么关键：**
管理者不想“看图表”，他们想知道“接下来要做什么”。
通过趋势预测 + 推荐卡片，就能回答：

> “未来 2 年哪个 SDG 领域最值得提前投资？”
> “哪个研究群正崛起，需要资金或协作支持？”

---

### **Phase 5 — 决策型 UX（Insight to Action）**

**目的：**
把复杂的数据转化为**一目了然、可点击的决策路径**。

**为什么必要：**
如果洞察难以找到或操作，决策者不会使用。
Insight Tile + Drill + Action Bar 的设计逻辑是：

> “看到→理解→点击→执行”。

---

### **Phase 6 — 治理与信任（Governance & Trust）**

**目的：**
建立可信的系统，使用户敢依赖分析结果。

**为什么必须有：**
LLM 分类有误差，用户必须能查逻辑、看置信度、打标反馈。
通过 Accuracy Check 页 + 抽检机制 + Flag 机制，实现“可审计透明”。

---

### **Phase 7 — 试点、度量与迭代**

**目的：**
验证可用性、量化价值、建立持续优化闭环。

**为什么最后做：**
任何智能仪表要成为真实决策工具，必须经历“试点验证 → 用户采纳 → 数据驱动改进”。
这一步让方案真正落地，而不是停留在“概念”。

---

## 🧩 三、总结逻辑链（一句话串起来）

> 我们的商业问题是：**仪表盘停留在展示层，无法转化为决策智能。**
>
> 我们的方案逻辑是：
> **定义决策 → 构建指标 → 建模数据 → 生成洞察 → 提供预测 → 设计UX → 建立信任 → 验证成效。**
>
> 最终让 Dashboard 成为 UIUC 的“数据大脑”，能告诉校方、教师、捐赠人——**下一步应该投在哪、合作谁、讲什么故事。**

---

# Phase 1 — 指标体系与KPI设计（Insight Taxonomy & KPI Design）

## 1) 从“决策问题”反推指标（Decision → Metric）

* **产出**：Decision–Metric 矩阵（决策问题 → 指标 → 数据源 → 口径/周期）。
* **怎么做**：

  1. 把三类受众的关键决策写成一句话问题（Leadership/Collaboration/Donor）。
  2. 每个问题列出“能直接支持该决策”的度量（Leading 与 Lagging 指标都要）。
  3. 给每个指标绑定数据源、刷新频率、维度（SDG/学院/系/时间）。
* **示例**：

  * 决策：未来24个月在 **SDG-7** 投哪几个团队最有效？
  * 指标：近8季产出增长率、近3年每$100万经费产出、合作网络中心性、转化成果（专利/政策/社区项目）等。
  * 数据源：Illinois Experts、Grants、Patents、Courses、Projects。

## 2) KPI 分层（Foundational → Diagnostic → Impact）

* **产出**：分层KPI清单（定义+计算公式+解释）。
* **怎么做**：

  * **基础（Foundational）**：量与覆盖

    * `pub_count`：期内SDG映射≥阈值的论文数。
      *SQL 核心*：`COUNT(DISTINCT pub_id)` with `sdg_conf >= 0.6`
    * `active_faculty`：期内至少有1项可计入产出的教师数。
    * `sdg_coverage`：覆盖到的SDG数/17。
  * **诊断（Diagnostic）**：结构与效率

    * `growth_4q`：滚动4季增长率 = `(curr_4q - prev_4q) / NULLIF(prev_4q,0)`
    * **集中度（HHI）**：衡量某学院在各SDG的“偏科”程度
      
      ![HHI Formula](https://raw.githubusercontent.com/pep-27/pep-27.github.io/main/HHI_Formula.png)
      
      *SQL 片段*：对各SDG占比求平方后汇总。
    * **经费产出效率**：`outputs_per_$ = outputs / (grant_$ / 1e6)`
  * **影响（Impact）**：转化与外溢

    * `patent_count`、`policy_citations`、`community_projects`、`student_outcomes`（RA/Capstone/就业/创办企业）。
* **注意点**：所有KPI注明**口径**（如是否去重、是否含共同作者）、**时间窗**（YTD/滚动4季/滚动12季）。

## 3) 标准化与可比性（Normalization）

* **产出**：标准化口径与字段（使不同学院/规模可比）。
* **怎么做**：

  * **人均**：`per_faculty = outputs / headcount_faculty_fte`
  * **经费标准化**：`per_$1m = outputs / (grant_$ / 1e6)`
  * **规模/历史基线**：`z_score = (value - mean_dept) / std_dept`
  * **时间标准化**：统一到滚动窗口（4Q / 8Q）。
* **注意点**：保留原值 + 标准化值两列，便于解读与审计。

## 4) 置信度与质量标签（Confidence & QA）

* **产出**：每条记录的置信度与审计字段。
* **怎么做**：

  * **SDG分类置信度**：`sdg_conf ∈ [0,1]`；至少三档：`High(≥0.8) / Med(0.6–0.8) / Low(<0.6)`。
  * **可见化**：任何聚合指标旁显示“加权样本量”和“低置信样本占比”。
  * **审计列**：`source`, `last_updated_at`, `method_version`, `reviewer_id`, `is_verified`.
* **计算示例（置信加权产出）**：
  [
  \text{weighted_pubs}=\sum_i \mathbb{1}(\text{pub}_i \text{映射到SDG})\cdot \min(1,\max(0,\text{sdg_conf}_i))
  ]

## 5) 复合影响指数（Composite Impact Score）

* **产出**：一个可解释、可调权重的综合分。
* **Baseline 公式（示例，可调权）**：
  [
  \text{Impact} = 0.35\cdot \widetilde{\text{Quality Pub}} + 0.25\cdot \widetilde{\text{Grants}} + 0.20\cdot \widetilde{\text{Translation}} + 0.10\cdot \widetilde{\text{Collab}} + 0.10\cdot \widetilde{\text{Teaching Link}}
  ]

  * `~` 表示**标准化**（如z-score或0–100分位）。
  * `Translation` 由（专利/政策/社区项目/企业合作）构成；`Collab` 来自图网络指标（度/介数/跨院边比例）；`Teaching Link` 来自课程与学生项目的挂钩度。
* **权重校准**：

  * **主观法**：AHP + 利益相关方打分矩阵；
  * **经验法**：用“成功事件”（如大型捐赠/国家级项目中标）做逻辑回归/排序学习，回推能最好解释事件发生的权重。

## 6) KPI 说明书（Spec Sheet）

* **产出**：每个KPI 1页说明（字段定义、单位、分母分子、时间窗、示例SQL、数据源、 caveats）。
* **示例SQL（HHI，院×SDG）**：

```sql
WITH sdg_counts AS (
  SELECT dept_id, sdg_id, COUNT(DISTINCT pub_id) AS n
  FROM fact_publication_sdg
  WHERE pub_year BETWEEN 2022 AND 2025 AND sdg_conf >= 0.6
  GROUP BY dept_id, sdg_id
),
dept_total AS (
  SELECT dept_id, SUM(n) AS total_n
  FROM sdg_counts GROUP BY dept_id
)
SELECT s.dept_id,
       SUM(POWER(CAST(s.n AS float)/NULLIF(d.total_n,0), 2)) AS hhi
FROM sdg_counts s
JOIN dept_total d ON s.dept_id = d.dept_id
GROUP BY s.dept_id;
```

---

# Phase 2 — 洞察用的数据建模（Data Modeling for Insights）

## 1) 主题域与实体边界（What tables do we need）

* **产出**：事实/维度/桥接清单。
* **事实（Facts）**：

  * `fact_publication`（论文条目，含期刊年、质量代理如被引/分区）
  * `fact_grant`（项目/金额/起止/资助方）
  * `fact_patent`（专利族/申请/授权）
  * `fact_policy`（政策/白皮书/引用）
  * `fact_course`（课程、作业/Capstone关联SDG）
  * `fact_project`（学生/社区项目、交付物、影响人群）
  * `fact_partner_event`（产学/社区合作活动、MoU）
* **维度（Dims）**：

  * `dim_faculty`（含SCD2跟踪在职/部门变动、邮箱、ORCID）
  * `dim_dept`、`dim_college`、`dim_org_partner`、`dim_sdg`、`dim_time`
* **桥表（Bridges）**：

  * `bridge_pub_sdg(pub_id, sdg_id, sdg_conf)`
  * `bridge_faculty_pub(faculty_id, pub_id, author_order)`
  * `bridge_faculty_sdg(faculty_id, sdg_id, sdg_strength)` （基于其全部产出聚合）
  * `edge_collab(faculty_id_a, faculty_id_b, edge_wt, edge_type)`（合著/共申/共授课）

## 2) 主键、缓慢变化维（SCD）、溯源（Provenance）

* **产出**：建模规范。
* **怎么做**：

  * 每个事实表用业务主键 + `src_system`, `src_id` 保障去重；
  * `dim_faculty` 用 **SCD2**（`valid_from`, `valid_to`, `is_current`）跟踪院系/职称变更，用于“当期在职验证”；
  * 全表统一的审计列：`source`, `ingested_at`, `method_version`, `hash_raw`.

## 3) 支撑洞察的物化视图/派生表（Materialized Views）

* **产出**：每个洞察的“即取即用”数据集。
* **示例**：

  * `mv_strength_gap_heatmap(dept_id, sdg_id, pub_z, grant_z, impact_z, hhi)`
  * `mv_efficiency(dept_id, sdg_id, outputs_per_$, outputs_per_faculty)`
  * `mv_collab_graph(faculty_id_a, faculty_id_b, wt, cross_dept_flag, betweenness)`
  * `mv_translation_rollup(dept_id, sdg_id, patent_cnt, policy_cite_cnt, community_benefit)`
  * `mv_teaching_link(sdg_id, course_cnt, capstone_cnt, student_reach_est)`
* **刷新**：按域定频（论文/周，项目/周，专利/月），带**增量**与**回填**策略。

## 4) 关键指标的实现样例

* **经费产出效率（per $1M）**：

```sql
WITH g AS (
  SELECT dept_id, sdg_id, SUM(grant_amount_usd) AS grant_usd
  FROM fact_grant
  WHERE start_date >= '2023-01-01'
  GROUP BY dept_id, sdg_id
),
o AS (
  SELECT dept_id, sdg_id, COUNT(DISTINCT pub_id) AS pubs
  FROM fact_publication_sdg
  WHERE pub_year >= 2023 AND sdg_conf >= 0.6
  GROUP BY dept_id, sdg_id
)
SELECT COALESCE(o.dept_id,g.dept_id) AS dept_id,
       COALESCE(o.sdg_id,g.sdg_id) AS sdg_id,
       CAST(o.pubs AS float) / NULLIF(g.grant_usd/1000000.0,0) AS outputs_per_1m
FROM o FULL JOIN g
  ON o.dept_id=g.dept_id AND o.sdg_id=g.sdg_id;
```

* **跨学院“桥接分”（Betweenness，先产边表，再离线计算）**：

  1. 生成 `edge_collab`（合著/共申为边，权重=次数或近3年加权）；
  2. 用图算法（如Brandes）离线计算介数中心性，写回 `mv_collab_graph_stats(faculty_id, betweenness, cross_college_ratio)`。

* **White-Space Finder（外部需求 × 校内供给）**：

  1. 取州/行业需求指标（如能源转型、公共卫生缺口）到 `fact_external_need(sdg_id, need_index, year)`；
  2. 计算 `gap = need_index_z - supply_index_z`，按学院/SDG排序输出候选投资方向。

## 5) 质量控制与回溯（QA & Explainability）

* **产出**：Accuracy Check 字段与视图。
* **怎么做**：

  * 任何聚合表中加入：`low_conf_share`（低置信样本占比）、`n_weighted`（置信加权样本量）；
  * 提供 `mv_explain_pub_sdg(pub_id, sdg_id, conf, top_terms, method_version)`，供Dashboard“为什么这样分”的解释展开；
  * 保留“用户纠错”回写表 `fact_user_feedback(object_id, issue_type, note, status, resolved_by, resolved_at)`，形成审计链。

## 6) 性能与分区（Performance）

* **产出**：大表的分区与索引策略。
* **怎么做**：

  * 事实表按 `pub_year`/`start_date` 分区；
  * 联接常用键（`dept_id`, `sdg_id`, `faculty_id`）建聚簇/覆盖索引；
  * 物化视图按月刷新并缓存分位数/标准化参数到 `mv_norm_params(entity, metric, window_start, window_end, mean, std, p50, p90)`。

---

## 可交付物小清单（Phase 1 & 2）

* **KPI 目录与说明书**（含公式/SQL/口径/刷新频率/ caveats）
* **标准化与置信策略**（阈值、权重、显示规则）
* **ER 图 + 表DDL草案**（事实/维度/桥表 + 审计/溯源列）
* **洞察用物化视图列表**（含依赖关系与刷新策略）
* **示例Notebook/SQL**（HHI、效率、桥接分、White-Space）


---

# **Phase 3 — Insight Engines（洞察引擎）**

## **1. Leadership Insights（领导层决策）**

**目标：** 让院长/系主任快速看出研究强项、投入回报、短板。

**分析步骤：**

1. **强项-短板分析（Strength-Gap Matrix）**

   * 指标：每 SDG 在学院中的 Impact Score z-score 与 大学平均差距。
   * 方法：
     [
     gap = z_{\text{dept, sdg}} - z_{\text{univ, sdg}}
     ]
     正值 = 优势；负值 = 待投资。
   * 可视化：二维热力图（SDG × 院系）。

2. **投入产出效率（Resource Efficiency）**

   * 指标：`outputs_per_$`, `impact_per_$`, `growth_per_$`。
   * 方法：回归 y = Impact Score ~ Grant Funding + Faculty Count。
   * 结果：残差 > 0 → 超预期表现。

3. **投资情景模拟（Investment Scenario）**

   * 思路：用 OLS 或 Elasticity 估算 “资金增加 x% → 产出变化 y%”。
   * 计算：
     [
     \text{Elasticity}=\frac{\Delta\text{Impact}/\text{Impact}}{\Delta\text{Funding}/\text{Funding}}
     ]
   * 输出：若 Elasticity > 1 → 投资回报高。

---

## **2. Collaboration Insights（跨学科合作）**

**目标：** 识别潜在合作团队与跨院连接者。

**分析步骤：**

1. **协作网络构建**

   * 节点：faculty；边：共著、共申、共授课。
   * 边权：近 3 年合作次数 × 论文置信度权重。
   * 工具：NetworkX 或 Neo4j 图算法。

2. **指标计算**

   * 度中心性（Degree） → 活跃度。
   * 介数中心性（Betweenness） → 桥梁角色。
   * 社区发现（Louvain） → 自然研究群。

3. **潜在团队推荐**

   * 规则：主题相似度 > 0.7 且 曾无合作 → 推荐。
   * 主题相似度：TF-IDF or embedding cosine similarity。

4. **可视化**

   * 网络图：节点颜色 = 学院；连线粗细 = 合作强度。
   * 可交互过滤：按 SDG、学院、主题词 筛选。

---

## **3. External Storytelling & Accountability（外部展示）**

**目标：** 把冷数据变成“可讲的影响故事”。

**分析步骤：**

1. **故事模板化**

   * 模板：Problem → Research → Partnership → Impact → Metrics。
2. **数据填充**

   * 用 LLM summary 或 rule-based 模板生成短文，自动从 Impact Score 最高的 faculty 抽取内容。
3. **可视化**

   * 时间轴 (Timeline)：展示项目历程。
   * 地图 (Map)：显示合作城市/国家。
4. **质量指标**

   * 每个故事附：SDG、受益人数、就业创造、政策被采纳次数。

---

## **4. Insight Prototype 交付**

**产出文件：**

* SQL / Python Notebook：计算 Strength-Gap、Elasticity、Network Metrics。
* 图表：热力图、气泡图、网络图。
* 短故事文案示例（Markdown 格式）。

---

# **Phase 4 — Predictive & Next-Best-Action（预测与行动建议）**

## **1. 趋势预测（Trend Forecasting）**

**目标：** 预测未来 12–24 个月各 SDG 方向的研究趋势。

**分析步骤：**

1. **时间序列建模**

   * 数据：`pub_count_sdg_month` 或 `impact_score_sdg_month`。
   * 模型：ARIMA / Prophet / Exponential Smoothing。
   * 评估：MAPE、RMSE。
2. **输出**

   * 未来 6 季预测曲线。
   * 标出上升 (top 3 SDGs) 与下降趋势 (bottom 3 SDGs)。

---

## **2. 早期信号检测（Early-Signal Detection）**

**目标：** 识别潜在新兴研究热点。

**分析步骤：**

1. **主题提取**

   * 对论文摘要 embedding → 聚类（UMAP + HDBSCAN）。
2. **时间窗比较**

   * 最近 12 个月 vs 前 12 个月的主题频次差 Δfreq。
3. **热点判定**

   * 若 Δfreq > 阈值且覆盖院系 > 2 → 定义为 Emerging Topic。
4. **可视化**

   * 气泡图（横轴 时间、纵轴 增长率、气泡 主题）。

---

## **3. Next-Best-Action 推荐卡片**

**目标：** 把预测结果转化为可操作的建议。

**分析步骤：**

1. **逻辑规则**

   * Leadership 卡片：
     “在 SDG-7 能源方向投资 +$1M → 预计 Impact ↑ 15% 。”
   * Faculty 卡片：
     “您与 Prof. X 在可再生能源共现 4 次关键词，相似度 0.82，可合作。”
   * Donor 卡片：
     “您的基金主题与 3 个正在扩张的 SDG-4 项目匹配 > 90%。”
2. **生成机制**

   * 基于预测模型 + 业务规则（if/then 逻辑） + 模板。
3. **可视化**

   * Dashboard 小卡片（含 行动按钮：Share / Export / Flag / Contact）。

---

## **4. 模型监控与解释**

* **指标：** 预测 RMSE 、趋势一致率、推荐点击率。
* **解释：** 每条预测附带“Top 3 驱动特征”。
* **校准：** 季度更新模型参数与特征权重。

---

## **5. 产出交付**

* **Notebook：** ARIMA/Prophet 预测、热点检测、推荐逻辑。
* **Dashboard 原型：** 预测曲线 + Next-Best-Action 卡片。
* **指标文档：** 说明每个预测模型的输入/输出、评估方式。


---

# Phase 5 — 决策型 UX 与可操作界面

## 5.1 Insight Tiles（首页“要点卡片”）

* **做什么**：在首页展示“本月最重要的3条洞察”，可一键下钻。
* **怎么做**

  1. 排序规则：`priority = impact_gain * novelty * confidence`

     * `impact_gain`：按 KPI 提升潜力（如白区差距缩小幅度）
     * `novelty`：近30天是否首次出现/显著变化
     * `confidence`：基于样本量与置信度
  2. Tile 信息：标题、关键数字、置信度、时间窗、行动按钮（Share/Export/Drill/Flag）
* **产出**：`mv_insight_tiles`

  * 字段示例：`tile_id, title, metric_name, value, delta, window, confidence, priority, drill_link, created_at`

## 5.2 Drill-Down（下钻到“解释 + 数据”）

* **做什么**：从Tile进入可解释页面（“为什么这么判断”）。
* **怎么做**

  * 展示：计算公式、数据来源、样本量、低置信比、影响因素Top 3
  * 提供：下载CSV、复制引用（供报告/PPT）
* **产出**：可视化/明细接口

  * `GET /insights/{tile_id}/explain` 返回：`formula_md, sources[], n_weighted, low_conf_share, top_drivers[]`

## 5.3 Action Bar（行动栏）

* **做什么**：让洞察**变成决策动作**。
* **怎么做**

  * 按钮：`Save to Brief`（加入简报）、`Export`（PNG/PDF/CSV）、`Share`（生成带参数链接）、`Flag`（纠错/反馈）、`Contact`（拉起联系人）
* **产出**：交互事件日志表

  * `fact_user_actions(user_id, tile_id, action_type, ts)`

## 5.4 Personas → User Journeys（两类典型路径）

* **学生（可持续金融导师检索）**

  * 起点：首页搜索框 → 过滤 `SDG=8, 17`，`Topic=ESG, climate risk` → Faculty卡片 → 查看课程/RA/Capstone → 一键“联系/预约办公室时间”
  * 必备过滤器：`SDG`、`主题关键词`、`学院/系`、`是否在招RA`、`课程学期`
* **捐赠人（可再生能源资助）**

  * 起点：`Impact Stories` → 选择 `SDG-7` → 查看“团队/项目/落地成果” → 一键“匹配基金主题” → 生成一页提案PDF
* **产出**：两张旅程图（触点/页面/CTA/成功指标）

## 5.5 组件库与信息架构（IA）

* **做什么**：统一组件和导航，减少“找不到”的认知负担。
* **怎么做**

  * 导航：`Home` | `Explore SDG` | `People & Teams` | `Stories` | `Accuracy Check`
  * 组件：Tile、热力图、网络图、地图、表格、解释抽屉、反馈表单
* **产出**：低保真线框/组件规格（Figma或等效图）

## 5.6 可访问性与文案（A11y & Microcopy）

* **做什么**：保证读者易懂、可读、可用。
* **怎么做**

  * 色盲友好调色；图表≥12pt；为图表添加Alt文本
  * 微文案模板（示例）：

    * Tile 标题：「**在SDG-7的跨院合作增长 18%（最近12个月）**」
    * 解释提示：「基于 243 篇样本，低置信占比 6%。方法版本 v1.3。」

## 5.7 仪表的可发现性（导流/外链）

* **做什么**：把用户从学院网站、课程页、新闻页导到Dashboard。
* **怎么做**

  * 在相关页面嵌入“预览卡片”组件（最小化的三数据点 + “在仪表查看”按钮）
  * 生成可嵌入 `iframe`/`img + deeplink`
* **产出**：`/oembed` 接口与预览卡片规范

---

# Phase 6 — 治理与可信度（Governance & Trust）

## 6.1 指标与方法学透明（Method Cards）

* **做什么**：公开每个KPI/模型的“说明卡”。
* **怎么做**

  * 字段：`metric_name, definition, formula_md, data_sources[], update_cadence, caveats, owner, method_version`
* **产出**：`dim_metric_methodology`（供“Accuracy Check”页展示）

## 6.2 数据质量与抽检（QA Program）

* **做什么**：建立固定节奏的抽检与复核。
* **怎么做**

  * 季度抽检：随机抽样 `N` 条 SDG 映射结果，由领域教师复核
  * 计算：**一致性（inter-rater reliability）**：Cohen’s κ / Krippendorff’s α
  * 阈值与处置：低于阈值→回溯样本→调整阈值或模型版本
* **产出**：`fact_audit_samples(audit_id, object_type, object_id, sampled_at, reviewer_id, label, conf, final_decision)`

  * 及 `mv_audit_scores(metric, period, kappa, sample_n)`

## 6.3 反馈闭环（Flag→Triage→Resolve→Log）

* **做什么**：用户纠错的完整链路与看板。
* **怎么做**

  1. 用户点击 **Flag this Insight** → 记录问题类型
  2. Triage 分流（数据问题/方法问题/文本问题）与优先级
  3. 处理人领取、修正、回填说明、通知用户
* **产出**：三张表

  * `fact_user_feedback(feedback_id, user_id, object_type, object_id, issue_type, note, created_at, status, priority)`
  * `dim_issue_type(issue_type, description, sla_days)`
  * `fact_feedback_activity(feedback_id, actor_id, action, ts, comment)`

## 6.4 变更管理与版本控制（Change Log）

* **做什么**：记录任何影响指标的变更，保证可追溯。
* **怎么做**

  * 模型/权重/阈值/算法升级 → 在 `dim_change_log` 登记
  * 每条洞察关联 `method_version` 与 `norm_params_id`
* **产出**：

  * `dim_change_log(change_id, change_type, description_md, owner, effective_from)`
  * `mv_release_notes(period, changes[], impact_scope[])`（供“更新说明”页）

## 6.5 角色与权限（R&R）

* **做什么**：清晰化谁能改什么。
* **怎么做**

  * 角色：`viewer`（查看）、`editor`（改文案/标注）、`owner`（改方法/阈值）、`admin`（全权）
  * 审批：方法学和权重改动需 `owner + admin` 双签
* **产出**：权限映射表

  * `dim_role(role, desc)`、`map_user_role(user_id, role)`、`policy_matrix(action, min_role)`

## 6.6 “Accuracy Check” 专页（用户可信度入口）

* **做什么**：集中展示**置信度、样本量、抽检结果、版本与变更**。
* **怎么做**

  * 卡片：`本期置信度分布`、`抽检一致性 κ`、`低置信占比 Top5 维度`、`最新变更`
  * 支持下载：方法学卡片PDF、抽检报告CSV
* **产出**：仪表子页线框 + 接口

  * `GET /accuracy/summary`、`GET /accuracy/reviews`, `GET /methods/{metric}`

## 6.7 日志与可追溯 SQL 样例

* **样例：抽检一致性（月度）**

```sql
SELECT month, metric_name,
       AVG(kappa) AS avg_kappa, SUM(sample_n) AS total_samples
FROM mv_audit_scores
WHERE month BETWEEN '2025-06-01' AND '2025-11-01'
GROUP BY month, metric_name
ORDER BY month;
```

* **样例：被标记问题的SLA达成率**

```sql
SELECT DATE_TRUNC('month', created_at) AS month,
       SUM(CASE WHEN resolved_at IS NOT NULL 
                 AND resolved_at <= created_at + (sla_days || ' days')::interval THEN 1 ELSE 0 END
          )::float / COUNT(*) AS sla_on_time_rate
FROM fact_user_feedback f
JOIN dim_issue_type t ON f.issue_type = t.issue_type
GROUP BY 1
ORDER BY 1;
```

## 6.8 成功度量（Governance KPIs）

* **最低达标线**：

  * `κ ≥ 0.70`（抽检一致性）
  * `SLA 达成率 ≥ 90%`（反馈按期解决）
  * `低置信占比 ≤ 10%`（核心看板）
  * `方法变更公告覆盖率 = 100%`

---

## 交付清单（Phase 5 & 6）

* 首页 Tiles 与 Drill 线框（含文案模板与阈值逻辑）
* `Accuracy Check` 子页线框与接口契约
* 三类数据表 DDL：`fact_user_actions`、`fact_user_feedback`、`dim_metric_methodology`
* QA 抽检流程与SOP（角色、频次、κ计算方式）
* 变更管理与发布说明模板（含影响评估）


---

# **Phase 7 — 上线、测量与迭代**

## **7.1 试点范围 (Pilot Scope & Setup)**

**目标：** 在有限范围验证指标、可视化与反馈机制。
**步骤：**

1. **选择对象**

   * 2 个 SDG 主题（建议 SDG-7 Clean Energy 与 SDG-3 Good Health）。
   * 2 个 学院（如 Gies + Grainger）。
2. **部署环境**

   * 上线 Beta 仪表站点（含 Dashboard、Accuracy Check 页）。
   * 建立 每日自动刷新 + 备份。
3. **目标定义**

   * 首月活跃 ≥ 30 名 用户（含 领导、教师、学生、捐赠人代表）。
   * 生成 ≥ 10 条 可验证洞察 与 5 条 反馈。

**产出：** 试点计划表 (主题、用户、指标、时程、负责人)。

---

## **7.2 采集使用与成效数据 (Adoption & Engagement Tracking)**

**目标：** 量化工具使用与真实决策支持。
**关键指标：**

| 类别         | 示例                                             | 获取方式                   |
| ---------- | ---------------------------------------------- | ---------------------- |
| Usage      | `daily_active_users`, `session_duration`       | 日志 `fact_user_actions` |
| Engagement | `tile_click_rate`, `share_count`, `drill_rate` | 前端事件                   |
| Feedback   | `feedback_n`, `sla_on_time_rate`               | 反馈表                    |
| Impact     | “报告被引用/决策采用” 数                                 | 人工登记                   |
| Quality    | `low_conf_share`, `κ score`                    | Accuracy Check 页       |

**分析：**

```sql
SELECT DATE_TRUNC('week', ts) AS week,
  COUNT(DISTINCT user_id) AS wau,
  AVG(session_duration) AS avg_min,
  SUM(CASE WHEN action_type='share' THEN 1 END) AS shares
FROM fact_user_actions
GROUP BY 1;
```

---

## **7.3 季度回顾 (Quarterly Review Cycle)**

**目标：** 用数据驱动优化。
**步骤：**

1. 召开 Review Meeting (领导+开发+分析团队)。
2. 展示：

   * 用户增长曲线与留存率；
   * Top 5 最常用洞察 & Top 5 被忽视模块；
   * 反馈关闭率 & 低置信度分布。
3. 识别：**无效指标** (长期低点击、低相关) → 退役；**高价值指标** → 推广。
4. 记录行动项 (改进、重权重、增加新数据源)。

**产出：** 季度复盘报告（含 KPI 表、改进 backlog）。

---

## **7.4 权重与模型更新 (Model Re-Calibration)**

**目标：** 维持模型代表现实。
**做法：**

1. 重新训练 Impact Score 权重（用最近 12 个月事件 = 成功资助/高引用 作为标签）。
2. 更新 预测模型（Prophet/Elastic Net）并验证 RMSE 下降≥10%。
3. 通过 变更管理系统 登记 `method_version` + 发布说明。

**产出：** `mv_model_eval(period, metric, rmse, r2, change_from_prev)` + release note。

---

## **7.5 规模化扩展 (Scale-Up Plan)**

**目标：** 从试点扩展到全 UIUC 甚至其他高校。
**步骤：**

1. 通用化数据管道（参数化学院、SDG 维度）。
2. 文档化 ETL 与 API 接口。
3. 制定跨院部署时间线（Quarter 1–4）。
4. 设立 “Campus Data Steward Network” 负责维护质量。

**产出：** 扩展路线图 + 资源预算表 (人力、服务器、维护经费)。

---

## **7.6 沟通与推广 (Communication & Visibility)**

**目标：** 让成果被看到、被使用。
**行动：**

* 制作 1 页 Dashboard 海报 + 视频演示。
* 在 Gies / UIUC 官方渠道发新闻稿。
* 邀请教师学生投稿“如何用 Dashboard 指导决策”的短文。
* 定期邮件 Newsletter 展示最新洞察。

**产出：** 推广日历 + 模板文案。

---

## **7.7 持续改进循环 (Continuous Improvement Loop)**

**逻辑：**

```
[Data → Insights → Actions → Feedback → Review → Model Update]
```

**执行：**

* 设 月度 Sync ：检查反馈闭环、指标健康。
* 设 季度 Review ：更新权重、调整阈值、发布版本。
* 设 年度 Audit ：全局抽检 κ + SLA 合规。

**核心目标：**

* 保持 ≥ 85% 用户满意度；
* 季度发布 ≥ 1 次 新洞察功能；
* 实现 “数据→决策→社会影响” 闭环。

---

### **Phase 7 交付清单**

* 试点方案文档 + 仪表部署清单
* 使用分析 Dashboard 与 SQL 脚本
* 季度回顾模板 + 改进 backlog 表
* 权重更新 Notebook + release note
* 推广计划与 Newsletter 模板

---

