# 研究员B报告 — 催化剂分析

> 议题#11 先进制程GAA与半导体制造架构变革 | 2026-07-10 | Round 3

---

## 核心发现 Top 3

### 发现1：VLSI 2026 + Computex 2026 集中披露——GAA+背面供电从"路线图"进入"硅验证"

2026年6月是先进制程的技术集中验证窗口。两个顶级会议（VLSI Symposium 6/14-18 檀香山、Computex 6月 台北）密集披露：

- **TSMC A16 论文（VLSI Late News T1.5）**：首次展示 "A16 Angstrom-class CMOS featuring Enhanced Nanosheet with **Super Power Rail**（背面直接接触供电）"，明确量产目标 **4Q26**。这是 A16 背面供电从纸面路线图走向硅数据的关键节点。
- **Intel 18A 被确认为"目前市场上唯一同时集成 GAA 晶体管 + 背面供电（BSPD）的工艺"**，公布 **~30% 核心频率提升@0.5V** 的实测数据。
- **Intel 18A-P 新变体进入风险生产**（+9% 性能、设计规则兼容 18A），专门面向外部代工客户。
- **Computex**：Intel 正式发布 **Xeon 6+ "Clearwater Forest"**——288 核 Darkmont E-core，12 个 18A 计算小芯片 + 3 个 Intel 3 基底芯片 3D 堆叠，已进入量产，号称单线程比 AMD 192 核 EPYC 9965 快 ~30%。这是 **18A 首次进入数据中心规模验证**。

**判断**：背面供电（BSPD）+ GAA 的"双技术叠加"在 2026 年中已不再是 PPT，而是有实测硅数据支撑。Intel 在 BSPD 的"首发商用"上确实抢占了叙事高点（TSMC A16 要到 4Q26 才风险生产），但 TSMC 的量产规模与客户厚度仍是护城河。★★★

### 发现2：NVIDIA 超越 Apple 成 TSMC 第一大客户——客户结构质变 + Rubin Ultra 4-die 取消

两件相互对冲的事件同时发生：

- **客户结构质变（正面）**：据 TSMC 财报披露，第一大客户（推断为 NVIDIA）贡献 **19% 营收**，正式超越 Apple 的 **17%**。NVIDIA 2025 年采购额 **~$23.3B** vs Apple **~$20.7B**。NVIDIA 要求 TSMC 将 N2 产能扩至 **16 万片/月**（TSMC 上限定在 14 万片）。Apple 已锁定初期 N2 产能 **>50%**（iPhone 18 A20）。TSMC 对 sub-5nm 晶圆 **涨价 3-5%**。N2 产能未来两年售罄。
- **Rubin Ultra 4-die 取消（负面，7/1）**：SemiAnalysis 报道，GTC 2026 发布仅 3 个月后，原定 4-die Rubin Ultra 因 **CoWoS-L 封装基板翘曲（substrate warpage）**、~9.5X reticle 互连复杂度被取消，改为双 die 版本。**直接将 2027 年峰值性能预期砍半**。

**判断**：客户结构质变（NVIDIA 登顶 + 涨价权）强化了 TSMC HPC 占比上行的逻辑；但 Rubin Ultra 取消暴露了**先进封装而非晶体管缩放**才是 2027 年的真正瓶颈——这对"先进制程=持续降本"的 H4 叙事是隐忧，也意味着 CoWoS-L 良率将成为下一个关键催化剂。★★★

### 发现3：Intel 18A 良率拐点确认——D0 进入成熟区间，但市场仍惩罚

- **D0 缺陷密度降至 0.1-0.2**（成熟节点典型区间，与同期 TSMC N3B 相当），产量达 **~3 万片/月**（双厂）。
- **18A PDK 1.0 于 7 月发布**，外部客户可正式启动设计。
- Lip-Bu Tan 称代工为"国家瑰宝"，外部客户"敲门"，**多个外部客户将在 2026H2 正式进入量产**。
- **但**：INTC 7 月初单周暴跌 21%（-7.67% 至 $110.68），归因于"18A 良率延迟"叙事 + AMD 首次在数据中心营收上超越 Intel。

**判断**：技术拐点（D0 0.1-0.2）与市场叙事（"延迟"）出现背离。这对催化剂视角是**典型的预期差机会**——若 Q3 外部客户签约兑现，Intel 期权价值（Round 2 给 7% 权重）有上修空间。但 AMD 数据中心反超是结构性风险信号，需在退场标准中跟踪。★★

---

## 一、已发生催化剂回顾（2026-06-05 → 07-10）

| 日期 | 事件 | 方向 | 影响 | 来源 |
|------|------|------|------|------|
| 06.01 | 美国澄清 AI 芯片禁令适用于**境外中资企业** | ↓收紧 | ★★ | Al Jazeera |
| 06.上旬 | Computex：Intel 发布 Xeon 6+ Clearwater Forest（288 核 18A，量产）、Nova Lake 52 核、Panther Lake Arc G3 | ↑ | ★★★ | Tom's HW/TweakTown |
| 06.10 | TSMC 5 月营收 NT$416.98B（~$13.2B，+30.1% YoY，纪录） | ↑ | ★★ | Focus Taiwan |
| 06.14-18 | VLSI Symposium：TSMC A16 Super Power Rail 论文（量产目标 4Q26）；Intel 18A 实测 +30%@0.5V；18A-P 风险生产 | ↑ | ★★★ | vlsisymposium.org |
| 06月中 | Intel 18A D0 降至 0.1-0.2，产量 ~3 万片/月；Lip-Bu Tan"国家瑰宝"论 | ↑ | ★★★ | TechPowerUp/SemiWiki |
| 06月中 | NVIDIA 正式超越 Apple 成 TSMC 第一大客户（19% vs 17%）；TSMC sub-5nm 涨价 3-5% | ↑ | ★★★ | Ameya360/Medium |
| 06月 | Intel Foundry 18A-P 平台发布（VLSI），面向外部代工客户 | ↑ | ★★ | SemiWiki |
| 07.01 | SemiAnalysis：NVIDIA Rubin Ultra 4-die **取消**（CoWoS-L 翘曲），改双 die，2027 性能预期减半 | ↓ | ★★★ | SemiAnalysis/TechTimes |
| 07.07 | 美中缓和部分技术限制（芯片设计软件出口许可） | ↑缓和 | ★★ | YouTube 新闻 |
| 07上旬 | INTC 周跌 21%（-7.67% 至 $110.68），"18A 延迟"+AMD 数据中心反超叙事 | ↓ | ★★ | Phemex |
| 07.10 | TSMC 6 月月度营收公布日；Intel 18A PDK 1.0 发布（启用外部客户设计） | ↑ | ★★ | TSMC IR/Intel |
| 持续 | Samsung SF2 良率 ~55%（低于 60% 量产阈值），Qualcomm 可能转向 TSMC | ↓（对 Samsung） | ★★ | TrendForce |

**5 周净判断**：正面催化密集（VLSI + Computex + 18A 良率 + 客户结构质变），但被两件负面事件（Rubin Ultra 取消、INTC 股灾）部分对冲。**方向偏正面，但市场对 Intel 的预期已先行下修**。

---

## 二、关键催化剂深度分析

### 深度1：TSMC A16 Super Power Rail——背面供电商用时间表锁定

VLSI 2026 的 Late News 论文是 A16 自 2024 年公布以来**首次有实测硅数据**披露：
- **Super Power Rail（SPR）**：背面直接接触供电，将电源网络从信号层下方移至硅基底背面。
- 量产目标 **4Q26 风险生产 → 2027 量产**，与 Round 2 PM 给的"40% 推迟概率"形成对照——目前看按期概率上升。
- NVIDIA 已被多个来源（Wccftech/TradingKey）点名为 **A16 首发唯一客户**，原计划用于 Feynman GPU（2028）。但 Rubin Ultra 4-die 取消后，A16 的客户节奏可能调整——**这是需在 Q3 财报法说会上重点确认的变量**。
- imec 同步发表 CFET 背面接触改进论文——CFET（A10/1nm 节点）路线仍在推进。

**对投资论点影响**：H1（GAA 必经之路）+ H3（设备商确定性）继续强化。背面供电带来的**额外设备需求**（晶圆键合/解键合/背面图形化）是 KLAC/LRCX/AMAT 的增量订单来源。

### 深度2：Intel 18A 良率拐点 vs 市场惩罚——典型预期差

- **技术事实**：D0 = 0.1-0.2 是业界公认的高产量制造（HVM）成熟区间。Intel 达到此水平意味着 18A 从"工程样品"跨入"可商业化"。
- **市场反应**：INTC 7 月初周跌 21%。归因不是技术数据恶化，而是：（a）AMD 数据中心营收首次反超 Intel 的叙事冲击；（b）部分卖方对"18A 良率延迟"的旧叙事仍未更新；（c）Rubin Ultra 取消引发的 AI 芯片板块情绪传导。
- **前瞻催化**：18A PDK 1.0（7 月发布）+ 多个外部客户 2026H2 签约承诺（Lip-Bu Tan 公开表态）+ 14A PDK 0.9（10 月）。**若 Q3 财报披露具体外部客户名单，当前 $110 的 INTC 有期权价值修复空间**。
- **风险**：SemiWiki 指出 18A 在 Fab 52 **未满载运行**，Panther Lake 虽是好 CPU 但单价高。AMD 数据中心结构性反超若持续，Intel 代工"国家瑰宝"叙事会被侵蚀。

### 深度3：Rubin Ultra 取消——先进封装成为新瓶颈

- **技术根因**：CoWoS-L 4-die 集成中，~9.5X reticle 尺寸的硅互连在组装中产生基板翘曲，良率不达标。
- **影响**：（a）2027 年 NVIDIA 旗舰性能预期减半；（b）TSMC CoWoS-L 路线 credibility 受损；（c）市场开始重新评估"晶体管缩放 vs 先进封装"哪条路径更易触顶。
- **对 H4（每晶体管成本下降）的含义**：Round 2 已将 H4 下调至 55%。Rubin Ultra 取消说明**封装瓶颈正在间接推升每晶体管系统成本**（即使晶圆本身在降价）。这是 H4 进一步下行的先兆信号。
- **受益方**：先进封装设备商（ASML 高 NA、KLAC 检测、AMAT 键合）的"卖铲子"逻辑反而强化——封装难度越大，检测与工艺控制设备需求越刚性。

---

## 三、客户制程选择更新（谁倒向谁）

| 客户 | 制程选择 | 动态 | 信号强度 |
|------|---------|------|---------|
| **NVIDIA** | TSMC N2（Rubin）、A16（Feynman，首发） | 超越 Apple 成 TSMC 第一大客户（19% 营收）；要求 16 万片/月（被限 14 万）；Rubin Ultra 转双 die | ★★★ |
| **Apple** | TSMC N2（A20 iPhone 18） | 锁定初期 N2 产能 >50%；年采购 $20.7B | ★★★ |
| **Qualcomm** | 倾向 TSMC N2（远离 Samsung SF2） | Samsung SF2 良率 55% 不达标，Qualcomm 可能全面转 TSMC | ★★ |
| **AMD** | TSMC N2（首批客户） | 数据中心营收首超 Intel；传闻评估 Intel 14A 用于服务器 | ★★ |
| **MediaTek** | TSMC N2（首批） | 与 Apple/NVIDIA/AMD 同列首批 N2 客户 | ★ |
| **Intel Foundry 外部** | 18A（2 家评估中）、14A（2028 风险生产） | PDK 1.0 7 月发布；H2 2026 预期客户承诺；AMD/NVIDIA 传闻对 14A 有兴趣 | ★★（待兑现） |
| **Samsung SF2** | 自家 Exynos 2600 + 少量外部 | 良率 55%，客户流失风险高；Taylor Texas fab 上线 | ↓ |

**净判断**：TSMC 在 N2 客户名单上**进一步巩固垄断**（NVIDIA/Apple/AMD/Qualcomm/MediaTek 全在）。Intel 18A 外部客户"敲门"叙事需 Q3 兑现。Samsung 是明显输家，Qualcomm 倒戈 TSMC 概率上升。

---

## 四、未来 8-12 周催化剂日历

| 日期 | 事件 | 影响标的 | 方向 | 兑现概率 |
|------|------|---------|------|---------|
| **07.10**（今日） | TSMC 6 月月度营收；Intel 18A PDK 1.0 | TSM/INTC | ↑ | 100%（已发生） |
| **07.15** | ASML Q2 2026 财报（EUV 订单、High-NA 客户进展） | ASML | ↑/↓ | 100% |
| **07.16** | **TSMC Q2 法说会**（N2 营收%、A16 时间线确认、2027 CapEx 指引、Rubin Ultra 事件回应） | TSM/ASML | ↑/↓ | 100% |
| **07 下旬** | Intel Q2 财报（18A 良率数据、IFS 营收/亏损、外部客户披露） | INTC | ↑/↓ | 100% |
| **07 下旬** | Samsung Q2 财报（SF2 良率、代工订单） | 005930.KS | ↓偏 | 100% |
| **08 月** | TSMC N2P 量产启动（良率目标 80%+） | TSM | ↑ | 75% |
| **08-09 月** | Intel 18A 外部客户签约公告（Lip-Bu Tan 承诺 H2） | INTC | ↑ | 60% |
| **09.02-04** | **SEMICON Taiwan 2026**（量大量子区/智能 fab 区，先进封装/3DIC 议题） | 全板块 | ↑ | 100% |
| **10 月** | Intel 14A PDK 0.9 发布（客户可定稿设计） | INTC | ↑ | 90% |
| **Q4** | TSMC A16 风险生产（4Q26 目标，NVIDIA 首发） | TSM/ASML | ↑ | 70%（PM 给 40% 推迟） |
| **Q4** | TSMC N2 产能达 10 万片/月 | TSM | ↑ | 85% |
| **Q4** | ASML 全年 60+ 台 EUV 出货（含 High-NA 量产型） | ASML | ↑ | 90% |
| **11 月** | Hyperscaler 2027 CapEx 指引（K3 退场标准关键变量） | 全板块 | ↑/↓ | 100% |

---

## 五、对 Round 2 假设的增量验证（催化剂视角）

| 假设 | Round 3 催化剂视角 | 变化 |
|------|------------------|------|
| H1 GAA 必经之路 | **强确认**（VLSI 实测 +30%@0.5V；A16 SPR 论文） | 无变化（95%） |
| H2 EUV 不可替代 | **确认**（ASML 2026 €36-40B 营收指引；60→80 台 EUV） | 无变化（95%） |
| H3 设备商确定性 | **强化**（背面供电 + 先进封装带来增量设备需求） | 上行（88%→90%） |
| H4 每晶体管成本下降 | **进一步趋近中立**（Rubin Ultra 取消暴露封装成本上升） | 下行（55%→45%） |
| H5 TSMC 护城河 | **强化**（NVIDIA 登顶第一大客户 + 涨价 3-5% + N2 售罄） | 无变化（90%） |

---

## 六、未来最关键的 3 个催化剂（一句话总结）

1. **07.15-16 ASML+TSMC Q2 法说会**——N2 营收%、A16 时间线、Rubin Ultra 事件官方回应，是未来 1 周的方向定调事件。
2. **Intel 18A 外部客户签约（2026H2 承诺兑现）**——决定 INTC 7% 期权权重是上修还是清仓的关键。
3. **TSMC A16 风险生产（4Q26）**——PM 给 40% 推迟概率，VLSI 论文后按期概率上升，是背面供电商用的里程碑。

---

*来源：TSMC IR、ASML、Intel Newsroom、VLSI Symposium 2026 Tipsheet、SemiWiki、SemiAnalysis、Tom's Hardware、TrendForce、TechPowerUp、Focus Taiwan、Al Jazeera、Phemex。检索窗口 2026-06-05 → 07-10。*
