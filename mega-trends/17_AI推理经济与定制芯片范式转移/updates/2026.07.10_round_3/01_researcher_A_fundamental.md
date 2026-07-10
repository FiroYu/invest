# 基本面研究员 A | 第三轮研究

> **议题#17：AI推理经济与定制芯片范式转移**
> 研究窗口：2026.06.05 → 2026.07.10（~5周）
> 研究员：基本面研究员 A
> 日期：2026-07-10

---

## 1. Executive Summary

### 方向投票

**维持做多，加仓NVDA/AVGO。**

本轮研究窗口的核心发现是：NVIDIA基本面持续加速（Q2 FY2027指引$91B，+95% YoY），而估值却压缩至2019年以来最低水平（Forward PE 20.4-22.2x，PEG 0.45），创造了Round 2以来显著改善的风险收益比。与此同时，ASIC范式转移加速确认——NVIDIA加速器出货量份额从2022年~95%下降至2026年~62-66%，四大Hyperscaler全部推出或量产自研芯片，验证了子论点1的侵蚀方向。但NVIDIA的收入主导地位通过总算力增长（推理需求爆发）得以维持，形成"份额下降、收入飙升"的结构性窗口。

### 置信度

**高（8/10）** — 较Round 2（7/10）提升一档。估值压缩+基本面加速+ASIC方向确认三重因素提升了核心论点的确定性。但K4（Neocloud/H100价格）逼近触发线、半导体板块整体回调-16%、Hyperscaler金融脆弱性加剧（Alphabet $84.75B股权融资、Oracle负FCF）限制了最高置信度。

### 加权收益 vs Round 2

| 标的 | Round 2加权收益 | Round 3加权收益 | 变化 | 驱动因素 |
|------|----------------|----------------|------|---------|
| NVDA | +10.0% | **+16.8%** | +6.8pp | Forward PE 25.5→20.4x（2019年最低），Q2指引+95%，PEG 0.69→0.45 |
| AVGO | +8.3% | **+10.9%** | +2.6pp | ASIC加速确认（Maia 200/TPU v7/MTIA），Forward PE口径明确24.68x，PEG 0.54 |
| GOOGL | +9.8% | **+9.7%** | -0.1pp | TPU v7 Ironwood GA+Anthropic 3.5GW协议，但基本持平 |
| MRVL | +0.8% | **+8.0%** | +7.2pp | Forward PE 68→42.92x大幅压缩，FY28 $16.5B路径清晰化，但PEG 1.39仍贵 |

> 情景权重调整：Bull 18%（↓2pp）/ Base-bull 37%（↑2pp）/ Base-bear 27%（=）/ Bear 13%（↓2pp）/ Disaster 5%（=）。Base-bull权重提升因NVDA估值洼地+ASIC方向确认。

---

## 2. 假设验证

### 核心假设 H1-H5

| 假设 | Round 2评级 | Round 3评级 | 变化 | 证据 |
|------|------------|------------|------|------|
| **H1** AI推理需求将超过训练，成为主导计算负载 | 通过（高置信） | **通过（高置信↑）** | 维持+强化 | Deloitte确认2026年2/3算力为推理；企业AI预算85%为推理（vs 2023年40%）；Token使用量持续爆发 |
| **H2** 定制ASIC将从NVIDIA夺取推理份额，2027年追平GPU | 有条件通过 | **有条件通过（信心↑）** | 维持+加速 | NVIDIA加速器出货量份额95%→62-66%（2022-2026E）；ASIC服务器+64.2% vs GPU服务器+43.8%；Goldman 2027追平预测在轨 |
| **H3** 推理成本年降~10x驱动AI应用爆发（Jevons悖论） | 通过 | **通过（高置信↑）** | 维持+强化 | Token成本累计降280-600x；企业AI支出$1.2M→$7M（+483%）；推理占AI预算85% |
| **H4** CoWoS封装瓶颈持续至2027H2，TSMC产能扩张缓解 | 有条件通过 | **有条件通过** | 维持 | CoWoS供需缺口20%→~10%（Mizuho上调产能预测），但利用率仍>95%，交期>20周，缓解路径确认 |
| **H5** Hyperscaler CapEx超级周期可持续至2027 | 有条件通过 | **有条件通过（风险↑）** | 维持+风险升 | 2026 CapEx $725B（+77%）；但金融脆弱性加剧——CapEx消耗94%经营现金流+Alphabet $84.75B融资+Oracle负FCF |

### 子论点验证

| 子论点 | Round 2评级 | Round 3评级 | 关键变化 |
|--------|------------|------------|---------|
| **子论点1** NVIDIA推理端份额将被侵蚀 | 有条件通过 | **有条件通过（信心显著提升）** | NVIDIA单位份额从~84%（2024）降至~62-66%（2026E），侵蚀速度超预期。但收入份额仍占主导（总算力增长弥补份额下降）。Microsoft Maia 200量产（10,200 TFLOPS FP4），Google TPU v7 GA（4,614 TFLOPS FP8，TCO比GB200低44%），Meta MTIA 400 9月量产（6 PFLOPS FP8），AWS Trainium 4年底推出（288GB HBM）。Midjourney从NVIDIA切换到TPU v6e节省$16.8M/年。 |
| **子论点2** 推理成本通缩利好AI应用 | 通过 | **通过** | 维持。GPT-4级性能成本从$60/M降至$0.40/M（150-1000x下降）。Jevons悖论确认：单价下降280x，总支出增长320%。推理占AI预算60%→85%。 |
| **子论点3** GPU过剩风险 | 技术关注 | **技术关注（警报↑）** | H100 spot触及$0.79-1.40（接近K4触发线$1.0），on-demand $1.79-3.50。但B200仍紧俏（$2.35-7.00/hr），1年承诺价回升。代际转换正常，全行业过剩概率2027前<20%维持。 |
| **子论点4** CoWoS封装瓶颈投资机会 | 有条件通过 | **有条件通过** | 维持。供需缺口收窄（20%→10%），但利用率>95%、交期>20周、CoPoS下一代2028+。TSMC 2026底月产能~130K片（+80% YoY）。 |

---

## 3. 关键数据更新

| 标的/指标 | Round 2值（06.04） | Round 3值（07.10） | 变化 | 来源 |
|-----------|-------------------|-------------------|------|------|
| **NVDA** Q2 FY2027指引 | $91B（+95% YoY） | 维持$91B指引，8/26财报 | 未变（待验证） | NVIDIA Q1 FY2027财报 |
| **NVDA** Q1 FY2027 DC收入 | $75.2B（+92%） | 维持 | 未变 | NVIDIA财报 |
| **NVDA** TTM收入 | $215.9B（FY2026） | **$253.49B（TTM）** | +17.4% | stockanalysis.com 07/09 |
| **NVDA** TTM净利润 | $120.07B（FY2026） | **$159.61B（TTM）** | +32.9% | stockanalysis.com 07/09 |
| **NVDA** TTM EPS | $4.90（FY2026） | **$6.53（TTM）** | +33.3% | stockanalysis.com 07/09 |
| **NVDA** Forward PE | 25.5x | **20.4-22.2x** | -13~20%（2019年来最低） | stockanalysis/TipRanks/Goldman |
| **NVDA** PEG | 0.69 | **0.45** | -35% | stockanalysis.com |
| **NVDA** EV/EBITDA | N/A | **29.43x** | 新数据 | stockanalysis.com |
| **NVDA** 股价 | ~$222（Round 2入场参考） | **$202.78**（07/09收盘） | -8.7% | NASDAQ |
| **NVDA** 分析师目标价 | N/A | **$309.46**（共识）/ $350（BofA） | +52.7% / +72.5%上行空间 | SharesGrow/TipRanks |
| **NVDA** 52周范围 | N/A | $161.61 - $236.54 | 当前-14.3%从ATH | NASDAQ |
| **AVGO** Forward PE | 待澄清 | **24.68x** | 新明确数据 | stockanalysis.com |
| **AVGO** PEG | N/A | **0.54** | 新数据 | stockanalysis.com |
| **AVGO** AI收入/季 | $8.4B（Q1 FY2026，+106%） | 维持趋势 | 未变 | Broadcom财报 |
| **AVGO** FY27 SAM | $60-90B | 维持 | 未变 | 公司指引 |
| **MRVL** Forward PE | 68x | **42.92-60.61x** | -11~37% | Yahoo Finance |
| **MRVL** PEG | N/A | **1.39** | 新数据，仍>1.0 | Yahoo Finance |
| **MRVL** FY2028指引 | $16.5B | 维持 | 未变 | 公司指引 |
| ASIC服务器出货占比 | 27.8%（+44.6% YoY） | **27.8%（+64.2% YoY加速）** | 增速上调 | TechInsights/Deloitte |
| NVIDIA加速器单位份额 | ~73%（2025） | **~62-66%（2026E）** | -7~11pp | Omdia/JPR |
| Hyperscaler自研ASIC总量 | N/A | **~1.9M加速器**（Google ~900K, AWS ~600K, MSFT ~250K, Meta ~180K） | 新数据 | 行业追踪 |
| CoWoS月产能 | ~130K片（+80% YoY） | 维持，Mizuho上调产能预测 | 缓解确认 | TSMC/Mizuho |
| CoWoS供需缺口 | ~20% | **~10%** | 缓解50% | Mizuho |
| Token成本累计下降 | ~280x（2023-2026） | **~600x**（2020-2026，Tiered Super-Moore论文） | 更新 | arXiv/Epoch AI |
| Token成本年降率 | ~10x/年 | **9x-900x/年**（因任务而异） | 更精确 | Epoch AI |
| 企业AI支出 | $120万→$700万/年 | **$1.2M→$7M**（+483%确认） | 维持 | AnalyticsWeek/FinOps Foundation |
| 推理占AI预算 | ~60% | **85%**（2026） | +25pp | Deloitte/AnalyticsWeek |
| H100租赁价（on-demand） | $1.38-2.69/hr | **$1.79-3.50/hr** | 底部回升 | GridStackHub/gpufinder |
| H100 spot价 | N/A | **$0.79-1.40/hr** | 接近K4触发线 | Vast.ai/Shadeform |
| B200租赁价 | 紧俏，+24% | **$2.35-7.00/hr**（中位~$4.95） | 可用性改善 | GridStackHub/Vultr |
| Hyperscaler 2026 CapEx | ~$700B（+77%） | **$725B**（+77%确认） | 微调 | PIMCO/行业汇总 |
| NVDA财报日期 | N/A | **2026-08-26**（盘后） | 关键催化 | stockanalysis.com |

### API定价快照（07.04-07.09验证）

| 模型 | 输入 $/M | 输出 $/M | 缓存输入 $/M | 趋势 vs 上代 |
|------|---------|---------|------------|-------------|
| GPT-5.5 Pro | $30.00 | $180.00 | N/A | 新增（最贵） |
| GPT-5.5 | $5.00 | $30.00 | $0.50 | ↑ 涨价（vs GPT-5.4 $2.50/$15） |
| Claude Opus 4.8 | $5.00 | $25.00 | $0.50 | 持平 |
| Claude Sonnet 5 | $2.00 | $10.00 | $0.20 | ↓ 降价（vs Sonnet 4.6 $3/$15） |
| Gemini 3 Flash | $0.50 | $3.00 | $0.05 | ↑ 涨价（vs 2.5 Flash $0.30/$2.50） |
| Gemini 2.5 Flash-Lite | $0.10 | $0.40 | $0.01 | 底部定价 |
| DeepSeek V4 Flash | $0.14 | $0.28 | $0.0028 | 开源底部 |
| GPT-5.4 nano | $0.20 | $1.25 | $0.02 | 商品级 |

> 关键洞察：市场正在**双分化**——前沿推理模型定价上涨或持平（"奢侈品"），商品级推理竞相降至零（"廉价品"）。300-600x价差。K5（两家同季降价>50%）未触发——前沿价格反而上涨。

---

## 4. 估值与操作建议

### NVDA — 核心多头（升级）

| 维度 | Round 2 | Round 3 | 变化 |
|------|---------|---------|------|
| 仓位建议 | 25-30% | **25-30%（维持，逢低加仓）** | 维持 |
| Forward PE | 25.5x | **20.4x** | -20%（2019年来最低） |
| PEG | 0.69 | **0.45** | -35% |
| 入场区间 | ~$222 | **$195-210**（当前$202.78，已在区间内） | -8.7%更优入场 |
| 止损 | $175 | **$170**（下移$5，匹配52周低$161.61缓冲） | 微调 |
| 12月目标 | $270-297 | **$280-320**（Base-bull $270 + Bull $350融合） | 上移中位 |
| 分析师共识 | N/A | $309.46（+52.7%上行）/ BofA $350 | 强力支撑 |

**操作逻辑：** NVDA YTD仅+4% vs SOXX +75%，从ATH回调-14%。Forward PE 20.4x为2019年6月以来最低（当时NVDA年收入$11.7B，如今$253B）。Goldman称21.7x"compelling"。Q2 FY2027指引$91B（+95%）若兑现将驱动估值重评。8/26财报是关键催化——若超预期，有望突破$203-210阻力区向$250+进发。建议当前$202附近分批建仓。

### AVGO — ASIC龙头（升级）

| 维度 | Round 2 | Round 3 | 变化 |
|------|---------|---------|------|
| 仓位建议 | 15-20% | **15-20%（维持）** | 维持 |
| Forward PE | 待澄清 | **24.68x** | 口径明确化 |
| PEG | N/A | **0.54** | 新数据，与NVDA接近 |
| 入场区间 | ~$481 | **维持当前水平分批建仓** | - |
| 止损 | N/A | **-15%从入场** | 新设 |
| 12月目标 | N/A | **+20-25%从入场** | 基于PEG+ASIC增长 |

**操作逻辑：** ASIC范式转移加速的最直接受益者。Forward PE 24.68x + PEG 0.54终于给出了清晰合理的估值口径（Round 2的最大不确定性已消除）。Microsoft Maia 200、Google TPU v7/v8、Meta MTIA 400/500、AWS Trainium 3/4均由Broadcom设计或相关。FY27 SAM $60-90B提供收入可见性。Seeking Alpha分析PEG 0.42-0.48仅基于FY26-27增长，未计入FY28加速。

### GOOGL — TPU隐藏期权（维持）

| 维度 | Round 2 | Round 3 | 变化 |
|------|---------|---------|------|
| 仓位建议 | 10-15% | **10-15%（维持）** | 维持 |
| 入场区间 | ~$362 | **维持$350-370区间** | 微调 |
| 止损 | N/A | **$320** | 新设 |
| 12月目标 | N/A | **$400-430** | 基于TPU期权+搜索现金流 |

**操作逻辑：** TPU v7 Ironwood已GA（4,614 TFLOPS FP8，9,216芯片superpod = 42.5 EFLOPS），TCO比GB200低44%。Anthropic协议扩大至2027年3.5GW——Google正从内部工具转变为AI基础设施提供商。第8代TPU已分裂为训练(8t/Broadcom)和推理(8i/MediaTek)，2027末量产，采用TSMC 2nm。搜索广告现金流提供估值保护。

### MRVL — 投机改善（升级但维持谨慎）

| 维度 | Round 2 | Round 3 | 变化 |
|------|---------|---------|------|
| 仓位建议 | 0-5%投机 | **0-5%投机（维持）** | 维持 |
| Forward PE | 68x | **42.92-60.61x** | -11~37% |
| PEG | N/A | **1.39** | 仍>1.0（偏贵） |
| 评估 | 概率加权收益+0.75% | **概率加权收益+8.0%** | 显著改善 |

**操作逻辑：** 估值从极端贵（68x）压缩至偏贵（42.92-60.61x），加权收益从近乎零提升至+8.0%。FY2028 $16.5B指引路径随ASIC加速而更可信。但PEG 1.39仍高于NVDA(0.45)和AVGO(0.54)——在ASIC龙头（AVGO）估值更优的情况下，MRVL仍为可选项而非首选。Celestial AI和XConn收购（6月23日）拓展光互联能力，但整合风险存在。

---

## 5. 情景分析

| 情景 | 概率 | NVDA | AVGO | GOOGL | MRVL | 驱动因素 |
|------|------|------|------|-------|------|---------|
| **Bull** | 18%（↓2pp） | +58%（$320） | +35% | +25% | +45% | Q2超预期+Rubin按时+ASIC收入加速+CapEx 2027继续增长 |
| **Base-bull** | 37%（↑2pp） | +33%（$270） | +22% | +18% | +20% | NVDA维持主导+ASIC份额增+CapEx持续但适度放缓 |
| **Base-bear** | 27%（=） | -1.5%（$200） | +3% | +5% | -5% | ASIC侵蚀加速+CapEx增速放缓+金融压力+ROI质疑 |
| **Bear** | 13%（↓2pp） | -26%（$150） | -20% | -12% | -30% | CapEx逆转>10%+K4触发+Hyperscaler削减 |
| **Disaster** | 5%（=） | -41%（$120） | -35% | -25% | -45% | K4+K5+K8同时触发+AI泡沫破裂 |

### 加权收益

| 标的 | 加权计算 | 加权收益 |
|------|---------|---------|
| NVDA | 0.18×58 + 0.37×33 + 0.27×(-1.5) + 0.13×(-26) + 0.05×(-41) | **+16.8%** |
| AVGO | 0.18×35 + 0.37×22 + 0.27×3 + 0.13×(-20) + 0.05×(-35) | **+10.9%** |
| GOOGL | 0.18×25 + 0.37×18 + 0.27×5 + 0.13×(-12) + 0.05×(-25) | **+9.7%** |
| MRVL | 0.18×45 + 0.37×20 + 0.27×(-5) + 0.13×(-30) + 0.05×(-45) | **+8.0%** |

### 黑天鹅风险

1. **NVIDIA Kyber NVL144延迟**（已部分price-in）：7月有传言称Kyber NVL144延迟至2028，NVDA已否认。若后续证实，将严重影响Rubin放量时间线。
2. **DeepSeek效应重演**：DSpark推理模块据称提升85%推理速度而无需新硬件——若开源推理效率突破使现有GPU算力过剩，将触发K3/K4。
3. **半导体板块系统性回调**：SOXX从ATH回调-16%，Burry做空半导体。若DRAM/NAND周期见顶信号传导至AI芯片，可能形成板块级踩踏。
4. **Hyperscaler联合自研**：若Google+AWS+Microsoft+Meta联合开源ASIC设计或共享制造产能，将系统性削弱Broadcom+NVIDIA的定价权。

---

## 6. 退场标准触发状态

| 编号 | 标准 | 触发条件 | Round 3状态 | 详情 |
|------|------|---------|------------|------|
| **K1** | 核心逻辑失效 | ASIC份额连续2Q停滞/下降 | **未触发** ✅ | ASIC加速器出货+64.2%，GPU服务器+43.8%。份额侵蚀方向确认且加速。NVIDIA单位份额95%→62-66%。 |
| **K2** | CapEx周期逆转 | Hyperscaler削减AI CapEx>10% | **未触发** ⚠️（风险升） | 2026 CapEx $725B（+77%）。但金融脆弱性加剧：CapEx消耗94%经营现金流；Alphabet $84.75B股权融资（历史最大科技融资之一）；Oracle负FCF。2027指引是关键验证。 |
| **K3** | 技术替代 | 光计算/模拟计算/LPU商用突破 | **未触发** | Groq LPU在推理加速领域获得关注（GPT-OSS 120B 500 tps），但非NVIDIA替代品。FuriosaAI进入欧洲数据中心但属利基。 |
| **K4** | Neocloud信用风险 | CoreWeave违约或H100<$1.0/hr | **逼近触发** 🟡 | H100 spot在Vast.ai/Shadeform低至$0.79-1.40，已触及$1.0阈值低端。但on-demand底部$1.79，1年承诺价回升。CoreWeave未违约。**代际转换型过剩（Hopper退役），非全行业过剩。需密切监控。** |
| **K5** | API定价战 | 任两家同季API降价>50% | **未触发** ✅ | 市场双分化：前沿涨价（GPT-5.5从$2.50→$5.00输入，翻倍），商品级趋零（DeepSeek $0.14）。Anthropic Sonnet 5降价33%（$3→$2），但未达>50%。无两家同季>50%降价。 |
| **K6** | NVIDIA收入减速 | DC增速连续2Q<30%或环比下降 | **未触发** ✅ | Q1 FY2027 +92% YoY，Q2指引+95% YoY——**加速而非减速**。TTM收入$253B。 |
| **K7** | CoWoS利用率下降 | 利用率<85%或交期<3个月 | **未触发** ✅ | 利用率仍>95%，交期>20周。但供需缺口从~20%收窄至~10%，Mizuho上调产能预测。缓解方向确认。 |
| **K8** | AI应用ROI失败 | F500 AI预算连续2Q下降或AI融资>30%降幅 | **未触发** ⚠️ | 企业AI支出$7M/年（+483%）。但ROI仍存疑（Round 2记录仅23%有可衡量ROI）。推理占预算85%。需关注是否转化为可持续收入。 |

### K4 专项深度分析

K4是当前最值得关注的退场标准。H100 spot在市场化云（Vast.ai, Shadeform）已触及$0.79-1.40，低端突破了$1.0阈值。但需要区分三个层次：

1. **Spot市场（最波动）**：$0.79-1.40 — 受加密货币挖矿需求波动、突发性供给涌入影响
2. **On-demand（按需）**：$1.79-3.50 — 专业GPU云（Lambda, CoreWeave, RunPod）底部$1.79-2.40，超大规模云（AWS, GCP）$12+
3. **1年承诺价**：趋势上升 — 长期需求仍稳固

**判断**：K4的"CoreWeave违约或H100<$1.0"中，spot短暂触及$0.79属于市场化云的瞬时信号，不等于结构性触发。on-demand底部$1.79仍高于$1.0阈值。1年承诺价上升说明核心需求未崩。但若on-demand跌破$1.5且CoreWeave出现债务重组信号，将正式触发K4。

**建议**：将K4细化为"H100 on-demand中位价<$1.5/hr（持续2周）或CoreWeave债务违约/重组"作为更精确的触发条件。

---

## 7. 时间维度

| 时间窗口 | 关键事件/催化 | 影响评估 |
|---------|-------------|---------|
| **2026.07-08** | 半导体板块回调（-16%从ATH），NVDA回调-14%。夏季低波动期。 | 短期噪声，创造入场窗口。 |
| **2026.08.26** | **NVIDIA Q2 FY2027财报**（盘后） | **关键催化**。市场预期收入~$393B年化。若Q2超$91B指引+Q3指引强→验证加速 thesis；若低于指引或Q3 guidance疲软→触发回调。 |
| **2026.09** | Meta MTIA 400量产；Broadcom Q3 FY2026财报 | ASIC收入确认。AVGO AI收入是否维持$8-9B/季趋势。 |
| **2026.Q4** | AWS Trainium 4推出；Microsoft Maia 200扩大部署；NVDA Rubin量产准备 | ASIC vs GPU竞争白热化。Rubin是否能按计划H2 FY2027（2027年1-7月）量产。 |
| **2026.11-12** | Hyperscaler 2027 CapEx指引发布 | **K2验证窗口**。若2家以上下调>20%将触发系统性减仓。目前市场预期2027继续增长但增速放缓。 |
| **2027.H1** | NVIDIA Rubin架构量产；CoWoS产能进一步释放 | Rubin 10x throughput-per-watt。若兑现将重新拉开GPU vs ASIC性能差距。CoWoS缺口预计<5%。 |
| **2027.H2** | CoWoS可能开始缓解；CoPoS下一代封装试产 | K7可能开始接近触发（利用率下降）。但CoPoS 2028+量产意味着先进封装瓶颈长期化。 |

---

## 8. 盲点

1. **NVDA收入份额 vs 单位份额背离的可持续性**：NVIDIA单位份额从95%降至62-66%，但收入仍+95% YoY。这一"份额下降、收入飙升"的窗口能持续多久？若ASIC性能追平（Google TPU v7 TCO比GB200低44%），价格竞争将从单位扩展到收入。当前分析低估了ASIC对NVIDIA定价权的侵蚀速度。

2. **Token定价的"奢侈品/廉价品"双分化是否可持续**：GPT-5.5涨价而DeepSeek趋零。若开源模型（DeepSeek V4、Llama 4）性能持续追赶前沿，前沿溢价将被压缩。Epoch AI的"Tiered Super-Moore"论文显示经济型模型价格半衰期1.10年，中端1.55年，但前沿模型R²=0.031（近乎零指数拟合）——前沿定价能否维持是最大不确定性。

3. **推理成本下降的驱动力构成**：arXiv论文显示总要素生产率（软件/架构创新）贡献了103.7%的成本下降，GPU硬件贡献-0.9%（即硬件变贵了）。这意味着：若软件优化触及天花板（MLPerf v5.1 vs v5.0改善已从30-50%收窄），推理成本下降可能急剧放缓。Presenc AI预测2025-2027降至3-5x/年（vs 2021-2025的10x/年），2027+降至1.5-2x/年。

4. **Hyperscaler自研芯片的真实成本优势**：Google声称TPU v7 TCO比GB200低44%，Midjourney切换到TPU节省$16.8M/年。但这些都是理想条件下的数据。实际部署中的迁移成本、生态锁定（CUDA）、模型兼容性、人才稀缺性可能大幅削弱成本优势。Broadcom设计的ASIC有18-24月的设计-流片-量产周期，存在技术迭代风险。

5. **中国因素**：DSpark推理模块据称提升85%速度无需新硬件。若中国开源推理优化（类似DeepSeek效应）持续突破，可能改变全球推理经济学。H200对华出口限制的反复（允许→AI Overwatch Act可能撤销）增加了供应链不确定性。

6. **半导体板块回调的信号意义**：SOXX -16%从ATH，Burry做空。是健康轮动还是周期见顶信号？DRAM/NAND制造商近期回调更剧烈——若存储周期见顶传导至AI芯片，可能形成板块级压力。NVDA YTD +4% vs SOXX +75%的巨大落后，可能是市场在price in ASIC侵蚀风险。

---

## 9. 来源列表

### NVIDIA估值与基本面
1. stockanalysis.com — NVDA Statistics & Valuation（07/09收盘$202.78，Forward PE 20.40，PEG 0.45，市值$4.91T）https://stockanalysis.com/stocks/nvda/statistics/
2. TipRanks — "Nvidia Stock Price Forecast: Is It a Buy Now as Valuation Hits Lowest Level Since 2019?"（07/09）https://www.tipranks.com/news/nvidia-stock-price-forecast-is-it-a-buy-now-as-valuation-hits-lowest-level-since-2019
3. Simply Wall St — NVIDIA Valuation（Forward PE 29.7x trailing，同行均值87.9x）https://simplywall.st/stocks/us/semiconductors/nasdaq-nvda/nvidia/valuation
4. SharesGrow — NVDA Valuation & Earnings（Forward PE 21.8，PEG 0.48，分析师目标$309.46）https://sharesgrow.com/valuation/NVDA/
5. TradingKey — "Goldman Says 21.7x Is Compelling After Kyber Delay Denied"（07/07）https://www.tradingkey.com/analysis/stocks/us-stocks/262015350-nvidia-nvda-stock-forecast-july-2026-kyber-denial-goldman-tradingkey
6. 24/7 Wall St — "Here's Why Nvidia Might Be the New Value Play"（07/08，YTD +4% vs SOXX +75%，Forward PE 22.2x）https://247wallst.com/investing/2026/07/08/heres-why-nvidia-might-be-the-new-value-play-in-semiconductors/
7. Yahoo Finance/Zacks — "NVIDIA Valuation Falls to Multi-Year Low"（Forward PE 22.22x，2019年6月以来最低）https://nz.finance.yahoo.com/news/nvidia-valuation-falls-multi-low-160000298.html
8. MarketScreener — NVIDIA Valuation Ratios（FY2027E P/E 21.7x，FY2028E 15.7x）https://www.marketscreener.com/quote/stock/NVIDIA-CORPORATION-57355629/valuation/
9. Motley Fool — "Is Nvidia Stock Too Cheap to Ignore?"（07/09，16x FY2028E盈利）https://www.fool.com/investing/2026/07/09/is-nvidia-stock-too-cheap-to-ignore-right-now/

### Broadcom/Marvell估值
10. stockanalysis.com — AVGO Statistics（Forward PE 24.68，PEG 0.54）https://stockanalysis.com/stocks/avgo/statistics/
11. GuruFocus — AVGO Summary（Forward PE 20.36，PEG 2.5不同方法）https://www.gurufocus.com/stock/AVGO/summary
12. Seeking Alpha — "Broadcom: Multi-Year Growth Visibility At ~0.5x PEG"（Forward PE 27.72x，PEG 0.42-0.48）https://seekingalpha.com/article/4888461-broadcom-multi-year-growth-visibility-for-sale-at-0-5x-peg
13. Yahoo Finance — MRVL Key Statistics（Forward PE 42.92-60.61，PEG 1.39）https://finance.yahoo.com/quote/MRVL/key-statistics/
14. Macrotrends — MRVL PE Ratio（97.77 trailing，07/09）https://www.macrotrends.net/stocks/charts/MRVL/marvell-technology/pe-ratio

### ASIC/自研芯片进展
15. Microsoft Maia 200发布（10,200 TFLOPS FP4，5,000 TFLOPS FP8，216GB HBM3E，750W）— 行业报道
16. Google TPU v7 Ironwood GA（Cloud Next 04/22，4,614 TFLOPS FP8，192GB HBM3E，TCO比GB200低44%，Anthropic 3.5GW协议）
17. AWS Trainium 3（2,517 PFLOPS FP8，UltraServer 144芯片）+ Trainium 4（年底，288GB HBM，NVLink Fusion）— Digitimes 07/06 Q3出货量上调
18. Meta MTIA 400/500（TechCrunch 07/09，Broadcom设计，TSMC制造，400 9月量产6 PFLOPS FP8，500 2027年10 PFLOPS FP8）
19. Google第8代TPU分裂：TPU 8t（Sunfish/Broadcom/训练）+ TPU 8i（Zebrafish/MediaTek/推理），TSMC 2nm，2027末
20. NVIDIA加速器单位份额追踪：2022 ~95% → 2023 ~92% → 2024 ~84% → 2025 ~73% → 2026E ~62-66% — Omdia/JPR
21. Midjourney从NVIDIA切换到TPU v6e：月费从$2.1M降至$700K（年省$16.8M）— 行业报道

### GPU租赁价格
22. GridStackHub — H100 vs B200 Cost Comparison（07/09，H100 $1.79/hr起，B200 $2.35/hr起）https://gridstackhub.ai/comparison/h100-vs-b200-cost
23. gpufinder.dev — B200 Cloud Pricing（07/09，11家供应商，$3.44-$160.28/hr）https://gpufinder.dev/gpu/b200
24. GridStackHub — GPU Pulse Stack（B200中位~$4.95/hr，H100 spot $0.79-1.40）https://gridstackhub.ai/gpu-pulse-stack

### LLM API定价
25. TLDL — LLM API Pricing July 2026（23个验证模型，07/04更新）https://www.tldl.io/resources/llm-api-pricing-2026
26. Developers Digest — Frontier Model API Pricing June 2026（GPT-5.5 vs Claude vs Gemini vs DeepSeek，643x价差）https://www.developersdigest.tech/blog/frontier-model-api-pricing-june-2026
27. BenchLM.ai — LLM Pricing Comparison（07/09，Score/$排名）https://benchlm.ai/llm-pricing
28. The Register — "AI is becoming a bargain hunter's market"（07/08，双分化趋势，前沿涨价vs商品趋零）https://www.theregister.com/ai-and-ml/2026/07/08/ai-is-becoming-a-bargain-hunters-market-with-a-few-luxury-models-on-top/5268050

### 推理经济学/Token成本
29. Epoch AI — LLM Inference Price Trends（9x-900x/年，因任务而异）https://epoch.ai/data-insights/llm-inference-price-trends
30. arXiv — "Tiered Super-Moore's Law"（600倍下降，经济型半衰期1.10年，软件贡献103.7%）https://arxiv.org/html/2603.28576v1
31. tianpan.co — "The Inference Cost Paradox"（Jevons悖论：成本降1000x，支出增320%）https://tianpan.co/blog/2026-04-14-the-inference-cost-paradox
32. Oplexa — "AI Inference Cost Crisis 2026"（推理占AI预算85%，企业$7M/年）https://oplexa.com/ai-inference-cost-crisis-2026/
33. Presenc AI — Inference Cost Trajectory 2022-2026（10x/年→3-5x/年→1.5-2x/年预测）https://presenc.ai/research/ai-inference-cost-trajectory-2022-2026

### CoWoS/HBM（Round 2数据维持，Mizuho产能上调）
34. Mizuho Securities — CoWoS产能预测上调（2026底~130K片/月，供需缺口20%→10%）— Round 2引用+本轮确认

---

*研究员A | 基本面研究 | 2026-07-10*
*等待CIO综合（_synthesis.md）整合研究员B/C/D观点*
