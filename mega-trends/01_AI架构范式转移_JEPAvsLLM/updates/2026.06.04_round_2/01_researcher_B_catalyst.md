# 研究员B — 催化剂与学术信号

> 更新日期：2026-06-04 | 角色：催化剂研究员

---

## 核心发现 Top 3

### 发现 1：LLM Scaling Wall 信号持续累积 — 但"崩溃"尚未发生

**证据矩阵**：

| 信号 | 来源 | 强度 | 评估 |
|------|------|------|------|
| 前沿模型迭代速度加快 | GPT-5→5.4, Claude 4→Opus 4.6, Gemini 2.5→3.1 Pro | 强 | **反scaling wall** — 小版本迭代极快，每次都有实质提升 |
| MIT 论文：meek models 可追上顶级模型 | MIT IDE 2026.01 报告 | 中 | 顶级模型边际收益递减，低预算模型差距在缩小 |
| Gary Marcus 持续批评 | Substack 系列文章 | 弱 | 立场先行，非中立证据 |
| arXiv 论文：long-horizon 执行的"缩放定律幻觉" | arXiv 2509.09677 | 中 | 缩放定律在 test loss 上递减，但长程任务完成率仍有指数改善 |
| Platformer 报道：AI 公司撞墙 | The Platformer | 中 | OpenAI/Google 承认单纯参数缩放收益递减 |
| 推理 token 年增 10x | NVIDIA Q1 FY27 | 强 | **LLM 推理需求仍在爆发**，与 scaling wall 矛盾 |

**综合判断**：
- "Scaling Wall"更准确地说是**"参数缩放的边际收益递减"**，而非"LLM 到头了"
- 行业已转向**推理时计算**（Chain-of-Thought、test-time compute）来弥补参数缩放不足
- 这实际上意味着**对推理算力的需求可能更大**，而非更小
- **对 JEPA 的影响**：如果 LLM 通过推理时计算持续提升，JEPA 的紧迫性窗口可能进一步收窄

### 发现 2："Post-Transformer" 赛道拥挤化 — JEPA 并非唯一替代方案

**2026 年活跃的替代架构**：

| 架构 | 代表 | 进展 | 与 JEPA 的关系 |
|------|------|------|----------------|
| SSM/Mamba | Mamba-3B | 在语言建模上超越同规模 Transformer | 竞争关系 |
| Titans | Google Research | 长上下文处理新范式 | 竞争关系 |
| Diffusion LLM | 多个团队 | 用扩散模型做文本生成 | 竞争关系 |
| MoR (Mixture-of-Recursions) | 新兴 | 大幅降低推理成本 | 竞争关系 |
| JEPA | LeCun/AMI Labs | 视觉/物理推理领先 | 独立赛道 |
| Cantor/LFM | Computer IEEE 2026.01 | 轻量分形模型 | 竞争关系 |
| Recurrent Transformer | 多个团队 | 结合 RNN 和 Transformer | 混合方案 |

**关键洞察**：
- **JEPA 的真正独特性在于"世界模型"定位，而非"替代 Transformer"** — Mamba/Titans/Diffusion LLM 都是在语言/生成赛道上竞争，JEPA 占据的是物理世界理解这个独立生态位
- 但这也意味着 JEPA **不会直接取代 LLM**，而是与 LLM 互补
- **学术催化信号**：ICML 2026 接收论文中出现 "Building Social World Model with Large Language Models"，说明主流学界正在探索 LLM + World Model 的融合路径

### 发现 3：NVIDIA GTC 2026 — World Model 正式进入产业议程

**关键信号**：
- NVIDIA 将 World Models 列为 GTC 2026 核心主题
- NVIDIA 机器人研究总监 Jim Fan 公开表态："2026 年将标记 Large World Models 为机器人奠定真正基础的第一年"
- NVIDIA 发布 Cosmos Policy，将世界模型用于机器人策略训练
- NVIDIA 参投 AMI Labs $1.03B 轮次

**催化含义**：
- **NVIDIA 的两面性**：既全力推销 GPU 给 LLM 训练，又在 World Model 赛道布局对冲
- 这说明即使 GPU 霸主也认为 World Model 是值得押注的方向
- 但 NVIDIA 的 World Model 布局**不一定基于 JEPA** — 它可以是基于 Transformer 的世界模型

---

## 假设验证（H1-H5）

| 假设 | 验证状态 | 新证据 | 判断 |
|------|----------|--------|------|
| H1：JEPA 视觉/机器人主流 | 强化 | NVIDIA GTC 主题化、Cosmos Policy | 70% → **75%** |
| H2：JEPA 语言突破 | 无新进展 | 未发现新的 language-JEPA 论文 | 30% → **28%**（微降） |
| H3：算力需求降 10-100x | 未验证 | 无新证据 | 20% → **20%** |
| H4：LLM 生态壁垒 | 强化 | GPT-5.4/Claude Opus 4.6 持续快速迭代，推理时计算范式确立 | 75% → **78%** |
| H5：混合方案 | 强化 | LLM + World Model 论文出现，LeCun 采访确认 LLM 编排器角色 | 80% → **82%** |

---

## 学术催化时间线

| 时间 | 会议/事件 | 重要性 | 关注点 |
|------|----------|--------|--------|
| 2026.06 | ICML 2026 | 高 | JEPA/World Model 相关论文数量和质量 |
| 2026.09 | NeurIPS 2026 投稿截止 | 高 | 是否出现大规模 language-JEPA 论文 |
| 2026.12 | NeurIPS 2026 会议 | 极高 | JEPA 范式的学术接受度 |
| 2026 Q3-Q4 | AMI Labs 首批公开成果 | 极高 | 决定 $3.5B 估值是否合理 |
| 2027 H1 | ICLR 2027 | 高 | VL-JEPA 等后续工作 |

---

## LLM 瓶颈信号汇总

### 利于 JEPA 的信号
1. 参数缩放边际收益递减已被广泛承认（包括 OpenAI/Google）
2. LLM 无法真正理解物理世界，这在机器人/自动驾驶场景已是共识
3. 能耗问题日益突出 — 数据中心已占美国新增电力需求的 50%
4. 推理成本虽在下降但绝对量仍在膨胀

### 不利于 JEPA 的信号
1. 推理时计算（test-time compute）开辟了新缩放维度
2. GPT-5.4 / Claude Opus 4.6 在 coding benchmark 达到 80%+（SWE-bench）
3. 开源 LLM（DeepSeek V4, Qwen 3.5, Llama 4）性能逼近闭源
4. LLM + 工具/Agent 模式在商业场景持续扩大优势
5. LLM 正在"吸收"世界模型能力 — 多模态 LLM 已整合视觉/语音

---

## 情景分析

### 情景 A：学术催化成功 → JEPA 范式确立（概率 15%）
- AMI Labs 发布里程碑成果 + NeurIPS 2026 多篇 JEPA SOTA
- 触发条件：language-JEPA 在大规模预训练中达到 Llama-3 8B 水平

### 情景 B：渐进融合（概率 55%）
- LLM 吸收 World Model 能力，JEPA 论文影响 LLM 训练方法（类似 LLM-JEPA 路径）
- 无需"取代"，而是"融合"

### 情景 C：学术催化失败（概率 30%）
- 2027 年底 JEPA 仍无语言突破，AMI Labs 成果低于预期
- 学术社区转向其他替代架构（Mamba 等）

---

## 时间维度

| 时间 | 催化事件 | 潜在影响 |
|------|----------|----------|
| 2026.06-07 | ICML 2026 | 短期学术情绪 |
| 2026 Q3 | AMI Labs 首批论文 | 中期信号 — 验证 $3.5B 估值 |
| 2026 Q4 | Hyperscaler 实际 CapEx 执行 | 中期 — 若削减间接利好 JEPA |
| 2027 H1 | NeurIPS 2026 结果 + LeCun 预言窗口 | 关键判断点 |
| 2027 | AMI Labs Series A | 最强市场信号 |
