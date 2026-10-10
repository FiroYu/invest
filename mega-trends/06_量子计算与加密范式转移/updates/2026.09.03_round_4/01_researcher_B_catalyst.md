# 催化剂研究员（研究员B）独立研究报告

> 课题: #06 量子计算与加密范式转移
> 分析日期: 2026-10-10 | 角色: catalyst（技术里程碑、政策、监管事件）
> 捕获窗口: 2026-07-10 → 2026-10-10；搜索源: WebSearch（Nature/arXiv/白宫/监管/币媒）

---

## 一、核心发现（Top 3）

1. **量子纠错在 9 月出现「里程碑群」——逻辑比特竞赛从 50 量级跳向效率竞争。** (a) **Infleqtion 30 逻辑比特/仅 80 物理原子**（9/24，Sqale 中性原子平台，NYSE: INFQ）——编码效率 ~2.7:1，为商业机器上中性原子路线首次；口径注记：依赖 error detection（非完整纠错）。(b) **Iceberg Quantum+Diraq qLDPC 演示**（9/15）：qLDPC 架构+硅 CMOS 自旋比特实现 10x 纠错效率提升——qLDPC 从理论走向硬件验证（IBM Starling 的核心架构假设同步受益）。(c) **LUMI-IQ 蓝图**（9/11）：芬兰 Kajaani 2029 年底建成欧洲首台国家级容错超导量子计算机的完整纠错路线图。**(d) IBM Nighthawk r2 实时错误解码 100K circuits/s**（9/9，提前达标 2026 roadmap）。**方向判读**：行业重心从「逻辑比特数量」转向「编码效率+实时解码」——这是通往 2029 容错（Starling 200 逻辑比特）的正确斜率。

2. **IBM 9/23 arXiv RCS 量子优势论文（2609.28657）= 条件 #1 的「预兑现」。** IBM+UChicago 在超导处理器（61/120 比特 Nighthawk r2、36 层深度）上宣称随机电路采样优势：19 秒生成 100 万样本，宣称领先经典超算无法实际复现。**三点保留**：(i) RCS 是「采样优势」非「实用优势」（Google 2019 先例，后被算法压缩削弱）；(ii) 论文为 arXiv 预印本，IBM 自己要求的「community-verified」标准尚未完成；(iii) 经典模拟追赶历史上多次反超（JUPITER 50Q 等）。**但事件本身的信号意义**：管理层选择在 Summit（~11 月）前 6 周放论文=对 11 月宣布的信心路标。T3（Summit 无宣布→IBM 下调）触发概率下降。

3. **Q-Day 叙事在 10 月出现「监管级」升级：Europol 双报告（10/7）+Glassnode 链上数据（6.26M BTC 暴露）+ETH 研究员「bunker mode」呼吁——威胁对象被权威重新定义为「钱包而非链」。** Europol EC3 结论：加密货币不会因量子计算崩溃，但**公钥已上链的地址是暴露点**；Glassnode：~6.26M BTC（31.2% 供应）处于此类地址；Justin Drake（ETH 基金会）呼吁行业提前规划「bunker mode」迁移。**白宫 10/8「Science: A New Golden Age」峰会**另含 $215M 量子专项（总 $6B 科学计划）。这组事件把 Q-Day 从「学术估算」推进到「监管机构的威胁建模」——T4（RSA 破解预测 <10 年）未触发，但**PQC 迁移的社会紧迫性定价在上升**（确定性层逻辑的免费期权）。

---

## 二、逐项分析

### D6：PQC 政策执行（H1）

- EO 14412（PQC 强制）/EO 14413（量子创新）6/22 签署后进入执行期：M-26-15 要求联邦机构 120 天内交迁移计划（≈10 月下旬首批到期）——**本轮信息截止日恰在首批计划提交窗口**，未检索到系统性延期报道=按期推进假设维持。
- NIST FIPS 206（ML-DSA 补充变体）草拟中（R3 载录），无新发布。
- 执行面信号：Zscaler/Cloudflare 等合规产品营销全面 PQC 化；银行端（BIS 2026 报告）继续「评估中」。**H1 维持通过，无新催化亦无回撤**。

### D7：加密监管（关联 #09）

- **CLARITY Act 9/15 参院程序性投票失败**（未过 60 票门槛）——Trump 先在 9/14 让步伦理条款试图救票未果；BTC 当日从近 $80K 跌至 $76.9K（Coindesk 实时报道）；Polymarket 年内立法概率一夜腰斩。
- 对本课题含义：(i) 美国加密监管框架继续悬置→量子-加密交叉产品（QRL 类抗量子链、量子安全托管）的合规路径不明，投机热度受抑；(ii) BTC $76-84K 区间（10/8 blockchain.com $83.8K——周内反弹）高波动≠趋势。**中性偏负，无操作含义**。

### D1 补充：IonQ 技术事件线（与 A 报告财务线互补）

- 9/23 实时量子错误解码器测试+Superion 集成消息（盘前 +12%）。
- SkyWater 交割（7/31）=「首个垂直整合全栈量子平台」公司口径；DARPA HARQ/DOE/SDA 合同管线延续（R3 载录）。

### D3 补充：IBM Summit 前瞻

- 瑞士 System Two（9/10，ETH Zurich+Lockheed Martin）扩张安装基数；Nighthawk r2 云上线（9 月）。
- 若 Summit 宣布「独立验证的实用量子优势」→ 条件 #1 达成 → 升级讨论启动；若仅重复 RCS 叙事 → T3 部分触发（路线图未后撤则 IBM 配置不下调，只冻结加仓）。

---

## 三、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|------|------|------|:-----------:|
| H1 PQC 确定性 | 成立 | M-26-15 首批计划 10 月下旬到期，无延期报道 | 5 |
| H2 硬件 roadmap | **成立（上修）** | 里程碑群（Infleqtion/Iceberg-Diraq/Nighthawk r2/RCS 论文）；重心转向效率与实时解码=正确斜率 | 4 |
| H3 IonQ 商业化 | 成立 | 技术事件流+合同管线延续 | 4 |
| H4 估值承受利率 | 不成立 | 见 A/C 报告（本报告视角：估值事件全部被利率环境压制，10/1 单日板块 -3~5%） | 4 |
| H5 Q-Day 时间表 | 成立但紧迫性上移 | Europol/Glassnode/Drake=监管级威胁建模启动；破解时间表未前移（仍 15 年+） | 4 |

## 四、情景分析

| 情景 | 概率 | 核心驱动 | 时间 |
|------|:----:|---------|------|
| Goldilocks | 13% | Summit 独立验证+M-26-15 按期+FIPS 206 发布 | 11 月-12 月 |
| Moderate（主） | 47% | 优势声明但验证渐进；PQC 执行按部就班 | 持续 |
| Winter | 30% | Summit 无宣布+利率 >5.5%+锁定期抛售 | Q4-Q1 |
| Q-Day 定价 | 10% | 更多监管机构跟进 Europol 口径；BTC 侧抗量子迁移争议公开化 | 2027 |

## 五、时间维度

- **短期（1-3 月）**：IBM Summit（~11 月）；IONQ Q3（~11 月）；M-26-15 首批迁移计划审计（10 月下旬-11 月）；QNT 锁定期前窗口。
- **中期（3-12 月）**：FIPS 206；Nighthawk→Loon 路线节点；CHIPS $20.13 亿正式协议（LOI→definitive）。
- **长期（1-3 年）**：Starling 2029；PQC 2030/2031 联邦截止；抗量子 BTC 迁移争论（BIP 流程）。

## 六、关键来源

- postquantum.com（9/24）：Infleqtion 30 逻辑比特；cryptobriefing（Sqale 80 原子）
- kickhammernews（9/15）：Iceberg Quantum+Diraq qLDPC 10x 效率
- techtimes（9/11）：LUMI-IQ 芬兰容错蓝图（Kajaani 2029）
- GCN（9/9）：Nighthawk r2 100K circuits/s 提前达标；arXiv 2609.28657（9/23）；CiVL（61 比特/19 秒/100 万样本）
- IBM Newsroom（9/10）：ETH Zurich System Two+Lockheed Martin
- Europol EC3（10/7）双报告：钱包而非链为暴露点（tradingview/cryptobriefing/ethnews 转载）
- Glassnode（10 月）：6.26M BTC（31.2%）公钥暴露；mpost.io
- blockchainreporter：Justin Drake「bunker mode」
- Coindesk（9/14-15）：CLARITY Act 参院失败+BTC $76.9K；Polymarket 概率腰斩
- cryptotimes.io（10/9）：白宫 $6B 科学计划含 $215M 量子专项
- White House：EO 14412/14413+M-26-15（R3 载录，执行期）

---

*本报告为独立研究，未参考其他研究员结论。*
