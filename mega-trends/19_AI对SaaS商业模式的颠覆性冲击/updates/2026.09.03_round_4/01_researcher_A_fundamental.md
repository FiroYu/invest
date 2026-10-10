# 基本面研究员 A 独立研究报告

> 课题: #19 AI 对 SaaS 商业模式的颠覆性冲击
> 分析日期: 2026-10-10 | 角色: fundamental | 增量窗口: 2026-07-10 → 2026-10-10

---

## 一、核心发现（Top 3）

1. **席位制的死亡有了第一份公司级实证：Salesforce 从"每席位"整体迁移到"按结果计费"。** FY26 代理书确认 Agentforce ARR $800M（+169%），09 月第三方口径达 **~$1.5B**；Q2 FY27（08.26）收入 +11%、cRPO 增速回升至 +14% CC、上调 FY27 指引 $200M。更重要的是定价结构：**Flex Credits + $2/resolved case（人工介入不计费）**——SaaStr 现场案例"10 个人类席位+2 人+1 API 席位、年账单 -80%"被官方口径验证。Salesforce 不是在"加 AI 溢价"，而是在**主动拆毁自己的席位定价塔**——这是 H1（定价支柱颠覆）从叙事变财务事实的标志（Salesforce IR/代理书 2026.08.26；Yahoo Finance/Zacks 2026.09.09；koda 2026.09.17）。

2. **受益层/承压层的财务分化在 Q2-Q3 财报季全面显形：** 受益层——PLTR Q1 +85%/Q2 +93%、美商业 Q1 +133%，市值破 $300B；ORCL FY27Q1 云 infra +121%、backlog $664B；SNOW 产品收入 +37%（加速）；Databricks $7B 年化 +80%；WDAY agentic ARR ~$500M、新 ACV +200%。承压层——SAP 云 +24% 但 **AI Agent 部署仅 17/200 客户**（滞后于叙事）、且为 AI 收购下修利润指引；WDAY 收入 +12.8% 但 backlog miss 股价下跌；HUBS 管理层承认客户"先试用再承诺"。**分化不是"AI vs 非 AI"，是"数据上下文/infra vs 工作流应用"**——深集成平台韧性（R3 判断）首次获得季度级财务验证（各公司 IR 2026.06-09；druckfin 2026.09；metirai 2026）。

3. **AI-native 颠覆者已从"案例"变成"品类"：80+ 家 AI-native 公司 $100M+ ARR（Sapphire 2026 报告），头部进入 $300M-4B 区间。** Glean $300M ARR（一年三倍）、Harvey $11B 估值、Sierra agents-as-a-service、Intercom Fin $0.99/工单八位数 ARR（+393% 年化）；**Cursor $4B ARR 被 SpaceX $60B 全股票收购**——AI 编程工具把"中端企业自建"的 R3 假设推到极致（连 IDE 都成为资产级收购标的）。Sapphire：$100M ARR 俱乐部从"世代成就"变为"80+ 常态"。**每一类传统 SaaS 品类（CRM/HR/客服/法务/BI）都出现了对应的 AI-native 替代者且都过了 $100M 门槛**——替代不再需要"会不会发生"的讨论，只剩"以什么速度"（SaaStr/Sapphire 2026; themeridiem 2026.05.29; agentmarketcap 2026.04; clinkbill/Sacra 2026.06-09）。

---

## 二、详细分析

### 2.1 R3→R4 假设对账表

| R3 判断 | R4 实况 | 裁定 |
|---------|---------|------|
| AI 不是简单利润杀手，是价值迁移 | $2T 蒸发+受益/承压分化财务验证 | **成立且加速** |
| 浅层承压、深集成韧性 | SAP agent 17/200 滞后 vs ORCL/SNOW/PLTR 加速 | 成立（分界线=数据上下文） |
| Agentforce 成熟度不足 | $1.5B ARR + outcome 定价落地 | **修正：成熟度超 R3 预期** |
| 数据治理瓶颈=incumbents 护城河 | 部分成立（WDAY 4000 客户 agent 翻倍） | 部分成立 |
| usage-based 转型承压毛利 | Databricks margin 因 agent swarm 收缩 | 成立 |

### 2.2 定价革命的三级火箭（席位→hybrid→outcome）

- **第一级（已完成）**：纯 per-seat 交易占比崩至 8%；AI 公司席位定价 21%→15%（12 个月）；hybrid 27%→41%。
- **第二级（进行中）**：NOW 04.09 三层 AI-native 改版把 AI **强制打包**（"不可拒绝"），旧 SKU 07.01 停售——这是"席位通胀"的最后晚餐： incumbents 用打包提价对冲未来席位流失。
- **第三级（开启）**：outcome 定价——Salesforce $2/resolved case、Intercom $0.99/ticket、Sierra agents-as-a-service。**定价单位从"人"变成"完成的工作"**，这是 H1 的最终形态。
- 净效应：hybrid（base+用量）是过渡赢家，纯 outcome 是终局。**"10 个人类席位→2 人+1 API 席位"案例说明单位经济从席位数 × ARPU 变成工作量 × 单价**——TAM 重算而非 ARPU 上调。

### 2.3 巨头 AI 贡献的真实含金量

| 公司 | AI 口径 | 含金量评估 |
|------|---------|-----------|
| MSFT | M365 Copilot >30M 付费席位（~$4.7B 年化） | 真实但增速依赖捆绑；席位仍在净增（H4 反证之一） |
| CRM | Agentforce $1.5B ARR、outcome 计费 | 真实增长但基数仅 ~3% 总收入；核心云 +11% 仍个位数 |
| ORCL | 云 +121%、$664B backlog | infra 层最强，但 FCF 负值——AI 需求≠AI 利润 |
| SAP | 云 +24%、agent 17/200 | **叙事超前于部署**；AI 收购压利润 |
| NOW | 三层打包提价 | 收入效应待 2027 续约周期验证 |
| WDAY | agentic ARR ~$500M、ACV +200% | 增速真实但 backlog miss 说明转化率存疑 |

### 2.4 H4 席位通胀的净效应（关键分歧点）

- **反方证据**：微软 Copilot 席位净增（>30M）、NOW 打包=变相席位通胀、WDAY 4000 客户 agent 采用翻倍
- **正方证据**：Salesforce 案例 -80% 账单、Gartner $234B agentic arbitrage、pure per-seat 8%
- **A 的裁定**：席位**数量**仍在膨胀（ incumbents 捆绑），但席位**定价权**已开始通缩（outcome 定价把锚从 $100/席/月拉到 $2/任务）。净效应在 2027 续约周期才见分晓——**NOW 三层改版（旧 SKU 07.01 停售）是第一个大规模自然实验**，R5 必查续约率与净留存（NRR）。

### 2.5 估值重估的结构拆解

- 3.3x EV/Rev（03.31）vs 2024 底 6.2x：一半归因利率（10Y 从 ~4.2%→5.3%），一半归因 AI 颠覆溢价消失。**即使降息，倍数也回不到 6x**——3.3-4.5x 是新均衡带（结构性折价）。
- 受益层定价已不便宜：PLTR ~120-140x P/E、Databricks $190B（~27x ARR）、Cursor $60B（15x ARR）——**颠覆者比被颠覆者贵**，多头表达要用期权/事件结构而非追高。

---

## 三、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|------|------|------|:-----------:|
| H1 席位制三支柱颠覆 | **成立（定价支柱已实证）** | $2/任务定价落地；pure per-seat 8%；$234B Gartner 口径 | 5 |
| H2 价值迁移至数据上下文/infra | **成立（加速）** | ORCL +121%/SNOW +37%/PLTR +93% vs SAP agent 17/200 | 5 |
| H3 浅层先死/深集成先活 | **成立（修正分界线）** | 分界线=数据上下文而非集成深度（SAP 深集成仍滞后） | 4 |
| H4 席位通胀逆转 | **待验证（2027 续约周期）** | NOW 三层改版=自然实验；Copilot 席位仍增 vs Salesforce -80% 案例 | 3 |
| H5 3.3x=结构性新均衡 | **成立** | 利率归因约一半；倍数-利率相关性破坏 | 4 |

---

## 四、情景分析（12 个月，议题多空组合口径）

| 情景 | 概率 | 核心驱动 | 预期回报 |
|------|:----:|---------|:-------:|
| Bull | 30% | NOW 续约周期验证 outcome 定价成功+AI-native 继续翻倍+空头篮子（SAP/协作类）继续 -20% | +20% |
| Base | 45% | 分化延续：受益层 +15%/承压层 -10%，对冲后 +8% | +8% |
| Bear | 18% | 推理成本骤降救活 SaaS 毛利+ incumbents 打包防御成功+AI-native 增速失速 | -12% |
| 黑天鹅 | 7% | AI 泡沫整体破裂（#17 CapEx 证伪传导）| -30% |

---

## 五、时间维度

- **短期(1-3月)**：Q3 财报季（CRM 12 月初/NOW 10 月底/MSFT 10 月底）、NOW 续约率首批数据、Gartner 口径修正
- **中期(3-12月)**：2027 续约周期（NOW/CRM 大规模 outcome 计费迁移）、AI-native IPO 窗口（Harvey/Sierra?）、PLTR 倍数压力测试
- **长期(1-3年)**：outcome 定价成为默认（>50% 新合同）、$234B agentic arbitrage 兑现度、SaaS 行业整合潮（被 AI-native 低价收购）

---

## 六、数据来源

| # | 数据点 | 来源 | 时间 | 可靠性 |
|---|--------|------|------|:------:|
| 1 | SaaSpocalypse 02.03 单日 -13%/$2T | ai2.work/buildmvpfast/jabbfusion | 2026.02-09 | 高 |
| 2 | EV/Rev 3.3x（03.31）/私募 3.5x | Windsor Drake/quantpillar | 2026.03-07 | 高 |
| 3 | Gartner $234B agentic arbitrage | Gartner（beri/foundersreport 转引） | 2026.07 | 高 |
| 4 | 席位 21%→15%/hybrid 41% | valueaddvc/agentmarketcap | 2026.04 | 中高 |
| 5 | Agentforce $800M→$1.5B/Flex Credits | Salesforce 代理书+IR/Zacks | 2026.08-09 | 高 |
| 6 | Salesforce $2/resolved case/-80% 案例 | koda（SaaStr 现场） | 2026.09.17 | 中（单一案例） |
| 7 | NOW 三层 AI-native 04.09 改版 | Crossfuze/redress/digino | 2026.04-07 | 高 |
| 8 | SAP 云 +24%/agent 17/200/利润下修 | SAP IR/Reuters/ad-hoc-news | 2026.07-09 | 高 |
| 9 | MSFT Copilot 30M 席位/Azure $100B | Microsoft Source | 2026.07.29 | 高 |
| 10 | ORCL $664B backlog/+121%/FCF 负 | billionaires.africa/webpronews | 2026.09.11 | 高 |
| 11 | PLTR Q1 +85%/Q2 +93%/$300B | vaasblock/aistockbubbleindex/edgen | 2026.08-09 | 高 |
| 12 | Cursor $4B ARR/SpaceX $60B | clinkbill/Sacra/au.investing | 2026.06-09 | 中高（ARR 未审计） |
| 13 | Glean $300M/Harvey $11B/Sapphire 80+ 家 | themeridiem/agentmarketcap/SaaStr | 2026.04-09 | 中高 |
| 14 | WDAY agentic ~$500M/ACV +200% | druckfin/metirai | 2026.06-09 | 高 |
| 15 | SNOW +37%/Databricks $7B +80% | Snowflake IR/CNBC | 2026.06-09 | 高 |
