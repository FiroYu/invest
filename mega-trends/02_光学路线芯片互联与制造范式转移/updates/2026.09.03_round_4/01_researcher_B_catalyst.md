# 催化剂研究员（研究员B）独立研究报告

> 课题: #02 光学路线芯片互联与制造范式转移
> 分析日期: 2026-10-10 | 角色: catalyst（事件、管线、监管、预期修正）
> 捕获窗口: 2026-07-10 → 2026-10-10；搜索源: WebSearch（Reuters/FCC/公司公告/产业链媒体）
> 声明：本报告独立完成，未接触其他研究员

---

## 一、核心发现（Top 3）

1. **FCC 中国光模块禁令风波（8/4-10/9）是本轮最大单一事件：一只靴子落地、第二只悬空**。8/4 Reuters：FCC 起草禁令，拟禁止进口中国产新型号数据中心光收发模块（800G/1.6T 主力），点名中际旭创（全球市占 ~27%），目标年内实施——A股光模块板块剧烈震荡（观察者网/腾讯新闻回顾）。8/7 FCC 新规提案管控清单未含光模块。**9/10 FCC 公布最终规则（30 日后生效）：未提及光模块、未提及旭创新易盛，均不在 Covered List**（推特产业追踪 @tuolaji2024 9/10；观察者网 9/11 证实「市场最担心的一幕没有出现」）；但拟议部分把光模块列为**未来 BOM 物料清单披露候选组件**，保留「禁止一切组件」口子，评论期 9/8 刚过。10/9 Covered List 更新仅加无人机（UAS）。**SCMP 定性（9 月）：中国光模块厂商"dodge the ban for now"——暂时躲过。残留风险：65% 本地含量条款讨论（xxquant 转述：中国模块若 65% 零部件非中国或可继续进口）+ 10 月 FCC 可能再动作。**

2. **CPO 催化剂密度骤升：从"量产元年"进入"部署元年"**。①NVIDIA Spectrum-X Ethernet Photonics **full production**，4x 更少激光器+五厂商 CPO 供应链，命名首批客户 **CoreWeave/Lambda/Meta/Microsoft/Oracle**（StorageReview 7 月；edgewisely 汇总）；②NVIDIA 高级 VP Gilad Shainer 宣布为 **Vera Rubin 平台量产 CPO**（thebuildout 7 月）；③**Spectrum-6 102.4T** 交换机发布（7/21，biggo/官方）；④Broadcom Tomahawk 6 "Davisson"——业界首个 102.4T CPO 交换芯片（官方页面，量产推进中）；⑤**Lambda 部署全球首批 NVIDIA Quantum-X InfiniBand Photonics 交换机**：每机架省 3kW、等效释放 3,000+ GPU 额外容量（edgen.tech 8 月）；⑥TrendForce 7/27：NVIDIA 与 Broadcom CPO 交换机 **volume ramp 开始**，瓶颈=光引擎良率+先进封装产能；⑦TSMC COUPE 从开发转入量产（bits-chips/TrendForce 4 月，Semi 会议）。

3. **需求侧卖方预期发生 2026 年内第二次大幅上修——从"短缺"升级为"结构性短缺"**。Goldman 9/7（调研 15 家中国光电子公司后）：800G+ 2027 需求上调至 **144M 只**、全球出货 2026-28E +21/31/31%、1.6T+ +29/61/50%、TAM +33/81/115%；旭创目标价 2,645 元（隐含 225%）——当天旭创 A 股 +10.38%、市值破万亿、创业板 +3.41%（itiger/remio 9/7）。Jefferies：2027 光模块市场翻三倍、1.6T 供给短缺 ~30%（bit.fan 转述）。Nomura 专家会（xxquant 转述）：Google 主导 OCS 2027 需求 40-50k 台；**材料短缺可能约束 2026 1.6T 出货**。Cignal AI：1Q26 数据com 光器件营收 $7.7B（YoY 翻倍，纪录）。

---

## 二、催化剂日历（按时间排序）

| 日期 | 事件 | 影响标的 | 预期影响 | 定价程度 |
|------|------|---------|:---:|:---:|
| 已发生 7/21 | NVIDIA Spectrum-6 102.4T 发布 | NVDA/AVGO/TSM | 高 | 部分定价 |
| 已发生 7/27 | TrendForce CPO volume ramp 报告 | 全链 | 中 | 部分定价 |
| 已发生 8/4-9/10 | FCC 禁令风波（未落地+留口子） | 旭创/新易盛 | 极高 | 部分定价（尾部风险仍在） |
| 已发生 8/11-8/17 | LITE/COHR/FN 财报超预期 | LITE/COHR/FN | 高 | 部分定价 |
| 已发生 8/21-8/24 | 旭创/新易盛中报 | 300308/300502 | 高 | 已定价（当日兑现） |
| 已发生 9/7 | Goldman TAM 大幅上调 | 旭创为首 | 高 | 已定价（+10.38%） |
| 已发生 9/10 | FCC 最终规则未列光模块 | 中国链 | 高 | 已定价（反弹） |
| 已发生 10/8 | TSMC 9 月营收 +54.6%/Q3 纪录 | TSM | 中 | 部分定价 |
| **2026-10 下旬** | **四大+TSMC Q3 财报：2027 CapEx 首批半量化** | 全链 | **极高** | **未定价（T3 裁定点）** |
| **2026-11-27** | **中国镓/锗/锑出口管制到期/恢复** | 中国链/LITE | 高 | 未定价 |
| 2026-11 中 | NVIDIA Q3 FY27（$108B 兑现+Rubin 斜率） | 全链 | 高 | 部分定价 |
| 2026 Q4 | FCC BOM 披露规则落地形态 / 光模块是否入列 | 中国链 | 极高 | 未定价 |
| 2026 Q4-2027 H1 | 3.2T 标准化推进（2028 放量前置） | 旭创/LITE/COHR | 中 | 未定价 |
| 2027 H1 | Broadcom TH6-Davisson 规模出货 | AVGO/TSM | 中 | 未定价 |

---

## 三、关键催化剂 Top 3 及投资含义

1. **10 月底 Q3 财报季（T3 裁定点）**：四大 2027 CapEx 首批数字。>+25% → Bull 情景打开；+15-25% → Base 维持；<+15% → T3 触发整体减仓 40%。与 #01/#17 完全同源——**这是 #02 未来 3 周唯一必须盯的事件**。
2. **FCC BOM 披露规则 Q4 落地**：若光模块正式入列披露/限制 → 中国链估值再压 15-25%、Lumentum/Coherent/Fabrinet 受益（Counterpoint 8/4 已给出 win/lose 矩阵）；若维持不入列 → 中国链风险溢价消退。**二值事件，波动率定价不足。**
3. **NVIDIA Vera Rubin CPO 全量爬坡（Q4-2027H1）**：Rubin Q3 起占 NVDA DC 收入 ~20%（#17 R4），其 CPO 配套（Spectrum-X/Quantum-X Photonics）决定 2027 CPO 渗透率能否从 0-2% 爬到 3-5%——H2 直接验证项。

---

## 四、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|------|------|------|:---:|
| H1 光替代铜方向 | 成立（强化：部署证据） | Lambda 首部署 3kW/机架节省；五客户名单；Spectrum-6 102.4T；TH6-Davisson | 5 |
| H2 CPO 渗透节奏（2028 10%+） | 成立偏上修 | volume ramp 已启动；瓶颈=良率+封装产能（TrendForce 7/27）而非需求 | 4 |
| H3 光子计算商用 | 不成立 | Ayar 转向 CPO 量产叙事（3/3 新闻稿标题即为 co-packaged optics）；Lightmatter-GUC 走 CPO/Hyperscaler ASIC 路线（1/26） | 4 |
| H4 中国定价权 | 成立（经历压力测试） | FCC 最终规则未列（9/10）；Goldman 调研 15 家中国公司后上调（9/7）；旭创市占 27% 第一 | 4 |
| H5 CapEx 支撑 | 成立（等待 10 月底二验） | Q2 全上调；Goldman/Nomura 材料短缺判断；10 月底 Q3 为终验 | 4 |

---

## 五、情景分析（6-12 个月）

| 情景 | 概率 | 核心驱动 | 预期回报 |
|------|:---:|---------|:---:|
| Bull | 30% | Q3 CapEx 2027 >+25% + FCC 维持不入列 + Rubin CPO 爬坡超预期 | +40% |
| Base | 45% | CapEx 高位延续 + FCC 悬而未决 + CPO 渐进爬坡 | +15% |
| Bear | 25% | 2027 CapEx <+15% 或 FCC Q4 入列 / 11/27 出口管制恢复 | -28% |

---

## 六、时间维度

- **短期（1-3 月）**：10 月底 Q3 财报（T3）；11/27 出口管制；FCC Q4 动作。
- **中期（3-12 月）**：Rubin CPO 爬坡数据；TH6-Davisson 出货；3.2T 2028 前置信号；光引擎良率改善斜率。
- **长期（1-3 年）**：CPO 渗透 2028-2030 放量；OCS（Google 40-50k 台@2027）与 CPO/LPO 的形态竞争。

> 来源：Reuters（8/4 via 观察者网/The Verge/SDxCentral/Digitimes）、FCC.gov（10/8 Fact Sheet、10/9 Covered List）、观察者网（8/24、9/11）、SCMP（9 月）、StorageReview、TrendForce（7/27、4/1）、Broadcom/NVIDIA/Lambda 官方（7 月）、thebuildout（7 月）、biggo（7/21）、edgen.tech（8 月）、Goldman via gate/longbridge/xxquant（9/7-9）、Jefferies via bit.fan、Nomura via xxquant、Cignal AI（6 月）、Counterpoint（8/4）。
