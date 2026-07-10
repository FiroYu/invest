# 宏观研究员报告 — #01 JEPA vs LLM（Round 3，07.10）

> 2026-07-10 | 角色：宏观/资金/估值/跨资产传导研究员
> 窗口：2026-06-05 → 2026-07-10（约 5 周）
> 审阅对象：PM + CIO + 魔鬼辩护人

---

## 一、执行摘要（TL;DR）

**核心宏观判断：CapEx 进入「债务融资」阶段，架构锁定效应加深，JEPA 窗口进一步收窄。**

R2→R3 最重要的宏观变化不是 CapEx 削减（升级条件 #3 未触发），而是 **CapEx 从现金流融资转向债务融资**——Amazon 自由现金流被压毁 95%（-FCF ~$17B），Oracle FCF 转负（-$24B，股价单日跌 11%），五大巨头合计 FCF 预计跌 >70% 至 ~$100B。这意味着 Hyperscaler 在利率走高（10Y UST 4.56%，7 月初两周内从 4.38%→4.56%）的环境下**借债加注 Transformer**，这是比现金支出更强的架构锁定信号。同时 DeepSeek V4 用 MoE 将推理成本降 50x，**抽走了 JEPA 的「高效」独有叙事**——Transformer 路线自身正在变高效。JEPA 产业资金占比仍为 ~0.15%，无新融资、无第三方采纳。

---

## 二、Delta 摘要表（★ 排序，06.05→07.10）

| ★ | 事件/数据 | 日期 | 来源 | 对 JEPA 影响 |
|---|----------|------|------|-------------|
| ★★★★★ | **CapEx 进入债务融资阶段**：Amazon -FCF ~$17B（FCF 压毁 95%），Oracle -FCF $24B（6/10 财报后跌 11%），5 巨头合计 FCF 跌 >70% 至 ~$100B；Amazon 再借 $25B，Oracle 拟融资 $45-50B | 06.10-07.08 | CNBC/Reuters/MarketWatch/Breckinridge | **利空**：债务锁定 = 比现金更强的架构承诺，升级条件 #3（CapEx 削减）远离触发 |
| ★★★★★ | **Goldman 上调 2027 CapEx 至 $1.1T**（原 $920B，上行 $1.4T），2026 基线 $765B→2031 $1.6T；同时发布「AI: In a Bubble?」警告投资循环性 | 06-07 月 | Goldman Sachs Research | **利空**：CapEx 绝对值持续膨胀，全部投向 Transformer |
| ★★★★☆ | **DeepSeek V4「效率革命」**：MoE 架构推理成本低 50x，Forbes 称「下一场竞赛是效率」；支持华为芯片 | 04.24-26 | Forbes/PYMNTS/Fortune/Lightning.ai | **两面性，净利空**：验证效率叙事但被 LLM 路线吸收——JEPA 不再是「高效」唯一选项 |
| ★★★★☆ | **10Y UST 升至 4.56%**（7/8），两周内 4.38%→4.56%，逼近 52 周高 4.690%；Fed 6/17 暂停于 3.50-3.75%；JPM 预计 2026 全年不降息+2027.09 可能加息 | 06.17-07.08 | FRED/Fed/CNBC/JPM/iShares | **利空**：高贴现率压制 AMI Labs 等长周期研究型公司估值 |
| ★★★★☆ | **LLM 开源生态锁定**：Qwen 下载量破 10 亿（3 月，最快达此里程碑），DeepSeek V4/Qwen 3.5/Llama 4 全线逼近闭源前沿，全部 Transformer | 03-06 月 | Forbes/Particula.tech/HuggingFace | **强利空 H4**：开发者生态锁定加深 |
| ★★★☆☆ | **6/1 美国商务部将芯片禁令延伸至海外中资企业**；Chatham House/CSIS 质疑出口管制效果；DeepSeek V4 支持华为芯片 | 06.01 | Al Jazeera/Chatham House/CSIS | **利空**：中国 AI 路线锁定 Transformer（DeepSeek/Qwen 为旗舰），JEPA 无地缘赞助者 |
| ★★★☆☆ | **能源约束确认加深**：数据中心占美国新增电力 ~50%（确认），EPRI 预测 2030 年达美国总发电量 9%；time-to-power 成决定性瓶颈 | 持续 | DOE/EPRI/MarketScale/Harvard Belfer | **两面性**：理论上利好高效架构，但政策反应是建更多核电而非换架构 |
| ★★★☆☆ | **机器人世界模型收敛**：1X World Model（900 小时第一人称视频训练）、V-JEPA 2（1.2B 参数，零样本规划 65-80% 成功率）、Figure/Tesla 均朝世界模型方向 | 2025-26 | Meta AI/1X.tech/Robot Report | **利好 H1**：机器人物理世界建模确认走世界模型路线 |
| ★★☆☆☆ | **ICML 2026（华盛顿）**：Causal-JEPA 论文入选；LeCun 在 MILA（2/4）和 NYU 做世界模型主题演讲，但无 ICML 官方主题演讲确认 | 06-07 月 | icml.cc/LeCun FB/LinkedIn | **中性**：学术存在感维持，无突破性论文 |
| ★★☆☆☆ | **NVIDIA $194-215（较 5/14 ATH 回撤 14-16%）**，估值压缩至「AI 前最低」；GTC 2026 黄仁勋 flagged $1T Blackwell+Vera 需求；定制硅片占 AI 芯片份额 20.9%→27.8% | 06-07 月 | Yahoo/Capital.com/Intellectia.ai | **中性**：市场定价 CapEx 可持续性风险，未定价架构更替风险 |
| ★★☆☆☆ | **AMI Labs 仍为 $1.03B/12 人/4 城（巴黎/纽约/蒙特利尔/新加坡），无新融资、无研究成果发布** | 03 至今 | TechCrunch/Futurum/Cathay Capital | **利空**：R2 升级条件 #1（世界级成果）未触发 |

---

## 三、风险因子交互表

| 风险因子 | 当前状态（07.10） | R2（06.04）状态 | 趋势 | 对 JEPA 净影响 |
|---------|-----------------|----------------|------|---------------|
| **AI CapEx 总量** | 2026: ~$700-765B（4 巨头 $610-700B + Oracle $55B）；Goldman 2027: $1.1T（上行 $1.4T） | $700B（4 巨头指引） | ↑ 加速 | **利空**：全部投向 Transformer，JEPA 占比从 0.15% 进一步稀释 |
| **CapEx 融资模式** | **债务融资阶段**：Amazon -FCF $17B/Oracle -FCF $24B/5 巨头合计 FCF 跌 >70%；Amazon 再借 $25B+，Oracle 拟融 $45-50B | 现金流为主（FCF 尚正） | ↑↑ 阶段转变 | **强利空**：债务 = 比现金更强的架构锁定（沉没成本 + 债权人义务） |
| **10Y UST 利率** | **4.56%**（7/8），两周内 +18bp；52 周区间 3.923%-4.690% | ~3.50-3.75%（Fed funds） | ↑ 鹰派 | **利空**：高贴现率压制 AMI Labs（无收入长周期研究）；但 Hyperscaler 不顾利率加注 |
| **Fed 路径** | 6/17 暂停于 3.50-3.75%；JPM 预计全年不降+2027.09 可能加息；iShares 预计降息 | 3.50-3.75% | → 分歧加大 | **利空**：流动性预期收紧，私募融资环境趋紧 |
| **LLM 生态壁垒** | Qwen 10 亿下载；DeepSeek V4 推理 50x 便宜；开源全线逼近闭源 | Qwen 7 亿下载 | ↑ 强化 | **强利空 H4**：开发者锁定 + 效率叙事被 LLM 吸收 |
| **能源/电力** | 数据中心占新增电力 ~50%（确认）；EPRI: 2030 年 9% 总发电量 | ~50% 新增 | → 持续 | **两面性**：政策反应是建核电而非换架构 |
| **中美脱钩** | 6/1 延伸至海外中资；DeepSeek V4 支持华为；主权 AI 叙事 | 出口管制持续 | ↑ 加速 | **利空**：中国路线锁定 Transformer；JEPA 无地缘赞助者 |
| **AI 泡沫风险** | Goldman「AI: In a Bubble?」报告；循环性警告；NVIDIA 回撤 14-16% | ROI 质疑渐起 | ↑ 风险上升 | **两面性**（见下文 §六） |
| **私募流动性** | 10Y UST 4.56% + Fed 路径分歧 → 长周期 VC 谨慎 | 尚可 | ↓ 收紧 | **利空**：AMI Labs 后续融资难度上升 |

---

## 四、跨课题传导更新

### #17 推理芯片 / AI 泡沫
- **传导增强**：Goldman「AI: In a Bubble?」报告正式量化了投资循环性风险（AI 公司投资 AI 公司）。Oracle 6/10 财报 -FCF $24B + 股价跌 11% 是**首个 Hyperscaler 级别的 CapEx 可持续性警告信号**。
- **对 JEPA 影响**：若 CapEx 崩塌（#17 Bear 30%），JEPA 面临两面性——短期同跌（风险资产全跌），但中长期若政策推动「高效架构」则受益。但 R3 关键发现：**当前 CapEx 不是在削减而是在借债加注**，这使得短期 Bear 情景的概率低于 R2 预期。

### #11 机器人 / 具身智能
- **传导正向**：1X World Model、V-JEPA 2、Figure、Tesla Optimus 均朝世界模型收敛。JEPA 为机器人提供技术基础的假设（H1）持续验证中。
- **但**：机器人世界模型 ≠ JEPA。1X 的世界模型是生成式的（非 JEPA 能量模型），V-JEPA 2 的零样本规划成功率（65-80%）虽是 SOTA 但离工业部署仍有距离。

### #21 / #04 Hyperscaler CapEx
- **共同变量**：$700-765B 2026 CapEx 全部投向 Transformer 基础设施。Goldman 上调至 $1.1T（2027）。这是 JEPA 的**最大宏观阻力**——可用的算力、数据中心、HBM 全部为 Transformer 架构优化。

### #14 能源
- **耦合维持**：数据中心占美国新增电力 ~50%（确认），EPRI 预测 2030 年 9% 总发电量。但政策反应是加速核电 PPA（Constellation/Vistra）和天然气项目，**不是推动架构效率革命**。JEPA 的「高效」叙事尚未获得政策推动力。

---

## 五、对 H1-H5 的宏观判断

| 假设 | R3 信心 | R2 信心 | 变化 | 宏观依据 |
|------|---------|---------|------|---------|
| **H1：JEPA 视觉/机器人主流** | **74%** | 73% | +1pp | 机器人世界模型收敛（1X/V-JEPA 2/Figure）持续验证；但能源约束未转化为架构推动力 |
| **H2：JEPA 语言突破** | **22%** | 28% | **-6pp** | LLM 前沿加速（GPT-5.5/Claude Fable 5/Gemini 3.1 Pro SWE-bench 90%+）；DeepSeek V4 MoE 证明 LLM 路线自身可大幅提效；JEPA 零语言进展 |
| **H3：算力需求降 10-100x** | **14%** | 18% | **-4pp** | DeepSeek V4 推理 50x 便宜（MoE）= Transformer 自身变高效；JEPA 不再是「降低算力」的唯一路径；Hyperscaler 债务融资 $700B+ 扩大算力供给 |
| **H4：LLM 生态壁垒阻止 JEPA** | **86%** | 80% | **+6pp** | Qwen 10 亿下载；DeepSeek V4 开源前沿；开发者生态全面 Transformer 锁定；中美两国 AI 路线均锁定 Transformer |
| **H5：混合方案成主流** | **82%** | 80% | +2pp | 机器人世界模型 + 语言 LLM 的分层共存模式持续确认；NVIDIA Cosmos 3 推动物理 AI 工具链 |

---

## 六、情景 C「LLM 吸收 JEPA」的宏观深度分析

**R3 核心论点：情景 C 概率应从 25% 上调至 30%，因为 DeepSeek V4 抽走了 JEPA 的「高效」独有叙事。**

### C 情景的宏观机制

```
DeepSeek V4 MoE（推理 50x 便宜）
  → 证明 Transformer 路线自身可大幅提效
    → JEPA「高效架构」独特价值主张被稀释
      → LLM 路线吸收「效率」叙事
        → JEPA 作为独立架构的差异化消失
```

### 三重锁定效应（R3 新增）

1. **资金锁定**：$700B+ CapEx（债务融资）→ 全部 Transformer 基础设施 → 沉没成本效应
2. **生态锁定**：Qwen 10 亿下载 + DeepSeek V4 开源前沿 → 开发者心智份额全面 Transformer
3. **效率锁定（新）**：DeepSeek V4 MoE 推理 50x 便宜 → 「高效」不再是 JEPA 专利 → JEPA 差异化被吸收

### C 情景触发信号（监测）

- [ ] OpenAI/Google/Anthropic 在研究中提及 JEPA/世界模型作为**其模型的组件**（而非独立架构）
- [ ] AMI Labs 团队成员流失至 Hyperscaler（被吸收）
- [ ] LeCun 公开表态与某 Hyperscaler 合作而非独立
- [ ] 主流分析框架不再区分「JEPA vs LLM」而是「LLM + 世界模型模块」

---

## 七、AI 泡沫风险的两面性分析

### 短期（若 CapEx 崩塌，#17 Bear 30%）
- **JEPA 同跌**：AMI Labs 等风险资产全跌；私募融资冻结；NVIDIA/芯片股崩塌拖累整个 AI 板块
- **无例外**：2000 年互联网泡沫中，即使「正确方向」的公司也跌 80%+

### 长期（若 CapEx 崩塌后政策转向）
- **JEPA 可能受益**：若政策制定者将「高效架构」作为应对 AI 能源危机的工具
- **但 R3 发现**：当前政策反应是建核电而非换架构 → 长期政策推动力**弱于 R2 预期**

### R3 关键修正
R2 假设「CapEx 崩塌 → JEPA 反而获政策推动」。R3 数据显示：CapEx **不是在崩塌而是在借债加注**（Amazon -FCF/Oracle -FCF），这使得短期 Bear 情景概率**低于 R2 预期**，JEPA 的「反向受益」路径更远。

---

## 八、市场对「架构之争」的定价

**结论：市场完全未定价架构更替风险。**

- NVIDIA（$194-215，较 ATH 回撤 14-16%）：回撤原因 = CapEx 可持续性担忧 + 定制硅片竞争，**非架构不确定性**
- 定制硅片份额 20.9%→27.8%：这是**Transformer 推理芯片**的内部竞争，非 JEPA
- 无卖方报告发现提及 JEPA/世界模型作为投资风险因子
- Goldman「AI: In a Bubble?」：讨论估值循环性，未提及架构路线风险
- **定价含义**：架构之争仍属「学术关注」范畴，未进入机构投资者风险雷达

---

## 九、情景概率建议（A/B/C/D 合计 100%）

| 情景 | R2 概率 | R3 建议 | 变化 | 依据 |
|------|---------|---------|------|------|
| **A：JEPA 独立成功**（取代 LLM 成主流） | 10% | **8%** | -2pp | 债务融资锁定 + 无第三方采纳 + AMI Labs 无成果 |
| **B：JEPA+LLM 融合**（主情景） | 50% | **48%** | -2pp | 机器人世界模型验证融合路径，但基础设施层仍全 Transformer |
| **C：LLM 吸收 JEPA** | 25% | **30%** | +5pp | DeepSeek V4 抽走效率叙事 + 三重锁定效应（资金/生态/效率） |
| **D：JEPA 完全失败** | 15% | **14%** | -1pp | AMI Labs $1B 资本信号虽小但非零；机器人世界模型维持学术活力 |
| **合计** | 100% | **100%** | — | — |

**净变化方向**：概率质量从 A/B 向 C 转移。JEPA 作为独立架构存活的概率下降，被 LLM 生态吸收的概率上升。

---

## 十、评级建议

**维持「技术关注」。不升级，不下调。投资可操作性：仍不具备（无直接标的）。**

### 升级至「有条件通过」条件复核

| 条件 | R3 状态 | 判断 |
|------|---------|------|
| 1. AMI Labs 发布世界级研究成果 | 无成果发布，12 人团队无扩张信号 | **未触发** |
| 2. 非 Meta/AMI 第三方采纳 JEPA | 零采纳（Google/Apple/OpenAI/Anthropic 均无） | **未触发** |
| 3. Hyperscaler 削减 CapEx 指引 | 反向：Goldman 上调至 $1.1T（2027），进入债务融资阶段 | **远离触发** |

**结论**：3/3 条件均未触发，升级条件比 R2 更远。

### 下调至「观察」条件复核

| 条件 | R3 状态 | 判断 |
|------|---------|------|
| 1. 2027 年底 JEPA 仍无语言突破 | 跟踪中（当前无进展） | 未到期 |
| 2. AMI Labs Series A 困难/估值下调 | 无新融资动作（seed 后静默） | **半触发**（需持续观察） |
| 3. LLM 在物理推理/机器人突破 | V-JEPA 2 仍是机器人世界模型 SOTA；但 LLM 多模态整合加速 | 未触发 |

**结论**：下调条件未完全满足，但条件 #2 处于半触发状态（AMI Labs seed 后 4 个月无新动作）。

---

## 十一、验证窗口（下一轮关注）

| 时间 | 事件 | 关注点 |
|------|------|--------|
| 2026-07-28/29 | FOMC 会议 | 利率路径对 AMI Labs 估值/私募融资的影响 |
| 2026-08 上旬 | Hyperscaler Q2 财报 | Amazon/Google/Microsoft/Meta CapEx 实际执行 vs 指引；FCF 恶化程度；是否有削减信号 |
| 2026-09 | AMI Labs 成立 6 个月 | 首批研究成果？团队扩张？ |
| 2026 Q4 | NVIDIA Q3 FY27 | 数据中心营收增速；架构路线信号 |
| 2027 H1 | LeCun 预言窗口 | JEPA 是否有语言/机器人突破 |

---

## 十二、来源链接（按主题）

### AI CapEx / 债务融资
- [Tech AI spending approaches $700 billion in 2026, cash taking big hit](https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html) — CNBC, 2026-02
- [Oracle's AI spending blows past estimates, raising worries](https://www.reuters.com/technology/oracle-beats-fourth-quarter-revenue-estimates-2026-06-10/) — Reuters, 2026-06-10
- [Amazon Starts To Run Low On Cash](https://www.aol.com/articles/amazon-starts-run-low-cash-132648822.html) — AOL, 2026
- [The Price of AI: How Capex Is Rewriting Tech Balance Sheets](https://www.breckinridge.com/insights/the-price-of-ai-how-capex-is-rewriting-tech-balance-sheets) — Breckinridge, 2026
- [Bad News for NVIDIA, Amazon, and Microsoft: There's no longer enough cash for AI](https://247wallst.com/investing/2026/06/17/bad-news-for-nvidia-amazon-and-microsoft-theres-no-longer-enough-cash-for-ai/) — 247WallSt, 2026-06-17

### Goldman Sachs CapEx 预测
- [Tracking Trillions: The Assumptions Shaping the Scale of the AI Build-Out](https://www.goldmansachs.com/insights/articles/tracking-trillions-the-assumptions-shaping-scale-of-the-ai-build-out) — Goldman Sachs, 2026
- [Why AI Companies May Invest More than $500 Billion in 2026](https://www.goldmansachs.com/insights/articles/why-ai-companies-may-invest-more-than-500-billion-in-2026) — Goldman Sachs
- [AI: In a Bubble? (Report)](https://www.goldmansachs.com/pdfs/insights/goldman-sachs-research/ai-in-a-bubble/report.pdf) — Goldman Sachs Research
- [Goldman says the AI boom is bigger than investors think](https://www.businessinsider.com/stock-market-wall-street-tech-selloff-ai-token-goldman-sachs-2026-6) — Business Insider, 2026-06
- [As AI capital expenditures rise, so do the risks for AI stocks](https://www.morningstar.com/news/marketwatch/20260611131/) — MarketWatch/Morningstar, 2026-06

### 利率 / Fed
- [FRED DGS10 — 10-Year Treasury Constant Maturity Rate](https://fred.stlouisfed.org/series/DGS10) — FRED, 2026-07-08: 4.56%
- [FOMC Meeting Calendars](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm) — Federal Reserve, July 28-29, 2026
- [FOMC Statement June 17, 2026](https://www.federalreserve.gov/newsevents/pressreleases/monetary20260617a.htm) — Federal Reserve, rate maintained at 3.50-3.75%
- [J.P. Morgan Fed Rate Cuts Outlook](https://www.jpmorgan.com/insights/global-research/economy/fed-rate-cuts) — JPM, hold through 2026
- [iShares Fed Outlook 2026](https://www.ishares.com/us/insights/fed-outlook-2026-interest-rate-forecast) — iShares

### LLM 开源生态
- [China's DeepSeek V4 and Qwen Reshape the Open-Source AI Race](https://www.forbes.com/sites/jonmarkman/2026/04/28/chinas-deepseek-v4-and-qwen-reshape-the-open-source-ai-race/) — Forbes, 2026-04-28
- [DeepSeek V4 Shows That the Next AI Race Is About Efficiency](https://www.forbes.com/sites/geruiwang/2026/04/26/deepseek-v4-shows-that-the-next-ai-race-is-about-efficiency/) — Forbes, 2026-04-26
- [DeepSeek V4 vs US AI Models: The Cost and Capability Gap](https://www.mindstudio.ai/blog/deepseek-v4-vs-us-ai-models) — MindStudio
- [DeepSeek's Low Inference Cost Explained: MoE & Strategy](https://intuitionlabs.ai/articles/deepseek-inference-cost-explained) — IntuitionLabs, 50x cheaper
- [DeepSeek V4 unveils model with rock-bottom prices + Huawei chip support](https://fortune.com/2026/04/24/deepseek-v4-ai-model-price-performance-china-open-source/) — Fortune, 2026-04-24

### JEPA / 世界模型 / 机器人
- [Introducing the V-JEPA 2 world model](https://ai.meta.com/blog/v-jepa-2-world-model-benchmarks/) — Meta AI, 1.2B params
- [V-JEPA 2 paper (arXiv)](https://arxiv.org/html/2506.09985v1) — arXiv
- [1X World Model](https://www.1x.tech/discover/world-model-self-learning) — 1X, 900h egocentric video
- [ICML 2026 Accepted Papers](https://icml.cc/virtual/2026/papers.html) — Causal-JEPA accepted
- [LeCun MILA World Modeling Workshop Keynote](https://www.facebook.com/yann.lecun/photos/video-of-my-keynote-at-the-world-modeling-workshop-held-at-mila-on-2026-02-04/) — 2026-02-04

### AMI Labs
- [Yann LeCun's AMI Labs raises $1.03B](https://techcrunch.com/2026/03/09/yann-lecuns-ami-labs-raises-1-03-billion-to-build-world-models/) — TechCrunch, 2026-03-09
- [How Yann LeCun's Startup Challenges the Logic Behind Future AI](https://observer.com/2026/06/yann-lecun-startup-ami-labs-future-ai/) — Observer, 2026-06
- [AMI Labs Raises $1BN Seed Round](https://futurumgroup.com/insights/yann-lecuns-ami-raises-1bn-seed-round-is-the-world-model-era-finally-here/) — Futurum Group

### 中美脱钩
- [US says ban on AI chip shipments applies to Chinese firms outside China](https://www.aljazeera.com/economy/2026/6/1/us-says-ban-on-ai-chip-shipments-applies-to-chinese-firms-outside-china) — Al Jazeera, 2026-06-01
- [AI export controls are not the best bargaining chip](https://www.chathamhouse.org/2026/04/ai-export-controls-are-not-best-bargaining-chip) — Chatham House, 2026-04
- [Choking off China's Access to the Future of AI](https://www.csis.org/analysis/choking-chinas-access-future-ai) — CSIS

### 能源 / 电力
- [Clean Energy Resources to Meet Data Center Electricity Demand](https://www.energy.gov/oe/clean-energy-resources-meet-data-center-electricity-demand) — DOE/EPRI, 9% by 2030
- [Data centers drive 50% of US power demand](https://www.marketscale.com/industries/energy/data-centers-drove-half-of-us-electricity-demand-growth-as-time-to-power-becomes-the-defining-constraint-2d609d) — MarketScale
- [AI, Data Centers, and the U.S. Electric Grid](https://www.belfercenter.org/research-analysis/ai-data-centers-us-electric-grid) — Harvard Belfer Center

### NVIDIA / 市场定价
- [Nvidia Stock Weighs AI Momentum Against Mixed Valuation Signals](https://finance.yahoo.com/markets/stocks/articles/nvidia-nvda-stock-weighs-ai-100834813.html) — Yahoo Finance, 2026-06
- [NVIDIA GTC 2026 Keynote](https://www.nvidia.com/gtc/keynote/) — NVIDIA, Cosmos 3 / $1T demand
- [Custom Silicon AI Chip Market Share](https://intellectia.ai) — Intellectia.ai, 20.9%→27.8%
