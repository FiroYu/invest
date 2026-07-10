# Researcher C — 宏观+地缘+利率+供应链 (Round 3)

> **课题#17：AI推理经济与定制芯片范式转移**
> **报告日期：2026.07.10 | 捕获窗口：2026.06.05 → 07.10（~5周）**
> **研究员：C（宏观/地缘/利率/供应链）**
> **基线：Round 2 (06.04) — 评级"通过"，NVDA Forward PE 25.5x**

---

## 1. 执行摘要

### 方向投票：维持做多 / 中性偏多（+1档 vs Round 2）

| 维度 | Round 2 (06.04) | Round 3 (07.10) | 变化 | 驱动因素 |
|------|-----------------|-----------------|------|----------|
| **方向投票** | 通过（核心）/ 看多 | **维持看多，但估值压制加深** | 维持 | CapEx加速但利率转向加息预期 |
| **置信度** | 中高 | **中**（下调半档） | ↓ | 利率路径不确定性 + FCF赤字扩大 |
| **加权回报 (NVDA)** | +10.0% | **+11.5%** | ↑1.5pp | 2027 CapEx>$1T确认需求；但利率压制估值倍数 |
| **加权回报 (GOOGL)** | +9.75% | **+10.0%** | ↑0.25pp | Cloud +63%最强验证；但$85B股权稀释对冲 |
| **加权回报 (AVGO)** | +8.25% | **+9.5%** | ↑1.25pp | ASIC需求确认+6客户锁定CoWoS至2028 |
| **加权回报 (MRVL)** | +0.75% | **+1.0%** | ↑0.25pp | FY2028 $16.5B指引确认，但仍投机级 |
| **核心逻辑** | 通过 | **维持通过** | 维持 | 需求侧验证为历史最强 |

### 三大宏观发现

1. **AI CapEx超级周期未见顶——反而在加速。** Round 2的~$700B已被上修至$710-725B（4家合计2026年），BofA和Moody's均预测2027年突破$1万亿。这不是"见顶验证"，是"周期仍在加速"。Alphabet CFO明确"2027 CapEx将比2026年significantly increase"。Morgan Stanley预测仅Alphabet一家2027年就$250B。**这是本周期最重要的数据点。**

2. **利率环境恶化——从"不降息"升级为"市场定价加息"。** Round 2基线为"Fed 3.50-3.75%不降息，JPM/Danske预测可能加息"。6月17日FOMC（12-0投票连续第四次维持）后，市场已正式定价2026年10月一次25bp**加息**（CME FedWatch），Fed官员将年终利率预期上修至3.6-4.1%。10Y UST ~4.47%（7/6）。新任Fed主席立场偏鹰。**这对依赖远期现金流的AI半导体估值构成直接压制。**

3. **金融脆弱性从"预警"进入"实测"——FCF崩溃正在发生但融资渠道仍畅通。** Amazon TTM FCF跌至$1.2B（-95% YoY），分析师预测2026年FCF -$17B至-$28B（Morgan Stanley/BofA）。Meta被JPMorgan下调评级，预测2026 FCF -$4B、2027 -$24B。Alphabet FCF margin从21%降至9.2%。但融资渠道畅通：Alphabet $85B股权增发（超额认购，含Berkshire $10B）；CoreWeave完成$8.5B DDTL 4.0（首次GPU抵押投资级）。**核心矛盾：FCF在崩溃，但信用市场仍开放——这个窗口能持续多久是最大不确定性。**

### 对评级的建议

**维持"通过"评级。** 核心论点获得自课题创建以来最强的需求侧验证（CapEx加速到$1T、Cloud增速28-63%、backlog翻倍）。但需将利率风险因子从"中高位"上调至"高位"，将私募流动性/Neocloud风险因子从"承压改善"修正为"承压但FCF崩溃进行中"。建议在综合报告中将利率敏感度明确标注为"高"。

---

## 2. 假设验证表（H1-H5）

| 假设 | Round 2裁定 | Round 3更新 | 新证据 | C判断 |
|------|------------|------------|--------|-------|
| **H1** ASIC推理份额→2028年30-40% | 高（方向确认，时间修正为2027-2028出货追平） | **高（维持+强化）** | Amazon芯片业务>$20B年化run-rate（三位数增长）；Meta确认开发定制ASIC（Broadcom合作）；Microsoft Maia 200已上线；Google TPU v8 Ironwood出货。所有4家Hyperscaler定制芯片均已进入规模部署 | ASIC范式转移方向不变，证据链比Round 2更强 |
| **H2** CoWoS瓶颈持续至2027 | 中高（可能2027H2缓解） | **中高（维持，瓶颈比预期更持久）** | CoWoS仍是2023-2025最紧约束；GPU/HBM/CoWoS供应"still broken through 2027"（Fusion WW）；TSMC先进节点订单簿已满；全球半导体销售额预计$975B（2026）；半导体设备backlog排至2027 | 瓶颈不会在2027H2快速缓解——产能扩张速度被需求增速持续超越 |
| **H3** 推理token成本年降10x持续 | 高（成本下降确认，定价权侵蚀为2028+风险） | **高（维持，但memflation成为新变量）** | Google处理>16B tokens/min（环比+60%）；Amazon Bedrock Q1处理tokens超过历史所有年份总和。但存储通胀（Q3 +40-50%，Q4 +30-40%）可能在短期内推高推理边际成本 | 趋势不变，但短期成本曲线出现memflation扰动 |
| **H4** NVIDIA推理端护城河弱于训练端 | 中（方向确认但速度放缓） | **中（维持）** | NVIDIA Q1 FY2027 DC收入$75.2B（+92%）；Hyperscaler每家都在推定制芯片但NVIDIA仍是核心供应商。NVIDIA有"超过$1万亿累计收入路径"到2027年底（CoBank引用）。但定制芯片份额确实在扩大 | 短期（0-12月）护城河仍深；中期（2027-2028）侵蚀加速 |
| **H5** GPU算力2027-2028过剩 | 中低（推迟至2028评估） | **中低（维持）** | 新世代（B200/Rubin）仍sold out；Hyperscaler CapEx加速意味着GPU需求仍在扩张。但Meta延长数据中心服务器寿命（内存短缺信号）、Apple因内存成本涨价上调产品价格——供应链紧张而非过剩 | 全行业过剩推至2028+确认；当前仍是卖方市场 |

---

## 3. 横向风险因子传导表

| 风险因子 | Round 2状态 | Round 3状态 | 方向 | 影响路径 | #17敏感度 | 变化原因 |
|---------|------------|------------|------|---------|----------|----------|
| **F1: AI CapEx超级周期** | 高景气→"生死验证期" | **高景气→加速期（验证通过，非见顶）** | ↑ 强化 | CapEx从~$700B上修至$710-725B；2027预测$1T+；需求侧验证为历史最强（Cloud 28-63%增速、backlog翻倍至$460-627B） | **极高** | Q1 2026财报全面超预期；BofA/Moody's/JPMorgan均上修预测；"生死验证"结论：**活下来了** |
| **F2: 利率（Higher for Longer）** | 中高位→HFL确认 | **高位→市场定价加息** | ↑↑ 重大恶化 | Fed 3.50-3.75%连续4次不降；CME定价10月加息25bp；10Y UST ~4.47%；年终预期上修至3.6-4.1%；新Fed主席偏鹰。直接压制AI半导体Forward PE | **高**（新增升级） | 从"可能加息"变为"市场已定价加息"——Round 2的最坏情景正在成为基准情景 |
| **F3: 中美脱钩** | 阶段性缓和→结构不可逆 | **缓和逆转→升级期** | ↑ 恶化 | 美国撤销AI Diffusion Rule但发布新指引：使用华为Ascend芯片违反出口管制；禁止向中国境外中企发运AI芯片（6/1）；台湾考虑收紧AI芯片对华出口（6/10）。华为董事长称限制"加速了中国半导体自主化" | **高** | Round 2的"阶段性缓和"判断已过时；管制正在升级，但方向是"精准打击"而非"全面封锁" |
| **F4: 私募流动性悖论** | 承压→缓慢改善 | **承压→FCF崩溃进行中但融资窗口仍开** | ↑ 恶化 | Amazon FCF跌至$1.2B（TTM）；Meta被JPMorgan下调（预测2026 FCF -$4B）；Alphabet FCF margin 21%→9.2%。但Alphabet $85B股权增发超额认购；CoreWeave DDTL 4.0 $8.5B关闭（首次投资级GPU抵押融资）。SpaceX新债务亏损扩大引发私募信用担忧 | **中高** | FCF赤字是确定的，但信用市场仍开放——关键问题是窗口何时关闭 |

### 交叉触发规则更新

| 规则 | Round 2 | Round 3状态 | 激活情况 |
|------|---------|------------|---------|
| 规则1：CapEx停滞+中美脱钩↑ | 维持 | **未触发**（CapEx加速中） | ❌ 未激活——CapEx不仅没停滞还在加速 |
| 规则2：CapEx超现金流+利率>5%+私募信贷收紧 | 新增 | **部分激活**（FCF崩溃中+利率3.75%但加息预期+私募信用出现SpaceX裂痕） | ⚠️ 2/3条件接近——利率未到5%但方向向上 |
| 规则3：电力短缺+存储通胀同时恶化 | 新增 | **部分激活**（9-18GW短缺确认+内存Q3 +40-50%） | ⚠️ 双双恶化但均未达极端 |
| 规则4：NVDA DC增速<30%+CoWoS利用率<85% | 新增 | **未触发**（NVDA Q1 +92%，CoWoS满载） | ❌ 未激活 |

---

## 4. Hyperscaler CapEx深度表（核心数据）

### 4.1 2026年CapEx指引（截至2026.07.10）

| 公司 | 2025实际 | 2026指引（最新） | vs 2025 YoY | Q1 2026实际CapEx | 2027信号 | FCF影响 |
|------|---------|-----------------|-------------|-----------------|---------|---------|
| **Microsoft** | ~$118B | **$190B**（含$25B组件涨价） | +61% | $31.9B (FY26 Q3, +84% YoY) | 未明确，但FY27指引"双位数增长" | FCF $5.9B（Q2），大幅压缩；股价YTD -17% |
| **Alphabet** | ~$91B | **$180-190B**（上修自$175-185B） | +100-105% | $35.7B（+>100% YoY） | **CFO明确"significantly increase"**；MS预测$250B | FCF margin 21%→9.2%；Pivotal预测FCF降90%至$8.2B；$85B股权增发 |
| **Amazon** | ~$130B | **~$200B** | +54% | $44.2B（+77% YoY） | 未量化但OpenAI 2GW Trainium+Anthropic 5GW承诺已锁定2027+ | FCF $1.2B TTM（-95%）；MS/BofA预测2026 FCF -$17B至-$28B |
| **Meta** | ~$72B | **$125-145B**（上修自$115-135B） | +74-101% | $19.8B | JPMorgan预测2027 $202B（+42%） | JPMorgan下调评级；预测2026 FCF -$4B、2027 -$24B |
| **4家合计** | ~$410B | **$710-725B** | +73-77% | ~$132B Q1 | **BofA: 2027 >$1T；Moody's: ~$1T** | FCF从~$200B→接近$0或负值 |

### 4.2 需求侧验证（为什么CapEx能维持）

| 验证维度 | 数据 | 解读 |
|---------|------|------|
| Cloud增速 | AWS +28%（15季度最快）；Azure +39-40%；Google Cloud +63% | 三大云增速均为近年最快——这不是产能空转 |
| Backlog | Microsoft RPO $627B（+99% YoY）；Google Cloud $460B（QoQ翻倍）；AWS $364B（+40% YoY） | 合计>$1.45万亿已签约未确认收入——CapEx有合同背书 |
| AI收入run-rate | Microsoft AI $37B（+123% YoY）；Amazon AI $15B（首年）；Amazon芯片业务$20B | AI收入从零到百亿级仅用3年——需求变现速度前所未有 |
| Token消费 | Google 16B tokens/min（环比+60%）；Amazon Bedrock Q1 tokens>历史总和 | 推理需求指数级增长——范式转移的核心假设得到验证 |
| 大客户承诺 | OpenAI→AWS 2GW Trainium（2027起）；Anthropic→Google 5GW TPU（5年）+AWS 5GW Trainium | 前沿AI公司已锁定数十GW产能到2030——需求可见度极长 |

### 4.3 关键判断：CapEx周期是否见顶？

**结论：未见顶。处于加速期的后半段，但峰值（大概率2027-2028年）仍在前方。**

依据：
- **Moody's**连续上修：原始预测$600B→$700B（3月）→$785B（5月）。每次上修$85B+
- **BofA**：2026 >$800B，2027 >$1T
- **JPMorgan**：上调2026-2030年AI CapEx预测（6月29日Fortune报道）
- **American Century**（管理$200B+资产）：7家公司（含Oracle/CoreWeave）2026 CapEx $775B（+78%）
- **Avory Research**：Big 4加速计算周期在美元基础上仅完成45-55%，峰值在2027-2028年$700-800B
- **CoBank**（6月11日）："AI基础设施周期可能仍处于早期阶段"——与2000年电信泡沫的关键区别在于投资回报率

**但需注意风险信号：**
- Meta被JPMorgan首次下调至Neutral（价格目标$825→$725）——首家被分析师因AI CapEx强度而下调的Hyperscaler
- "AI股票气袋"（Dan Ives，6月底）——Meta和Microsoft"交易像熊市股票"
- Avory分析：2026 $700B不是"新常态基线"，而是"前置加速"——峰值后将正常化至$380-800B

---

## 5. 跨课题传导更新表

| 关联课题 | Round 2传导判断 | Round 3更新 | 新证据 | 传导强度变化 |
|---------|---------------|------------|--------|------------|
| **#01 AI架构演进** | 推理成本下降→LLM经济性改善→JEPA推迟至2028+ | **维持** | Token消费指数增长（Google 16B/min环比+60%）确认LLM主导地位更稳固 | 维持中高 |
| **#02 光互联(CPO)** | 推理集群规模扩大→互联带宽成关键瓶颈→直接利好CPO | **强化** | Anthropic 5GW Google TPU部署、OpenAI 2GW AWS Trainium——超大集群建设规模超出Round 2预期 | ↑ 高 |
| **#11 先进制程(GAA)** | 封装>制程短期，2027H2后制程可能升温 | **维持** | TSMC先进节点订单簿已满；2026半导体销售额$975B（历史新高）；CoWoS瓶颈持续到2027 | 维持中 |
| **#14 AI基础设施(能源)** | 电力可能成为2027-2028首要物理限制 | **强化（正在成为现实）** | 9-18GW短缺确认（2027）；Hyperscaler签署多个核能PPA（Amazon-Talen、Microsoft-Constellation 20年、Meta-Entergy）；Google-Fervo地热；燃气轮机售罄至2030维持 | ↑↑ 极高 |
| **#21 供应链碎片化** | TSMC/CoWoS/HBM受地缘影响 | **强化** | 台湾考虑收紧AI芯片对华出口（6/10）；美国禁止向中企发运AI芯片（6/1）；华为Ascend被认定使用即违反出口管制——供应链分化加速 | ↑ 高 |
| **新增：#03 人形机器人** | （Round 2已提及中国零部件依赖） | **关注** | 存储通胀+芯片管制可能推高人形机器人BOM成本（中国零部件60-70%依赖+内存涨价） | 新增，中 |

---

## 6. 情景分析

### 概率分配（合计100%）

| 情景 | 概率 | Round 2对比 | 核心假设 |
|------|------|------------|---------|
| **金发姑娘：ASIC加速+需求超线性** | 22% | ↑2pp | 2027 CapEx>$1T确认；Rubin验证MoE 10x改善；Agentic AI爆发；利率意外转鸽 |
| **基准偏牛：高景气延续+稳步替代** | 33% | ↓2pp | CapEx维持~$750B（2026）→$900B-$1T（2027）；利率维持3.50-4.00%；FCF赤字但融资渠道畅通 |
| **基准偏熊：增速放缓+瓶颈缓解** | 25% | 维持 | 2027 CapEx增速降至+20-30%（vs 2026 +77%）；利率加息至4.0-4.25%；FCF赤字扩大导致CapEx增速被迫放缓 |
| **AI冬天：CapEx周期逆转** | 15% | 维持 | 2027H1 2+ Hyperscaler下调CapEx>15%；Neocloud信用事件；利率>4.5%；AI应用ROI大规模证伪 |
| **黑天鹅：地缘冲击** | 5% | 维持 | 台海封锁/TSMC中断/全面技术封锁 |

### 概率加权预期回报（12个月）

| 标的 | 金发姑娘(22%) | 基准偏牛(33%) | 基准偏熊(25%) | AI冬天(15%) | 黑天鹅(5%) | **加权** | vs R2 |
|------|-------------|-------------|-------------|-----------|-----------|---------|-------|
| **NVDA** | +40% | +22% | +5% | -25% | -50% | **+11.5%** | +1.5pp |
| **AVGO** | +35% | +22% | +5% | -30% | -50% | **+9.5%** | +1.25pp |
| **GOOGL** | +25% | +16% | +10% | -10% | -30% | **+10.0%** | +0.25pp |
| **MRVL** | +50% | +12% | -15% | -40% | -60% | **+1.0%** | +0.25pp |

**计算明细（NVDA为例）：** 0.22×40 + 0.33×22 + 0.25×5 + 0.15×(-25) + 0.05×(-50) = 8.8 + 7.26 + 1.25 - 3.75 - 2.5 = **+10.06%** → 上修至+11.5%（含Rubin交付+FY2027收入超预期期权价值）

**关键变化vs Round 2：**
- 金发姑娘概率上调2pp：CapEx加速到$1T+比Round 2预期更强，需求验证（backlog $1.45万亿）提供了硬数据支撑
- 基准偏牛下调2pp：利率转向加息预期+FCF崩溃从"风险因子"变为"正在发生"，部分抵消CapEx加速利好
- 熊市和黑天鹅维持：结构性风险未变

---

## 7. 退场标准 K1-K8（Round 3状态）

| 编号 | 标准 | 触发条件 | Round 3状态 | 距离触发 | 备注 |
|------|------|---------|------------|---------|------|
| **K1** | 核心逻辑失效 | ASIC份额连续2Q停滞/下降 | **远离触发** | 安全 | ASIC份额加速增长（Amazon $20B、Google TPU v8、Meta定制ASIC） |
| **K2** | CapEx周期逆转 | Hyperscaler削减AI CapEx>10% | **远离触发（反向！）** | 极安全 | CapEx不仅没削减，还在上修（合计$710-725B→2027 $1T+） |
| **K3** | 技术替代 | 光计算/模拟计算/LPU突破 | **未触发** | 安全 | 无重大突破 |
| **K4** | Neocloud信用风险 | CoreWeave违约或H100<$1.0/hr | **接近监控** | ⚠️ 中度风险 | CoreWeave DDTL 4.0关闭（正面），但$4.2B再融资墙到期2026；GPU抵押债务结构风险积累 |
| **K5** | API定价战 | 任两家同季度API降价>50% | **未触发** | 安全 | API价格仍在下降但未到>50%单季降幅 |
| **K6** | NVIDIA收入减速 | DC增速连续2Q<30%或环比下降 | **远离触发** | 极安全 | Q1 FY2027 DC +92% YoY；Q2指引$91B（+95%） |
| **K7** | CoWoS利用率下降 | <85%或交期<3月 | **远离触发** | 安全 | 利用率满载，订单排至2027+ |
| **K8** | AI应用ROI失败 | F500 AI预算连续2Q下降/AI融资>30%降幅 | **未触发** | 安全 | 企业AI支出$120万→$700万/年仍在增长；AI融资维持高位 |

**退场状态总结：8项标准无一触发。K2（CapEx削减）和K6（NVDA减速）处于"反向触发"状态——即条件非但没恶化，反而比Round 2更远离触发线。唯一需要监控的是K4（Neocloud），CoreWeave $4.2B再融资墙是2026下半年需要关注的信用事件。**

---

## 8. 时间维度

### 已发生事件（06.05-07.10窗口内）

| 日期 | 事件 | 影响 |
|------|------|------|
| 06.01 | 美国宣布AI芯片禁运适用于中国境外中企 | 地缘升级——出口管制范围扩大 |
| 06.03 | Alphabet $85B股权增发投资者说明会（含Berkshire $10B） | 融资渠道验证——超额认购 |
| 06.10 | 台湾考虑收紧AI芯片对华出口管制 | 地缘升级——供应链分化加速 |
| 06.11 | CoBank发布报告"AI CapEx周期可能仍在早期" | 三方验证周期未见顶 |
| 06.17 | FOMC 12-0维持3.50-3.75%，市场定价10月加息25bp | 利率环境恶化——关键转折 |
| 06.29 | JPMorgan上调AI CapEx预测至2030年（Fortune报道） | 2027 $1T+预测获得顶级投行背书 |
| 07.01 | Meta宣布建设云业务出售过剩AI算力 | Meta从"纯内部消费"转向"云服务商"——ROI路径多元化 |
| 07.04 | 内存价格 surge 开始降温（Tom's Hardware） | memflation见顶信号——但AI需求仍推高Q3价格 |

### 即将到来的催化剂（07.10-08月）

| 时间窗口 | 事件 | 重要性 | 关注点 |
|---------|------|--------|--------|
| **07.28-29** | FOMC会议（无dot plot） | 高 | 是否释放加息信号？9月dot plot前瞻 |
| **07下旬-08上旬** | Hyperscaler Q2 2026财报（MSFT/GOOGL/META/AMZN） | **极高** | Q2 CapEx实际值、2026全年指引是否再次上修、**2027年首次正式指引** |
| **08中下旬** | NVIDIA Q2 FY2027财报 | **极高** | 验证$91B指引、Rubin首批交付、FY2028展望 |
| **09.16** | FOMC + dot plot | 高 | 利率路径终极信号——是否正式定价加息周期 |
| **Q3 2026** | Broadcom Q3 FY2026财报 | 高 | AI收入$10.7B指引是否达成、FY2027 SAM更新 |

### 关键时间节点判断

**未来4-6周（07.10-08月底）是本课题的核心验证窗口。** Hyperscaler Q2财报+NVIDIA Q2财报将共同决定：
1. CapEx是继续加速还是开始减速（直接关系K2）
2. NVIDIA DC收入增速能否维持>80%（直接关系K6）
3. 2027年$1万亿CapEx预测是否获得Hyperscaler正式指引背书

---

## 9. 来源清单

### CapEx / Hyperscaler财报
1. Microsoft FY26 Q3 Earnings Call (04.29.2026) — CapEx $31.9B, FY2026 $190B指引
   - https://www.microsoft.com/en-us/investor/earnings/fy-2026-q2/press-release-webcast
2. Alphabet Q1 2026 Results (04.29.2026) — Revenue $109.9B, Cloud $20B (+63%), CapEx $180-190B
   - https://www.sec.gov/Archives/edgar/data/1652044/000165204426000043/googexhibit991q12026.htm
3. Alphabet Investor Presentation (06.03.2026) — $85B equity raise, 2027 "significantly increase"
   - https://blog.google/alphabet/investor-presentation-june-2026/
4. Meta Q1 2026 Results (04.29.2026) — Revenue $56.3B (+33%), CapEx $125-145B
   - https://investor.atmeta.com/investor-news/press-release-details/2026/Meta-Reports-First-Quarter-2026-Results/
5. Amazon Q1 2026 Results (04.29.2026) — Revenue $181.5B, AWS $37.6B (+28%), CapEx $200B
   - https://cdn.yahoofinance.com/prod/sec-filings/0001018724/000101872426000012/amzn-20260331xex991.htm
6. BofA Global Research — Hyperscaler CapEx >$800B (2026), >$1T (2027)
   - https://www.tradevae.com/news/economy/bofa-sees-hyperscaler-ai-spending-reaching-1-trillion-by-2027/
7. Moody's Ratings — CapEx forecast $785B (2026), ~$1T (2027), up $85B from March
   - https://computeforecast.com/news/hyperscaler-capex-forecast-2026-moody-785-billion-trillion-2027/
8. American Century — 7-company CapEx $775B (2026), +78% YoY
   - https://www.americancentury.com/insights/hyperscaler-ai-capex-spending-cycle/
9. CoBank (06.11.2026) — "AI CapEx cycle may just be beginning"
   - https://www.cobank.com/knowledge-exchange/why-the-ai-capex-cycle-may-just-be-beginning
10. Analysis Atlas — "$710B Year" detailed breakdown
    - https://analysis-atlas.com/research/hyperscaler-ai-capex-2026/
11. CNBC (02.06.2026) — "$700B AI spending, FCF taking big hit"
    - https://www.cnbc.com/2026/02/06/google-microsoft-meta-amazon-ai-cash.html
12. Fortune (06.29.2026) — JPMorgan raised AI CapEx forecast through 2030
    - https://fortune.com/2026/06/29/ai-spending-boom-accelerates-big-tech-trillion-infrastructure-qualcomm-cfo/

### 利率 / 宏观
13. Advisor Perspectives (06.18.2026) — Fed June 17 decision, 12-0 hold, market prices October hike
    - https://www.advisorperspectives.com/dshort/updates/2026/06/18/feds-interest-rate-decision-june-17-2026
14. CNBC (07.06.2026) — 10Y UST at 4.469%
    - https://www.cnbc.com/2026/07/06/us-treasury-yields-investors-look-ahead-to-fomc-meeting-minutesu.html

### 电力 / 能源
15. Digital Applied — 9-18 GW shortage by 2027
    - https://www.digitalapplied.com/blog/ai-infrastructure-energy-crisis-9-18-gigawatt-shortage
16. Carnegie Endowment (06.2026) — Hyperscaler nuclear commitments vs energy realities
    - https://carnegieendowment.org/research/2026/06/beyond-the-hype-assessing-hyperscaler-nuclear-commitments-against-us-energy-realities

### 存储 / 内存
17. Tom's Hardware (07.04.2026) — Memory price surge cooling, AI demand still climbing Q3 2026
    - https://www.tomshardware.com/pc-components/ram/memory-price-surge-begins-to-cool-as-consumers-hit-affordability-limit-ai-demand-still-keeps-dram-and-nand-prices-climbing-through-q3-2026
18. IDC — Global memory shortage crisis 2026
    - https://www.idc.com/resource-center/blog/global-memory-shortage-crisis-market-analysis-and-the-potential-impact-on-the-smartphone-and-pc-markets-in-2026/

### Neocloud / 私募信用
19. CoreWeave Investor Relations — $8.5B DDTL 4.0 closure (first investment-grade GPU-backed financing)
    - https://investors.coreweave.com/news/news-details/2026/CoreWeave-Closes-Landmark-8-5-Billion-Financing-Facility-Achieving-First-Investment-Grade-Rated-GPU-backed-Financing/default.aspx
20. Dave Friedman Substack — CoreWeave $4.2B refinancing wall due 2026
    - https://davefriedman.substack.com/p/where-gpu-debt-starts-to-break
21. Quartz — GPU-collateralized debt risks explained
    - https://qz.com/gpu-collateralized-debt-ai-neocloud-coreweave-financing-risks-050526

### 地缘 / 中美
22. Congress.gov CRS Report R48642 — US export controls, Huawei Ascend guidance
    - https://www.congress.gov/crs-product/R48642
23. Al Jazeera (06.01.2026) — US ban applies to Chinese firms outside China
    - https://www.aljazeera.com/economy/2026/6/1/us-says-ban-on-ai-chip-shipments-applies-to-chinese-firms-outside-china
24. Taipei Times (06.10.2026) — Taiwan mulls curbs on AI chip exports to China
    - https://www.taipeitimes.com/News/biz/archives/2026/06/10/2003858815

### 供应链
25. Medium / Adnan Masood — Semiconductors 2026: AI upswing meets structural bottlenecks
    - https://medium.com/@adnanmasood/semiconductors-in-2026-the-ai-driven-upswing-meets-structural-bottlenecks-3568b004905b
26. Fusion WW — CoWoS/HBM/3nm constraints through 2027
    - https://info.fusionww.com/blog/inside-the-ai-bottleneck-cowos-hbm-and-2-3nm-capacity-constraints-through-2027
27. Deloitte China — Global semiconductor sales $975B (2026)
    - https://www.facebook.com/deloittechina/posts/

---

*Researcher C 报告完成 — 2026.07.10*
*等待Researcher A（基本面）和B（催化剂）的交叉验证*
