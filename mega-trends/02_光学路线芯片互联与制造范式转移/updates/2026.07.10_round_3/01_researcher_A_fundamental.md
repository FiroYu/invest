# R3 基本面研究报告 — #02 光学路线芯片互联与制造范式转移

> **研究员**：A 基本面 | **日期**：2026.07.10 | **周期**：R2（2026.05.25 基线）→ R3，覆盖 2026 H1（重点 5-7 月）
> **范围**：公司财务 + 技术里程碑 + 量产/出货数据
> **数据源**：公司财报/公告、TrendForce、LightCounting、SEMI、Reuters、券商研报、公司新闻稿（均带链接与日期）

---

## 一、执行摘要（头号发现）

1. **CPO 量产元年已实质兑现**：NVIDIA Spectrum-X Photonics（Ethernet）于 2025 GTC 宣布 "full production" 并 H2 2025 出货；Quantum-X Photonics（InfiniBand）Q3450-CD 115.2Tbps 于 2026 初交付；Broadcom 51.2T Bailly CPO 量产且"故障率极低"、5.4W/800G（节能 65%），Tomahawk 6 102.4Tbps 已发布。**基线"CPO 量产元年"的判断已从预期变为事实**。

2. **中国光模块双雄业绩炸裂，验证 1.6T 起量**：中际旭创 2026 Q1 营收 194.96 亿元（+192.12% YoY）、归母净利 57.35 亿元（**+262.28% YoY**，单季超 2024 全年），毛利率 ~46%；800G FY2025 出货 200 万+只（占营收 60%+），1.6T 2025 Q3 已开始量产、2026 正式起量（券商预测全球 800 万只需求，旭创占 ~50% = 400 万只×$1500）。新易盛 Q1 营收 83.38 亿（+105.76%）但受 5.22 亿汇兑损失拖累、利润环比回落引发板块波动。

3. **硅光子占比 2026 首次突破 50%（里程碑）**：LightCounting 2026 年 5 月报告指出，2026 年将是硅光子调制器 transceiver 销售首次超过 50% 的年份，硅光路线相对 InP 路线胜出趋势确立。

4. **High-NA EUV 出现重大变数**：TSMC 在 2026 北美技术论坛宣布 A14（2028 量产）、A13、A12（2029）**全部不用 ASML High-NA EUV**，改用现有 EUV 工具多重曝光。这是对 R2 基线"High-NA EUV 2026 量产用于 sub-2nm"判断的部分证伪——**最大代工厂拒绝该技术路线**。Intel 14A（2027）则成为 High-NA EUV 首个生产节点，已下单两台 EXE:5200、设备订单 2026 同比 +50%。

5. **光子计算资本热度高，但商用案例仍为零**：Ayar Labs 2026 年 3 月完成 $500M Series E（估值 $37.5 亿，光子史上最大单轮），曦智科技港交所上市市值突破 800 亿港元；但 Lightmatter 最新融资仍停留在 2024 年 10 月 $400M Series D，**三家公司均无公开的大客户营收或大规模商用案例**——资本驱动估值而非业务驱动。

6. **铜的反击比预期更强**：Molex Impress 与 Amphenol XtremePass 的 224G PAM-4 CPC（共封装铜）产品**已商用**，路线图指向 448G。这延长了铜在机柜内的寿命，CPO 的渗透节奏可能慢于此前乐观预期。

---

## 二、各公司/技术线详细数据

### 2.1 NVIDIA — CPO 龙头，量产已兑现

| 产品 | 类型 | 关键参数 | 状态 |
|------|------|----------|------|
| **Spectrum-X Photonics** | Ethernet CPO | 128×800G 或 512×200G，100Tb/s 总带宽；3D 堆叠 CPO ASIC | **2025 GTC 宣布 full production，H2 2025 出货** |
| **Quantum-X Photonics Q3450-CD** | InfiniBand CPO | 115.2Tbps 全双工，144 端口，液冷，4 个 Quantum-X 芯片 | **early 2026 交付** |
| 未来 Spectrum-X 变体 | Ethernet CPO | 512×800G 或 2048×200G | 路线图 |

**客户公开确认**：TACC（Texas Advanced Computing Center）、Lambda（已收到样品并公开开箱）、CoreWeave。

**功耗宣称**：CPO 功耗从 30W 降至 <9W（基线已记录），带宽密度数倍提升。

**来源**：
- [NVIDIA 官方新闻稿（2025）](https://investor.nvidia.com/news/press-release-details/2025/NVIDIA-Announces-Spectrum-X-Photonics-Co-Packaged-Optics-Networking-Switches-to-Scale-AI-Factories-to-Millions-of-GPUs/default.aspx)
- [NVIDIA Silicon Photonics 产品页](https://www.nvidia.com/en-us/networking/products/silicon-photonics/)
- [Lambda 开箱博客](https://lambda.ai/blog/unbox-one-of-nvidias-first-co-packaged-optics-samples-with-lambda)
- [Naddod 分析：Quantum-X early 2026](https://www.naddod.com/ai-insights/nvidia-s-silicon-photonics-cpo-the-beginning-of-a-transformative-journey-in-ai)

### 2.2 TSMC COUPE — 硅光子代工平台 2026 量产

- **COUPE（Compact Universal Photonic Engine）**：TSMC 集成硅光子平台
- **路线图**：2025 小形状可插拔资质 → **2026 CoWoS-based CPO 集成量产**（on track）
- **行业定位**：SEMI 指定 **2026 为硅光子规模部署元年**
- **对比**：Samsung 目标 **2029** CPO turnkey（落后 TSMC 约 3 年）
- **2026 技术论坛亮点**：5.5-reticle CoWoS（世界最大），**>98% 良率**

**来源**：
- [TrendForce 2026.04：Silicon Photonics Race Intensifies](https://www.trendforce.com/news/2026/04/01/news-silicon-photonics-race-intensifies-as-tsmc-targets-2026-coupe-production-samsung-eyes-2029-cpo-turnkey/)
- [SEMI：2026 inaugural year](https://www.creating-nanotech.com/en-US/newsc302-semi-2026-marks-the-inaugural-year-for-scaled-silicon-photonics-deployment-optical-interconnects-key-to-mass-production)
- [TSMC 2026 Tech Symposium](https://www.tsmc.com/static/english/campaign/Symposium2026/index.htm)
- [Semiconductor Engineering：TSMC Tech Symposium 2026 By The Numbers](https://semiengineering.com/tsmc-tech-symposium-2026-by-the-numbers/)

### 2.3 Broadcom — CPO 量产标杆，已发布 102.4T 下一代

- **Bailly（51.2T CPO switch）**：**已量产出货，故障率极低**；功耗 5.4W/800G（节能 65%）；单台成本 ~$1000
- **Tomahawk 6（102.4T CPO）**：已发布，16×6.4Tbps 接口
- **战略意义**：Broadcom 的 CPO 走在系统公司前列，NVIDIA 是追赶者之一

**来源**：
- [SemiAnalysis：CPO Book（Broadcom Bailly 5.4W/800G）](https://newsletter.semianalysis.com/p/co-packaged-optics-cpo-book-scaling)
- [Broadcom Tomahawk 6 102.4T（LinkedIn 行业报道）](https://www.linkedin.com/posts/%E9%8A%98%E5%B3%B0-%E6%9E%97-64b46b319_opticalinterconnect-cpo-npo-activity-7439219650048978944-y323)
- [IDTechEx：CPO Race NVIDIA vs Broadcom](https://www.idtechex.com/en/research-article/co-packaged-optics-race-strategic-approaches-from-nvidia-and-broadcom/34467)

### 2.4 Marvell / Cisco — 开放 CPO 生态

- **Marvell + Jabil**：OFC 大会展示**开放设计 CPO switch 系统**，液冷、中平面光纤管理、224G signaling
- **Cisco**：在 51.2T/102.4T/204.8T 各代 CPO 设计上持续投入
- **注意**：Marvell 已于 2025 收购 **Celestial AI**（光子互联），重塑市场格局

**来源**：[Marvell OFC 贡献（Facebook）](https://www.facebook.com/MarvellTechnology/posts/marvell-will-contribute-to-an-important-discussion-at-the-ofc-conference-on-the-/1490540519741891/)

---

### 2.5 中际旭创（300308.SZ）— 业绩超预期，1.6T 起量

#### 2026 Q1 财报（2026.04.16 披露）

| 指标 | 2026 Q1 | 同比 | 环比 |
|------|---------|------|------|
| 营业收入 | **194.96 亿元**（~$28.5亿） | **+192.12%** | +47.3% |
| 归母净利润 | **57.35 亿元**（~$8.4亿） | **+262.28%** | +56.5% |
| 毛利率 | ~46% | 持续扩张 | （vs FY2025 42.61%） |
| 经营性现金流 | 33.68 亿元 | +55.58% | — |
| 研发支出 | 6.45 亿元 | +122% | — |

**历史意义**：Q1 单季归母净利**超过 2024 全年归母净利**。

#### 800G / 1.6T 出货结构

- **800G**：FY2025 出货 **>200 万只**，占营收 **60%+**；2026 Q1 继续环比增长；Goldman Sachs 预测 2026 800G 收入有望同比翻倍
- **1.6T**：**2025 Q3 开始量产**关键客户，2025 Q4 攀产，**2026 正式起量**；Goldman Sachs 预估 1.6T 占收入从 2025 的 8% 大幅提升
- **券商综合预测**：2026 全球 1.6T 需求 ~**800 万只**，中际旭创拿下 ~**50% 份额 = 400 万只×$1500/只** ≈ 60 亿美元收入潜力
- **800G + 1.6T 合计**：预计贡献 2026 增量收入 **>70%**

#### FY2025 全年（对比基准）
- 营收 382.4 亿元（+60.25%）
- 归母净利 107.97 亿元（+108.78%）

#### 估值
- 同花顺综合预测 2026 EPS ~26.99 元（同比 +175.41%）
- 当前股价对应 PE ~41.68 / 21.74 / 14.21（2026/2027/2028）

**来源**：
- [钛媒体：Q1 净利暴增 262%](https://www.tmtpost.com/7957799.html)
- [富途：800G 放量驱动业绩兑现](https://news.futunn.com/en/post/72750156)
- [同花顺 F10 盈利预测](https://basic.10jqka.com.cn/300308/worth.html)
- [moomoo：1.6T 放量元年与英伟达共舞](https://www.moomoo.com/news/post/67178090)

### 2.6 新易盛（300502.SZ）— 高增长但 Q1 风波

#### 2026 Q1 财报
| 指标 | 2026 Q1 | 同比 |
|------|---------|------|
| 营业收入 | **83.38 亿元** | **+105.76%** |
| 净利润 | 受 **5.22 亿汇兑损失** 拖累，还原后约 33 亿元 | — |
| 毛利率 | 维持高位（800G/1.6T 占比提升） | — |

**问题信号**：净利润**环比回落**（vs 2025 Q4），市场一度"炸锅"，板块回调。反映高速光模块板块在产能扩张+汇率波动下的盈利韧性考验。

#### FY2025 全年
- 营收 248.42 亿元（+187.29%）
- 销售毛利率 47.81%（同比 +3.09pp）

#### 800G / 1.6T
- 800G Q1 出货同比翻倍，占营收 **>60%**
- 1.6T：2025 市占率 ~0%，**2026 预计 ~10%**（逐步起量，慢于中际旭创）

**来源**：
- [21 世纪经济报道：新易盛一季报风波](https://www.21jingji.com/article/20260424/herald/7d4b72f6df31c9c7c029cbafeb2e7643.html)
- [钛媒体一季报点评](https://www.tmtpost.com/7967261.html)
- [财联社：Q1 净利润环比回落](https://m.cls.cn/detail/2354227)
- [证券时报：2025 业绩跨越式增长](https://www.stcn.com/article/detail/3795816.html)

---

### 2.7 Ayar Labs — 光互联独角兽，资本确认

- **2026.03.03：$500M Series E**，估值 **$37.5 亿**（光子计算史上最大单轮）
- 累计融资 **~$870M**
- 上一轮：2025.12 的 $155M Series D，**AMD Ventures** 领投，NVIDIA/Intel 联合战略投资 $1.55 亿（基线已记录的 $5 亿总盘即此轮系列）
- **产品**：UCIe-compliant **TeraPHY** chiplets，CPO 解决方案
- **目标**：2028 AI 系统量产爬坡
- **荣誉**：Fast Company "2026 最创新公司" 计算类前 5

**来源**：
- [Ayar Labs 官方公告](https://ayarlabs.com/news/ayar-labs-closes-500m-series-e-accelerates-volume-production-of-co-packaged-optics/)
- [The Next Platform](https://www.nextplatform.com/connect/2026/03/04/ayar-labs-gets-500-million-to-ramp-photonics-into-2028-ai-systems/)

### 2.8 Lightmatter — 进展平稳，无新融资

- **最新融资仍是 2024.10 的 $400M Series D**，估值 $44 亿，T. Rowe Price 领投，**Google 再次跟投**
- 累计融资 $850M
- **产品线**：Passage（3D 光子中介层，商业化推进中）、Envise（光子 AI 加速器，两块板 1.2M ResNet-50 推理/秒）、Guide（激光系统）、EVK50/100/M1000
- **2026 动态**：Lightmatter InterConnect 2026 活动展示 Passage 路线图
- **关键空白**：**未披露明确的大客户商用营收数字**，也无 2026 新融资

**来源**：
- [Lightmatter 官网](https://lightmatter.co/)
- [Optics.org：Google 再次投资](https://optics.org/news/google-backs-lightmatter-again-in-400m-fundraising)
- [Yole Group](https://www.yolegroup.com/industry-news/lightmatter-raises-more-funding-for-photonic-ai-chips/)

### 2.9 曦智科技 — 港交所"全球 AI 硅光芯片第一股"

- **上市**：港交所 IPO，**市值突破 800 亿港元**
- **融资史**：A 轮 $2600 万（经纬中国/中金资本领投）；**2025.09 C 轮超 15 亿元人民币**
- **2025 营收**：约 **1.06 亿元**（光互连业务占 **71%**，光计算为辅）
- **技术**：oMAC（光子矩阵计算）+ oNOC（片上光网络）+ oNET（片间光网络）
- **关键节点**：**PACE 3 芯片计划 2026 H1 完成流片**；CPO 量产待兑现
- **风险**：招股书披露财务与治理风险，光算力商业化能否重构算力格局取决于 PACE 3 流片与 CPO 量产

**来源**：
- [财联社：市值突破 800 亿港元](https://www.cls.cn/detail/2357610)
- [证券时报：通过港交所上市聆讯](https://stcn.com/article/)

### 2.10 其他玩家
- **nEye.ai**：2026.04.14 完成 $80M Series C（Sutter Hill 领投，累计 $152M），AI 光路交换
- **Salience Labs**：2026.02 与 Tower Semiconductor 合作量产光路交换芯片
- **Lumentum / Coherent**：光器件巨头，持续供应 CPO 光引擎所需

---

### 2.11 ASML High-NA EUV — 重大变数

#### 量产与订单
- **首台 EXE:5200B**：2025 Q4 出货（CFO Roger Dassen 在 2026.01 财报会确认）
- **Intel 是首个客户**，用于 14A 节点（2027 生产）
- Intel 已**增订第二台** High-NA 机器，2026 设备订单同比 **+50%+**（TrendForce）
- Intel 14A 验收测试完成，yield 达里程碑

#### ASML 2025 Q4 财报
- 营收 **€8.5B（+15% YoY）**
- **Booking €44B 创纪录**，AI 驱动光刻需求
- 2026/2027 earnings 预计增长 **21.7% / 22.5%**（Zacks 共识）

#### TSMC 拒绝 High-NA（重大信号）
- **TSMC 2026 北美技术论坛**：A14（2028）+ A13 + A12（2029）**全部不用 High-NA EUV**
- 改用现有 EUV 工具 + NanoFlex Pro 技术 + nanosheet 晶体管
- 性能：A14 vs N2 → 10-15% 速度提升 或 25-30% 功耗降低，逻辑密度 +20%+
- **Reuters 标题**："TSMC shows smaller, faster chips without a pricey new tool from ASML"
- **含义**：最大代工厂拒绝该技术，**High-NA EUV 近期客户池显著收窄**至 Intel + Samsung + Rapidus

#### Intel 14A 客户
- Intel Foundry 14A 吸引 **Apple、NVIDIA、AMD** 潜在代工客户
- 14A 将是**首个使用 ASML High-NA EUV（NA 0.55）的生产节点**
- 但 Intel 保留"若性价比不成立则 14A 切回低-NA 流程"的权利

**来源**：
- [TSMC A14 Press Release](https://pr.tsmc.com/english/news/3302)
- [Reuters：TSMC without ASML pricey tool](https://www.reuters.com/world/asia-pacific/tsmc-shows-smaller-faster-chips-without-pricey-new-tool-asml-2026-04-22/)
- [TechPowerUp：TSMC skips High-NA for A14](https://www.techpowerup.com/336034/tsmc-skips-high-na-lithography-for-a14-node-development)
- [TrendForce：ASML EXE:5200 首出货](https://www.trendforce.com/news/2025/07/17/news-asml-confirms-first-high-na-euv-exe5200-shipment-reportedly-prepping-for-intels-14a-in-2027/)
- [Intel Newsroom：High NA EUV New Frontier](https://newsroom.intel.com/intel-foundry/intel-foundry-opens-new-frontier-chipmaking)
- [NineScrolls：Intel Foundry 订单 +50%](https://ninescrolls.com/news/intel-foundry-boosts-equipment-orders-50-as-14a-node-draws-apple-nvidia-and-amd)

---

### 2.12 光模块速率与 LightCounting 预测

#### 整体市场
- AI cluster optics：**~$5B（2024）→ ~$10B（2026）**，2026 增长 ~60%
- LightCounting 2030 总市场可能达 **$1000 亿**（上调预期）
- 2025 出货 >6000 万只，2026 接近 1 亿只
- 2025-2026 年化增长 30-35%，2027-2030 回落至 15-20%

#### 1.6T
- **1.6T 芯片组 2026 销售预计 >$20 亿**
- 800G 2026 出货翻倍；1.6T 从 2025 小基数增长至**数千万端口**
- 800G + 1.6T 合计占 2026 光模块市场 ~64%（~$146 亿）

#### 3.2T
- LightCounting 2024.07 已将 3.2T transceiver 纳入预测
- Coherent 预测 800G/1.6T/3.2T 数据通信 transceiver 市场 5 年 CAGR **>40%**
- 3.2T 路线图已明确，但量产部署时间表仍较远（2027-2028）

#### CPO 渗透预测（LightCounting 口径调整）
- 定性：**"no longer if, but when"**，2027-2028 规模部署
- CPO 在 AI scale-up 场景 2026-2030 期间是最佳选项
- **Mordor Intelligence**：CPO 市场 **$161M（2026）→ $749M（2031），CAGR 35.7%**
- ⚠️ **对比基线**：R2 基线引用 Yole 的"$46M（2024）→ $8.1B（2030），CAGR 137%"——**新口径显著下修**（35.7% vs 137%）。R2 的 137% CAGR 可能过于激进。

#### 硅光子占比（里程碑）
- LightCounting 2026.05 报告：**2026 年硅光子调制器 transceiver 销售首次 >50%**
- 硅光路线相对 InP 路线胜出趋势确立

**来源**：
- [LightCounting 2026.03：$100B by 2030](https://www.lightcounting.com/newsletter/en/march-2026-ethernet-optics-382)
- [LightCounting 2026.05：Year of Silicon Photonics](https://www.lightcounting.com/newsletter/en/may-2026-silicon-photonics-lpolro-and-npocpo-377)
- [LightCounting 2025.07：Scale-up networks](https://www.lightcounting.com/newsletter/en/july-2025-cloud-data-center-optics-330)
- [Mordor Intelligence：CPO Market](https://mordorintelligence.com/industry-reports/co-packaged-optics-market)

---

### 2.13 铜的最后反击 — 224G CPC 已商用

#### Co-Packaged Copper（CPC）产品
| 厂商 | 产品 | 速率 | 状态 |
|------|------|------|------|
| **Molex** | Impress CPC | **224G PAM-4 现货**，开发中 448G | 已商用 |
| **Amphenol** | XtremePass CPC | **224/448G** | 已发布 |
| **Samtec** | CPX（共封装铜+光学 SMT） | 224G PAM-4+ | 开发中 |

**战略含义**：CPC 让铜在 224G 这一代继续可用，**延长机柜内铜互联寿命 1-2 代**。这与 CPO 形成直接竞争，可能将 CPO 大规模渗透推迟到 102.4T 之后（而非 51.2T）。

**来源**：
- [Molex Impress CPC 产品页](https://www.molex.com/en-us/products/connectors/high-speed-internal-io/impress-co-packaged-copper-solution)
- [Molex 224G PAM-4 技术](https://www.molex.com/en-us/industries-applications/servers-storage/224-gbps-pam4-high-speed-data-centertechnology)
- [Amphenol XtremePass CPC](https://www.amphenol-cs.com/product-series/xtremepass-overpass-cpc.html)
- [Samtec CPX 博客](https://blog.samtec.com/post/innovations-in-co-packaged-interconnects-for-224-gbps-pam4-and-beyond/)

---

## 三、关键指标 R3 更新（对照 README 关键指标表）

| 指标 | R2 值（2026.05） | **R3 值（2026.07）** | 趋势 | 验证状态 |
|------|------------------|----------------------|------|----------|
| 光模块速率主流 | 800G → 1.6T 过渡 | **800G 仍主导（2026 翻倍出货），1.6T 正式起量（数千万端口），3.2T 已上路线图** | ↑ 加速 | 验证光学路线不可逆 |
| CPO 渗透率（AI DC） | ~0%（量产元年） | **~0-2%（NVIDIA/Broadcom CPO 已量产但出货量小；规模化推至 2027-2028）** | 持平 | 量产兑现但规模延后 |
| 硅光子占光模块比例 | ~30% | **2026 首次 >50%（里程碑）** | ↑↑ 显著加速 | **硅光路线胜出**（触发 README 判断阈值） |
| Ayar Labs 等光互联独角兽营收 | 未公开 | **仍无公开 ARR；Ayar Labs 估值 $37.5 亿（资本驱动）** | 持平 | 商用案例仍为 0 |
| 铜缆最大单通道速率 | 200G（物理极限附近） | **224G PAM-4 已商用（Molex/Amphenol），448G 开发中** | ↑ 铜反击 | 突破 224G，铜路线终结论需修正 |
| 光子计算芯片商用案例 | 0（实验室/原型） | **仍为 0 大客户；但 PACE 3 2026H1 流片、Ayar Labs 2028 量产目标** | 持平 | 维持"高潜力但遥远"判断 |
| CPO 市场 CAGR | 137%（Yole） | **35.7%（Mordor 2026-2031）** | ↓ 预测下修 | R2 的 137% 过于激进 |
| High-NA EUV 量产用于 sub-2nm | 2026 量产（ASML 规划） | **TSMC A14 拒绝 High-NA；仅 Intel 14A（2027）采用** | ↓↓ 重大变数 | 层次一逻辑部分证伪 |

**触发的判断阈值**：
- ✅ **硅光子占比 2026 突破 50%**（README 阈值：50%+ 时确认硅光路线胜出）——**确认硅光路线胜出**
- ✅ **光模块速率持续向 3.2T 推进**（README 阈值：3.2T 量产时确认光学路线不可逆）——3.2T 已上路线图但未量产，方向不可逆性进一步增强
- ⚠️ **铜突破 224G**（README 阈值：无法突破 224G 时确认铜路线终结）——**已被突破（224G CPC 商用），铜路线终结论暂缓**

---

## 四、评级相关变化提示

### 支持升级（向上）

1. **中国光模块双雄业绩兑现**：中际旭创 Q1 净利 +262%、1.6T 正式起量、400 万只潜在订单——**基本面已支持"积极关注 → 有条件通过"**。这是中国具有全球定价权的少数科技领域，业绩可持续性强。

2. **CPO 量产已兑现**：NVIDIA Spectrum-X、Broadcom Bailly 均已量产；TSMC COUPE 2026 量产；不再是"预期"而是"事实"。

3. **硅光路线胜出确认**：硅光子占比 2026 >50%，是 README 设定的判断阈值。

4. **AI 光学市场潜力上调**：LightCounting 2030 $1000 亿可能性；AI cluster optics 2026 翻倍至 $100 亿。

### 支持谨慎（向下 / 风险）

1. **High-NA EUV 层次一逻辑部分证伪**：TSMC（最大代工厂）拒绝 High-NA，仅 Intel 14A（2027）采用。层次一（光刻演进）应从"延续性创新"进一步下调为"**客户基础显著窄于预期的延续性创新**"，对 ASML High-NA 的中期收入贡献应下修。

2. **CPO 市场 CAGR 预测下修**：从 Yole 的 137% 降至 Mordor 的 35.7%。R2 基线的 CPO 市场 $8.1B（2030）可能过于乐观，**Mordor 的 $749M（2031）是更保守的口径**。真相可能介于两者之间，但方向明确：**CPO 渗透节奏慢于此前乐观预期**。

3. **铜的反击强于预期**：224G PAM-4 CPC 已商用，448G 开发中。README 关键指标"铜无法突破 224G"的阈值**未触发**。CPC 与 CPO 在 51.2T 这一代直接竞争，CPO 大规模渗透可能要等到 102.4T 之后。

4. **光子计算商用仍为 0**：资本热度高（Ayar Labs $37.5 亿估值、曦智 800 亿港元市值），但**无大客户营收**。估值风险高，若 2027-2028 量产目标未兑现将面临深度回调。

5. **新易盛 Q1 风波**：利润环比回落、汇兑损失、板块波动——反映板块在高速增长中的盈利韧性考验，估值已不便宜（中际旭创 2026 PE ~42x）。

### 综合评级建议

**维持"积极关注"，可考虑升档"有条件通过"**，条件：
- 投资主线聚焦**层次二（光学互联）+ 中国光模块双雄**，这是业绩已兑现、确定性最强的部分
- **层次一（High-NA EUV）应下调权重**——TSMC 拒绝、客户池窄化
- **层次三（光子计算）维持"跟踪但不投资"**——商用案例 0、估值资本驱动
- 关注**铜（CPC）vs 光（CPO）在 51.2T/102.4T 的竞争**——这是未来 12-24 个月最大的不确定性

---

## 五、跨议题传导提示（给整合者）

- **#11 先进制程 GAA**：TSMC A14 不用 High-NA EUV 但仍用 nanosheet（GAA），**GAA 路线不受影响，High-NA 受影响**。需联动更新 #11 中 High-NA 假设。
- **#17 AI 推理经济/定制芯片**：互联带宽是 scaling 瓶颈，CPO/Optical I/O 是集群规模解锁器。NVIDIA CPO 量产意味着 AI 集群可继续扩张。
- **#21 铜铝超级周期**：CPC（共封装铜）已商用，铜在数据中心的生命比此前预期更长，**短期铜需求下行情景应上修**。但长期（2030+）光替代铜方向不变。
- **#01 AI CapEx**：光模块双雄业绩爆发是 AI CapEx 兑现的直接受益者；LightCounting $1000 亿（2030）口径进一步确认 AI CapEx 持续性。

---

## 附：数据源汇总（按主题）

**CPO/硅光巨头**：NVIDIA 官方 / TrendForce / SEMI / SemiAnalysis / IDTechEx / TSMC 2026 Symposium
**中国双雄**：钛媒体 / 富途 / 同花顺 / 财联社 / 21 世纪经济报道 / 证券时报 / 雪球 / moomoo / Goldman Sachs（华尔街见闻）
**光子计算**：Ayar Labs 官方 / The Next Platform / Lightmatter 官网 / Optics.org / Yole / 财联社（曦智）
**High-NA EUV**：TSMC Press / Reuters / TechPowerUp / TrendForce / Intel Newsroom / SemiWiki / NineScrolls / Zacks
**光模块速率/市场**：LightCounting 2026.03/05 / Mordor Intelligence / Coherent
**铜反击**：Molex / Amphenol / Samtec / ConnectorTips

> 报告完。所有数据截至 2026.07.10，关键财报到 2026 Q1，事件覆盖至 2026 年 6 月。
