# 课题 #11: 先进制程GAA与半导体制造架构变革 — 基本面研究报告

> **研究日期**: 2026年6月5日  
> **研究员**: Researcher A (基本面/半导体技术方向)  
> **报告类型**: Round 1 全面更新

---

## 一、TSMC N2量产进展

### 1.1 良率最新数据

| 时间节点 | 良率 | 说明 | 来源 |
|---------|------|------|------|
| 2025Q4 (量产初期) | ~70% | 官方确认量产，优于同期3nm初期良率 | TSMC官方/LinkedIn |
| 2026年1月 | ~70-75% | 分析师Ming-Chi Kuo报告 | Wccftech |
| 2026年中期 | 90%+ (SRAM/存储类) | SRAM测试芯片良率突破90% | TechPowerUp / Design-Reuse |
| 2026年5月 | 相比三星SF2(~40%，后改善至50-60%)，Intel 18A(~65%) | 三方对比，TSMC优势显著 | SemiWiki / Semicone |

**关键判断**: N2整体逻辑良率目前约70-75%，SRAM测试芯片可达90%+。相比N3量产初期的~55%良率，N2的良率爬坡曲线显著优于前代。TSMC在2026技术论坛上表示，第一年N2产出将比N3初期高45%。

### 1.2 客户Tape-Out与产能

**已确认N2客户**:
- **Apple**: 锁定TSMC N2超过一半产能，预计用于2026年iPhone (A20芯片)  | 来源: LinkedIn/TechPowerUp
- **NVIDIA**: 已tape-out 2nm设计，2025年采购TSMC达$233亿(超过Apple的$207亿成为最大客户) | 来源: Culpium
- **AMD**: Zen 6 CCD于2025年4月完成tape-out，预计2026年量产 | 来源: TechPowerUp
- **MediaTek**: Dimensity 9600已完成tape-out | 来源: TechPowerUp
- **Qualcomm**: 首批2nm芯片规划中 | 来源: Igor's Lab
- **Intel**: 不在N2首批客户名单中 (Intel使用自家18A) | 来源: TechPowerUp

**产能规划**:
- 2025Q4: 初始产能~40K wpm (宝山Fab 20 + 高雄Fab 22)
- 2026年: 扩至~100K wpm (4座2nm工厂)
- 2027年: 目标~200K wpm (产能再翻倍)
- 2026年全年产能已**售罄** (fully booked)

### 1.3 与Intel 18A / 三星SF2对比

| 维度 | TSMC N2 | Intel 18A | 三星 SF2 |
|------|---------|-----------|----------|
| 晶体管架构 | Nanosheet GAA (第一代) | RibbonFET (GAA) | MBCFET (GAA，第三代) |
| 背面供电(BSPDN) | 无 (N2无，A16才有) | **有 (PowerVia)** | 无 (预计后期加入) |
| 初始良率 | ~70% → 90%+(SRAM) | ~65% | ~30%→50%→60% |
| 量产时间 | 2025Q4 | 2026Q1 (HVM) | 2025Q4-2026Q1 |
| 主要客户 | Apple, NVIDIA, AMD, MediaTek, Qualcomm | Intel内部(Panther Lake/Clearwater Forest), MSFT, AWS | 三星内部(Exynos 2600), 潜在BYD |
| SRAM密度 | 优势明显 | 不及N2 | 较低 |
| 晶圆价格 | ~$30,000 | 未披露 | 预计低于TSMC |

**来源**: hwbusters.com, SemiWiki, 250mm.co.kr, techovedas.com, LinkedIn

**关键洞察**: TSMC N2在良率、客户生态、产能规模上全面领先。Intel 18A的技术差异化在于BSPDN (PowerVia) — 这是全球首个大规模量产的背面供电技术，能带来显著的功耗优势。三星SF2良率虽有改善(从30%→60%)，但距TSMC仍有较大差距。

---

## 二、ASML 2026年Q1-Q2订单及EUV出货

### 2.1 Q1 2026核心财务数据 (ASML官方)

| 指标 | Q1 2026 实际 | Q1 2025 对比 | 来源 |
|------|-------------|-------------|------|
| 总净销售额 | **€8.8B** | €7.7B (+14.3%) | ASML Press Release |
| 净收入 | **€2.8B** | €2.4B | ASML Press Release |
| 毛利率 | 54%+ (高端) | 54.0% | ASML / CNBC |
| 系统净销售 | €6.3B | — | TIKR |
| EUV贡献 | **€4.1B** (含2台高NA) | — | TIKR |
| Q1 EUV出货 | 12台(含高NA) | — | techovedas |

### 2.2 全年展望与订单

| 指标 | 数据 | 来源 |
|------|------|------|
| 2026全年营收指引 | **€36B-€40B** (上调自€34-39B) | ASML Q1 2026 Press Release |
| 2026年毛利率指引 | 51%-53% | ASML |
| Q1净预订额 | ~€39.4亿 (此前有报道Q4 2025订单创纪录€13B) | wireunwired |
| 裁员 | 1700个管理岗位 (尽管订单创纪录) | wireunwired |

### 2.3 高NA EUV进展

| 节点 | 状态 | 来源 |
|------|------|------|
| Intel (首家客户) | EXE:5200B安装完毕，通过验收测试，用于14A节点开发 | TechPowerUp / bits-chips |
| Intel 14A进度 | PDK 0.5已发货，客户反馈积极；风险生产预计2026年底 | LinkedIn / TokenRing |
| EXE:5200B参数 | NA 0.55 (vs 标准0.33)，吞吐量>200 wph，单价~$400M/台 | TokenRing / Wedbush |
| TSMC | 高NA已下单但节奏较Intel保守，优先用标准EUV推N2/A16 | 行业分析 |
| EXE:5200B累计 | Intel安装1台用于研发，后续将用于量产 | 多来源 |

**背景验证**: 原始README中"2026年60台标准EUV、2027年80台+10台高NA"的预测与当前ASML全年指引(€36-40B)和EUV出货12台/Q1的节奏基本吻合。

---

## 三、GAA供应链: 设备商收入增长

### 3.1 关键设备商GAA相关动态

| 公司 | 2026年表现 | GAA关联 | 来源 |
|------|-----------|---------|------|
| **Applied Materials (AMAT)** | 股价YTD +67%，2026年5月28日收盘$449.68 | 沉积/刻蚀/外延设备，GAA纳米片的关键工艺（SiGe/Si选择性刻蚀） | TechTimes / InsiderMonkey |
| **Lam Research (LRCX)** | 半导体设备龙头，等离子刻蚀市场份额~50% | 各向同性刻蚀是GAA纳米片释放的关键步骤；低温刻蚀技术 | SeekingAlpha / TradingView |
| **KLA (KLAC)** | 毛利率和设备股Quant评分最高 | 量测/检测设备，GAA工艺控制要求显著提升 | SeekingAlpha |
| **Tokyo Electron (TEL)** | IR Day强调GAA和BSPDN为技术拐点 | GAA刻蚀+沉积(与AMAT/LAM竞争) | TEL IR Day 2025.02 |

### 3.2 市场规模与WFE支出

- **300mm Fab设备支出 2026-2028**: 总计**$374B** (SEMI 2025Q3 300mm Fab Outlook)
- **Logic/Micro细分**: $175B (2026-2028)，领先所有细分市场
- **先进制程产能**: 982K wpm (2025) → 1.16M wpm (2026) → 2028年1.4M+ wpm，CAGR 14%
- **GAAFET市场规模**: $76.9B (2025) → $251.9B (2035)，CAGR 12.6% (market.us)

### 3.3 专利与技术壁垒

三星和TSMC的GAA专利均提及SiGe-to-Si选择性刻蚀比>150:1用于纳米片释放 — 这是AMAT/LAM/TEL三家刻蚀设备的核心战场。来源: PatSnap

**关键判断**: GAA转型为设备商创造了显著的增长机会。(1)纳米片形成需要高精度各向同性刻蚀，Lam Research和TEL直接受益；(2)多层外延沉积增加AMAT机会；(3)工艺复杂度提升→检测/量测需求增加→KLA受益。

---

## 四、HBM4/HBM4E进展及与GAA协同

### 4.1 HBM4量产状态 (2026年6月)

| 厂商 | 状态 | 关键参数 | 来源 |
|------|------|---------|------|
| **SK海力士** | HBM4量产中 (2026年2月起)，市场份额**62%** | 10Gbps数据率，功耗改善40% | Astute Group |
| **三星** | HBM4量产中 (2026年2月起)，首批交付Q1 2026 | 11.7-13Gbps | Qatar Observer |
| **美光(Micron)** | HBM3E收入$2B，HBM4送样中 | 与TSMC合作，毛利率目标50%+ | AInvest |
| 三星 vs SK | 三星加速追赶，价格战(HBM3E降价30%) | — | LinkedIn |

### 4.2 HBM4E — 下一代竞速

| 厂商 | 时间 | 规格 | 来源 |
|------|------|------|------|
| **三星** | 2026年5月**送样**12层HBM4E (提前于原计划) | **3.6 TB/s**带宽，16Gbps/pin，48GB/stack，1c DRAM + 4nm逻辑基底 | TechTimes / AJU Press |
| **三星 GTC 2026** | 展示HBM4E | **4.0 TB/s**，16Gbps/pin | Samsung Newsroom |
| **SK海力士** | 加速至**2026年** (原计划2027年) | 第七代HBM | The Elec |
| **Google** | 已转向HBM4E评估 | 加剧三星/SK竞争 | CHOSUNBIZ |

### 4.3 HBM与GAA的协同

**逻辑基底Die的工艺升级是关键协同点**:
- HBM4的逻辑基底Die使用先进逻辑工艺(4nm级别)，这些工艺本身基于GAA/FinFET
- 三星HBM4E的逻辑基底使用**4nm级工艺**
- 随着HBM带宽需求持续增长，逻辑基底Die的晶体管密度和功耗要求将推动其向GAA工艺迁移
- HBM4E的量产时间(2026H2)与GAA大规模普及(2026-2027)高度重合

**三星HBM5**: Computex 2026上首次展示，目标4TB/s带宽 | 来源: PCVenus

---

## 五、背面供电(BSPDN)商业化时间线

### 5.1 三大厂商BSPDN路线图

| 厂商 | 节点 | BSPDN名称 | 时间线 | 状态 | 来源 |
|------|------|-----------|--------|------|------|
| **Intel** | 18A (及20A) | **PowerVia** | **2026Q1 HVM** | ✅ **已量产** — Panther Lake CES 2026发布 | Intel Newsroom / LinkedIn |
| **TSMC** | A16 (1.6nm级) | Super PowerRail | **2026H2** 风险生产，大规模量产可能2027 | 🔄 开发中 | Tom's Hardware / TSMC |
| **三星** | SF2P 或更晚 | 待定 | **2027+** | 🔄 规划中 | 行业分析 |

### 5.2 BSPDN技术意义

BSPDN将供电网络从晶圆正面移至背面：
- **IR Drop降低**: 供电路径从15+金属层缩短至直接背面连接
- **正面空间释放**: 改善信号布线密度
- **Intel PowerVia实测**: 频率提升6%，功耗降低30%+ (来源: SemiAnalysis)
- **Intel的关键差异化**: 18A是目前全球唯一同时量产GAA+BSPDN的节点

### 5.3 关键技术挑战与展望

TSMC选择在N2上**不使用BSPDN**(聚焦良率爬坡)，单独推出A16节点搭载背面供电。这体现了TSMC保守稳健的策略。Intel则选择18A"一步到位"同时引入GAA+BSPDN，技术风险更高但成功后差异化显著。目前18A供应短缺的报道暗示Intel的激进路线面临良率挑战。

---

## 六、Intel代工业务最新进展

### 6.1 18A量产状态

| 维度 | 数据 | 来源 |
|------|------|------|
| 量产时间 | 2025年底首批出货，2026Q1 HVM | Intel CES 2026 / 雅虎财经 |
| 首批产品 | Core Ultra Series 3 (Panther Lake, AI PC) | CES 2026 Intel Newsroom |
| 数据中心产品 | Xeon 6+ "Clearwater Forest" (Computex 2026) | PConline |
| PDK 1.0 | 2024年7月发布，累计**100+ tape-outs** | Electronics Weekly |

### 6.2 外部代工客户

| 客户 | 状态 | 来源 |
|------|------|------|
| **Microsoft** | 已宣布合作 (Maia AI加速器) | ITdaily / CRN |
| **AWS** | 已宣布合作 | CRN |
| **NVIDIA** | **已测试但未承诺量产** (2025年12月暂停评估) | Reuters / TechPowerUp |
| CEO Lip-Bu Tan | 称代工业务吸引到更多客户兴趣 | MLQ.ai |

### 6.3 核心挑战

1. **供应短缺**: Panther Lake/Wildcat Lake芯片供应不足，多家OEM担忧 | 来源: Culpium / ITHome
2. **NVIDIA退出**: 最受期待的外部客户暂停评估，对市场信心打击显著 | 来源: Reuters
3. **无重大外部量产客户**: MSFT/AWS虽宣布但未见量产，SemiAccurate称至少有一个"量产客户"，但身份未明 | 来源: Investing.com
4. **18A非理想代工节点**: Electronics Weekly分析认为18A需要与客户深度协同设计，不利于第三方代工模式
5. **真正对决在14A**: 预计2027年，将是Intel能否追赶TSMC的决胜节点 | 来源: Forbes / Electronics Weekly

### 6.4 判断: Intel能否追上TSMC?

**短期(2026)**: 大概率**不能**。TSMC N2良率、客户、产能全面碾压。Intel 18A虽有BSPDN差异化，但良率问题、供应短缺、外部客户不足构成巨大阻力。

**中期(2027-2028)**: 取决于**14A节点的执行力**和能否赢得至少一个大客户量产订单。Intel已安装ASML EXE:5200B高NA EUV，PDK 0.5获积极反馈，这是追赶的必要条件但非充分条件。

**长期风险**: Intel Foundry Direct Connect 2026已被取消，信号偏负面。

---

## 七、中国先进制程进展与出口管制

### 7.1 SMIC技术状态

| 节点 | 状态 | 技术路线 | 良率估计 | 来源 |
|------|------|---------|---------|------|
| **7nm (N+2)** | ✅ 量产中 (华为Kirin芯片) | DUV多重曝光(无EUV) | ~30% (远低于台积电同类) | TechInsights/Reddit |
| **5nm (N+3)** | 🔄 开发中/小规模试产 | DUV极限扩展 | ~3%或更低 | wccftech/Reddit |
| **2nm设计** | ⚠️ 有设计(Dishan Technology)但无制造能力 | — | N/A | ABHS |

### 7.2 出口管制最新动态

| 时间 | 管制措施 | 影响 | 来源 |
|------|---------|------|------|
| 2022年10月 | 美国首次限制先进计算/半导体对华出口 | 切断EUV获取 | Wikipedia |
| 2023年10月 | 进一步收紧 | 限制更多DUV设备 | CSIS |
| 2024年12月 | 再次收紧 | — | CSIS |
| **2025/2026** | **荷兰要求ASML NXT:1970i和1980i出口需许可证** | 进一步限制DUV浸没式光刻机 | Tom's Hardware |
| 当前 | SMIC产能扩张计划: 7nm产能目标翻倍 | 依靠现有DUV库存设备 | Nikkei Asia |

### 7.3 核心判断

1. **SMIC已实现7nm量产**，但严重依赖DUV多重曝光，良率远逊于台积电（~30% vs ~95%+）
2. **5nm有突破但无法规模化**：FT和SemiAnalysis确认Huawei/SMIC在尝试5nm，但仅限极小规模
3. **出口管制有效性**: 延缓了中国进展但未完全阻止；美国/荷兰不断扩大管制范围
4. **关键瓶颈**: 没有EUV光刻机，中国在5nm以下节点的经济性和良率将持续受制
5. **Samsung Foundry新变量**: 据2026年6月3日报道，三星正与BYD等中国车企洽谈2nm/4nm自动驾驶SoC代工（来源: TrendForce）。这可能为中国提供替代路径，但也受美国出口管制限制。

---

## 八、GAA渗透率 2026-2028预测

### 8.1 从FinFET到GAA的迁移

| 年份 | GAA晶圆产能占比 | 关键驱动事件 | 来源 |
|------|---------------|-------------|------|
| **2025** | <5% | TSMC N2试产、三星SF2初期 | 推算 |
| **2026** | **~15-20%** | TSMC N2 100K wpm量产、Intel 18A HVM、三星SF2/SF2P | 行业推算 |
| **2027** | **~30-35%** | TSMC N2扩至200K wpm、Intel 14A(高NA)、三星SF2P全速 | Globalsemiresearch |
| **2028** | **~45-50%** | 先进制程总产能1.4M+ wpm，GAA成为逻辑制程主流 | SEMI |

### 8.2 支撑数据

- **先进制程产能**(≤7nm): 2025年982K wpm → 2026年1.16M wpm → 2028年1.4M+ wpm (SEMI)
- **TSMC N2产能**: 2026年~100K wpm，2027年~200K wpm (Globalsemiresearch)
- **Intel 18A产能**: 初期规模较小(Arizona fab)，14A高NA助力2027年
- **三星SF2产能**: 2026年产能扩充163%，但基数较低
- **GAAFET市场**: $76.9B(2025) → $251.9B(2035)，CAGR 12.6% (market.us)
- 到2026年所有主要逻辑厂商都将采用GAA (Medium/Semiconductors in 2026)

### 8.3 渗透率爬坡的关键假设

| 假设 | 乐观情景 | 基准情景 | 悲观情景 |
|------|---------|---------|---------|
| TSMC N2良率 | 2026H2达85%+ | 2026H2达80% | 维持70% |
| Intel 18A外部客户 | 2026签2家量产 | 2027首签 | 2027仍无 |
| 三星SF2良率 | 2026H2达70% | 达60% | 维持50% |
| 高NA EUV | 2026年5台出货 | 3台 | <3台 |
| AI芯片需求 | 持续爆发 | 稳步增长 | 见顶回落 |

---

## 九、关键投资结论

### 9.1 高确信度判断

1. **TSMC N2统治力确立**: 良率(70-90%+)、客户(Apple/NVIDIA/AMD/MediaTek)、产能(100K wpm 2026→200K 2027)三项指标全面领先
2. **GAA时代正式开启**: 2026年TSMC/Intel/三星三家全线转向GAA，设备商(AMAT/LAM/KLA/TEL)直接受益
3. **HBM4/HBM4E超级周期**: 三星/SK海力士/美光全面扩产，2026年为HBM4量产元年，HBM4E提前至2026年底送样
4. **BSPDN为大势所趋**: Intel已量产，TSMC A16于2026H2跟上，三星规划中

### 9.2 需关注的关键变量

1. **Intel 14A vs TSMC A16**: 2027年的真正决胜局，高NA EUV的应用效果是关键
2. **Samsung Foundry能否翻盘**: SF2良率改善和BYD等中国客户的获取
3. **中国5nm进展**: 尽管无EUV，DUV路线的极限在哪里？
4. **特朗普/拜登之后的出口管制政策变化**: 若放松，将加速中国进展
5. **ASML高NA EUV渗透节奏**: 2026-2027年实际出货和客户接受度

### 9.3 数据质量说明

- 所有数据截至2026年6月5日可获取的最新公开信息
- TSMC部分良率数据来自行业报告和分析师，未经TSMC官方确认
- SMIC的5nm良率数据为行业推算，实际数据不可获取
- GAA渗透率为基于SEMI产能数据和公司指引的综合推算

---

*报告完*
