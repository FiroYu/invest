# 魔鬼辩护人报告 — #01 JEPA vs LLM（Round 3，07.10）

> 立场：最强熊方。目的是迫使 CIO 正视下调至「观察」的论据，不是平衡叙述。

## 一句话论点

**过去 5 周（06.05→07.10）零证据支持上调 JEPA：AMI Labs 拿了 $1.03B 后 4 个月无任何研究产出、无产品、无第三方采纳；同时 LLM 阵营（Sora 2 / NVIDIA Cosmos / VLA 模型 / World Labs Marble）正以非-JEPA 路径独立吸收"世界模型"能力，JEPA 作为"独立架构"的存在意义正在被掏空——这不是"维持技术关注"的局面，这是滑向情景 D（学术项目）与情景 C（被吸收）的临界点。**

---

## 一、证伪矩阵 — H1-H5 逐条攻击

### H1：JEPA 视觉/机器人主流（R2 信心 72%）→ 应下调至 55-60%

| 攻击 | 证据 | 来源/日期 |
|------|------|-----------|
| NVIDIA 官方框架根本不含 JEPA | NVIDIA Developer Blog 把机器人基础模型归纳为"两大配方"：VLA 模型 + World-Action Models（WAMs）。JEPA 在 NVIDIA 的产业叙事里**完全缺席**——最关键的硬件/平台方不押 JEPA | [NVIDIA Developer Blog](https://developer.nvidia.com/blog/pretrained-to-imagine-fine-tuned-to-act-the-rise-of-world-action-models/)（2026） |
| "五种世界模型路径"中 JEPA 只占 1 席 | Themesis 2026 年 1 月横向对比把世界模型归为五种竞争路径：Google DeepMind（SIMA 2/Genie 3）、World Labs（Marble，NeRF 基、非 JEPA）、AMI Labs（JEPA）、Decart、Wayve。JEPA = 1/5，不是主流 | [Themesis](https://themesis.com/2026/01/07/world-models-five-competing-approaches/)（2026.01） |
| Cosmos 是生成式（像素空间）而非 JEPA（潜空间），且已落地 | NVIDIA Cosmos 训练于 ~2000 万小时视频 + 9000T token，已用于 AV 与机器人合成数据；是产业最重的世界模型押注，**架构上与 JEPA 对立**（生成式 vs 预测式） | [arXiv 2501.03575](https://arxiv.org/html/2501.03575v1)；[Introl](https://introl.com/blog/world-models-race-agi-2026) |
| 最被引用的 JEPA 结果只是 15M 参数、单 GPU | LeWM（LeWorldModel）是 JEPA 阵营近期最吸睛的成果——但仅 15M 参数、单 GPU 训练。与"JEPA 是下一代主流架构"的叙事严重不匹配 | [arXiv 2603.19312](https://arxiv.org/html/2603.19312v1)；[Medium/AIGuys](https://medium.com/aiguys/lecuns-world-model-is-real-useful-and-nowhere-near-as-new-as-the-funding-round-implies-ecc3b05e2204) |
| V-JEPA 2 已超 12 个月无重大升级 | V-JEPA 2 于 2025-06-25 发布，参数量 ViT-g（~1B）。R3 必查项要求"向 10B+ 推进"——**未发生**。Meta 至今未发 V-JEPA 3，语言-视觉 JEPA 路线停滞 | [Meta AI Blog](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/)（2025.06） |

**熊方结论**：H1 的"主流"判定被 NVIDIA/Cosmos/World Labs 架构竞争稀释。JEPA 是 Meta 内部主线，但产业层面只是 5 条路径之一，且硬件龙头（NVIDIA）不押它。72% → 应降至 55-60%。

---

### H2：JEPA 语言突破（R2 信心 25%）→ 应下调至 12-15%（"观察"触发条件 #1 已实质命中）

| 攻击 | 证据 | 来源/日期 |
|------|------|-----------|
| 社区共识："JEPA 不为语言优化" | Reddit r/artificial 顶层讨论明确："the JEPA model is not optimized for language"——JEPA 设计点在视觉/机器人，语言是结构性短板 | [Reddit r/artificial](https://www.reddit.com/r/artificial/comments/1tjuats/so_what_is_yann_lecuns_world_models_and_jepa_and/) |
| 唯一的"LLM-JEPA"只是微调附件，非突破 | arXiv 2509.14252《LLM-JEPA》把 JEPA 用作 LLM 微调的自监督辅助，**不是用 JEPA 架构从头做语言**。是寄生在 LLM 上的增强，不是替代 | [arXiv 2509.14252](https://arxiv.org/html/2509.14252v1) |
| LeJEPA 形式化证明的适用条件极窄 | Klindt/LeCun/Balestriero（2026-05-25）证明 LeJEPA 能恢复隐变量**当且仅当隐变量为高斯分布**。这是 toy-model 理论，不是真实语言/视觉的可扩展性证明。论文标题反问"何时学到世界模型"——答案是"只在理想化假设下" | [arXiv 2605.26379](https://arxiv.org/html/2605.26379v1)；[alphaXiv](https://www.alphaxiv.org/abs/2605.26379)（2026.05） |
| Benchmark 反证当前模型"脆弱" | 同期 Tech Times 报道：JEPA 形式证明发布同时，benchmark 发现"current models brittle"——连 JEPA 阵营自己都承认现状不堪用 | [Tech Times](https://www.techtimes.com/articles/317452/20260531/yann-lecuns-world-model-earns-formal-proof-benchmark-finds-current-models-brittle.htm)（2026.05.31） |
| 06.05→07.10 零语言进展 | ICML 2026 论文列表中 JEPA 相关仅 Causal-JEPA（物体级因果）与 Policy-Driven World Model（离线 RL），**无一条语言突破** | [ICML 2026 Papers](https://icml.cc/virtual/2026/papers.html) |

**熊方结论**：H2 已实质命中 R2 设定的下调触发条件 #1（"2027 年底 JEPA 仍无语言突破"——现在 2026 年中已经可以判定趋势）。25% → 12-15%。LeCun 自己的赌注是"语言"，但他的产出全在视觉/机器人。

---

### H3：算力需求降 10-100x（R2 信心 17%）→ 维持或下调至 10-12%

| 攻击 | 证据 | 来源/日期 |
|------|------|-----------|
| AMI Labs 拿 $1.03B 后仍在烧大算力 | 世界模型训练仍需互联网级视频（V-JEPA 2 ~100 万小时；Cosmos ~2000 万小时）。"高效"是相对的，绝对算力门槛未降 | Meta/NVIDIA 训练规模披露 |
| Hyperscaler CapEx 不降反升（见下文 H4） | 若 JEPA 真能降 10-100x 算力，$700B CapEx 应见顶——它没有。市场用钱投票，不信"效率叙事" | Goldman/Yahoo Finance（2026） |

**熊方结论**：H3 在 R2 已低（17%），R3 无任何新证据上调，应维持或微降。

---

### H4：LLM 生态壁垒阻止 JEPA（R2 信心 80%）→ 应上调至 88-90%

| 攻击 | 证据 | 来源/日期 |
|------|------|-----------|
| 2026 CapEx ~$700B，长期 $5.3T，全部投向 Transformer | Goldman 预测四大 Hyperscaler 长期 CapEx 合计 **$5.3 万亿**；2026 单年 ~$700B（同比 +77%）。**没有任何削减信号**。R2 设的"上调至有条件通过"条件 #3（Hyperscaler 削减 CapEx 指引）距离触发无限远 | [Yahoo Finance/Goldman](https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html)；[ValueAdd VC $725B Tracker](https://www.valueadd.vc/) |
| NVIDIA/AMD/Broadcom TPU 路线锁死 Transformer | 整个 AI 硬件栈（GPU/HBM/TPU/网络）为 Transformer 优化，合同锁定到 2027+。JEPA 的"CapEx 削减利好"触发条件可能**永远不会发生** | 产业链合同披露 |
| 开源 LLM 进一步逼近闭源 | DeepSeek V4 / Qwen 3.5 / Llama 4 持续缩小差距，Qwen 下载量破 10 亿。Transformer 生态自我强化，JEPA 的生态缺口在扩大而非缩小 | R2 已记录，R3 无反转 |

**熊方结论**：H4 不只是"阻止 JEPA"，而是"生态护城河每季度加深"。80% → 88-90%。这是 JEPA 最难翻越的墙。

---

### H5：混合方案成主流（R2 信心 80%）→ 应下调至 60-65%（"混合"是 JEPA 被吞的委婉语）

| 攻击 | 证据 | 来源/日期 |
|------|------|-----------|
| 若 LLM 已在做多模态/世界模型，"混合"= JEPA 被吸收 | Sora 2 被 OpenAI 明确定位为"world simulator"，开发"尊重物理的内部世界模拟器"。Sequoia 播客证实 Sora 2 团队的世界模型路线图。**LLM 阵营不需要 JEPA 也能做世界模型** | [OpenAI](https://openai.com/index/video-generation-models-as-world-simulators/)；[Sequoia Podcast Sora 2](https://sequoiacap.com/podcast/openai-sora-2-team-how-generative-video-will-unlock-creativity-and-world-models/) |
| GPT-5/Gemini/Claude 全是 VLM，已具备视觉推理 | Not Boring 深度指出"GPT-5、Gemini、Claude 都是 VLM，能看能推理"。前沿 LLM 已是事实上的多模态世界模型（弱版本） | [Not Boring](https://www.notboring.co/p/world-models) |
| World Labs Marble 已是商用世界模型，且非 JEPA | Fei-Fei Li 的 World Labs 于 2025-11 发布 Marble（3D 空间世界模型，NeRF 基），**已有商业产品**。AMI Labs 无产品。"混合"在市场上已被非-JEPA 路径实现 | [TechCrunch Marble](https://techcrunch.com/2025/11/12/fei-fei-lis-world-labs-speeds-up-the-world-model-race-with-marble-its-first-commercial-product/)（2025.11） |
| "混合"叙事下 JEPA 的独立贡献不可辨识 | 如果 LLM 负责语言 + Sora 负责视频世界模型 + VLA 负责机器人动作 + Cosmos 负责合成数据——JEPA 在"混合"里负责什么独立、不可替代的模块？答不出，则"混合"就是 JEPA 被稀释的修辞 | 逻辑推演 |

**熊方结论**：H5 的"混合"若是 JEPA+LLM 各占一半，则 80% 合理；但现实是 LLM 阵营正以非-JEPA 手段完成"世界模型"功能，JEPA 在混合中的份额趋零。80% → 60-65%，且应标注"混合 = 被吸收"的风险。

---

## 二、情景 D（JEPA 完全失败）与 C（LLM 吸收 JEPA）应上调多少

### R2 → R3 熊方建议

| 情景 | R2 | 熊方R3建议 | 变化 | 依据 |
|------|-----|-----------|------|------|
| A：JEPA 独立成功 | 10% | **5%** | -5pp | 无任何新证据支撑；AMI 无产出、无第三方采纳 |
| B：JEPA+LLM 融合 | 50% | **35%** | -15pp | "融合"被 LLM 阵营单方面实现（Sora/Cosmos/VLA），JEPA 独立贡献被稀释 |
| C：LLM 吸收 JEPA | 25% | **40%** | +15pp | 最危险的证伪路径正在加速：LLM 多模态 + 视频生成 + 具身 VLA 三路并进，JEPA 作为独立架构的必要性下降 |
| D：JEPA 完全失败 | 15% | **20%** | +5pp | AMI 4 个月零产出 + 学术质疑 + 历史类比（Mamba）+ 0.15% 资金占比 |

**合计 100%。** 注意：C+D = 60%，意味着熊方认为"JEPA 作为独立架构消失或失败"的概率过半。

---

## 三、最强 3 个"下调至观察"的论据

### 论据 1：AMI Labs 的"静默 4 个月"——$1.03B 后零产出，符合下调条件 #2

R2 明确设定下调条件 #2："AMI Labs Series A 融资困难或估值下调"。虽然未发生估值下调，但**更致命的信号已出现**：

- AMI Labs 官网（amilabs.xyz）无任何研究/产品/论文发布
- French Tech Journal 的 AMI Tracker 最新动态仅停留在"Mar 2026 team"
- 招聘页（Ashbyhq）仅 5 个开放职位——$3.5B 估值公司、4 个月只招 5 个岗
- 对比：World Labs（Fei-Fei Li）同期已发布 Marble 商用产品；NVIDIA 已发布 Cosmos Reason

**$1.03B 不是验证信号，是 LeCun 个人品牌的变现。** 资本押的是"LeCun 诺奖光环"，不是 JEPA 的工程验证。12 人团队 + 零产品 + 研究周期以年计 = 烧钱周期已启动。若 2026 Q4 仍无世界级成果，估值下调是大概率事件。

来源：[Futurum Group](https://futurumgroup.com/insights/yann-lecuns-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/)；[AMI Labs 官网](https://amilabs.xyz/)；[French Tech Journal Tracker](https://ami.frenchtechjournal.com/)

### 论据 2：H2（语言突破）已实质命中下调条件 #1，可提前判定

R2 下调条件 #1："2027 年底 JEPA 仍无语言突破"。我们不需要等到 2027：

- 06.05→07.10 五周内，JEPA 语言方向**零进展**
- 唯一相关论文（LLM-JEPA）是 JEPA 寄生于 LLM 的微调增强，不是 JEPA 替代 LLM 做语言
- LeJEPA 形式证明只在高斯隐变量假设下成立——toy model，不是真实语言
- LeCun 自己的核心论点"LLM 是死胡同"正在被 LLM 阵营的持续进化（GPT-5.4/Opus 4.6/Gemini 3.1）证伪

**LeCun 赌的是"语言必须用 JEPA 重做"，但 18 个月过去了，他没有任何语言成果，只有视觉/机器人。** 这是方向性失败的早期信号。来源：[arXiv 2605.26379](https://arxiv.org/html/2605.26379v1)；[Reddit r/agi LeCun 立场](https://www.reddit.com/r/agi/comments/1imqson/lecun_if_you_are_interested_in_humanlevel_ai_dont/)

### 论据 3：情景 C（LLM 吸收世界模型）正在加速，符合下调条件 #3

R2 下调条件 #3："LLM 在物理推理/机器人领域取得突破（多模态整合）"。这正在发生：

- **OpenAI Sora 2**：被定位为"world simulator"，团队公开讨论"尊重物理的内部世界模拟器"
- **NVIDIA Cosmos**：2000 万小时视频训练的生成式世界模型，已用于 AV/机器人合成数据；提出 WAM（World-Action Model）框架，JEPA 不在其内
- **VLA 模型**（PaLM-E、RT-2 后继）：LLM 直接输出机器人动作，跳过 JEPA 的"潜空间预测"中间层
- **Google DeepMind**：Genie 3 / SIMA 2 走自己的世界模型路径

**当 LLM 阵营用 Transformer 原生架构（视频生成 + VLA + 多模态）实现了 JEPA 想实现的世界模型功能，JEPA 作为"独立架构"的存在理由就消失了。** 这不是 JEPA+LLM 融合（情景 B），这是 JEPA 被 LLM 吞掉（情景 C）。

来源：[OpenAI Sora](https://openai.com/index/video-generation-models-as-world-simulators/)；[NVIDIA Cosmos arXiv](https://arxiv.org/html/2501.03575v1)；[Sequoia Sora 2 Podcast](https://sequoiacap.com/podcast/openai-sora-2-team-how-generative-video-will-unlock-creativity-and-world-models/)

---

## 四、历史类比表 — "更优雅但未被采纳"的架构

| 架构 | 提出者 | "更优"主张 | 实际结局 | 与 JEPA 的相似度 |
|------|--------|-----------|----------|-----------------|
| **Mamba（SSM）** | Gu & Dao | O(N) 线性复杂度 vs Transformer O(N²)；5x 推理速度 | Reddit r/MachineLearning 专帖"Why MAMBA did not catch on"——hype 后生态未跟上，Transformer 仍统治。被吸收为 MoE 混合组件，非独立替代 | ★★★★★（极相似：效率优势真实，但生态/硬件惯性碾压） |
| **Capsule Networks** | Hinton | 等变性、部分-整体关系，比 CNN 更优的归纳偏置 | 从未取代 CNN；Transformer 出现后更边缘化。仅医疗等垂直小场景 | ★★★★（诺奖级人物押注，学术界叫好，产业界不采纳） |
| **Energy-Based Models** | LeCun 自己 | 统一概率框架，原理优雅 | LeCun 推了 15 年未成主流；他自己转向 JEPA = 变相承认 EBM 未竟 | ★★★★★（同一人、同一"更优雅"叙事、同样的采纳困境） |
| **Neural Turing Machines / Memory-Augmented Networks** | DeepMind | 外部可微内存，解决长程依赖 | 被 Transformer 的注意力机制 + RAG 取代；概念被吸收，架构未存活 | ★★★★（被"粗暴但有效"方案吸收） |
| **Sparse RNN / Liquid Neural Networks** | 多方 | 生物启发、高效、可解释 | 利基应用（无人机控制），从未主流 | ★★★ |

**模式总结**：AI 历史上"学术更优雅 + 效率更高"的架构，在 Transformer 时代几乎全部未取代"粗暴但有效"的自回归/注意力范式。JEPA 正在精准重演这个模式——LeCun 的 Energy-Based Models 就是前车之鉴（他自己放弃了）。

来源：[Reddit r/ML Mamba](https://www.reddit.com/r/MachineLearning/comments/1hpg91o/d_why_mamba_did_not_catch_on/)；[DeepLearning.ai The Batch](https://www.deeplearning.ai/the-batch/mamba-a-new-approach-that-may-outperform-transformers)

---

## 五、对"维持技术关注"的反驳 — 为何应下调至"观察"

多头研究员可能会主张"维持技术关注"——理由是 AMI $1.03B 是非零资本信号、LeCun 形式证明是理论进展、World Model 概念破圈。这些我都承认，但逐一反驳：

### 反驳 1：$1.03B 是 0.15% 的噪音，不是信号

- $1.03B / $700B = **0.147%**。即使翻 10 倍到 $10B，也仅 1.47%
- World Labs（Fei-Fei Li）也融了 ~$1B——**世界模型资金里 JEPA 路线（AMI）不占多数**，NeRF/生成式路线（World Labs）分庭抗礼
- "资本信号从零到非零"听起来动听，但绝对量级说明：**市场不认为 JEPA 是下一代主流**，市场认为 Transformer 是
- Goldman 预测的 $5.3T 长期 CapEx，是 JEPA 全部融资的 **5000 倍**

### 反驳 2：形式证明是"理论补丁"，不是工程突破

- LeJEPA 证明只在**高斯隐变量**下成立——这是教科书 toy model 假设
- LeCun 在 Meta 时期推 JEPA 多年，临走才发理论证明 = 此前一直是"经验性架构"，理论是事后补的
- benchmark 同期发现"current models brittle"——**连 JEPA 阵营自己都承认现状不可用**
- 形式证明 ≠ 可扩展性证明 ≠ 产品。学术进展到产业落地之间是"死亡之谷"

### 反驳 3：World Model "破圈"是泡沫信号，不是真进展

- AMI CEO Alexandre LeBrun **自己**预测："六个月内，每家公司都会自称 World Model 公司来融资"
- Rex Woodbury（Digital Native）提名"World Model"为 **2026 年度科技热词**，同时预测 AI 搜索基金泡沫破裂
- 当概念被用来融资的程度超过它被用来做产品的程度，信号噪音比已恶化
- 这符合 Gartner 炒作周期的"膨胀期望顶峰"——接下来是幻灭低谷

### 反驳 4：学术质疑是实在的

- Hacker News 顶层评论："Lecun still can't show JEPA competitive at scale with autoregressive LLM"
- "From Dead End to Hybrid AI: What LeCun Gets Wrong About Language"——直接反驳
- CU Denver 研究者公开提出不同路径
- LeCun 的"LLM 是死胡同"论被 GPT-5.4/Opus 4.6/Gemini 3.1 的持续进化**逐月证伪**

来源：[French AI Report 2026](https://www.linkedin.com/posts/laurencehemery_the-french-ai-report-2026-activity-7470731810931564545-Wavu)；[Digital Native 26 Predictions](https://www.digitalnative.tech/p/26-predictions-for-2026-part-ii)；[HN LeJEPA](https://news.ycombinator.com/item?id=45960922)；[AI Plain English 反驳](https://ai.plainenglish.io/from-dead-end-to-hybrid-ai-what-yann-lecun-gets-wrong-about-language-93164517b607)

### 熊方评级建议

**下调至「观察」。** 触发的硬条件：
1. H2（语言突破）已实质命中 R2 下调条件 #1——零语言进展 + 唯一论文是寄生微调
2. AMI Labs 4 个月静默 + 仅 5 个招聘岗位 + 零产品 = 下调条件 #2（融资困难/估值虚高）的早期形态
3. 情景 C（LLM 吸收）加速——Sora 2/Cosmos/VLA 三路独立实现世界模型，JEPA 独立性被掏空

**保留"观察"而非"否决"的唯一理由**：LeCun 个人品牌 + AMI 资金存量仍允许 1-2 年的研究周期。若 2027 Q1 AMI 仍无世界级成果，则应彻底否决。

---

## 六、来源链接（按日期）

### 2026 年（R2 后）

- **[2026.07] AMI Labs Tracker（French Tech Journal）** — 仅停留在 Mar 2026 team 更新，无研究产出 — https://ami.frenchtechjournal.com/
- **[2026.06] ICML 2026 Papers** — JEPA 相关仅 Causal-JEPA、Policy-Driven World Model，无突破 — https://icml.cc/virtual/2026/papers.html
- **[2026.05.31] Tech Times：LeCun World Model 获形式证明，benchmark 发现模型脆弱** — https://www.techtimes.com/articles/317452/20260531/yann-lecuns-world-model-earns-formal-proof-benchmark-finds-current-models-brittle.htm
- **[2026.05.25] Klindt/LeCun/Balestriero：When Does LeJEPA Learn a World Model（arXiv）** — 高斯假设下的 toy model 证明 — https://arxiv.org/html/2605.26379v1
- **[2026.03.09] TechCrunch：AMI Labs $1.03B seed** — https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/
- **[2026.03] Futurum Group：AMI $1B seed 分析** — https://futurumgroup.com/insights/yann-lecuns-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/
- **[2026.03] Verdantix：AMI CEO 预测"六个月内每家公司自称 World Model"** — https://www.verdantix.com/insights/blog/the-world-cup-is-now--are-world-models-next
- **[2026.01.22] MIT Technology Review：AMI Labs 专访（LeCun 对赌 LLM）** — https://www.technologyreview.com/2026/01/22/1131661/yann-lecuns-new-venture-ami-labs/
- **[2026.01.07] Themesis：五种世界模型竞争路径** — JEPA 仅 1/5 — https://themesis.com/2026/01/07/world-models-five-competing-approaches/
- **[2026.01] Digital Native（Rex Woodbury）：World Model = 2026 年度科技热词 + AI 泡沫预测** — https://www.digitalnative.tech/p/26-predictions-for-2026-part-ii
- **[2026] Goldman Sachs via Yahoo Finance：四大 Hyperscaler 长期 $5.3T CapEx** — https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html
- **[2026] NVIDIA Developer Blog：World-Action Models（WAMs）框架，不含 JEPA** — https://developer.nvidia.com/blog/pretrained-to-imagine-fine-tuned-to-act-the-rise-of-world-action-models/
- **[2026] French AI Report 2026（CEO 自述泡沫）** — https://www.linkedin.com/posts/laurencehemery_the-french-ai-report-2026-activity-7470731810931564545-Wavu

### 2025 年及更早（背景）

- **[2025.11.12] TechCrunch：World Labs 发布 Marble（非-JEPA 商用世界模型）** — https://techcrunch.com/2025/11/12/fei-fei-lis-world-labs-speeds-up-the-world-model-race-with-marble-its-first-commercial-product/
- **[2025.06.25] Meta AI：V-JEPA 2 发布（~1B 参数，12 个月无后继）** — https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/
- **[2025] OpenAI：Sora 作为 world simulator** — https://openai.com/index/video-generation-models-as-world-simulators/
- **[2025] arXiv LLM-JEPA（JEPA 寄生于 LLM 微调）** — https://arxiv.org/html/2509.14252v1
- **[2025] Hacker News：LeJEPA 讨论——"JEPA 未在大规模上击败 LLM"** — https://news.ycombinator.com/item?id=45960922
- **[2025] Reddit r/MachineLearning：Why MAMBA did not catch on** — https://www.reddit.com/r/MachineLearning/comments/1hpg91o/d_why_mamba_did_not_catch_on/
- **[2025] NVIDIA Cosmos（arXiv）** — https://arxiv.org/html/2501.03575v1
- **[2025] Not Boring：World Models 深度（GPT-5/Gemini/Claude 都是 VLM）** — https://www.notboring.co/p/world-models

---

## 附：熊方一句话交付

> **"维持技术关注"是对 LeCun 品牌的礼貌，不是对 JEPA 工程现实的判断。R2 设的三个下调条件中，#1（语言突破失败）已实质命中、#2（AMI 困难）正在形成、#3（LLM 物理突破）由 Sora 2/Cosmos/VLA 加速触发。CIO 应下调至「观察」，并把 AMI Labs 2027 Q1 成果作为唯一的复活条件。在 LLM 阵营自我实现世界模型的 2026 年，继续给 JEPA "技术关注"评级，是用 2022 年的认知锚定 2026 年的现实。**
