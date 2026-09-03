# 魔鬼辩护人报告 — Round 4

> 课题: #08 AI Agent与白领劳动力市场重构
> 分析日期: 2026-09-03
> 角色: 魔鬼辩护人（只看背景包，未读任何研究员报告）
> 信息截止: 2026-09-03；捕获窗口 2026.07.10 → 2026.09.03
> 方法论备注: anysearch MCP 持续报错（返回账号生成提示），按预案回退 WebSearch（web_search_prime 后端）。全部论据均标注来源与日期；强弱分级按可验证性与来源独立性。

---

## 〇、本轮一句话立场

本课题最大风险已从"Agent 续约崩塌"迁移到"AI 融资层断裂"：CoreWeave CDS 实质触发 K12（~855bp，隐含 5 年违约概率 50%），五大 Hyperscaler Q2 合并 FCF 仅 $4.8B，而所有需求侧指标（NVDA Q3 指引 $108B、Copilot 30M 座位、NOW AI ACV $1B）都在加速——**这不是需求证伪，而是"需求为真、融资先死"的电信泡沫 2.0 结构**，恰恰是最难对冲的一种。

---

## 一、反方论据汇总

| 假设 | 反方论点 | 证据 | 证据强度 | 来源（日期） |
|------|---------|------|:-------:|------|
| H1 能力跃升 | **首选基准体系陷入可信度危机**：OpenAI 已于 2026-02-23 弃用 SWE-bench Verified，理由是 59.4% 的失败测试用例本身有缺陷、且所有前沿模型均检出训练数据污染。R3 赖以打 3.5/5 分的"基准分数"这一测量层正在崩塌 | OpenAI 官方退役 + 独立复核（59.4% 缺陷率） | 强 | byteiota.com（2026-04-27）；adwaitx.com（2026-02-23） |
| H1 | "Agent 80% 分数 vs 真实代码库失败"的 leaderboard-生产落差被多方记录；SWE-bench Pro 同样被质疑 verifier gaming 与污染 | 行业分析多篇，方向一致但非同行评审 | 中 | agentmarketcap.ai（2026-04-05/04-09）；niteagent.com（2026-06-28）；kansei-link（2026-04-29） |
| H1 | CMU TheAgentCompany 顶部成绩仍为 ~30.3%（Gemini 2.5 Pro），未检索到 2026 年下半年突破 40% 的更新；K11 阈值（<40% → 拐点推迟 2029+）正在逼近 | 榜单数据可能滞后（负向证据的固有弱点） | 中 | the-agent-company.com 榜单/arXiv 2412.14161 |
| H1（反向） | 能力侧无法全面证伪：NVDA DC 收入 +117%、编码 Agent 收入真实。基准危机 ≠ 能力停滞，本轮只能降置信度不能翻结论 | 需求与收入数据 | —（不利证据，如实记录） | NVIDIA 财报（2026-08-26） |
| H2 采纳拐点 | **使用率官方口径第 4 个季度缺席**：MSFT FY26 Q4（7/29）只披露付费座位（30M，环比 +10M），仍拒绝披露 DAU/活跃率。独立口径：~3.3% 的 450M Office 用户使用（来源弱）；75% 受访管理者称员工难以把 Copilot 融入日常（TechCrunch 引述调查）；50% 技术负责人不确定是否值回票价（SAMexpert） | 官方披露缺位本身即最强证据；独立数字来源偏弱 | 中 | MSFT FY26 Q4 新闻稿（2026-07-29）；TechCrunch 调查引述；SAMexpert（2026） |
| H2 | Gartner "40% agentic AI 项目 2027 年底前取消"预测的兑现路径在累积（管理层问题而非模型能力）；配合 MIT NANDA "95% 企业 GenAI 试点零回报"（2025-08，方法论受批评） | 预测非实测；MIT 报告有争议 | 弱-中 | Gartner 官方（2025-06-25）；Forbes（2026-07-07）；Fortune（2025-08-18） |
| H2（反向） | 座位与 ACV 加速反证空头：Copilot 20M→30M（一季 +50%）；ServiceNow AI ACV 破 $1B、净新 AI ACV 环比 +40%、$1M+ AI 交易 +50% QoQ。**H2 空头本轮弹药不足，使用率不透明是唯一持久抓手** | 财报与官方新闻稿 | —（不利证据） | MSFT/NOW 财报（2026-07-29 / 07-22） |
| H3 劳动力替代 | **AI 裁员流数据急速退潮**：5 月峰值 38,579 → 7 月 10,970（连续第 5 个月居首，占当月 33%）→ **8 月骤降至 3,462，跌至第 4 大裁员原因**；7 月总体裁员 33,429 为两年新低。R3 的"结构性成分 40-50%"归因若失去持续数据流支撑，叙事层面先于基本面褪色 | Challenger 官方 + Trading Economics | 中（单月数据，待 9 月确认趋势） | challengergray.com（2026-08）；tradingeconomics.com |
| H3（反向） | 企业端结构性证据反而增强：BPO 崩塌确认——Teleperformance 自高点 -60%、Concentrix -40%（单日 -24%，FY26 收入指引中值下调 ~$130M，EPS 指引 $10.83-11.18 vs 预期 $11.71）；Revelio Labs：18 个月内入门级招聘 -11%；大学毕业生占失业人口比例创纪录（~1/4）；半数组织以"资深员工+AI"替代多名应届生 | 多源交叉 | —（不利证据，支持论题） | Bloomberg/Nearshore Americas（2026-06-30 后）；Revelio Labs（2026-02）；HR Dive（2026） |
| H4 监管不构成硬刹车 | **证伪失败——监管比 R3 假设的更软**：EU Digital Omnibus（2026-06 获批）将 Annex III 高风险条款（含雇佣场景——恰是本课题核心场景）推迟至 2027-12-02（16 个月）；推迟系大科技公司游说结果。8/2 生效的执法（罚则最高全球营收 3%）首批案例未检索到；美国 6/2 行政令为亲产业"早期政府访问"框架；GPT-5.6 12 天 gate 后 7/9 放行，此后无第二次干预（K8 未触发） | 官方文件 + 路透 | —（不利证据：H4 假设方向正确） | Gibson Dunn/Reuters（2025-11-19、2026-06）；EC 官网（2026-08-02）；White House（2026-06-02） |
| H5 CapEx 不中断 | **融资层先行恶化（本轮最强弹药）**：① 五大（AMZN/MSFT/GOOGL/META+Oracle）Q2 2026 合并 FCF 仅 **$4.8B**；② Epoch AI：合计现金 CapEx 将于 2026Q3 超过经营现金流；③ FactSet：CapEx 中 ~60% 为短寿命算力资产（2022 年 43%），Hyperscalers 开始依赖外部融资；④ CoreWeave：Q2 净亏 $626M（H1 累亏 $1.37B）、总债务 $35.6B、Q2 利息费用 $640M（去年同期 $267M）、Q1 FCF -$4.71B、股价较峰值 -51%；⑤ **CDS ~855bp、隐含 5 年违约概率 50%**（7/29 单日 -9%）；⑥ AI 相关债务存量 ~2026 年逼近 $570B；私募信贷整体违约率 6.0%（2026-04，有统计以来最高） | 财报 + 一级/二级信用市场数据，多源独立 | 强 | Mohit Agrawal（LinkedIn，2026-08）；epoch.ai（2026-06-16）；insight.factset.com（2026-07-23）；CoreWeave IR/10-Q（2026-08-11）；TechTimes（2026-07-30）；MarketWise（2026-08）；FSB（2026-05） |
| H5 | 市场开始惩罚支出：Alphabet 上调 2026 CapEx 至 $195-205B 后财报被"panned"，Meta/MSFT 跟跌——CapEx 疲劳是削减的前置信号；Burry：2026-28 折旧低估 $176B、利润虚高（NVDA 方有异议），已清盘 Scion 并持有 NVDA/PLTR 看跌期权 | 市场反应属实；Burry 为单一投资人观点 | 中 | CNBC（2026-07-28）；Dave Friedman Substack/Fortune（2025-11） |
| H5（反向） | 需求侧未断裂：2026 指引全员上调（AMZN ~$220B / GOOGL $195-205B / META $130-145B / MSFT ~$175B，合计 ~$733B，同比近翻倍）；无任何一家下调 >20%（K3/K10 未触发）；NVDA Q2 超预期（$96.2B，DC $89.0B +117%），Q3 指引 ~$108B；CoreWeave backlog $104B、并完成 $8.5B IG 评级 GPU 融资 + $2.6B 贷款 | 财报 | —（不利证据） | 各公司财报（2026-07/08）；NVIDIA（2026-08-26）；CoreWeave IR（2026-08-10） |
| CRM（专题） | **Agentforce ARR 口径扩容**：Q2 FY27 ">$1.5B，+240% Y/Y" 系把 Slackbot 与 Headless 360 并入后的数字（Q1 为 $1.2B、更早 $800M）。在市场最需要验证续约质量（K9）的季度，Salesforce 选择扩口径而非披露 NDR——**指标通胀直接使 K9 失明** | 官方脚注 + 卖方/独立分析均指出 | 强 | Salesforce IR（2026-08-26）脚注；Quasa；IndMoney |
| CRM（专题） | 7/9 KeyBanc+Bernstein 同日双降（KeyBanc 降至 Sector Weight 并撤销目标价："Agentforce 未就绪"、企业数据基础不足、"几乎没有 Agentforce 提速的证据"）；Benioff 公开回击——管理层对空头观点的敏感度本身是信号 | 卖方渠道调查 | 强（但已被 8/26 财报部分回击：attrition 接近纪录低位、CRPOB 强、股价 +22.6% 至 $257.54） | Yahoo Finance/IBD/TipRanks（2026-07-09） |
| CRM（专题） | 执行纪律风险：R3 入场区 $155-175、止损 $140；财报后股价 $257.54（8/31 收盘，两个月 +33%），**已高于入场区上限 47%**。若现在按计划"续约率>75% 加至 5%"，等于在利已兑现后追高；且"agentic 自噬"论（按消费计费的 Agent 侵蚀座位制收入）在 Headless 360（API 即 UI、免浏览器）战略下被公司自身加速 | 价格事实 + 结构性论点 | 中 | Investors.com/StockStory（2026-08-26 后）；businessengineer.ai |

---

## 二、最可能的失败模式（Top 3）

### 失败模式 1: AI 融资层断裂 + 债务危机（电信泡沫 2.0 完整兑现）【升为第一】
- 描述: 需求为真但融资先死。CoreWeave（及未上市 neocloud）的 GPU 抵押融资链断裂 → 私募信贷（违约率已达 6.0%）与 AI IG 债利差急速走阔 → Hyperscaler 被迫在 FCF 转负（Q3 CapEx>OCF）后削减 2027 CapEx → NVDA 链条量价齐缩 → 全部 AI 关联资产（含本课题 CRM/MSFT/NOW）遭遇 2022 SaaS 式系统性 de-rate。
- 触发条件: ① CoreWeave 债务重组/资产出售/优先级减记（CDS 855bp、隐含违约 50% 已是半只脚 inside）；② 任一 Hyperscaler 首次给出 2027 指引即低于市场预期；③ 私募信贷违约率 >7% 或 AI IG 利差再走阔 150bp。
- 传导路径: [CoreWeave CDS/重组] → [私募信贷抽贷 + AI 债发行失败] → [2027 CapEx 指引下修] → [NVDA 撤单/折旧恐慌（Burry $176B 论）] → [软件 AI 估值整体压缩] → [CRM/MSFT/NOW 多头组合受损 + #01/#17/#05 连锁]
- 概率: **25%**（R3 的 CapEx 断裂 20-22% 上调：Q2 财报季全部利空信号兑现——FCF $4.8B、CDS 触发 K12、市场开始惩罚 CapEx）
- 预期损失: -25% ~ -35%（对课题多头篮子；参考 2022 SaaS 篮子 -60% 的折半情景）
- 附注: 该失败模式与本课题 Bull 情景并不互斥于"AI 最终成功"——电信泡沫后互联网确实改变了世界，但 2000-2002 年间多头照样亏 80%。这是背景包"所有人都同意 AI 是真趋势"的共识中最被低估的路径。

### 失败模式 2: Agentforce 增长质量证伪 + 追高回吐（原"续约崩塌"的变体降级）【下调】
- 描述: Q2 FY27 已证明"续约崩塌"短期不成立（attrition 接近纪录低位），失败模式改以"增长质量"形态存活：ARR 靠口径扩容维持高增速、有机成分不可分解；Dreamforce（9/15-17）若只拿出 demo 而非生产 ROI，或 FY27 H2 cRPO/cNAR 减速，市场将同时重估"AI 收入成色"与 22.6% 的单日涨幅。
- 触发条件: ① Agentforce ARR 连续两季依赖口径变更/并购维持增速；② cRPO 增速跌破 ~10%；③ 座位制核心收入因 Agent 消费计费出现自噬性减速；④ 股价 $257 上方建仓后的任何负向意外被放大。
- 传导路径: [ARR 口径游戏被卖方点名] → [Dreamforce 兑现不足] → [AI 收入成色重估] → [戴维斯双杀：EPS 下修 × PE 回吐] → [课题第一权重仓受损]
- 概率: **15%**（R3 的 20-25% 下调：8/26 财报实质削弱了空头论据；但口径扩容与追高纪律风险为新添加剂）
- 预期损失: -20% ~ -25%（回到 $200 下方即 -22%）

### 失败模式 3: 能力天花板 + 基准信任崩塌 + Agent 洗涤反噬【上调】
- 描述: 与 R3 相同骨架但弹药更新：OpenAI 退役 SWE-bench Verified（污染 + 59.4% 缺陷用例）意味着"能力跃升"的公共测量层破产；若 CMU TheAgentCompany 到年底仍 <40%（当前 30.3%），Gartner 40% 取消潮与 MIT 95% 试点失败在 2027 续约季形成合力——企业把"Agent 预算"砍向"Agent 洗涤"清算，CRM/NOW 的 AI 溢价凭证消失。8 月 AI 裁员骤降至 3,462 同步抽走"劳动力重构"叙事的现实感。
- 触发条件: ① K11 正式触发（2026-12-31 榜单顶部仍 <40%）；② Gartner 取消潮在 2027 财年企业预算中显性化；③ Agentforce/Copilot 续约季出现首个公开大客户流失案例。
- 传导路径: [基准可信度崩塌] → [企业 PoC 批量放弃] → [AI ARR 增速换挡] → [叙事从"数字员工"退回"高级 Copilot"] → [课题核心逻辑失效、评级降至技术关注]
- 概率: **16%**（R3 的 12-15% 上调：基准退役 + K11 逼近 + 裁员流退潮三重增量）
- 预期损失: -15% ~ -20%（课题级）

---

## 三、历史类比

### 类比 1: 1998-2002 电信泡沫 / 光纤过剩
- 相似度: **高**
- 最终结果: 失败（需求最终为真，资产负债表先死）
- 失败原因: 2002 年仅 ~5% 骨干光纤被点亮；设备商供应商融资（朗讯借钱给运营商买自家设备）制造循环收入；WorldCom/Global Crossing 破产。今天的同构物：NVDA—neocloud—Hyperscaler 的循环（CoreWeave $104B backlog 的对手方集中度）、CoreWeave 以 Meta 合同支撑的 $8.5B "IG 评级" GPU 融资、GPU 4-5 年折旧 vs 1-2 年代际淘汰（Burry $176B 论）。Hyperscaler CapEx/EBITDA 已被多方比对至周期爆破前水位。
- 对当前课题的启示: 电信泡沫的教训不是"互联网是假的"，而是**融资结构与资产寿命错配可以在需求为真时先杀死股东**。本课题的退场标准过度聚焦收入侧（续约、ARR），对信用侧只有 K12 一条——而 K12 本轮已触发。另注意一个反面差异：五大 Hyperscaler 自身经营现金流仍庞大（与 2000 年 telecom 纯杠杆不同），断裂点更可能在 neocloud/私募信贷层，再传染。
### 类比 2: 2020-2022 SaaS/零利率泡沫
- 相似度: **中-高**
- 最终结果: 失败（使用率大体为真，估值凭证消失）
- 失败原因: Zoom/协作 SaaS 在"永久远程办公"叙事下获得永久成长股定价；2022 年折现率上行后篮子 -60%+，收入没崩、倍数崩了。同构物：Copilot/Agentforce 以座位数叙事获得 AI 溢价，而使用率口径持续缺席；一旦宏观（利率）或增长质量任一变量翻转，$257 的 CRM 与 30M 座位的 Copilot 都没有估值缓冲。
- 对当前课题的启示: 入场纪律（$155-175）是上一轮用亏损换来的便宜保险；两个月 +33% 后放弃该纪律，等于主动把 SaaS-2022 型风险装入组合。
### 类比 3（补充）: 2021-2023 元宇宙企业级炒作流产
- 相似度: 中
- 最终结果: 失败（Meta 累计 ~$70B+ 投入后企业级场景无 PMF）
- 失败原因: 把旧产品改名迎合新名词（Gartner 称之为 agent washing 的前身）；Gartner 本轮明确警告厂商把聊天机器人重新包装成 Agent。
- 对当前课题的启示: "Agent 洗涤"反噬有先例可循——当买家学会区分口径（正如本轮 Agentforce ARR 扩容被卖方立刻点名），洗涤溢价消退速度远快于基本面。

---

## 四、退场标准 K1-K12 触发状态核查与补充建议

### R3 标准 K1-K12 实际状态（本轮核查）

| # | 标准 | R3 状态 | 本轮核查结果 |
|---|------|--------|-------------|
| K1 | Agentforce/Copilot 收入增速连续两季 <10% | 接近监控 | **未触发**：Copilot 座位 20M→30M（QoQ +50%）；Agentforce ARR +240%（口径污染但 >10%）；NOW AI ACV +40% QoQ |
| K3/K10 | 2 家+ Hyperscaler 下调 2027 CapEx >20% | 未触发 | **未触发**：2026 指引全员上调（合计 ~$733B）；正式 2027 指引仍稀缺——注意"不上报"不等于"上调"，可测性差本身是问题 |
| K8 | 前沿模型政府干预再发 | 未触发 | **未触发**：GPT-5.6 12 天 gate 止于 7/9；其后仅 6/2 亲产业 EO，无新干预（沙箱逃逸传闻可靠性低，仅监控） |
| K9 | Agentforce NDR<80% 或净新 ARR 环比 <10% | 未触发 | **名义未触发、实质失明**：公司未披露 NDR；净新 ARR 环比 +25% 但含 Slackbot+Headless 360 口径扩容，有机成分不可分解 |
| K11 | CMU Agent 基准 6 个月无突破（<40%） | 未触发（30.3%） | **接近触发/待核实**：未检索到顶部成绩突破 40% 的更新；建议 2026-12-31 以官方榜单为准做正式裁定 |
| K12 | H100 租金 <$1.50/hr 或 CoreWeave CDS>600bp | 未触发（~450bp） | **已触发（CDS 分量）**：CDS ~855bp（7/30 隐含 5 年违约概率 50%）；H100 市场价 $1.09-1.49/hr（合约指数仍 $2.35，现货/合约劈叉）——按 OR 逻辑 K12 成立。**建议 CIO 本轮明确 K12 触发的既定后果并执行**（若 R3 未定义后果，立即补充定义，见 K-new） |

### 补充建议

| 建议编号 | 建议退场条件 | 后果 | 理由 |
|---------|-----------|------|------|
| K13 | Agentforce/AI ARR 口径再次变更，或连续两季不提供可比同比口径 | 禁止加仓 + 增长质量降级 | Q2 FY27 口径扩容已使 K9 失明；披露退化是最廉价的领先预警 |
| K14 | 任一上市 neocloud（CoreWeave/Nebius 等）宣布债务重组、优先级减记或大规模资产出售 | 课题降级复核；BPO 空腿立即获利了结并对软件多腿做对冲 | 电信类比中的 WorldCom 时刻；BPO 空头届时大概率已 price in（TP -60%/CNXC -40%），空腿收益风险比反转 |
| K15 | 私募信贷违约率 >7%，或 AI 相关 IG 债利差自 2026-07 水位走阔 >150bp | 触发 H5 专项复查（合并 #01/#17 联席） | H5 已是第一失败模式，信用侧仅有 K12 一条腿不够 |
| K16 | Copilot 付费座位环比转负，或 MSFT 停止披露座位数 | H2 降级 | 座位是 H2 唯一可验证官方口径；披露停止=使用率问题的官方默认 |
| K17 | Challenger AI 裁员连续 3 个月 <3,000 且总体裁员低于 5 万均值 | H3 降级（叙事退潮） | 8 月 3,462 已是预警样本；H3 的"结构性替代"需要持续数据流背书 |
| K18 | MSFT FY27 正式 CapEx 指引低于市场预期（而非未披露） | 视幅度触发 K3/K10 | 本轮"2027 首次正式指引"并未真正落地为可验证数字，标准需要量化锚点 |

---

## 五、数据来源

| # | 数据点 | 来源 | 时间 | 可靠性 |
|---|--------|------|------|:------:|
| 1 | MSFT FY26 Q4：收入 $90B(+18%)、Copilot 30M 付费座位（环比 +10M）、Azure>$100B、RPO $678B | microsoft.com 官方新闻稿/news.microsoft.com | 2026-07-29 | 高 |
| 2 | Copilot 使用率无官方口径；75% 管理者称员工难融入；50% 负责人不确定值回票价 | TechCrunch 引述调查；SAMexpert；Reddit 3.3%（弱） | 2026 | 中-低 |
| 3 | Salesforce FY27 Q2：收入 $11.35B(+10.8%)、Agentforce ARR>$1.5B(+240%) **含 Slackbot+Headless 360 口径扩容**、attrition 接近纪录低位、FY27 指引上调 $46.1-46.4B；股价财报后 +22.6% 至 $257.54(8/31) | Salesforce IR 新闻稿+投资者 deck；Quasa/IndMoney/StockStory | 2026-08-26 | 高（数字）/中（解读） |
| 4 | 7/9 KeyBanc（Sector Weight、撤目标价）+Bernstein 双降："Agentforce 未就绪"、数据基础不足 | Yahoo Finance、IBD、TipRanks、Seeking Alpha | 2026-07-09 | 高 |
| 5 | 五大 Hyperscaler Q2 合并 FCF $4.8B；Epoch AI：2026Q3 CapEx>OCF；CapEx ~60% 为短寿命资产、依赖外部融资 | Mohit Agrawal(LinkedIn)；epoch.ai；FactSet Insight | 2026-06-16 / 07-23 / 08 | 高 |
| 6 | 2026 CapEx 指引：AMZN ~$220B、GOOGL $195-205B（财报被"panned"、Meta/MSFT 跟跌）、META $130-145B、MSFT ~$175B、合计 ~$733B | CNBC；FutureX Capital/Agrawal | 2026-07-28/08 | 高 |
| 7 | CoreWeave Q2：收入 $2.58B、净亏 $626M（H1 $1.37B）、债务 $35.6B、利息 $640M/Q、backlog $104B、$8.5B IG GPU 融资 + $2.6B 贷款 | CoreWeave IR/10-Q/电话会实录 | 2026-08-10/11/12 | 高 |
| 8 | CoreWeave CDS ~855bp、隐含 5 年违约 50%（7/29 股价 -9%）；H100 市场租金 $1.09-1.49/hr、现货/合约劈叉（SemiAnalysis 合约指数 $1.70→$2.35） | TechTimes；MarketWise；IntuitionLabs；SemiAnalysis | 2026-07-30 / 08 | 中-高 |
| 9 | OpenAI 退役 SWE-bench Verified（59.4% 失败用例有缺陷+全面污染）；SWE-bench Pro 亦受 gaming 质疑 | byteiota；adwaitx；agentmarketcap；niteagent；kansei-link | 2026-02-23 ~ 06-28 | 中-高 |
| 10 | CMU TheAgentCompany 顶部仍 ~30.3%（Gemini 2.5 Pro），未见 2026 突破 40% 更新 | the-agent-company.com；arXiv 2412.14161 | 2026（数据滞后风险） | 中 |
| 11 | Challenger：7 月 AI 裁员 10,970（占 33%、连续 5 月居首、总体裁员两年新低 33,429）；8 月骤降 3,462（第 4 位）；2026 累计 112,713 | challengergray.com；Trading Economics | 2026-08 | 高 |
| 12 | BPO：Teleperformance -60%、Concentrix -40%（单日 -24%）、FY26 收入指引下调 ~$130M；入门级招聘 18 个月 -11%；毕业生占失业人口纪录 ~25% | Bloomberg/Nearshore Americas；Revelio Labs；Washington Monthly；HR Dive | 2026-02 ~ 07 | 高 |
| 13 | EU AI Act：8/2 执法生效（罚则至全球营收 3%）、首批案例未见；Annex III 高风险（含雇佣）推迟至 2027-12-02（Digital Omnibus） | EC 官网；Gibson Dunn；Reuters；Morgan Lewis | 2026-06 ~ 08-02 | 高 |
| 14 | GPT-5.6 于 6/26 被 White House 要求推迟、12 天 gate 后 7/9 公开（Sol/Terra/Luna）；6/2 早期政府访问 EO；其后无二次干预 | Reuters；TechCrunch；TechTimes；White House | 2026-06-02 ~ 07-09 | 高（沙箱逃逸细节除外=低） |
| 15 | NVIDIA Q2 FY2027：收入 $96.2B(+106%)、DC $89.0B(+117%)、Q3 指引 ~$108B | NVIDIA 官方 | 2026-08-26 | 高 |
| 16 | ServiceNow Q2：AI ACV 破 $1B、净新 AI ACV +40% QoQ、$1M+ AI 交易 +50% QoQ、续约率 98% | ServiceNow 新闻稿/SEC | 2026-07-22 | 高 |
| 17 | AI 债务存量 ~$570B（2026）；私募信贷违约率 6.0%（4 月，历史最高；FSB 称 AI 相关违约尚低）；Burry：折旧低估 $176B、持有 NVDA/PLTR 看跌 | FSB 报告；Goldman 引述；Fortune/Dave Friedman | 2026-04 ~ 11 | 中-高 |
| 18 | Gartner：>40% agentic AI 项目 2027 年底前取消（成本/价值/风控）；~50% GenAI PoC 弃置；MIT NANDA 95% 试点零回报（方法论有争议） | Gartner 官方；Forbes；Fortune | 2025-06 ~ 2026-07 | 中 |

> 检索工具备注：anysearch MCP 本轮持续故障（返回自动账号生成串，非搜索结果），全部检索经 WebSearch 回退完成；关键数字（CRM 口径脚注、CDS、Challenger 8 月、SWE-bench 退役）均经 2 个以上独立来源交叉。
