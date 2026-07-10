# 宏观/竞争格局研究 — #09 稳定币与数字货币基础设施革命

> **研究员**：C 宏观/竞争格局 | **轮次**：R3（2026.07.10）| **基线**：R2（2026.05.25）
> **覆盖**：UST 需求冲击 / 银行存款外流 / 美元数字霸权 / 市场规模与估值 / 风险矩阵
> **数据时点**：2026 H1（截至 2026.07.09）

---

## 1. 执行摘要

R3（07.10）较基线（05.25）的核心增量：**合规化进入实质落地期，但竞争格局剧变**。

1. **GENIUS 实施规则进入 NPR 阶段**（OCC/FDIC/Fed 三机构联合，评论期 05.01 截止，下一里程碑 08.04）。最终规则未落地但方向已锁：1:1 储备、PPSI（合规发行人）纳入 BSA 金融机构、**禁止支付型稳定币付息**。
2. **市场规模超基线**：总市值 ~$308–321B（ATH $318.6B @ 04.11），+34% YoY，已突破基线的 $290B。USDT $184–188B（~63%），USDC $73.3B（~25%）。链上交易量记录 $1.79T（2026.06，+63% MoM）。
3. **国库券需求冲击**：实证确认存在但**当前量级被高估**。BIS WP #1270 实测稳定币流入压低 3M T-bill 收益率 0.71 bps（即时）/ ~4 bps（10 日内）。Kansas City Fed：市场需达 $900B（较当前 +180%）才有"实质影响"。当前 ~$230B T-bill 持仓 < UST 市场的 2%，影响可忽略。
4. **银行存款外流**：仍为情景假设而非已实现事实。BPI 模型显示 $4T 稳定币场景下存款 -19%、贷款收缩；State Street 估算 $2T 场景侵蚀 $1.2–2.5T 放贷能力。但 GENIUS 禁止付息的条款**显著缓冲了存款迁移动力**。
5. **竞争格局黑天鹅（新）**：2026.06，Stripe/Visa/Mastercard 被曝联合筹建稳定币平台，剑指 Circle/Tether（Forbes："可能击沉 Circle"）。这是 R3 最重要的结构性变化——**支付巨头亲自下场，发行人溢价面临挤压**。
6. **美元数字霸权强化**：USD 稳定币占全球 ~$315B 市场的 ~98%。e-CNY/mBridge 反击（$55.49B 交易量，e-CNY 占 95.3%），但 Foreign Policy（06.24）与 PIIE 判断"去美元化撞墙"。

**评级影响**：维持"积极关注"，但**确定性从"发行人"层向"支付集成/基础设施"层迁移**。Circle（CRCL）估值风险显著上升（IPO $31 → 峰值 $263 → 现 ~$80，-23.5%/周），Visa/Stripe 联合体是结构性威胁。Tether 合规化进展（四大审计、$141B UST）降低了即时黑天鹅概率但未消除。

---

## 2. 国库券需求冲击宏观分析

### 2.1 实证证据：影响存在但当前量级有限

| 研究 | 来源 | 量化结论 | 时点 |
|------|------|---------|------|
| **BIS WP #1270**（Ahmed）| BIS | 稳定币流入压低 3M T-bill 收益率 **0.71 bps（即时）**，**~4 bps（10 日内）**；被引 77 次 | 2025 |
| SSRN 定价模型 | 学术 | $3.5B 稳定币流入 → 3M T-bill 收益率 -2.5~5 bps | 2025 |
| Kansas City Fed | 美联储 | 市场需达 **$900B**（较当时 +260%）才有"实质影响" | 2025 |
| Brookings | 智库 | 确认结构性 bid，但当前占比 <2% UST 市场 | 2025 |
| Oxford Academic（Yadav）| 学术 | 短端券发行结构反过来也助推稳定币扩张 | 2025 |

**关键判断**：基线 "$900B 需求冲击" 是 **TBAC 建模的上限值**，对应稳定币市值需达 $900B（当前 $310B，需再涨 ~180%）。当前阶段（~$230B T-bill 持仓）对短端利率的影响处于**统计可测但宏观可忽略**的区间（几个 bps）。

### 2.2 对收益率曲线与货币政策传导

- **短端下行压力**：稳定币发行人是 T-bill 的"永久性买方"（1:1 储备要求），创造结构性 bid。随市值向 $1T+ 演进，将**系统性压低短端收益率**（2Y 及以内），加剧收益率曲线陡峭化压力。
- **Fed 货币政策传导的新通道**：
  - ECB WP（Burlon et al.）证实稳定币**改变政策利率向银行资金成本的传导**。
  - Liang（2026）/ Barbon（2025）发现**政策利率与链上稳定币借贷利率之间存在"持续性脱节"**——Fed 降息/加息不能 1:1 传导到 DeFi/稳定币收益率，形成传导漏损。
  - GENIUS 允许央行储备 backing 稳定币（Fed Notes 2026.03），意味着 ON RRP 设施可能成为稳定币储备的合规去向，**反向强化 Fed 对短端的控制**。
- **Fed 资产负债表约束**：Anbil（Fed, 2026）提出回购市场容量成为资产负债表规模的新约束。稳定币储备若大规模涌入 repo/RRP，将影响 Fed 缩表（QT）的终点判断。

### 2.3 情景推演（更新基线表）

| 阶段 | 稳定币市值 | T-bill 需求 | 短端利率影响 | 状态 |
|------|-----------|------------|-------------|------|
| 当前（2026 H1）| ~$310B | ~$230–250B | <5 bps，可忽略 | **已证实** |
| 中期（2027–2028）| $500B–1T | $400–800B | 10–30 bps 下行压力 | TBAC/Citi base |
| 长期（2029–2030+）| $1.6–1.9T（Citi base）| $800B–1.6T | 显著结构性需求，可能扭曲短端定价 | 预测 |

**跨议题传导**：与 #20（日本通缩终结/全球利率）高度相关——若稳定币以万亿美元级吸纳短端 UST，将**压低全球短端利率锚**，叠加 AI CapEx（#01）的长期融资需求，形成"短端被压、长端被拉"的曲线形态。

---

## 3. 银行存款外流实证

### 3.1 仍为情景假设，非已实现事实

| 机构 | 场景 | 存款影响 | 放贷能力影响 |
|------|------|---------|------------|
| **BPI** | 基准增长 | **-10%** 存款 | 资金成本 +24 bps |
| **BPI** | $4T 稳定币 | **-19%** 存款 | 贷款对应收缩 |
| **State Street** | $2T（主要源自存款）| — | **-$1.2~2.5T** 放贷能力 |
| **Fed Notes**（2025.12）| 情境依赖型 | 取决于稳定币需求**来源**与转换的资金类型 | 不确定 |
| **White House**（2026.04）| 禁止付息 vs 允许付息 | 禁止付息显著缓冲存款迁移 | — |

**关键缓冲因素**：
1. **GENIUS 禁止支付型稳定币付息**——若无收益，用户迁移存款的动力大幅削弱（银行存款有 FDIC 保险 + 可能的利息）。
2. **银行入场**：若银行发行自有稳定币，存款只是"形式变化"（活期 → 银行稳定币），**仍在银行体系内**，不构成系统性外流（Fed Notes 2025.12 的核心论点）。
3. **M2 影响**：取决于储备存放地——存商业银行（M2 中性）vs 存央行（M2 收缩）。

### 3.2 监测指标

- **M2 存款成分月度增速**（频度：月）
- **银行稳定币牌照申请数**（若 JPM/BAC 发行，外流风险转为企业内迁移）
- **GENIUS 实施规则是否允许"收益型稳定币"**（最大变量——BPI/银行游说团体正推动维持禁令）

---

## 4. 美元数字霸权 vs 去美元化

### 4.1 美元稳定币：数字美元化引擎

- **市场份额**：USD 稳定币 = ~98% 的 ~$315B 全球市场（SEC/CoinGecko）。
- **战略意图**：GENIUS 法案被哥伦比亚大学 CER 定性为"**数字化主导地位**"——通过合规化在数字世界锁定美元优势。
- **IMF 背书**：Hélène Rey（IMF F&D 2025.09）论证美元稳定币可**强化美国"世界银行家"资产负债表**，帮助稳定美国外部赤字融资。
- **新兴市场美元化实证**：
  - 阿根廷、土耳其、尼日利亚、越南——美元稳定币已成为事实上的价值存储与抗通胀工具。
  - 学术（Murakami 2025）：新兴市场"数字美元化"通过消费平滑**提升福利**。

### 4.2 去美元化反击：e-CNY / mBridge / BRICS

| 维度 | 数据 | 评估 |
|------|------|------|
| e-CNY 规模 | ~3.5B 笔交易，16.7 万亿元（截至 2025.11）| 国内为主 |
| mBridge | 交易量 **$55.49B**（较 2022 早期试点 +2,500 倍）；e-CNY 占 **95.3%** | 批发跨境赛道崛起 |
| 2026 框架 | 升级版数字元管理框架 **2026.01.01 生效** | 制度推进 |
| BRICS 协调 | "BRICS Neutral Digital" 架构提案（新德里宣言 2026）| 仍在构想 |

**但去美元化动能受阻**：
- **Foreign Policy（2026.06.24）**："中国的去美元化驱动撞墙了"——PBOC 行长 06.17 公布新蓝图，但动能停滞。
- **PIIE（2026）**：甚至认为"中国放弃了国家支持的数字现金"，美国和欧洲应警觉反向信号。
- **结构性原因**：美元稳定币是**市场自发 + 合规背书**的全球扩张；e-CNY 是**自上而下、资本管制约束**的受控体系。前者侵略性远强于后者。

**判断**：美元数字霸权在 R3 进一步巩固。e-CNY 在 mBridge 批发端有局部突破，但零售/消费端美元稳定币的渗透速度与规模压倒性领先。**去美元化叙事在 R3 从"威胁"降级为"长期存在但动能衰减"。**

---

## 5. 市场规模与估值

### 5.1 TAM 预测分歧（2030）

| 来源 | 2030 市值（存量）| 2030 支付流量 | 备注 |
|------|----------------|-------------|------|
| **Citi GPS（base）**| **$1.6–1.9T** | — | 机构基准 |
| Citi GPS（bull）| $4T | — | 激进情景 |
| Digital Dollar Report | $3.7T | — | 行业乐观 |
| **Bloomberg Intelligence**| — | **$56.6T** | 流量口径 |
| Chainalysis（2025 实绩）| — | $28T（2025）| 已超 Visa 量级 |
| Artemis（2025 实绩）| — | $33T（+72% YoY）| — |
| Juniper（汇款）| — | P2P 汇款 >$10B（2030）| 细分 |

**当前市值**：~$308–321B（ATH $318.6B @ 04.11.2026，+34% YoY）。向 Citi base case（$1.6–1.9T）需 5x+，年化增速需 ~40%+。

### 5.2 份额结构（2026.07）

| 稳定币 | 市值 | 份额 | 趋势 |
|--------|------|------|------|
| **USDT（Tether）**| $184–188B | **~63%** | 份额稳定，合规化推进 |
| **USDC（Circle）**| $73.3B | **~25%** | 交易量追赶（06 月 $1.79T 记录）|
| USDS（Sky Dollar）| $11B | ~3.8% | — |
| DAI | $4.6B | ~1.6% | 衰退 |
| 其他 | — | ~6% | — |

USDT+USDC ≈ **88%** 双寡头。

### 5.3 估值

| 标的 | 价格（07.09）| 市值 | 估值指标 | 核心驱动 |
|------|------------|------|---------|---------|
| **Circle（CRCL）**| ~$80（峰值 $263，-23.5%/周）| ~$32B（峰值 FD）| 公允价值估 $35.82（Yahoo）；共识 PT $137.12 | 净息差（USDC 储备利息）；**Visa/MC/Stripe 联合体是结构性威胁** |
| **Coinbase（COIN）**| ~$158.75 | ~$41.7B | P/E ~60x | FY25 营收 $7.2B（+9.4%），稳定币收入 **$1.4B/年**（$364M Q4）；2026 ~$7B（趋平）|
| **Robinhood（HOOD）**| — | — | FY25 营收 +52%，但**加密收入 -47%**（高波动）| 加密弹性 vs 可预测性 |

**发行人盈利模式**：净息差（Net Interest Margin on Reserves）——稳定币发行人将 1:1 美元储备投入 T-bill/RRP，赚取利差。
- **利率敏感型**：降息周期直接压缩发行人利润（Circle 对利率高度敏感）。
- **规模经济**：随市值增长，边际成本趋零。
- **风险**：Visa/Mastercard/Stripe 自建稳定币 → 若支付巨头吃下结算层，发行人沦为"商品化管道"，净息差被竞争压薄。

**Circle 估值警示**：IPO $31（06.2025）→ 首日飙至 $123 → 峰值 $263 → 现 ~$80。**已回吐大部分 IPO 后涨幅**。Yahoo 公允价值估算 $35.82 暗示当前价被高估 ~55%。下次财报 2026.08.11 是关键验证点。

---

## 6. 风险矩阵

| 风险 | 概率 | 影响 | 时点 | 迹象/证据 |
|------|------|------|------|----------|
| **Tether 黑天鹅** | 中→低（下降）| 极高（60% 份额）| 持续 | 四大审计（KPMG/PwC）+ $141B UST + $8.23B 缓冲**降低**即时风险；但 USAT 子公司"围栏"结构使 $183B 离岸 USDT 游离于 GENIUS 之外（Forbes 05.2026）；Sen. Reed S.3907 试图堵漏 |
| **监管反复/收紧** | 中 | 高 | 2026.08 后 | NPR 评论期已收，08.04 下一里程碑；银行游说团体（BPI）推动维持"禁止付息"条款——若通过，抑制增长但利好银行体系稳定 |
| **支付巨头挤压私人稳定币** | **高（新）** | 高（发行人）| 已发生（06.2026）| **Stripe/Visa/Mastercard 联合筹建稳定币平台**（CoinDesk 06.03；Forbes 06.11 "可能击沉 Circle"）——这是 R3 最重要的结构性变化 |
| **银行稳定币挤压** | 中 | 中 | 2026 H2–2027 | BPI 成员（JPM/BAC/Citi）通过游说积极参与规则制定；但 GENIUS 实施细则未定，银行尚未正式发行 |
| **技术（链分叉/黑客）** | 低 | 中 | 持续 | 主流链（ETH/SOL）未发生系统性事件；NY Fed（06.2026）警示"合成稳定币"金融稳定风险 |
| **地缘（制裁/OFAC）** | 中 | 中 | 持续 | 美元稳定币强化美元霸权，OFAC 合规通过链上 AML（Chainalysis/TRM）逐步嵌入；去美元化阵营动能衰减 |
| **利率下行压缩发行人利润** | 高（周期）| 中 | 2026–2027 | Fed 降息周期直接压缩净息差——Circle 估值对利率最敏感 |

**头号风险（R3 更新）**：从基线的"Tether 黑天鹅"调整为**"支付巨头（Visa/MC/Stripe）自建稳定币挤压发行人溢价"**——这是已发生、高概率、且直接影响 Circle（占 ~25% 市场份额的合规标杆）的结构性威胁。Tether 黑天鹅概率下降（四大审计 + 储备透明度改善）但仍为尾部风险。

---

## 7. 投资逻辑分层（评级影响建议）

### 7.1 确定性层（核心配置）

| 主题 | 标的 | 逻辑 | 风险 |
|------|------|------|------|
| **支付网络集成** | Visa (V)、Mastercard (MA) | 支付巨头"转型而非受损"——自建稳定币结算层 + 前端卡网络护城河；**从"潜在受损"转为"受益方"** | 传统收单费率长期承压 |
| **国库券储备受益** | BlackRock (BLK) | BUIDL 链上国库券基金 + 全球最大资管，稳定币储备管理的天然管道 | 直接 UST 需求影响有限（长期主题）|
| **托管基础设施** | State Street (STT)、Fidelity (FNF) | 稳定币储备托管 + 资产服务 | 商品化竞争 |

### 7.2 弹性层（精选配置）

| 主题 | 标的 | 逻辑 | 风险 |
|------|------|------|------|
| **合规发行标杆** | Circle (CRCL) | 合规化最大受益者，但**估值已透支**（现 ~$80 vs 公允 $35.82）| **高**——Visa/MC/Stripe 联合体挤压 + 利率下行 + IPO 后波动 |
| **交易所+L2 生态** | Coinbase (COIN) | USDC 收入分成（$1.4B/年）+ Base L2 + 交易所弹性 | P/E ~60x，2026 营收趋平；加密周期性 |
| **跨境支付** | Wise (WISE)、Stripe（私有）| 稳定币作为后端结算降本 | Stripe 已亲自下场发币，既是受益方又是竞争方 |

### 7.3 投机/规避层

| 主题 | 标的 | 逻辑 |
|------|------|------|
| **Tether 尾部对冲** | （非上市）| 风险下降但仍占 60% 份额；USAT 离岸结构是隐患；Sen. Reed S.3907 是催化剂 |
| **做空传统汇款** | 避免 Western Union (WU)、MoneyGram | 商业模式被稳定币直接颠覆（成本 6–10% vs <1%）|
| **银行转型** | JPM、BAC（长期观察）| GENIUS 实施后银行稳定币落地时点未定 |

### 7.4 评级影响结论

- **维持"积极关注"**，但**确定性重心迁移**：从基线的"合规发行人"层（Circle/USDC）向"支付集成/基础设施"层（Visa/MC/BlackRock）转移。
- **新增核心判断**：支付巨头自建稳定币是 R3 最重要的结构性变化——Visa/Mastercard 从"潜在受损"升级为"转型受益方"，应从"风险标注"提升为"确定性配置"。
- **Circle 估值预警**：当前 ~$80 仍显著高于公允价值估算 $35.82，叠加利率下行与竞争挤压，短期估值风险高于基线。建议**等待 08.11 财报与 08.04 GENIUS 实施里程碑后再评估**。
- **Tether 风险降级**：从基线"头号黑天鹅"下调——四大审计 + $141B UST + $8.23B 缓冲改善透明度；但 USAT 离岸结构是残余隐患。

---

## 8. R3 关键监测清单

| 信号 | 指标 | 频度 | 阈值 |
|------|------|------|------|
| GENIUS 最终规则 | 08.04 里程碑 / OCC-FDIC-Fed 联合发布 | 持续 | 是否允许付息（最大变量）|
| 支付巨头联合体落地 | Stripe/Visa/MC 稳定币正式发布 | 持续 | 是否开放/许可制、链选择 |
| Circle 财报 | 08.11 发布 | 季度 | 净息差变化、市值增速 |
| 稳定币总市值 | DefiLlama | 周 | 向 $400B 突破则确认加速 |
| T-bill 持仓 | 稳定币发行人储备披露 | 月 | 向 $300B+ 突破则短端影响实质化 |
| 银行稳定币牌照 | JPM/BAC/Citi 申请状态 | 持续 | 任一大型银行正式发行则格局重塑 |

---

## 来源索引

**UST 需求冲击**
- [Kansas City Fed — $900B 阈值分析](https://www.kansascityfed.org/research/economic-bulletin/stablecoins-could-increase-treasury-demand-but-only-by-reducing-demand-for-other-assets/)
- [BIS Working Paper #1270（Ahmed 2025）— 收益率影响量化](https://www.bis.org/publ/work1270.pdf)
- [Brookings — Treasury 市场影响](https://www.brookings.edu/articles/the-rise-of-stablecoins-and-implications-for-treasury-markets/)
- [Oxford Academic（Yadav 2025）](https://academic.oup.com/jiel/article/28/4/665/8439773)

**银行存款外流**
- [Fed Notes — Banks in the Age of Stablecoins（2025.12）](https://www.federalreserve.gov/econres/notes/feds-notes/banks-in-the-age-of-stablecoins-implications-for-deposits-credit-and-financial-intermediation-20251217.html)
- [BPI — Risks from Allowing Stablecoins to Pay Interest](https://bpi.com/the-risks-from-allowing-stablecoins-to-pay-interest/)
- [State Street — Interest-bearing stablecoins & macro stability](https://www.statestreet.com/br/en/insights/stablecoins-macroeconomic-stability)
- [ECB OP353 — Toss a Stablecoin to Your Banker](https://www.ecb.europa.eu/pub/pdf/scpops/ecb.op353~11120d3428.en.pdf)
- [White House — Effects of Stablecoin Yield Prohibition on Bank Lending（2026.04）](https://www.whitehouse.gov/wp-content/uploads/2026/04/Effects-of-Stablecoin-Yield-Prohibition-on-Bank-Lending.pdf)

**美元霸权 / 去美元化**
- [IMF F&D（Hélène Rey 2025.09）— Stablecoins, Tokens, and Global Dominance](https://www.imf.org/en/publications/fandd/issues/2025/09/stablecoins-tokens-global-dominance-helene-rey)
- [Columbia CER — GENIUS Act 强化美元霸权](https://cer.econ.columbia.edu/news/digitalizing-dominance-how-genius-act-reinforces-us-dollar-hegemony)
- [Atlantic Council — e-CNY 2026 展望](https://www.atlanticcouncil.org/blogs/econographics/what-to-watch-as-china-prepares-its-digital-yuan-for-prime-time/)
- [Foreign Policy（2026.06.24）— 中国去美元化撞墙](https://foreignpolicy.com/2026/06/24/china-dollar-dedollarization-yuan-renminbi-brics-finance-banks-sanctions/)
- [PIIE（2026）— China gives up on state-backed digital cash](https://www.piie.com/blogs/realtime-economics/2026/china-gives-state-backed-digital-cash-us-and-europe-should-take-note)
- [Euromoney — mBridge 去美元化](https://www.euromoney.com/article/2dd0z8ym848elao2gar5s/fintech/could-china-led-wholesale-cbdc-fuel-de-dollarization/)

**市场规模 / 估值**
- [Citi GPS — Stablecoins 2030](https://www.citigroup.com/rcs/citigpa/storage/public/GPS_Report_Stablecoins_2030.pdf)
- [Chainalysis — 2025 $28T 支付流量](https://www.chainalysis.com/blog/stablecoin-utility-future-of-payments/)
- [Bloomberg Intelligence — $56.6T by 2030（Yahoo）](https://finance.yahoo.com/news/stablecoins-hit-56t-valuation-2030-090407498.html)
- [DefiLlama — 市值数据](https://defillama.com/stablecoins)
- [CoinDesk（2026.07.06）— USDC 交易量 $1.79T 记录超越 Tether](https://www.coindesk.com/business/2026/07/06/circle-s-usdc-is-leaving-tether-behind-in-the-stablecoin-volume-race)
- [Reuters — Circle 上市峰值 $32B FD](https://www.reuters.com/business/stablecoin-firm-circle-scales-record-high-after-blockbuster-nyse-listing-2025-06-06/)
- [Yahoo Finance — CRCL 估值分析](https://finance.yahoo.com/markets/stocks/articles/circle-internet-group-crcl-valuation-180833121.html)
- [Robinhood — COIN 数据](https://robinhood.com/us/en/stocks/COIN/)

**Tether 风险 / GENIUS 实施**
- [Forbes（2026.05.27）— Tether USAT 围栏结构](https://www.forbes.com/sites/digital-assets/2026/05/27/tethers-usat-exists-so-usdt-never-has-to-comply/)
- [Forbes（2026.04.18）— GENIUS 合规细则被忽视](https://www.forbes.com/sites/digital-assets/2026/04/18/everyone-celebrated-the-genius-act-nobody-read-the-compliance-section/)
- [Sen. Reed S.3907 — Foreign Stablecoin Transparency Act](https://www.reed.senate.gov/news/releases/reed-seeks-to-close-alarming-loophole-in-genius-act)
- [OCC Bulletin 2026-3 — NPR](https://www.occ.gov/news-issuances/bulletins/2026/bulletin-2026-3.html)
- [FDIC — NPRM GENIUS Act](https://www.fdic.gov/news/financial-institution-letters/2026/notice-proposed-rulemaking-establish-genius-act)
- [Fed Notes（2026.03.30）— Payment Stablecoins & Cross-Border](https://www.federalreserve.gov/econres/notes/feds-notes/payment-stablecoins-and-cross-border-payments-benefits-and-implications-for-monetary-policy-20260330.html)
- [Chapman — GENIUS Rulemaking Tracker](https://www.chapman.com/publication-genius-act-rulemaking-tracker)

**支付集成（R3 关键变化）**
- [CoinDesk（2026.06.03）— Stripe/Visa/Mastercard 联合稳定币平台](https://www.coindesk.com/business/2026/06/03/payment-giants-stripe-visa-mastercard-said-to-be-among-backers-of-soon-to-debut-stablecoin-platform)
- [Forbes（2026.06.11）— Visa/MC 稳定币可能击沉 Circle](https://www.forbes.com/sites/digital-assets/2026/06/11/why-visa-and-mastercard-are-building-the-stablecoin-that-could-sink-circle/)
- [Visa Press — Visa & Bridge 稳定币结算](https://usa.visa.com/about-visa/newsroom/press-releases.releaseId.22206.html)

---

*报告完成于 2026.07.10 | Round 3 宏观/竞争格局研究员（C）*
