# AI架构范式转移 — 事件时间线

## 2022
- **2022-06**: LeCun 发表纲领性论文 *"A Path Towards Autonomous Machine Intelligence"*，首次系统阐述 JEPA 架构构想 — [论文](https://openreview.net/forum?id=BZ5a1r-kVsf)

## 2023
- **2023-06**: Meta 发布 **I-JEPA**（Image JEPA），首个基于 JEPA 原理的图像模型，300M 参数，无需数据增强即达到强表现 — [Meta Blog](https://ai.meta.com/blog/yann-lecun-ai-model-i-jepa/)
- **2023**: LeCun 多次公开批评 LLM 路线，称"自回归生成是死胡同"

## 2024
- **2024-02**: Meta 发布 **V-JEPA**（Video JEPA），将 JEPA 扩展到视频理解领域 — [arXiv](https://arxiv.org/abs/2404.12345)
- **2024**: LeCun 在多个场合称"done with LLMs"，全力推进 JEPA 路线
- **2024-10**: LeCun 在 NVIDIA GTC 大会详细讲解 JEPA 技术原理

## 2025
- **2025-01**: LeCun 创立 AMI 公司，核心研究方向为基于 JEPA 的世界模型
- **2025-06**: Meta 发布 **V-JEPA 2**，编码器从 300M 扩展至 1B+（ViT-g），训练数据从 200 万扩展到 2200 万视频，实现零样本机器人规划 — [arXiv](https://arxiv.org/html/2506.09985v1)
- **2025-09**: **LLM-JEPA** 论文发布，将 JEPA 训练目标引入 LLM pipeline，v2 版本将计算开销从 200% 降至 25%，在多模型/多数据集上超越标准 LLM 训练目标 — [arXiv](https://arxiv.org/html/2509.14252v2)
- **2025-09**: LeCun 在 MIT 演讲，预测 JEPA 将在 3-5 年内取代 LLM
- **2025-12**: **VL-JEPA** 论文发布，首个基于 JEPA 的视觉-语言模型，解码速度 2.85x 更快，参数减少 50% — [arXiv](https://arxiv.org/abs/2512.10942)

## 2026
- **2026-01**: LeCun 在 MIT Technology Review 专访中公开阐述 AMI Labs 愿景 — "非美非中的第三极"，明确反对 LLM 路线 — [MIT TR](https://www.technologyreview.com/2026/01/22/1131661/yann-lecuns-new-venture-ami-labs/)
- **2026-03**: **AMI Labs 完成 $1.03B 种子轮融资**，$3.5B pre-money 估值（欧洲史上最大种子轮）。联合领投：Cathay Innovation/Greycroft/Hiro Capital/HV Capital/Bezos Expeditions。战略投资者：**NVIDIA**/Temasek/Samsung/Toyota Ventures — [Futurum](https://futurumgroup.com/insights/yann-lecuns-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/)
- **2026-03**: NVIDIA GTC 2026 将 **World Models** 列为核心主题之一。NVIDIA 机器人研究总监 Jim Fan："2026 年将标记 Large World Models 为机器人奠定真正基础的第一年"
- **2026-03**: Not Boring 发表万字深度文章 *World Models: Computing the Uncomputable*，系统性梳理 World Model 理论与产业进展 — [Not Boring](https://www.notboring.co/p/world-models)
- **2026-04**: LeCun 在 Welch Labs 播客详细阐述 JEPA 架构，对比传统生成式模型优劣
- **2026-05-21**: 本跟踪项目创建
- **2026-06-04**: Round 2 更新 — 辩论评级维持「技术关注」

## 2026 Q2-Q3（Round 3，07.10）— "思想胜利、架构失败"悖论 + 第三方采纳归零 + AMI Labs 静默

- **GPT-5.6 发布（7/8）**：距 GPT-5.5（4/23）仅 11 周。LLM 进入「5 周一迭代」节奏。SWE-bench Verified GPT-5.5 = 82.6%，距 R2 阈值 85% 仅 -2.4pp — [CNBC](https://www.cnbc.com/2026/07/08/)
- **CapEx 进入债务融资阶段（★★★★★，架构锁定加深）**：Amazon -FCF $17B（再借 $25B）、Oracle -FCF $24B（6/10 财报后跌 11%，拟融 $45-50B）、5 巨头合计 FCF 跌 >70%。Goldman 上调 2027 CapEx 至 $1.1T，全周期 $5.3T。**借债加注比现金支出更强的 Transformer 架构锁定信号** — 升级条件 #3 不仅未触发且**远离触发** — [Goldman Sachs Research](https://www.goldmansachs.com/insights/articles/tracking-trillions-the-assumptions-shaping-scale-of-the-ai-build-out)
- **JEPA 第三方采纳 = 0（头号利空）**：Google Genie 3（生成式）/ OpenAI Sora 2（diffusion，"world simulator"）/ NVIDIA Cosmos 3（omnimodal 生成式）/ World Labs Marble（NeRF）/ Figure Helix 02（VLM 混合）——**全部选择非 JEPA 路径**。升级条件 #2 明确未触发 — A+B+魔鬼三源一致
- **AMI Labs 4 个月零 main-track 产出**：seed 闭于 3/9（$3.5B **pre-money**），至 7/10 无 main-track 论文/产品/demo。ICML 2026（**首尔 COEX** 7/6-11，背景包误作华盛顿已纠正）仅 3 篇 workshop paper — [TechCrunch 3/9](https://techcrunch.com/2026/03/09/)
- **LeJEPA 归属 CIO WebSearch 查证**：arXiv 2605.26379「When Does LeJEPA Learn a World Model?」作者 LeCun 机构 = **Meta FAIR/NYU，非 AMI**。原始 LeJEPA（arXiv 2511.08544, 2025.11）为 LeCun 离开 Meta 前工作。**不计入"AMI 发布世界级研究"** — 升级条件 #1 未触发
- **DeepSeek V4 效率锁定（★★★★☆）**：V4 MoE（1.6T 参数）推理成本降 50x。Forbes 称「下一场竞赛是效率」。Transformer 自身变高效——JEPA「高效架构」独有叙事被摘桃子 — [Forbes 4/26](https://www.forbes.com/sites/geruiwang/2026/04/26/)
- **Hyperscaler 2026 CapEx 升至 $725B**（R2 时点 ~$700B）。JEPA 产业资金占比 0.15%→**0.14%** — [CNBC](https://www.cnbc.com/2026/02/06/)
- **World model 概念破圈但标签通胀（★★★★☆）**：H1 2026 VC 向 world model 投入 **>$3B**（World Labs $1B + AMI $1.03B + Decart $300M + Manifold）。但 AMI Labs CEO Alexandre LeBrun 3 月预警「六个月内每家公司都自称 world model」已应验。JEPA 在 $3B 中占比 ≤10% — [Forbes 6/30](https://www.forbes.com/sites/josipamajic/2026/06/30/)
- **机器人具身智能加速但去 JEPA 化**：1X World Model Lab（6/4）/ Figure Helix 02（8h 工厂班次）/ PI π0.7（4/16）/ Tesla Optimus Gen 3——全选生成式/视频预测/VLA 混合，未采用 JEPA
- **V-JEPA 2.1 + C-JEPA 发布**：V-JEPA 2.1（2026-03，Ego4D 7.71 mAP，+35%）。年度节奏持续（I-JEPA→V-JEPA→2→2.1），但参数量未推至 10B+；**V-JEPA 3 截至 07-10 未发布**（T2 触发监测）
- **OpenAI 重建 robotics team**："从 chatbot 到 physical AI"成行业叙事。路线可能是 LLM+多模态+机器人 stack 而非 JEPA——支持情景 C — [DigitalCXO](https://digitalcxo.com/)
- **stable-worldmodel benchmark 揭示脆弱**（5/20 arXiv）：所有世界模型架构（含 JEPA）在轻微扰动下性能急剧下降 — [TechTimes 5/31](https://www.techtimes.com/)
- **Goldman「AI: In a Bubble?」报告**：正式量化 AI 投资循环性风险（AI 公司投资 AI 公司）。但未提及架构路线风险——市场完全未定价架构更替
- **10Y UST 升至 4.56%（7/8）**：两周内 +18bp。JPM 预计全年不降息+2027 可能加息。高贴现率压制 AMI Labs 等长周期研究型公司 — [FRED DGS10](https://fred.stlouisfed.org/series/DGS10)
- **CIO Round 3 裁定（07.10）**：维持「技术关注」+ 新增 **12 个月日落条款**（AMI Labs 2027 Q1 无 main-track → 自动降级「观察」）。H1 72%→65%、H2 25%→20%、H4 80%→**86%**（本轮最强化）；情景 C 25%→**32%**，C+D=48%。魔鬼辩护人利空事实全部查证属实但降级时机过度（R2 降级条件 #1 距到期 18 个月 + 非可投资课题降级=自毁监测价值）。**不基于 JEPA 调整任何 GPU/HBM 仓位**。下次复查 8 月下旬（Hyperscaler Q2 财报是 #01/#17/#21 共同裁定时刻）

## 2026 Q3-Q4（Round 4，10.10）— 产出破冰但自证不达工业标准 + GPT-6 Astra 提前触发 + 日落条款写死

- **07.09**：GPT-5.6 正式发布（Sol 三档，Codex/API 全线）——R3 已载基线 — [OpenAI](https://openai.com/index/gpt-5-6)
- **08.29**：AMI Labs 首批团队署名论文之一 **LpWM**（稀疏表征 world model，arXiv，Kuang/Midlarsky 等）——产出破冰起点 — [AMI Observatory](https://ami.frenchtechjournal.com/)
- **09.03**：**OpenAI 发布 GPT-6 Astra**（API id `gpt-6-astra`）——1.05M token 上下文、五档推理、$10/$50 per M（较 5.6 Sol +2.5x）、OpenAI Preparedness 框架下首个 **Critical（网络安全）** 评级、computer-use 旗舰、Brockman「Welcome to the AGI era」。「GPT-5.7」为被吸收的候选名。**R2 阈值「GPT-6 若 Q4 发布=LLM 加速」提前一季触发**；LLM 迭代间隔缩至 ~8 周 — [pondero](https://pondero.ai/news/2026-09-04-openai-gpt6-astra-launch)/[codewalkers](https://codewalkers.com/news/ai-models/openai-gpt-6-astra)
- **09.03**：**NVIDIA 宣布 $12.9B 收购 Hugging Face**——开源模型分发核心节点被算力垄断者收编，H4 生态壁垒资本结构化 — [Fortune 9/4](https://fortune.com/2026/09/04/its-official-nvidia-acquire-hugging-face-12-9-billion)
- **09.10**：DeepSeek 发布 **V4.1-Flash**——全新因果 encoder-decoder 架构（Transformer 家族内变异）、552-763B MoE、原生多模态、1M 上下文、$0.30/1M——效率叙事继续被 Transformer 内部演化摘走 — [tpsreport](https://tpsreport.news/news/deepseek-v4-1-flash-encoder-decoder-architecture)
- **09.12**：**Amodei 发表「We Must Pace the Frontier」**——LLM 阵营首次自愿减速共识（Altman/Musk/Hassabis 呼应）；**但 9 月三家全部照常发货（Astra 9/3、Gemini 4 Argon 官宣、Opus 5.5 9/22）——姿态非行为** — [darioamodei.com](https://darioamodei.com/post/we-must-pace-the-frontier)/[TechCrunch](https://techcrunch.com/2026/09/12/anthropic-ceo-outlines-plan-to-pace-the-frontier/)
- **09.16-22**：Anthropic 6 天两发（Fable 5.1 9/16、**Opus 5.5** 9/22，$4/$20 per M）；SWE-bench Pro 榜 Opus 5.5 = 89.9% 重回榜首（10/9） — [Anthropic](https://www.anthropic.com/claude-opus-5-5)/[BenchLM](https://benchlm.ai/benchmarks/swe-bench-pro)
- **09.16**：**FOMC 加息 25bp 至 3.75-4.00%**（12-0，点阵图年底再+25bp 至 4.00-4.25%）——R3 利率逆风从预期变事实 — [Fed](https://www.federalreserve.gov/newsevents/pressreleases/monetary20260916a.htm)/[Reuters](https://www.reuters.com/business/warshs-words-may-matter-more-than-anticipated-fed-rate-hike-2026-09-16/)
- **09.20**：TechCrunch「World model companies are keeping a lot of secrets」——赛道保密化，LeBrun 标签通胀预言全兑现 — [TechCrunch](https://techcrunch.com/2026/09/20/world-model-companies-are-keeping-a-lot-of-secrets/)
- **09.22**：Vals AI：**SWE-bench Verified GPT-5.6 Sol = 96.20%**——R2 阈值 85% 被碾 11pp；同期测量层危机：SWEBench Pro GPT-5.5 失败的 68.5% 源于坏测试用例、OpenAI 已退役 SWE-bench Verified（#08 载录） — [Vals AI](https://www.vals.ai/benchmarks/swebench)
- **09.24-28**：AMI 论文流密集期——Kempe 世界建模物理工坊（Aspen）、**AD-E2E-JEPA（9/28）**：现有 JEPA 世界模型（LeWM/DINO-WM/JEPA-WM）在自动驾驶 goal-conditioned 规划**全部不达标**——JEPA 阵营首次公开负面自审，本轮最重要单一证据 — [AMI Observatory](https://ami.frenchtechjournal.com/)
- **09.29**：General Intuition 关闭 $220M——world model 赛道融资继续（Q1'24-Q2'26 累计 41 笔 >$9.5B），JEPA 显性资金仍≈AMI 一家 — [SiliconANGLE](https://siliconangle.com/2026/09/29/world-model-startup-general-intuition-closes-220m-investment/)
- **10.01**：Balestriero 公开指出竞品 LeWM 的 temporal collapse 缺陷并指向 AMI SIGReg 修复；Amir Bar 发布 **FAR 记忆框架**（借鉴 RAG）；LeCun Fortune 专访骂 Amodei「deluded/crazy」——阵营对抗白热化 — [AMI Observatory](https://ami.frenchtechjournal.com/)/[Fortune](https://fortune.com/2026/10/01/yann-lecun-anthropic-ceo-dario-amodei-deluded-crazy-cybersecurity/)
- **10.05**：**10Y UST 盘中 5.349%、收 5.307%**——2002 年以来最高；FOMC 后长端继续走高 — [CNBC](https://www.cnbc.com/2026/10/05/treasury-yields-bonds-fed-rates.html)
- **10 月**：arXiv 2610.07540（Toso/**LeCun 挂靠 NYU+AMI Labs**/Anderson/Bounou，逆动力学保不稳定模态）——LeCun 机构归属首次明确挂 AMI；AMI 招聘流入持续（Assran/Gu/Fung/Giraut-Pierron，四办公室扩张，T4 反向） — [arXiv](https://arxiv.org/pdf/2610.07540)
- **V-JEPA 3 全窗口未发布**：V-JEPA 2.1（3/16）后 GitHub 停更 7 个月，Meta 无 JEPA 旗舰接力——「母港撤资」强信号；T2 将于 12/31 自动执行 — [github.com/facebookresearch/vjepa2](http://www.github.com/facebookresearch/vjepa2)
- **CapEx 定格 $733-750B**：CreditSights ~$750B（+67%，第三年 >60% YoY）/TMT Finance $720-745B/#17 R4 现金口径 ~$733B+FCF 转负——升级条件 #3 远离触发，债务化锁定加深 — [CreditSights](https://know.creditsights.com/insights/tech-raising-hyperscaler-capex-2026-estimates/)
- **CIO Round 4 裁定（10.10）**：维持「技术关注」+ **日落条款结算机制写死**（T1 按 R3 原文 2027-03-31 自动裁定，arXiv 不算 main-track；新增 T5 工业级 ≥20% 优势门槛/T6 标签-架构脱钩检测）。H1 65→60%、H2 20→16%、H4 86→**88%**（减速共识记为首次软裂缝注记）；情景 C 32→**36%**（连续第三轮），C+D=49%。GPT-6 Astra 提前触发 R2 加速阈值。**不基于 JEPA 调整任何仓位**（第四轮）。下个观测点：10 月底 Q3 财报（2027 CapEx 指引）+12 月 NeurIPS 悉尼名单
