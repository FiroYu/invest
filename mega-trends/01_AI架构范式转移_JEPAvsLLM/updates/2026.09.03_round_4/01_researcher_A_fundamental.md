# 基本面研究员（研究员A）独立研究报告

> 课题: #01 AI架构范式转移：JEPA vs LLM
> 分析日期: 2026-10-10 | 角色: fundamental（架构生态、学术产出、产业资本、间接标的）
> 捕获窗口: 2026-07-10 → 2026-10-10；搜索源: WebSearch + AMI Labs Observatory（French Tech Journal）+ arXiv

---

## 一、核心发现（Top 3）

1. **AMI Labs 产出破冰——从零到论文流，但全部是「审计与补件」而非「突破」。** 8/29 LpWM（稀疏表征，arXiv，AMI 团队署名含 Kuang/Midlarsky 等）、9/28 AD-E2E-JEPA（自动驾驶 JEPA 世界模型 benchmark：**结论是现有 JEPA 世界模型全部不达标准**）、10/1 Balestriero 公开指出竞品 LeWM 的 temporal collapse 缺陷并指向 AMI 自家 SIGReg 修复、10 月 arXiv 2610.07540（Toso/LeCun/Bounou，LeCun 挂靠 NYU+AMI Labs）、FAR 记忆框架（Amir Bar，10/1）。**定性判断**：T1 日落条款的「无 main-track 发表」字面条件正在被解除（arXiv+署名挂靠持续流出），但内容无一属于「机器人规划大幅超 SOTA」的升级条件 #1 类型；AD-E2E-JEPA 是对自家阵营的诚实揭短——**工业级任务（自动驾驶端到端）上 JEPA 现状=不及格**。

2. **学术-工业身份重构：JEPA 正在变成「AMI 及朋友圈的内部标准」而非行业路线。** LeCun 的署名机构已从 Meta FAIR/NYU 切换为 NYU+AMI Labs；Kempe（NYU）牵头 World Modeling for Physics Workshop（Aspen，申请截止 10/15）；新 hires 持续流入（Mahmoud Assran——V-JEPA 论文一作级别人物、Jiatao Gu、VP Finance Giraut-Pierron、Pascale Fung 加入）。团队在扩张（T4 反向：无流失、在流入），但产出以「 JEPA 内部方法论补丁」（LpWM 稀疏表征/FAR 记忆/SIGReg 修复/逆动力学保不稳定模态）为主——这是把架构从「概念」往「可用工具箱」推进的工程，不是向 LLM 阵营的进攻。

3. **World model 赛道资本继续膨胀但 JEPA 份额仍边缘。** Q1'24-Q2'26 累计 41 笔披露融资 >$9.5B（newmarketpitch 汇总）；9/29 General Intuition $220M；World Labs 累计 ~$1.23B、Decart 近 $4B（NVIDIA 参投）、Odyssey $1.45B。9/20 TechCrunch「World model companies are keeping a lot of secrets」确认全行业保密化。**JEPA 显性资金仍≈AMI $1.03B 一家**，在 world model 总盘占比随分母膨胀继续稀释——「概念胜利、架构边缘」的 R3 结构未变。

---

## 二、逐项分析

### D4：AMI 产出定性（T1 条款）

| 项 | 日期 | 性质 | 判定 |
|----|------|------|------|
| LpWM（稀疏表征） | 8/29 | 方法论补丁 | arXiv+AMI 署名，非 NeurIPS/ICML main track |
| AD-E2E-JEPA | 9/28 | 自家阵营审计（负面结论） | benchmark 类；**现有 JEPA 世界模型在端到端自动驾驶 goal-conditioned planning 上不达标** |
| Balestriero LeWM 批评 | 10/1 | 学术权威卡位 | 指出竞品 temporal collapse，指向 AMI 修复 |
| arXiv 2610.07540 | 10 月 | 机器人 JEPA 世界模型（逆动力学保不稳定模态） | LeCun 挂靠 **AMI Labs**——机构归属首次明确 |
| FAR 记忆框架 | 10/1 | 架构扩展（借鉴 RAG） | 把「记忆/检索」引入世界模型栈 |
| SCOPE / PDE-OBS | 10 月 | 物理场恢复 | LeCun 共同署名，与 Kempe 物理工坊呼应 |

**T1 判定**：按 R3 字面（「无 main-track 论文发表」）——arXiv 流≠main-track（NeurIPS/ICML/CVPR 主会）。NeurIPS 2026 12/6-12 悉尼，接收结果若在 11-12 月披露且 AMI 有 main-track 论文，T1 提前解除；否则 T1 倒计时继续（2027 Q1 到期）。**我的建议：T1 应在本轮改写为「2027 Q1 前无工业级 benchmark（自动驾驶/机器人操作）上超 SOTA 的 main-track 论文」**——因为单纯 arXiv 流水不能证明 $1.03B 的转化。

### D5：V-JEPA 3（T2）——未发布，Meta 线近乎静默

V-JEPA 2.1（3/16，ViT-g/G 1B/2B + 蒸馏 ViT-B/L）后，截至 10/10 **无 V-JEPA 3 发布**。GitHub facebookresearch/vjepa2 更新停在 2.1；Meta AI 视频线无新旗舰。T2 条款（「不在 2026 H2 发布→H1 再降 5pp」）**剩余窗口仅 ~11 周**，从节奏（V-JEPA 2025-06→2.1 2026-03）推断发布概率 <40%。**V-JEPA 系列疑似进入维护模式**——Meta 在 LeCun 离开后没有 JEPA 旗舰接力，这是比 AMI 静默更深的结构性信号：JEPA 的「母港」正在撤资。

### D7：AMI 团队流动（T4）

流入：Mahmoud Assran（V-JEPA/I-JEPA 作者群核心，Montreal）、Jiatao Gu（NY）、Chloe Giraut-Pierron（VP Finance，Paris）、Pascale Fung（研究领导层）。无公开流失。**T4 未触发且反向**——学术明星持续流入，机构健康度高于 R3 判断。但注意：招聘方向（Gu 的 agent 研究/FAR 记忆）显示 AMI 在把 thesis 从「JEPA 架构」外扩为「物理世界 agent 全栈」——**公司正在变成「world model 公司」而非「JEPA 公司」**。

### D8：赛道资金与标签通胀

- General Intuition $220M（9/29）加入 world model 盘子；Dexterity「Foresight」工业世界模型上产线。
- 标签通胀印证：LeBrun 3 月预言「六个月内每家公司都自称 world model」在 10 月已成为行业默认——区分度进一步丧失。
- **JEPA 产业资金占比**：$1.03B / (2026 CapEx ~$733-750B) ≈ **0.14%**（持平 R3）；在 world model VC 盘子（H1 >$3B + Q3 增量）中占比 **≤8-10%（继续稀释）**。

### 间接标的逻辑更新（D10 部分）

- **NVIDIA 收购 Hugging Face（$12.9B，9/3 官宣）**：开源 Transformer 生态的最大分发平台被 GPU 最大的既得利益者收编。对 JEPA 的含义：若未来开发者要尝试 JEPA 类架构，其模型分发/工具链将处于 NVIDIA 控制之下——**生态壁垒从「资金+工具」升级为「资本结构级」**。NVIDIA 同时是 AMI 战略投资者（兼裁判与运动员，但对 JEPA 的直接 GPU 需求拉动仍≈0——LpWM 等在单卡/小集群可复现）。
- **机器人（#11 耦合）**：Dexterity Foresight、1X、Figure 路线未变（生成式/VLA），JEPA 仍非主流底座。

---

## 三、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|------|------|------|:-----------:|
| H1 视觉/机器人主流 | **方向不变（边缘化）+ 新增实证反证** | AD-E2E-JEPA：现有 JEPA 世界模型在工业级任务不达标（自家审计）；V-JEPA 3 缺席；机器人公司路线全非 JEPA。产出破冰≠工业验证 | 4 |
| H2 语言突破 | 不成立（维持） | 零语言侧动作；前沿语言模型距 JEPA 更远（见 B 报告） | 5 |
| H3 算力降 10-100x | 不成立（维持） | LpWM/FAR 均为效率补丁但无数量级证据；CapEx 全周期 $5.3T 继续膨胀 | 4 |
| H4 LLM 生态壁垒 | 成立（强化，待 C 交叉） | NVIDIA-HF 收购把开源分发平台资本化；SWE-bench 96.2%（见 B）；但 Anthropic 减速宣言是首次裂缝信号（待裁定） | 4 |
| H5 混合主流 | 成立（微升） | FAR「借鉴 RAG 的记忆框架」= JEPA 阵营主动向 LLM 工具箱借力；Gemini 4 Argon 1M 输出多模态深化 | 3 |

## 四、情景分析

| 情景 | 概率 | 核心驱动 | 预期影响（对架构格局） |
|------|:----:|---------|---------|
| Bull（JEPA 路线复兴） | 5% | NeurIPS 2026 main-track + 工业级 SOTA + V-JEPA 3 年内发布 | H1 回升至 70%+，评级讨论升级 |
| Base（工程化渗透） | 55% | AMI 论文流持续但无 SOTA；JEPA 组件化进 world model 工具箱 | 维持「技术关注」，B 情景（融合）主导 |
| Bear（架构边缘化定型） | 40% | T2 触发+T3 维持零+NeurIPS 无 main-track | 2027 Q1 T1/T3 双降级讨论 |

## 五、时间维度

- **短期（1-3 月）**：NeurIPS 2026（12/6-12 悉尼）main-track 名单= T1 提前裁决点；V-JEPA 3 是否年底发布=T2 终裁。
- **中期（3-12 月）**：AMI Labs seed 后 12 个月（2027 Q1）T1/T3 到期；首轮 demo/产品传闻窗口；2027 CapEx 指引（#17 K16）。
- **长期（1-3 年）**：world model 商业化（医疗 Nabla 伙伴/机器人）能否给出 JEPA 优势的收入证据。

## 六、关键来源

- AMI Labs Observatory（French Tech Journal）10 月周报：AD-E2E-JEPA（9/28）、Balestriero LeWM 批评（10/1）、FAR（10/1）、Assran/Gu 招聘、LeCun-Fortune 专访（10/1「Amodei deluded」）
- arXiv 2610.07540（Preserving Unstable Modes Through Inverse Dynamics in JEPA World Models；Toso/LeCun(AMI Labs)/Anderson/Bounou）
- AMI Observatory 新闻页：LpWM（arXiv 8/29）；World Modeling for Physics Workshop（Aspen，截止 10/15）
- newmarketpitch：41 笔 world model 融资（Q1'24-Q2'26）>$9.5B；SiliconANGLE：General Intuition $220M（9/29）
- TechCrunch：World model companies are keeping a lot of secrets（9/20）
- GitHub facebookresearch/vjepa2（最后更新 V-JEPA 2.1，2026-03-16）
- Fortune：NVIDIA acquires Hugging Face $12.9B（9/4）；WSGR 客户公告（9/3）
- NeurIPS 2026 官网（Sydney 主会 12/6-12）

---

*本报告为独立研究，未参考其他研究员结论。*
