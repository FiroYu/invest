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
