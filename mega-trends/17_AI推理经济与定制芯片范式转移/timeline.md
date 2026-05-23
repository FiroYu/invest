# 议题23：AI推理经济与定制芯片范式转移 — 时间线

## 2020-2022：GPU统治训练时代

### 2020
- OpenAI GPT-3发布（175B参数），训练使用约10,000张V100 GPU
- NVIDIA A100发布，成为AI训练的"标准硬件"
- Google TPU v3在内部使用，但外部影响力有限
- AI计算需求几乎全部集中在训练阶段

### 2021
- 全球"大模型竞赛"开始：Google PaLM、Meta OPT、BLOOM等
- NVIDIA数据中心收入约$100亿，主要由训练需求驱动
- 台积电7nm/5nm产能被苹果和高通主导，AI芯片占比极小
- CoWoS封装产能尚未成为瓶颈

### 2022
- **11月**：ChatGPT发布，引爆全球AI热潮
- 推理需求开始快速增长，但GPU仍是唯一可行方案
- Google开始内部扩大TPU部署用于推理
- AWS推出Inferentia2（低推理成本实例）
- HBM3开始量产（SK Hynix领先）

## 2023：推理需求爆发元年

### Q1-Q2
- ChatGPT用户突破1亿，推理成本成为OpenAI的核心运营挑战
- Microsoft部署数万张H100用于Azure OpenAI Service推理
- NVIDIA H100发布并迅速成为"最紧缺的芯片"
- 推理成本估算：GPT-4级别模型每次查询约$0.03-0.06

### Q3-Q4
- LLM API价格战开始：OpenAI多次降价，GPT-3.5 Turbo降至$0.001/1K tokens
- Google宣布TPU v5e（推理优化版），对外提供Vertex AI推理服务
- AWS Inferentia2实例价格比GPU实例低50%+
- Broadcom确认多个定制ASIC设计中标（客户为Hyperscaler）
- CoWoS产能开始出现紧张信号
- AI推理开始占NVIDIA数据中心收入的30%+

## 2024：定制芯片崛起

### Q1-Q2
- NVIDIA B200/GB200发布，推理性能大幅提升但价格高昂
- Google TPU v5p部署用于Gemini模型推理
- Microsoft宣布Maia 100自研芯片（为OpenAI工作负载优化）
- Broadcom定制AI芯片收入达$80亿（2024年全年）
- Meta宣布与Broadcom合作的推理ASIC项目
- AI ASIC市场达$120亿

### Q3-Q4
- Token使用量加速增长，每月超过5万亿tokens
- CoWoS产能成为全行业瓶颈——TSMC月产能~2.5万片，需求>4万片
- SK Hynix HBM3E量产，$79亿EUV订单扩张产能
- Marvell宣布多个定制芯片设计中标
- TSMC AI收入占比突破20%
- 先进封装产能扩张计划：TSMC目标2025年月产3万片CoWoS

## 2025：推理战争全面展开

### Q1-Q2
- NVIDIA推理收入占比突破50%——推理正式超过训练成为GPU核心用途
- Broadcom定制芯片收入快速增长，2025年预计$150-200亿
- Google TPU v6（下一代）进入测试
- AWS Trainium2量产并开放客户使用
- 推理成本持续下降：GPT-4o级别模型降至约$0.005/1K tokens
- 边缘AI推理芯片（Qualcomm、MediaTek）进入手机/PC

### Q3-Q4
- LLM token使用量持续飙升
- AI基础设施投资2025年预计超$2,000亿（全球）
- TSMC AI收入占比接近30%
- CoWoS产能扩张至月产~3万片，但仍供不应求
- 多家Hyperscaler的定制ASIC进入量产阶段
- AI推理"成本效率"成为企业选择云厂商的关键指标

## 2026（至今）：范式转移加速

### 2026年1月-4月
- LLM token使用量从1月6.4万亿增至4月22.7万亿（+250%）
- Broadcom定制AI芯片收入继续攀升
- CoWoS产能仍为瓶颈，TSMC计划进一步扩张
- NVIDIA Blackwell Ultra出货，推理性能进一步提升
- Qualcomm AI PC芯片出货量增长
- Morgan Stanley预测2028年AI基础设施投资约$3万亿
- AI ASIC市场预计2027年达$300亿+

## 2027-2029：架构多元化时代

### 2027（预期）
- AI ASIC市场达$300亿+
- Broadcom定制芯片收入达$300-400亿
- 至少3-4家Hyperscaler大规模使用自研推理芯片
- CoWoS产能瓶颈缓解，月产能达5万片+
- HBM4量产，内存带宽进一步提升
- 推理成本降至2024年的1/10以下

### 2028（预期）
- AI基础设施投资约$3万亿（Morgan Stanley估计）
- 推理占AI计算需求的90%+
- 边缘AI推理（手机、汽车、IoT）成为重要增长点
- GPU在推理中的份额从~90%降至~60-70%
- ASIC+专用推理加速器占~30-40%

### 2029（预期）
- AI芯片架构多元化完成：GPU/ASIC/FPGA/光计算混合部署
- 推理效率提升使"AI无处不在"成为经济上可行的现实
- 中国国产AI芯片（华为昇腾、寒武纪）在特定场景中有竞争力
- 先进封装技术演进：CoWoS之后的新一代3D封装

---

*最后更新：2026.05.21*
