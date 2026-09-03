# 基本面研究员（研究员A）独立研究报告

> 课题: #08 AI Agent与白领劳动力市场重构
> 分析日期: 2026-09-03
> 角色: fundamental（估值、财务建模、行业对比）
> 搜索工具: anysearch（首轮配额中断）→ WebSearch 回退；捕获窗口 2026-07-10 → 09-03

---

## 一、核心发现（Top 3）

1. **K9 关键验证通过，但含两处口径水分**：Salesforce FY27 Q2（8/26 发布）营收 $11.345B（+11%）、cRPO $33.5B（+14%，超指引 1pt 且环比加速）、**收入流失率（attrition）约 8% = 隐含续约率 ~92%，历史低位**——管理层明确将 cRPO 超预期归因于"创纪录 bookings + 近历史低位 attrition"。R3 失败模式 #1（Agentforce 续约崩塌，概率 20-25%）实质证伪，我下修至 ~12%。但两个折扣：①Agentforce ARR "$1.5B+，+240% Y/Y" 自本季起**并入口径** Slackbot 与 Headless 360，与 Q1 的 $1.2B 不可直接比；②Non-GAAP EPS $5.90（+103%）含 **Anthropic 股权 $2.6B 浮盈**（持仓约 $5.1B），经营性 beat 幅度远小于表观。股价单日 +22.6% 收 $252.05（史上第二佳）、8 月 +40%、9/2 报 $259.22，Forward PE 从 11-12x 修复至 ~16x——**R3"显著低估"的错杀段已兑现大半**。

2. **H5 的 2026 段全面强化、2027 段仍未闭环，约束从"意愿"转向"融资"**：Q2 财报季四大 Hyperscaler 无一下调（K3/K10 未触发）：Alphabet 上调 2026 CapEx 至 $195-205B、Amazon ~$220B、Meta 收窄至 $135-145B、MSFT FY27 定性"同比增长"+ Q1 FY27 指引 >$50B；合计 2026 tracking **~$733B**（R3 基线 $710-725B）。**2027 正式公司指引依然缺席**（Citi 预估 GOOGL ~$308B/META ~$205B/三家 >$800B，为卖方口径）。代价端：Q2 四家合计 CapEx $165B vs 合计 FCF 仅 ~$7B（Meta 单季 FCF $784M、Alphabet 首次单季负 FCF）；Meta+MSFT+Oracle 年初 5 个月发债 $159B，2026 全年 AI 相关债券发行预估 $300-570B，Meta $30B 走 Blue Owl SPV（233% 杠杆、表外零追索）。NVDA Q2 FY27（8/26）营收 $96.22B（超 $91B 指引 5.7%）、DC $89.0B（+117%）、Q3 指引 **$108B±2%**（超共识 $104B，且不含中国 DC 计算）为需求侧最强佐证。

3. **编码 Agent 赛道复利加速 + 战略溢价确认**：Cursor/Anysphere 年化收入 $2B（2026/2）→ $3B（4 月底）→ **$4B+（6 月初）**，公司指引年末 $6B+；且据 CNBC/Zacks（引 SEC 文件）报道，**SpaceX（联合 xAI）以 ~$60B 收购 Anysphere，8/14 完成**——编码 Agent 是唯一同时拿到"收入复利"与"巨头战略并购溢价"双验证的场景。Cognition（Devin）维持 $492M run-rate（5/27 Series D 披露，$1B 融资 @$26B 估值，企业用量年内 >10x），本轮无更新。对照企业横向 Agent：MSFT Copilot 付费座位 20M→**30M**（单季 +10M、净增环比翻倍）、Copilot 收入环比 +60%——货币化在加速，但 D8 遗留的使用率硬数据仍缺位（详见 2.2）。

---

## 二、详细分析（按标的）

### 2.1 Salesforce (CRM) — 本课题定义性催化剂已落地（D2/K9）

| 指标 | Q2 FY27（截至 7/31，8/26 发布） | 判读 |
|---|---|---|
| 营收 | $11.345B，+11%（含 Informatica 贡献 $456M） | 略超共识 $11.33B |
| cRPO | $33.5B，+14%（名义与 cc 同） | 超指引 1pt，环比加速 |
| 总 RPO | $66.3B | — |
| attrition | ~8%（投资者 deck 披露） | **续约率 ~92%，K9 的 NDR<80% 远未触发** |
| Agentforce ARR | >$1.5B，+240% Y/Y | **口径并入口径 Slackbot+Headless 360**；Q1 为 $1.2B |
| Agentforce+Data 360 ARR | ~$3.9B，+210% Y/Y | — |
| Agentic Work Units | 3.2B 次/季，环比 +97% | 消费量信号真实 |
| Non-GAAP EPS | $5.90（+103%） | 含 Anthropic 浮盈，GAAP $4.29 |
| FCF | ~$1.1B，+81% | — |
| FY27 指引 | 营收上调至 $46.1-46.4B（+11-12%）；non-GAAP 运营利润率维持 ~34.3% | 上调 $200-300M |

**判读**：①K9 三条件（NDR<80% / 净新增 ARR 环比<10% / 收入增速连续两季<10%）全部远离触发——即使对口径变更打折，旧口径环比也应 >10%（$1.2B→保守 $1.35B+）。②Q1 披露 Agentforce 生产客户环比 +50%、Agentforce/Data360 bookings 约 50% 来自存量客户 = 扩张型收入占主导，隐性 NDR >100%（第三方估全部客户中付费渗透仅 ~6%，天花板仍远）。③管理层公开反驳"SaaSpocalypse"，称净新增 AOV 增速为四年最强。④**利润质量**：剔除 Anthropic 浮盈后经营性 EPS beat 温和；Anthropic IPO 目标 2026/10（有推迟至 Q4+ 传闻），若 IPO 受阻，浮盈项反噬 GAAP 利润。⑤估值：9/2 股价 $259.22，Forward PE ~16x（GuruFocus，"适度低估"），trailing 19.1x；Morningstar 提示"估值开始变满"。**R3 的 $155-175 入场区间与 11-12x 低估窗口已关闭**；DCF 复算：维持 FY28-29 EPS CAGR 12-14% 假设，合理区间从 $293.74 上移有限（利润率指引未上调），约 $270-300，安全边际收窄至 5-15%。

### 2.2 Microsoft (MSFT) — D1 全部到位，D8 部分闭环

- **FY26 Q4（7/29）**：营收 $90.0B（+18%），FY26 全年 $331B；EPS $4.74 超预期；Microsoft Cloud $59.3B（+27%）；Azure 年化破 $100B（Q4 增速 43-45%）；商业 RPO ~$678B。
- **Copilot**：付费座位 **30M+**（Q3 FY26 为 20M，单季 +10M、净增环比翻倍以上）；**Copilot 收入环比加速 +60%**；AI 业务年化 run-rate 最后官方口径为 Q3 FY26 的 **$37B（+123% Y/Y）**，Q4 未更新。
- **CapEx/FCF**：Q4 CapEx $41B（约 2/3 为短寿命资产，含元器件涨价影响，略低于街预期 $42.4B）；Q4 FCF $19.64B（-23%）。FY27：官方仅给定性"同比增长"（媒体流传的 $255-260B 为 UBS 等预期而非指引）；**Q1 FY27 指引 >$50B**（含租赁重分类影响，数据中心资产折旧寿命会计延长约十年）；Amy Hood 承诺 **FY27 全年 FCF 为正**。
- **D8 使用率（R3 遗留 P0-1）**：Q4 未披露官方 DAU 比例；7/30 官网发文"下一个 AI 动量度量是 work transformed"，口径从座位数**主动切换**到使用/工作成果（称周活跃已可类比 Outlook/Teams 级别）；历史锚点：Q2 FY26 称 DAU 同比 ~10x（~1.2M→12M+），2026/2 第三方估 Copilot DAU ~60M（含消费者）。**结论：官方给了加速的收入与座位，但没有给可独立复核的使用率%——售用差 95.5% 的指控未被硬数据否定，也未确认**。市场选择相信收入：财报次日 +8-9%、单日市值 +$260B（公司史上最大），现价 ~$513、市值 ~$3.7T、Forward PE ~22.6x（20 年区间中位附近）。

### 2.3 ServiceNow (NOW) — D4：AI ACV 提前跨过 $1B

Q2 2026（7/22）：营收 $3.987B（+~22%）；**AI ACV 突破 $1B**（R3 基线 Now Assist $750M），9 个月内 agentic 部署量 9x；123 笔净新增 ACV >$1M 交易（+40% Y/Y）、16 笔 >$5M；**整体续约率 97%**；FY26 订阅收入指引上调至 $15.755-15.77B（+21% cc）、运营利润率 31.5%。估值：股价 ~$137-145（拆股后），Forward PE 27.2-30.2x（口径分歧大）、trailing ~75-90x。**判读**：AI Pro Plus 货币化证明"垂直+工作流嵌入"路线优于通用 Copilot 座位模式；但 27x+ 对应 21-22% 增速，PEG ~1.3，估值中性，维持 1% 仓位合理，不加。

### 2.4 NVIDIA + Hyperscaler CapEx（D3/D6，H5/K3/K10）

- **NVDA Q2 FY2027（8/26）**：营收 $96.22B（+106%，超 $91B 指引 5.7%）；DC $89.0B（+117%；Hyperscale $49B 环比 +13%、另一类 $40B）；non-GAAP EPS $2.22；**Q3 指引 $108B±2%**（共识 $104.19B），毛利率指引降至 ~74%（存储成本）；Vera Rubin 预计占 Q3 DC 收入 ~20%；FY27 全年隐含 ~$394B。
- **2026 CapEx 指引汇总**：Alphabet $195-205B（自 $180-190B 上调，Cloud backlog $514B，财报被"panned"、引发同业连坐下跌）；Amazon ~$220B 现金 CapEx（Q2 单季 $53.1B，AWS backlog $496B、AWS 收入 +36.7%）；Meta $135-145B（Q2 单季 $31.08B，+83% Y/Y，EPS miss ~14%）；四家合计 tracking **~$733B**（+70% Y/Y 量级）。
- **2027**：**无一家给出正式数字指引**——这是 D3 的关键答案：K3/K10（2 家+ 下调 >20%）不仅未触发，方向反而向上（Citi：GOOGL $308B +21%、META $205B +22%、三家合计 >$800B）。正式指引预计在 Q3/Q4 电话会给出，为 H5 的下一个验证点。
- **融资面**：Meta/MSFT/Oracle 1-5 月发债 $159B；2026 AI 债券发行全年预估 $300-570B；Meta $30B 走 Blue Owl SPV（233% 杠杆、零公司追索、反向收 $3B 现金）；Oracle 有正式 2026 股债融资计划。**FCF 是新的硬约束**：Q2 合计 $165B CapEx vs $7B FCF（Jefferies/Chris Wood）。
- **CoreWeave（K12 canary，8/11）**：Q2 营收 $2.575B（+112%，超预期），backlog ~$104B（对应的"支出性 backlog" $115B）；净亏损扩大至 $626M，**单季利息费用 $640M（占营收 ~25%）**；债务 $25.1B + 租赁 $10B（Q1 末）；2026 调整后经营利润指引 $960M-1.15B 并上调 CapEx。K12 判定：**未触发**——H100 一年期合约价从 2025/10 低点 $1.70 回升至 $2.35（2026/3，SemiAnalysis 指数，+40%），高于 $1.50 阈值；CoreWeave CDS 本轮未获新数据（R3 ~450bp，**待验证**）。

### 2.5 编码 Agent 基本面（H1 需求侧证据）

Cursor/Anysphere：$100M（2025/1）→ $1B（2025/11）→ $2B（2026/2）→ $3B（4 月底）→ **$4B+（6 月初）**，年末指引 $6B+（TechCrunch）；**SpaceX/xAI ~$60B 收购于 8/14 完成**（CNBC/Zacks，引 SpaceX S-1；该交易金额与结构极不寻常，可靠性中，建议 C 角色复核）。Cognition：$492M run-rate（5/27）、$26B 估值、企业用量年内 >10x，7-8 月无新披露。GitHub Copilot 付费用户 R3 口径 470 万，本轮未获更新（待验证）。

### 2.6 BPO 做空观察（H3，CNXC/Teleperformance）

- **Teleperformance H1 2026（7/30）**：营收 €4,883M，**-1.7% LFL**（名义 -4.5%）；Q2 -1.2% vs Q1 -2.2%（边际收窄）；recurring EBITA margin 13.6%（Q1 为 14.6%）；净利 €216M（同比降）；重组费 H1 €109M、全年指引上调至 €120-140M；**FY26 指引重申**（LFL 0-2%、margin ~14.6%）；AI 解决方案"强双位数增长"。
- **Concentrix 财年 Q2（5 月末止，6/29 发布，略早于本窗口）**：收入/利润符合指引；Q2 经营现金流 $258M、调整后 FCF $242M 创同期纪录；FY26 收入指引 $9.925-10.025B；EPS/收入较街预期微 miss。
- **判读**：结构性侵蚀（Trust&Safety 下滑、离岸加速、AI 替代）继续但**恶化速率没有加速**——TP 收入同比降幅收窄、指引重申、CNXC 现金流正常。做空逻辑（估值十年低位+收入拐头向下）最陡峭的一段可能已在上半年走完；BPO 空头从"进攻"降级为"观察"，0.5-1% 空头仓位的边际收益下降。
- **AI 裁员（H3 佐证）**：Challenger——7 月 AI 为裁员首要原因连续第 5 个月（7 月 10,970 例）；2026 前 7 个月科技业裁员 149,023（+67% Y/Y）；**2026 前 5 个月 AI 归因裁员 87,714，已超 2025 全年 54,836**；8 月总裁员 52,881、AI 占比环比回落。R3 区间"87-186K"将按当前速率上穿——结构性替代的经济账在强化，但月度节奏有波动。

---

## 三、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|------|------|------|:-----------:|
| H1 Agent 能力持续跃升 | 间接支持（需求侧收入证据） | Cursor $2B→$4B+/4 个月、Devin 企业用量 >10x、SpaceX $60B 战略溢价；基准榜单非本职范围 | 3 |
| H2 采纳拐点 2027H2-2028H1 | 正向偏移（2.5→3/5，或前移至 2027H1） | Copilot 座位单季 +10M、收入环比 +60%；NOW agentic 部署 9x/9 月；Agentforce AWU +97% QoQ；但使用率官方口径仍缺，试点→生产转化待验 | 3 |
| H3 劳动力替代经济账 | 维持通过（范围扩大，趋势在上沿） | AI 归因裁员 5 个月 87.7K>2025 全年；TP 重组费上调、LFL -1.7%；入门级岗位收缩快于裁员 | 3 |
| H4 监管不构成硬刹车 | 待验证（本职未覆盖） | 本轮未检索 EU AI Act 执法与新干预事件，留研究员 C | 2 |
| H5 AI CapEx 周期不中断 | **2026 强化通过；2027 待验证；断裂概率 20-25%→15%** | 四家全部上调/维持、合计 ~$733B；NVDA Q3 指引 $108B；K3/K10 未触发；对冲项：合计 FCF $7B、AI 债 $300-570B | 4 |

---

## 四、情景分析

| 情景 | 概率 | 核心驱动 | 预期回报（CRM/MSFT/NOW 篮子） |
|------|:----:|---------|---------|
| Bull | 30% | Dreamforce（9/15-17）Claudeforce GA 放量；Agentforce FY27 末 >$2B；2027 CapEx 正式指引 ≥$850B 且信用利差平稳；CRM FY28 EPS 上修 | +28% |
| Base | 45% | 增长兑现但已定价：CRM 16x 区间消化、MSFT 高位震荡、2027 指引"符合卖方" | +8% |
| Bear | 25% | 2027 CapEx 指引低于 Citi 口径 >15%/AI 债券利差走阔/Anthropic IPO 受阻引发 CRM 浮盈反噬+高估值回吐；Agentforce 口径问题被做空报告引爆 | -22% |
| **加权** | | | **+7.4%** |

（对照 R3 加权 +10%：**确信度上升、期望回报下降**——因为最肥的估值修复段已被 8 月 +40% 走完。）

---

## 五、时间维度

- **短期(1-3月)**：Dreamforce 9/15-17（Claudeforce GA、Agentforce 新口径首个公开检验）；Anthropic IPO 窗口 10 月（CRM 浮盈兑现/反噬双刃）；Hyperscaler Q3 财报（10 月底-11 月初，**2027 CapEx 正式指引最可能落地处**）；NOW/CRM 下季 attrition 与 cRPO 连续性。
- **中期(3-12月)**：2027 CapEx 指引 vs Citi >$800B 的偏差是 H5 终审；AI 债券（$300-570B）发行吸收度与 Blue Owl 类 SPV 的审慎性审查；Copilot 使用率是否有首次官方硬披露（D8 闭环）；BPO 在 2027 预算季的定价权检验。
- **长期(1-3年)**：采纳拐点若如 H2 前移，CRM/MSFT/NOW 的 Agent 收入从 <5% 提升至 10-15% 混合占比；劳动力端 AI 归因裁员年化 200K+ 与入门级白领就业的宏观数据联动。

---

## 六、基本面排名（研究员A 视角）

| 排名 | 标的 | 一句话理由 |
|:---:|---|---|
| 1 | MSFT | Copilot 收入环比 +60% + 30M 座位、Azure $100B、CapEx 有会计与 FCF 纪律叙事，22.6x forward 不贵不便宜——风险收益比最稳 |
| 2 | CRM | 证据最硬（attrition 8%/cRPO 加速/指引上调）但 $259 已兑现大半低估，16x 从"显著低估"降为"合理偏低"；持有优先于追高 |
| 3 | NOW | AI ACV >$1B + 97% 续约，货币化路径最干净，但 27-30x/21% 增速 PEG 中性，维持小仓 |
| 4 | NVDA（间接，#17 主战场） | $108B 指引为 H5 最强佐证，非本课题直接标的 |
| 5 | TP/CNXC 空头 | 逻辑仍成立但恶化速率未加速、指引重申、估值已在地板——空头性价比下降，建议降级观察 |

---

## 七、数据来源

| # | 数据点 | 来源 | 时间 | 可靠性 |
|---|--------|------|------|:------:|
| 1 | MSFT Q4 FY26：$90B/+18%、Copilot 30M 座位、CapEx $41B | microsoft.com IR 新闻稿 | 7/29 | 高 |
| 2 | Copilot 收入环比 +60%、Q1 FY27 CapEx >$50B、FY27 FCF 正 | MSFT FY26 Q4 电话会/IR | 7/29 | 高 |
| 3 | FY27 CapEx "同比增长"为定性、$255-260B 系 UBS 预期 | Digital Applied CapEx Scorecard | 7/30-8/5 | 中 |
| 4 | AI run-rate $37B/+123% | MSFT FY26 Q3 IR | 4 月 | 高 |
| 5 | Copilot 使用口径转向"work transformed"、无官方使用率% | MSFT 365 官方博客 | 7/30 | 高 |
| 6 | MSFT +8-9%、$513、3.7T、22.6x forward | CNBC/Perplexity Finance | 7/30-9 月 | 中 |
| 7 | CRM Q2 FY27 全套：$11.345B、cRPO $33.5B、attrition ~8%、Agentforce $1.5B 口径变更、FY27 上调 | Salesforce 新闻稿+投资者 Deck+电话会 | 8/26 | 高 |
| 8 | Agentforce 生产客户 +50% QoQ、~50% bookings 存量客户、~6% 渗透 | Q1 FY27 披露/第三方 | 5/28 | 中 |
| 9 | Anthropic 持仓 $5.1B/$2.6B 浮盈、IPO 目标 10 月或推迟 | Value Add VC/Bloomberg、Forge/Kiplinger | 6-8 月 | 中 |
| 10 | CRM +22.6% 收 $252.05、8 月 +40%、$259/16x forward | Perplexity/GuruFocus/Facebook 财经页 | 8/27-9/2 | 中 |
| 11 | NOW Q2：AI ACV >$1B、123 笔 >$1M、97% 续约、指引上调 | ServiceNow 新闻稿/电话会 | 7/22 | 高 |
| 12 | NVDA Q2 FY27 $96.22B、DC $89B、Q3 指引 $108B | NVIDIA 新闻稿/Reuters | 8/26 | 高 |
| 13 | GOOGL $195-205B/AMZN ~$220B/META $135-145B、合计 ~$733B、Q2 合计 FCF $7B | CNBC、Mohit Agrawal、Jefferies | 7/28-8 月 | 中 |
| 14 | Citi 2027：GOOGL $308B、META $205B、三家 >$800B | Yahoo Finance/Citi | 7/16 | 中 |
| 15 | Meta/MSFT/Oracle 5 个月发债 $159B；全年 AI 债 $300-570B；Blue Owl SPV 233% 杠杆 | NYT/Vanguard/Tomasz Tunguz | 6-7 月 | 中 |
| 16 | CoreWeave Q2：$2.575B、亏损 $626M、利息 $640M、backlog $104B | CoreWeave IR/CNBC/Yahoo | 8/11 | 高 |
| 17 | H100 合约价 $2.35（3 月，+40% vs 10 月低点）、CDS 未更新 | SemiAnalysis 指数/X | 3-8 月 | 中 |
| 18 | Cursor $4B+（6 月初）/$6B 年末指引/SpaceX $60B 收购 8/14 | Dealroom/TechCrunch/CNBC/Zacks | 6-8 月 | 中（交易待复核） |
| 19 | Cognition $492M、$26B 估值 | Cognition Series D 博客/Sacra | 5/27 | 高 |
| 20 | TP H1：€4,883M/-1.7% LFL、重组上调、指引重申 | TP 新闻稿/CentralCharts | 7/30 | 高 |
| 21 | CNXC 财年 Q2 符合指引、FY26 $9.925-10.025B | Concentrix IR | 6/29 | 高 |
| 22 | Challenger：7 月 AI 连续 5 月居首、前 5 月 87,714、科技业 YTD 149K | Challenger Gray/HR Dive/TradingEconomics | 7-8 月 | 高 |

**未覆盖/待验证**：CoreWeave CDS 最新水位；GitHub Copilot 用户更新；EU AI Act 执法（H4，研究员 C 职责）；SpaceX-Anysphere 交易细节复核；CRM NDR 官方数值（仅有 attrition 代理）。
