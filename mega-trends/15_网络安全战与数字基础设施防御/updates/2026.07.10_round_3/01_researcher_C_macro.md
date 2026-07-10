# Round 1 研究员 C 宏观 — #15 网络安全战与数字基础设施防御
> 轮次: R3(2026.07.10) | 基线: R2(2026.05.25) | 角色: C 宏观（系统性/二阶影响）

---

## 1. 宏观/系统性变化（2026.06-07）

### 1.1 市场规模与渗透率——R2 基线的一个重要修正

**已发生（高置信度）**：Gartner 2026 年全球信息安全支出指引 **~$244B**，同比增长 **12-13%**（2025 约 $215B），位于 R2 基线 $219-255B 区间的中段偏下。同期全球 IT 总支出 **$6.15-6.31T**（Gartner 2026.02 / 后续上修至 +13.5%）。

**关键修正**：R2 README 暗示网安占 IT 预算 "5-15%"，但用 Gartner 顶层口径计算，2026 年实际渗透率仅 **~3.9-4.0%**（$244B / $6.15T）。两者差异来自分母定义（企业 IT 预算 vs 含消费者/电信设备的全球 ICT 总支出），但即便取企业口径，行业普遍反馈 6-8% 是更真实的中位数。**这意味着"网安渗透率上行"的长期 TAM 故事仍有很大空间——目前处于早期渗透阶段，而非接近饱和**。

**警示信号**：Gartner 同时指出，企业在生成式 AI 工具上的花费已是信息安全投入的 **~17 倍**。AI CapEx 爆发正在挤压安全预算的相对优先级——这是 R2 未充分识别的短期逆风。与 #01 AI / #19 AI 对 SaaS 的传导：AI 投入并非自动转化为安全投入，反而可能先扩大攻击面再倒逼安全追加。

**趋势推断（中置信度）**：若维持 12-13% CAGR，2030 年全球网安市场将达 **~$385-420B**，落在 R2 的 $335-580B 区间下半段。要触及上沿（$500B+），需要 AI 攻防 + 监管 + 国防三重催化同时兑现。

### 1.2 监管框架的重大分化（本季最重要的结构性变化）

**已发生（高置信度）——大西洋两岸监管走向相反方向**：

| 维度 | 美国（Trump 时代转向） | 欧盟（持续收紧） |
|------|----------------------|----------------|
| 总体战略 | "President Trump's Cyber Strategy for America"（2026.03.06 发布，7 页 + 配套 EO），明确"清除 Biden 时代监管重负"、America First、AI 主导 | NIS2 + DORA + CRA + AI Act + Product Liability Directive 五法协同 |
| 软件安全/SBOM | **OMB 2026.01.23 备忘录撤销联邦软件强制安全自证**，SBOM 从"必须"变"可选"——重大逆转 | **EU Cyber Resilience Act** 分阶段强制：2026.09 漏洞/事件报告生效，2027.12 全 SBOM 要求 |
| 责任 | 软件厂商责任改革（Biden 国家网安战略核心）在 Trump 下方向不明，"减少合规负担"优先 | **EU Product Liability Directive** 2026.12.09 前成员国必须实施，**首次将软件和 AI 纳入产品责任**——历史性 |
| 关键事件披露 | SEC 4 天规则（2023.12 生效）持续执行，但执法力度观察分歧 | DORA 宽限期 2026 结束，转主动执法；NIS2 首次合规审计截止 2026.06.30 |
| 罚款上限 | 相对温和，倾向于"促创新" | NIS2 关键实体最高 **€10M 或全球营收 2%**；DORA 同等量级 |

**宏观含义**：
1. **监管套利机会消失**：跨国企业（尤其金融服务、云、医疗）无法回退到更宽松的美国标准，因为只要触及欧盟客户/运营就受 EU 法管辖。**欧盟事实上成为全球合规基线的设定者**——与 GDPR 效应相同。
2. **碎片化市场机会**：SBOM 标准、责任框架、披露要求在 US/EU/中/印日益分化，催生"合规即服务"细分市场（V-Comply、Sbomify、Orbiq 等专注多法域合规的工具崛起）。
3. **Trump 软化的短期抵消有限**：OMB SBOM 撤销主要影响联邦政府采购，私营部门和欧盟供应链不受影响。净效应仍是合规驱动支出上行。

### 1.3 国防与国家级威胁——Volt/Salt Typhoon 持续活跃

**已发生（高置信度）**：
- FBI 2026.02 确认 **Salt Typhoon 威胁持续活跃**，基础配置错误和已知 CVE 仍是主要入口。电信间谍活动未收敛。
- "台风系列"已扩展至至少 **4 个协调 APT**：Volt（IT/OT 预置）、Salt（电信间谍）、Flax（台湾/东南亚）、Brass——显示系统性、多层次国家级行动。
- timeline.md 记录的"中国罕见公开承认 Volt Typhoon 相关活动"标志着网络空间从灰色地带向公开博弈转移。

**2026 重大攻击事件（已发生）**：
- University of Mississippi Medical Center 勒索（2026.02，CSIS 列入重大网络事件）
- 德国国家铁路运营商攻击（2026.02，票务/时刻表系统中断）
- 北欧关键基础设施攻击
- 医疗勒索 QoQ +8.5%，2025.04 单月 90 个受害组织（Cyfirma）

**趋势推断（中置信度）**：R2 国防网安 $20.35B→$54.46B（2025-2033，CAGR ~13%）的路径继续。Trump "America First"战略反而可能**加速**国防网安支出（把网络安全框为国家主权/国防前线），即使民用监管放松。

---

## 2. 二阶影响与攻防经济学

### 2.1 AI 正在系统性改变"攻易守难"的不对称——但方向比 R2 预期更复杂

**已发生（高置信度）——攻击侧成本崩塌**：
- 2025 年 AI 驱动网络犯罪全球成本 **~$193B**（SQ Magazine）
- 2025 H1 美国 deepfake 欺诈损失 **$547.2M**（ZeroThreat AI）
- **Prompt 注入攻击 YoY +340%**，出现在 **73% 的生产 AI 部署**中（BabyBots/Pillar Security）
- 2025 全球 prompt 注入相关损失 **~$2.3B**
- AI 使"钓鱼、凭证填充、漏洞利用更快、更便宜、更可扩展"（Shumaker、DeepStrike）

**关键洞察**：R2 倾向于把 AI 框为"攻防双刃剑"。但 2026 数据显示，**攻击侧的成本下降曲线远快于防御侧的成本下降曲线**——因为攻击者享受了 AI 的杠杆（一次 prompt 注入模板可复用 73% 的部署），而防御者仍需针对每个企业环境定制防护。**结构不对称在恶化，而非缓解**。

**二阶影响（中置信度）**：
- 防御成本上升 → 企业被迫向平台化/整合方向集中（利好 PANW 的平台化策略、CRWD 的 Falcon Complete）——这是 R2 未充分展开的"规模经济"论点。
- AI 工具花费 17x 于安全的比例若持续，将形成"AI 扩大攻击面 → 安全预算追涨"的滞后循环，2027-2028 年可能出现补偿性安全支出跳升。

### 2.2 网络保险——保费软化与底层风险上升的危险背离

**已发生（高置信度）**：
- 2026 网络保险市场 ~**$22.5B**（Security.org，比 R2 的 $14B 基线显著上修）
- 美国网络费率 2024 Q4 同比 **-5%**（Marsh），延续 2023-2025 的软化周期
- S&P Global 2026 展望：盈利韧性强但竞争加剧，**保险业 cyber 定价能力仍落后其他险种**
- Gallagher 2026 展望：AI、量子、供应链成系统性风险新驱动

**危险信号（重要）**：CNI Solutions 明确指出"**低保费 ≠ 低风险**"——近期费率下降反映的是 loss ratio 改善和竞争，而非底层真实风险下降。CrowdStrike 2024.07 中断事件（全球经济损失 $10B+，保险损失 $400M-$1.5B）被 Gen Re 称为"保险业的警钟"，但尚未转化为定价硬ening。

**趋势推断（低-中置信度）**：
- R2 假设"网络保险费率大幅上调"在 2026 H1 **未兑现**。
- 但这与"攻防不对称恶化"背离——潜在定价不足正在积累。**触发点**：一次系统性多基础设施同时受影响的事件（WEF 2026 警告的"连锁效应"），将迫使保费跳涨并出现政府支持的"网络再保险"机制（R2 2028-2029 假设维持，但可能提前）。
- 部分保险公司可能退出高风险行业（公用事业、医疗、金融服务）——与 R2 一致。

---

## 3. 地缘与监管演化

### 3.1 地缘——网络战作为战争前线（已确认）

**已发生**：EclecticIQ、CSIS 2026 报告确认，国家级/国家级黑客活动在区域冲突（俄乌、中东、台海周边）中已成为与动能攻击高度协同的前线。"IT Army of Ukraine"模式（平民黑客参与）扩散。

**趋势推断（中置信度）**：台海场景下，Volt Typhoon 预置的"战时破坏准备"性质未变。任何地缘升级都将直接催化美国国防网安 + 关键基础设施保护支出（CISA、FBI、NSA 预算）。**这是 #15 最硬的长期多头论据**——与短期监管周期无关。

### 3.2 主权数字基础设施——碎片化加速

**已发生**：
- S&P Global 2026 专题报告：计算主权依赖控制平面、密钥管理、供应链、软件栈的控制。
- EU、印度、中东推动"数字主权"——去美国化/去中国化的双轨。
- Spectro Cloud 等厂商推出"主权计算"产品线服务政府/国防。

**宏观含义**：全球网安市场不再是单一美国主导市场。**主权需求催生区域性玩家和本地化合规栈**——碎片化既是风险（厂商面临多法域成本）也是机会（区域玩家蓝海）。这与 #16 供应链碎片化议题强传导。

---

## 4. 跨议题传导（#19 AI 对 SaaS / 其他）

### 4.1 #15 ↔ #19 AI 对 SaaS：AI Agent 是下一个攻击面爆炸点

**已发生（高置信度）**：
- 2026 企业 AI Agent 安全面临三大风险：**prompt 注入、内存投毒、工具/MCP 滥用**（TrueFoundry、Help Net Security）
- 2026 实录：一个 GitHub PR 标题中的恶意指令导致 3 个独立 AI 编码代理执行有害操作（Luby）——**首个公开的 Agent 级供应链攻击实证**
- miniOrange 2026：AI Agent 主要风险——权限过度、弱凭证、prompt 注入、不安全工具集成、可见性差
- 传统安全工具对 Agent 攻击面"覆盖不足"（TrueFoundry）

**宏观传导链**：
```
#19 AI 对 SaaS 普及（AI Agent 走向生产）
  → 新增攻击面：Agent 权限/数据外泄/MCP/工具集成
  → 现有 EDR/SIEM 无法覆盖 Agent 执行层
  → 催生新安全品类：AI Agent Security（Pillar Security、Luby 等新玩家）
  → 反向催化 #15：每多一个 Agent 部署，安全支出需求随之上升
```

**趋势推断（中-高置信度）**：AI Agent Security 将成为 2027-2028 年网安市场增长最快的子品类之一。**#15 与 #19 是强正相关传导**——AI 应用越多，安全需求越大。R2 未充分识别这条传导链。

### 4.2 #15 ↔ #06 量子/PQC：加密敏捷性时间表
R2 提及 Q-Day 威胁。2026.06 Trump 发布 EO"Securing the Nation Against Advanced Cryptographic Attacks"（Ballotpedia），推动后量子加密迁移。这强化了 #15 的长期加密迁移支出流——与 #06 的传导不变。

### 4.3 #15 ↔ #16 供应链碎片化：SBOM 标准分化
US（OMB 撤销强制）vs EU（CRA 强制）vs 中印各自标准的分化，直接传导 #16 的供应链碎片化。SBOM 格式（SPDX/CycloneDX/自定义）和合规义务日益法域特定——OpenSSF 呼吁"统一、可操作的 SBOM 框架"。

### 4.4 #15 ↔ #04 地缘冲突：网络战是现代战争第一波
俄乌/台海预置未变，详见 3.1。

---

## 5. 对 R2 基线的冲击

| R2 基线假设 | 2026 H1 实证 | 冲击 |
|------------|-------------|------|
| 全球网安市场 $219-255B (2025) | Gartner $244B (2026)，+12-13% | ✅ 确认中段，路径正确 |
| 网安占 IT 预算 5-15% | 顶层口径 ~4%；企业口径 6-8% | ❗ **下修**——但反向意味着长期上行空间更大 |
| 国防网安 CAGR ~13% | 路径未变，Trump America First 可能加速 | ✅ 维持 |
| 关键基础设施保护 $154B→$197B | Volt/Salt Typhoon + 2026 攻击事件持续催化 | ✅ 维持 |
| 平均数据泄露成本 $4.88M 持续上升 | AI 攻击推高损失，路径不变 | ✅ 维持 |
| 网络保险"保费大幅上调" | 2024-2026 H1 保费软化（-5% Q4 2024） | ⚠️ **短期未兑现**；潜在定价不足在积累，系统性事件将触发 |
| AI 攻防双刃剑 | 攻击侧成本下降快于防御侧 | ❗ **下修中性假设**——不对称在恶化，利好防御侧长期支出 |
| NIS2/DORA/SEC 驱动合规支出 | EU 收紧兑现；US Trump 软化（OMB SBOM 撤销）部分抵消 | ✅ 净正向（EU 主导基线） |
| CrowdStrike 类中断风险 | 2026.01 股东诉讼被驳回——**关键正向**；但 EU Product Liability 2026.12 实施开启新责任 | ⚠️ 短期缓解、长期责任未消除 |

**未在 R2 但 2026 浮现的新因素**：
- AI Agent 攻击面（#19 传导）
- 监管大西洋分化（Trump 软化 vs EU 收紧）
- EU Product Liability Directive 覆盖软件/AI（2026.12）
- AI 工具花费 17x 于安全的比例（短期挤压）

---

## 6. 评级建议与长期视角

### 评级建议：维持"积极关注"，倾向上调至"超配/核心配置"

**维持/上调理由（结构性多头）**：
1. **攻防不对称在恶化**（AI 攻击成本下降快于防御）——结构性倒逼防御支出
2. **网安渗透率仅 ~4% IT 预算**——长期 TAM 上行空间大，处于早期渗透
3. **欧盟监管收紧不可逆**（NIS2/DORA/CRA/Product Liability 五法协同）——即使 Trump 软化美国联邦要求，跨国企业无法回退
4. **国家级威胁升级路径未变**（Volt/Salt/Flax/Brass 台风系列）——国防网安支出与短期政治周期脱钩
5. **AI Agent 普及带来新攻击面爆炸**（#19 传导）——催生全新安全子品类
6. **CrowdStrike 诉讼风险消除**（2026.01 股东案驳回）——平台化龙头估值压制解除

**风险因素（需监控）**：
1. **Trump 监管放松**可能短期压制美国联邦/合规驱动支出（OMB SBOM 撤销是信号）
2. **网络保险保费软化**可能误导企业低估风险，延迟安全投入（潜在定价不足积累）
3. **AI CapEx 挤压**（17x 比例）短期可能压制安全预算相对优先级
4. **估值**：CRWD/PANW 等 PS 倍数高，对利率敏感
5. **系统性事件黑天鹅**：一次多基础设施同时受影响的攻击可能同时利好（支出跳升）和利空（保险/责任重定价）

### 长期视角（5-10 年）

**TAM 终局假设（中置信度）**：
- 2030 全球网安市场：**$385-500B**（R2 区间下半段至上半段下沿）
- 网安占 IT 预算比例：从 ~4% 移向 **6-8%**（仍非 20%+ 极端假设；要达到更高需系统性事件催化）
- 网络保险市场：2030 **$30-40B**（R2 假设维持）
- AI Agent Security：2028 成为主流安全品类，目前 < $5B

**不确定性标注**：
- 高置信度：EU 监管收紧、Volt Typhoon 类威胁持续、AI 攻击成本下降
- 中置信度：市场 CAGR 12-15%、渗透率上行节奏、CrowdStrike 类责任演化
- 低置信度：Trump 政策最终方向、网络保险定价拐点时点、系统性事件触发窗口

---

## 7. 来源清单

### 市场规模与 IT 预算
- [Gartner: Worldwide IT Spending 2026 $6.15T](https://www.gartner.com/en/newsroom/press-releases/2026-02-03-gartner-forecasts-worldwide-it-spending-to-grow-10-point-8-percent-in-2026-totaling-6-point-15-trillion-dollars)
- [Gartner 2025.10 IT Spending Forecast $6.08T](https://www.gartner.com/en/newsroom/press-releases/2025-10-22-gartner-forecasts-worldwide-it-spending-to-grow-9-point-8-percent-in-2026-exceeding-6-trillion-dollars-for-the-first-time)
- [Louis Columbus: Gartner $244B Security Spending 2026](https://www.linkedin.com/pulse/gartner-projects-244-billion-security-spending-2026-ai-louis-columbus-dciec)
- [Picus: Optimize Cybersecurity Budget](https://www.picussecurity.com/resource/blog/optimize-cybersecurity-budget)
- [Elisity: 2026 Cybersecurity Budget Guide](https://www.elisity.com/blog/2026-cybersecurity-budget-complete-enterprise-planning-guide)
- [Software Strategies: Information Security Spending 2026 (17x AI ratio)](https://softwarestrategiesblog.com/2026/03/24/information-security-spending-2026/)
- [Cybersecurity Ventures: Spending 2031 (IDC US+EU 70%)](https://cybersecurityventures.com/wp-content/uploads/2023/11/CybersecuritySpending2031.pdf)

### 监管（US 转向 + EU 收紧）
- [White House: Trump Cyber Strategy EO 2026.06 AI Innovation & Security](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/)
- [Mayer Brown: Trump Cyber Strategy 2026.03](https://www.mayerbrown.com/en/insights/publications/2026/03/trump-administration-releases-cyber-strategy-for-america-and-related-executive-order-on-combatting-cybercrime)
- [Wiley Law: Trump EO Analysis](https://www.wiley.law/alert-President-Trump-Cyber-Mandate-Analysis-of-Executive-Order-on-Strengthening-US-Cybersecurity)
- [Wiley Law: OMB Rescinds Secure Software Development Mandate (2026.01.23)](https://www.wiley.law/alert-OMB-Rescinds-Secure-Software-Development-Mandate-in-Favor-of-a-Risk-Based-Approach)
- [GovCIO Media: OMB Memo SBOM optional](https://govciomedia.com/omb-memo-rescinds-mandatory-software-security-vetting/)
- [Congress.gov: EO 14306 Sustaining Cyber Efforts](https://www.congress.gov/crs_external_products/IN/HTML/IN12570.html)
- [Global Policy Watch: 2026 National Cyber Strategy + EO](https://www.globalpolicywatch.com/2026/03/white-house-releases-new-national-cyber-strategy-and-executive-order/)
- [Sidley: Cyber Strategy at AI Frontier](https://datamatters.sidley.com/2026/06/04/cyber-strategy-at-the-ai-frontier-president-trump-releases-executive-order-to-promote-advanced-artificial-intelligence-innovation-and-security/)
- [Ballotpedia: EO Securing Against Cryptographic Attacks](https://ballotpedia.org/Executive_Order:_Securing_the_Nation_Against_Advanced_Cryptographic_Attacks_(Donald_Trump,_2026))
- [SEC: Cybersecurity Risk Management Rules (2023.139)](https://www.sec.gov/newsroom/press-releases/2023-139)
- [V-Comply: SEC Cyber Disclosure Rules 2026](https://www.v-comply.com/sec-cybersecurity-disclosure-rules-in-2026/)
- [Holland & Knight: SEC 4-day Rule](https://www.hklaw.com/en/insights/publications/2023/07/sec-finalizes-cybersecurity-incident-and-governance-disclosure)
- [Orbiq: DORA vs NIS2 penalties](https://www.orbiqhq.com/eu-regulations/dora-vs-nis2)
- [Cleary Gottlieb: EU Product Liability Directive 2026.12](https://www.clearygottlieb.com/news-and-insights/publication-listing/the-new-eu-product-liability-reform-addressing-the-digital-age)
- [Lawyer Month 2026.06: EU Product Liability AI/Software](https://www.lawyer-monthly.com/2026/06/eu-product-liability-directive-ai-software-liability-risks/)

### 国家级威胁与 APT
- [CISA Advisory AA24-038A: PRC Volt Typhoon](https://www.cisa.gov/news-events/cybersecurity-advisories/aa24-038a)
- [NJCCIC: Salt Typhoon profile](https://www.cyber.nj.gov/threat-landscape/nation-state-threat-analysis-reports/china-linked-cyber-operations-targeting-us-critical-infrastructure/salt-typhoon)
- [Congress.gov CRS IF12798: Salt Typhoon policy](https://www.congress.gov/crs-product/IF12798)
- [Vectra AI: Salt Typhoon briefing](https://www.vectra.ai/resources/vectra-ai-threat-briefing-salt-typhoon)
- [CSIS: Significant Cyber Incidents 2026](https://www.csis.org/programs/strategic-technologies-program/significant-cyber-incidents)
- [Anapaya: Top 5 Critical Infrastructure Cyberattacks 2026](https://www.anapaya.net/blog/top-5-critical-infrastructure-cyberattacks)

### 网络保险
- [Gallagher: 2026 Cyber Insurance Market Outlook PDF](https://www.ajg.com/-/media/files/gallagher/us/news-and-insights/2025/2026-cyber-insurance-market-outlook.pdf)
- [Munich Re: Cyber Insurance Risks and Trends 2026](https://www.munichre.com/en/insights/cyber/cyber-insurance-risks-and-trends-2026.html)
- [S&P Global: Cyber Insurance Market Outlook 2026](https://www.spglobal.com/ratings/en/regulatory/article/cyber-insurance-market-outlook-2026-resilient-earnings-tougher-competition-pockets-of-growth-s101658506)
- [Marsh: US Cyber Insurance Q4 2024 rates -5%](https://www.marsh.com/en/services/cyber-risk/insights/cyber-insurance-market-update.html)
- [Security.org: Cyber Insurance Statistics 2026 ($22.5B)](https://www.security.org/insurance/cyber/statistics/)
- [CNI Solutions: Lower Premiums ≠ Lower Risk](https://cnicsolutions.com/statistics/cybersecurity/cyber-insurance-statistics-2026/)
- [Geneva Association: Cyber Resilience Through Insurance](https://www.genevaassociation.org/publication/cyber/strengthening-cyber-resilience-through-insurance)
- [Gen Re: CrowdStrike wake-up call for insurers](https://www.genre.com/us/knowledge/publications/2025/february/the-crowdstrike-incident-a-wake-up-call-for-insurers-en)

### CrowdStrike 中断后续
- [Wikipedia: 2024 CrowdStrike IT Outages](https://en.wikipedia.org/wiki/2024_CrowdStrike-related_IT_outages)
- [Reuters 2026.01.14: CrowdStrike defeats shareholder lawsuit](https://www.reuters.com/legal/government/crowdstrike-defeats-shareholder-lawsuit-over-huge-software-outage-2026-01-14/)
- [Reed Smith: CrowdStrike insured losses $400M-$1.5B](https://www.reedsmith.com/our-insights/blogs/the-policyholder-perspective/102k33j/recovering-from-the-crowdstrike-outage/)
- [CrowdStrike blog: Customer Commitment Package $60M+](https://www.crowdstrike.com/en-us/blog/to-our-customers-and-partners/)
- [Burges Salmon: CrowdStrike Regulatory Implications](https://www.burges-salmon.com/our-thinking/crowdstrike-incident-regulatory-implications-and-lessons-learned/)
- [CSIS Analysis: Biden National Cybersecurity Strategy](https://www.csis.org/analysis/biden-harris-administrations-national-cybersecurity-strategy)

### AI 攻防经济学
- [WEF 2026.02: AI supercharging cyber fraud crisis](https://www.weforum.org/stories/2026/02/ai-supercharging-global-cyber-fraud-crisis-could-also-solve-it/)
- [SQ Magazine: AI Cyber Attacks Statistics ($193B)](https://sqmagazine.co.uk/ai-cyber-attacks-statistics/)
- [ZeroThreat AI: Deepfake & AI Phishing 2026 ($547.2M H1)](https://zerothreat.ai/blog/deepfake-and-ai-phishing-statistics)
- [BabyBots: AI Agent Prompt Injection ($2.3B 2025, 73% deployments)](https://www.babybots.ai/blog/ai-agent-security-prompt-injection-enterprise)
- [Pillar Security: 3 AI Security Predictions 2026](https://www.pillar.security/blog/the-new-ai-attack-surface-3-ai-security-predictions-for-2026)
- [Help Net Security 2026.02: AI Agent Security Risks](https://www.helpnetsecurity.com/2026/02/23/ai-agent-security-risks-enterprise/)
- [TrueFoundry: Enterprise AI Agent Security Buyer's Guide](https://www.truefoundry.com/blog/enterprise-ai-agent-security-solutions)
- [Luby: AI Agent Execution Layer Risk 2026 (GitHub PR incident)](https://blog.luby.co/ai-agent-security-why-the-execution-layer-is-the-biggest-enterprise-risk-in-2026/)
- [miniOrange: AI Agent Security Risks 2026](https://www.miniorange.com/blog/ai-agent-security-risks/)
- [Shumaker: AI-Driven Cyber Threats 2026](https://www.shumaker.com/insight/analysis-of-new-cyber-threats-artificial-intelligence-ai%E2%80%91driven-risks-accelerating-in-2026/)
- [DeepStrike: AI Cybersecurity Threats 2026](https://deepstrike.io/blog/ai-cybersecurity-threats-2025)
- [The Global Economics 2026.06: AI-Powered Cyber Threats](https://theglobaleconomics.com/2026/06/22/ai-powered-cyber-threats/)

### 供应链 / SBOM / 主权
- [CISA: SBOM hub](https://www.cisa.gov/topics/information-communications-technology-supply-chain-security/sbom)
- [Sonatype: 2026 State of Software Supply Chain (CRA)](https://www.sonatype.com/blog/what-the-2026-state-of-the-software-supply-chain-report-reveals-about-regulation)
- [Cloudsmith: 2026 Guide to Software Supply Chain Security](https://cloudsmith.com/blog/the-2026-guide-to-software-supply-chain-security-from-static-sboms-to-agentic-governance)
- [Sbomify: Ultimate SBOM Compliance Guide 2026](https://sbomify.com/compliance/)
- [OpenSSF: SBOMs in the Era of CRA](https://openssf.org/blog/2025/10/22/sboms-in-the-era-of-the-cra-toward-a-unified-and-actionable-framework/)
- [RunSafe Security: Global SBOM Requirements Guide](https://runsafesecurity.com/blog/sbom-requirements-global-guide/)
- [S&P Global: Compute Sovereignty](https://www.spglobal.com/en/research-insights/special-reports/compute-sovereignty-strategic-importance-of-digital-infrastructure)
- [Industrial Cyber: Supply Chain Risk in Cyber Sovereignty](https://industrialcyber.co/features/supply-chain-risk-takes-center-stage-in-cyber-sovereignty-as-hidden-dependencies-long-tail-vendors-come-into-focus/)
- [Spectro Cloud: Sovereign Compute for Defense](https://www.spectrocloud.com/government/sovereign-compute)

### 零信任 / SASE / 勒索
- [TechnologyMatch: Zscaler vs Netskope vs PANW vs Cato 2026](https://technologymatch.com/blog/zscaler-vs-netskope-vs-palo-alto-vs-cato-the-sase-selection-guide-2026)
- [Zscaler: Public Sector Summit 2026](https://www.zscaler.com/public-sector-summit-on-demand)
- [Zscaler: FedRAMP Authorization](https://www.zscaler.com/privacy-compliance/customer-compliance/fedramp)
- [Etr Research: SASE Convergence 2026](https://research.etr.ai/blog-observatory/sase-security-further-convergence-expected-among-leaders-in-2026)
- [IBM Think: When Ransomware Kills](https://www.ibm.com/think/insights/when-ransomware-kills-attacks-on-healthcare-facilities)
- [Industrial Cyber / Cyfirma: Healthcare ransomware +8.5% QoQ](https://industrialcyber.co/ransomware/healthcare-sector-faces-escalating-ransomware-supply-chain-and-apt-risks-as-cyber-threats-intensify-cyfirma-warns/)
- [Canadian Centre for Cyber Security: National Threat Assessment 2025-2026](https://www.cyber.gc.ca/en/guidance/national-cyber-threat-assessment-2025-2026)
- [Halcyon: Ransomware Public Health Crisis](https://www.halcyon.ai/resources/whitepapers/ransomware-a-public-health-crisis-white-paper)
- [EclecticIQ: Escalating Cyber Risk in Regional Conflicts 2026](https://blog.eclecticiq.com/the-escalating-cyber-risk-landscape-in-regional-conflicts-strategic-actions-for-2026)
