# R3 基本面研究报告 — #14 电网储能与能源市场终极重构

> **研究员**：A（基本面） | **日期**：2026.07.10 | **基线**：R2（2026.05.25）
> **覆盖周期**：2026 H1（重点 5-7 月），对照基线约 6 周增量

---

## 1. 执行摘要 — 头号发现

1. **2026 部署增速放缓但仍强劲：+41% YoY（非翻倍）**。BNEF 预测 2026 全球新增 **158 GW / 459 GWh**，较 2025 年的 112 GW / 307 GWh 增长 41%。增长依然迅猛，但相比 2025 年的"翻倍"明显减速。中美欧三大市场 Q1 2026 均创同期历史新高。累计装机预计 2035 年达 2 TW / 7.3 TWh。

2. **AI/数据中心需求重塑整个逻辑——储能与燃气轮机同步爆发**。这是基线未充分预期的重大变化。GE Vernova Q1 2026 订单 $18.3B（+71% YoY），重型燃气轮机售罄至 2028 年；Siemens Energy Q2 FY26 订单创纪录 €17.7B（Gas Services +32%、Grid Tech +42%）。AI 驱动的电力需求"水涨船度"，**天然气调峰的"受损"逻辑被推迟/弱化**——至少在 2028 年前，燃气轮机与储能是互补而非替代关系。

3. **Form Energy 铁-空气电池获里程碑验证：Google $1B 订单（300 MW / 30 GWh）**。2026.02.24 公布，隐含系统成本约 **$33/kWh**（介于 $20 目标和当前 LFP ~$55-60 之间）。加上 Maine 85 MW / 8,500 MWh 项目（DOE $147M 资助）和 Georgia Power 15 MW 项目，Form Energy 已选定 JPMorgan/Jefferies 领导 IPO，将成为**首家上市的长时储能公司**。

4. **钠离子电池成本可能断崖式下降**。CATL Naxtra 钠离子电芯宣称量产成本约 **$19/kWh**（vs LFP 电芯 $55-60/kWh），能量密度达 175 Wh/kg，2026 量产。若得到独立验证，将比 LFP 低约 65%，从根本上改变储能成本曲线。但该数据为 CATL 单方宣称，BNEF 独立调查尚未覆盖钠离子。

5. **户用太阳能/储能仍处低谷，电网级大储与数据中心储能是主驱动力**。Enphase Q1 2026 营收 $282.9M（-20.6% YoY），SolarEdge 预亏；但 Fluence 创纪录 $5.6B 积压订单（超大规模数据中心驱动），Sungrow 储能毛利率 ~30%。LDES 行业分化加剧：Form Energy 独走，ESS Inc（铁液流）面临 NYSE 退市风险。

---

## 2. 2026 部署量数据（分区）

### 全球总量

| 指标 | 2025 实际 | 2026 预测 | YoY |
|------|----------|----------|-----|
| 新增 GW | 112 GW (BNEF) / 106 GW (Wood Mac) | **158 GW** (BNEF) | **+41%** |
| 新增 GWh | 307 GWh (BNEF) | **459 GWh** (BNEF) | **+49%** |
| 累计（2035E） | — | 2 TW / 7.3 TWh | 8× 2025 |

**注**：BNEF 年中展望将 2026 预测从此前 ~123 GW 上调至 158 GW（市场韧性超预期）。但增速从 2025 年的 ~23-43% 进一步放缓，**不再是"翻倍"增长**。全球 BESS 电芯出货 2025 年达 421.2 GWh（+75.5% YoY），TrendForce 预测 2026 年达 **901 GWh**（+~50%）。

### 中国（~60% 全球份额）

- Q1 2026 新增 **10.5 GW / 27.1 GWh**（其中独立储能 8.7 GW / 23.0 GWh）
- 2 月单月新增 3.56 GW / 8.19 GWh（+120% / +95% YoY）
- 累计装机已达 **213.3 GW**（+54% YoY）
- 2025 全年新增 66.4 GW / 189.5 GWh（+52% YoY）
- 2026 年 4 月中国 ESS 出货创纪录 93.1 GWh（+92% YoY）
- OEM 储能承购协议 H1 2026 为 H1 2025 的 4 倍（GWh 口径）
- 预计 2030 年超 370 GW

### 美国

- Q1 2026 安装 **3.3 GW / 8.4-9.7 GWh**（最强 Q1，+32% YoY，超上次 Q1 纪录 54%）
- 电网级占 >75%
- 太阳能+储能占 Q1 2026 新增电网容量的 **91%**
- 2026-2031 预计安装 146 GW / 499 GWh；2031 年总装机达 200 GW / 655 GWh
- Wood Mackenzie 预测未来 6 年四倍增长

### 欧洲

- 2026 年初累计 ~100 GW
- Q1 2026 电网级安装量同比翻倍以上（>6.5 GWh）
- 3 月单月部署 1.4 GW / 3.4 GWh（德国、法国、英国等）
- 德国占欧盟电池容量 ~46%
- 2026 年电池安装预计超 50 GWh（SolarPower Europe 中情景），2030 年达 138 GWh
- 2030 年预计累计超 215 GW，其中电化学 128 GW / 300 GWh

**关键信号**：欧洲正从户储向大储转型（户储 2024 见顶后回落，大储 2026 加速）。

---

## 3. 电池成本曲线 R3 更新

### 当前价格水平（2026 H1）

| 电池类型 | 电芯价格 | Pack 价格 | 来源/备注 |
|---------|---------|----------|---------|
| **LFP（磷酸铁锂）** | $55-60/kWh | — | Battery-Tech.net，大宗交易价 |
| **LFP（基线值）** | $52/kWh | — | R2 基线（2025 年值） |
| **全锂离子（加权平均）** | — | **$108/kWh** | BNEF 2025 年度调查（降 8% YoY，新纪录） |
| **钠离子（CATL Naxtra）** | **~$19/kWh**（宣称） | — | 量产成本宣称；能量密度 175 Wh/kg |
| **铁-空气（Form Energy）** | — | **~$33/kWh**（系统级） | Google $1B/30 GWh 订单隐含 |

### 成本下降驱动力

1. **锂价持续低位**：碳酸锂从 2022 年峰值 ~$80/kg 降至约 $10/kg，2026 H1 维持低位
2. **中国制造业规模效应**：CATL/BYD/EVE 主导成本曲线下移
3. **电芯能量密度提升**：LFP 从 150 Wh/kg 向 200 Wh/kg
4. **钠离子新路线**：若 CATL $19/kWh 可验证，将比 LFP 低 ~65%

### 关键判断

- **LFP 电芯 $50/kWh 关口已实质性突破**（$52-60 区间，大宗交易可低于 $50）
- **Pack 级成本仍是瓶颈**：全锂离子 pack 均价 $108/kWh，系统级（含 PCS/BMS/安装）约 $150-200/kWh
- **钠离子是最大变量**：CATL 宣称 2026 量产，BYD 同步加速部署。若 $19-40/kWh 可实现，2027-2028 年储能系统成本将再降 30-50%
- **铁-空气 $20/kWh 目标仍待验证**：Google 订单隐含 $33/kWh 高于目标，但已证明系统级成本低于 LFP 的 $55-60/kWh 电芯价

### 成本曲线对比（R2 → R3）

| 指标 | R2 基线（05.25） | R3 更新（07.10） | 变化 |
|------|-----------------|-----------------|------|
| LFP 电芯 | $52/kWh | $55-60/kWh | 持平/微升（锂价波动） |
| 钠离子电芯 | $59/kWh | **$19/kWh（CATL 宣称）** | 大幅下降（待验证） |
| 全锂离子 Pack | $115/kWh (2024 BNEF) | **$108/kWh (2025 BNEF)** | -6% |
| 铁-空气系统 | 目标 $20/kWh | **~$33/kWh（Google 订单验证）** | 首个商业化数据点 |

---

## 4. 储能公司财报对比表

### 受益方（电网级储能/电池制造商）

| 公司 | 2026 H1 关键财务 | 储能业务表现 | 评级信号 |
|------|-----------------|-------------|---------|
| **CATL (300750.SZ)** | Q1 营收 ¥129.1B（+52.45% YoY），净利 ¥20.7B（+48% YoY）；2025 储能营收 ¥59.9B；锂电销量 661 GWh（+~40%） | 储能业务强劲增长，分析师预测 2026 储能营收 ~¥85B | ⬆️ 最强受益者 |
| **Tesla (TSLA)** | Q1 2026 总营收 $22.4B（+16%），营业利润 +136% YoY；但 **Energy 部署 -15% YoY，储能营收 -12% YoY** | Megapack Q1 软，但仍是**公司最高利润率业务**；结构性受益不变 | ➡️ 短期波动，长期正面 |
| **Fluence (FLNC)** | FY26 Q2 营收 $465M（+7.7%，miss 预期 24%）；**积压订单 $5.6B（创纪录）**；FY26 指引 $3.2-3.6B | 超大规模数据中心驱动订单爆发；收入确认节奏波动 | ⬆️ 订单验证趋势 |
| **Sungrow 阳光电源 (300274.SZ)** | 2025 营收 ¥89.18B（+14.55%），净利 ¥13.46B（+22%），毛利率 31.83%；储能出货 **43 GWh**，逆变器 143 GW | 储能毛利率 ~30%（环比上升）；BNEF 可融资性第一（100%，连续 6 年） | ⬆️ 盈利稳健 |
| **GE Vernova (GEV)** | Q1 2026 营收 $5.0B（+12%），订单 $18.3B（**+71%**），Adj EBITDA +87%；指引上调至 $44.5-45.5B | 重型燃机售罄至 2028；Power Equipment 订单 +52% | ⬆️ 但来自燃气而非储能 |
| **Siemens Energy (ENR)** | Q2 FY26 订单 **€17.7B（创纪录）**，营收 €10.3B（+8.9%）；Gas Services +32%，Grid Tech +42%；book-to-bill 1.72 | 上调全年指引；$1B 美国扩产 | ⬆️ 燃机+电网双驱动 |

### 承压方（户用太阳能/储能 + LDES 二线）

| 公司 | 2026 H1 关键财务 | 状态 | 评级信号 |
|------|-----------------|------|---------|
| **Enphase (ENPH)** | Q1 2026 营收 $282.9M（**-20.6% YoY**），毛利率 43.9%；Q2 指引 $280-310M | 微逆出货 141 万台；股价创年内新低；近期复苏可见度低 | ⬇️ 户用市场低谷 |
| **SolarEdge (SEDG)** | Q1 2026 预亏 EPS -$0.24 | 持续亏损，户用太阳能承压 | ⬇️ 尚未见底 |
| **ESS Inc (GWH)** | Q1 2026 EPS -$0.54（miss 86%）；净亏 $15.9M；股价 $1.14（6 月 -75%） | **NYSE 退市风险**，权证已退市，进行反向拆股；$31M 内部人融资（2025.07）；Google-SRP 试点推迟至 2027.12 | ⬇️ 高风险 |

---

## 5. Form Energy / LDES 进度

### Form Energy（铁-空气）— R3 重大进展

| 维度 | R2 基线 | R3 更新 |
|------|--------|--------|
| 首个商业项目 | Xcel/Georgia Power 签约 | **Google-Xcel $1B 订单（300 MW / 30 GWh，Minnesota）**；Georgia Power 15 MW / 1,500 MWh（2026 上线）；Maine 85 MW / 8,500 MWh（DOE $147M） |
| 隐含系统成本 | 目标 $20/kWh（未验证） | **~$33/kWh**（Google 订单反算）— 首个真实商业化数据点 |
| 商业化时间 | 2027-2029 | 2026 首个项目上线（Georgia Power），Google 项目规模远超预期 |
| IPO | 关注时间表 | **已选定 JPMorgan + Jefferies 领导**（2026.06.17 Axios 报道），Goldman/Morgan Stanley 参与；或成首家上市 LDES 公司 |
| 技术验证 | 循环寿命/效率待验证 | 首个商业示范系统（Great River Energy）已部署；Google 订单为 10 年期长期验证提供规模 |

**关键判断**：Form Energy 从"技术概念"进入"商业验证"阶段。$33/kWh 系统成本虽高于 $20 目标，但已低于 LFP 电芯成本（$55-60/kWh），且放电时长 100 小时无竞争对手。Google $1B 订单是**长时储能行业迄今最大单笔商业验证**。

### LDES 行业分化

| 路线 | 代表企业 | R3 状态 | 评级 |
|------|---------|--------|------|
| 铁-空气 | Form Energy | $1B Google 订单 + IPO 在即 | ⬆️ 独走 |
| 铁液流 | ESS Inc (GWH) | NYSE 退市风险，反向拆股，股价 $1.14 | ⬇️ 困境 |
| 重力/氢储 | Energy Vault | $300M 投资关闭；技术多元化但商业化缓慢 | ➡️ 观望 |
| 压缩空气 | 多个项目 | 少量部署，地质条件依赖 | ➡️ 利基 |
| 抽水蓄能 | 传统 | 成熟但增量有限 | ➡️ 基线 |

**判断**：LDES 正在 Form Energy 单极化收敛。铁-空气路线如果 Google 项目成功验证（2027-2028），将主导 100 小时级长时储能。其他路线（液流/重力/压缩空气）在储能系统集成商的成本竞争中难以胜出。

---

## 6. 关键指标 R3 更新（对照 README 指标表）

| 指标 | R2 基线值 | R3 更新值 | 变化 | 评级影响 |
|------|----------|----------|------|---------|
| LFP 电芯成本 | $52/kWh (2025) | $55-60/kWh（大宗交易） | 持平/微波动 | ➡️ 中性（已过 $50 关口） |
| 全锂离子 Pack 成本 | — | **$108/kWh** (BNEF 2025) | -8% YoY | ⬆️ 持续下降 |
| 钠离子电芯成本 | $59/kWh | **$19/kWh**（CATL 宣称，待验证） | 大幅下降（若属实） | ⬆️ 重大利好（待验证） |
| 4h LFP LCOS | $100-150/MWh | 维持（LFP 成本持平） | ➡️ | ➡️ |
| 2025 全球部署 | 110 GW | **112 GW / 307 GWh** (BNEF 确认) | 微调 | — |
| 2026 全球部署预测 | — | **158 GW / 459 GWh (+41%)** | 增速放缓 | ⬇️ 不再翻倍 |
| 全球总装机 | 267 GW / 610 GWh | 持续增长（中国累计已 213 GW） | ⬆️ | ⬆️ |
| 储能市场规模 | $15.8B (2025) | $44.2B (2034E) 维持 | — | ➡️ |
| Form Energy 铁-空气 | 目标 $20/kWh | **~$33/kWh 系统级（Google 订单）** | 首个验证数据点 | ⬆️ 商业化推进 |
| 天然气调峰退役 | "面临经济性淘汰" | **推迟 — 燃机订单创纪录（AI 需求）** | 重大修正 | ⬇️ 受损逻辑弱化 |

### README 关注模型追踪

1. **电池 $/kWh 成本曲线** — LFP 持平于 $52-60；钠离子可能断崖式下降至 $19（待验证）；铁-空气首个真实数据点 $33
2. **储能部署 GW/GWh 增速** — 2026 +41%（从翻倍减速），中美欧 Q1 均创新高
3. **弃电率** — 未获取 2026 H1 新数据（建议 B 研究员补充）
4. **天然气调峰退役速度** — **重大修正**：AI/数据中心需求推动燃机订单爆发（GE Vernova +71%，Siemens Gas Services +32%），退役逻辑推迟至 2028 年后
5. **负电价小时数** — 未获取 2026 H1 新数据（建议 B 研究员补充）

---

## 7. 评级相关变化提示

### 对 R2 隐含评级（"积极关注"）的影响

**维持"积极关注"，但需调整逻辑框架：**

#### 正面因素（支持升级）
- 2026 全球部署 158 GW / 459 GWh 确认（+41%），虽减速但绝对量持续创新高
- Form Energy 铁-空气获 Google $1B 订单验证（$33/kWh 系统级），IPO 在即，LDES 从概念进入商业化
- 钠离子电芯 $19/kWh（若验证）将是成本曲线的下一个断点
- Fluence $5.6B 积压订单 + CATL Q1 营收 +52% 确认行业高景气
- 中国储能 OEM 承购 H1 2026 为去年同期 4 倍

#### 负面因素（支持审慎）
- **天然气调峰"受损"逻辑被严重弱化**：AI/数据中心需求使燃机订单创纪录（GEV 售罄至 2028），天然气并非被"挤出"而是与储能同步增长。README 中"结构性受损：天然气调峰电厂运营商"的判断需修正——至少 2028 年前，GE Vernova/Siemens Energy 是**受益者而非受损者**
- **2026 增速从翻倍降至 +41%**：虽然强劲，但减速趋势明确（2025 ~23-43% → 2026 ~41%，BNEF 预测 2027 后进一步放缓）
- **户用太阳能/储能低谷**：Enphase -20.6%、SolarEdge 亏损，户储复苏时间不确定
- **LDES 二线分化**：ESS Inc 退市风险，行业集中度加速向 Form Energy 收敛
- **钠离子 $19/kWh 为单方宣称**：BNEF 尚未独立调查钠离子价格，存在营销夸大风险

#### 逻辑框架调整建议

README 核心判断"储能成本曲线何时将化石燃料彻底挤出电力市场"需要修正为：

> **储能 + 可再生能源 vs 化石燃料的竞争，因 AI/数据中心需求爆发而延迟。2026-2028 年储能与燃气轮机互补增长（共同填补电力缺口），而非储能替代燃机。真正的"挤出"时间表推迟至 2029-2032 年（需 LFP <$40/kWh 或铁-空气 <$25/kWh + AI 需求增速放缓）。**

#### 投资含义修正

| README 原判断 | R3 修正 |
|-------------|--------|
| CATL/BYD：长期受益 | ✅ 维持 — Q1 2026 CATL +52% 营收验证 |
| Tesla Megapack：受益 | ✅ 维持（短期波动，长期最高利润率业务） |
| Fluence：受益 | ✅ 维持 — $5.6B 积压订单 |
| **天然气调峰：结构性受损** | ❌ **修正** — 2028 年前为受益者（GE Vernova/Siemens Energy 订单创纪录） |
| **GE Vernova：需关注转型** | ❌ **修正** — 燃机业务本身爆发，转型压力降低 |
| Form Energy：关注 IPO | ✅ 维持 — IPO 已选定承销商，Google $1B 订单验证 |

---

## 来源索引

### 部署量
- [BNEF: Energy Storage Enters the 100-Gigawatt Era](https://about.bnef.com/insights/clean-energy/energy-storage-enters-the-100-gigawatt-era-three-things-to-know/) (2026.05)
- [BNEF forecasts 158GW of global energy storage deployments in 2026 — Energy-Storage.news](https://www.energy-storage.news/bloombergnef-forecasts-158gw-of-global-energy-storage-deployments-in-2026/)
- [Wood Mackenzie: Global energy storage surpasses 100 GW milestone in 2025](https://www.woodmac.com/news/opinion/global-energy-storage-market-surpasses-100-gw-annual-installation-milestone-in-2025/)
- [China CNESA: February Analysis — new installations +120% YoY](http://en.cnesa.org/latest-news/2026/3/23/new-installations-surge-over-120-yoy-february-analysis-of-chinas-new-energy-storage-projects)
- [Utility Dive: US record Q1 2026 storage installations](https://www.utilitydive.com/news/us-sees-record-q1-2026-energy-storage-installations-amid-rosy-outlook/823547/)
- [SolarPower Europe: European Battery Market Outlook 2026-2030](https://www.solarpowereurope.org/insights/outlooks/european-battery-market-outlook-2026-2030-1/detail)
- [TrendForce: Global ESS cell shipment rankings Q1 2026](https://www.energytrend.com/news/20260525-51447.html)

### 电池成本
- [BloombergNEF: New Record Lows for Battery Prices](https://about.bnef.com/insights/clean-transport/new-record-lows-for-battery-prices/) (2025 survey, $108/kWh pack avg)
- [Battery-Tech.net: Sodium-ion disrupting the market in 2026](https://battery-tech.net/how-sodium-ion-technology-is-disrupting-the-global-battery-market-in-2026/) ($19/kWh Na-ion, $55-60/kWh LFP cell)
- [Council Fire: $19 sodium-ion battery cell for grid storage](https://www.councilfire.org/blog/19-dollar-sodium-ion-battery-cell-grid-energy-storage)

### 公司财报
- [CATL Q1 2026 Report (Official PDF)](https://www.catl.com/uploads/1/file/public/202604/20260415213228_0fxgc0dcvb.pdf)
- [Tesla Q1 2026 Update (Official PDF)](https://assets-ir.tesla.com/tesla-contents/IR/TSLA-Q1-2026-Update.pdf)
- [Energy-Storage.news: Tesla reports declines in energy storage revenues](https://www.energy-storage.news/tesla-reports-declines-in-quarterly-energy-storage-revenues-and-deployments/)
- [Fluence FY2025 Results & FY2026 Guidance](https://ir.fluenceenergy.com/news-releases/news-release-details/fluence-energy-inc-reports-2025-financial-results-and-initiates/)
- [GE Vernova Q1 2026 Financial Results](https://www.gevernova.com/news/press-releases/ge-vernova-reports-first-quarter-2026-financial)
- [Siemens Energy Q2 FY26 Earnings](https://www.siemens-energy.com/global/en/home/investor-relations.html)
- [Enphase Q1 2026 Financial Results](https://investor.enphase.com/news-releases/news-release-details/enphase-energy-reports-financial-results-first-quarter-2026)
- [ESS Inc Q1 2026 / Reverse Stock Split](https://essinc.com/ess-reverse-stock-split-statement/)

### Form Energy / LDES
- [Utility Dive: Google-Xcel 300 MW/30 GWh Form Energy battery](https://www.utilitydive.com/news/worlds-largest-grid-battery-part-of-google-xcel-energy-agreement/813793/) (2026.02.24)
- [Form Energy: Georgia Power 15 MW agreement](https://formenergy.com/form-energy-georgia-power-continue-forward-with-15-megawatt-iron-air-battery-system-agreement/)
- [Canary Media: Form Energy Maine world's biggest battery](https://www.canarymedia.com/articles/long-duration-energy-storage/form-energy-set-to-build-worlds-biggest-battery-in-maine)
- [Axios Pro: Form Energy selects JPMorgan/Jefferies for IPO](https://forgeglobal.com/form-energy_ipo/) (2026.06.17)
