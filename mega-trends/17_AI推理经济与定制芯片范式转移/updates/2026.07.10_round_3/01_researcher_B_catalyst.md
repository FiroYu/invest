# 议题#17 Round 3 研究员B（催化剂）报告

> 捕获窗口：2026.06.05 → 07.10（约5周）
> 报告日期：2026.07.10
> 角色：催化剂研究员B（产品/路线图/技术里程碑/合同/产能/定价/能源/地缘）
> 基线：Round 2 综合（2026.06.04）— 核心通过、ASIC 占比27.8%、NVDA Forward PE 25.5x

---

## 1. 执行摘要

### 方向投票：通过（置信度 高，较 Round 2 略升）

Round 3 窗口内（06.05→07.10）出现 **9 个方向性催化剂**，其中 6 个利好核心论点、3 个利空。核心范式转移逻辑（训练→推理、GPU→ASIC、CoWoS 瓶颈）在 5 周内获得 **超预期强化**，但同步浮现两个新的风险因子：**Rubin Ultra 封装受限致 2027 算力减半** 与 **API 定价战信号（OpenAI 考虑大幅降价）**。

**最关键的三个新催化剂**：
1. **Rubin Ultra 四芯版取消（06.30 SemiAnalysis / 07.01）** — CoWoS-L 基板翘曲迫使改为双两芯，2027 名义算力减半。这是 Round 2 "CoWoS 2027H2 可能缓解"判断的反向修正：**封装物理极限开始实质性限制 NVIDIA 路线图斜率**，同时保护 ASIC 阵营（ASPU 设计受 CoWoS-L 翘曲影响小于四芯 GPU）。
2. **Hyperscaler 自研 ASIC 合同集中落地（04-06月，Round 2 后续确认）** — OpenAI-Broadcom 10GW（"Nexus"项目 $18B）+ Meta-Broadcom 1GW 起步/多-GW 至 2029（首个 2nm AI 芯片）+ Anthropic 3.5GW Google/Broadcom TPU + Google LTA 至 2031。**Broadcom AI SAM 已从 Round 2 的 $60-90B FY27 进一步上修**，Hock Tan 公开目标 ">$100B AI 收入 2027"。
3. **API 定价战信号浮现（06.11 WSJ）** — OpenAI 正"考虑大幅降价"对抗 Anthropic；Google Plus 月费 $7.99→$4.99。**这是 K5 退场标准的早期预警**（虽未触发：需任两家同一季度降>50%）。推理商品化压垮定价权的"通缩陷阱"场景（Round 2 概率 15-20%）正在从 2028+ 提前到 2026H2 的可见窗口。

### 加权回报 vs Round 2

| 标的 | Round 2 加权回报 | Round 3 修正 | 变化 | 关键驱动 |
|------|----------------|-------------|------|---------|
| **NVDA** | +10.0% | **+11.5%** | 上修 | $91B Q2 指引（零中国假设）+ Rubin 量产 Q3 + Forward PE 27x（仍板块最低）；Rubin Ultra 延迟部分抵消 |
| **AVGO** | +8.25% | **+11.0%** | 上修（最大） | OpenAI 10GW + Meta 多-GW + Google LTA + Hock Tan >$100B 目标；客户基础从 6 确认客户扩至 8+ |
| **GOOGL** | +9.75% | **+10.5%** | 轻微上修 | Ironwood GA + TPU 8t/8i 2027末路线图 + Anthropic 锚客户 + 搜索现金流保护 |
| **MRVL** | +0.75% | **+1.0%** | 基本持平 | 窗口内无重大新催化剂，仍投机级 |

**研究员B的核心判断**：Round 3 是 "ASIC 范式转移从方向性判断变为已签约订单储备" 的确认窗口。Broadcom 的合同可见度已使其从"主题标的"转变为"订单可量化标的"。NVIDIA 的 Rubin Ultra 受挫恰恰反讽地 **强化** 了范式转移逻辑——因为封装物理极限对通用 GPU（大芯片、多芯堆叠）的惩罚比对 ASIC（小芯片、单芯为主）更严重。建议在 CIO 综合中 **上修 AVGO 仓位权重、维持 NVDA 核心、将 GOOGL 作为风险收益比首选**。

---

## 2. 假设验证表（H1-H5 + 子论点）

| 假设 | Round 2 裁定 | Round 3 新证据 | 研究员B建议修订 |
|------|-------------|--------------|----------------|
| **H1** ASIC 推理份额 2028 增至 30-40% | 高（2027-2028 出货追平） | **上修**。2026 ASIC 合计出货 ~1.9M（Google 900k + AWS 600k + MSFT 250k + Meta 180k）；NVIDIA 单位份额 2025 73%→2026E 62-66%。Microsoft Maia 200 FP4 10+ PFLOPS、3x Trainium3 已部署 GPT-5.2。Meta MTIA TCO -44%。Broadcom 手握 OpenAI/Meta/Google/Anthropic 四大合同，订单可见至 2029。**出货追平时间线维持 2027-2028，但收入份额追平可能从 2028-2029 提前至 2028** | 上修为 **高+**。建议将"2027 追平"的口径明确为"出货量"而非"收入" |
| **H2** CoWoS 瓶颈持续至 2027 | 中高（2027H2 可能衰减） | **方向维持但机制反转**。瓶颈持续确认：2026 ~1M 片需求已满载、NVIDIA 预定过半产能至 2027、嘉义+日本扩产。但 **新发现**：CoWoS-L 基板翘曲已迫使 Rubin Ultra 四芯取消——瓶颈不仅是"产能不足"，更是"良率/物理极限"。这意味着即使产能扩张，**超大型多芯 GPU 设计空间被结构性限制**，反而利好单芯 ASIC。SK Hynix-SK Hynix 06.07 签 HBM4 至 2030 | 维持中高。但增加 **子论点 2a：封装物理极限开始保护 ASIC 免受 GPU 代际跃迁冲击** |
| **H3** 推理 token 成本年降 10x | 高（定价权侵蚀 2028+） | **方向维持，定价权风险前移**。OpenAI 06.11 WSJ 考虑大幅降价；Google Plus $7.99→$4.99。但缓冲证据更强：Anthropic 运营收入 $30B（vs $9B 2025底）+ 1000+ 企业客户年消费>$100万 + reasoning 模型 token 消耗（GPT-5.5 vs 5.4 少用 40% 但绝对量仍高）。**成本通缩+需求超线性增长同时成立** | 维持高。但 **定价权侵蚀时间从 2028+ 前移至 2027H1**。建议新增 K5 监测频率（季度而非半年度） |
| **H4** NVIDIA 推理端护城河弱于训练端 | 中（速度放缓） | **方向维持，但 Groq 收购+LPU 是新变量**。NVIDIA $20B 收购 Groq（12月完成），GTC 2026 发布 Groq 3 LPX，使 Vera Rubin 每瓦 token 吞吐提升 35x。这是 NVIDIA **主动补齐推理短板** 的战略动作——护城河被低估的概率上升。但 Rubin Ultra 受挫说明硬件路线图斜率受限。CFO Kress 确认 H100 租金 YTD +20%、A100 +15%（"Fine Wine"效应） | 维持中。但 **子论点 4a 修订**：NVIDIA 通过 Groq LPU 主动防御推理端，护城河被低估的概率较 Round 2 上升 |
| **H5** GPU 2027-2028 从稀缺转向过剩 | 中低（推迟至 2028 评估） | **下修过剩概率**。Rubin 2026 出货仅 200-300k（TSMC N3 限制）；Rubin Ultra 改双两芯后 2027 算力减半意味着供给曲线更平缓而非更陡。H100 租金回升至 YTD +20%。**新世代稀缺比 Round 2 预期更持久**。全行业过剩需 Blackwell 大规模退役 + ASIC 替代加速 + Rubin 产能同时释放——三者 2027 前同时发生概率 <15% | 下修至 **低**。建议将 K4/H5 触发监测的重心从"H100 价格"转向"B200 利用率 + Rubin 实际量产节奏" |

### 子论点验证

| 子论点 | Round 2 | Round 3 | 修订建议 |
|--------|---------|---------|---------|
| ASIC 份额侵蚀速度 | 有条件通过 | **方向确认加速**：2026 单位份额 NVIDIA 62-66%，较 Round 2 的 73%（2025）下降显著 | 升级为 **通过**（条件：2027 验证收入份额） |
| 推理成本通缩利好应用 | 通过 | 方向维持，定价权风险前移 | 维持通过，新增 K5 季度监测 |
| GPU 过剩风险 | 技术关注 | 新世代稀缺比预期持久 | **降至低优先级观察** |
| CoWoS 投资机会 | 有条件通过 | 瓶颈持续+物理极限保护 | 维持有条件通过，但 **封装设备/良率解决商标的优先级上升** |

---

## 3. 催化剂时间线表（06.05 → 07.10 窗口 + 关键前置事件）

| 日期 | 事件 | 影响 | 强度 | 标的 |
|------|------|------|------|------|
| **06.07** | NVIDIA-SK Hynix 签多年 HBM4 技术合作+共同开发协议，覆盖至 2030 年前瞻 AI 内存供应 | + | 强 | NVDA / SK Hynix |
| **06.11** | WSJ 报道 OpenAI"考虑大幅降价"以对抗 Anthropic 竞争 | - | 中强 | K5 预警；OpenAI 隐含利空；推理通缩风险前移 |
| **06.27** | GE Vernova 燃气轮机驱动 AI 数据中心：xAI Colossus 1 + Microsoft Texas 7 台涡轮机；Q1 2026 数据中心电气化设备订单超过 2025 全年 | + | 中 | GE Vernova / 电力链（#14） |
| **06.30** | SemiAnalysis 确认 Rubin Ultra 四芯版因 CoWoS-L 基板翘曲取消，改为双两芯配置 | - | 强 | NVDA（2027 算力减半）/ AVGO（间接利好：ASIC 受影响小） |
| **07.01** | Rubin Ultra 改双两芯后 2027 名义算力减半确认；NVIDIA 重新分配部分 Rubin wafer start 至 Blackwell | - | 强 | NVDA 短期利空（路线图斜率）；Blackwell 产能缓解部分对冲 |
| **07.03** | TrendForce：AI 服务器需求持续支持 3Q26 存储价格，但消费需求走弱+高基数使涨幅收窄 | + | 中 | 存储链（HBM/DRAM） |
| **07.06** | TrendForce：AI 对高端 MLCC 需求推高日韩供应商 book-to-bill 至后疫情新高，2H26 短缺风险上升 | + | 中 | MLCC 供应商（Murata/Taiyo Yuden/Samsung EM） |
| **07.07** | NVIDIA 官方否认 SemiAnalysis 的 Rubin/Kyber 延迟传闻，称"芯片路线图完整"，Rubin 在 Oberon rack 出货，Rubin Ultra 继续 Kyber rack NVL576 | + | 中 | NVDA（市场情绪修复） |
| **Q2 2026** | CoreWeave 完成 $8.5B 投资级 GPU 抵押融资设施（首个投资级 GPU 背书证券化），DDTL 4.0 仅动用 $1.26B | +/- | 中 | K4 监测：融资条件改善但债务规模仍 $29B |
| **前置（04.06）** | Anthropic 扩大与 Google+Broadcom 合作：多 GW TPU 产能 2027 上线（~3.5GW），运营收入超 $30B（vs $9B 2025底） | + | 强 | GOOGL / AVGO / Anthropic（私有） |
| **前置（04.14）** | Meta-Broadcom 延伸合作：1GW 初始 MTIA 部署、多-GW 至 2029、**首个 2nm AI 芯片**；Hock Tan 离开 Meta 董事会 | + | 强 | AVGO / META / MTIA 链 |
| **前置（04.22）** | Google Cloud Next 2026：预览第八代 TPU 分拆——TPU 8t "Sunfish"（Broadcom 设计，训练）+ TPU 8i "Zebrafish"（MediaTek 设计，推理），目标 TSMC 2nm、2027 末 | + | 强 | GOOGL（路线图深度）/ AVGO（8t）/ MediaTek（8i） |
| **前置（05.08）** | OpenAI-Broadcom "Nexus" 项目融资谈判：$18B 生产成本，Broadcom 要求 Microsoft 承购 40% 芯片才肯融资第一阶段；OpenAI 2026 预计亏损 ~$14B、2029 前烧 >$200B | - | 中强 | OpenAI 财务脆弱性；K2/K8 间接预警 |
| **窗口内** | Google Plus 订阅降价 $7.99→$4.99/月；Anthropic 新模型（Opus 4.8/Fable 5）定价低于旧 Opus（$15/$75→$5/$25 或 $10/$50） | - | 中 | K5 定价战监测 |
| **窗口内** | Hyperscaler 2026 CapEx 指引：四大 $600-725B（+60% YoY）；Amazon ~$200B、MSFT ~$190B、GOOGL ~$180-190B、Meta ~$125-145B；Goldman 长期 $5.3万亿 | + | 强 | 全板块（CapEx 高景气确认） |
| **窗口内** | NVIDIA Q1 FY2027 $81.6B 收入（+85% YoY），DC $75.2B（+92%）；Q2 指引 $91B（±2%，**零中国收入假设**）；Vera Rubin 进入量产，Q3 首批出货 | + | 强 | NVDA（核心标的） |
| **窗口内** | Microsoft 在 GTC 宣布首个 Vera Rubin NVL72 系统点亮（Fairwater 数据中心，Wisconsin/Atlanta） | + | 中 | MSFT / NVDA |
| **窗口内** | GTC 2026（03.16）：Jensen Huang 宣布 Blackwell+Vera Rubin 至 2027 采购订单管道 **$1万亿**；预览 Feynman 2028 架构（3D 堆叠、TSMC A16 1.6nm、Rosa CPU） | + | 强 | NVDA（长期路线图） |
| **窗口内** | TrendForce（04.08）：Blackwell 占 2026 高端 GPU 出货 71%（从 61%），Rubin 占比从 29% 降至 22%（延迟），Hopper 10%→7% | +/- | 中 | NVDA 代际转换确认 |

### 催化剂密度分析
- **利好事件**：11 个（强强度 6 个）
- **利空事件**：4 个（强强度 2 个——均为 Rubin Ultra 受挫）
- **净方向**：明确利好主导，但利空事件集中在 **NVIDIA 路线图斜率** 这一单一维度

---

## 4. 假设修订建议（汇总）

### 建议上修
| 假设 | 从 → 到 | 理由 |
|------|---------|------|
| **H1** ASIC 份额侵蚀 | 高 → **高+** | 2026 出货数据 + Broadcom 四大合同 + NVIDIA 单位份额降至 62-66% |
| **AVGO 加权回报** | +8.25% → **+11.0%** | 订单可见度从主题变为可量化；Hock Tan >$100B 目标 |
| **GOOGL 锚定价值** | 维持 → **明确为风险收益比首选** | Ironwood GA + 8t/8i 路线图 + Anthropic 锚客户 |

### 建议下修/前移风险
| 假设/风险 | 从 → 到 | 理由 |
|-----------|---------|------|
| **H3 定价权侵蚀时间** | 2028+ → **2027H1** | OpenAI 降价信号 + Google Plus 降价 + Anthropic 新模型定价低于旧款 |
| **H5 GPU 过剩概率** | 中低 → **低** | Rubin Ultra 减半+Rubin 2026 仅 200-300k，新世代稀缺更持久 |
| **K5 触发监测频率** | 半年度 → **季度** | 定价战信号已出现，需高频跟踪 |

### 建议新增
| 项目 | 内容 |
|------|------|
| **子论点 2a** | 封装物理极限（CoWoS-L 翘曲）开始结构性保护 ASIC 免受 GPU 代际跃迁冲击 |
| **子论点 4a 修订** | NVIDIA 通过 Groq LPU 收购主动补齐推理短板，护城河被低估概率上升 |
| **新风险因子** | OpenAI 财务脆弱性（2026 亏损 ~$14B、2029 前烧 >$200B、Broadcom 要求 Microsoft 承购才肯融资）——是 K2/K8 的先行指标 |

---

## 5. 情景分析

### 情景概率调整（vs Round 2）

| 情景 | Round 2 概率 | Round 3 建议 | 调整理由 |
|------|-------------|-------------|---------|
| **牛：ASIC 加速+需求超线性** | 20% | **25%** | Broadcom 合同落地+Rubin Ultra 受挫反向利好 ASIC+Anthropic 收入验证需求 |
| **基准偏牛：高景气延续+稳步替代** | 35% | **40%** | $91B 指引+CapEx $600-725B+Rubin 量产 Q3 确认 |
| **基准偏熊：增速放缓+瓶颈缓解** | 25% | **20%** | CoWoS 瓶颈未缓解（物理极限）+HBM 全部售罄+定价战前移反而说明需求竞争激烈 |
| **熊：CapEx 周期逆转** | 15% | **12%** | OpenAI 财务脆弱性是真实风险，但 Microsoft/Amazon/Google 资产负债表仍健康（D/E 0.23） |
| **灾难：地缘冲击** | 5% | **3%** | 台海无新事件；AI Overwatch Act 立法进度未加速；H200 出口中国已放行 |

### 关键情景细化

**牛市情景（25%）的核心验证路径**：
- Rubin Q3 量产交付顺利 → Vera Rubin NVL72 部署超 80 站点 → NVIDIA Q2 FY2027 超 $91B 指引 → Broadcom Q3 FY2026 AI 收入超 $107B 指引 → Anthropic/OpenAI 收入持续超线性 → ASIC 出货 2027 追平 GPU

**熊市情景（12%）的核心触发链**：
- OpenAI 融资困难（Microsoft 拒绝承购 40%）→ OpenAI 削减 Broadcom Nexus 订单 → Hyperscaler Q3 财报 CapEx 指引下调 → CoreWeave 债务压力 → NVIDIA DC 增速降至 <30%（K6 触发）→ 板块 PE 压缩

**定价权侵蚀子情景（独立跟踪，概率 20%，2027H1 显现）**：
- OpenAI 大幅降价 → Anthropic 跟进 → 推理 API $/M tokens 降至 $0.05 以下 → 推理毛利率 <10% → Hyperscaler 压价 ASIC → Broadcom/NVIDIA ASP 季度下降 → K5 触发

---

## 6. 退场标准 K1-K8 触发状态

| 编号 | 标准 | Round 2 状态 | Round 3 状态 | 触发信号强度 |
|------|------|-------------|-------------|-------------|
| **K1** 核心逻辑失效（ASIC 停滞） | 未触发 | **远离触发**（ASIC 出货 +44.6%，合同加速落地） | 极低 |
| **K2** CapEx 周期逆转（削减>10%） | 未触发 | **未触发，但先行指标出现**：OpenAI 财务脆弱性（2026 亏损 $14B）+ Broadcom 要求 Microsoft 承购才肯融资 Nexus。需 Q3 Hyperscaler 财报验证 | 中（早期信号） |
| **K3** 技术替代（光计算/LPU） | 未触发 | **部分相关**：NVIDIA 收购 Groq 后 LPU 已纳入自身生态，不再是独立替代威胁；Tensordyne Napier 芯片声称 13x Blackwell 但未量产 | 低 |
| **K4** Neocloud 信用风险（CoreWeave 违约/H100<$1） | 未触发 | **未触发，风险分化**：CoreWeave 完成 $8.5B 投资级融资（改善），但总债务 $29B、流动负债 $17.8B、Capex $30B 仍高；H100 租金 YTD +20%（远离 $1 触发线） | 低（改善方向） |
| **K5** API 定价战（任两家同季降>50%） | 未触发 | **早期预警**：OpenAI 考虑降价（06.11）+ Google Plus 降价 37%（$7.99→$4.99，未达 50%）+ Anthropic 新模型定价低于旧款。**尚未触发**（需同季>50% 且两家），但信号方向明确 | 中强（预警升级） |
| **K6** NVIDIA 收入减速（DC 增速<30% 环比下降） | 未触发 | **远离触发**：Q1 FY27 DC +92% YoY；Q2 指引 $91B（+95% YoY，零中国假设） | 极低 |
| **K7** CoWoS 利用率下降（<85%/交期<3月） | 未触发 | **远离触发**：2026 ~1M 片需求满载；排队 >50 周；NVIDIA 预定过半产能至 2027；Rubin Ultra 受挫说明产能极度过紧 | 极低 |
| **K8** AI 应用 ROI 失败（F500 预算降/AI 融资降>30%） | 未触发 | **信号分化**：Anthropic 收入 $30B+1000 企业客户>$100万（强）；OpenAI 亏损 $14B+用户目标未达（弱）。VC 融资 $150B（Jensen GTC 数据）。**未触发但 OpenAI 财务是薄弱环节** | 中 |

### 退场监测优先级调整建议
1. **K5（API 定价战）** — 从第 5 位升至 **第 2 位**（定价战信号已出现）
2. **K6（NVIDIA 收入）** — 维持第 1 位（最高频直接）
3. **K2（CapEx 削减）** — 从第 2 位降至第 3 位（OpenAI 脆弱但 Hyperscaler 健康）
4. **K7（CoWoS）** — 维持（物理极限确认，未缓解）
5. **K4/K8** — CoreWeave 改善/OpenAI 脆弱，分化跟踪

---

## 7. 时间维度

### 短期（0-3个月，至 2026.10）
- **NVIDIA Q2 FY2027 财报（~08月）**：验证 $91B 指引；FY2028 展望；Rubin 首批交付数据
- **Hyperscaler Q2 财报季（07-08月）**：CapEx 指引是否维持 $600-725B；OpenAI 财务压力是否传导至 Microsoft
- **Rubin 首批客户交付（08月，Quanta 确认）**：Vera Rubin NVL72 实际部署节奏
- **OpenAI API 定价决策**：是否实际执行"大幅降价"

### 中期（3-9个月，2026.10-2027.06）
- **Broadcom Q3 FY2026 财报（~09月）**：AI 收入是否达 $107B 指引；Nexus 项目融资落地
- **Rubin 量产爬坡（Q4 2026-Q1 2027）**：从 200-300k 能否扩至 Rubin 目标
- **ASIC 大规模部署**：Maia 200 Phoenix 站点；Trainium3 GA；MTIA v3 全量
- **2027 CapEx 指引**：Hyperscaler 是否继续加码

### 长期（9-18个月，2027H1-2027 末）
- **Rubin Ultra 双两芯版交付（2027H2）**：算力减半后客户接受度
- **TPU 8t/8i 量产（2027 末）**：2nm 制程+训练/推理分拆
- **OpenAI Broadcom Nexus 首批芯片（2026H2-2027）**：自研 ASIC 能否替代 NVIDIA
- **AI Overwatch Act 立法进展**：是否通过，影响 H200/Rubin 出口中国

---

## 8. 盲区与数据缺口

### 研究员B明确承认的盲区

1. **AVGO Forward PE 口径仍未澄清（Round 2 遗留 RQ-3）**：当前 $380 股价、$63.8B 2025 收入、市值 $1.7T。若按 FY2027 自然年 EPS $12-13，PE ~29-32x（合理）；若按 FY2026 报告 EPS，PE 可能 >38x。**研究员B 无法从公开搜索确认权威 EPS 共识**，建议 Researcher A 或 PM 用 Bloomberg/Refinitiv 澄清。

2. **Rubin Ultra "算力减半"的实际影响范围**：SemiAnalysis 报告与 NVIDIA 官方否认存在分歧。双两芯设计是否真能在 2027 交付、客户（OpenAI/Microsoft/Google）的采购合同是否允许规格变更——这些细节不公开。**可能高估或低估影响**。

3. **OpenAI 财务真实状况**：WSJ 报道 OpenAI "错过内部用户/收入目标"+ CFO 担忧无法支付未来算力合同，但 Altman/Friar 公开否认。2026 预计亏损 $14B、2029 前烧 $200B 的数据来源是 The Information 引述内部备忘录，**未经审计**。若是真的，OpenAI-Broadcom Nexus 项目的 $18B 融资风险被低估。

4. **NVIDIA Q2 FY2027 实际数据**：本报告基于 Q1 财报+Q2 指引，**Q2 实际财报尚未发布（~08月）**。Rubin 量产爬坡的真实速度、Blackwell Ultra 需求持续性、中国收入恢复情况——均需财报验证。

5. **Broadcom "AI 收入"中加速器 vs 网络的拆分**：Round 2 RQ-2 未解决。Hock Tan 公开目标 ">=$100B AI 收入 2027" 但未拆分。Broadcom 网络收入（Ethernet/SerDes/PCIe）本应独立于 ASIC 设计收入，但财报口径混合。**这直接影响 AVGO 估值**。

6. **Hyperscaler 自研 ASIC 的真实 benchmark**：Microsoft 声称 Maia 200 "3x Trainium3"、Anthropic 未公开 TPU vs GPU 的实际 TCO。**第三方独立基准缺失**（RiiVEN 报告确认）。ASIC 份额侵蚀的"质量"无法量化。

7. **地缘政策的时效性**：AI Overwatch Act 立法进度、H200 出口中国的 50% 量上限实际执行情况、华为昇腾全球禁令的执法力度——这些在 06.05-07.10 窗口内无重大新事件，但 **高波动性**（Round 2 已标注）。任何中美关系变化可在 1-2 周内翻转。

### 建议补充研究
- RQ-11（新增）：Broadcom AI 收入拆分——加速器设计 vs 网络组件的 FY2027 自然年口径
- RQ-12（新增）：Rubin Ultra 双两芯 vs 四芯的客户合同影响——采购方是否允许规格变更
- RQ-13（新增）：OpenAI 财务可持续性——Nexus 项目融资落地条件 + Microsoft 承购意愿

---

## 9. 来源清单

### NVIDIA 路线图与 GTC 2026
1. TrendForce (2026.04.08) — Rubin Faces Delay Risks; Blackwell to Account for Over 70% — https://www.trendforce.com/presscenter/news/20260408-13003.html
2. WCCFtech — NVIDIA Confirms Vera Rubin Launch Q3, Volume Ramp Q4 — https://wccftech.com/nvidia-confirms-vera-rubin-launch-in-q3-volume-ramp-q4-blackwell-continues-to-see-massive-demand/
3. TechTimes (2026.07.01) — NVIDIA Rubin Ultra Four-Die GPU Cancelled — https://www.techtimes.com/articles/319410/20260701/nvidia-rubin-ultra-four-die-gpu-cancelled-packaging-limits-cut-2027-performance-half.htm
4. NVIDIA Newsroom (2026.01.05) — NVIDIA Kicks Off Next Generation with Rubin — https://nvidianews.nvidia.com/news/rubin-platform-ai-supercomputer
5. VRLA Tech — NVIDIA GPU Roadmap 2026-2030 — https://vrlatech.com/nvidia-gpu-roadmap-2026-2030/
6. TechDefused (2026.04.01) — Nvidia redesigns Rubin Ultra, shifts wafer starts — https://techdefused.com/a/OjN825i/nvidia-redesigns-rubin-ultra-chip-and-shifts-wafer-starts-to-boost-blackwell-sup
7. PCCentral (2026.07.07) — NVIDIA Denies Rubin Delay Rumors — https://pccentral.net/nvidia-denies-rubin-delay-rumors-confirms-roadmap/
8. Next Waves Insight — Nvidia Rubin in Production: Allocation Map — https://nextwavesinsight.com/nvidia-rubin-gpu-production-silicon-hyperscaler-2026/
9. WCCFtech — NVIDIA Rubin AI Servers to Ship by August (Quanta) — https://wccftech.com/nvidia-rubin-ai-servers-to-ship-to-customers-by-august-this-year/
10. NVIDIA GTC 2026 Keynote (YouTube) — https://www.youtube.com/watch?v=jw_o0xr8MWU
11. NVIDIA Investor Relations (2026.03.16) — Vera Rubin Opens Agentic AI Frontier — https://investor.nvidia.com/news/press-release-details/2026/NVIDIA-Vera-Rubin-Opens-Agentic-AI-Frontier/default.aspx
12. NVIDIA Blog — GTC 2026 Live Updates — https://blogs.nvidia.com/blog/gtc-2026-news/
13. CNBC (2026.03.16) — Jensen Huang: $1 trillion in orders through 2027 — https://www.cnbc.com/2026/03/16/nvidia-gtc-2026-ceo-jensen-huang-keynote-blackwell-vera-rubin.html
14. Jon Peddie Research — Nvidia GTC 2026 keynote — https://www.jonpeddie.com/news/nvidia-gtc-2026-keynote/
15. Presenc AI — GPU Shipment Tracker Blackwell to Rubin 2026 — https://presenc.ai/research/gpu-shipment-tracker-blackwell-rubin-2026

### Google Ironwood TPU / Anthropic
16. Anthropic (2026.04.06) — Expands partnership with Google and Broadcom — https://www.anthropic.com/news/google-broadcom-partnership-compute
17. Google Cloud Blog (2025.11.06) — Ironwood TPUs GA — https://cloud.google.com/blog/products/compute/ironwood-tpus-and-new-axion-based-vms-for-your-ai-workloads
18. Google Cloud Press Corner (2026.04.06) — Anthropic Expands Use of TPUs — https://www.googlecloudpresscorner.com/2026-04-06-Anthropic-Expands-Use-of-Google-Cloud-and-TPUs
19. Futurum Group (2026.04.09) — Anthropic TPU Deal Structural Advantage — https://futurumgroup.com/insights/anthropics-gigawatt-scale-tpu-deal-with-broadcom-creates-a-structural-advantage/
20. PulseMark — Google Ironwood TPU Expansion: 3.2M Units — https://pulsemark.ai/google-tpu-expansion-40-percent-growth-3-2m-units/
21. Google Blog (2025.04.09) — Ironwood: first TPU for age of inference — https://blog.google/innovation-and-ai/infrastructure-and-cloud/google-cloud/ironwood-tpu-age-of-inference/
22. TopTechNews — Google Ironwood TPU Mass Scale 2026 — https://toptechnews.net/articles/google-ironwood-tpu-mass-scale-2026.html
23. The Next Web (2026.04.22) — Google previews 8th-gen split TPU at 2nm — https://thenextweb.com/news/google-ironwood-tpu-inference-cloud-next
24. Anthropic (2025.10.23) — Expanding Use of Google Cloud TPUs — https://www.anthropic.com/news/expanding-our-use-of-google-cloud-tpus-and-services

### AWS / Microsoft / Meta ASIC
25. Microsoft Blog (2026.01.26) — Maia 200: AI accelerator for inference — https://blogs.microsoft.com/blog/2026/01/26/maia-200-the-ai-accelerator-built-for-inference/
26. GeekWire (2026.01.26) — Microsoft unveils Maia 200 — https://www.geekwire.com/2026/microsoft-unveils-maia-200-ai-chip-claiming-performance-edge-over-amazon-and-google/
27. AWS — EC2 Trn3 UltraServers — https://aws.amazon.com/ec2/instance-types/trn3/
28. FinancialContent (2026.01.26) — Custom Silicon Titans: Meta and Microsoft — https://markets.financialcontent.com/stocks/article/tokenring-2026-1-26-custom-silicon-titans-meta-and-microsoft-challenge-nvidias-dominance
29. Tom's Hardware — Custom AI ASIC state of play (May 2026) — https://www.tomshardware.com/tech-industry/semiconductors/custom-ai-asics-examined-from-broadcom-to-mtia
30. Presenc AI — Hyperscaler Custom Silicon Tracker 2026 — https://presenc.ai/research/hyperscaler-custom-silicon-tracker-2026

### Broadcom 合同
31. Broadcom Investors (2025.10.13) — OpenAI 10GW collaboration — https://investors.broadcom.com/news-releases/news-release-details/openai-and-broadcom-announce-strategic-collaboration-deploy-10
32. Digitimes — Broadcom secures $10B ASIC win, Apple/xAI next — https://apps.digitimes.com/news/a20250908PD221/broadcom-asic-earnings-openai-guidance.html
33. DCD (2025.10.13) — OpenAI-Broadcom 10GW — https://www.datacenterdynamics.com/en/news/openai-partners-with-broadcom-for-development-of-custom-ai-accelerators-and-ethernet-solutions/
34. CNBC (2026.04.14) — Meta commits 1GW with Broadcom — https://www.cnbc.com/2026/04/14/meta-commits-to-one-gigawatt-of-custom-chips-with-broadcom-as-hock-tan-agrees-to-leave-board.html
35. Nasdaq/Broadcom (2026.04.14) — Extended Partnership with Meta MTIA — https://www.nasdaq.com/press-release/broadcom-announces-extended-partnership-meta-deploy-technology-support-multi
36. CNBC (2025.10.13) — OpenAI partners with Broadcom — https://www.cnbc.com/2025/10/13/openai-partners-with-broadcom-custom-ai-chips-alongside-nvidia-amd.html
37. DCD (2026.05.08) — OpenAI-Broadcom $18bn Nexus financing discussions — https://www.datacenterdynamics.com/en/news/openai-and-broadcom-in-discussions-over-financing-of-18bn-custom-chip-project-report/
38. DCD (2026.04.15) — Meta partners with Broadcom for MTIA generations — https://www.datacenterdynamics.com/en/news/meta-partners-with-broadcom-for-development-of-multiple-generations-of-mtia-chips/
39. Motley Fool (2026.03.25) — OpenAI as Broadcom's newest chip customer — https://www.fool.com/investing/2026/03/25/openai-just-became-broadcoms-newest-chip-customer/

### CoWoS / HBM / 产能
40. LinkedIn (Mark Hirsch) — HBM Supply Chain Interdependence — https://www.linkedin.com/posts/markdhirsch_hbm-ai-semiconductors-activity-7462630687024726016-uQ3u
41. TrendForce (2026.07.03) — AI Server Demand Supports 3Q26 Memory Prices — https://www.trendforce.com/presscenter/news/20260703
42. TrendForce (2026.07.06) — AI MLCC Book-to-Bill Post-Pandemic Highs — https://www.trendforce.com/presscenter/news/20260706-13136.html

### 推理模型 / API 定价
43. CNBC (2026.06.11) — OpenAI mulls slashing prices vs Anthropic (WSJ) — https://www.cnbc.com/2026/06/11/openai-mulls-slashing-prices-ahead-of-competition-from-anthropic-wsj.html
44. Inc. — Google AI Plus price cut $7.99→$4.99 — https://www.inc.com/chloe-aiello/googles-new-ai-price-cuts-should-make-openai-and-anthropic-nervous/91359297
45. OpenAI — Introducing GPT-5.5 — https://openai.com/index/introducing-gpt-5-5/
46. Anthropic — Introducing Claude Opus 4.6 — https://www.anthropic.com/news/claude-opus-4-6
47. Towards AI — Thinking Tokens Are Not Free — https://pub.towardsai.net/thinking-tokens-are-not-free-most-pipelines-treat-them-like-they-are-846708fdcef1

### 电力 / 能源
48. Meta (2026.01) — Nuclear Energy Projects 6.6 GW — https://about.fb.com/news/2026/01/meta-nuclear-energy-projects-power-american-ai-leadership/
49. CNBC (2026.06.27) — GE Vernova Gas Turbines for AI — https://www.cnbc.com/2026/06/27/ge-vernova-gas-turbines-ai-data-centers.html
50. Power Engineering — GE Vernova turbine slots tighten through 2030 — https://www.power-eng.com/gas/turbines/data-centers-drive-record-surge-in-ge-vernova-power-equipment-orders-as-turbine-slots-tighten-through-2030/

### Neocloud / CoreWeave
51. CoreWeave Investors (2026.03.31) — $8.5B Financing Facility, Investment Grade — https://investors.coreweave.com/news/news-details/2026/CoreWeave-Closes-Landmark-8-5-Billion-Financing-Facility-Achieving-First-Investment-Grade-Rated-GPU-backed-Financing/default.aspx
52. CoreWeave SEC Filing — Q4/FY2025 Earnings — https://www.sec.gov/Archives/edgar/data/1769628/000176962826000094/coreweave4q25earningspress.htm
53. Tech-Insider — CoreWeave $30B Capex Gamble — https://tech-insider.org/coreweave-30-billion-capex-ai-cloud-2026/
54. IO Fund — Nvidia/CoreWeave/Nebius Circular Financing — https://io-fund.com/ai-stocks/nvidia-coreweave-nebius-circular-financing-gpu-boom

### 地缘 / 出口管制
55. Congressional Research Service R48642 — US Export Controls China Semiconductors — https://www.congress.gov/crs-product/R48642
56. WSJ Opinion — AI Overwatch Act would help China — https://www.wsj.com/opinion/ai-overwatch-act-would-help-china-5e5e61fe
57. American Action Forum — Beyond CHIPS: expanding export controls — https://www.americanactionforum.org/insight/beyond-chips-can-expanding-export-controls-slow-chinas-ai-progress/
58. Built In — Trump lifts AI chip ban China Nvidia — https://builtin.com/articles/trump-lifts-ai-chip-ban-china-nvidia
59. Oplexa — US-China Chip War 2026 — https://oplexa.com/us-china-chip-war-2026-semiconductor/
60. CSIS — DeepSeek, Huawei, Export Controls — https://www.csis.org/analysis/deepseek-huawei-export-controls-and-future-us-china-ai-race

### Hyperscaler CapEx / 估值
61. Yahoo Finance — Hyperscaler $600-725B spending — https://finance.yahoo.com/sectors/technology/article/meta-microsoft-amazon-and-alphabet-are-about-to-spend-a-shocking-amount-of-money-to-dominate-the-ai-era-115359575.html
62. CNBC (2026.02.06) — Tech AI spending approaches $700B — https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html
63. 247wallst — NVIDIA back above $5 trillion — https://247wallst.com/investing/2026/06/16/nvidia-is-back-above-5-trillion-heres-what-comes-next/
64. Yahoo Finance — NVIDIA Forward PE multiyear low — https://finance.yahoo.com/technology/article/nvidias-valuation-just-hit-a-multiyear-low--even-as-revenue-sets-records-155948933.html
65. INDMoney — NVIDIA Q2 FY2027 $91B guidance, zero China — https://www.indmoney.com/blog/us-stocks/why-is-nvidia-stock-falling-dip-analysis-nvda-outlook

---

*研究员B Round 3 报告完成 — 2026.07.10*
*捕获窗口：2026.06.05 → 07.10*
*下次计划更新：2026.08（NVIDIA Q2 FY2027 财报后 CIO 综合）*
