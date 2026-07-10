# 研究员A报告 — 基本面分析

> 议题#11 先进制程GAA与半导体制造架构变革 | 2026-07-10 | Round 3
> 捕获窗口：2026-06-05 → 07-10

---

## 0. 时序说明（重要）

本轮捕获窗口恰好落在两场关键财报之间，均为 **财报前(pre-release)** 视角：
- **TSMC Q2 2026 财报**：定于 7月16日（本周四）——本轮仅有 Q1 实际 + 5月营收 + Q2 指引
- **ASML Q2 2026 财报**：定于 7月15日（本周三）——本轮仅有 Q1 实际 + 2026 上调指引
- **TSMC 6月营收**：原定 7月10日(今日)发布，截至检索时尚未在公开索引中出现

因此本轮判断以 **Q1 实际 + 指引 + 月度趋势 + 第三方产业数据** 为基础，关键财报数据(营收/HPC占比/N2营收%)留待 Round 3.5 或下一次复查补强。

---

## 1. Delta 摘要表（vs Round 2 基线 06-04）

| 变量 | 06-04 状态(R2) | 07-10 更新(R3) | 方向 | 重要性 |
|------|---------------|----------------|------|--------|
| TSMC Q2 指引 | — | $39.0–40.2B（+~10% QoQ，+~32% YoY，中位数） | 季度纪录再确认 | 高 |
| TSMC 5月营收 | — | NT$416.98B（+30.1% YoY，月度纪录） | AI需求持续 | 高 |
| TSMC Q2 财报细节 | 待出 | **7/16 发布**(本轮未及) | 待确认 | — |
| TSMC N2P | 进展中 | 量产定 2H26，目标良率~80% | 符合预期 | 中 |
| TSMC A16 | 风险产 2026Q4 | **风险生产自2026年3月起**（提前） | 略好于预期 | 中 |
| ASML Q2 财报 | 待出 | **7/15 发布**(本轮未及) | 待确认 | — |
| ASML 中国营收 | 关注中 | **Q1 2026 降至 19%**（vs 历史~33%） | 大幅下降 | 高 |
| 美国出口管制 | 不主动加新规 | **4月新法案拟限制 DUV+服务**；ASML -6% | 重新收紧 | 高 |
| Intel 18A外部客户 | 200+设计 | **NVIDIA测试后退出**（Reuters） | 重大负面 | 高 |
| Intel 14A | 0.5 PDK | 仍是 0.5；**14A-E** 面向外部，2027/28 | 无突破 | 中 |
| High-NA EUV | EXE:5200B已验收 | **TSMC确认A16/A14不用High-NA**；Intel独家 | ROI存疑加深 | 中高 |
| Samsung SF2 | 50-60%良率，$20K | 50-70%(SF2P达70%)；$20K确认 | 小幅改善 | 中 |
| WFE 2026 | $130-135B | **KLA上调至~$140B**；AMAT称增长>30% | 上修 | 高 |
| 每晶体管成本(H4) | N2仅~5%改善 | **transistors/$从562M→412M(首次倒退)** | 恶化 | 极高 |
| Chiplet替代 | 观察中 | **可降总硅成本20-35%**部分对冲 | 缓解 | 中高 |
| 设备商估值 | ASML 39x PE | **全板块PE扩张**：ASML~48x/LRCX~60x/KLAC~61x | 显著变贵 | 高 |
| Hyperscaler 2027 | 增速放缓15% | **Goldman累计$1.15T至2027；S&P预计2027单年$1T** | 持续强劲 | 高 |

---

## 2. H1–H5 逐条更新

### H1: GAA 必经之路 — 维持 95%
**强确认**。TSMC N2(已量产)/N2P(2H26)/A16(风险生产自3月起)全 GAA nanosheet；Intel 18A RibbonFET + PowerVia；Samsung SF2/SF2P。FinFET 在 3nm 以下无法缩放，chiplet 是互补路径（见 H4 缓解项）。无变化。

### H2: EUV 不可替代 — 维持 95%
**强确认，但 High-NA 出现分化**。ASML Low-NA EUV 计划 2027 年产量近翻倍（~90台），订单积压 €38B+ 创纪录。**但 High-NA EUV(EXE:5200)出现关键分化**：TSMC 公开确认 A16/A14 **不采用** High-NA，坚持 Low-NA 多重图形；Intel 成为 High-NA 唯一领先客户（已增订第二台用于 14A）。这意味着 High-NA 的 ROI 在 2027 前主要靠 Intel 一家验证，垄断地位不等于 High-NA 立即放量。整体 H2 无变化（ASML 仍垄断），但 High-NA 商业化节奏略慢于乐观预期。

### H3: 设备商确定性最高 — 维持 88%（估值风险上升）
**确认 + 上修 WFE 基本面，但估值全面变贵**。KLA Q3 FY26 营收 $3.415B(+11% YoY)，市占率 58%，将 2026 WFE 指引上调至 ~$140B；AMAT 称 WFE 增长 >30%；LRCX 预计 WFE 从 $110B(2025)→$135B(2026)。基本面强于 Round 2。**但估值风险显著上升**：LRCX 自 3/31→7/7 涨 52.7%（其中 40.9% 来自 PE 扩张），KLAC 涨 58.7%（54.4% 来自 PE 扩张）。这是"卖铲子"逻辑在周期顶部被充分定价的信号，需加强估值纪律。

### H4: 每晶体管成本下降 — 进一步下调 55% → 40%（本轮最显著弱化）
**这是本轮核心负面信号，确认 Round 2 的下调趋势延续甚至恶化：**

1. **N2 晶圆价 $30,000 确认**，较 N3($18-20K) 涨 50-66%（Phemex/Simon-Kucher/NeoGAF 多源一致）
2. **Exponential View 数据**：N2 节点每美元晶体管数从 562M 降至 **412M**——这是该指标首次出现实质性倒退
3. **TSMC 2026 对 sub-5nm 再涨价 3-5%**（已通知 Nvidia/Apple/AMD）
4. **Simon-Kucher 定性结论**："The End of Automatic Cost Decline"——自动降本时代结束
5. **未来节点趋势 $45K/wafer**，capex $28-30B/fab
6. **部分对冲**：chiplet 设计可降总硅成本 20-35%（CrispIdea）；但 CoWoS-L 封装本身 $1,000-1,100/颗（+47% premium），成本重心从晶体管缩放转向封装

**判断**：每晶体管成本"停止下降"的概率从 Round 2 的"趋近中立"进一步走向"基本确认"。N2P 即使达 80% 良率，晶圆价刚性 + 封装溢价意味着系统级降本路径已改变。K5（连续2节点上升）风险上升。建议 CIO 将 H4 下调至 40%，并将"成本重心从制程缩放转向先进封装"纳入叙事修订。

### H5: TSMC 护城河加深 — 维持 90%
**强确认**。Q2 指引 $39-40B(+32% YoY)，5月营收 NT$416.98B 月度纪录。N2 售罄至 2027Q2，N2P 2H26 量产(目标80%良率)，A16 风险生产提前至3月。**N2+CoWoS 组合成为"最难绕过的组合"**（tspasemiconductor），定价权(3-5%涨价)被客户接受。新增风险注释：HPC 客户集中度(NVIDIA Rubin 占 N2 营收~30%)上升，但暂不构成威胁。

---

## 3. 标的估值更新表（截至 2026-07-08/09）

| 标的 | 当前价 | PE(TTM) | PE(NTM/Fwd) | R2 PE | 估值变化 | 加权收益重算(R3) | R2加权 | 仓位建议 |
|------|--------|---------|-------------|-------|---------|------------------|--------|---------|
| **TSM** | ~$437 | 36.3x | **27.7x** | 23.4x(Fwd) | 变贵 | **+2.5%**（指引强但估值已折价部分） | +3.5% | 28%→**25%**(PE>40纪律逼近) |
| **ASML** | ~€1,989/ADR | ~60x | **~48x** | 39x | 显著变贵 | **-3.5%**（中国风险+估值昂贵） | -1.3% | 12%→**8%**(PE>45触发减仓) |
| **LRCX** | — | — | **~60x** | 隐含合理 | 大幅变贵 | **+4.0%**（WFE上修但PE透支上行） | +8.8% | 18%→**14%**(PE扩张过快减仓) |
| **KLAC** | ~$1,808 | 59.4x | **~61x** | 隐含合理 | 大幅变贵 | **+4.5%**（确定性最高但估值贵） | +7.3% | 15%→**12%**(PE>60减仓) |
| **AMAT** | — | 53.7x | **~38x** | ~23x | 变贵但最便宜 | **+4.0%**（WFE>30%增长最受益） | +3.8% | 10%→**12%**(加仓，估值保护最好) |
| **INTC** | ~$108-110 | 负 | **~66.7x** | 投机 | YTD+83%已大涨 | **+12.0%**（NVIDIA退出降低胜率） | +17.5% | 7%→**5%**(外部客户受挫减仓) |

**重算逻辑**：
- TSM：Bull/Base/Bear 概率维持 25/50/25，但 PE(Fwd) 从 23.4→27.7x 压缩 Bull 上行，加权 +2.5%
- ASML：中国营收降至 19% + PE 48x，Bear 概率微升，加权转负 -3.5%
- LRCX/KLAC：WFE 上修($140B)是实质利好，但 PE 扩张(60x)已透支大量上行，加权收益较 R2 下调
- AMAT：PE(Fwd) 38x 仍是设备商最便宜，WFE>30% 增长直接受益，加权略升，建议加仓
- INTC：NVIDIA 测试后退出(Reuters)是外部客户战略的实质负面，YTD +83% 已反映大量乐观，胜率下调

**新增现金释放**：减仓 TSM/ASML/LRCX/KLAC/INTC 释放约 8% 仓位，其中 2% 加仓 AMAT，6% 转现金（等 7/15-16 财报后决策）。

---

## 4. 退场标准 K1–K5 状态

| ID | 退场标准 | R2 状态 | R3 状态 | 变化 |
|----|---------|---------|---------|------|
| **K1** | TSMC N2 良率<60%持续2季度 | 未触发(65-75%) | **未触发**（N2P目标80%，量产2H26） | 无变化 |
| **K2** | ASML EUV订单积压<20台 | 未触发(45台) | **未触发**（积压€38B+，2027产量近翻倍） | 无变化 |
| **K3** | AI CapEx见顶(Hyperscaler同时削减) | 观察中 | **未触发**（2027预计$1T单年；Goldman累计$1.15T至2027） | 风险降低 |
| **K4** | TSMC先进制程市占<85% | 未触发(92%) | **未触发**（Intel外部客户受挫，NVIDIA退出18A） | 风险降低 |
| **K5** | 每晶体管成本连续2节点上升 | 未触发但趋势恶化 | **接近触发**（transistors/$ 562M→412M 首次倒退；N2确认+未来$45K） | **风险显著上升，建议升级监控** |

**K5 特别注释**：若 N2P(2H26)实际良率数据确认每晶体管成本 vs N2 不降反升，K5 将正式触发。建议下次复查(9月)将 K5 列为首要验证项。

---

## 5. 关键风险更新

| 风险 | R2 概率 | R3 概率 | 变化原因 |
|------|---------|---------|---------|
| 每晶体管成本停止下降(结构) | 35% | **45%** | transistors/$ 首次倒退；$30K→$45K 趋势确认 |
| 设备商估值回调 | 20% | **35%** | PE全面扩张(ASML 48x/LRCX 60x/KLAC 61x)，纪律触发 |
| AI CapEx崩塌 | 15% | **12%** | 2027指引持续上修($1T单年) |
| 台海危机 | 5% | 5% | 无变化 |
| Intel 14A追平TSMC | 12% | **8%** | NVIDIA退出18A；外部客户重心移至14A-E(2027/28) |
| Samsung SF2崛起 | 8% | 8% | 良率改善但仍落后；$20K定价未抢到大客户 |
| ASML中国管制升级 | — | **25%(新增)** | 4月新法案拟限DUV+服务；中国已降至19% |

---

## 6. 数据来源清单

**TSMC**
- TSMC IR Q2 2026 季度页（财报7/16）investor.tsmc.com/english/quarterly-results/2026/q2
- TSMC 5月营收 NT$416.98B(+30.1% YoY) — FocusTaiwan 2026-06-10 / TSMC PR#3320
- TSMC 2nm 技术页（N2P 2H26 量产）tsmc.com/english/dedicatedFoundry/technology/logic/l_2nm
- A16 风险生产自2026年3月 — Tom's Hardware / eeNews Europe (2026-03)

**ASML**
- ASML Q1 2026 €8.8B(+13% YoY)，2026指引上调至€36-40B — tikr.com / Stockopine (2026-04)
- ASML 中国营收 Q1 2026 降至19% — MarketWise / CNBC 2026-04-15
- ASML High-NA：TSMC 确认 A16/A14 不用 — Tom's Hardware (2026)
- ASML 2027 Low-NA EUV 产量近翻倍 — SemiWiki / tikr (2026-04)

**出口管制**
- Reuters 2026-04-03: US targets Chinese chipmaking export restrictions (ASML)
- Reuters 2026-04-07: US Congress plan restrict DUV+servicing

**Intel**
- Reuters/TechPowerUp: NVIDIA tested 18A but did not commit(退出) — techpowerup.com/344401
- Intel 14A 0.5 PDK，14A-E 面向外部 2027/28 — Intellionaire Substack Ep.24
- Intel CEO Lip-Bu Tan "going big time into 14A" — Tom's Hardware

**Samsung**
- SF2 晶圆价 $20K(vs TSMC $30K，-33%) — Reddit r/hardware / Tom's HW
- SF2 良率 50-70%(SF2P达70%) — Semicone semicone.com/article-252.html

**H4 每晶体管成本（核心）**
- Exponential View "Broken Bargain of Moore's Law"：transistors/$ 562M→412M — exponentialview.co
- Simon-Kucher "End of Automatic Cost Decline" — simon-kucher.com
- N2 $30K/wafer(+50-66% vs N3) — Phemex / NeoGAF / WCCFTech
- Chiplet 降总硅成本20-35% — CrispIdea crispidea.com
- CoWoS-L $1,000-1,100/颗(+47%) — SiliconAnalysts (2026)

**设备商**
- KLA Q3 FY26 营收$3.415B(+11% YoY)，市占58%，WFE~$140B — KLA IR 2026-07 / Trefis 2026-07-07
- LRCX: 3/31→7/7 涨52.7%(PE扩张40.9%)；WFE $110B→$135B — Trefis / 247wallst
- AMAT: Q1 FY26 $7.01B，WFE增长>30% — Perplexity Finance / Yahoo Finance

**估值（截至7/08-09）**
- TSM ~$437 PE(TTM)36.3x PE(Fwd)27.7x — Yahoo Finance / Morningstar / GuruFocus 2026-07-09
- ASML ~€1,989 PE(TTM)~60x PE(Fwd)~48x — 多源
- LRCX PE(Fwd)~60x — ValueInvesting.io 2026-07-09
- KLAC ~$1,808 PE(TTM)59.4x PE(Fwd)~61x — Macrotrends / ValueInvesting.io 2026-07-08
- AMAT PE(TTM)53.7x PE(Fwd)~38x — Stock Analysis
- INTC ~$108-110 PE(Fwd)~66.7x PE(TTM)负 YTD+83% — Investing.com / Yahoo / Simply Wall St 2026-07-08

**Hyperscaler CapEx**
- Goldman Sachs 累计$1.15T至2027 — IO Fund io-fund.com
- S&P Global 2027单年可能$1T — spglobal.com/ratings
- 2026 四大hyperscaler $610-725B — CNBC 2026-02 / LinkedIn(Morgan Stanley)

---

## 7. 给 CIO 的核心提示

1. **H4 是本轮主线**：transistors/$ 首次倒退(562M→412M)是结构性信号，建议下调至 40%，并将叙事从"先进制程=持续降本"修订为"成本重心从制程缩放转向先进封装"。
2. **估值全面变贵**：ASML 48x / LRCX 60x / KLAC 61x 远超 R2，设备商"卖铲子"逻辑被充分定价，建议对 LRCX/KLAC/ASML 减仓，加仓估值保护最好的 AMAT。
3. **财报窗口(7/15-16)**：ASML(7/15)+TSMC(7/16) 本周连发，建议保留 6% 现金等数据落地再决策，特别是 N2 营收% 与 ASML Q2 订单。
4. **Intel 外部客户受挫**：NVIDIA 退出 18A 测试是实质负面，INTC 从"高赔率期权"降级，建议仓位 7%→5%。
5. **K5(每晶体管成本)接近触发**：下次复查(9月)首要验证 N2P 实际良率与定价。

---

**报告完成时间**：2026-07-10
**下次关键事件**：ASML Q2(7/15)、TSMC Q2(7/16)、KLA Q4 FY26(7/28)
