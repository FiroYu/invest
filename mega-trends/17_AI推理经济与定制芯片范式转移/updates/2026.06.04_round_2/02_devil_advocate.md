# 魔鬼辩护人：议题#17 投资论点反面分析

> 对"AI推理经济与定制芯片范式转移"核心假设H1-H5的系统性质疑
> 生成日期：2026.06.04

---

## 一、反方论据汇总（对H1-H5逐个反驳）

### H1反驳：定制ASIC推理份额将从~10%增长到2028年~30-40%

**反方立场：ASIC份额增长被高估，时间线可能推迟至2029-2030年**

**论据1 — ASIC项目失败率极高，hyperscaler自研芯片屡屡延期** 【证据强度：中】

AnySilicon的行业分析总结了ASIC项目的7大失败模式：规格不稳定即启动、验证工作量被低估、技术选型先于约束理解、NRE成本被低估、制造/测试/bring-up被推迟考虑、决策权不清、commitment缺乏检查点。这些失败模式不仅存在于小公司——Google TPU从v5到Ironwood跨越了多代，每代间隔约2年；Amazon Trainium 2比计划推迟约6个月量产。定制芯片从设计到量产的周期（18-24个月）意味着任何当前的design win要到2027年才能反映在收入中。

**论据2 — NVIDIA软件生态（CUDA）的护城河比预期更深** 【证据强度：强】

CUDA生态经过10+年积累，拥有数百万开发者和大量优化库。Hyperscaler虽然自研ASIC，但内部仍有大量工作负载依赖CUDA。迁移成本不仅是软件重写，还包括调试工具、性能调优知识、以及人才储备。Google内部都有团队在TPU和GPU之间切换使用。这意味着即使硬件就绪，软件迁移也会拖慢ASIC渗透速度。

**论据3 — Broadcom/Marvell客户集中度极高，单一客户流失即致命** 【证据强度：强】

- Broadcom的AI收入极度依赖3个客户（Google、Meta、OpenAI），其中Google TPU占大头。Marvell则高度依赖Amazon AWS。Gotrade分析指出，Broadcom约70%的定制AI加速器市场份额看似领先，但多源采购趋势已经出现——2026年Marvell获得了Google TPU的部分设计合同，打破了Broadcom的垄断。
- 如果任何一个hyperscaler推迟下一代芯片计划（如Meta因AI ROI不佳削减MTIA投入），对应ASIC供应商的收入预期将大幅下调。
- Marvell市占率从12%降至8%的预期已经反映市场对其执行力的担忧。

**论据4 — Hyperscaler可能选择"GPU+少量ASIC"的混合策略而非全面转向ASIC** 【证据强度：中】

CNBC 2025年11月报道，所有hyperscaler都在同时采用GPU和自研芯片的双轨策略。AWS明确采用"混合"方案——开发Trainium的同时深度绑定NVIDIA。Microsoft Azure同样如此。这意味着ASIC可能不会替代GPU，而是作为补充。如果推理负载中只有特定类型（如大规模batch推理）适合ASIC，那么30-40%的份额上限可能偏高。

---

### H2反驳：CoWoS产能瓶颈持续至2027年，封装议价权维持

**反方立场：CoWoS瓶颈可能提前缓解，封装议价权正在被侵蚀**

**论据1 — TSMC CoWoS产能扩张速度超预期** 【证据强度：中】

背景包承认Morgan Stanley已将CoWoS月产能从~10万片上调至12-13万片（上调20%+），良率>98%。TSMC还在持续增加CoWoS产线。历史上看，半导体产能瓶颈通常在2-3年内被解决（如2018-2021年的8寸晶圆短缺、2020-2022年的汽车芯片短缺）。如果CoWoS月产能到2027年达到20万片+，瓶颈将不复存在。

**论据2 — 替代封装技术正在追赶** 【证据强度：弱】

三星的I-Cube4、Intel的Foveros Direct、以及中国本土的先进封装方案都在快速追赶。虽然目前CoWoS在性能上领先，但封装技术不像EUV光刻那样有绝对的专利壁垒。一旦替代方案达到"够用"水平，TSMC的定价权就会被削弱。

**论据3 — 良率>98%说明技术已趋成熟，产能爬坡将加速** 【证据强度：中】

高良率意味着CoWoS已经从"技术挑战"转变为"规模制造"问题。历史上，半导体制造环节一旦进入高良率阶段，产能扩张通常呈指数级加速。这与H2"瓶颈持续至2027"的假设矛盾——如果良率已>98%，瓶颈更可能在中期（2026H2-2027）缓解。

---

### H3反驳：推理token成本年降10x持续，推动AI应用商业化

**反方立场：推理成本下降是双刃剑，可能毁灭硬件厂商的定价权**

**论据1 — LLMflation正在毁灭硬件供应商的利润空间** 【证据强度：强】

a16z的"LLMflation"分析确认了推理成本每年下降约10x。GPT-4等效性能的推理成本从2021年的$60/million tokens降至当前的$0.40/million tokens。但这意味着：
- 2023年花$100万购买的推理容量，2026年只需$1,000即可获得
- 硬件供应商必须每代产品提供10x性能提升才能维持定价
- 这种通缩速度远超任何硬件技术曲线的改善速度

如果推理成本持续以10x/年下降，那么到2028年，当前$700B的AI CapEx所建设的推理基础设施的商业价值将被稀释99.9%。这是不可持续的——硬件投资无法跟上软件优化的速度。

**论据2 — 推理成本下降主要由软件/算法优化驱动，而非硬件进步** 【证据强度：强】

Weighty Thoughts的分析指出，AI推理价格暴跌主要是软件故事而非硬件故事——量化（INT8/INT4/FP8）、蒸馏、稀疏注意力、speculative decoding等算法优化贡献了大部分成本下降。这意味着即使没有新一代ASIC/GPU，推理成本也会大幅下降。硬件投资的价值因此被进一步稀释。

**论据3 — "Jevons悖论"可能不适用于推理** 【证据强度：中】

背景包隐含假设"推理成本下降→推理需求增长→硬件需求增长"（类似Jevons悖论）。但AI推理不是煤炭——当推理免费时，用户不会无限增加使用量。Gartner预测2030年前LLM推理成本再降90%，但如果杀手级AI应用始终未能出现（目前仅23%的GenAI采用者报告可衡量的收入提升或成本下降，42%的公司放弃了大部分AI项目），需求可能不会随价格下降而无限增长。

**论据4 — API定价战已导致推理服务商亏损** 【证据强度：中】

Per-token价格在3年内下降了1000x，而总AI基础设施支出增长320%（SoftwareSeni 2025年报告）。这种"量增价跌"的模式意味着推理服务商正在打价格战——这正是商品化的典型特征。当价格接近边际成本时，推理将变成无差异化的commodity，对Broadcom/Marvell的定制芯片定价权构成致命打击。

---

### H4反驳：NVIDIA推理端护城河弱于训练端，中期面临份额侵蚀

**反方立场：NVIDIA的护城河被低估，份额侵蚀速度远慢于预期**

**论据1 — NVIDIA单季$75.2B数据中心收入证明GPU绝对主导** 【证据强度：强】

背景包自身承认NVIDIA单季度数据中心收入$75.2B，说明GPU短期内绝对主导。这个收入规模相当于Broadcom全年AI收入的数倍。如果NVIDIA推理护城河真的弱，其收入增速应该已经在放缓——但2026年NVIDIA仍在快速增长。

**论据2 — NVIDIA通过生态锁定（CUDA+NVLink+网络）构建了全栈护城河** 【证据强度：强】

NVIDIA不仅仅卖GPU——它卖的是GPU+NVLink+InfiniBand/Spectrum-X网络+CUDA生态的完整解决方案。hyperscaler自研ASIC只能替代GPU本身，但还需要解决网络互联问题（这正是NVIDIA NVLink的优势领域）。2026年NVIDIA对Marvell的$20亿战略投资（共同开发NVLink兼容互联和光学DSP）表明，NVIDIA正在将潜在竞争者纳入自己的生态系统。

**论据3 — Hyperscaler自研芯片的ROI未必优于直接采购GPU** 【证据强度：中】

定制芯片需要巨额NRE投入（单颗先进制程ASIC的NRE可达$5000万-$1亿）、18-24个月的开发周期、以及持续的迭代投入。如果NVIDIA每代产品提供3x性能提升，那么自研芯片在tape out时可能已经落后于NVIDIA的最新产品。只有Google（TPU已迭代到v7/Ironwood）证明了长期自研的可行性，其他hyperscaler仍在早期阶段。

---

### H5反驳：GPU算力2027-2028可能从稀缺转向过剩

**反方立场：GPU过剩已经在发生，比预期更早更严重**

**论据1 — H100租赁价格已暴跌70-80%，过剩信号明确** 【证据强度：强】

- H100租赁价格从2023年的$8-16/GPU-hr降至2024年8月的$1-2/GPU-hr（拍卖价），降幅达70-80%。
- 2025年H100 Rental Index继续下降：从2024年9月的$3.06降至2025年6月的$2.36（23%降幅）。
- 2026年5月市场数据显示：A100起价$0.78/hr，H100起价$1.38/hr。
- 收回成本的盈亏平衡点在$2.85/GPU-hr——当前价格已经低于这个水平，意味着新进入者正在亏损运营。

这不仅是"价格正常化"，而是明确的产能过剩信号。当H100在$1.38/hr出租时，购买H100的投资回报率已经低于股票市场平均回报。

**论据2 — 供给反应速度远超需求增长（历史教训）** 【证据强度：强】

Fabricated Knowledge的电信泡沫分析指出：电信时代光纤容量在7年内增长了186,000倍，而需求只增长了约100倍。到2002年，仅2.7%的光纤被实际使用。

AI基础设施可能正在重演这一模式。NVIDIA将产品发布节奏从每2年一代加速到每年一代（Hopper→Blackwell→Rubin），加上AMD/Intel/Google/Amazon的替代产品同时涌入市场，供给的复合增长率可能远超AI推理需求的增长。

**论据3 — Neocloud的脆弱性可能引发供给海啸** 【证据强度：强】

7gc&co的分析详细揭示了neocloud（CoreWeave、Lambda Labs等）的系统性风险：
- CoreWeave 62%的收入来自单一客户Microsoft
- CoreWeave通过GPU作为抵押品获得$100亿+债务融资
- NVIDIA持有CoreWeave 5%+股权并承诺$63亿的云服务采购——这是典型的vendor financing循环
- 如果neocloud因需求不足而被迫清算GPU库存，将在二手市场释放大量廉价算力，进一步压低租金

**论据4 — 开源模型降低了对高端GPU的需求** 【证据强度：中】

Llama 3、DeepSeek等开源模型使大多数企业可以通过fine-tuning（而非从头训练）满足需求。Fine-tuning只需要1-4个H100节点，而从头训练需要16+节点。这种需求结构的变化直接减少了高端GPU的需求量。

---

## 二、最可能失败模式 Top 3

### 失败模式 #1：AI CapEx超级周期提前终结（"电信泡沫2.0"）

**描述**：Hyperscaler集体意识到AI ROI不及预期，同时削减CapEx指引，引发半导体全链条重估。

**触发条件**：
- 2个以上hyperscaler在同一季度下调AI CapEx指引超过15%
- NVIDIA数据中心收入连续2个季度环比下降
- AI应用层迟迟无法证明商业化路径（当前仅23%的GenAI采用者有可衡量的ROI）
- OpenAI等AI公司融资困难（HSBC预测OpenAI到2030年仍不盈利，资金缺口$2070亿）

**传导路径**：
1. OpenAI/Claude等AI应用公司增长放缓或融资受阻
2. Microsoft/Amazon/Google下调云基础设施需求预期
3. Hyperscaler集体削减2027-2028 CapEx指引（从~$700B降至~$400-500B）
4. NVIDIA数据中心收入增速从+100%骤降至负增长
5. Broadcom/Marvell的ASIC订单被推迟或取消
6. TSMC CoWoS利用率从>95%降至<70%
7. Neocloud（CoreWeave等）因债务无法偿还而被迫清算GPU资产
8. AI半导体板块整体PE从40x+压缩至20x以下

**概率估计**：25-30%（2027年底前发生）

**关键区别于2000年**：核心hyperscaler（Amazon、Microsoft、Alphabet）资产负债表健康、无净债务、有多元化现金流，因此不会出现电信泡沫式的系统性崩溃。但neocloud和边缘参与者（Oracle、OpenAI）的脆弱性可能引发局部危机。

---

### 失败模式 #2：推理商品化压垮硬件厂商定价权（"通缩陷阱"）

**描述**：推理token价格以每年10x的速度下降，导致硬件投资回报率持续恶化，最终使定制ASIC项目失去经济合理性。

**触发条件**：
- 推理API价格在12个月内再降90%+
- AI推理市场CR5（前5名市占率）超过80%，形成寡头定价
- 开源模型性能追平闭源模型，推理变成无差异化服务
- Hyperscaler内部自研芯片成本低于向Broadcom/Marvell采购

**传导路径**：
1. 软件优化（量化/蒸馏/稀疏化）持续推动推理成本10x/年下降
2. API定价战加剧（OpenAI vs Anthropic vs Google vs 开源）
3. 推理利润率从40%+压缩至10%以下
4. Hyperscaler要求Broadcom/Marvell下一代芯片价格下降50%+
5. ASIC供应商毛利率从60%+降至40%以下
6. 定制芯片NRE无法被摊薄，新项目ROI转负
7. Broadcom/Marvell估值从30x+ EV/EBITDA重估至15-20x

**概率估计**：20-25%（2028年底前显现）

**反驳点**：推理需求可能呈超线性增长（Jevons悖论），推理模型（chain-of-thought）使每查询token消耗增加10-100倍。但"量增价跌"的商品化陷阱在光伏、LCD面板等行业反复出现过——最终结果通常是全行业利润率被压缩至资本成本水平。

---

### 失败模式 #3：地缘政治冲击TSMC供应链（"台湾断供"）

**描述**：台海紧张局势升级导致TSMC先进制程/CoWoS产能中断，AI芯片供应链全面瘫痪。

**触发条件**：
- 台海军事封锁或隔离（RAND研究指出台湾供应链在2027年前对此特别脆弱）
- 美中技术脱钩急剧升级（60%+关税、全面技术封锁）
- TSMC被迫中断先进制程出货

**传导路径**：
1. TSMC先进制程（3nm/2nm）和CoWoS产能中断
2. NVIDIA、Broadcom、Marvell全部依赖TSMC先进制程，无替代方案
3. AI芯片出货量在3-6个月内下降80%+
4. 全球AI基础设施建设暂停
5. NVIDIA收入暴跌、Broadcom/Marvell定制芯片项目无法tape out
6. 美国AI战略受重创，CHIPS Act产能远未成熟（2028年前无法替代TSMC）
7. AI半导体板块出现恐慌性抛售

**概率估计**：10-15%（未来3年），但影响是灾难性的

**缓解因素**：TSMC正在亚利桑那建设先进制程产能，但CoWoS产能迁移更困难，且美国产能规模远小于台湾。Intel的代工业务尚未证明可替代TSMC的先进制程能力。

---

## 三、历史类比

### 类比1：2000年电信泡沫与光纤过度投资

**相似度评估：高（60-70%）**

| 维度 | 电信泡沫（1996-2002） | AI基础设施（2023-2026?） |
|------|----------------------|-------------------------|
| 需求叙事 | "互联网流量每100天翻倍"（WorldCom，后被证伪） | "AI推理需求指数增长"（部分真实，但可能高估） |
| CapEx规模 | 峰值$213B/年（调整通胀），累计>$500B，占GDP 1.0-1.2% | 2025年$405B，2026年~$700B，占GDP 1.28%——已超过电信泡沫峰值 |
| 供给反应 | 光纤容量7年增长186,000倍，仅2.7%被使用 | GPU性能每代3x+，产品节奏从2年加速至1年 |
| 投资者行为 | 电信公司通过capacity swap、vendor financing、equity cross-holdings虚增收入 | Neocloud通过GPU抵押债务、NVIDIA vendor financing循环、equity交叉持有 |
| 杠杆水平 | 极高，WorldCom负债$300亿+，行业平均D/E极高 | 核心hyperscaler D/E仅0.23（低），但neocloud/Oracle高杠杆 |
| 崩溃触发 | 美联储加息（5.5%→7%）、需求不及预期、会计丑闻 | 尚未出现明确触发因素 |

**关键教训**（来自Fabricated Knowledge / 7gc&co分析）：

1. **供给总是超调**：电信时代的光纤供给增长比需求快1000倍以上。AI芯片的供给反应速度（NVIDIA年更节奏+AMD/Intel/Google/Amazon并行投入）可能正在复制这一模式。

2. **循环投资结构是脆弱的**：电信泡沫的核心问题是capacity swap和vendor financing创造了虚假需求。当前AI生态中，NVIDIA投资CoreWeave→CoreWeave购买NVIDIA GPU→GPU作为抵押品获得贷款→贷款购买更多GPU的循环，与Lucent/Nortel的vendor financing高度类似。

3. **但有关键差异**：核心hyperscaler（Amazon/Microsoft/Alphabet）资产负债表健康、有真实的多元化收入、使用自由现金流而非债务投资。这降低了系统性崩溃的风险——7gc&co的分析认为，如果AI投资失败，核心hyperscaler可以吸收损失并继续运营，而neocloud和边缘参与者将首当其冲。

**核心结论**：AI CapEx占GDP比例已超过电信泡沫峰值，但杠杆水平显著更低。"电信泡沫2.0"不太可能以系统性崩溃的形式重演，更可能是边缘参与者（neocloud、Oracle、OpenAI）的局部危机传导至整个板块的估值重估。

---

### 类比2：2018年加密货币挖矿芯片泡沫

**相似度评估：中（40-50%）**

| 维度 | 加密挖矿泡沫（2017-2018） | AI芯片周期（2023-2026?） |
|------|------------------------|-------------------------|
| 需求驱动 | 比特币/以太坊价格暴涨→挖矿需求飙升 | AI应用爆发→训练/推理需求飙升 |
| GPU价格 | 2017-2018年GPU价格翻倍，游戏玩家无法买到 | 2023年H100炒至$8+/hr |
| 供给反应 | 挖矿专用ASIC（比特大陆等）迅速取代GPU | Hyperscaler自研ASIC可能取代通用GPU |
| 崩溃 | 2018年加密货币价格暴跌→GPU挖矿收入降至$0→NVIDIA加密相关GPU销售暴跌94% | ??? |
| 余波 | 大量二手GPU涌入市场，NVIDIA库存积压 | H100租赁价格已从$8降至$1.38/hr |

**关键教训**：

1. **NVIDIA曾在类似场景中遭受重创**：2018年Q2，NVIDIA加密相关GPU销售暴跌94%，公司被迫承认"加密货币繁荣对业务的影响超出预期"。这表明NVIDIA对终端需求的可见性有限，且"一次性需求"的消退可以极其突然。

2. **专用芯片替代通用芯片的速度可以很快**：比特币挖矿从CPU→GPU→ASIC只用了约3年。AI推理从GPU→ASIC的过渡可能也很快——但关键区别是，AI推理的多样性远高于比特币挖矿（后者的算法完全固定），这使ASIC替代的速度可能更慢。

3. **资产贬值是残酷的**：2018年加密泡沫破裂后，大量挖矿GPU以30-50%的折扣涌入二手市场，直接冲击了NVIDIA的新品销售。当前H100租赁价格暴跌80%可能导致类似的资产减值——尤其是对neocloud这类以GPU为抵押品的公司。

---

### 类比3（补充）：光伏产业的大规模产能过剩与通缩（2010-2013）

**相似度评估：中（40%）**

光伏产业在2010-2013年经历了严重的产能过剩：中国制造商（尚德、英利、天合光能）大规模扩产，导致光伏组件价格在3年内下降60%，全球产能利用率降至50%以下。最终结果是多晶硅价格从$400/kg跌至$16/kg，数十家公司破产，幸存者的利润率被永久压缩。

AI推理市场可能面临类似的"通缩陷阱"——供给快速增加（NVIDIA+AMD+Google+Amazon+Broadcom+Marvell同时扩产），而需求虽然增长但可能不及供给增速。推理token价格3年下降1000x的趋势与光伏组件价格的暴跌轨迹惊人相似。

---

## 四、对退场标准的补充建议

### 现有退场标准K1-K3的不足

| 现有标准 | 缺陷 |
|---------|------|
| K1 ASIC份额连续2季度停滞 | 过于滞后——当份额数据确认时，股价可能已调整30%+ |
| K2 Hyperscaler削减CapEx>20% | 阈值过高——10%的削减就足以引发板块重估 |
| K3 新架构突破 | 过于模糊——缺乏可量化的触发条件 |

### 建议新增退场/预警标准

**K4：Neocloud信用风险触发（预警级）**

| 条件 | 触发行动 |
|------|---------|
| CoreWeave或主要neocloud出现债务违约/重组 | 立即评估vendor financing循环风险，减仓受影响的ASIC/GPU标的 |
| H100/H200租赁价格跌破$1.0/GPU-hr | 触发GPU过剩模式评估，审视持有GPU租赁相关标的的仓位 |

**K5：推理API定价战升级（预警级）**

| 条件 | 触发行动 |
|------|---------|
| OpenAI/Google/Anthropic中任意两家在同一季度将API价格下调超过50% | 评估推理商品化对ASIC/GPU定价权的传导影响 |
| 推理API价格降至$0.05/million tokens以下 | 触发"通缩陷阱"模式评估，降低ASIC供应商仓位 |

**K6：NVIDIA推理收入占比下降（核心级）**

| 条件 | 触发行动 |
|------|---------|
| NVIDIA数据中心收入增速连续2季度低于30%（当前~100%） | 这将是最直接的"AI CapEx降温"先行指标 |
| NVIDIA单季度DC收入环比下降 | 高度预警——历史上半导体周期拐点通常伴随环比下降 |

**K7：TSMC CoWoS利用率降至85%以下（核心级）**

| 条件 | 触发行动 |
|------|---------|
| TSMC CoWoS月度利用率从>95%降至<85% | 说明供给已开始超过需求，封装瓶颈正在缓解 |
| CoWoS交期从>6个月缩短至<3个月 | 封装议价权消失的前兆 |

**K8：AI应用层ROI验证失败（预警级）**

| 条件 | 触发行动 |
|------|---------|
| Fortune 500企业AI预算占比连续2季度下降 | 需求端萎缩的先行指标 |
| AI初创公司融资规模季度环比下降>30% | 说明投资者对AI商业化失去信心 |
| Gartner将"AI应用采用率"从乐观预测下调 | 官方承认AI应用商业化不及预期 |

### 退场优先级排序

1. **K6（NVIDIA收入减速）** — 最直接、最可量化、最高频数据
2. **K7（CoWoS利用率）** — 产业链最关键瓶颈的实时指标
3. **K2修订版（CapEx削减>10%即预警）** — 下调原阈值
4. **K4（Neocloud风险）** — 系统性风险的先行指标
5. **K5（API定价战）** — 推理商品化的直接证据

---

## 五、数据来源

### 核心研究与分析

1. **Fabricated Knowledge** — "Lessons from History: The Rise and Fall of the Telecom Bubble" (2023.10) — 电信泡沫与AI基础设施的详细历史对比分析
2. **7gc&co** — "AI Capex and the Telecom Bubble: A Comparative Analysis" (2025.12) — 最全面的AI CapEx与电信泡沫对比研究，包含neocloud风险分析
3. **AnySilicon** — "7 Reasons ASIC Projects Fail" — ASIC项目失败模式行业分析

### 市场数据

4. **NVIDIA PE Ratio** — Public.com, FullRatio, Macrotrends (2026.06) — NVDA当前P/E约34-41x，12个月均值46x，10年均值54x
5. **H100 Rental Index** — Silicon Data, Introl, ThunderCompute (2025-2026) — H100租赁价格从$8/hr降至$1.38/hr
6. **a16z** — "Welcome to LLMflation" — 推理成本每年下降约10x的数据和分析
7. **Gartner** — "LLM inference costs to fall 90% by 2030" (CloudFest报道)
8. **SoftwareSeni** — "The AI Inference Market in 2025" — 推理token价格3年下降1000x，总支出增长320%

### 公司与行业分析

9. **Gotrade** — "Broadcom vs Marvell: Custom AI Silicon Battle 2026" (2026.04) — 两大ASIC供应商的竞争格局、客户集中度风险
10. **CNBC** — "Nvidia Blackwell, Google TPUs, AWS Trainium: Comparing top AI chips" (2025.11) — Hyperscaler芯片策略对比
11. **Trefis/Forbes** — Marvell vs Broadcom valuation analysis — 客户集中度和估值差异分析
12. **PANews/Techub News** — "The price plummeted by 70%. How did the AI computing power rental bubble burst?" — H100市场供需分析

### 地缘政治风险

13. **RAND Corporation** — "Supply Chain Interdependence and Geopolitical Vulnerability" — 台湾半导体供应链脆弱性分析
14. **ScienceDirect** — "Taiwan's semiconductor industry and geopolitical challenges" (RC Liu, 2025) — 2027年前台湾供应链对隔离的脆弱性
15. **Stimson Center** — "Why Taiwan Fears 'America First' Risks Eroding Its 'Silicon Shield'" (2025) — 美国onshore制造对台湾"硅盾"的潜在影响

### 历史数据

16. **Ars Technica** — "Cryptocurrency boom, a problem for gamers" (2018.02) — 2018年加密货币GPU泡沫
17. **CNBC** — "This chart shows how cryptocurrency mining on your own is no longer profitable" (2018.11) — 加密挖矿利润归零
18. **MarketWatch** — "A crypto-influenced boom amid a chip shortage? Sounds familiar" (2021) — NVIDIA历史上的加密相关收入波动

### AI应用层数据

19. **7gc&co** (同上) — 仅23%的GenAI采用者报告可衡量的ROI，42%的公司放弃了大部分AI项目
20. **HSBC** — OpenAI预计到2030年仍不盈利，资金缺口$2070亿

---

*本报告仅从反面视角分析投资风险，不代表看空结论。所有假设和预测均基于当前可得信息，可能随新数据出现而调整。*
