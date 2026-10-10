# 魔鬼辩护人报告

> 课题: #01 AI架构范式转移：JEPA vs LLM
> 分析日期: 2026-10-10 | 角色: devil's advocate（只基于背景包+独立检索，未读研究员报告）
> 任务：对当前论点（含潜在的多头叙事）做系统性证伪

---

## 一、本轮多头可能提出的叙事（预先拆解）

背景包显示多方可能的兴奋点：(1) AMI 论文流破冰（8-10 月 5+ 篇）；(2) Anthropic「减速共识」给替代路线开窗口；(3) benchmark 危机（SWE-bench 污染）削弱 LLM 的能力证据。以下逐一举证伪证据。

## 二、反方论据

**R1：「产出破冰」是幻象——arXiv 流水 ≠ main-track ≠ 工业价值。证据强度：强。**
- AD-E2E-JEPA（9/28）的结论是**自家阵营审计失败**：现有 JEPA 世界模型（LeWM/DINO-WM/JEPA-WM）在自动驾驶 goal-conditioned 规划上**全部不达标**。多头若把「论文数量」当进展，恰恰读反了最重要的那篇。
- LpWM/FAR/SIGReg 补丁/逆动力学保模态——全部是方法论小件，无一篇含机器人 SOTA 或 10B+ 规模证据。$1.03B 换来 7 个月「工具箱整理」，按 DeepMind/Sys 资本效率标准这是**负里程碑**。
- 来源：AMI Observatory 10 月周报；arXiv 2610.07540；TechCrunch 9/20（全行业保密化=无法验证）。

**R2：「减速共识」是空头陷阱——宣言发布 10 天内 Anthropic 自己发了 Opus 5.5（9/22），Google 官宣 Gemini 4 Argon，此前 9 天 GPT-6 Astra 上线。证据强度：强。**
- 「Pace the frontier」无任何执行机制（无暂停、无评估期延长、无发布间隔承诺）；Altman/Musk 口头支持≠行为改变。三家 9 月的发货节奏是四年来最密。
- 即便真减速：减速的是「发布」不是「训练」——算力继续被 Transformer 训练占用，JEPA 拿不到释放的算力（hyperscaler GPU 全部长约锁定）。
- LeCun 骂 Amodei「deluded」（10/1 Fortune）显示的是阵营营销战，不是路线转折。

**R3：benchmark 危机伤害 JEPA 更深。证据强度：中-强。**
- SWE-bench 污染（68.5% 失败源于坏测试用例）确实削弱 LLM 能力数字，但**JEPA 连被污染的资格都没有**——它从未在任何主流 benchmark 上有可争议的数字。测量层破产的结果是「公认战场消失」，对挑战者不利（incumbent 靠部署规模而非榜单取胜）。
- TheAgentCompany（真实办公任务）榜首仍是 DeepSeek V3.2（Transformer）。

**R4：T1 日落条款正在被「重新解释」以避免触发——方法论风险。证据强度：中。**
- R3 原文：「2027 Q1 无 main-track 论文→自动降级」。现在多头（预判）会说「论文已经有了」。但 NeurIPS 2026 main-track 名单未出，arXiv 不构成 main-track；若 CIO 接受 arXiv≈main-track，等于移动自己立的门柱——与 R3 维持评级时批评魔鬼「移动门柱」形成双标。
- **我的立场：T1 必须按原文字面执行到 2027 Q1，且应增设工业级条款（见下）**。

**R5：结构性边缘化的三重固化。证据强度：强。**
- 资本：JEPA 产业资金占比 0.14% 持平四个季度；world model 融资在涨但流向生成式/3D（World Labs $1.23B/Decart $4B）。
- 人才：AMI 在流入（Assran/Gu），但流入的是「world model 公司」而非「JEPA 教派」——公司 thesis 外扩=架构标签稀释。
- 生态：NVIDIA-HF $12.9B 把开源分发收编；DeepSeek V4.1-Flash 用 encoder-decoder（Transformer 家族内变异）解决效率——**JEPA 的差异化主张（效率+世界理解）两条都被 Transformer 内部演化覆盖**。

**R6：历史类比的补强（对 R3 魔鬼报告的延续）。证据强度：中。**
- 新类比：**BitTorrent vs IPv6**——技术上优越、行业共识认可、部署永不发生，因为 incumbent 的迁移成本锁定。JEPA 正在走 IPv6 路线（「重要但不被需要」）。
- 反面教训修正：上轮我方历史类比被指 outcome-based selection；本轮换用结构性类比（迁移成本锁定）而非结果类比。

## 三、最可能的失败模式（Top 3，针对「维持技术关注+继续监测」这一立场）

1. **「永久技术关注」陷阱（概念僵尸化）** — 触发：T1/T3 到期后 CIO 再次以「概念渗透仍在」为由维持评级 → 本课题变成永不结算的期权，监测资源被无限占用。概率：**45%**。
2. **反弹踏空（方向性错误）** — 触发：若 2027 CapEx 指引 <+$15%（升级条件 #3）+ AMI NeurIPS main-track 同季发生，JEPA 叙事急转弯而仓库仓位（GPU 逻辑）未重估。概率：**10%**。
3. **误把 AMI 公司风险当架构信号** — 触发：AMI Series A 估值下调（10Y 5.3% 环境下概率上升）被解读为 JEPA 失败，但实际是私募市场利率现象——过早降级丢失真实信号。概率：**20%**。

## 四、历史类比

- **IPv6**：技术优越性从未被否认，但 NAT 先行方案锁定部署路径 25 年。JEPA 的 latent prediction≈IPv6 的地址空间——正确但迟到的解决方案。「正确但迟到」在投资上等于错误。
- **Async/await vs 线程库**：编程范式更替只在「新语言运行时」（新平台）发生，从不通过「改写现有系统」。JEPA 若成功，载体将是新平台（机器人 native 栈），而非替换 LLM。

## 五、对退场标准的补充

- **建议新增 T5（工业级验证条款）**：AMI 或任何第三方在 2027 Q3 前未在公开工业级基准（自动驾驶规划/机器人操作长序列）上展示 JEPA 类架构优于生成式基线 ≥20% → 情景 C 概率直接上调至 45% 并冻结 H1 上调权限。
- **建议新增 T6（概念僵尸检测）**：若 2027 Q1 裁定时「world model」一词在融资材料中的出现率继续上升而 JEPA 采纳仍为 0，则确认「标签与架构脱钩」完成——课题应转归 #11 机器人课题处理，本课题降级「观察」。
- **重申**：T1 按 R3 原文执行（main-track=NeurIPS/ICML/ICLR/CVPR 主会，arXiv 不算）。

## 六、结论

R3 的全部利空事实在本轮**无一反转**：第三方采纳仍为 0、V-JEPA 3 缺席、CapEx 反向加码、LLM 迭代加速（GPT-6 Astra 提前触发 R2 阈值）。新增的「多头叙事」（产出破冰/减速共识/benchmark 危机）经查证全部为幻象或双刃剑。情景 C 应上修至 36-40%。评级可以维持「技术关注」（我接受 R3 关于监测价值的论证），但 **T1/T3 到期执行必须写死，不允许再次展期**。

---

## 关键来源

- AMI Observatory（French Tech Journal）10 月：AD-E2E-JEPA 结论、Balestriero 批评、FAR、招聘流
- arXiv 2610.07540（Toso/LeCun，AMI Labs 挂靠）
- TechCrunch（9/20）：World model companies are keeping a lot of secrets
- Anthropic：We Must Pace the Frontier（9/12）；Opus 5.5（9/22）；Gemini 4 Argon 官宣（9 月）；GPT-6 Astra（9/3）
- Vals AI / BenchLM / BenchLeader（benchmark 水位与污染）
- Fortune（10/1）：LeCun 专访；Fortune（9/4）：NVIDIA-HF
- CreditSights（10 月）：~$750B；FOMC 9/16 声明+Warsh 发布会
