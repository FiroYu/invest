# Researcher C: AI基础设施与供应链研究报告

> **日期**: 2026年6月5日  
> **主题**: 课题 #01 — AI架构范式转移：JEPA vs LLM（基础设施与供应链视角）  
> **研究员**: Researcher C (Infrastructure & Supply Chain)

---

## 执行摘要

2026年的AI基础设施格局正处于历史性拐点：全球数据中心总支出超$650B，在建容量22GW，规划容量41GW——这是"一代人只出现一次"的基础设施建设浪潮。TSMC CoWoS产能到2026年底预计达130K晶圆/月，NVIDIA独占60%，GPU交付周期推至Q1 2027。HBM4已量产（三星2026年2月首发），边缘NPU进入45-50 TOPS时代（Apple M5 Max 614 GB/s带宽可运行70B模型）。同时，光子计算已实现1,000+ TOPS原型，IBM NorthPole芯片在推理效率上超越GPU 46-72倍。

**核心发现**：
1. 当前AI基础设施以LLM范式为中心建设，但新范式（JEPA/世界模型）可能在5-10年内从根本上改变硬件需求格局
2. Jevons悖论正在实时上演：效率提升（芯片每代性能翻倍）并未降低总能耗——数据中心耗电从2025年485 TWh预计增至2030年950 TWh
3. JEPA的算力优势（V-JEPA 2仅需60 GPU-years vs GPT-4级的1e25+ FLOP）可能在长期颠覆GPU需求结构，但短期看训练需求总量仍处于爆炸增长期

---

## 1. AI数据中心基础设施建设进度

### 1.1 全球数据中心容量现状（2026年6月）

| 指标 | 数值 | 来源 |
|------|------|------|
| 全球数据中心总数 | 11,038座 | Cloudscene, 2026.03 |
| 覆盖国家 | 174个 | Cloudscene |
| 美国数据中心 | 4,011座（占全球36%） | Cloudscene |
| 全球运营容量 | 49 GW | 行业共识 |
| 在建容量 | 22 GW | — |
| 规划容量（未开工） | 41 GW | — |

### 1.2 新增容量预测

- **JLL Research (2026)**：2026-2030年间将新增近**100 GW**数据中心，全球容量翻倍，CAGR约14%
- **ABI Research**：主权AI容量从2026年1.3 GW增至2031年3.1 GW，增长近3倍
- **Goldman Sachs**：全球数据中心容量需求到2030年可能翻三倍，AI工作负载占70%
- **IDCA (2026)**：AI正从根本上改变数据中心，增加大量新容量的同时提升效率和安全

### 1.3 超大规模云厂商资本支出（2026年）

| 公司 | 2026年CapEx | 重点 |
|------|-------------|------|
| Meta | $115–135B | Llama模型集群、AI训练基础设施 |
| Amazon (AWS) | $75–200B | 自定义芯片(Trainium 2)、AWS区域扩张 |
| Microsoft | $80B | Azure数据中心、OpenAI合作 |
| Alphabet (Google) | $75B | GCP、TPU基础设施、Gemini |
| Oracle | $8–10B | OCI云区域、AI GPU集群 |
| Apple | $500B (5年) | Apple Intelligence、私有云计算 |

> **五大巨头合计约$600-630B**，其中约75%直接投向AI基础设施。Meta的$115-135B约等于其2025年收入的67%。

### 1.4 数据中心建设支出

- 2026年总数据中心支出：**$650B+**（Synergy Research Group）
- 同比增长：**31.7%**
- 新建建设支出：**$128B**（JLL Research）
- 全球托管市场：**$78.4B**，CAGR 14.2%
- 到2030年计划投资总额：**$7万亿**（McKinsey/行业共识）

---

## 2. GPU / HBM / CoWoS产能扩张最新进展

### 2.1 TSMC CoWoS先进封装（系统瓶颈）

CoWoS是当前AI芯片供应链中最关键的硬瓶颈：

| 时间点 | CoWoS产能（晶圆/月） | 备注 |
|--------|---------------------|------|
| 2024年底 | ~35K | 基准线 |
| 2025年中 | ~75-80K | TSMC CEO: "sold out through 2025 and into 2026" |
| 2026年底（预计） | **120-130K** | TSMC加速扩产中 |

- **NVIDIA独占约60%**的CoWoS产能（约510K晶圆中大部分为CoWoS-L）
- Broadcom、AMD紧随其后
- TSMC在竹南、嘉义、台中、台南全线满载运营
- **新一代CoPoS技术推迟至2030 Q4之后**（延期约2年），意味着CoWoS生命周期延长

### 2.2 GPU供应状况（2026年）

**关键事实**：
- 数据中心GPU交期：**36-52周**
- Blackwell级（GB200 NVL72）硬件交付已滑入**Q1 2027**
- GB200 NVL72：72 Blackwell GPU + 36 Grace CPU，单一液冷计算架构，130 TB/s NVLink带宽
- 单机架功耗：**120-132 kW**（液冷115 kW，风冷17 kW）
- HBM3e总容量：13.5 TB/机架
- 机架重量：1.36公吨
- **下一代的Vera Rubin NVL144预计单机架功耗接近600 kW**

### 2.3 GPU供给危机：结构性而非周期性

不同于疫情时期的芯片短缺，2026年的GPU危机是**结构性**的，由三个力量驱动：

1. **超大规模厂商的资本支出规模**：五大巨头$600-630B的联合资本支出，多数锁定多年供应协议，挤压企业级买家
2. **TSMC CoWoS产能硬瓶颈**：即使扩产到130K/月，NVIDIA独占60%
3. **H100到Blackwell的代际转换**：积压需求在市场上集中释放

### 2.4 HBM4内存进入量产

**三星**（2026年2月12日宣布）：业界首个商业化HBM4量产：
- 持续传输速度：11.7 Gbps（最高13 Gbps）
- 采用4nm逻辑基础芯片
- 总带宽超2.8 TB/s
- 相比HBM3e大幅提升

**SK海力士**：与TSMC 12nm工艺合作，为NVIDIA Vera Rubin供应HBM4

**美光**：加速HBM4产能布局

> HBM3e供应在整个2026年已完全分配完毕。NVIDIA指定三星和SK海力士为Vera Rubin AI芯片的独家HBM4供应商。

### 2.5 替代加速器评估

| 方案 | 状态 | 适用性 |
|------|------|--------|
| AMD MI300X | ROCm生态改进明显，推理性能有竞争力 | 特定推理工作负载 |
| Google TPU v5e | 仅通过GCP提供 | 云端原生 |
| Amazon Trainium 2 | 仅通过AWS提供 | 云端原生 |
| Microsoft Maia 100 | 仅通过Azure提供 | 云端原生 |
| Groq LPU | 特定架构 | 推理专用 |
| Cerebras WSE-3 | 晶圆级芯片 | 特定训练任务 |

> **关键结论**：对于大多数企业，**未来18个月内NVIDIA仍是主加速器策略**，替代加速器在软件生态深度上仍落后CUDA生态相当距离。但在JEPA/世界模型场景下，可能不需要NVIDIA级别的高端GPU。

---

## 3. 边缘AI芯片发展

### 3.1 主流NPU对比（2026年）

| 芯片 | NPU算力 | 内存带宽 | 最佳场景 |
|------|---------|----------|----------|
| Apple M5 Max (40核GPU) | ~38 TOPS (NE + Neural Accelerators) | **614 GB/s** | 大型模型(70B+) |
| Apple M5 Pro (20核GPU) | ~38 TOPS (NE + Neural Accelerators) | 307 GB/s | 中型(14B–30B) |
| Apple M5 (基础版) | 16核Neural Engine | 153.6 GB/s | 小型(≤7B) |
| Qualcomm Snapdragon X Elite | **45 TOPS** | ~135 GB/s | Windows应用推理 |
| Intel Lunar Lake | ~48 TOPS (NPU 4) | ~120 GB/s | Copilot+轻薄本 |
| AMD Ryzen AI 300 | 50 TOPS | ~100 GB/s | Copilot+笔记本 |
| Intel Arrow Lake | 13 TOPS | 不等 | 桌面，有限AI任务 |

**关键洞察**：对于LLM推理，**内存带宽比TOPS更重要**。M5 Max的614 GB/s是它能运行70B模型的原因（非TOPS数字）。解码阶段（逐token生成）是内存带宽瓶颈，而非计算瓶颈。

### 3.2 Apple Silicon关键进展

- **M5 Max**可运行70B模型（Q4量化，约42 GB内存需求）
- Apple Neural Engine嵌入每个GPU核心（M5新特性），GPU和Neural Engine协作推理
- **Core AI框架**将在WWDC 2026（6月8-12日）发布，取代Core ML：
  - 统一设备端和Apple托管模型的Swift API
  - Foundation Models访问权限（驱动iOS 27升级版Siri的模型）
  - 可能支持第三方模型和MCP协议集成

### 3.3 Qualcomm / MediaTek动态

- **Qualcomm Snapdragon X Elite**：45 TOPS NPU，通过ONNX Runtime + QNN Execution Provider支持开发
- **MediaTek Dimensity 9600 Pro**：TSMC N2P 2nm工艺（2026年下半年），直接对标Apple
- **OpenAI手机**（传闻）：使用MediaTek Dimensity 9600定制版，TSMC N2P节点
- **边缘AI芯片市场**：预计到2036年超**$800亿**（Future Markets Inc.）

### 3.4 边缘AI对JEPA的潜在意义

JEPA的世界模型（如LeWorldModel仅15M参数，单GPU数小时训练）天然适合边缘部署：
- 小型世界模型可运行在手机/笔记本NPU上
- 不需要云端API调用
- 实时物理推理、机器人控制等场景

---

## 4. 神经拟态芯片与光子计算

### 4.1 神经拟态芯片：Intel Loihi 2 & IBM NorthPole

#### Intel Loihi 2
- 第二代神经拟态处理器，处理速度提升10倍（vs第一代）
- 模拟超**10亿神经元**
- 附带Lava开源软件框架
- 能源效率：比传统CPU/GPU高100-1000倍（特定稀疏工作负载）
- 局限性：**缺乏标准编程模型、软件生态有限、任务兼容性窄**，仍限于研究和利基边缘应用

#### IBM NorthPole（AI推理加速器）
- 消除片外内存，采用片上内存/存内计算架构（消除冯·诺依曼瓶颈）
- 12nm工艺，22B晶体管，795 mm²
- 片上内存带宽：**13 TB/s**
- 最新LLM推理结果：
  - **3B参数Granite LLM**：每token延迟<1ms
  - 比次优GPU快**46.9倍**
  - 能效高**72.7倍**
  - 16卡2U服务器：**28,356 tokens/s**
- 288卡垂直集成原型系统已构建（2025年11月论文）

> **对JEPA的影响**：NorthPole的能效和低延迟特性天然适合世界模型的实时推理——尤其是机器人控制和自动驾驶场景。

### 4.2 光子计算：下一代AI加速器

光子神经拟态计算2026年技术全景：

| 维度 | 指标 |
|------|------|
| 目标每MAC能耗 | **<1 pJ**（亚皮焦耳） |
| 速度加速 | **294倍** vs 电子基准（Princeton 2017） |
| 原型性能 | >1,000 TOPS（Homodyne光子张量处理器，2026年4月arXiv） |
| 光神经元频率 | GHz级（Strathclyde 2023，单个VCSEL实现完整SNN） |

**四大技术集群**：
1. **集成硅光子神经网络**（最大集群，CMOS兼容）——最接近商业化的路径
2. **VCSEL基脉冲光子神经元**（欧洲学术主导，GHz速率，超紧凑）
3. **光子忆阻/光电突触器件**（相变材料、铁电隧道结、钙钛矿量子点）
4. **储备池计算与非线性光子动力学系统**（单器件实现数百虚拟节点）

**地缘分布**：
- **中国**：最大创新集群（10+机构：上海交大、同济、浙大、华中科大、华为等），有2022年国家神经拟态器件路线图
- **美国**：系统级创新领先（Princeton、GWU、NIST、UC San Diego、Intel Labs、Qualcomm）
- **欧洲**：VCSEL和储备池计算领先（Strathclyde、Ghent-imec、CNRS、VUB）

**关键瓶颈**：**片上训练**仍是未解决的核心挑战——仅极少数团队（GWU、UC San Diego）在解决；推理占主导。

### 4.3 对JEPA世界模型的硬件启示

JEPA的架构特征天然匹配新型硬件的优势：
- **稀疏性**：JEPA的编码器-预测器结构天然稀疏，适合Loihi 2的稀疏SNN
- **低延迟**：北Pole的<1ms/token和光子计算的亚纳秒延迟，适合世界模型的实时推理
- **能效**：JEPA + 神经拟态/光子 = 可能达到100-1000倍能效提升
- **边缘部署**：LeWorldModel（15M参数）这种极小模型本就可在低功耗硬件上运行

---

## 5. AI电力需求预测

### 5.1 全球数据中心电力消耗

| 指标 | 数值 | 来源 |
|------|------|------|
| 2022年全球数据中心耗电 | 240-340 TWh | IEA |
| 2025年全球数据中心耗电 | 485 TWh | IEA (2026更新) |
| 2026年全球数据中心耗电（预估） | **~1,000 TWh** | 行业综合（含MedhaCloud/布鲁金斯） |
| 2030年全球数据中心耗电（IEA预测） | **~950 TWh** | IEA |
| 2026年占全球电力比 | **3.5-4%** | 综合估算 |
| 2030年占全球电力比 | **~3%** | IEA |
| AI工作负载专用耗电 | 200+ TWh | 行业估算 |

> **IEA关键报告**（2026年4月23日）：全球数据中心电力消耗预计到2030年翻倍至约950 TWh。IEA正在追踪超过**4,500个数据中心项目**，计划在2029年前开工。

### 5.2 AI训练 vs 推理：能耗结构的根本转变

- AI训练机架功耗：**40-100 kW**（传统计算仅6-10 kW）
- 推理已成为主导能耗：**占AI总能耗的80-90%**（UN报告，2026年6月）
- ChatGPT估计每天处理约**25亿次提示查询**
- 数据中心液冷采用率：**28%**（2023年仅8%）

### 5.3 核能协议

所有主要超大规模厂商均已签署核能协议：
- Microsoft
- Amazon
- Google
- Oracle

原因：AI数据中心需要基载电力，仅靠可再生能源无法在所需规模和可靠性上提供。

### 5.4 Jevons悖论在AI基础设施中的实证

- **1865年Jevons发现**：煤炭效率提升→煤价下降→需求激增→总消耗不降反升
- **2026年AI实证**：
  - GPU每代能效提升2-3倍
  - 但数据中心总耗电从2022年~300 TWh增至2026年~1,000 TWh（**3倍增长**）
  - 效率使单位推理成本下降→更多应用场景→总推理量爆炸
  - Mit研究（2025年）将AI能耗拆解为构建、供给、消费三阶段分析
- **JEPA场景下的Jevons悖论**：如果JEPA将算力需求降低10-100倍，理论上前沿模型训练门槛大幅降低→更多团队参与→更广泛应用→总需求反而可能增长（类似"价格降200倍→需求涨90倍"的规律）

---

## 6. 开源世界模型

### 6.1 Meta的JEPA系列（全部开源）

| 模型 | 发布日期 | 规模 | GitHub Stars | 许可 |
|------|---------|------|-------------|------|
| **V-JEPA 2** | 2025年6月 | 1.2B参数 | 3,854 ⭐ | MIT |
| **V-JEPA 2.1** | 2026年3月 | 升级版 | 同仓库 | MIT |
| **I-JEPA** | 2023年6月 | ViT-H/14 | Meta开源 | CC BY-NC |
| **V-JEPA** | 2024年2月 | — | — | CC BY-NC |
| **Point-JEPA / 3D-JEPA** | 2024 | — | — | — |
| **LeWorldModel** | 2026年 | **15M参数** | — | — |
| **C-JEPA** | 2026年 | — | — | — |

**关键仓库**：
- `github.com/facebookresearch/vjepa2` — V-JEPA 2主要仓库（MIT许可，**可商用**）
- `github.com/facebookresearch/jepa-wms` — JEPA世界模型物理规划（246 ⭐）

### 6.2 V-JEPA 2核心能力

- **训练数据**：>100万小时视频 + 100万张图片（VideoMix22M数据集）
- **两阶段训练**：
  - 第1阶段：无动作预训练（自监督）
  - 第2阶段：动作条件训练（仅需62小时机器人数据）
- **zero-shot机器人规划**：在新的未见环境中对未见物体实现65-80%拾取放置成功率
- **新基准**：IntPhys 2（物理直觉）、MVPBench（最小视频对）、CausalVQA（因果推理）
- **人类表现85-95%**，当前最佳模型远低于此

### 6.3 JEPA Wiki（社区知识库）

- URL: `mishig-jepawiki.hf.space`
- 涵盖：训练配方、数据集清单、collapse prevention机制、vision transformer、世界模型与规划
- 训练食谱记录了从**LeWorldModel (15M参数，单GPU，数小时)** 到**V-JEPA 2 (1B参数，60 GPU-years)** 的完整跨度

### 6.4 LeCun团队其他开源项目

- **DINOv2**（自监督视觉特征学习）
- **VideoSAUR**（视频自监督）
- **物理推理基准套件**：IntPhys 2、MVPBench、CausalVQA（全部开源，HuggingFace leaderboard）

---

## 7. JEPA训练计算需求 vs LLM训练

### 7.1 LLM训练成本（当前前沿）

| 模型 | 训练FLOPs | 估计训练成本 | 时间 |
|------|----------|-------------|------|
| GPT-4 (2023) | 2.1e25 | $78-100M+ | 2023 |
| Llama 3.1 405B | 3.8e25 | ~$50-80M | 2024 |
| GPT-4.5 | 6.4e25 | 估计$150-250M | 2025 |
| Claude Opus 4 | 1.5e26 | 估计$300-500M+ | 2025 |
| Grok-3 | **4.6e26** | 估计$500M-1B+ | 2025 |

**趋势**：
- 到2025年6月，已有**33个公开模型**训练量超1e25 FLOP（即GPT-4级别）
- 训练成本自2024年以来增长约**4倍**
- 2016年以来的长期增长：~2.4倍/年，每8个月翻倍（前沿实验室）
- **2026年的前沿模型可能接近10^26-10^27 FLOPs**

### 7.2 JEPA训练成本

| 模型 | 参数 | 训练计算 | 等效GPU |
|------|------|---------|----------|
| **V-JEPA 2**（完全分辨率） | 1.2B | ~60 GPU-years | 大型集群 |
| **V-JEPA 2**（渐进训练） | 1.2B | **~7 GPU-years**（8.4倍加速） | 中等集群 |
| **V-JEPA 2.1** | 升级版 | 两阶段，进一步优化 | — |
| **LeWorldModel** | **15M** | **单GPU，数小时** | 单个GPU |
| **C-JEPA** | — | 冻结编码器，仅训练预测器 | 极低 |
| **I-JEPA** | ViT-H/14 | 同计算预算下比MAE快**2-3倍**（wall-clock） | — |

### 7.3 直接对比：JEPA vs LLM

| 维度 | LLM（前沿） | JEPA（前沿） | 倍数差距 |
|------|------------|------------|----------|
| 最大模型参数 | ~2T+ (传闻) | 1.2B（V-JEPA 2） | ~1000x |
| 训练FLOPs | 10^25-10^26 | ~7-60 GPU-years等效 | — |
| 训练成本（$） | $100M-1B+ | ~估算$500K-5M | **20-2000x** |
| 推理需求 | 每个token需全模型前向 | 编码器+预测器（潜空间） | 更低 |
| 硬件需求 | 大规模GPU集群（千-万卡） | 可运行于单GPU甚至NPU | 轻量 |
| 非语言能力 | 主要语言 | 物理理解/预测/规划 | 互补 |

### 7.4 关键洞察

1. **V-JEPA 2的60 GPU-years vs GPT-4级模型的数百万GPU-years**：这是约**10-100倍量级的差距**，验证了JEPA降低算力需求的核心论点

2. **渐进训练技巧**可以将成本再降8.4倍（60→7 GPU-years）

3. **LeWorldModel (15M参数) 可在消费级硬件上运行**：这意味着JEPA的入门门槛极低，可能引发大量草根创新

4. **I-JEPA在同计算预算下比MAE高效2-3倍**：因为潜空间预测比像素重建更便宜

5. **但JEPA目前不做语言生成**——这是魔鬼辩护人的核心论点。LLM-JEPA尝试将两种范式融合（arXiv:2509.14252），但仍在早期阶段

6. **推理侧的对比更极端**：LLM推理需要逐token解码整个模型；JEPA世界模型在推理时只需编码当前状态并通过预测器前向传播

### 7.5 长期推演：Jevons悖论与JEPA

假设JEPA在未来5-10年将训练成本降低**50倍**，同时广泛取代LLM的部分应用场景：

- **乐观场景**：能效革命→AI总能耗下降
- **Jevons场景**（更可能）：训练成本下降50倍→全世界更多团队训练世界模型→前沿模型竞争维度从LLM转移到世界模型→训练总量增长→能效提升被需求增长完全抵消甚至反超
- 参考：GPU性能提升1000倍（过去10年），但数据中心总耗电不降反升3倍

---

## 综合结论

### 对基础设施投资的启示

1. **短期（1-3年）**：当前$650B+的基础设施赌注全部基于LLM/scaling law范式。如果JEPA范式在3年内取得突破，可能造成大量GPU/Capex的"搁浅资产"风险。

2. **中期（3-7年）**：硅光子/神经拟态芯片的成熟（2028-2030？）可能正好与JEPA世界模型的商用化同步，形成硬件-软件的协同突变。

3. **长期（7-15年）**：Jevons悖论表明，即使JEPA大幅降低单位计算成本，AI总能耗和基础设施投资**不会减少**——只会转向新范式下的新需求。

### AMI Labs的投资逻辑验证

- $1.03B种子轮对应的是"范式转移"的赌注
- **基础设施侧的数据支撑**：当前LLM训练成本$100M-1B+，V-JEPA 2仅需约$1-5M等效——100x+差距真实存在
- **风险**：Jevons悖论意味着JEPA成功≠算力需求下降；混合架构（LLM-JEPA）可能是必然路径
- **时机**：HBM4量产、TSMC N2节点、硅光子突破、北Pole 288卡系统——硬件基础正在为世界模型范式铺路

---

## 关键参考来源

1. JLL Research — 2026 Data Center Market Outlook
2. Synergy Research Group — Data Center Spending Tracker Q1 2026
3. IEA — Energy and AI Report (2026年4月)
4. TSMC / CNBC — NVIDIA Advanced Packaging Capacity (2026年4月)
5. Vamsi Talks Tech — GPU Supply Chain Crisis 2026
6. Epoch AI — Models Over 1e25 FLOP (2025年6月)
7. Meta AI — V-JEPA 2 Blog & Technical Report (2025年6月)
8. JEPA Wiki — Training Recipes (HuggingFace Spaces)
9. IBM Research — NorthPole LLM Inference Results
10. PatSnap — Photonic Neuromorphic Computing Landscape 2026
11. Samsung Newsroom — HBM4 Mass Production (2026年2月)
12. Nature — Data Centres Energy Doubling by 2030
13. DEV Community — On-Device AI 2026 Developer Guide
14. MedhaCloud — Data Center Statistics 2026
15. S&P Global — 2026 Trends in Data Center Services & Infrastructure
