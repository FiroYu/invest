# 课题 #01 AI架构范式转移：JEPA vs LLM — Round 4 背景包

> 构建日期：2026-10-10（目录沿用 Round 4 批次命名 2026.09.03，实际信息截止 2026-10-10）| 构建者：CIO (orchestrator)
> 捕获窗口：2026.07.10 → 2026.10.10（约 13 周，Round 4 增量最长窗口）
> 基线：Round 3 CIO 综合（2026-07-10）

## 一、历史摘要

- **辩论评级**：技术关注（R1→R4 连续维持）+ R3 新增 12 个月日落条款。非可投资课题（无直接标的），价值=架构路线判断→间接标的（GPU/HBM vs 边缘/机器人）长期逻辑校准。
- **R3 头号裁定**：JEPA「思想胜利、架构失败」悖论——world model 概念破圈（H1 2026 VC >$3B）但 JEPA 作为具体架构被 Google/OpenAI/NVIDIA/Apple 全部绕开（第三方采纳=0），AMI Labs 拿 $1.03B 后 4 个月零 main-track 产出（LeJEPA 证明经查证属 Meta 时期工作）。
- **H1-H5（R3 信心度）**：H1 视觉/机器人主流 65%（↓7pp）/ H2 语言突破 20%（↓5pp）/ H3 算力降 10-100x 14%（↓3pp）/ H4 LLM 生态壁垒 86%（↑6pp，最强化）/ H5 混合主流 78%（↓2pp）。
- **情景（R3）**：A JEPA 独立成功 7% / B 融合（modal）45% / C LLM 吸收 JEPA 32%（↑7pp）/ D 完全失败 16%。C+D=48%（未过半）。
- **R3 收紧触发**：T1 日落条款（AMI seed 后 12 个月即 2027 Q1 无 main-track → 自动降级「观察」）/ T2 V-JEPA 3 不在 2026 H2 发布 → H1 再降 5pp / T3 第三方采纳 2027 Q1 仍为 0 → 降级讨论 / T4 AMI 团队流失至 Hyperscaler → 情景 C 上修 40%+。
- **R3 关键事实纠正**：ICML 2026 首尔 COEX；AMI $3.5B pre-money；LeJEPA 证明属 Meta 时期；AMI CEO=Alexandre LeBrun（LeCun 任 Executive Chairman）。
- **R3 操作结论**：不基于 JEPA 调整任何 GPU/HBM/芯片仓位（$725B CapEx 债务融资锁定 Transformer 栈 3-5 年）；机器人配置基于产业进展而非 JEPA 假设。

## 二、横向风险因子（敏感度）

- **因子1 AI CapEx**：**极高敏感（本课题核心变量）**。R3 时点 2026 CapEx $725B；R4 窗口内 CreditSights ~$750B（+67% YoY，连续三年 >60%），四大现金口径 ~$733B（#17 R4 已裁定）。10 月底 Q3 财报=2027 指引首批窗口。
- **因子2 利率**：**高敏感**。R3 时点 10Y 4.56% → 本轮 **5.30%**（10/5 盘中 5.349%，2002 年来最高）；FOMC 9/16 加息 25bp 至 3.75-4.00%（12-0 票），点阵图年底再加息一次至 4.00-4.25%。高贴现率压制 AMI Labs 等长周期研究型公司估值。
- **因子3 中美脱钩**：中敏感（AMI 定位「非美非中第三极」，Paris/NY/Montreal/Singapore 四办公室）。
- **因子4 私募流动性**：中敏感（world model 融资仍在：Q1'24-Q2'26 累计 41 笔 >$9.5B；但加密/投机板块收紧）。

## 三、关联课题

- **#17 推理芯片**：强耦合·共同生死门。R4 已裁定 K5/K12 双触发（CoreWeave CDS ~855bp）、NVDA 20-25%、2027 指引为终审。本课题升级条件 #3（Hyperscaler 削减 CapEx）跟随 #17 的 K16（2027 指引锚）。
- **#11 机器人/具身智能**：正向但去 JEPA 化（R3 裁定）。机器人世界模型路线全选非 JEPA。
- **#04/#21 CapEx 共同变量**：极强·架构锁定（债务融资阶段）。
- **#06 量子**：共同利率敞口（10Y 5.3% 压制长周期技术资产）。

## 四、假设清单（本轮需重验）

| # | 假设 | R3 状态 | 本轮验证焦点 |
|---|------|--------|------------|
| H1 | JEPA 成为视觉/机器人主流架构 | 65%（↓7pp） | AMI 产出破冰后的实质内容（论文/基准结论）；V-JEPA 3 是否发布（T2，H2 剩 ~11 周）；第三方机器人公司路线 |
| H2 | JEPA 在语言任务上突破 | 20%（↓5pp） | GPT-6 Astra/Gemini 4/Opus 5.5 后语言前沿与 JEPA 的差距；AMI 是否有任何语言侧动作 |
| H3 | 算力需求降 10-100x | 14%（↓3pp） | DeepSeek V4.1-Flash 效率架构；CapEx 上行（$733-750B）；Jevons paradox |
| H4 | LLM 生态壁垒阻止 JEPA 取代 | 86%（↑6pp） | NVIDIA 收购 Hugging Face（$12.9B）对开源生态的整合；SWE-bench 96.2%；Anthropic「pace the frontier」减速共识是否构成 H4 首次裂缝信号 |
| H5 | 混合方案成主流 | 78% | 前沿模型多模态/世界模型能力（Gemini 4 Argon 1M 输出）；JEPA 组件化渗透（FAR 记忆框架/VLA-JEPA） |

## 五、退场标准与收紧触发（R3 后状态）

| # | 定义 | R3 状态 | 本轮必查 |
|---|------|---------|---------|
| T1 | AMI Labs 2027 Q1 无 main-track 论文 → 自动降级「观察」 | 4/12 个月，零 main-track | **AMI 挂靠论文是否出现？是否构成 main-track？NeurIPS 2026（12/6-12 悉尼）提交/接收状态** |
| T2 | V-JEPA 3 不在 2026 H2 发布 → H1 再降 5pp | 未发布 | V-JEPA 2.1（3/16）后 Meta 线是否静默至今 |
| T3 | 第三方 JEPA 采纳 2027 Q1 仍为 0 → 降级讨论 | = 0 | GPT-6 Astra / Gemini 4 Argon / Opus 5.5 / Cosmos 后续的架构选择 |
| T4 | AMI 团队流失至 Hyperscaler → 情景 C 上修 40%+ | 无流失 | AMI 招聘方向（流入 vs 流出） |
| K1 | Transformer 生态系统性失败（CapEx 崩塌 >30%） | 远未触发 | 跟随 #17 K12-K16 |
| K5 | LLM 在物理推理/机器人明确超 JEPA 突破 | 部分信号 | computer-use 旗舰（GPT-6 Astra）与机器人基础模型进展 |

## 六、Delta 疑问清单（本轮必须回答）

| # | 问题 | 对应节点 |
|---|------|---------|
| D1 | OpenAI 下一代模型实际名称/时点/能力？R2 阈值「GPT-6 若 Q4 发布 = LLM 加速」是否触发？ | H4/升级条件 |
| D2 | SWE-bench 等前沿 benchmark 最新水位？85% 阈值是否突破？benchmark 自身是否出现测量危机？ | H4 |
| D3 | Anthropic「pace the frontier」宣言内容与行业响应——LLM 阵营是否首次出现自愿减速共识？对 JEPA 窗口含义？ | H4/新变量 |
| D4 | AMI Labs 产出状态：8-10 月论文流（LpWM/AD-E2E-JEPA/arXiv 2610.07540/Balestriero/FAR）是否含 main-track？内容定性（突破 vs 审计）？T1 是否仍处倒计时？ | T1 |
| D5 | V-JEPA 3 发布了吗？Meta AI 视频线动态？ | T2/H1 |
| D6 | 第三方 JEPA 采纳仍为 0？前沿四家（OpenAI/Google/Anthropic/NVIDIA）新发布架构路线？ | T3/H1 |
| D7 | AMI 团队流动：新 hires（Assran/Gu/Fung 等）与流失；办公室扩张？ | T4 |
| D8 | World model 赛道融资增量（General Intuition 等）？JEPA 占比？标签通胀是否恶化？ | H1 |
| D9 | Hyperscaler CapEx 最新口径与融资结构（债务占比/FCF）？10 月底 Q3 财报窗口预判？ | 升级条件 #3/K1 |
| D10 | NVIDIA-Hugging Face 收购对开源 Transformer 生态锁定的含义？ | H4 |
| D11 | FOMC 9/16 实际决议与 10Y 走势？对 AMI 类长周期资产估值影响？ | 宏观 |
| D12 | Gemini 4 Argon / DeepSeek V4.1-Flash 等对手迭代节奏与效率叙事？ | H3/H4 |

## 七、研究分工提示

- 研究员 A（基本面）：D4/D5/D7/D8（AMI 产出/招聘/融资/学术生态）+ 间接标的逻辑（NVDA-HF）
- 研究员 B（催化剂）：D1/D2/D3/D6/D12（LLM 前沿竞速+benchmark+减速共识）
- 研究员 C（宏观）：D9/D10/D11（CapEx/利率/生态并购整合）
- 魔鬼辩护人：对「产出破冰=趋势反转」与「减速共识=JEPA 窗口」两个潜在多头叙事做证伪
