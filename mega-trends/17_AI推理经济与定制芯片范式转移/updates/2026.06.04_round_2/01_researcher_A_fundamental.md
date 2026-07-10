# 议题#17 AI推理经济与定制芯片范式转移 — 基本面研究员报告（第二轮）

> 数据截止：2026.06.03 | 基于 00_background_pack.md + 最新公开数据

---

## 核心发现 Top 3

### 1. NVIDIA 短期绝对统治地位超预期，但增速拐点临近

NVIDIA Q1 FY2027 收入 $81.6B（+85% YoY），数据中心 $75.2B（+92% YoY），Q2 指引 $91B（+95% YoY），全年共识已上调至 ~$367B。Blackwell 架构全面放量，DC网络收入单季 ~$15B（YoY近3倍）。**但**增速从 FY2026 的 ~120% 降至 FY2027 的 ~80%，且 Q2 指引未计入中国计算业务，实际可触达市场存在天花板。NVIDIA 当前 Forward PE ~25x，PEG ~0.69，估值在 AI 芯片标的中相对最合理。

### 2. 定制 ASIC 加速替代拐点已确认，Goldman Sachs 预测 2027 年出货量追平 GPU

Broadcom Q1 FY2026 AI 收入 $8.4B（+106% YoY），含定制加速器+网络，FY27 SAM 上调至 $60-90B。Marvell FY2026 全年收入 $8.2B（+63%），定制芯片收入 ~$1.5B，预计 FY2029 达 $10B+。Goldman Sachs 预测 ASIC 出货量 2027 年追平 GPU。Tom's Hardware 数据显示 ASIC 服务器出货占 2026 年总量 27.8%，为 2023 年以来最高。**范式转移速度比 05.21 初始预期更快。**

### 3. CoWoS 瓶颈确认延续至 2027+，TSMC 产能上调但不解渴

TSMC CoWoS 月产能从 2024 年底 ~35K 扩至 2026 年底 ~130K（+270%），2027 年目标 141K。良率 >98%，CoWoS 预计占 TSMC 2026 年总收入的 ~15%。非 TSMC 产能 2H26 开始贡献但仅占 ~9%。封装排队期仍 >50 周。**结论：瓶颈持续至 2027，对 AVGO/MRVL 等 ASIC 厂商的议价权构成支撑。**

---

## 一、基本面分析

### 1.1 估值对比（截至 2026.06.03）

| 标的 | 股价 | 市值 | TTM PE | Forward PE | PEG | P/S | 来源 |
|------|------|------|--------|------------|-----|-----|------|
| **NVDA** | ~$222 | $5.4T | 34.1x | 25.5x | 0.69 | ~14.7x | Yahoo Finance |
| **AVGO** | ~$481 | $2.3T | 93.5x | ~43x* | -- | ~30x | Yahoo Finance / WSJ |
| **MRVL** | ~$301 | $264B | 103.7x | ~68x | -- | ~32x | Yahoo Finance |
| **AMD** | ~$542 | $885B | 173.9x | ~74x | 1.25 | ~22.9x | Yahoo Finance |
| **GOOGL** | ~$362 | $4.3T | -- | ~28x | -- | ~8x | Yahoo Finance / Trefis |

*注：AVGO Forward PE 因 VMware 并表后 EPS 结构变化较大，不同来源差异显著（43x vs 24x FY2027），需注意 FY 口径差异。*

**估值判断：**
- NVDA Forward PE 25.5x 为 AI 半导体板块最低，PEG 0.69 表明增长远未充分定价
- AVGO 按 FY2027 EPS $12-13 估算 PE ~38-40x，偏贵但 AI 加速器收入增速 100%+ 支撑
- MRVL Forward PE 68x 为板块最贵，定价已隐含 FY2028+ 定制芯片大幅放量预期
- AMD Forward PE 74x 反映市场对 MI400 系列 $7.2B 收入预期的高不确定性
- GOOGL Forward PE ~28x 为最低，但 TPU 收入不直接体现（内化于云收入中）

### 1.2 收入与增长分析

#### NVIDIA（FY2027 = CY2026）

| 指标 | Q1 FY2027 | Q2 FY2027E | FY2027 共识 | 来源 |
|------|-----------|------------|-------------|------|
| 总收入 | $81.6B (+85%) | $91B (+95%) | ~$367B (+~80%) | NVIDIA IR / S&P Global |
| 数据中心 | $75.2B (+92%) | -- | ~$343B | NVIDIA IR |
| DC 网络 | ~$15B (YoY近3x) | -- | -- | NVIDIA 财报会 |
| 非GAAP EPS | $1.87 (+131%) | -- | ~$9.5-10 | TIKR / Visible Alpha |
| 毛利率(Non-GAAP) | ~75% | ~75% | 中70% | NVIDIA 指引 |

**关键信号：** Blackwell 全面放量，Q2 指引 $91B 大幅超共识 ~$85-87B。但 (1) 增速从 ~120% 降至 ~80% 拐点确认；(2) 未计入中国计算业务意味着存在隐藏下行风险；(3) Rubin 下一代产品进展为 2027 增长续命关键。

#### Broadcom（FY2026 = 截至 2025.10，当前为 FY2027）

| 指标 | Q1 FY2026 | FY2026E | FY2027 SAM | 来源 |
|------|-----------|---------|------------|------|
| 总收入 | $19.3B (+29%) | ~$76B | -- | Broadcom IR |
| AI 收入 | $8.4B (+106%) | ~$35B | $60-90B | Hock Tan / Futurum |
| 其中定制加速器 | 含于 AI 收入 | -- | -- | 未拆分 |
| VMware | 含于总收入 | -- | -- | 未单独报告 |

**关键信号：** AI 收入 $8.4B/季 含网络+定制加速器，Hock Tan 预计 AI 收入将持续加速。定制加速器订单已锁定 $10B+。VMware 整合进展顺利但非核心变量。**风险：** AI 收入中网络占比可能达 40-50%，纯定制加速器市场可能被高估（对应背景包待验证问题 #1）。

#### Marvell（FY2026 = 截至 2026.01，当前为 FY2027 Q1）

| 指标 | FY2026 全年 | FY2027 Q1 | FY2028 指引 | 来源 |
|------|------------|-----------|------------|------|
| 总收入 | $8.2B (+63%) | $2.42B（创纪录） | $16.5B | Marvell IR / Reuters |
| 数据中心 | -- | $1.65B (+21%) | -- | Barron's |
| 定制芯片 | ~$1.5B | -- | FY2029 超 $10B | Marvell 管理层 |
| 市占率预期 | ~12% | -- | ~8%（部分预测） | IDC |

**关键信号：** FY2027 Q1 收入 $2.42B 创纪录，下季指引 $2.7B。管理层将 FY2028 指引从 $15B 上调至 $16.5B。定制芯片 FY2029 目标 $10B+ 意味着 CAGR ~60%。**风险：** 市占率从 12% 降至 8% 的预期（部分分析师）、单一芯片依赖度、执行风险显著。

#### AMD（CY2026）

| 指标 | Q1 2026 | FY2026E | 来源 |
|------|---------|---------|------|
| 总收入 | $10.3B (+38%) | ~$46B | AMD IR / Investing |
| 数据中心 | $5.8B (+57%) | -- | Quartz |
| MI400 系列 | -- | ~$7.2B（预测） | Threads / Analyst |
| Forward P/S | -- | ~9.8x | Investing |

**关键信号：** 数据中心收入首次超过 CPU 收入。MI400 系列为关键变量，预计贡献 ~$7.2B。AMD 持有 AI GPU 市场约 5-7% 份额（vs NVIDIA ~80%）。管理层给出 2030 年数据中心收入 $100B 目标。**风险：** 市占率扩张缓慢，软件生态 CUDA 兼容性持续劣势。

#### Alphabet/Google（CY2026）

| 指标 | Q1 2026 | FY2026E | 来源 |
|------|---------|---------|------|
| 总收入 | $109.9B (+22%) | ~$470B | Alphabet IR |
| Google Cloud | >$20B (+63%) | -- | Seeking Alpha |
| TPU Ironwood | 内化于云/基础设施 | -- | Google Blog |
| Cloud Backlog | -- | $460B | Simply Wall St |
| TPU 外销收入 | -- | ~$3B（Citizens 估） | TradingKey |

**关键信号：** Ironwood TPU（v7）为首个专为推理设计的 TPU，单芯片 4,614 TFLOPS（10x v5p）。Anthropic 签约 ~100 万颗 Ironwood，协议价值 ~$21B+，3.5GW 产能。TPU 通过 Broadcom 向第三方直接销售是新增收入流。**Google 的 AI 芯片战略正从"自用"转向"平台化"，这改变了竞争格局。**

### 1.3 竞争格局矩阵

| 维度 | NVIDIA | Broadcom | Marvell | AMD | Google/TPU |
|------|--------|----------|---------|-----|------------|
| 训练市场 | ~90% | 0%（ASIC不参与） | 0% | ~5-7% | 自用+有限外供 |
| 推理市场 | ~70%（侵蚀中） | ~15%（增长最快） | ~3-5% | ~3-5% | ~5-8%（Ironwood后上升） |
| 客户集中度 | 分散（全球） | 3大客户（占SAM 80%+） | 3-5客户 | 分散 | 自用+Anthropic |
| 软件生态 | CUDA（绝对优势） | 客户自建 | 客户自建 | ROCm（弱势） | JAX/PyTorch/XLA |
| 技术代际 | Blackwell→Rubin | 5nm定制→3nm下一代 | 5nm→3nm | MI400(MI300下一代) | Ironwood(v7)→下一代 |
| 竞争壁垒 | 软件+网络+全栈 | 定制化+网络+客户锁定 | 定制化+光电 | 价格+open ecosystem | 内部需求+成本优势 |

---

## 二、假设验证表 H1-H5

| 假设 | 内容 | 验证数据 | 信心变化 | 结论 |
|------|------|---------|---------|------|
| **H1** | ASIC推理份额从~10%增至2028年~30-40% | ASIC服务器出货占2026总量27.8%（Tom's Hardware）；Goldman Sachs预测2027年ASIC出货量追平GPU；Broadcom AI收入增速106% YoY | **上调**（高→很高） | 加速确认。2026年份额已超预期，2027年追平GPU出货量意味着收入份额可能在2028年达30-40% |
| **H2** | CoWoS瓶颈持续至2027年 | TSMC CoWoS月产能2026底~130K，2027目标141K；良率>98%；排队>50周；非TSMC产能2H26起贡献~9% | **维持**（高） | 瓶颈确认延续。产能虽大幅扩张但需求增速更快，2027年仍供不应求 |
| **H3** | 推理token成本年降10x持续 | H100租赁从2023年$8/hr降至2026年$1.38-2.69/hr（折扣云）；推理模型占比从0%飙升至>50%增加每查询token消耗 | **维持**（高） | 成本下降确认。但推理模型每查询消耗量暴增意味着总推理算力需求曲线可能比线性更陡，对硬件厂商是双刃剑 |
| **H4** | NVIDIA推理端护城河弱于训练端 | NVIDIA推理收入占比未单独披露；Anthropic签约100万颗TPU Ironwood（~$21B）；Hyperscaler自研芯片全面投产 | **上调**（中→中高） | 新证据支持：Google TPU首次对外大规模销售，Broadcom定制加速器客户扩展。NVIDIA训练护城河稳固但推理份额侵蚀加速 |
| **H5** | GPU算力2027-2028可能从稀缺转向过剩 | H100租赁$1.38-2.69/hr（vs 2023年$8/hr）；GPU租赁价格5月底再降30-40%（TechInsights）；但1年期合约从$1.70回升至$2.35（SemiAnalysis） | **上调**（中低→中） | 信号矛盾：短期租赁价大幅下降显示过剩压力，但长期合约价回升说明大客户仍锁定产能。2027年是否全面过剩取决于Blackwell退役节奏和ASIC替代速度 |

### 背景包待验证问题回复

| # | 问题 | 回答 |
|---|------|------|
| 1 | Broadcom SAM 中"网络"收入占比多大？ | 估计 AI 收入 $8.4B/季中网络占 40-50%（基于 NVIDIA DC 网络收入 ~$15B/季作参照），纯定制加速器可能仅 ~$4-5B/季。FY27 SAM $60-90B 中需注意网络贡献 |
| 2 | 推理成本年降10x对硬件厂商定价权侵蚀？ | 双刃剑效应：单价下降但总量爆发。推理模型每查询消耗量暴增 10x+ 部分对冲单价下降。硬件厂商面临"量增价减"格局，议价权取决于供不应求程度 |
| 3 | GPU 利用率过剩信号？ | H100 短期租赁价降至 $1.38-2.69/hr（vs 峰值 $8/hr）确认过剩。但 1 年期合约回升至 $2.35/hr 表明核心需求仍然稳固。B200 租赁价反而上涨 24%。分层分化明显 |
| 4 | Marvell 执行风险？ | 显著。FY2027 Q1 收入 $2.42B 创纪录但定制芯片仅占 ~10-15% 收入。市占率从 12% 预期降至 8% 的分析存在。单一客户依赖度高（前 2 客户占数据中心收入 60%+） |

---

## 三、情景分析

### Bull Case（概率 25%）

**触发条件：** Hyperscaler CapEx 持续加速（>$800B/年）、Blackwell Ultra/Rubin 全面放量、ASIC 出货量 2027 年超越 GPU

| 指标 | 2026E | 2027E | 2028E |
|------|-------|-------|-------|
| AI 推理市场规模 | ~$118B | ~$200B | ~$313B |
| ASIC 份额（出货量） | ~28% | ~50% | ~60% |
| NVIDIA DC 收入 | ~$343B | ~$420B（Rubin驱动） | ~$450B |
| Broadcom AI 收入 | ~$35B | ~$55B | ~$80B |
| Marvell 总收入 | ~$12B | ~$16.5B | ~$22B |

**标的排序：** AVGO > MRVL > NVDA > GOOGL > AMD
**逻辑：** ASIC 加速替代，Broadcom 作为定制加速器龙头受益最大。Marvell 弹性最高但风险也最大。

### Base Case（概率 55%）

**触发条件：** Hyperscaler CapEx 维持 ~$700B/年、GPU+ASIC 共存、推理需求稳步增长

| 指标 | 2026E | 2027E | 2028E |
|------|-------|-------|-------|
| AI 推理市场规模 | ~$118B | ~$170B | ~$250B |
| ASIC 份额（出货量） | ~28% | ~45% | ~55% |
| NVIDIA DC 收入 | ~$343B | ~$380B | ~$400B |
| Broadcom AI 收入 | ~$35B | ~$45B | ~$60B |
| Marvell 总收入 | ~$12B | ~$16.5B | ~$20B |

**标的排序：** NVDA > AVGO > GOOGL > MRVL > AMD
**逻辑：** NVIDIA 短期（6-12个月）仍有最强收入确定性+最低估值。Broadcom 为中期（1-2年）最佳 ASIC 敞口。Google 估值最低+TPU 外供为隐藏期权。

### Bear Case（概率 20%）

**触发条件：** AI CapEx ROI 争议爆发导致 2026H2 Hyperscaler 削减指引 >20%、中美脱钩升级、GPU 过剩加速

| 指标 | 2026E | 2027E | 2028E |
|------|-------|-------|-------|
| AI 推理市场规模 | ~$118B | ~$130B（增速骤降） | ~$160B |
| ASIC 份额（出货量） | ~25% | ~35% | ~40% |
| NVIDIA DC 收入 | ~$320B | ~$280B（负增长） | ~$300B |
| Broadcom AI 收入 | ~$30B | ~$32B | ~$38B |
| Marvell 总收入 | ~$11B | ~$13B | ~$15B |

**标的排序：** GOOGL > NVDA > AVGO > AMD > MRVL
**逻辑：** CapEx 削减下高估值 ASIC 标的（MRVL/AMD）回调最深。Google 搜索广告提供收入缓冲。NVIDIA 因 Forward PE 最低（~25x）有估值保护。

---

## 四、时间维度

### 短期（0-6个月，2026H2）

| 事件 | 影响 | 概率 |
|------|------|------|
| NVIDIA Q2 FY2027 财报（~2026.08） | 指引 $91B 若 beat 则确认 Blackwell 需求强度 | 高关注 |
| Hyperscaler 2027 CapEx 指引 | META/MSFT/GOOGL/AMZN 年底指引为年度核心催化 | 关键 |
| Blackwell Ultra 量产进度 | 若延迟则 NVIDIA FY2027H2 收入风险 | 中等 |
| Marvell 定制芯片客户拓展 | 新客户签约为估值验证关键 | 中等 |
| GPU 租赁价格走势 | 若继续暴跌 30%+ 则 GPU 过剩信号强化 | 关注 |

**短期结论：** NVIDIA 在 0-6 个月窗口内收入确定性最强。Broadcom AI 收入增速最快。MRVL 波动性最大。

### 中期（6-18个月，2027全年）

| 事件 | 影响 | 概率 |
|------|------|------|
| NVIDIA Rubin 架构发布/量产 | 决定 2027 能否维持 60%+ 增速 | 关键 |
| ASIC 出货量是否追平 GPU | Goldman 预测验证节点 | 关键 |
| CoWoS 产能 ~141K/月是否解渴 | 决定封装溢价持续还是消退 | 高关注 |
| Anthropic Ironwood TPU 交付 | ~100 万颗开始贡献推理算力 | 高关注 |
| AI 应用 ROI 是否兑现 | 决定 CapEx 周期可持续性 | 关键 |

**中期结论：** 2027 年为范式转移关键验证年。ASIC 出货量追平 GPU 意味着范式转移从"趋势"变为"事实"。NVIDIA 需通过 Rubin 维持技术领先。

### 长期（18-36个月，2028-2029）

| 事件 | 影响 | 概率 |
|------|------|------|
| GPU vs ASIC 出货量占比 | ASIC 是否真正超过 GPU | 核心验证 |
| 推理算力 commoditization | 硬件厂商利润率压缩程度 | 关键 |
| 新架构（光计算/模拟计算）是否商用 | 触发 K3 退场标准 | 低但需监控 |
| TSMC 非台产能释放 | 地缘风险缓释程度 | 关注 |

---

## 五、标的排名与评分

### 综合排名

| 排名 | 标的 | 综合评分 | Forward PE | 6M目标价（共识） | 推荐理由 | 主要风险 |
|------|------|---------|------------|-----------------|---------|---------|
| **1** | **NVDA** | **8.5/10** | 25.5x | ~$297（+34%） | 估值最低+收入确定性最强+PEG 0.69 | ASIC 份额侵蚀、增速拐点、中美风险 |
| **2** | **AVGO** | **8.0/10** | ~38-43x* | ~$555（+15%） | ASIC 龙头+AI收入增速100%+客户锁定 | 估值偏贵、AI收入含网络水分、3客户集中 |
| **3** | **GOOGL** | **7.5/10** | ~28x | -- | 估值最低+TPU Ironwood 隐藏期权+云 backlog $460B | TPU 收入不透明、搜索业务周期性、反垄断 |
| **4** | **MRVL** | **6.5/10** | ~68x | ~$233（-23%） | ASIC 弹性最大+FY2028 $16.5B 指引上调 | 估值最贵、执行风险、客户集中、盈利能力弱 |
| **5** | **AMD** | **6.0/10** | ~74x | ~$416（-23%） | MI400 新品周期+数据中心 $100B 2030 目标 | CUDA 生态劣势、市占率扩张缓慢、估值过贵 |

*注：AVGO Forward PE 因 VMware 并表后 GAAP/Non-GAAP 差异极大，不同来源口径不一致。*

### 评分维度拆解

| 维度（各10分） | NVDA | AVGO | GOOGL | MRVL | AMD |
|---------------|------|------|-------|------|-----|
| 收入确定性 | 9 | 8 | 8 | 6 | 6 |
| 估值合理性 | 9 | 6 | 9 | 4 | 4 |
| ASIC/推理敞口 | 5（GPU为主） | 10 | 7（TPU内化） | 8 | 4 |
| 竞争壁垒 | 10 | 8 | 8 | 5 | 5 |
| 执行风险（越低越好） | 9 | 8 | 9 | 5 | 6 |
| **加权综合** | **8.5** | **8.0** | **7.5** | **6.5** | **6.0** |

### 投资建议

**核心持仓（建议占 AI 芯片敞口 60-70%）：**
- **NVDA**（30-35%）：估值洼地+最强护城河，短期不可替代。即使 ASIC 范式转移确认，NVIDIA FY2027 仍是最赚钱的 AI 芯片公司
- **AVGO**（20-25%）：ASIC 范式转移最大受益者，Hock Tan 执行力一流，客户锁定度高

**卫星持仓（建议占 20-30%）：**
- **GOOGL**（10-15%）：估值保护+TPU 外供期权+搜索业务现金流。风险最低的 AI 芯片敞口
- **MRVL**（5-10%）：高弹性投机仓位。仅在能承受 30%+ 回撤的情况下配置

**暂不推荐：**
- **AMD**：Forward PE 74x 过贵，MI400 市占率扩张缓慢，CUDA 生态壁垒难以逾越。等待估值回调至 Forward PE ~40x 或 MI400 出货量超预期再考虑

---

## 六、与第一轮研究的 Delta

### 判断变化

| 维度 | 05.21 初始判断 | 06.04 更新判断 | 变化原因 |
|------|---------------|---------------|---------|
| ASIC 替代速度 | 2028年超越GPU出货量 | **加速至2027年追平**（Goldman Sachs） | Q1数据确认加速 |
| NVIDIA 短期地位 | 绝对主导但面临侵蚀 | **比预期更强**（Q1 $75.2B beat） | Blackwell 需求超预期 |
| CoWoS 瓶颈 | 持续至2027 | **确认持续，产能上调但不解渴** | TSMC 良率>98%+排队>50周 |
| MRVL 投资价值 | 高弹性标的 | **下调至谨慎**，估值过贵 | FY2027 PE 68x 已充分定价 |
| TPU 路线 | 新增变量 | **确认重要性上升** | Ironwood 专为推理设计+Anthropic $21B 订单 |

### 新增风险信号

1. **GPU 短期租赁价格 5 月暴跌 30-40%**（TechInsights），过剩压力信号强于预期
2. **推理模型占比飙升**导致每查询 token 消耗暴增——总推理算力需求曲线可能比线性更陡，这是正面因素
3. **Broadcom AI 收入中网络占比**可能被市场低估（估计 40-50%），纯定制加速器市场可能偏小

---

## 数据来源索引

| 数据点 | 来源 |
|--------|------|
| NVIDIA Q1 FY2027 财报 | nvidianews.nvidia.com, CNBC, Investopedia, TIKR |
| NVIDIA Q2 指引 $91B | CNBC, Perplexity Finance, Facebook post |
| NVIDIA FY2027 共识 ~$343B DC | S&P Global, Simply Wall St |
| NVIDIA Forward PE 25.5x | Yahoo Finance (6/2/2026) |
| NVIDIA 股价 ~$222 | CNN Markets, Yahoo Finance (6/3/2026) |
| Broadcom Q1 FY2026 AI $8.4B | Broadcom IR, Futurum, Investing.com |
| Broadcom 定制加速器 $10B 订单 | mlq.ai |
| AVGO 股价 ~$481, 市值 $2.3T | Yahoo Finance, WSJ (6/3/2026) |
| AVGO Forward PE ~38-43x | Yahoo Finance, Trefis, Motley Fool |
| Marvell FY2026 $8.2B, Q1 FY2027 $2.42B | Marvell IR, Reuters, Quartz, Barron's |
| Marvell 定制芯片 FY2029 $10B+ | Reuters |
| MRVL 股价 ~$301, 市值 ~$264B | Yahoo Finance (6/3/2026) |
| MRVL Forward PE ~68x | StockAnalysis |
| AMD Q1 2026 $10.3B, DC $5.8B | AMD IR, Quartz, Yahoo Finance |
| AMD MI400 ~$7.2B 预测 | Threads/@milkroadai |
| AMD 股价 ~$542, 市值 ~$885B | Yahoo Finance, Macrotrends (6/2/2026) |
| AMD Forward PE ~74x | Yahoo Finance |
| Google Ironwood 4,614 TFLOPS, 10x v5p | Google Blog, VentureBeat |
| Anthropic ~100万颗 Ironwood, ~$21B | Reddit r/mlscaling, Anthropic blog |
| Google Q1 2026 $109.9B, Cloud >$20B | Seeking Alpha, Simply Wall St |
| GOOGL 股价 ~$362, 市值 ~$4.3T | CNBC, Yahoo Finance (6/3/2026) |
| GOOGL Forward PE ~28x | Trefis |
| TSMC CoWoS 月产能 ~130K (2026底), 141K (2027) | x.com/jukan05, financialcontent.com, digitimes |
| TSMC CoWoS 良率 >98% | digitimes (2026.05.15) |
| CoWoS 排队 >50 周 | Silicon Analysts |
| ASIC 出货追平 GPU (2027) | Goldman Sachs via LinkedIn/Yahoo Finance |
| ASIC 服务器出货占比 27.8% (2026) | Tom's Hardware |
| AI 推理市场 $118B (2026) → $313B (2029) | Fortune Business Insights |
| GPU 租赁价格 H100 $1.38-2.69/hr | thundercompute.com, jarvislabs.ai |
| GPU 租赁 5 月降 30-40% | Reddit r/StockMarket (TechInsights) |
| 1 年期 H100 合约回升 $2.35/hr | SemiAnalysis newsletter |

---

*报告日期：2026.06.04*
*研究员：基本面研究员（AI Agent）*
*下一轮更新触发：NVIDIA Q2 FY2027 财报（~2026.08）/ Hyperscaler 2027 CapEx 指引*
