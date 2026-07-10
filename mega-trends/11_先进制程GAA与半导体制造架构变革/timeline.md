# 议题13：2nm/GAA/背面供电 — 时间线

## 历史回顾

### 2011年
- **FinFET架构由Intel率先商业化（22nm）**：Intel在Ivy Bridge处理器中首次采用FinFET（鳍式场效应晶体管），取代平面晶体管。FinFET通过将沟道竖起形成"鳍"状，增强栅极对沟道的控制，显著降低漏电。这一架构统治了半导体行业超过10年（22nm→14nm→10nm→7nm→5nm→4nm→3nm）。

### 2022年
- **Samsung率先在3nm引入GAA（GAA-NM）**：Samsung Foundry在SF3节点首次采用GAA纳米片（Samsung称为MBCFET - Multi-Bridge Channel FET），比TSMC更早一步。但初期良率较低（ reportedly <50%），限制了商业影响。

### 2023年
- **ASML首台高NA EUV交付Intel**：ASML将第一台High-NA EUV（Twinscan EXE:5000）交付Intel在俄勒冈的D1X工厂。数值孔径从0.33提升到0.55，分辨率从13nm提升到8nm，是EUV技术的重大飞跃。这台设备价值约3.5亿欧元。

## 当前阶段（2025-2026）

### 2025年Q4
- **TSMC N2（GAA）开始量产**：TSMC在新竹和台南的Fab 20开始N2制程量产。良率约70%，高于预期。Apple的A20芯片和NVIDIA的下一代GPU是首批客户。N2采用GAA纳米片架构，相比N3E在相同功耗下性能提升15%，或在相同性能下功耗降低30%。

### 2025年底
- **Samsung SF2（GAA）开始量产**：Samsung Foundry的2nm节点SF2进入量产。Samsung在GAA上有先发优势（从SF3开始积累经验），但良率仍是挑战（估计50-70%）。Qualcomm是主要客户之一。

### 2026年
- **TSMC N2P改进版**：N2的优化版本，进一步提升良率和性能。预计良率达到80%+。
- **Intel 18A首批芯片出货**：Intel的1.8nm等效节点（18A）首次同时采用GAA（Intel称为RibbonFET）和背面供电（Intel称为PowerVia）。这是Intel代工复兴的关键里程碑，但已从原计划的2025年延迟至2026年。
- **ASML出货60台EUV**：2026年是ASML的EUV出货高峰年之一，包括标准EUV（NXE:3800）和首批量产型高NA EUV（EXE:5200）。

### 2026年Q2-Q3（Round 3，07.10）— H4叙事裂痕 + PE泡沫 + CapEx融资脆弱
- **每美元晶体管数首次倒退（本轮核心）**：Exponential View 数据显示 N2 节点 transistors/$ 从 562M 降至 **412M**——该指标首次出现实质性倒退。N2 晶圆 $30K（+50-66% vs N3 $18-20K），mixed-design 密度仅 +15%，15% 密度无法覆盖 60% 涨价 → 每晶体管硬成本上升 ~35%。A16 传闻 $45K（+50%）。Simon-Kucher 定性宣告"自动降本时代终结"。H4 从 55% 下调至 **40%**，叙事从"持续降本驱动民主化"修订为"溢价性能驱动集中化"。K5 接近触发（70% 概率 12 月内）。
- **设备商全板块 PE 泡沫化（互联网泡沫水平）**：半导体指数 ~60x。ASML PE(TTM) **47-48x**（R2 39x，已破 45x 减仓纪律，Morningstar 下调至 Sell）；LRCX ~60x（涨幅 52.7% 中 40.9% 来自 PE 扩张）；KLAC ~61x；TSM PE(Fwd) 23.4→27.7x。LRCX/KLAC 新增 PE>55x 减仓纪律。
- **Intel 18A 失去 NVIDIA**：Reuters 确认 NVIDIA 测试后退出 18A，外部客户移至 18A-P/14A-E（2027/28）。但 D0 降至 0.1-0.2 进入 HVM 成熟区间，PDK 1.0 七月发布——技术拐点与客户流失并存，INTC 减仓 7%→5%（非清仓）。
- **High-NA EUV 遭 TSMC 公开弃用**：TSMC 确认 A16/A14 不用 High-NA（Bloomberg "too pricey"），Intel 成唯一领先客户。ASML 垄断地位不变（Low-NA 仍是刚需，积压 €38B+，2027 产量近翻倍），但 High-NA 商业化节奏慢于预期，ASML 长期 SAM 扩张期权需打折。
- **AI CapEx 进入融资驱动阶段**：Goldman 预测 $1.15T 至 2027、TSMC N2 售罄至 2027Q2 确认短期管线；但 Amazon TTM FCF 转负、Oracle $40-50B 融资、PIMCO 称 94% 靠 OCF 不可持续。CoreWeave 金丝雀活跃（债务 + Chanos 做空）。K3 预警温度上调，AI CapEx 崩塌概率 15%→**20%**。
- **Rubin Ultra 4-die 版取消**：CoWoS-L 基板翘曲迫使改双 die，2027 峰值性能减半。封装物理极限开始结构性限制 NVIDIA 路线图斜率。7/16 TSMC 法说会列为重点确认项。
- **长端利率上行**：10Y UST **4.54%（+24bp）**，收益率曲线陡峭化，成长股 PE 压力（#05 利率传导上调至中高）。
- **WFE 上修**：KLA 上调至 ~$140B，AMAT 称增长 >30%。
- **VLSI 2026 硅验证**：A16 Super Power Rail 实测论文；Intel 18A +30%@0.5V 实测。H1/H2 技术护城河进一步确认。
- **CIO Round 3 裁定（07.10）**：评级降级至「有条件通过」（通过→有条件通过）；H4 55%→40%；现金 5%→18%（释放 13pp）；ASML 12%→8%（触发减仓）、LRCX 18%→15%、KLAC 15%→12%、INTC 7%→5%、AMAT 10%→12%（唯一加仓）、TSM 28%→25%；加权回报 +5.3%→~+1.1%。保留 4 条件（TSMC Q2 N2营收>5%+毛利≥65% / ASML Q2 EUV积压≥€35B / Hyperscaler 2027 CapEx+15%+ / K5未被A16确认）。**Round 3.5 非常规窗口：7/15 ASML Q2 + 7/16 TSMC Q2 验证**。

## 前瞻（2026年底-2029）

### 2026年底-2027年
- **TSMC A16（"Super Power Rail"背面供电）**：TSMC的背面供电方案，将电源网络从晶体管前侧移到晶圆背面。与N2的GAA架构叠加，进一步提升性能和密度。预计2027年开始风险生产（risk production），2027年底-2028年量产。
- **Intel PowerVia验证**：Intel的背面供电方案在18A节点首次商用。PowerVia的性能数据将决定Intel代工的技术竞争力。

### 2027年
- **ASML交付10台高NA EUV**：Intel是首个大规模采用者。高NA EUV允许单次曝光完成更精细图案，减少多重曝光步骤，但代价是更大的机器和更小的视场（需要拼接）。
- **A16节点竞争白热化**：TSMC A16 vs Intel 14A vs Samsung SF1.4，三大代工厂在1.6nm等效节点展开正面竞争。

### 2028-2029年
- **1.4nm/1nm节点开发**：TSMC的A14（1.4nm）和A10（1nm）节点进入开发。GAA纳米片可能演进为CFET（互补场效应晶体管），将N型和P型晶体管垂直堆叠。
- **高NA EUV成为标配**：到2028-2029年，所有先进制程都将需要高NA EUV。ASML的垄断地位进一步巩固。
- **背面供电全面普及**：所有主要代工厂在1.4nm及以下节点采用背面供电技术。
