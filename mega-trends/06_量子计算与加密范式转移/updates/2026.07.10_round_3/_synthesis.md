# CIO 综合裁定 — #06 量子计算与加密范式转移（Round 3）

> CIO 最终裁定 | 2026-07-10 | 基于 R2 基线 + 4 份研究员报告（A 基本面 / B 催化剂 / C 宏观 / 魔鬼辩护人）+ PM 审阅 + WebSearch 独立查证
> **本轮头号裁定**：魔鬼辩护人在 PQC 市场规模上正确（$2-3.5B 非 $50-80B，宏观 C 独立佐证），R2 为第二次高估；但 Quantinuum IPO 一项魔鬼只讲了半截故事（首日破发→EO 催化回升→+25% 稳定 5 周），Wolfpack 指控标风险旗不采信。维持"积极关注"，投机层权重从 15% 下调至 12%。

---

## 一、Delta 摘要（相对 R2 的关键变化，按重要性排序）

| # | 变化项 | 方向 | 级别 | 说明 | 来源 |
|---|--------|------|------|------|------|
| 1 | **★ Trump 双行政令（06.22）** | 偏多 | ★★★★★ | EO 14412 首次将 PQC 迁移定为联邦强制（2030 密钥 / 2031 数字签名）+ 国家量子计划。全球最激进 PQC 时间表。直接利好确定性层 | [White House EO](https://www.whitehouse.gov/presidential-actions/2026/06/securing-the-nation-against-advanced-cryptographic-attacks/)；[Mayer Brown](https://www.mayerbrown.com/en/insights/publications/2026/06/)；[Cloudflare](https://blog.cloudflare.com/post-quantum-eo-2026/) |
| 2 | **★ PQC TAM 第二次修正（头号冲突）** | 偏空修正 | ★★★★★ | 魔鬼 + 宏观 C 独立收敛：PQC 外部采购市场 2026 ~$2-3.5B（非 R2 $50-80B）。R1 $150B → R2 $50-80B → R3 $2-3.5B。R2 为第二次高估。但确定性层逻辑重述为特许经营+监管顺风 | MarketsandMarkets $0.42B / Precedence $2.31B / MarkNtel $2.0B |
| 3 | **Quantinuum IPO 半截故事合并** | 中性 | ★★★★ | 完整故事：首日 tepid（$60.38 / 盘中 $55.26 破发）→ 6/22 EO 催化 → 回升至 $74-76（+25%）稳定 5 周。条件 #3 = 5/13 周（40%）。WebSearch 查证 QNT $74.60-75.61（07.09-10） | CNN Markets / TradingView / StockTitan |
| 4 | **IBM $100 亿承诺 + 创新高 $320.42** | 偏多 | ★★★★ | 5 年期押注 Starling 2029（200 逻辑比特/1 亿门）。量子贡献 ~$26B（10-11%）。P/S ~4.4x 合理。后回撤至 $295.30 | [IBM Newsroom 06-02](https://newsroom.ibm.com/2026-06-02-ibm-commits-more-than-10-billion-to-quantum-computing) / Barron's |
| 5 | **CHIPS $20.13 亿 LOI 签署（政府股权创新）** | 偏多 | ★★★★ | 9 家公司（IBM ~$10 亿/GF $3.75 亿/7 家分 $6.38 亿）。联邦政府首次以非控股股权换拨款 | [NIST 05-21](https://www.nist.gov/news-events/news/2026/05/department-commerce-announces-letters-intent-9-companies-2-billion) |
| 6 | **Wolfpack 做空 IONQ（风险旗）** | 偏空 | ★★★★ | 指控 86% booked 收入来自已取消 earmarks / $546M 收入黑洞。对抗性来源，标风险旗不采信。IONQ -25.81%（30 天），做空 24% | [Fortune 02-04](https://fortune.com/2026/02/04/ionq-wolfpack-research-short-seller-says-quantum-computing-company-misled-investors-about-cancelled-government-backdoor-earmarks/) |
| 7 | **内部人抛售 $857M** | 偏空 | ★★★ | IonQ $454.1M + D-Wave $331.1M + Rigetti $71.5M。信息优势方在用脚投票 | Yahoo Finance / TQI |
| 8 | **Helios Nature 论文 + Atom Toric Code** | 偏多 | ★★★ | Helios 50 逻辑量子比特（98 物理，色码 2:1 编码比，Nature 同行评审）/ Atom Computing 中性原子首次完整 toric code QEC | [Nature s41586-026-10676-4](https://www.nature.com/articles/s41586-026-10676-4) |
| 9 | **10Y UST 4.54%（投机层估值压制主因）** | 偏空 | ★★★ | 长端利率走高（R2 隐含下行假设错误）。DCF 折现率上升压亏损股。IONQ P/S 100x→69x | Trading Economics / FRED |
| 10 | **量子 VC -58%**（被主权 $40B+ 对冲） | 中性 | ★★ | 私有市场冬天信号，但 CHIPS + 全球主权资金维持地板。资金结构从市场驱动→政策驱动 | Tracxn / Crunchbase / Qureca |
| 11 | **拓扑路线被边缘化** | 路线收敛 | ★★ | MSFT Majorana 2（06.02）声称 20s 相干但未独立验证，学界公开质疑。MSFT 转向与 Atom Computing 合作=实质承认拓扑不足 | Nature/SciAm/TQI |
| 12 | **D-Wave RSA-2048 声明被广泛质疑** | 维持 | ★★ | Wang 2025 仅特殊结构整数（~90 bit），非通用 RSA。Q-Day 恐慌概率维持 10% | Homeland Security Today / HN |

**Delta 定性**：R2 核心矛盾是"技术进展 vs 估值极端"。R3 核心矛盾切换为**"政策催化空前强劲（Trump 双 EO + CHIPS + IBM $100 亿）vs PQC TAM 高估修正 + Wolfpack 风险旗 + 内部人抛售"的多空对峙**。政策催化使确定性层逻辑进一步强化（即使 TAM 小，合规截止是硬性的）；但投机层风险显著上升（Wolfpack + 内部人 + 估值去泡沫）。R3 是"确定性更确定、投机更投机"的分化轮。

---

## 二、评级裁定

### 头号裁定（一句话）

**维持"积极关注"**：R2 后政策催化（Trump 双 EO）+ 技术进展（Helios Nature）+ IPO 稳定（QNT +25%）= 向上推力；但 PQC TAM 高估修正（$50-80B→$2-3.5B）+ Wolfpack 风险旗 + 内部人 $857M 抛售 + IBM 量子优势措辞软化 = 向下修正力。多空对峙下不升级不降级，投机层从 15% 下调至 12%。

### 评级变化表

| 维度 | R2 | R3 | 变化 |
|------|-----|-----|------|
| **评级** | 技术关注 → 积极关注 | **积极关注（维持）** | 持平 |
| **PQ 时钟** | PQ1（7-8 点钟） | **PQ1+（向 8 点钟移动，未达 PQ2）** | 微进 |
| **确定性层逻辑** | PQC 迁移受益，$50-80B TAM | **特许经营质量 + PQC 监管顺风（EO 14412）。TAM ~$2-3.5B 但合规硬截止** | 逻辑重述 |
| **投机层权重** | 15% | **12%（-3pp）** | 下调 |
| **IBM 2029 延迟概率** | 50% | **45-50%（拆分裁定）** | 微降 |
| **升级窗口** | 2026 Q4-2027 Q1 | **2026 Q4-2027 Q1（维持）** | 持平 |

### 不升级到"有条件通过"的依据

1. 升级 4 条件 **0/4 完全达成**（详见第五节进度表）
2. PQC TAM 高估须修正——虽然确定性层逻辑重述后仍成立，但 R2 的具体数字（$50-80B）已被推翻
3. IBM 2026 量子优势措辞软化（"first cases" + "hybrid" + "community-verified"），7/10 零独立验证
4. Wolfpack 风险旗未消散（即使不采信为事实）

### 不降回"技术观察"的依据

1. **Trump 双 EO（06.22）是 R2 后最大新催化**——EO 14412 将 PQC 定为联邦强制（2030/2031 截止），全球最激进时间表。这不是"建议"，是法规
2. **Helios Nature 论文** = 离子阱路线获同行评审的硬件级纠错验证（50 逻辑量子比特 / 99.921% 双比特门 / 2:1 编码比）
3. **CHIPS $20.13 亿 + IBM $100 亿** = 国家战略级资金落地（含政府股权创新）
4. **Quantinuum IPO 未崩**——WebSearch 查证 +25% 稳定 5 周（魔鬼的"首日破发"是半截故事）
5. **确定性层完全不依赖量子何时实用化**——PANW/CRWD/NET 的核心是网安特许经营，PQC 是 tailwind
6. 魔鬼的 Wolfpack 采信过度（对抗性来源标旗非事实），泡沫类比缺差异性（量子有 Nature 同行评审）

---

## 三、PQ 投资时钟 + 三层组合

### PQ 时钟：维持 PQ1+（向 8 点钟移动但未达 PQ2）

**向 PQ2 推动的因素**：
1. Helios Nature 论文 = 离子阱同行评审硬件纠错验证
2. Trump EO 14412 = PQC 从建议→联邦强制
3. CHIPS $20 亿 = 国家级资金承诺→意向书落地
4. Quantinuum IPO +25% = 公开市场初步定价能力
5. IBM 分子模拟 = 从理论→首个真实物理对象模拟

**未达 PQ2 的阻碍**：
1. 无确认量子优势（速度意义）——CEO 仍"预测"非"已实现"
2. 逻辑量子比特 50-100 区间——距 1000（药物发现）/百万（RSA）仍远
3. 路线仅部分收敛（拓扑边缘化，4 主流并行）
4. IBM 2026 措辞软化

### 三层投资组合（R2→R3）

| 层级 | R2 | R3 | 变化 | 核心逻辑 |
|------|-----|-----|------|---------|
| **确定性层** | 60% | **60%** | 持平 | 特许经营质量（PANW/CRWD/NET 网安龙头）+ PQC 监管顺风（EO 14412 / M-26-15 / NSA CNSA 2.0 2030）。PQC TAM ~$2-3.5B 但合规硬截止。**PQC 是 catalyst 非 sole thesis** |
| **概率层** | 25% | **25%** | 持平 | IBM 主仓。量子期权价值 ~$26B（10-11%），$100 亿承诺 + CHIPS ~$10 亿。传统业务安全边际。**注意：量子敞口被核心业务稀释，IBM 不是纯量子代理标的** |
| **投机层** | 15% | **12%** | **-3pp** | IONQ 小仓位（2-3%）。下调理由：Wolfpack 风险旗 + 内部人 $454M 抛售 + P/S 69x 仍贵 + -25.81% 回撤。Q2 8/12 生死验证 |
| **现金/观察** | 0% | **3%** | +3pp | 等待 8/12 IonQ Q2 + QNT 财报 + 11 月 IBM Quantum Summit |

### 标的矩阵

| 标的 | R2 评级 | R3 评级 | 逻辑 |
|------|---------|---------|------|
| **PANW** | 确定性层核心 | **确定性层核心** | 网安龙头 + Quantum-Safe 产品（01/2026 发布）+ EO 14412 合规驱动。P/E ~263-278 高但 PQC 是业务质量强化因子 |
| **CRWD** | 确定性层 | **确定性层** | 网安板块龙头。PQC 集成中 |
| **NET** | 确定性层 | **确定性层（卫星）** | Cloudflare PQC 集成最深（~2% TLS 1.3 已 PQC → 2029 全 PQC），但估值更激进。PQC 集成深度=卫星定位理由 |
| **IBM** | 概率层主仓 | **概率层主仓（维持）** | 创新高 $320.42 验证叙事。量子 ~$26B（10-11%）。$100 亿承诺。P/S ~4.4x 合理。传统业务安全边际。**量子期权 ≤10-11%，非纯量子标的** |
| **GOOGL** | 辅仓 | **辅仓（维持）** | PQC + Willow 量子研究（Nature 1211 引用）。无重大新进展 |
| **IONQ** | 投机层（组合 2-3%） | **投机层（组合 2-3%，风险加剧）** | P/S 100x→69x（方向对）。RPO $470M + 政府合同管线。**但**：Wolfpack 风险旗（$546M 黑洞）+ 内部人 $454M 抛售 + 做空 24% + $1B 增发稀释。Q2 8/12 是"维持 vs 减半"生死验证 |
| **QNT** | 观察 | **观察→候选** | +25% 稳定 5 周 + 客户集中度 90%→7% 改善 + Honeywell 背景 + 分析师覆盖（最高目标 $155）。**但** P/S ~460x（2025 收入 $30.9M）/ 亏损扩大 / 锁定期 12 月。若 9 月稳定 3 月+Q2 财报不崩→入投机层小仓位 |
| **RGTI** | 回避 | **回避** | 收入基数极小（$4.4M/季）。-16%。做空 59.24M 股 |
| **QBTS** | 回避 | **回避→观察（非买入）** | 收入曾 -81%。P/S 极高。但 CHIPS 获款 + EO 动能。可观察但不买入 |
| **QUBT** | 回避 | **回避** | Q1 $3.7M 全靠并购。短空 29-32%。有机收入 ~0 |

---

## 四、关键事实裁定表（冲突点 + 裁决 + 来源）

| # | 冲突 | 多头方 | 空头方 | CIO 裁决 | 来源 |
|---|------|--------|--------|---------|------|
| 1 | **Quantinuum IPO 表现** | A/B：+25% 稳定 5 周，条件 #3 在轨 | 魔鬼：首日破发 -8%（$55.26），条件 #3 失败 | **合并：首日 tepid（$60.38 / 盘中 $55.26）→ EO 催化 → +25% 稳定 5 周。条件 #3 = 5/13 周（40%），在轨但脆弱。QNT 当前 $74.60-75.61（WebSearch 查证）** | CNN Markets / TradingView / StockTitan（07.09-10） |
| 2 | **PQC 可投资 TAM** | C：维持 $50-80B | 魔鬼：$2-3.5B（MarketsandMarkets/Precedence/MarkNtel） | **魔鬼正确（宏观 C 独立佐证）。R3 PQC 外部采购 ~$2-3.5B（2026）→ ~$3-5B（2030）。R2 $50-80B 为第二次高估（R1 $150B）。但确定性层逻辑重述为特许经营+监管顺风** | MarketsandMarkets $0.42B / Precedence $2.31B / MarkNtel $2.0B |
| 3 | **IBM 2029 延迟概率** | A：40-45%（Willow 1211+Helios 2:1 编码比） | 魔鬼：60-65%（2026 软化+延迟史+Kalai） | **拆分：2026 近期优势→魔鬼对（措辞软化）；2029 容错→基本面对（物理验证）。R3 = 45-50%。A 用 Willow 物理验证推导 IBM 工程路径=逻辑跳跃；魔鬼用 2026 软化推导 2029 失败=过度链式** | IBM Newsroom / Kalai Blog / Nature |
| 4 | **Wolfpack/IonQ 指控** | 其他 3 人未引用（+755%/RPO $470M） | 魔鬼：$546M 黑洞 / 86% 已取消 earmarks | **风险旗，非确认事实。Wolfpack 是对抗性做空机构，$546M 是指控非裁决。IonQ 已否认。监控 Q2 披露/反驳。做空 24%=未消散熊方** | Fortune 02-04 / Wolfpack 原报告 / Barron's |
| 5 | **内部人抛售** | 未充分讨论 | 魔鬼：$857M（IonQ+D-Wave+Rigetti） | **可查证事实，采信。反映信息优势方在用脚投票。投机层下调 3pp 的依据之一** | Yahoo Finance / TQI 02-26 |
| 6 | **路线收敛度** | A：拓扑边缘化=部分达成（50%） | 魔鬼/B：4 主流并行，未收敛 | **部分收敛（1/5 边缘化）。条件 #4 进度 20%。需第二条确认（PsiQuantum 2026-27 原型？）** | Nature/TQI/PostQuantum |

---

## 五、升级 4 条件进度表

| # | 条件 | R2 状态 | R3 进度 | 达成度 | 关键证据 | 下次验证 |
|---|------|---------|---------|--------|---------|---------|
| 1 | **IBM 2026 验证量子优势** | 未兑现 | 措辞软化 + 分子模拟实用案例 | **40%** | 3 月分子模拟（非速度优势）；CEO 仍"预测年底前"；措辞退缩为"first cases"+"hybrid"+"community-verified"。$100 亿承诺+Nighthawk 按计划 | ~11 月 IBM Quantum Summit |
| 2 | **IonQ Q2-Q3 增速 200%+** | 待验证 | Q1 +755% + RPO $470M | **55%**（Wolfpack 风险旗下调） | Q1 $64.7M 超指引；出售首台 256Q 系统；DARPA HARQ+DOE+SDA 合同。**但**：Wolfpack 风险旗（$546M 黑洞）+ GAAP 利润来自权证收益 + $1B 增发稀释 | ~8/12 Q2 财报 |
| 3 | **Quantinuum IPO 3 月稳定发行价上** | 待验证 | 5/13 周，+25% | **40%** | QNT $74-76（+25%）；客户集中度 90%→7% 改善；分析师 Buy。**但**：首日 tepid + P/S ~460x + 亏损扩大 + 锁定期 12 月 | 9/4 满 3 个月 + Q2 财报 |
| 4 | **1-2 条路线被淘汰** | 未达成 | 拓扑边缘化（1/5） | **20%** | Majorana 未独立验证 + MSFT 转向 Atom Computing。但 4 主流全活跃（超导/离子阱/中性原子/光量子），CHIPS 多模态资助 | 2027 后 |

**综合**：4 条件 0/4 完全达成。加权达成度 ~39%。升级窗口维持 2026 Q4-2027 Q1。最大障碍是 #1（IBM 量子优势）和 #4（路线收敛）。

---

## 六、4 风险情景概率（R2→R3）

| 情景 | R2 | R3 | 变动 | 调整理由 |
|------|-----|-----|------|---------|
| **金发姑娘**（利率↓+CapEx 持续+无地缘） | 20% | **15%** | -5pp | 10Y UST 4.54% 远高于预期（R2 隐含下行假设错误）。长端走高否定"利率↓"前提。AI CapEx $700B 支撑科技整体但挤压量子 VC（-58%） |
| **温和增长**（利率持平+技术渐进+PQC 推进） | 45% | **50%** | +5pp | PQC 确定性强化（EO 14412 + M-26-15 联邦强制）；CHIPS $20 亿+主权 $40B+ 对冲 VC 退潮；IBM/IonQ/Quantinuum 技术渐进。最可能路径 |
| **量子冬天**（利率↑+资金退潮+无突破） | 25% | **25%** | 持平 | VC -58%+内部人 $857M 抛售=冬天信号。**但**主权 $40B++CHIPS+EO 14412 构成地板。冬天风险主要在私有市场+投机层（IONQ/QBTS/RGTI/QUBT），确定性层不受影响 |
| **Q-Day 恐慌**（量子提前破解 RSA） | 10% | **10%** | 持平 | D-Wave RSA-2048 声明被广泛质疑（仅特殊结构整数 ~90 bit）。无近期破解迹象。PQC 迁移截止日本身是"渐进式 Q-Day 应对" |

**核心调整**：从金发姑娘向温和增长转移 5pp。长端利率走高使"利率↓"假设失效，但 PQC 联邦强制+主权资金支撑温和增长最可能路径。量子冬天维持 25%——魔鬼建议上调至 32-35% 被主权资金+EO 14412 抵消，冬天风险分层（投机层局部冬天已到，确定性层不受影响）。

---

## 七、IBM 2029 延迟概率（拆分裁定）

### R2 基线：50%（建模 2029 30% / 2031 40% / 2033+ 30%）

### R3 裁定：**45-50%**（建模 2029 30% / 2031 40% / 2033+ 30%，微调）

**拆分逻辑**：

| 维度 | 多头论据（A） | 空头论据（魔鬼） | CIO 裁定 |
|------|-------------|----------------|---------|
| **2026 近期量子优势** | CEO 承诺 + 分子模拟 | 措辞软化（"first cases"+"hybrid"+"community-verified"），7/10 零独立验证 | **魔鬼更接近正确**——近期优势延迟概率高。IBM 在铺设下台阶 |
| **2029 容错量子计算机** | Willow below-threshold Nature 1211 引用 + Helios 2:1 编码比 = 物理基础已确认 | Kalai 噪声论证未推翻 + 延迟史（Kookaburra/Condor）+ 120Q→百万级工程鸿沟 | **基本面对，但 A 逻辑跳跃**——Willow 验证的是表面码 below-threshold 可行性（距离-5/7），不等于 IBM Starling 200 逻辑比特/1 亿门工程路径已验证。物理基础≠产品路径 |

**R3 值 45-50% 的理由**：
1. 物理基础已确认（below-threshold + 色码 2:1）= 降低延迟概率（vs 魔鬼的 60-65%）
2. 但工程跳跃巨大（120Q→百万级物理量子比特）+ IBM 延迟史 + Kalai 未被推翻 = 维持较高延迟概率（vs A 的 40-45%）
3. 取两者中值偏保守：45-50%
4. 建模维持 2029（30%）/ 2031（40%）/ 2033+（30%）——微调但不变结构

---

## 八、跨课题传导

| 课题 | R2 传导判断 | R3 更新 | 传导强度 |
|------|------------|---------|---------|
| **#01 AI CapEx** | NVIDIA 是颠覆者还是卖铲人？ | **卖铲人定位确认**：NVQLink + CUDA-Q 平台，35+ 公司接入。黄仁勋"未来是混合计算"=量子不颠覆 GPU 而是补充。**风险**：AI CapEx $700B+ 挤压量子 VC（-58%），资金/人才/注意力比例 ~140:1 | ★★★★ |
| **#11 半导体** | IBM Poughkeepsie 300mm 工艺 | **升级为 Albany**：IBM "~$10 亿" CHIPS 资金建"Anderon"子公司在 Albany NY 建量子芯片晶圆厂；GlobalFoundries 同批获资。CHIPS 取股权非补贴=政府深度绑定制造。量子芯片从实验室向 300mm 工艺转型 | ★★★★ |
| **#05/#15 网安** | PQC 迁移是最大确定性主题 | **确定性再强化（最强传导）**：EO 14412（2030/2031 联邦强制）+ M-26-15（120 天迁移计划）+ PANW Quantum-Safe 产品（01/2026）+ FIPS 206 草拟中。PQC 是网安板块未来 3-5 年最硬性合规驱动。**但** PQC 外部采购 TAM ~$2-3.5B，增量收入 <2%/家——PQC 是催化剂非核心论据 | ★★★★★ |
| **#04 地缘** | 中美量子竞赛 | **竞赛制度化**：中国天衍-287（287Q 超导）+ 天衍-P2000（光量子）+ 十五五战略产业；美国 CHIPS $20 亿取股权（国家安全兜底）+ EO 14412。本源量子被制裁仍运营。Asia Times"量子企业在中美间重新站位" | ★★★★ |

---

## 九、退场标准 + 下次复查窗口

### 退场/降级触发（降回"技术观察"）

1. **Wolfpack 指控被独立证实**（IonQ Q2 财报披露收入大幅下修或 SEC 调查启动）
2. **QNT 跌破 $60 发行价持续 2 周**（系统性负面信号）
3. **IBM 2026 Quantum Summit 未宣布量子优势**（条件 #1 实质失败）
4. **10Y UST 突破 5% + AI CapEx 指引 < +15%**（投机层估值全面崩塌）

### 升级触发（升至"有条件通过"）

1. **IBM Quantum Summit（~11 月）宣布独立验证的商业量子优势**（条件 #1）
2. **IonQ Q2 维持 200%+ 且 Wolfpack 指控被澄清**（条件 #2 + 风险旗移除）
3. **QNT 9 月稳定在发行价以上 3 个月**（条件 #3 达成）
4. **第二条路线被边缘化**（如 PsiQuantum 2026-27 原型未达预期）（条件 #4）

### 下次复查：2026 年 8 月下旬（IonQ Q2 + QNT 财报 + FOMC 之后）

| # | 必答问题 | 数据源 | 判定标准 |
|---|---------|--------|---------|
| 1 | **IonQ Q2 财报（~8/12）**：200%+ 增速？Wolfpack 指控澄清？ | IonQ IR | 维持 200%+ 且无收入下修→投机层恢复至 15%；增速 <150% 或 Wolfpack 被证实→IONQ 减半至 1-1.5% |
| 2 | **Quantinuum Q2 财报（~8 月）**：首份上市后披露？ | QNT IR | 收入改善+亏损收窄→候选确认；收入大幅低于预期→观察维持 |
| 3 | **FOMC 7/28-29**：利率路径？ | Fed | 10Y UST 回落至 <4.3%→投机层估值压力缓解；维持 >4.5%→继续压制 |
| 4 | **IBM Quantum Summit 前瞻**：量子优势演示预告？ | IBM IR | 有 Nature/Science 论文预告→条件 #1 接近达成；无→维持待验证 |
| 5 | **EO 14413 执行**：7/22 30 天截止，联邦机构是否指定 PQC 负责人？ | White House | 按期执行→确定性层强化；延迟→PQC 时间表可信度下降 |
| 6 | **NVIDIA Q2（~8 月中）**：量子-经典混合平台进展？ | NVDA IR | CUDA-Q 接入公司数增长→#01 传导确认 |

### 监控指标

| 指标 | 当前值（R3） | 警戒线 | 行动 |
|------|------------|--------|------|
| QNT 价格 | ~$74-76（+25%） | 跌破 $60 持续 2 周=系统性负面 | 周度跟踪 |
| IONQ P/S | ~69x（FY26 前瞻） | >80x=重新泡沫化；<50x=估值正常化 | Q2 财报后重算 |
| IBM 量子优势 | CEO"预测年底前" | Quantum Summit 无宣布=条件 #1 失败 | ~11 月 |
| 10Y UST | 4.54% | >5%=投机层全面承压；<4%=估值缓解 | 7/28-29 FOMC |
| Wolfpack 指控 | 未裁决 | SEC 调查或收入下修=风险旗升级为确认事实 | Q2 财报披露 |
| QNT 锁定期 | ~12 月到期 | 11 月开始预警早期投资者减持动能 | 月度跟踪 |
| 路线收敛 | 拓扑边缘化（1/5） | 第二条边缘化=条件 #4 接近达成 | 半年度 |

---

## 十、关键来源（带日期）

### 政策（R2 后最大新催化）
1. [White House — EO 14412 "Securing the Nation Against Advanced Cryptographic Attacks"（2026-06-22）](https://www.whitehouse.gov/presidential-actions/2026/06/securing-the-nation-against-advanced-cryptographic-attacks/)
2. [White House — "Ushering in the Next Frontier of Quantum Innovation"（2026-06-22）](https://www.whitehouse.gov/presidential-actions/2026/06/ushering-in-the-next-frontier-of-quantum-innovation/)
3. [Mayer Brown — Two Quantum EOs 分析（2026-06）](https://www.mayerbrown.com/en/insights/publications/2026/06/president-trump-signs-two-executive-orders-on-quantum-computing-and-accelerated-post-quantum-cryptography-migration)
4. [Cloudflare Blog — Post-Quantum EO 2026 分析（2026-06）](https://blog.cloudflare.com/post-quantum-eo-2026/)
5. [White House — M-26-15 PQC 迁移备忘录（2026-06）](https://www.whitehouse.gov/wp-content/uploads/2026/06/M-26-15-Execution-of-the-Migration-to-Post-Quantum-Cryptography.pdf)

### Quantinuum IPO（WebSearch 查证）
6. [CNN Markets — QNT $75.61（2026-07-09）](https://www.cnn.com/markets/stocks/QNT) — CIO WebSearch 交叉验证
7. [TradingView — QNT $74.60（2026-07-10）](https://www.tradingview.com/symbols/NASDAQ-QNT/)
8. [StockTitan — QNT $74.56（2026-07-04）](https://www.stocktitan.net/news/QNT/)
9. [Quantinuum — IPO 定价公告（2026-06-04）](https://www.quantinuum.com/press-releases/quantinuum-announces-pricing-of-upsized-initial-public-offering)

### PQC 市场规模（魔鬼有效攻击）
10. [MarketsandMarkets — PQC 市场 $0.42B（2025）](https://www.marketsandmarkets.com/Market-Reports/post-quantum-cryptography-market-126986626.html)
11. [Precedence Research — PQC 市场 $2.31B（2026）](https://www.precedenceresearch.com/post-quantum-cryptography-market)

### IBM / 技术
12. [IBM Newsroom — $100 亿+ 量子承诺（2026-06-02）](https://newsroom.ibm.com/2026-06-02-ibm-commits-more-than-10-billion-to-quantum-computing,-funding-its-roadmap-from-todays-leading-systems-to-the-worlds-first-fault-tolerant-quantum-computers)
13. [Quantinuum Helios — Nature 论文（2026）](https://www.nature.com/articles/s41586-026-10676-4)
14. [Google Willow — Nature 论文（2025，被引 1211）](https://www.nature.com/articles/s41586-024-08449-y)
15. [Kalai 博文回应 Aaronson（2026-03-10）](https://gilkalai.wordpress.com/2026/03/10/scott-aaronsons-view-of-my-view-about-quantum-computing/)

### CHIPS / 主权资金
16. [NIST — 9 家公司 $20.13 亿 LOI（2026-05-21）](https://www.nist.gov/news-events/news/2026/05/department-commerce-announces-letters-of-intent-9-companies-2-billion)
17. [WSJ — 量子拨款 + 政府股权（2026-05）](https://www.wsj.com/tech/quantum-computing-grants-ibm-rigetti-globalfoundries-7382e6be)

### Wolfpack / 内部人（风险旗）
18. [Fortune — Wolfpack 做空 IonQ（2026-02-04）](https://fortune.com/2026/02/04/ionq-wolfpack-research-short-seller-says-quantum-computing-company-misled-investors-about-cancelled-government-backdoor-earmarks/)
19. [Yahoo Finance — 内部人抛售 $857M（2026）](https://finance.yahoo.com/markets/stocks/articles/quantum-computing-stocks-ionq-rigetti-092600459.html)

### 宏观
20. [Trading Economics — 10Y UST 4.54%（2026-07-10）](https://tradingeconomics.com/united-states/government-bond-yield)
21. [Tracxn — 量子 VC 融资 -58.34%（2026）](https://tracxn.com/d/sectors/quantum-computing/)

---

## 附录：CIO 核心裁定依据

### 裁定 1：为何维持"积极关注"而非升级或降级

**不升级**：4 条件 0/4 完全达成（加权 ~39%）。PQC TAM 高估须修正（R2 $50-80B→R3 $2-3.5B）。IBM 2026 量子优势措辞软化。Wolfpack 风险旗未消散。

**不降级**：Trump 双 EO（06.22）是 R2 后最大新催化——EO 14412 将 PQC 定为联邦强制（2030/2031 截止），这不是建议是法规。Helios Nature 论文（同行评审 50 逻辑量子比特）+ CHIPS $20 亿 + IBM $100 亿 = 三项可验证实质进展。Quantinuum +25% 稳定（魔鬼的"首日破发"是半截故事，WebSearch 查证当前 $74-76）。确定性层完全不依赖量子何时实用化。

**"积极关注"精准反映当前状态**：技术有实质进展但无范式级突破；政策催化空前但 PQC TAM 被修正；IPO 稳定但首日脆弱+锁定期未到；投机层风险加剧（Wolfpack+内部人）但确定性层逻辑强化（EO 14412）。

### 裁定 2：为何 PQC TAM 修正不改变确定性层权重

魔鬼指出 PQC 外部采购市场仅 $2-3.5B（三源收敛），PANW/CRWD/NET 的 PQC 增量收入 <2%/家。**这是正确的**。但确定性层 60% 权重的逻辑基础不是 PQC TAM 规模，而是：

1. **网安特许经营质量**——PANW（年化收入 ~$90 亿）/ CRWD / NET 是网安龙头，PQC 是其产品矩阵的一个功能模块。PQC 迁移不改变它们的龙头地位
2. **合规驱动的确定性**——EO 14412 + M-26-15 + NSA CNSA 2.0 2030 = 硬性联邦法规截止日。合规驱动是网安板块最确定的需求来源（不依赖量子何时实用化）
3. **PQC 是 catalyst/tailwind 非 sole thesis**——即使 PQC 增量收入 <2%，它强化了 PANW/CRWD/NET 的平台粘性（客户需要端到端 PQC 解决方案），间接支持续约率和 ARPU

因此，PQC TAM 修正从 $50-80B→$2-3.5B 改变的是**叙事规模**（不再是"巨大新市场"），不改变**投资逻辑**（网安龙头 + 合规驱动 + PQC 催化）。

### 裁定 3：为何投机层从 15% 下调至 12%

三个可查证的风险信号叠加：
1. **Wolfpack 风险旗**——$546M 收入黑洞指控 + 86% 来自已取消 earmarks。即使未证实，做空报告的存在 + 24% 做空比例增加了不确定性
2. **内部人 $454.1M 抛售**（IonQ 单家）——信息优势方在用脚投票
3. **$1.0B 股权增发**——管理层高位稀释

IONQ 维持投机层小仓位（2-3%），因为 RPO $470M + 政府合同管线 + 光子互连里程碑提供了基本面支撑。但 Q2（~8/12）是"维持 vs 减半"的生死验证。释放的 3pp 转入现金/观察，等待 Q2 结果。

### 裁定 4：Wolfpack 指控的处理原则

Wolfpack 是已知做空机构，有利益冲突（做空获利）。$546M 和 86% 是具体数字但未经裁决。IonQ 已否认。**标为风险旗而非确认事实**——这是处理对抗性来源的正确姿态：

- **不采信为事实**：做空报告可能夸大，$546M 黑洞需要 IonQ Q2 财报披露或 SEC 调查来证实/证伪
- **不忽视**：做空比例 24% 反映未消散的熊方观点，且 Wolfpack 的指控具体可查（DARPA 合同、earmarks 取消记录）
- **纳入监控**：Q2 财报是关键——若收入大幅下修或 SEC 启动调查，风险旗升级为确认事实；若 IonQ 提供收入来源明细反驳 Wolfpack，风险旗降级

---

> **一句话总结**：Trump 双行政令（06.22）将 PQC 定为联邦强制是 R2 后最大催化，但 PQC 外部采购市场被修正至 $2-3.5B（魔鬼正确，R2 第二次高估）。维持"积极关注"，三层组合从 60/25/15 调整为 60/25/12（+3% 现金）。确定性层逻辑重述为特许经营+监管顺风（PQC 是 catalyst 非 sole thesis）；投机层因 Wolfpack 风险旗+内部人 $857M 抛售下调 3pp。Quantinuum 半截故事合并（首日破发→EO 催化→+25% 稳定 5 周）。IBM 2029 延迟概率拆分裁定为 45-50%。**8/12 IonQ Q2 财报 + ~11 月 IBM Quantum Summit 是两个生死验证窗口。**

---

*本报告基于截至 2026-07-10 的公开信息与 4 份研究员报告 + PM 审阅。QNT 价格经 WebSearch 交叉验证（CNN Markets $75.61 / TradingView $74.60）。所有预测含不确定性，不构成投资建议。*
