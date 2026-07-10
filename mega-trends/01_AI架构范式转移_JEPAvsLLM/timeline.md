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
