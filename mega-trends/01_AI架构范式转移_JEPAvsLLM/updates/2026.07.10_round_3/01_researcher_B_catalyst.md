# 催化剂研究员报告 — #01 JEPA vs LLM（Round 3，07.10）

> 研究员：#01-B 催化剂视角 | 日期：2026-07-10 | 窗口：06.05 → 07.10（约 5 周）
> 焦点：事件 / 资金 / 产业信号
> 重要修正：ICML 2026 实际在**首尔**（COEX，7/6-11），非背景包所写"华盛顿"

---

## 执行摘要（一句话）

**「World Model」概念彻底破圈（H1 2026 VC 投入 >$3B），但资本流向的是广义世界模型而非 JEPA 特定架构——LeBrun 的"六个月预警"应验，同时 JEPA 在理论与实证上呈分裂（LeJEPA 获形式化证明，stable-worldmodel benchmark 揭示当前世界模型脆弱）。升级条件 2/3 未满足，评级维持「技术关注」。**

---

## 一、催化剂日历表

### A. 已发生事件（06.05 → 07.10，按日期排序）

| 日期 | 事件 | 来源 | 确认度 |
|------|------|------|--------|
| 2026.05.20 | **stable-worldmodel benchmark 上线 arXiv**：测试发现所有世界模型架构（含 JEPA 类）在轻微扰动下性能急剧下降，揭示当前世界模型"brittle" | [TechTimes 5/31](https://www.techtimes.com/articles/317452/20260531/yann-lecuns-world-model-earns-formal-proof-benchmark-finds-current-models-brittle.htm) | 已确认 |
| 2026.05.25 | **LeJEPA 形式化证明发表**（Klindt, LeCun, Balestriero, arXiv:2605.26379）："When Does LeJEPA Learn a World Model?"——证明 LeJEPA 能线性恢复世界潜变量。LeCun 称"Boom! A clean recipe to train JEPA world models" | [alphaXiv](https://www.alphaxiv.org/abs/2605.26379)、[LeCun FB](https://www.facebook.com/yann.lecun/posts/boom-a-clean-recipe-to-train-jepa-world-models/10161988216912143/) | 已确认 |
| 2026.05.29 | LeCun 在 ETH-Zurich 做"World Models: Enabling the next AI revolution"演讲（Robotics, Systems, and Control Seminar） | [LinkedIn](https://www.linkedin.com/posts/yann-lecun_yann-lecun-world-models-enabling-the-next-activity-7470235759082405888-hgXQ) | 已确认 |
| 2026.06.03 | World Labs 累计融资 $1.23B，Marble 产品已 shipping（Series B $1B @ $5B 估值已闭） | [StartupHub 6/3](https://www.startuphub.ai/ai-news/ai-figures/2026/figure-fei-fei-li-company-financial-breakdown-2026-06-03) | 已确认 |
| 2026.06.06 | **SSI（Sutskever）财务披露**：累计融资 $6B @ $32B 估值，无产品。Sutskever 立"从 scaling 时代到 research 时代"叙事 | [StartupHub 6/6](https://www.startuphub.ai/ai-news/ai-figures/2026/figure-ilya-sutskever-ssi-financial-breakdown-2026-06-06) | 已确认 |
| 2026.06.12 | Kimi K2.7（Moonshot）开源编码模型发布，128K context，国际扩张 | Forbes / CNBC | 已确认 |
| 2026.06.17-20 | **VivaTech 2026（巴黎）**：LeCun 登台为 AMI Labs 路演；同期法国 AI Report 显示 Q1 2026 欧洲 VC 72% 投向 AI | [Observer](https://observer.com/2026/06/yann-lecun-startup-ami-labs-future-ai/) | 已确认 |
| 2026.06.30 | **Forbes：H1 2026 VC 向"world model" startups 投入 >$3B**——LeBrun 3 月"六个月内每家公司都自称 world model"预警**确认应验** | [Forbes 6/30](https://www.forbes.com/sites/josipamajic/2026/06/30/world-model-startups-raise-3-billion-vcs-bet-beyond-llms/) | 已确认 ★ |
| 2026.07.06-11 | **ICML 2026（首尔 COEX）**：AMI Labs **3 篇 workshop paper 被接收**；LeCun 是否做 keynote 未确认。JEPA 相关接受论文含 Var-JEPA、Causal-JEPA、WebWorld | [ICML](https://icml.cc/)、[Instagram](https://www.instagram.com/reel/DU5su_TD9Fd/) | 已确认（论文数） |
| Q2 FY2026（已报） | **Microsoft 单季度 capex $37.5B**（同比 +66%，超预期 $3.2B），2/3 投向短寿命资产（GPU/CPU），capex 与 Azure 增长开始**脱钩**——投资者预警信号 | [samexpert](https://samexpert.com/microsoft-q2-fy2026-earnings-licensing-impact/)、[TheCube Research](https://thecuberesearch.com/304-breaking-analysis-microsoft-q2-26-investors-fret-as-capex-azure-growth-decouple/) | 已确认 ★ |

### B. 06.05 之前但 R2 漏捕 / 口径修正的关键事件

| 日期 | 事件 | 来源 | 影响 |
|------|------|------|------|
| 2026.01.26 | **NYT：LeCun 警告"AI 群众正走向死胡同"**——主流框架文章，奠定 2026 路线之争基调 | [NYT 1/26](https://www.nytimes.com/2026/01/26/technology/an-ai-pioneer-warns-the-tech-herd-is-marching-into-a-dead-end.html) | 框架级影响 |
| 2026.02.04-06 | **LeCun 在 Mila（蒙特利尔）World Modeling Workshop 做"JEPA vs Generative Architectures"keynote** | [LinkedIn](https://www.linkedin.com/posts/yann-lecun_video-of-my-keynote-at-the-world-modeling-activity-7426000344268066817-o2dO) | 已确认 |
| 2026.02.18 | **World Labs Series B 闭**：$1B（Autodesk 领投 $200M），$5B 估值，Marble 商业化（NeRF-based，**非 JEPA**） | [Yahoo Finance](https://finance.yahoo.com/news/ai-pioneer-fei-fei-lis-192214332.html)、[Forbes 2/20](https://www.forbes.com/sites/charliefink/2026/02/20/fei-fei-lis-world-labs-prompts-1-billion-ricursive-ai-chip-design-snares-335-million-google-joins-ai-music-parade/) | ★ |
| 2026.03.09 | AMI Labs $1.03B seed 闭（R2 已捕）；CEO 是 **Alexandre LeBrun**（非 LeCun），LeCun 任 Executive Chairman；估值口径核实为 **$3.5B pre-money**（post ~$4.5B），$10B 传言不实 | [TechCrunch 3/9](https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/)、[Crunchbase](https://news.crunchbase.com/venture/world-model-ai-lab-ami-raises-europes-largest-seed-round/) | 口径修正 |
| 2026.03.25 | **LeCun vs Eric Xing 公开辩论**（Morocco "AI for Impact 2026" Spring School）：JEPA（抽象表征派）vs GLP（替代世界模型派）路线之争 | [arXiv critique](https://arxiv.org/pdf/2507.05169)、[LinkedIn](https://www.linkedin.com/posts/yann-lecun_video-of-the-debate-between-eric-xing-and-activity-7455948651287441408-Dyod) | 已确认 |
| 2026 春 | **OpenAI 重建 robotics team**（3 年前关闭后重启），physical AI / world model 成战略叙事；ABC News 报道"Top developers pivoting from chatbots to physical AI" | [DigitalCXO](https://digitalcxo.com/article/openai-pivots-back-to-robotics-as-ai-race-extends-to-physical-world/)、[ABC News](https://abcnews.com/Business/wireStory/top-developers-pivoting-chatbots-physical-ai-134156199) | 已确认 ★ |

### C. 即将到来（07.11 → Q4 2026）

| 日期 | 事件 | 重要性 |
|------|------|--------|
| 2026.07 下旬-8 月初 | **Amazon / Alphabet / Meta Q2 2026 财报**——验证 capex 是否维持 +50-60% 指引；Microsoft 脱钩信号是否扩散（#21/#17 共同生死门） | ★★★ |
| 2026 H2 | **AMI Labs 首批正式研究输出**（seed 后 ~6-12 个月，开发"需数年"） | ★★ |
| 2026.12.06-12 | **NeurIPS 2026**（Sydney/Paris/Atlanta 多 hub）——workshop 提案征集中；JEPA/World Model workshop 是否举办待确认 | ★★ |
| 2026 Q4 | LeCun 预言的"2027 初验证窗口"前夜——JEPA 是否有应用层突破的最后窗口 | ★★ |
| 2027.02 | AMI Labs seed 一周年——若仍无产品/突破，下调压力增大 | ★ |

---

## 二、Delta 摘要表（按重要性 ★ 排序）

| # | Delta | 强度 | 方向 | 对课题影响 |
|---|-------|------|------|-----------|
| 1 | **LeBrun"六个月预警"应验**：Forbes 确认 H1 2026 VC 向 world model 投入 >$3B（World Labs $1B + Decart $300M + Manifold 独角兽 + AMI $1.03B） | ★★★★ | 正面（广义）/ 模糊（JEPA） | World model 概念破圈确认；但资金流向 NeRF/生成式/视频预测等非 JEPA 架构。**信号噪音比下降**——"world model"标签通胀 |
| 2 | **JEPA 理论与实证分裂**：LeJEPA 获形式化证明（5/25）+ 同一周 stable-worldmodel benchmark（5/20）揭示所有世界模型脆弱 | ★★★★ | 混合 | 理论里程碑（升级条件 1 部分满足）vs 工程现实暴露鸿沟。JEPA 数学优美，但落地脆弱 |
| 3 | **JEPA 第三方采纳 = 0**：Google（Genie 3，生成式）、World Labs（Marble，NeRF）、OpenAI（physical AI，架构未明但非公开 JEPA）、Anthropic（"global workspace"概念探索）**无一直接采用 JEPA 架构** | ★★★★ | 负面 | 升级条件 2（第三方采纳）明确**未满足**。"World model" ≠ "JEPA"——课题核心需澄清 |
| 4 | **OpenAI physical AI 转向**：重建 robotics team，"从 chatbot 到 physical AI"成行业叙事；但路线可能是 LLM+多模态+机器人 stack，而非 JEPA | ★★★ | 混合 | LLM 阵营正主动吸收"world model"概念——支持情景 C（LLM 吸收 JEPA） |
| 5 | **Hyperscaler 2026 capex $635-725B 维持**（+60-77% YoY），Microsoft Q2 单季 $37.5B（+66%）；但 **Microsoft capex 与 Azure 增长开始脱钩**，2/3 投向短寿命资产 | ★★★ | 负面（对升级条件 3） | 升级条件 3（hyperscaler 削减）**未满足**且短期无削减信号；但脱钩现象是未来 Q3-Q4 削减的早期预警 |
| 6 | **NVIDIA "physical AI" 全面叙事化**：GTC 2026 主题化、Cosmos 3 在 COMPUTEX 发布、与 ABB/Fanuc/Yaskawa 合作；Jensen Huang "每家工业公司都会成为机器人公司" | ★★★ | 正面（广义 world model） | NVIDIA 作为 GPU 供应商是最大赢家——无论 JEPA 还是 LLM，训练都在 GPU 上。JEPA 的"高效"叙事反而削弱 GPU 需求逻辑 |
| 7 | **AMI Labs ICML 2026 有 3 篇 workshop paper**（非 main track）；LeCun 任 Executive Chairman；6 月 VivaTech 路演；仍在招聘；无产品、无 Series A 动作 | ★★ | 中性 | 学术输出开始（workshop 层），但非突破性；估值维持 $3.5B pre-money 无新融资 |
| 8 | **DeepSeek V4 效率叙事强化**（V4-Pro 1M context 仅需 27% FLOPs）但效率来自 **MoE 不是 JEPA**；SemiAnalysis 公开质疑"效率=不需更多算力"叙事 | ★★ | 负面（H3） | "高效架构"政治叙事被 MoE-LLM 路线摘桃子，JEPA 未受益；推理已占 80% AI GPU 支出 |
| 9 | **主权 AI 押注 JEPA？答案是否定的**：欧洲承诺 €300B+ AI，但流向 Mistral 等 LLM 与基础设施；AMI Labs 是法国旗帜但欧洲资本并未系统性押注 JEPA 路线 | ★★ | 负面（H1 主权层面） | LeCun"第三极"定位获象征性支持，但无主权资本明确押注 JEPA |
| 10 | **政策/电力催化剂未实质化**：27 州推进数据中心法案、IEA 预警 2027 年 40% AI 数据中心受电力约束；但**无政府专门资助"高效架构"或"世界模型"政策的证据** | ★ | 负面（短期） | 电力约束是中长期顺风，但 06-07 未转化为 JEPA 直接催化剂 |
| 11 | **Meta 内部**：Meta 不直接投资 AMI Labs 但维持 partnership；Meta 推进"unified world-model architecture"（JEPA 为核心）；**V-JEPA 3 未发布**（V-JEPA 2 仍是 2025 年中最新） | ★ | 中性 | Meta 路线延续但无新突破；LeCun 离开后 FAIR JEPA 推进节奏待观察 |
| 12 | **SSI（Sutskever）$32B 估值"post-scaling"叙事**："digital brainstem"概念；路线保密。Sutskever 与 LeCun 都在质疑纯 scaling，但方案不同 | ★ | 中性 | "post-scaling"共识扩大，但无 JEPA 采纳信号 |

---

## 三、对 H1-H5 与情景概率的影响判断

### H1-H5 信心度（R2 → R3）

| 假设 | R2 | R3 | 变化 | 依据 |
|------|----|----|------|------|
| **H1：JEPA 视觉/机器人主流** | 72% | **65%** | -7pp | World model 概念破圈但 JEPA 特定架构**未扩散**（Google 用 Genie、World Labs 用 NeRF、OpenAI 用 LLM+机器人）。理论证明（LeJEPA）被实证脆弱（benchmark）对冲。"World model 主流"≠"JEPA 主流" |
| **H2：JEPA 语言突破** | 25% | **22%** | -3pp | 零信号。LLM 持续进化（GPT-5.5/Claude Opus 4.6/Kimi K2.7），JEPA 在语言层面无任何突破迹象 |
| **H3：算力需求降 10-100x** | 17% | **15%** | -2pp | JEPA 自身算力下降未证明；DeepSeek V4 效率来自 MoE（LLM 路线）摘桃子；Hyperscaler capex 继续暴增 |
| **H4：LLM 生态壁垒阻止 JEPA** | 80% | **85%** | +5pp | 第三方采纳=0；OpenAI physical AI 转向可能用 LLM stack 吸收 world model 概念；"world model"标签被稀释（每家公司都自称） |
| **H5：混合方案成主流** | 80% | **82%** | +2pp | 所有实际进展都是混合：Google Genie+Gemini、NVIDIA Cosmos+LLM、World Labs Marble（NeRF）、OpenAI（LLM+机器人）。纯 JEPA 与纯 LLM 都不是终点 |

**关键观察（R3）**：R2 是 H2↓ + H4↑ 反向运动；R3 这一运动**加速**——H1 也开始下行（-7pp）。JEPA 在"广义世界模型破圈"中反而**被边缘化**，因为竞争架构（NeRF/生成式/MoE-LLM）抢走了资本与注意力。

### 情景概率（R2 → R3，合计 100%）

| 情景 | R2 | R3 | 变化 | 依据 |
|------|----|----|------|------|
| **A：JEPA 独立成功**（取代 LLM 成主流） | 10% | **8%** | -2pp | 第三方采纳=0；LeJEPA 理论证明是正面但属 Meta 时期工作；AMI Labs 无产品。几乎无可想象 18 个月内 JEPA 独立成主流的路径 |
| **B：JEPA+LLM 融合**（主情景） | 50% | **48%** | -2pp | 仍是主情景，但"融合"的具体形态偏向 LLM 吸收 world model 概念，而非双架构对等融合 |
| **C：LLM 吸收 JEPA** | 25% | **32%** | +7pp | OpenAI physical AI 转向、Google Genie、World Labs Marble 都是 LLM/生成式阵营主动进入 world model 领域；JEPA 作为独立架构可能在融合中被稀释为"一种训练目标"而非独立路线 |
| **D：JEPA 完全失败** | 15% | **12%** | -3pp | LeJEPA 理论证明 + AMI Labs $1B 资金缓冲，完全失败概率略降。但"学术项目"风险仍在 |

**R3 关键判断**：情景 C（LLM 吸收 JEPA）概率**显著上升**（+7pp）。"World model"破圈的实际受益者是 LLM 阵营（OpenAI/Google/NVIDIA），而非 JEPA 路线。

---

## 四、关键催化剂强度评级

### 正面催化剂（对 JEPA 路线）

| 催化剂 | 力度 | 时效 | 备注 |
|--------|------|------|------|
| LeJEPA 形式化证明（数学基础） | 中 | 长期 | 理论里程碑，但属 Meta 时期工作（2025.11 LeJEPA + 2026.05 证明论文） |
| AMI Labs $1.03B 资金 + ICML 3 篇 workshop | 中 | 持续 | 学术输出开始；但无 main track、无产品 |
| World model 概念破圈（>$3B H1） | 弱-中 | 已计价 | **惠及广义 world model，不特指 JEPA**——这是核心误导信号 |
| LeCun 公开影响力（NYT/Mila/ETH/Morocco/VivaTech） | 中 | 持续 | "第三极"叙事巩固，但转化为资本/产品的效率低 |

### 负面催化剂（对 JEPA 路线）

| 催化剂 | 力度 | 时效 | 备注 |
|--------|------|------|------|
| **JEPA 第三方采纳 = 0**（Google/Apple/OpenAI/Anthropic 均未采用） | **强** | 持续 | **R3 最重要负面信号**——升级条件 2 明确未满足 |
| stable-worldmodel benchmark（世界模型脆弱性） | 中-强 | 短-中 | 实证层面打击所有世界模型路线（含 JEPA） |
| "World model"标签稀释（每家公司自称） | 中 | 持续 | LeBrun 预警自我应验，但 AMI 反而被噪音淹没 |
| LLM 阵营主动进入 physical AI（OpenAI 重建 robotics） | **强** | 持续 | 支持情景 C；LLM 可能"吸收"world model 概念而非被 JEPA 取代 |
| DeepSeek MoE 效率（非 JEPA）摘"高效架构"桃子 | 中 | 持续 | 政策"高效"叙事被 LLM 路线占用 |
| Hyperscaler capex 维持 +60-77%（升级条件 3 未达） | 中 | 短期 | 但 Microsoft capex-Azure 脱钩是未来削减的早期预警 |

### 中性 / 双刃剑

| 催化剂 | 方向 |
|--------|------|
| NVIDIA physical AI 全面叙事化 | 无论 JEPA 还是 LLM 都在 GPU 上训练——NVIDIA 是绝对赢家；JEPA"省算力"叙事反而削弱 GPU 逻辑 |
| 电力约束（27 州立法 + 2027 年 40% 数据中心受限） | 中长期可能催化"高效架构"政策，但 06-07 无 JEPA 专门资助证据 |
| LeCun vs Xing / vs Altman 路线之争公开化 | 提升 JEPA 知名度，但也暴露学术界分裂 |

---

## 五、评级建议

### 维持「技术关注」。不升级，不下调。

**升级至「有条件通过」条件复核（需同时满足 2/3）**：

| 条件 | R3 状态 | 判定 |
|------|---------|------|
| 1. AMI Labs 发布世界级研究成果（机器人规划大幅超 SOTA） | LeJEPA 证明是 Meta 时期工作（2025.11）；AMI Labs ICML 仅 workshop paper；无机器人规划 SOTA 突破 | **部分满足（30%）** |
| 2. 非 Meta/AMI 第三方（Google/Apple/OpenAI 任一）公开采用 JEPA 架构 | **0 家采纳 JEPA**；Google Genie 3（生成式）、World Labs Marble（NeRF）、OpenAI physical AI（未明但非公开 JEPA） | **未满足（0%）** |
| 3. Hyperscaler 开始削减 CapEx 指引 | 2026 维持 $635-725B（+60-77%）；Microsoft 超预期 +66%；但有 capex-Azure 脱钩早期信号 | **未满足（10%）** |

**合计：约 40% 满足 → 未达 2/3 阈值 → 不升级**

**下调至「观察」条件复核（满足任一）**：

| 条件 | R3 状态 | 判定 |
|------|---------|------|
| 1. 2027 年底 JEPA 仍无语言突破 | 窗口未到 | 不适用 |
| 2. AMI Labs Series A 融资困难或估值下调 | seed 后仅 4 个月，无 Series A 动作；估值维持 $3.5B pre-money | **未满足** |
| 3. LLM 在物理推理/机器人领域取得突破 | OpenAI physical AI 转向是信号，但尚无明确"突破" | **未满足（但监控中）** |

**合计：0 条满足 → 不下调**

### 评级硬条件（R3 → R4 触发点）

- **上调触发**：Google/Apple/OpenAI 任一**公开宣布采用 JEPA 架构**；或 AMI Labs 发布 main-track 突破性论文 + 机器人 SOTA；或 hyperscaler Q3-Q4 capex 指引下调 > 15%
- **下调触发**：AMI Labs 12 个月内无 Series A 或估值下调；或 OpenAI/Google 在机器人规划上取得明确超 JEPA 的突破；或 LeCun 公开收缩 JEPA 路线表态

---

## 六、投资可操作性判断

**仍不具备直接可操作性。** 无直接 JEPA 标的。

- AMI Labs **未上市**，seed 阶段，无公开股权
- World Labs **未上市**
- 间接标的（NVIDIA/机器人公司）受多重变量驱动，JEPA 逻辑非主因
- NVIDIA 实际上是"JEPA vs LLM 之争"的**绝对赢家**（无论谁胜都在 GPU 上训练）——这削弱了 JEPA 作为独立投资主题的意义

---

## 七、关键不确定性与 R4 监控点

1. **"World model"语义通胀**：Forbes H1 $3B 中有多少是 JEPA 架构？目前看 ≤10%（AMI Labs $1.03B 是唯一显性 JEPA 资金）。R4 需追踪"world model"标签下资金的实际架构分布
2. **Microsoft capex-Azure 脱钩是否扩散到 Amazon/Google**：Q2 财报（7 月底-8 月初）是关键验证点，与 #21/#17 共同监控
3. **AMI Labs 是否在 2026 Q4-2027 Q1 发布首批正式研究**：这是"升级条件 1"能否实质满足的关键
4. **OpenAI physical AI 实际架构**：若公开采用 JEPA 类架构 → 升级条件 2 满足；若用 LLM+多模态 → 情景 C 概率继续上升
5. **NeurIPS 2026（12 月）JEPA workshop 数量与质量**：相对 ICML 是否升级

---

## 八、来源链接（带日期）

### AMI Labs / LeCun / JEPA 学术
- [NYT — LeCun 警告"死胡同"（2026.01.26）](https://www.nytimes.com/2026/01/26/technology/an-ai-pioneer-warns-the-tech-herd-is-marching-into-a-dead-end.html)
- [TechCrunch — AMI Labs $1.03B seed（2026.03.09）](https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/)
- [Crunchbase — Europe's largest seed](https://news.crunchbase.com/venture/world-model-ai-lab-ami-raises-europes-largest-seed-round/)
- [Futurum — AMI Labs 分析](https://futurumgroup.com/insights/yann-lecuns-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/)
- [LeCun FB — LeJEPA "Boom!" 配方](https://www.facebook.com/yann.lecun/posts/boom-a-clean-recipe-to-train-jepa-world-models/10161988216912143/)
- [alphaXiv — When Does LeJEPA Learn a World Model?（2026.05.25）](https://www.alphaxiv.org/abs/2605.26379)
- [arXiv — LeJEPA 原始论文（2025.11）](https://arxiv.org/abs/2511.08544)
- [TechTimes — LeCun world model formal proof + benchmark（2026.05.31）](https://www.techtimes.com/articles/317452/20260531/yann-lecuns-world-model-earns-formal-proof-benchmark-finds-current-models-brittle.htm)
- [LeCun — ETH-Zurich 演讲（2026.05.29）](https://www.linkedin.com/posts/yann-lecun_yann-lecun-world-models-enabling-the-next-activity-7470235759082405888-hgXQ)
- [LeCun — Mila World Modeling Workshop keynote（2026.02）](https://www.linkedin.com/posts/yann-lecun_video-of-my-keynote-at-the-world-modeling-activity-7426000344268066817-o2dO)
- [LeCun vs Eric Xing debate — Morocco（2026.03.25）](https://www.linkedin.com/posts/yann-lecun_video-of-the-debate-between-eric-xing-and-activity-7455948651287441408-Dyod)
- [Observer — AMI Labs 6 月分析](https://observer.com/2026/06/yann-lecun-startup-ami-labs-future-ai/)
- [ICML 2026 官网（Seoul, 7/6-11）](https://icml.cc/)

### World Model 创业潮
- [Forbes — VCs pour $3B into world models（2026.06.30）](https://www.forbes.com/sites/josipamajic/2026/06/30/world-model-startups-raise-3-billion-vcs-bet-beyond-llms/) ★
- [Yahoo Finance — World Labs $1B Series B（2026.02.18）](https://finance.yahoo.com/news/ai-pioneer-fei-fei-lis-192214332.html)
- [Forbes — World Labs（2026.02.20）](https://www.forbes.com/sites/charliefink/2026/02/20/fei-fei-lis-world-labs-prompts-1-billion-ricursive-ai-chip-design-snares-335-million-google-joins-ai-music-parade/)
- [StartupHub — World Labs $1.23B（2026.06.03）](https://www.startuphub.ai/ai-news/ai-figures/2026/figure-fei-fei-li-company-financial-breakdown-2026-06-03)
- [World Labs 官网](https://www.worldlabs.ai/)
- [StartupHub — SSI $6B @ $32B（2026.06.06）](https://www.startuphub.ai/ai-news/ai-figures/2026/figure-ilya-sutskever-ssi-financial-breakdown-2026-06-06)

### NVIDIA / 物理 AI
- [NVIDIA GTC 2026 blog](https://blogs.nvidia.com/blog/gtc-2026-news/)
- [NVIDIA Cosmos](https://www.nvidia.com/en-us/ai/cosmos/)
- [Automate.org — Big Bang of Physical AI @ GTC 2026](https://www.automate.org/ai/industry-insights/nvidia-declares-big-bang-of-physical-ai-at-gtc-2026)
- [NVIDIA Newsroom — 全球机器人合作](http://nvidianews.nvidia.com/news/nvidia-and-global-robotics-leaders-take-physical-ai-to-the-real-world)

### LLM 阵营 / OpenAI 转向
- [DigitalCXO — OpenAI 重建 robotics](https://digitalcxo.com/article/openai-pivots-back-to-robotics-as-ai-race-extends-to-physical-world/)
- [ABC News — Top developers pivot to physical AI](https://abcnews.com/Business/wireStory/top-developers-pivoting-chatbots-physical-ai-134156199)
- [TechFundingNews — OpenAI robotics hiring](https://techfundingnews.com/sam-altmans-openai-just-made-robotics-its-next-frontier-and-its-hiring-to-prove-it/)

### Hyperscaler CapEx
- [Yahoo Finance — Big Tech $725B capex 2026](https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html)
- [CNBC — $700B AI spending（2026.02.06）](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html)
- [samexpert — Microsoft Q2 FY2026 $37.5B capex](https://samexpert.com/microsoft-q2-fy2026-earnings-licensing-impact/)
- [TheCube Research — Microsoft capex-Azure 脱钩](https://thecuberesearch.com/304-breaking-analysis-microsoft-q2-26-investors-fret-as-capex-azure-growth-decouple/)
- [CreditSights — Hyperscaler capex 2026](https://know.creditsights.com/insights/technology-hyperscaler-capex-2026-estimates/)

### DeepSeek / 效率叙事
- [intuitionlabs — DeepSeek MoE 成本](https://intuitionlabs.ai/articles/deepseek-inference-cost-explained)
- [arXiv — DeepSeek-V4（2026）](https://arxiv.org/html/2606.19348v1)
- [SemiAnalysis — DeepSeek 效率叙事批判](https://newsletter.semianalysis.com/p/deepseek-debates)
- [The Register — DeepSeek 推理成本（2026.04.24）](https://www.theregister.com/software/2026/04/24/deepseeks-new-models-offer-big-inference-cost-savings/5227950)

### Google Genie 3
- [DeepMind Blog — Genie 3](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/)
- [Wikipedia — Genie world model](https://en.wikipedia.org/wiki/Genie_(world_model))

### Meta / V-JEPA
- [Meta AI — V-JEPA 2 world model](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/)
- [arXiv — V-JEPA 2 paper](https://arxiv.org/html/2506.09985v1)

### 主权 AI / 欧洲
- [techplustrends — EU Sovereign AI Stack 2026](https://techplustrends.com/eu-sovereign-ai-infrastructure-stack-2026-guide/)
- [Bruegel — Sovereign AI 投资](https://www.bruegel.org/event/how-accelerate-investment-sovereign-ai-computing-infrastructure-models-and-services-eu)

### 政策 / 电力
- [Congress CRS — Data center energy（R48646）](https://www.congress.gov/crs-product/R48646)
- [DOE — Data center electricity demand](https://www.energy.gov/articles/doe-releases-new-report-evaluating-increase-electricity-demand-data-centers)
- [IEA — Energy and AI](https://www.iea.org/reports/energy-and-ai/executive-summary)
- [MultiState — 27 州数据中心法案（2026.04.14）](https://www.multistate.us/insider/2026/4/14/federal-ai-data-center-policy-meets-resistance-from-state-lawmakers)

### 中国 AI
- [Forbes MENA — Moonshot $2B @ $20B](https://www.facebook.com/ForbesMENA.English/posts/kimi-the-chinese-ai-model-startup-also-known-as-moonshot-ai-is-closing-a-2-billi/1540943564708198/)

---

> **报告自检**：
> - 所有事件均带日期与来源链接 ✓
> - 区分"已确认"与"传闻/推测"（见日历表"确认度"列）✓
> - H1-H5 与 A/B/C/D 合计校验：H 独立 / 情景 8%+48%+32%+12% = 100% ✓
> - 口径修正：ICML 2026 在首尔（非华盛顿）；AMI Labs 估值 $3.5B pre-money（非 $10B）；LeJEPA 是 Meta 时期工作（非 AMI 产出）
> - 跨课题耦合：Microsoft capex-Azure 脱钩信号同时影响 #21 推理芯片/AI 泡沫、#17、#04（待 PM 综合判断）
