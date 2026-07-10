# 研究员A — 基本面分析

> 更新日期：2026-06-04 | 角色：基本面研究员

---

## 核心发现 Top 3

### 发现 1：AMI Labs 完成 $1.03B 种子轮 — 资本开始用脚投票

**事实**：
- 2026 年 3 月，AMI Labs 宣布完成 $1.03B 种子轮融资，$3.5B pre-money 估值
- 这是**欧洲史上最大种子轮**，公司仅约 12 名员工，无产品
- 联合领投：Cathay Innovation, Greycroft, Hiro Capital, HV Capital, Bezos Expeditions
- 战略投资者：**NVIDIA**, Temasek, Samsung, Toyota Ventures, Bpifrance
- 个人投资者：Jeff Bezos, Mark Cuban, Eric Schmidt, Tim Berners-Lee
- 团队：LeCun（执行主席）、Alexandre LeBrun（CEO，前 Meta FAIR 巴黎负责人、Nabla 创始人）、Saining Xie（CSO，前 Google DeepMind）、Pascale Fung（首席研究与创新官）、Mike Rabbat（VP World Models）
- 办公室：巴黎、纽约、蒙特利尔、新加坡

**投资含义**：
- NVIDIA 参投极为关键 — 说明 GPU 霸主也在对冲 JEPA 路线
- Toyota Ventures 参投指向机器人/自动驾驶应用
- Samsung 参投指向端侧 AI 部署
- 这不是纯学术项目，是有明确商业化路线的独立公司

**投资可操作性**：
- AMI Labs 未上市，一级市场标的
- 后续可关注：若 AMI Labs 在 Series A 前发布研究成果，可能触发相关标的（边缘芯片、机器人）重估

### 发现 2：World Model 概念已破圈 — 从学术概念变为行业主题

**事实**：
- NVIDIA GTC 2026 将 World Models 列为核心主题之一
- Fei-Fei Li 的 World Labs 已融资超过 $1B
- General Intuition 完成 $133.7M 种子轮
- Packy McCormick（Not Boring）发表万字深度文章，将 World Models 与 LLM 并列为两条 AGI 路径
- NVIDIA 机器人研究总监 Jim Fan："2026 年将标记 Large World Models 为机器人奠定真正基础的第一年"
- **Wall Street Journal 称 2026 年为"后 Transformer 之年"**

**投资含义**：
- "World Model"已从小众学术概念变为投资圈热门话题
- AMI Labs CEO Alexandre LeBrun 预测："六个月内，每家公司都会自称 World Model 公司来融资"
- 这意味着信号噪音比正在下降 — 需要更严格区分真正的 JEPA 架构与蹭概念的项目

### 发现 3：JEPA 研究生态正在扩展 — 不再是 LeCun 一人的游戏

**事实**：
- **学术产出加速**：
  - JEPA 综述论文（TechRxiv）已发布，涵盖图像、音频、视频、点云等多模态实现
  - LeJEPA 将 JEPA 训练简化为单超参数，核心代码 ~50 行，大幅降低实验门槛
  - LeWorldModel 仅 15M 参数，单 GPU 几小时训练，规划速度比传统方法快 48x
- **ICML 2026 投稿量达 30,000+**，其中 World Model 相关 Workshop 显著增加
- **"Post-Transformer"研究线正在形成**：Mamba（SSM）、Titans、Diffusion LLM、MoR（Mixture-of-Recursions）等替代架构获得更多关注
- **AMI Labs 已从 OpenAI、Google DeepMind、xAI 招聘研究人员**

**投资含义**：
- JEPA 的研究不再依赖 LeCun 个人品牌
- 简化版本（LeJEPA/LeWorldModel）降低了学术社区的参与门槛
- 但"Post-Transformer"赛道拥挤，JEPA 只是众多替代方案之一，并非独占

---

## 假设验证（H1-H5）

| 假设 | 验证状态 | 新证据 | 判断 |
|------|----------|--------|------|
| H1：JEPA 成为视觉/机器人主流 | 强化 | GTC 主题化、AMI Labs $1B+、World Labs $1B+ | 70% → **75%** |
| H2：JEPA 语言突破 | 微弱进展 | 无新论文，LLM-JEPA 仍是唯一证据 | 30% → **30%**（维持） |
| H3：算力需求降 10-100x | 未验证 | 无新生产级验证 | 20% → **20%**（维持） |
| H4：LLM 生态壁垒阻止 JEPA | 强化 | GPT-5.4/Opus 4.6/Gemini 3.1 持续快速迭代 | 75% → **78%** |
| H5：混合方案成主流 | 维持 | LeCun 本人在采访中承认 LLM "编排器"角色 | 80% → **80%**（维持） |

---

## 标的梳理

### 直接标的（JEPA/Worl d Model 概念）
| 标的 | 类型 | 阶段 | 关联度 | 备注 |
|------|------|------|--------|------|
| AMI Labs | 一级 | Seed | 核心 | 未上市，$3.5B 估值 |
| World Labs (Fei-Fei Li) | 一级 | Seed | 高 | 非 JEPA 但同赛道 |
| General Intuition | 一级 | Seed | 高 | 非纯 JEPA |

### 二级市场受益标的
| 标的 | 逻辑 | 当前状态 |
|------|------|----------|
| NVIDIA | GPU 霸主 + 参投 AMI Labs | 两面性：短期受益于 LLM CapEx，长期需应对架构变化 |
| 高通/联发科 | 边缘 AI 芯片受益于轻量模型 | JEPA 若成功直接利好 |
| 特斯拉 | Optimus 机器人 + FSD | V-JEPA 类世界模型赋能 |
| 寒武纪 | NPU/ASIC 设计 | JEPA 推理更轻量，NPU 性价比优势放大 |

### 受损标的（若 JEPA 成功）
| 标的 | 逻辑 | 时间维度 |
|------|------|----------|
| SK 海力士/美光 | HBM 需求可能结构性下降 | 3-5 年 |
| Equinix/Digital Realty | 数据中心可能过剩 | 3-5 年 |
| Arista Networks | 高速互联需求下降 | 3-5 年 |

---

## 情景分析

### 情景 A：JEPA 独立成功（概率 15%）
- AMI Labs 发布世界级成果 → 主流公司采纳 JEPA → GPU 需求结构性下降
- 投资动作：增持边缘芯片/机器人，减持 HBM/高端 DC REIT
- 时间线：2028-2030

### 情景 B：JEPA + LLM 混合主流（概率 55%）
- JEPA 负责世界模型/视觉推理，LLM 负责语言编排
- 投资动作：同时持有 NVIDIA + 边缘芯片，关注混合架构工具链公司
- 时间线：2027-2029 逐步融合

### 情景 C：LLM 继续统治，JEPA 沦为学术项目（概率 30%）
- JEPA 未能在语言生成取得突破，产业资本继续全力投入 Transformer
- 投资动作：维持当前 AI 基础设施投资逻辑不变
- 时间线：2027 年底确认

---

## 时间维度

| 时间 | 预期事件 | 对判断的影响 |
|------|----------|-------------|
| 2026 Q3-Q4 | AMI Labs 首批研究发布 | 若成果显著，H1 信心上调 |
| 2026 Q3 | ICML/NeurIPS 2026 论文 | 关注 JEPA 相关论文数量和质量 |
| 2026 Q4 | Hyperscaler CapEx 实际执行 | 若削减指引，间接利好 JEPA 叙事 |
| 2027 H1 | LeCun 预言验证窗口 | 产业是否"认识范式转移" |
| 2027 | AMI Labs Series A | 估值和进展将是最强市场信号 |
