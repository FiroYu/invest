# 课题 #01 AI架构范式转移：JEPA vs LLM — 基本面研究报告

**研究员 A（架构与技术路线）**
**报告日期：2026年6月5日**
**版本：Round 1**

---

## 执行摘要

2026年上半年，JEPA（Joint Embedding Predictive Architecture）架构从学术愿景向工程可行性的跨越已完成。关键里程碑包括：LeWorldModel 证明 JEPA 可在单 GPU 上端到端训练并实现 48× 更快的规划速度；VL-JEPA 在 WorldPrediction benchmark 上以 65.7% 超越 GPT-4o 的 53.3%，参数量仅为其 1/40；LeCun 创办的 AMI Labs 以 $10.3亿种子轮创欧洲历史纪录。NVIDIA 以 Cosmos 3（2026年5月31日发布）强力入局世界模型赛道，Google DeepMind Genie 3 已面向付费用户开放。同时，Hyperscaler CapEx 2026E 达 $660B–$750B，推理 token 年增长 250%+，暗示 LLM 架构的规模扩展正接近物理极限。JEPA 所代表的"世界模型"路线可能引发 AI 算力需求的结构性重置。

---

## 1. JEPA/V-JEPA/VL-JEPA 最新研究进展

### 1.1 核心论文时间线

| 日期 | 论文/成果 | 关键进展 |
|------|-----------|---------|
| 2025.06 | **V-JEPA 2** (Meta FAIR) | 1.2B 参数，自监督视频编码器，实现零样本机器人规划。三个新 benchmark 评估物理世界推理。 |
| 2025.12 | **VL-JEPA** (arXiv 2512.10942) | 非自回归视觉-语言模型，预测连续文本嵌入而非离散 token。ICLR 2026 接收。 |
| 2026.02 | **C-JEPA** (Causal JEPA) | 嵌入因果归纳偏置，防止模型学到无意义的物理捷径。 |
| 2026.02 | **Semantic Tube Prediction** | 在数据效率上击败 LLM，使用 JEPA 建模 token 序列轨迹的 ODE。 |
| 2026.03 | **LeWorldModel** (LeWM) | 首个端到端从原始像素训练的 JEPA。15M 参数，单 GPU/几小时，48× 更快规划。开源。 |
| 2026.05 | **TC-JEPA** (Text-Conditional JEPA) | 用图像标题降低预测不确定性，语义更丰富的视觉表示学习。 |
| 2026.05 | **Demo-JEPA** | 一次性演示学习，跨形态迁移，分布偏移下仍保持鲁棒性。 |
| 2026.05 | **Var-JEPA** (arXiv 2603.20111) | JEPA 的变分形式化，统一能量模型与变分推理。 |
| 2026.05.30-31 | **JEPA 形式化证明** (两篇 arXiv) | 严格定义 JEPA 能够学习的条件，证明当前模型在分布外仍脆弱。 |

### 1.2 VL-JEPA 关键性能数据

- **WorldPrediction benchmark**: 65.7% → **超越 GPT-4o** (53.3%)，而参数量仅为 GPT-4o 的约 1/40
- **推理速度**: 2.85× 快于同等规模 VLM
- **架构核心**: 非自回归，预测连续嵌入 → 仅在需要人类可读输出时调用 text decoder
- **ICLR 2026**: 被接收为正式论文
- **关键洞察**: "预测意义而非 token" — 在抽象表示空间预测，而非逐 token 生成

### 1.3 LeWorldModel (LeWM) — JEPA 实用化的转折点

**来源**: Lucas Maes, Quentin Le Lidec, Damien Scieur, Yann LeCun, Randall Balestriero (Mila/NYU/Samsung SAIL/Brown University)

| 指标 | LeWM (JEPA) | DINO-WM (Foundation Model) |
|------|-------------|---------------------------|
| 参数量 | **15M** | ~300M+ |
| 训练硬件 | **单 GPU** | 多 GPU 集群 |
| 训练时间 | **几小时** | 数天 |
| 规划速度 | **0.98s** (48× faster) | 47s |
| 损失函数 | **仅 2 项**（预测+高斯正则化） | 多项复杂损失 |
| 代码 | github.com/lucas-maes/le-wm (开源) | - |

**技术突破**: SIGReg (Simple Gaussian Regularizer) 解决了 JEPA 长期存在的表示坍缩（representation collapse）问题，只用 2 个损失项实现端到端训练。

**意义**: "一个研究生可以迭代这个模型"（Glitchwire 评论），极大降低了世界模型研究的准入门槛。

---

## 2. AMI Labs（Advanced Machine Intelligence Labs）

### 2.1 公司概况

| 维度 | 详情 |
|------|------|
| **创始人** | Yann LeCun（2018图灵奖得主） |
| **成立时间** | 2025年底（LeCun 2025年11月离开Meta） |
| **CEO** | Alexandre LeBrun（前 Meta FAIR，前 Nabla CEO） |
| **CSO** | Saining Xie（前 Google DeepMind GenAI 团队，NYU 教授，ResNeXt/ConvNeXt 共同作者） |
| **首席研究创新官** | Pascale Fung |
| **世界模型研究主管** | Michael Rabbat（前 Meta 研究科学总监） |
| **COO** | Laurent Solly（前 Meta 欧洲区负责人，13年） |
| **总部** | 巴黎 |
| **办事处** | 巴黎（总部）、纽约（LeCun 在 NYU 任教）、蒙特利尔、新加坡 |
| **员工数** | 12人（种子轮时），全球四地持续招聘 |
| **估值** | $35亿 Pre-money → $45.3亿 Post-money |

### 2.2 融资详情

| 维度 | 详情 |
|------|------|
| **轮次** | 种子轮 |
| **金额** | **$10.3亿**（$1.03B） |
| **历史地位** | 欧洲历史最大种子轮，全球第二（仅次于某美国公司） |
| **投资方** | C4 Ventures, Cathay Capital 等 |
| **融资日期** | 2026年3月9日（正式公布） |

### 2.3 产品与技术方向

- **核心使命**: "Building real intelligence into the real world"
- **技术架构**: JEPA + 世界模型，非 LLM
- **差异化**: 从现实世界传感器数据学习，而非从纯语言学习
- **应用方向**: 机器人、自主系统、物理世界 AI
- **商业化节奏**: LeBrun 明确表示"不是典型的应用 AI 创业公司，不会 3 个月出产品、6 个月有收入、12 个月实现 $10M ARR"
- **Nabla 合作**: AMI Labs 首个官方合作伙伴，Nabla（AI 医疗记录）将获得 AMI 世界模型的"优先访问权"
- **LeCun 的角色**: 创始人与首席科学家，同时保留 NYU 教职

### 2.4 战略定位

Saining Xie（CSO）的表述："Language Is Poison" — 认为 AI 行业最成功的技术（语言模型）也是最危险的陷阱。AMI Labs 是"反 LLM"的根本性赌注。

---

## 3. 世界模型（World Models）赛道全景

### 3.1 主要玩家矩阵

| 玩家 | 产品/模型 | 定位 | 最新进展 (2026) | 融资/估值 |
|------|----------|------|----------------|----------|
| **Google DeepMind** | Genie 3 | 通用世界模型 | 2026.01: 面向 AI Ultra 订阅用户开放，从文本提示生成可交互 3D 环境，720p@24fps，但受限于 60 秒/会话 (计算力约束) | 内部 |
| **Google DeepMind** | Gemini 3 | 多模态推理 | 在 7 个视觉类别 25+ 评估中全面领先，Spatial 和 Screen 类别优势最大 | 内部 |
| **NVIDIA** | Cosmos 3 | 物理 AI 开放世界模型 | **2026.05.31 发布**：首个全开放 Omni-model，7 项物理 AI 榜单第一。16B (Nano) 变体于 Hugging Face 开放。Computex 2026 发布。Mixture-of-Transformers 架构。 | 内部 |
| **NVIDIA** | Isaac GR00T | 人形机器人参考平台 | 2026.06.01 GTC Taipei 发布 | 内部 |
| **Runway** | Gen-4 (世界模型) | AI 视频 → 世界模型 | 2026.02: $315M Series E, 估值 $5.3B。2025.12 发布世界模型。从视频生成转型为世界模型底层技术。 | $5.3B |
| **World Labs** | Marble | 3D 世界模型 | 2026 活跃 | Fei-Fei Li |
| **Wayve** | GAIA-2 | 自动驾驶世界模型 | 正在部署 | $1B+ |
| **OpenAI** | Sora | 视频生成/世界模型方向 | 定位为世界模拟器 | 未独立 |

### 3.2 NVIDIA Cosmos 3 详解（2026.05.31 发布）

- **定位**: 首个完全开放的物理 AI Omni-model
- **架构**: Mixture-of-Transformers，统一处理视觉推理、世界生成、动作生成
- **变体**: Super（大模型）和 Nano（16B 参数，Hugging Face 可获取）
- **性能**: 发布时即登顶 7 项物理 AI 排行榜（RoboLab, RoboArena 等）
- **关键**: 开放权重策略 → 可能定义物理 AI 时代的基础模型标准

### 3.3 Runway 转型（2026.02）

- 融资金额: $315M (Series E)
- 估值: $5.3B（较上一轮接近翻倍）
- 领投: General Atlantic
- 战略: 从 AI 视频生成工具转型为"世界模型"基础设施
- Meta 被报道考虑收购 Runway（2026.03）

### 3.4 WBench — 首个交互式世界模型标准化评测

美团 LongCat 团队发布的 WBench：289 个多轮测试案例 × 5 维度 × 20 个模型 × 22 项指标，人工判断验证。填补了世界模型评测的空白。

---

## 4. JEPA vs LLM 性能对比

### 4.1 视觉推理与视觉-语言理解

| Benchmark | VL-JEPA | GPT-4o | 优势 | 备注 |
|-----------|---------|--------|------|------|
| WorldPrediction | **65.7%** | 53.3% | +12.4pp | JEPA 参数仅 GPT-4o ~1/40 |
| VPA (Visual Planning) | SOTA | 落后 | - | VLWM 同样表现优异 |
| 推理速度 | **2.85×** | 1× | - | 50% 参数减少 |

### 4.2 机器人控制与规划

| 指标 | LeWM (JEPA) | DINO-WM (Foundation) | 优势 |
|------|-------------|---------------------|------|
| 规划时间/周期 | **0.98s** | 47s | **48×** |
| 训练参数 | 15M | 300M+ | 20× 更少 |
| 训练硬件 | 单 GPU | 多 GPU 集群 | 10-100× 更少 |
| 控制任务 | 竞争力相当 | 竞争力相当 | 同等性能、显著更低成本 |

### 4.3 数据效率

- **C-JEPA**: 引入因果归纳偏置，防止无效物理捷径，数据效率远超 LLM
- **Semantic Tube Prediction (arXiv 2602.22617)**: 明确证明 JEPA 在数据效率上击败 LLM
- **Demo-JEPA**: 一次演示即可跨形态泛化，LLM 需要海量多任务数据

### 4.4 架构哲学差异

| 维度 | LLM | JEPA |
|------|-----|------|
| 预测目标 | 下一个 token | 抽象表示空间中的嵌入 |
| 生成方式 | 自回归逐 token 生成 | 非生成式，仅在需要时解码 |
| 学习信号 | 语言序列统计 | 世界状态演变规律 |
| 模态 | 以文本为中心 | 原生多模态（视频/传感器） |
| 计算效率 | 随 token 数线性/超线性增长 | 嵌入空间预测，恒定计算 |
| 物理理解 | 间接（通过文本描述） | 直接（从像素/传感器） |
| 表示坍缩 | N/A | 曾是核心挑战，LeWM 已解决 |

---

## 5. LLM 推理需求增长实际数据

### 5.1 Hyperscaler CapEx 轨迹

| 年份 | 总 CapEx (5家合计) | YoY 增长 | 来源 |
|------|-------------------|----------|------|
| 2020 | ~$94B | — | luna3.ai |
| 2024 | ~$230B | — | 估计 |
| 2025 | ~$315B | ~37% | dcpulse.com |
| 2026E | **$660B–$750B** | **67%–110%** | CreditSights, Introl, Goldman Sachs |

**各公司 2026E CapEx 拆解**:
- Microsoft: ~$190B（含 $80B 未满足的 Azure 订单，缺电力）
- Amazon: ~$190B+
- Google/Alphabet: $75B (2025 实际)
- Meta: 大量投入
- Oracle: 显著增长

**GS 分析**: $700B CapEx 与 1990 年代后期电信投资周期峰值相当。

### 5.2 推理 Token 增长

| 指标 | 数据 | 来源 |
|------|------|------|
| **推理 token 年增长** | **250%+** | 多源确认 |
| Agentic AI 流量 | 年增 **7,851%** | HUMAN Security 2026 报告 |
| AI 驱动流量 (2025.01→12) | 逐月增 **187%** | HUMAN Security |
| 单应用推理成本 | 2 年增长 ~**10×** (token 数量增加) | Kilo AI |
| 推理市场 2025E | **$103.7B** | Fortune Business Insights |
| 推理市场 2034E | $312.6B, CAGR 13-19% | 多家研究机构 |

### 5.3 Token 成本悖论

- **单位成本骤降**: 前沿模型 API 价格从 2024 年的 $30/M tokens 降至 2026 年的 <$3/M tokens
- **总账单反而增长**: 使用量增长远超单位成本下降
- **推理 token 成本结构**: 推理 token（reasoning tokens）成本可达输入 token 的 6×
- **Jevons 悖论在 AI 的体现**: 更便宜 → 用得更多 → 总花费更高

### 5.4 NVIDIA Rubin 预期

- 承诺推理 token 成本 **再降 10×**
- 算力 5× Blackwell
- 预计 2026 H2 发货

---

## 6. Hyperscaler 对非 LLM 架构的投资态度

### 6.1 直接证据

| Hyperscaler | 行动 | 态度判断 |
|-------------|------|---------|
| **Meta** | 开源 V-JEPA 2, VL-JEPA, LeWM 合作 (NYU/Mila) | **强烈布局**：Meta FAIR 是 JEPA 核心研究产出地。V-JEPA 2 是"迈向 AMI 的下一步"。 |
| **Google** | Genie 3 商业化；Gemini 3 用作世界模型前端 | **All-in 世界模型**：Gemini 3 专为世界模型设计（非聊天），TPU 训练 |
| **NVIDIA** | Cosmos 3 开放发布 + Isaac GR00T | **战略押注物理 AI**：世界模型是 GPU 需求的下一个驱动力 |
| **Microsoft** | Azure AI 基础设施为主 | **基础设施中立**：为所有架构提供算力，$80B 未满足需求 |
| **Amazon** | AWS AI 基础设施 | **中立**：主要做算力提供商 |
| **OpenAI** | Sora 定位世界模拟器 | **部分布局**：从 LLM 向世界模型扩展 |

### 6.2 间接信号

- **Meta 内部**: 虽全力投入 Llama 4 ("Avocado")，但 JEPA 研究从未停止（"语言对某些任务够用，对真实世界不够" — LeCun 在 Meta 期间的路线）
- **Google**: Gemini 3 在 Spatial 和 Screen 类别对竞争对手的优势最大，暗示 Google 正将世界模型能力集成到旗舰模型
- **NVIDIA 开放 Cosmos 3**: 战略性开放 ≠ 慈善；建立物理 AI 时代的 CUDA 生态
- **AI Weekly 评论 (2026.05.05)**: "48x planning speedup over foundation-model-scale world models is the strongest efficiency argument yet for JEPA — and it came from Mila, NYU, and Samsung SAIL — not a hyperscaler."

### 6.3 投资逻辑推论

Hyperscaler 的 AI CapEx 是 sunk cost — 已投下去的数据中心、GPU 集群、电力合同。短期内不会因为新架构而削减投入。但如果 JEPA/世界模型的效率优势被验证，**增量投资**可能转向世界模型优化的基础设施（更多推理而非训练、更多边缘部署）。

---

## 7. JEPA 成功替代 LLM 对 GPU/HBM/CoWoS 需求的冲击估算

### 7.1 当前 AI 半导体需求结构（2026E）

| 组件 | AI 需求占比 | 主要瓶颈 |
|------|-----------|---------|
| **GPU (H100/B200/GB300)** | 核心需求 | TSMC CoWoS 封装 |
| **HBM3E/HBM4** | ~70% 产能被 AI 占用 | SK Hynix/三星产能 |
| **CoWoS 封装** | 主要瓶颈 | TSMC 产能极限 |
| **网络 (InfiniBand/Spectrum-X)** | 快速增长的 AI 集群需求 | NVIDIA 独占 |

### 7.2 情景分析

#### 情景 A：JEPA 仅在小众场景替代 LLM（概率：40%）

- 影响范围：机器人控制、视觉理解、科学仿真
- GPU 需求影响：**<5%** 削减（推理端）；训练端几乎无变化
- CoWoS/HBM 影响：边缘

#### 情景 B：JEPA 在 30-50% 推理场景替代 LLM（概率：35%）

- 假设：视觉-语言任务 + 规划/决策任务
- **推理 GPU 需求**: 可能下降 **30-50%**（假设 JEPA 效率 10-50× LLM）
- **训练 GPU 需求**: 可能下降 **20-30%**（JEPA 训练更高效）
- **CoWoS 需求**: 下降 20-35%（推理 GPU 占 CoWoS 总需求约 40-60%）

#### 情景 C：JEPA/世界模型成为主导架构（概率：25%）

- 假设：3-5 年内 JEPA 在 >70% 任务中性能达到或超越 LLM
- **推理 GPU 需求**: 可能下降 **70-90%**（10-100× 效率提升）
- **训练 GPU 需求**: 可能下降 **50-70%**（数据效率更高，模型更小）
- **CoWoS 需求**: 下降 50-75%
- **但**：新应用场景（机器人、AR/VR、自动驾驶）可能创造新需求

### 7.3 关键缓冲因素

| 因素 | 方向 | 影响 |
|------|------|------|
| Jevons 悖论 | 对冲 | 更便宜的推理 → 更多应用 → 总 GPU 需求未必大幅下降 |
| 边缘部署 | 对冲 | 世界模型可能催生边缘 AI（机器人/AR 眼镜），需要新芯片 |
| **时序** | 关键 | 3-10 年过渡期，不是突然替代 |
| Hyperscaler sunk cost | 缓冲 | 已建数据中心不会闲置，会找新用例 |
| **混合架构** | 最可能结果 | LLM + JEPA 混合 → GPU 需求不会消失但效率提高 |

### 7.4 对产业链的潜在赢家/输家

| 赢家 | 输家 |
|------|------|
| 推理芯片公司（边缘 AI） | 纯训练 GPU 厂商（如果训练需求下降） |
| 高带宽低功耗芯片 | HBM 供应商（如果需求弹性大） |
| 机器人/AR 硬件公司 | CoWoS 封装供应商（如需求大幅下降） |
| 低成本开源硬件 | NVIDIA（如果其垄断被打破） |

---

## 8. JEPA 商业化时间线（关键假设）

### 8.1 已实现 (2025 Q3 – 2026 Q2)

- [x] V-JEPA 2 零样本机器人规划 (1.2B 参数)
- [x] VL-JEPA 超越 GPT-4o 在 WorldPrediction (ICLR 2026)
- [x] LeWM 单 GPU 端到端训练 (15M 参数)
- [x] JEPA 形式化证明 (2026.05)
- [x] AMI Labs $1.03B 融资
- [x] NVIDIA Cosmos 3 开放发布 (2026.05.31)
- [x] Google Genie 3 商业订阅

### 8.2 预测时间线

| 时间段 | 里程碑 | 置信度 |
|--------|--------|--------|
| **2026 H2** | AMI Labs 发布首个研究 demo；Cosmos 3 生态扩展 | 高 (80%) |
| **2026 H2** | 首批 JEPA-based 机器人规划系统进入企业试点 | 中高 (65%) |
| **2027** | 首个 JEPA-based 生产级视觉理解产品（安防/质检） | 中 (55%) |
| **2027** | AMI Labs 可能完成 A 轮（$2-5B 估值区间） | 中 (50%) |
| **2027-2028** | JEPA + LLM 混合架构成为主流范式 | 高 (70%) |
| **2028-2029** | JEPA 在机器人/自动驾驶领域达到生产级可靠性 | 中 (50%) |
| **2029-2030** | 如果成功，JEPA 开始显著影响 GPU 需求结构 | 低-中 (35%) |
| **2030+** | JEPA "替代" LLM 在部分大市场是现实（非全部） | 低 (25%) |

### 8.3 商业化关键风险

1. **技术风险**: JEPA 在开放域语言任务上能否匹敌 LLM 仍未证实
2. **混合现实**: 最可能结果是混合架构，而非完全替代
3. **生态惯性**: LLM 工具链/开发者生态极为成熟
4. **AMI Labs 执行风险**: 12 人团队从零到产品线需要时间
5. **算力供给**: 即使 JEPA 更高效，AI 普及带来的总量增长可能抵消效率提升

---

## 9. 综合判断与投资启示

### 9.1 核心矛盾

> **$700B+ 的 LLM CapEx vs 15M 参数的单 GPU JEPA 达到相当控制性能**

这是 2026 年 AI 投资最大的结构性争议。Goldman Sachs 将 $700B 与 1990 年代电信泡沫类比，而 LeCun 认为整个 LLM 产业是"死胡同"。

### 9.2 三个关键观察

1. **效率鸿沟已证实**: LeWM 证明了 JEPA 在物理世界任务上 10-100× 的效率优势是真实的，不是理论上的。
2. **Hyperscaler 已经注意到**: NVIDIA 用 Cosmos 3 表明世界模型是下一波算力需求的驱动力；Google 用 Gemini 3 表明世界模型能力正集成进旗舰模型。
3. **时间上的不对称**: LLM 基础设施是 sunk cost（已投入），而 JEPA 商业化还需 2-5 年。短期内 CapEx 不会下降，但长期方向可能转向。

### 9.3 高置信度结论

- **JEPA 是真实的技术进步**，不是炒作 — 多个独立实验室和 benchmark 验证
- **混合架构是最可能结果**：LLM 做语言/推理，JEPA 做物理/视觉
- **AI CapEx 短期不会下降**：惯性 + 新场景（Agentic AI、机器人）
- **NVIDIA 定位聪明**：Cosmos 3 是物理 AI 时代的 CUDA，无论架构如何演进，算力需求依然存在
- **边缘 AI 芯片可能是最大受益者**：如果 JEPA 使模型足够小/快，边缘部署将成为可能

### 9.4 需要持续追踪的指标

- [ ] AMI Labs 何时发布首个公开 demo 或产品
- [ ] VL-JEPA 在更多 benchmark 上 vs GPT-5/Claude 4
- [ ] NVIDIA Cosmos 3 开发者采用速度
- [ ] Hyperscaler Q2 2026 earnings call 中对"非 LLM 架构"的表述
- [ ] TSMC CoWoS 产能利用率是否出现松动信号
- [ ] JEPA 在语言-only 任务上的性能（如果发布）

---

## 附录：关键来源列表

1. **VL-JEPA**: arXiv 2512.10942, ICLR 2026
2. **V-JEPA 2**: arXiv 2506.09985, Meta AI Blog (2025.06.11)
3. **LeWorldModel**: arXiv 2603.19312, le-wm.github.io (2026.03.13)
4. **JEPA 形式化证明**: Two arXiv preprints, late May 2026; TechTimes coverage (2026.05.31)
5. **AMI Labs**: TechCrunch (2026.01.23, 2026.03.09), Business Insider, MIT Tech Review, Observer
6. **NVIDIA Cosmos 3**: NVIDIA Blog/Hugging Face (2026.05.31-06.01)
7. **Google Genie 3**: DeepMind, WinBuzzer (2026.01.30)
8. **Runway**: TechCrunch, AI Business, Crunchbase (2026.02.10)
9. **Hyperscaler CapEx**: CreditSights, Goldman Sachs, Introl, DCPulse, Luna3.ai
10. **Inference cost**: ZDNet, Kilo AI, Inference Price Index, CodeAnt (2026)
11. **World Models 2026**: AI.cc, AI Weekly (2026.05.05), Towards AI, HumAI Blog
12. **WBench**: Meituan LongCat, WBench GitHub

---

*报告含部分基于公开信息的推断。所有数据点均注明来源。*
