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

### 2026年Q2-Q3（Round 3，07.10）— ASIC 范式确立 + 过剩信号浮现
- **ASIC 范式确立**：NVIDIA 推理单位份额从 ~95% 降至 **62-66%**。四大 Hyperscaler 全部推出/量产自研芯片——Microsoft Maia 200（10,200 TFLOPS FP4，驱动 GPT-5.2）、Google TPU v7 Ironwood GA（TCO 比 GB200 低 44%，Anthropic 3.5GW 协议）、AWS Trainium 4（288GB HBM）、Meta MTIA 400（9月量产）。Broadcom 锁定四大合同（OpenAI 10GW + Meta 多-GW + Google LTA 至 2031 + Anthropic 3.5GW），Hock Tan 公开 >$100B 2027 AI 收入目标。但 NVIDIA 收入仍 +95%——"份额降、收入升"结构性窗口持续。子论点1 升级为"通过"。
- **2026.06.30-07.01 Rubin Ultra 四芯版取消**：CoWoS-L 基板翘曲迫使改双两芯，2027 算力减半。封装物理极限开始结构性限制 NVIDIA 路线图斜率，反讽利好 ASIC（单芯设计受 CoWoS-L 翘曲影响小）。
- **2026.07.01 Meta 转卖方信号（本轮最关键）**：Meta 宣布对外销售 GPU 算力（Meta Compute），成为首个从超级买方转为卖方的 Hyperscaler；xAI 已向 Google 卖算力；NVDA 被曝从 neocloud 回租产能。子论点3（GPU 过剩）升级为"警报级技术关注"，新增 K9（买方转卖方）为最高优先级预警。
- **NVDA 估值重定价**：Forward PE 从 Round 2 的 25.5x 压至 **20-22x**（7年低），PEG 0.45；股价较 ATH 回调 -14%，YTD 仅 +4%（vs SOXX +75%）。CIO 裁定"justified cheap"——非洼地非陷阱，仓位 25-30%→22-28%、入场 $222→$195-210、止损 $168。
- **Hyperscaler CapEx 加速但 FCF 崩溃（同源相反）**：2026 指引 $710-725B（+77%），BofA/Moody's 预测 2027 破 $1 万亿；但 Amazon TTM FCF $38.2B→$1.2B（-95%）、Oracle -$23.7B。靠融资非 OCF 驱动（AI IG 倵 $121B +332%、Alphabet $85B 股权增发超额认购）。断裂概率 20-25%。
- **API 定价战白热化**：Meta Muse Spark $4.25/M、OpenAI 考虑大降、Google Plus -37%。K5 早期预警，定价权侵蚀从 2028+ 前移至 2027H1。
- **H100 spot 触及 $0.79-1.40**（市场云），但 B200 仍紧俏（$2.35-7.00/hr）——"二级市场过剩、一级市场仍紧"分化确认。

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

---

## 2026年7-8月：Round 4 捕获窗口关键事件（09.03 CIO 综合）

- **07.01**：Bloomberg 曝光 Meta Compute 商业计划（卖冗余算力+托管模型）——META 当日 +8.8%，neocloud 板块杀跌；后续报道 9 月与自研 ASIC Iris 投产同步启动（定价未官宣）。
- **07.21**：Nikkei——TSMC 2027 年 1 月起先进制程+先进封装涨价至多 10%；CoWoS 三座后段厂 2027 年前产能全部售罄、交期 52-78 周。
- **07.28-31**：四大 Hyperscaler Q2——2026 CapEx 全部上调（合计 ~$733B）：Alphabet $195-205B（财报被"panned" -7%）、Amazon ~$220B（"产能到 2027 追不上需求"）、Meta $130-145B（FCF -91% 至 $784M、单季发债 $24.9B）；四家滚动 FCF 合计转负（-$7.6B，2023 以来首次）。
- **07.29**：CoreWeave 5Y CDS 一度飙至 ~855bp（隐含 5 年违约 ~50%）——**K12 触发**；随后 $8.5B IG 评级 GPU 融资+$2.6B DDTL 落地（8/10），Fitch 给 BB，再融资墙推至 2027-28。
- **07.30**：OpenAI GPT-5.6 Luna 直降 80%（$0.20/$1.20/M）+ Gemini 同期 -67% + Claude -67%——**K5 形式触发**（三家同季 >50%）；8/30 Silicon Data 单价指数 $1.0018/M 历史新低。
- **08.11**：CoreWeave Q2——收入 $2.575B（+112%）、backlog $104B（+246%）、净亏 $626M、单季利息 $640M。
- **08.26**：**NVDA Q2 FY27**——营收 $96.22B（+106%，超 $91B 指引 5.7%）、DC $89.0B（+117%）、Q3 指引 $108B±2%、FY28 ~+70% 供给受限框架、Rubin 全面量产（Q3 占 DC ~20%）；盘后 +4%。
- **08 月**：Amazon 被报道首家回撤服务器折旧年限（6→5 年）——**K10 预警升级**；Burry"2026-28 折旧少提 $176B"论发酵。
- **08-09**：MRVL Q2 FY27（$2.739B 纪录+FY27 上调 $12B，股价仍 -2%）；私募信贷违约率 6.1% 创纪录（Fitch）；DRAM 2025-27 累计 +275-300%（存储通胀）。
- **09.02**：**AVGO Q3 FY26**——AI 收入 $16.7B（+221%）、FY26 上调 $58B、Hock Tan 首次给出 FY27 $115B/FY28 $230B 路线图+新客户 $10B 订单；Q4 总收入指引差 $230M 致 -5%。
- **09.03**：Round 4 CIO 综合——核心论点维持「通过」（注记升级金融可持续性预警）；K5/K12 双触发；K12 分步执行（NVDA 20-25%、现金 18-20%，11/1 二步裁定）。
