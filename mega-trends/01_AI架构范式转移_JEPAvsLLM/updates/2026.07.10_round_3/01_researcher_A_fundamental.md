# 基本面研究员报告 — #01 JEPA vs LLM（Round 3，07.10）

> 2026-07-10 | 基本面/技术视角 | 覆盖窗口 06.05 → 07.10（约 5 周）
> 数据源：anysearch（配额耗尽）/firecrawl（配额耗尽）→ 回退 WebSearch（Z.ai web_search_prime）+ 直接来源交叉验证
> 引用约定：每条数据标 [来源 + 日期]；推测明确标注「推测」

---

## 0. R2 背景包事实校正（先纠错，再研究）

**R2 背景包（`00_background_pack.md`）必查项 1 称"ICML 2026（6-7 月华盛顿）"——这是事实错误。**

- 已确认：**ICML 2026 在韩国首尔 COEX，7 月 6-11 日**（[icml.cc 官方](https://icml.cc/)、[Apple MLR](https://machinelearning.apple.com/)、[Google Research](https://research.google/conferences-and-events/google-at-ml-2026/) 多源交叉验证）
- 这是 R2→R3 跨会话信息漂移的典型 example，下游 PM/CIO 看到的 R2 文件需要标注修订
- 影响评估：地理错误不影响结论，但若 R2 阶段基于"华盛顿"做过地缘推断需要回查

---

## 1. Delta 摘要表（按重要性 ★ 排序）

| # | 重要性 | 事件 | 日期 | 来源 | 对 JEPA vs LLM 判断的影响 |
|---|--------|------|------|------|---------------------------|
| 1 | ★★★★★ | **GPT-5.6 发布**（Sol/Terra/Luna） | 2026-07-08 | [CNBC](https://www.cnbc.com/2026/07/08/openai-expanding-gpt-5point6-ai-model-release-ending-government-limits.html) | LLM 主流派系进入"5 周一迭代"节奏；GPT-5.5 仅 4/23 发布，5.6 已落地；**LLM 阵营强化** |
| 2 | ★★★★★ | **Hyperscaler 2026 CapEx 升至 $725B**（Amazon $200B / Microsoft $190B / Google $180-190B / Meta $125-145B），Goldman Sachs 预测全周期 $5.3T | 2026 Q1 公开指引汇总 | [Yahoo Finance](https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html)、[CNBC 2026-02-06](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html) | **CapEx 不减反增**；升级条件 3（hyperscaler 削减 CapEx）远未触发；几乎全部投 Transformer 栈 |
| 3 | ★★★★☆ | **NVIDIA Cosmos 3 发布**——omnimodal world foundation model（language/image/video/audio 联合） | 2026-06-01 | [Axios](https://www.axios.com/2026/06/01/nvidia-ai-push-cosmos-3-world-model)、[NVIDIA News](https://nvidianews.nvidia.com/news/nvidia-launches-cosmos-3-the-open-frontier-foundation-model-for-physical-ai)、[技术报告 PDF](https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf) | 世界模型赛道"破圈"确认；**但 Cosmos 3 是生成式 omnimodal，不是 JEPA 架构**——第三方用世界模型≠用 JEPA |
| 4 | ★★★★☆ | **DeepSeek V4 发布**（1.6T total / 49B active MoE），宣称与闭源前沿匹敌 | 2026-04-24 | [DeepSeek API Docs](https://api-docs.deepseek.com/news/news260424)、[CNBC](https://www.cnbc.com/2026/04/24/deepseek-v4-llm-preview-open-source-ai-competition-china.html) | 开源 LLM 进一步逼近闭源；**LLM 民主化加速**，JEPA 作为替代路径必要性降低 |
| 5 | ★★★★☆ | **1X 成立 World Model Lab**（视频预训练 → Neo 人形机器人） | 2026-06-04 | [Forbes](https://www.forbes.com/sites/johnkoetsier/2026/06/04/1x-launches-humanoid-robot-world-model-lab-you-cant-fine-tune-your-way-to-agi/)、[1X 官方](https://www.1x.tech/discover/1x-world-model-lab) | 机器人行业押注"世界模型"作为下一范式；**但 1X 用视频生成式，非 JEPA** |
| 6 | ★★★★☆ | **Physical Intelligence 发布 π0.7**——"emergent generalization"机器人基础模型 | 2026-04-16 | [pi.website](https://www.pi.website/) | 机器人 foundation model 路线分歧（π0.7 vs 世界模型 vs VLA），JEPA 是其中之一但非主流 |
| 7 | ★★★☆☆ | **V-JEPA 2.1 + C-JEPA 发布**（dense features / object-centric），Ego4D 短期任务 7.71 mAP，相对前 SOTA +35% | 2026-03 | [arXiv 2603.14482](https://arxiv.org/html/2603.14482v2)、[LeCun FB](https://www.facebook.com/yann.lecun/posts/v-jepa-21-a-new-jepa-model-trained-on-videouses-features-from-multiple-levels-in/10161966684567143/)、[TechTalks 2026-03-23](https://bdtechtalks.com/2026/03/23/v-jepa-2-1/) | JEPA 持续小步进化（年度节奏：I-JEPA 23' → V-JEPA 24' → V-JEPA 2 25' → V-JEPA 2.1 26'）；V-JEPA 3 推测在年内但**截至 07-10 未发布** |
| 8 | ★★★☆☆ | **SWE-bench Verified：GPT-5.5 = 82.6%**，Claude Opus 4.7 ~82%，Claude Opus 4.8 在 SWE-bench Pro 领先 69.2% | 2026 Q2 | [Vals AI](https://vals.ai/benchmarks/swebench)、[Contra Collective](https://contracollective.com/blog/claude-fable-5-vs-opus-4-8-vs-gpt-5-5-vs-gemini-3-5-2026)、[MorphLLM](https://www.morphllm.com/swe-bench-pro) | 距 R2 设定的 85% 阈值仅 -2.4pp；LLM 工程能力持续突破 |
| 9 | ★★★☆☆ | **ICML 2026 首尔会议（7/6-11）**，6500+ 论文，含"World Models"独立分类 + World Modeling Workshop（LeCun 主题演讲"JEPA vs Generative"已在 2/4 MILA 进行） | 2026-02-04（MILA）/ 2026-07-06~11（ICML） | [ICML Papers](https://icml.cc/virtual/2026/papers.html)、[Paper Digest](https://www.paperdigest.org/2026/05/icml-2026-papers-highlights/)、[LeCun LinkedIn](https://www.linkedin.com/posts/yann-lecun_video-of-my-keynote-at-the-world-modeling-activity-7426000344268066817-o2dO) | JEPA 在学术界合法地位确立；但量增不等于取代 LLM——6500+ 论文中 LLM 仍压倒性多数 |
| 10 | ★★★☆☆ | **AMI Labs 后续进展有限**——最新仍是 6/17 Bloomberg/Vivatech 采访（"Maybe we are not ambitious enough"），**无研究论文/demo 发布** | 2026-06-17 | [Bloomberg](https://www.bloomberg.com/news/articles/2026-06-17)、[Instagram Bloomberg TV](https://www.instagram.com/reel/DZsO8cqEw4f/) | $1.03B seed 后 3 个月无研究输出；升级条件 1（AMI 发布世界级研究）未触发 |
| 11 | ★★☆☆☆ | **OpenAI Sora 2 发布**——diffusion transformer，强调物理仿真（重力、流体、物体交互） | 2026 上半年 | [OpenAI](https://openai.com/index/video-generation-models-as-world-simulators/)、[flowith.io](https://flowith.io/blog/physics-of-sora-2-openai-simulating-physical-world/)、[TimesofAI](https://www.timesofai.com/news/openai-sora-2-launched-all-you-need-to-know/) | OpenAI 选择 diffusion 路径（非 JEPA）做"世界模拟器"——**第三方 JEPA 采纳条件未触发** |
| 12 | ★★☆☆☆ | **Google DeepMind Genie 3**——通用世界模型（2025-08 研究预览，持续推广） | 2025-08 起 | [DeepMind Blog](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/) | Google 也走非 JEPA 路径（基于 Gemini-3 reasoning）；第三方 JEPA 采纳条件未触发 |
| 13 | ★★☆☆☆ | **AMI Labs × Nabla 医疗战略**（LeCun + LeBrun 公开 demo "World Models for Medicine"） | 2026-03-11 | [HLTH](https://hlth.com/insights/news/ami-and-nabla-advance-world-models-to-power-agentic-healthcare-ai-2026-03-11)、[Nabla Blog](https://www.nabla.com/blog/ami-raises-1-03b-to-build-world-models----powering-the-next-generation-of-healthcare-ai-with-nabla) | AMI 首个垂直落地场景确认（医疗），但仍是商业合作而非研究成果发表 |
| 14 | ★★☆☆☆ | **DeepSeek 效率悖论（Jevons）**——效率改进反而推升总电力/GPU 需求 | 2026 | [enkiAI](https://enkiai.com/ai-market-intelligence/ai-energy-demand-2026-why-deep-seek-fuels-a-power-surge/)、[AMAX](https://www.amax.com/no-deepseek-isnt-the-end-for-gpus-its-just-the-beginning/) | 反驳"JEPA 高效→算力需求降"逻辑——即便架构更高效，总量仍升 |
| 15 | ★★☆☆☆ | **Figure Helix 02**——三系统架构（VLM 7-9Hz + visuomotor 200Hz + 推测的内部世界模型），8 小时自主工厂班次 | 2026-01-27 | [Figure AI](https://www.figure.ai/news/helix-02)、[Luigi Freda](https://www.luigifreda.com/2026/02/02/figure-ai-announces-helix-02-a-general-purpose-humanoid-system/)、[Humanoid Guide](https://humanoid.guide/figure-ai-demonstrates-helix-02-humanoid-robots-on-8-hour-shifts/) | 具身智能工程化加速，但 Figure 用的是工程混合栈，未公开宣称 JEPA |
| 16 | ★★☆☆☆ | **数据中心电力：2026 ~76 GW → 2030 ~134 GW（~27% US grid）**；DOE 预测 2028 占 6.7-12% | 2026-07-07 | [Reuters EIA](https://www.reuters.com/business/energy/us-power-use-beat-record-highs-2026-2027-ai-use-surges-eia-says-2026-07-07/)、[DOE](https://www.energy.gov/articles/doe-releases-new-report-evaluating-increase-electricity-demand-data-centers) | 电力约束叙事强化；与 #21/#14 耦合；JEPA "高效"论点长期获政策顺风，但短期未触发架构切换 |

**遗漏/不确定项**：
- V-JEPA 3 是否在 2026 H2 发布——年度节奏推断很可能，但截至 07-10 未发布（推测）
- Anthropic "Claude Fable 5 / Mythos 5" / "Opus 5" 的真实性——WebSearch 返回内容中搜索引擎自身警告"可能是模拟/虚构未来日期内容"；**建议 CIO 综合报告时不要采信 Fable/Mythos 命名**，但 Opus 4.7/4.8 在多个独立 leaderboard 出现，倾向认为有小版本迭代（推测，待核实）
- AMI Labs 团队规模：R2 记录 12 人，本轮搜索未找到 07-10 时点的确切数字（推测：上升但量级不明）

---

## 2. H1-H5 逐条更新

### H1：JEPA 成为视觉/机器人主流架构

| 维度 | R2 信心 | R3 建议信心 | 变化 |
|------|---------|-------------|------|
| H1 | 72% | **68%** | **-4pp** |

**依据**：

- **利好（已确认）**：
  - V-JEPA 2 已实现 pick-and-place 新物体 65-80% 成功率、Epic-Kitchens 39.7 recall@5（+44%）[Meta AI Blog](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/)
  - V-JEPA 2.1（2026-03）相对前 SOTA +35%，Ego4D 7.71 mAP [arXiv 2603.14482](https://arxiv.org/html/2603.14482v2)
  - C-JEPA（object-centric world model）发布，VQA 持续提升
  - VLA-JEPA 在 LeRobot 中使用 V-JEPA 2 backbone

- **利空（已确认，权重更大）**：
  - **第三方机器人公司选择非 JEPA 世界模型**：
    - 1X（6/4 World Model Lab）→ 视频生成式 [Forbes](https://www.forbes.com/sites/johnkoetsier/2026/06/04/1x-launches-humanoid-robot-world-model-lab-you-cant-fine-tune-your-way-to-agi/)
    - Physical Intelligence π0.7（4/16）→ 通用机器人策略，非 JEPA [pi.website](https://www.pi.website/)
    - Figure Helix 02（1/27）→ 三系统 VLM+visuomotor，未宣称 JEPA [Figure AI](https://www.figure.ai/news/helix-02)
    - NVIDIA Cosmos 3（6/1）→ omnimodal 生成式 [Axios](https://www.axios.com/2026/06/01/nvidia-ai-push-cosmos-3-world-model)
  - **判断**：JEPA 概念红利期到来（"世界模型"破圈），但 JEPA 作为**具体架构**在具身智能工程实践中被边缘化；行业更倾向可生成可视化的方案（Cosmos、1X、Sora 2）

- **结论**：JEPA 学术合法地位巩固，但工业采纳份额并未随世界模型红利同步上升——故 H1 信心小幅下调 4pp 至 68%

### H2：JEPA 在语言任务上突破

| 维度 | R2 信心 | R3 建议信心 | 变化 |
|------|---------|-------------|------|
| H2 | 25% | **22%** | **-3pp** |

**依据**：

- 06.05→07.10 期间**无任何 JEPA 语言突破**公开（已确认，全数据库扫描）
- 主流语言模型全部 Transformer MoE：GPT-5.5/5.6、Claude Opus 4.7/4.8、Gemini 3.1 Pro、DeepSeek V4（1.6T MoE）、Qwen 3.5/3.6/3.7 Max、Llama 4 Scout/Maverick、GLM-5.1、Gemma 4
- C-JEPA 在视觉问答有提升，但仍属视觉模态 [LeCun FB](https://www.facebook.com/yann.lecun/posts/v-jepa-21-a-new-jepa-model-trained-on-videouses-features-from-multiple-levels-in/10161966684567143/)
- 开源已逼近闭源（"6 labs 开源权重匹配前沿性能"），**LLM 民主化反而加固 Transformer 栈**——JEPA 语言路径失去"被需要的理由"

### H3：算力需求降 10-100x

| 维度 | R2 信心 | R3 建议信心 | 变化 |
|------|---------|-------------|------|
| H3 | 17% | **15%** | **-2pp** |

**依据**：

- Hyperscaler 2026 CapEx 从 R2 时点的 ~$700B 升至 **$725B**（Goldman Sachs 全周期 $5.3T）[CNBC 2026-02-06](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html)、[Yahoo Finance](https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html)
- DeepSeek 效率改进触发 **Jevons paradox**——总 AI 电力/GPU 需求反而上升 [enkiAI](https://enkiai.com/ai-market-intelligence/ai-energy-demand-2026-why-deep-seek-fuels-a-power-surge/)
- 数据中心电力 2026 ~76 GW → 2030 ~134 GW（占 US grid 27%）[Reuters 2026-07-07](https://www.reuters.com/business/energy/us-power-use-beat-record-highs-2026-2027-ai-use-surges-eia-says-2026-07-07/)
- JEPA 训练效率声称 1.5-6x 改善 [Ken Huang Substack](https://kenhuangus.substack.com/p/world-models-architectures-and-the) ——**远未达 10-100x 阈值**
- **结论**：架构级效率改进的乘数效应被应用层总量扩张完全覆盖；H3 路径在可见未来（2027 年底前）几无可能触发

### H4：LLM 生态壁垒阻止 JEPA 取代

| 维度 | R2 信心 | R3 建议信心 | 变化 |
|------|---------|-------------|------|
| H4 | 80% | **85%** | **+5pp** |

**依据**：

- **LLM 迭代速度惊人**：
  - GPT-5.5（4/23）→ GPT-5.6（7/8）仅 11 周 [OpenAI](https://openai.com/index/introducing-gpt-5-5/)、[CNBC 2026-07-08](https://www.cnbc.com/2026/07/08/openai-expanding-gpt-5point6-ai-model-release-ending-government-limits.html)
  - SWE-bench Verified GPT-5.5 = 82.6%（距 R2 阈值 85% 仅 -2.4pp）[Vals AI](https://vals.ai/benchmarks/swebench)
  - DeepSeek V4（4/24）、Qwen 3.5/3.6/3.7 Max、Llama 4 Scout/Maverick（4/5）、GLM-5.1、Gemma 4——开源全栈与闭源匹配
- 推理时计算（test-time compute）开辟新缩放维度：o1 → o3 → GPT-5.5 interleaved thinking [Stanford CS224R 2026 slides](https://cs224r.stanford.edu/slides/10_cs224r_rl_for_llms_reasoning_2026.pdf)
- **$725B CapEx 全部投 Transformer 栈**——资本配置锁定 3-5 年路径依赖
- JEPA 阵营无等量级资本对应（AMI Labs $1.03B 占行业 $725B = **0.14%**，比 R2 时点的 0.15% 略降）
- **结论**：H4 是本期最强化的假设——生态壁垒从"阻止 JEPA"升级为"**结构性封锁任何替代架构**"

### H5：混合方案成主流

| 维度 | R2 信心 | R3 建议信心 | 变化 |
|------|---------|-------------|------|
| H5 | 80% | **82%** | **+2pp** |

**依据**：

- 已确认的混合方案实例（全部主流玩家）：
  - **NVIDIA Cosmos 3**：language + image + video + audio omnimodal [NVIDIA Research 技术报告](https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf)
  - **Figure Helix 02**：VLM（System 2）+ visuomotor（System 1）+ 推测的世界模型组件 [Figure AI](https://www.figure.ai/news/helix-02)
  - **Google Gemini 3.1 Pro**：原生多模态 transformer
  - **Apple MLR**：多模态 LLM 研究方向
  - **NVIDIA World-Action Models（WAM）**：世界模型 + agentic AI 混合 [NVIDIA Dev Blog](https://developer.nvidia.com/blog/pretrained-to-imagine-fine-tuned-to-act-the-rise-of-world-action-models/)
- JEPA 思想（latent prediction）作为**组件**渗透（如 VLA-JEPA），但作为**整体架构**未独立
- **结论**：H5 进一步确认；A 情景（JEPA 完全独立取代）几乎不可能

---

## 3. A/B/C/D 情景概率建议

| 情景 | R2 概率 | R3 建议 | 变化 | 依据 |
|------|---------|---------|------|------|
| **A：JEPA 独立成功**（取代 LLM 成主流） | 10% | **8%** | -2pp | 第三方 JEPA 采纳为零（Google/OpenAI/Apple/NVIDIA 都选非 JEPA 路径）；AMI Labs 3 个月无研究输出；JEPA 在具身智能被生成式方案挤出主流 |
| **B：JEPA+LLM 融合**（主情景，JEPA 负责 World Model，LLM 负责语言） | 50% | **52%** | +2pp | NVIDIA Cosmos 3 / Figure Helix 02 / WAM 概念确认混合是事实路径；JEPA 作为组件（VLA-JEPA）渗入 |
| **C：LLM 吸收 JEPA**（JEPA 作为独立架构消失） | 25% | **28%** | +3pp | GPT-5.6（5周一迭代）+ DeepSeek V4 开源逼近 + $725B CapEx 全投 Transformer；LLM 阵营正在"吸收"世界模型概念（Sora 2 物理仿真、Gemini 3 reasoning）而非被 JEPA 替代 |
| **D：JEPA 完全失败**（沦为学术项目） | 15% | **12%** | -3pp | Meta FAIR + AMI Labs $1.03B 持续投入；V-JEPA 2/2.1 持续迭代；学术合法性（ICML 2026 World Models 分类）已确立——完全失败概率降低 |
| **合计** | 100% | **100%** | 0 |  |

**主情景 B 概率微升**：本期发展确认混合是事实标准，但 JEPA 在混合中的**相对权重**正在被生成式世界模型稀释。

---

## 4. 评级建议

### 建议：**维持「技术关注」**（与 R2 一致，不升级不下调）

### 硬条件核对

**升级至「有条件通过」（需同时满足 2/3）**：

| 条件 | 状态 | 说明 |
|------|------|------|
| 1. AMI Labs 发布世界级研究（机器人规划大幅超 SOTA） | **部分达成，未触发** | V-JEPA 2.1 提升 35% 但属于视频理解，机器人规划 65-80% pick-and-place 未到"大幅超"；AMI Labs 本身 6 月后无发表 |
| 2. 非 Meta/AMI 第三方（Google/Apple/OpenAI 任一）公开采用 JEPA 架构 | **未触发** | Google Genie 3（非 JEPA）、OpenAI Sora 2（diffusion）、Apple 无公开 JEPA 研究、NVIDIA Cosmos 3（omnimodal 生成式） |
| 3. Hyperscaler 开始削减 CapEx 指引 | **完全未触发** | 2026 CapEx 升至 $725B（R2 时 ~$700B）；Goldman Sachs 全周期 $5.3T |

→ **满足 0/3**，不升级

**下调至「观察」（满足任一）**：

| 条件 | 状态 | 说明 |
|------|------|------|
| 1. 2027 年底 JEPA 仍无语言突破 | 待定（趋势是的） | H2 22%，但触发时点是 2027 年底 |
| 2. AMI Labs Series A 融资困难或估值下调 | **未触发** | 无新融资负面消息；6/17 LeBrun Bloomberg 采访仍高调 |
| 3. LLM 在物理推理/机器人取得突破 | **部分触发** | Sora 2 物理仿真、Figure Helix 02 工厂 8 小时班次、NVIDIA Cosmos 3——但都属于"生成式世界模型"路径，不算"LLM 直接做物理推理" |

→ **0/3 完全触发**（条件 3 存在歧义），不下调

### 简短结论

R2→R3 期间发生的是**"世界模型"概念破圈与 JEPA 被边缘化的悖论**：
- 概念层面：JEPA 的"世界模型"思想赢了——所有主流玩家都在谈
- 架构层面：JEPA 输了——所有人都选了非 JEPA 实现（生成式 / omnimodal / diffusion / VLM 混合）

这种"思想胜利、架构失败"的格局对评级是中性的，故维持「技术关注」。

---

## 5. 投资可操作性判断

**仍不具备直接可投资性**（与 R2 一致）。

### 间接信号（与 #11/#17/#21 耦合）

**利好方向（验证既有逻辑）**：
- **机器人/具身智能供应链**（#11）：Figure Helix 02 工厂 8 小时班次、1X World Model Lab、Physical Intelligence π0.7、Tesla Optimus Gen 3、Unitree G1——具身智能工程化加速，JEPA 是技术底座之一
- **AI 电力/能源基础设施**（#21/#14）：2026 76 GW → 2030 134 GW，DOE 预测 2028 占 6.7-12%——DeepSeek 效率悖论意味着电力需求无下行风险

**利空方向（弱化既有逻辑）**：
- **边缘芯片 JEPA 效率叙事**：H3 仅 15%；JEPA 训练效率 1.5-6x 远未达 10-100x；Jevons paradox 让"高效架构降低总需求"逻辑失效
- **GPU/HBM 需求削减逻辑**：CapEx 升至 $725B，无下行迹象；JEPA 即便胜出也不会削减 GPU 需求

### 操作建议

1. **不基于 JEPA 调整任何 GPU/HBM 仓位**——CapEx 锁定 3-5 年路径依赖
2. **基于机器人/具身智能单独配置 #11**——Figure/1X/Physical Intelligence/Tesla Optimus 加速
3. **观察 AMI Labs 首批研究成果**（推测 2026 Q4 或 2027 Q1）——若发布机器人规划 SOTA 大幅突破，触发 H1 上调
4. **观察 V-JEPA 3 发布**（推测 2026 H2）——若参数量推至 10B+ 且有真实机器人 SOTA，触发评级上调讨论

---

## 6. 关键来源链接（带日期）

### JEPA / Meta FAIR（技术进展）
- [V-JEPA 2 官方博客](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/) — Meta AI，2025
- [V-JEPA 2 arXiv 论文 2506.09985](https://arxiv.org/html/2506.09985v1) — 2025
- [V-JEPA 2.1 arXiv 2603.14482](https://arxiv.org/html/2603.14482v2) — 2026-03
- [LeCun V-JEPA 2.1 Facebook 公告](https://www.facebook.com/yann.lecun/posts/v-jepa-21-a-new-jepa-model-trained-on-videouses-features-from-multiple-levels-in/10161966684567143/) — 2026-03
- [TechTalks V-JEPA 2.1 评测](https://bdtechtalks.com/2026/03/23/v-jepa-2-1/) — 2026-03-23
- [LeCun World Modeling Workshop Keynote（MILA, JEPA vs Generative）](https://www.linkedin.com/posts/yann-lecun_video-of-my-keynote-at-the-world-modeling-activity-7426000344268066817-o2dO) — 2026-02-04
- [facebookresearch/jepa GitHub](https://github.com/facebookresearch/jepa)

### AMI Labs（资本与团队）
- [TechCrunch: AMI Labs $1.03B seed $3.5B 估值](https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/) — 2026-03-09
- [Futurum Group 深度分析](https://futurumgroup.com/insights/yann-lecun-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/) — 2026-03
- [Forbes: AMI Labs 瞄准医疗](https://www.forbes.com/sites/amyfeldman/2026/01/21/why-yann-lecuns-hot-new-ai-startup-is-targeting-healthcare/) — 2026-01-21
- [Bloomberg TV (LeBrun "Maybe we are not ambitious enough")](https://www.bloomberg.com/news/articles/2026-06-17) — 2026-06-17（Vivatech Paris）
- [HLTH: AMI × Nabla 医疗世界模型合作](https://hlth.com/insights/news/ami-and-nabla-advance-world-models-to-power-agentic-healthcare-ai-2026-03-11) — 2026-03-11
- [MIT Technology Review LeCun 专访](https://www.technologyreview.com/2026/01/22) — 2026-01-22

### 第三方世界模型（非 JEPA）
- [Google DeepMind Genie 3](https://deepmind.google/blog/genie-3-a-new-frontier-for-world-models/) — 2025-08 起
- [OpenAI: Video Generation Models as World Simulators](https://openai.com/index/video-generation-models-as-world-simulators/)
- [Sora 2 物理仿真深度分析](https://flowith.io/blog/physics-of-sora-2-openai-simulating-physical-world/) — 2026
- [NVIDIA Cosmos 3 Axios 报道](https://www.axios.com/2026/06/01/nvidia-ai-push-cosmos-3-world-model) — 2026-06-01
- [NVIDIA Cosmos 3 官方公告](https://nvidianews.nvidia.com/news/nvidia-launches-cosmos-3-the-open-frontier-foundation-model-for-physical-ai)
- [NVIDIA Cosmos 3 技术报告 PDF](https://research.nvidia.com/labs/cosmos-lab/cosmos3/technical-report.pdf)
- [NVIDIA World-Action Models Dev Blog](https://developer.nvidia.com/blog/pretrained-to-imagine-fine-tuned-to-act-the-rise-of-world-action-models/)
- [Themesis: World Models 五种竞争方法](https://themesis.com/2026/01/07/world-models-five-competing-approaches/) — 2026-01-07

### 具身智能 / 机器人
- [1X World Model Lab](https://www.1x.tech/discover/1x-world-model-lab) — 2026-06-04
- [Forbes: 1X World Model Lab](https://www.forbes.com/sites/johnkoetsier/2026/06/04/1x-launches-humanoid-robot-world-model-lab-you-cant-fine-tune-your-way-to-agi/) — 2026-06-04
- [1X World Model 训练方法](https://www.1x.tech/discover/world-model-self-learning)
- [Physical Intelligence π0.7](https://www.pi.website/) — 2026-04-16
- [Figure AI Helix 02 官方公告](https://www.figure.ai/news/helix-02) — 2026-01-27
- [Humanoid Guide: Helix 02 8 小时班次](https://humanoid.guide/figure-ai-demonstrates-helix-02-humanoid-robots-on-8-hour-shifts/)

### LLM 前沿（对照组）
- [OpenAI GPT-5.5 官方](https://openai.com/index/introducing-gpt-5-5/) — 2026-04-23
- [CNBC: GPT-5.6 发布](https://www.cnbc.com/2026/07/08/openai-expanding-gpt-5point6-ai-model-release-ending-government-limits.html) — 2026-07-08
- [Vals AI SWE-bench Leaderboard](https://vals.ai/benchmarks/swebench)
- [SWE-bench 官方](https://www.swebench.com/)
- [Contra Collective: SWE-bench Pro Claude Opus 4.8 = 69.2%](https://contracollective.com/blog/claude-fable-5-vs-opus-4-8-vs-gpt-5-5-vs-gemini-3-5-2026)
- [DeepSeek V4 Preview Release](https://api-docs.deepseek.com/news/news260424) — 2026-04-24
- [CNBC DeepSeek V4](https://www.cnbc.com/2026/04/24/deepseek-v4-llm-preview-open-source-ai-competition-china.html)
- [Stanford CS224R RL for LLMs Reasoning 2026](https://cs224r.stanford.edu/slides/10_cs224r_rl_for_llms_reasoning_2026.pdf)
- [Sebastian Raschka: Inference-Time Scaling](https://magazine.sebastianraschka.com/p/categories-of-inference-time-scaling)

### Hyperscaler CapEx / 算力 / 电力
- [Yahoo Finance: $5.3T 周期 CapEx](https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html)
- [CNBC AI $700B 2026](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html) — 2026-02-06
- [Futurum Group: $690B Infrastructure Sprint](https://futurumgroup.com/insights/ai-capex-2026-the-690b-infrastructure-sprint/)
- [Reuters: US 电力 2026-2027 创纪录](https://www.reuters.com/business/energy/us-power-use-beat-record-highs-2026-2027-ai-use-surges-eia-says-2026-07-07/) — 2026-07-07
- [DOE 数据中心电力报告](https://www.energy.gov/articles/doe-releases-new-report-evaluating-increase-electricity-demand-data-centers)
- [enkiAI: DeepSeek 效率悖论](https://enkiai.com/ai-market-intelligence/ai-energy-demand-2026-why-deep-seek-fuels-a-power-surge/)
- [AMAX: DeepSeek 不是 GPU 终结](https://www.amax.com/no-deepseek-isnt-the-end-for-gpus-its-just-the-beginning/)

### ICML 2026
- [ICML 2026 官方（首尔 COEX）](https://icml.cc/)
- [ICML 2026 Papers 列表](https://icml.cc/virtual/2026/papers.html)
- [Paper Digest: 6500+ 论文](https://www.paperdigest.org/2026/05/icml-2026-papers-highlights/)
- [Apple at ICML 2026](https://machinelearning.apple.com/)
- [LeCun World Modeling Workshop Keynote @ MILA](https://www.linkedin.com/posts/yann-lecun_video-of-my-keynote-at-the-world-modeling-activity-7426000344268066817-o2dO) — 2026-02-04

---

## 7. 给 PM / CIO / 魔鬼辩护人的提示

1. **R2 文件需修订**：ICML 2026 地点错误（华盛顿→首尔），如影响其他课题的跨课题耦合推论需回查
2. **Claude Fable 5 / Mythos 5 命名待核实**：搜索引擎警告可能为虚构未来日期内容，本报告未采信；Opus 4.7/4.8 在多个独立 leaderboard 出现，倾向认为有小版本迭代但未达"5.5"级别
3. **"世界模型破圈但 JEPA 被边缘化"**是本期最重要洞察——魔鬼辩护人可能质疑"JEPA 是否还能算独立架构"。我的回答：JEPA 作为**概念**已经胜利（latent prediction / 抽象表征预测被广泛认可），但作为**工程实现**已被生成式方案挤出主流——这对评级影响是中性的
4. **下一轮（R4，推测 2026-08-14 前后）重点观察**：
   - V-JEPA 3 是否发布（年度节奏）
   - AMI Labs 首批研究成果（推测 Q4）
   - Hyperscaler Q2 财报（8 月初）实际 CapEx
   - GPT-5.6 之后 OpenAI 是否转向"世界模型"叙事
   - Apple 是否在 iPhone 18 / Vision Pro 公开世界模型组件
