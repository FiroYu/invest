# Researcher B — 催化事件研究（R3, 2026.07.10）

> **议题**：#02 光学路线芯片互联与制造范式转移
> **周期**：R2 基线 2026.05.25 → R3 刷新 2026.07.10（覆盖 2026 H1，重点 5-7 月）
> **研究员**：B 催化（事件/政策/产品发布/M&A/标准/里程碑）
> **工具回退说明**：anysearch 与 firecrawl 当日额度均耗尽，本轮以 WebSearch（Z.ai web_search_prime）为主，来源已逐条标注。

---

## 一、执行摘要（按重要性排序）

2026 H1 是本议题**催化密度最高的半年**，且催化方向**高度一致地确认基线判断**："CPO 量产元年"不是宣传口号，而是正在兑现的制造拐点。头号催化：

### 头号催化（确认制造业级拐点）

1. **NVIDIA $40亿战略投资 Lumentum + Coherent（2026.03.02）** — 各$20亿成长性股权，锁定激光/硅光供应链。这是 NVIDIA 将光子学**垂直整合**的最强信号：当 GPU 的瓶颈从"计算"转移到"光"时，NVIDIA 选择直接持有光的核心资产。**直接利好 CPO 路线、利好激光/硅光上游。**

2. **TSMC COUPE（Compact Universal Photonic Engine）2026 量产** — SoIC-X 3D 堆叠（电芯片叠在光芯片上），2025 年小尺寸可插拔认证 → 2026 年 CoWoS-based CPO 集成。SEMI 正式将 2026 定为"规模化硅光部署元年"。三星 CPO turnkey 目标 2029（落后 TSMC 3 年）。

3. **NVIDIA Quantum-X Photonics（InfiniBand CPO）2026 初出货 + Spectrum-X Photonics（Ethernet CPO）2H 2026** — 首批 CPO 交换机已进入量产。Quantum-X800 Q3450-LD 提供 144×800G 端口、115 Tbps 吞吐。基于 TSMC COUPE 硅光技术。

### 产业级催化（加速但不构成拐点本身）

4. **Marvell 完成 $32.5亿收购 Celestial AI（2026.02 交割）** — $10亿现金 + $22.5亿股票，重塑光子互联格局。Celestial 的"Photonic Fabric"归入 Marvell 的 scale-up 连接产品线。

5. **Ayar Labs $5亿 Series E（2026.03.12）** — 累计融资 ~$8.7亿，新竹设厂扩量产。NVIDIA/AMD/Intel 此前联合投$1.55亿。入选 Fast Company 2026 最创新公司（计算类前五）。

6. **OFC 2026（03.15-19，洛杉矶）= 1.6T 硅光阅兵**：Hyper Photonix 1.6T SiP 收发器 Q2 2026 量产；Coherent 多技术路线 1.6T；OpenLight III-V 异质集成；Tower SiPh 平台；Arista 1.6T LPO；Lightmatter 1.6T/光纤纪录 + Passage L20（NPO/OBO）。

7. **GTC 2026（03）Vera Rubin 平台** — 7 芯片量产，年度发布节奏确认（2026 Vera Rubin → 2027 Rubin Ultra → 2028 Feynman 硅光革命）。Spectrum-X Ethernet Photonics MCM 已捆绑进六芯片 Rubin 平台（CES 2026 发布）。

### 验证性催化（确认趋势但非新增量）

8. **中国光模块双雄 Q1 2026 爆发**：中际旭创营收 194.96 亿元（+192% YoY），新易盛 83.38 亿元（+106%），天孚通信 13.30 亿元（+41%）。1.6T 毛利率 52-55%。瓶颈在产能不在需求（"甜蜜的烦恼"）。

9. **铜的最后反击 = 计划性共存，非威胁**：黄仁勋 GTC 2026 明确"铜+光 2026-2027 共存，2028 全面转向光"，并喊话"需要更多铜产能"。CPC（共封装铜）无源用于机柜内 scale-up；Semtech OFC 2026 演示 1.6T ACC（224G）。这是**既定过渡节奏**，不动摇 CPO 时间表。

### 对评级的影响

R2 基线为隐含"积极关注/技术关注"。本轮催化**强烈支持上调倾向**：
- 制造业拐点已被三重验证（TSMC 量产 + NVIDIA CPO 出货 + NVIDIA 垂直整合供应链）
- 需求端爆发已被财报验证（中际旭创 +192%）
- 铜的反击是过渡性共存而非替代威胁
- **建议：进入"有条件通过"**——条件为 CPO 良率/热管理在 2H 2026 量产爬坡中得到规模化验证（见第四节催化日历）

---

## 二、事件详表（2026 H1）

| # | 日期 | 事件 | 类别 | 影响 | 来源 |
|---|------|------|------|------|------|
| 1 | 2026.02 | Marvell 完成 $32.5B 收购 Celestial AI（$10亿现金+$22.5亿股票） | M&A | 光子互联"Photonic Fabric"归入 Marvell scale-up 产品线，重塑竞争格局 | [SDxCentral](https://www.sdxcentral.com/news/marvell-completes-325b-acquisition-of-photonic-startup-celestial-ai/); [Photonics Spectra](https://www.photonics.com/Articles/Marvell-to-Acquire-Celestial-AI-for-33B/a71734) |
| 2 | 2026.03.02 | **NVIDIA $40亿投资 Lumentum + Coherent（各$20亿成长股权）** | 资本/供应链 | 垂直整合激光/硅光供应链；GPU 巨头直接持有光的核心资产 | [Photonics.com](https://www.photonics.com/Articles/NVIDIA-Invests-4B-in-Coherent-Lumentum/a72014); [NVIDIA Newsroom](http://nvidianews.nvidia.com/news/nvidia-announces-strategic-partnership-with-lumentum-to-develop-state-of-the-art-optics-technology) |
| 3 | 2026.03.12 | Ayar Labs $5亿 Series E（Neuberger Berman 领投），累计融资 ~$8.7亿，新竹设厂 | 融资 | CPO 独角兽进入量产爬坡；NVIDIA/AMD/Intel 三巨头背书 | [Ayar Labs](https://ayarlabs.com/news/ayar-labs-closes-500m-series-e-accelerates-volume-production-of-co-packaged-optics/) |
| 4 | 2026.03 | GTC 2026：Vera Rubin 平台 7 芯片量产；年度节奏确认（2027 Rubin Ultra / 2028 Feynman 硅光）；Spectrum-X Ethernet Photonics 捆绑 Rubin | 产品/里程碑 | CPO 正式成为 NVIDIA AI 工厂标配层；2028 Feynman = 硅光革命节点 | [TradingKey](https://www.tradingkey.com/analysis/stocks/us-stocks/261687829-nvidia-gtc-2026-how-vera-rubin-system-will-shape-next-decade-tradingkey); [StorageReview](https://www.storagereview.com/news/nvidia-gtc-2026-rubin-gpus-groq-lpus-vera-cpus-and-what-nvidia-is-building-for-trillion-parameter-inference) |
| 5 | 2026.03 | NVIDIA Quantum-X Photonics（InfiniBand CPO）2026 初出货；Spectrum-X Photonics（Ethernet CPO）2H 2026；CPO 交换机已量产 | 量产里程碑 | 首批 CPO 交换机进入客户手中（Lambda 获样品），CPO 元年兑现 | [NVIDIA Developer Blog](https://developer.nvidia.com/blog/scaling-ai-factories-with-co-packaged-optics-for-better-power-efficiency/); [Lambda](https://lambda.ai/blog/silicon-photonics-for-ai-clusters-performance) |
| 6 | 2026.03.15-19 | **OFC 2026（洛杉矶）= 1.6T 硅光阅兵**：Hyper Photonix 1.6T SiP（Q2 2026 量产）、Coherent 多路线 1.6T、OpenLight III-V 异质集成、Tower SiPh、Arista 1.6T LPO + XPO、Lightmatter 1.6T/光纤纪录 + Passage L20 | 行业展会 | 1.6T 从路线图走向量产；200G/lane 架构确立；LPO/LRO 与 CPO 并行 | [OFC](https://www.ofcconference.org/news-media/exhibitor-news/hyper-photonix-showcases-next-generation-1-6t-sip-optical-transceivers-at-ofc-2026-conference-%25E2%2580%2593-boot/); [Light Reading](https://www.lightreading.com/optical-networking/hyper-photonix-showcases-1-6t-sip-optical-transceivers-at-ofc-2026) |
| 7 | 2026.03 | Semtech OFC 2026 演示 1.6T ACC（CopperEdge GN8234 Redriver，224G 实时流量，NVIDIA 系统） | 铜反击 | 有源铜缆延长铜寿命至 1.6T/224G；铜与光并行而非互斥 | [Semtech Blog](https://blog.semtech.com/ofc-2026-semtech-advances-the-future-of-ai-data-center-optical-and-active-copper-interconnects) |
| 8 | 2026.Q1 | 中际旭创 Q1 营收 194.96 亿元（+192% YoY）；新易盛 83.38 亿元（+106%）；天孚通信 13.30 亿元（+41%） | 财报/需求 | AI 光模块需求爆发；瓶颈在产能非需求；1.6T 毛利率 52-55% | [21财经](https://www.21jingji.com/article/20260503/herald/cbdd6cc2ee8be8fa2cac353b5f2dd4ea.html) |
| 9 | 2026.04 | TSMC COUPE（Compact Universal Photonic Engine）确认 2026 量产；SoIC-X 3D 堆叠；CoWoS-based CPO 集成 | 量产/代工 | 代工龙头量产硅光引擎，SEMI 定 2026 为硅光规模化元年；三星落后至 2029 | [TrendForce](https://www.trendforce.com/news/2026/04/01/news-silicon-photonics-race-intensifies-as-tsmc-targets-2026-coupe-production-samsung-eyes-2029-cpo-turnkey/); [Design-Reuse](https://www.design-reuse.com/news/202530302-silicon-photonics-race-intensifies-as-tsmc-targets-2026-coupe-production-samsung-eyes-2029-cpo-turnkey/) |
| 10 | 2026.H1 | Broadcom 第三代 200G/lane CPO（Humboldt 路线延续）；CEO Hock Tan 态度谨慎，目标 400G→800G→1.6T | 产品 | CPO 生态成熟，但 Broadcom 节奏比 NVIDIA 保守 | [Broadcom CPO](https://www.broadcom.com/info/optics/cpo); [Institution of Electronics](https://institutionofelectronics.ac.uk/where-co-packaged-optics-cpo-technology-stands-in-2026/) |
| 11 | 2026.H1 | OIF CEI-448G 框架推进；IEEE 802.3 E4AI ad hoc（400G/lane PHY for AI）；Anritsu+Semtech OFC 2026 验证 224G/448G 驱动放大器 | 标准 | 224G 标准化落地支撑 1.6T；448G 为下一前沿（2027+） | [OIF](https://www.oiforum.com/technical-work/current-work/); [Broadcom DesignCon26](https://www.broadcom.com/blog/broadcom-power-efficiency-innovations-shine-at-designcon26); [Anritsu](https://www.anritsu.com/en-us/test-measurement/news/news-releases/2026/2026-03-16-us01) |
| 12 | 2026.H1 | Lightmatter Passage M1000（3D 光子中介层）+ Passage L20（NPO/OBO 统一光引擎）+ 1.6T/光纤纪录；客户评估套件出货 | 光子计算/互联 | 光子互联独角兽（$8.5亿融资，$44亿估值）进入客户测试阶段 | [Lightmatter](https://lightmatter.co/press-release/lightmatter-achieves-record-1-6-tbps-per-fiber-to-accelerate-ai-optical-interconnect/); [Lightmatter L20](https://lightmatter.co/press-release/lightmatter-expands-photonic-interconnect-roadmap-with-passage-l20-unified-optical-engine-for-npo-and-obo-applications/) |
| 13 | 2026.H1 | Arista 推 XPO（extra dense pluggable optics）面向 1.6T；800G LPO（LPO-800G-2DR4）部署；Meta 800G LPO 订单 | 可插拔生态 | LPO/XPO 延长可插拔寿命，与 CPO 在 1.6T 形成分工（短距 LPO / 长距 CPO） | [Arista OFC 2026](https://events.arista.com/ofc-2026); [Arista 800G FAQ](https://www.arista.com/assets/data/pdf/Datasheets/Arista-800G_Optics_FAQ.pdf) |
| 14 | 2026.H1 | 黄仁勋 GTC 2026 "copper-and-optics roadmap"：2026-2027 铜光共存，2028 全面转光；"需要更多铜产能" | 战略口径 | 铜的反击是计划性过渡，非对 CPO 的否定；CPC 无源铜用于机柜内 | [Futu](https://q.futunn.com/en/feed/116690920669588); [SDxCentral](https://www.sdxcentral.com/news/nvidia-backs-copper-in-next-gen-interconnects-amid-push-into-co-packaged-optics/) |
| 15 | 2026.H1 | High-NA EUV：Intel 领先（首台二代机，14A 节点 2026）；TSMC 延迟（A16/A14 不用 High-NA，成本顾虑）；ASML 称量产 2027-28 | 光刻演进 | High-NA 是连续演进非范式转移（与基线判断一致）；Intel vs TSMC 路线分化 | [TrendForce](https://www.trendforce.com/news/2026/02/16/news-asmls-high-na-euv-for-2027-28-which-giants-are-betting-big-intel-samsung-sk-hynix-or-tsmc/); [Tom's Hardware](https://www.facebook.com/tomshardware/posts/tsmc-reaffirmed-that-it-will-not-use-high-na-euv-lithography-for-its-upcoming-a1/1105668388264245/) |

---

## 三、催化强度评级

### ★★★★★ 制造业级拐点（范式转移正在发生）

| 事件 | 评级理由 |
|------|----------|
| NVIDIA $40亿投资 Lumentum+Coherent | GPU 巨头用真金白银声明：光的供应链是下一个必须掌控的战略资源。垂直整合信号无出其右 |
| TSMC COUPE 2026 量产 | 全球代工龙头将硅光引擎推过量产门槛，CPO 不再是 PPT。三星落后 3 年坐实 TSMC 垄断延伸 |
| NVIDIA CPO 交换机量产出货（Quantum-X） | 首批 CPO 交换机进入客户手中，CPO 元年从概念变实物 |

### ★★★★ 产业催化（强确认但不单独构成拐点）

| 事件 | 评级理由 |
|------|----------|
| Marvell $32.5亿收购 Celestial AI（交割） | 重塑光子互联格局，大厂并购验证赛道价值 |
| Ayar Labs $5亿 Series E + 新竹量产 | 独角兽级融资 + 三巨头背书，量产爬坡启动 |
| OFC 2026 1.6T 硅光阅兵 | 全行业 1.6T 从路线图走向量产，200G/lane 架构确立 |
| 中际旭创 Q1 +192% | 需求端爆发验证，中国光模块定价权坐实 |

### ★★★ 产业催化（方向确认，增量有限）

| 事件 | 评级理由 |
|------|----------|
| GTC 2026 Vera Rubin + 年度节奏 | 平台确认但 CPO 细节未超预期 |
| Lightmatter Passage L20 + 1.6T/光纤 | 客户测试阶段，尚无首个大客户商用部署公告 |
| Broadcom 第三代 CPO 200G/lane | 生态成熟但 CEO 谨慎，节奏慢于 NVIDIA |
| OIF CEI-448G / IEEE 224G 标准化 | 标准推进支撑 1.6T，448G 尚远 |

### ★★ 噪音/过渡（不改变方向）

| 事件 | 评级理由 |
|------|----------|
| 铜反击（CPC/AEC/ACC） | 计划性共存，2028 才全面转光；非威胁 |
| High-NA EUV 2026 | 连续演进非范式转移；Intel/TSMC 路线分化但与光互联主线无关 |
| LPO/XPO 势头 | 延长可插拔寿命，与 CPO 分工而非竞争 |

---

## 四、下一个 6 个月关键催化日历（2026.07 - 2026.12）

| 时间 | 事件 | 关注点 | 潜在影响 |
|------|------|--------|----------|
| 2026.Q3 | NVIDIA Spectrum-X Photonics（Ethernet CPO）量产出货 | 首批以太网 CPO 交换机交付客户；与 Quantum-X（InfiniBand）形成双产品线 | ★★★★★ 若如期出货，CPO 元年彻底坐实 |
| 2026.Q3 | 中际旭创/新易盛 H1 财报（8月底） | 1.6T 出货量、毛利率、产能爬坡 | ★★★★ 验证"瓶颈在产能非需求" |
| 2026.07.26-30 | Design Automation Conference（Long Beach） | Lightmatter 等光子计算厂商展示 | ★★ 技术社区信号 |
| 2026.08.19-21 | Hot Interconnects 2026（虚拟） | Lightmatter 已列为演讲者 | ★★ |
| 2026.Q3-Q4 | TSMC COUPE 量产爬坡 / 良率数据 | CoWoS-based CPO 集成良率；热管理 | ★★★★★ 良率是 CPO 能否规模化的关键变量 |
| 2026.Q4 | Ayar Labs Optical I/O 首个大客户部署公告？ | 是否宣布首个 hyperscaler 商用 | ★★★★ 若出现，光互联商业化拐点 |
| 2026.09 | ECOC 2026（欧洲光通信大会） | 3.2T 路线图、下一代硅光 | ★★★ 3.2T 时间表明确化 |
| 2026 下半年 | IEEE 802.3 E4AI（400G/lane PHY）标准进展 | 是否进入投票/批准阶段 | ★★ 标准前置 |
| 2026 下半年 | NVIDIA Feynman（2028）硅光细节 | GTC 2027 前是否有预热 | ★★ 远期叙事 |
| 2026 下半年 | 中国工信部光芯片/CPO 政策落地 | 《电子信息制造业稳增长方案》执行细则、补贴 | ★★★ 中国侧政策催化 |
| 2026 下半年 | Lightmatter 下一轮融资 / IPO 信号 | 是否启动 IPO 进程（$44亿估值） | ★★★ 资本市场信号 |

### 关键验证窗口（决定评级能否从"有条件通过"升至"通过"）

1. **CPO 量产良率**（2H 2026）：TSMC COUPE + NVIDIA Spectrum-X Photonics 的 CoWoS 集成良率是否达到经济规模（>70%）。这是 CPO 从"样品"到"商品"的唯一硬约束。
2. **首个光互联商用部署**：Ayar Labs 或 Lightmatter 是否宣布首个 hyperscaler 级商用客户（非评估套件）。
3. **3.2T 路线图**：ECOC 2026 是否给出 3.2T 明确量产时间（2027/2028），确认光学路线不可逆。

---

## 五、对基线关键问题的回答

| 基线问题（R3 需验证） | 回答 |
|----------------------|------|
| 1. CPO 量产元年兑现度？ | **兑现中**。TSMC COUPE 量产、NVIDIA Quantum-X 出货、Spectrum-X CPO 交换机量产。良率/热管理待 2H 2026 规模化验证 |
| 2. 1.6T 部署 / 3.2T 时间表？ | **1.6T 规模部署中**（Hyper Photonix Q2 量产、中际旭创出货、花旗预测 2027 年 1.6T 需求 1920 万片）。3.2T 待 ECOC 2026 明确 |
| 3. 光子计算商业化？ | **客户测试阶段，无首个大客户商用**。Lightmatter Passage 评估套件出货、1.6T/光纤纪录；Ayar Labs 量产爬坡中 |
| 4. 中国光模块双雄？ | **爆发**。中际旭创 Q1 +192%、新易盛 +106%、1.6T 毛利率 52-55%；瓶颈在产能 |
| 5. High-NA EUV？ | **Intel 领先（14A 2026），TSMC 延迟（成本顾虑，2027-28）**。连续演进，非范式转移（与基线一致） |
| 6. 铜的最后反击？ | **计划性共存，非威胁**。黄仁勋明确 2026-2027 铜光共存、2028 全面转光。CPC/AEC/ACC 延长铜寿命但不改变方向 |
| 7. 估值与配置？ | **强烈支持上调**。NVIDIA $40亿垂直整合 + 中国双雄财报爆发 = 产业共识与资本共识双重确认。建议进入"有条件通过" |

---

## 六、来源汇总

- NVIDIA Official: [Silicon Photonics](https://www.nvidia.com/en-us/networking/products/silicon-photonics/) / [Press Release](https://investor.nvidia.com/news/press-release-details/2025/NVIDIA-Announces-Spectrum-X-Photonics-Co-Packaged-Optics-Networking-Switches-to-Scale-AI-Factories-to-Millions-of-GPUs/default.aspx)
- NVIDIA $4B Lumentum/Coherent: [Photonics.com](https://www.photonics.com/Articles/NVIDIA-Invests-4B-in-Coherent-Lumentum/a72014) / [NVIDIA Newsroom](http://nvidianews.nvidia.com/news/nvidia-announces-strategic-partnership-with-lumentum-to-develop-state-of-the-art-optics-technology) / [Futurum Group](https://futurumgroup.com/insights/nvidias-4b-optics-bet-signals-photonics-as-ais-next-bottleneck/)
- TSMC COUPE: [TrendForce](https://www.trendforce.com/news/2026/04/01/news-silicon-photonics-race-intensifies-as-tsmc-targets-2026-coupe-production-samsung-eyes-2029-cpo-turnkey/) / [Design-Reuse](https://www.design-reuse.com/news/202530302-silicon-photonics-race-intensifies-as-tsmc-targets-2026-coupe-production-samsung-eyes-2029-cpo-turnkey/) / [SEMI](https://www.creating-nanotech.com/en-US/newsc302-semi-2026-marks-the-inaugural-year-for-scaled-silicon-photonics-deployment-optical-interconnects-key-to-mass-production)
- Marvell/Celestial AI: [SDxCentral](https://www.sdxcentral.com/news/marvell-completes-325b-acquisition-of-photonic-startup-celestial-ai/) / [Counterpoint](https://counterpointresearch.com/en/insights/Celestial-AI-Acquisition-Perfectly-Positions-Marvell-For-Upcoming-Multi-Rack-Scale-Up-Boom)
- Ayar Labs: [Series E PR](https://ayarlabs.com/news/ayar-labs-closes-500m-series-e-accelerates-volume-production-of-co-packaged-optics/) / [Fast Company 2026](https://ayarlabs.com/news/ayar-labs-named-to-fast-companys-list-of-the-worlds-most-innovative-companies-of-2026/)
- OFC 2026: [Hyper Photonix](https://www.ofcconference.org/news-media/exhibitor-news/hyper-photonix-showcases-next-generation-1-6t-sip-optical-transceivers-at-ofc-2026-conference-%25E2%2580%2593-boot/) / [Lightmatter 1.6T](https://www.ofcconference.org/news-media/exhibitor-news/lightmatter-achieves-record-1-6-tbps-per-fiber-to-accelerate-ai-optical-interconnect/) / [OFC Wrap-Up](https://iamfabian.substack.com/p/ofc-2026-wrap-up)
- GTC 2026: [TradingKey](https://www.tradingkey.com/analysis/stocks/us-stocks/261687829-nvidia-gtc-2026-how-vera-rubin-system-will-shape-next-decade-tradingkey) / [StorageReview](https://www.storagereview.com/news/nvidia-gtc-2026-rubin-gpus-groq-lpus-vera-cpus-and-what-nvidia-is-building-for-trillion-parameter-inference)
- 中国光模块: [21财经](https://www.21jingji.com/article/20260503/herald/cbdd6cc2ee8be8fa2cac353b5f2dd4ea.html)
- 铜反击: [Futu](https://q.futunn.com/en/feed/116690920669588) / [Semtech OFC 2026](https://blog.semtech.com/ofc-2026-semtech-advances-the-future-of-ai-data-center-optical-and-active-copper-interconnects) / [Marvell CPC](https://www.marvell.com/blogs/co-packaged-copper-extending-scale-up-networks.html)
- High-NA EUV: [TrendForce](https://www.trendforce.com/news/2026/02/16/news-asmls-high-na-euv-for-2027-28-which-giants-are-betting-big-intel-samsung-sk-hynix-or-tsmc/)
- Standards: [OIF](https://www.oiforum.com/technical-work/current-work/) / [Broadcom DesignCon26](https://www.broadcom.com/blog/broadcom-power-efficiency-innovations-shine-at-designcon26) / [Anritsu](https://www.anritsu.com/en-us/test-measurement/news/news-releases/2026/2026-03-16-us01)
- Lightmatter: [Passage M1000](https://lightmatter.co/press-release/lightmatter-unveils-passage-m1000-photonic-superchip-worlds-fastest-ai-interconnect/) / [Passage L20](https://lightmatter.co/press-release/lightmatter-expands-photonic-interconnect-roadmap-with-passage-l20-unified-optical-engine-for-npo-and-obo-applications/)
- Broadcom CPO: [Broadcom CPO page](https://www.broadcom.com/info/optics/cpo) / [Institution of Electronics](https://institutionofelectronics.ac.uk/where-co-packaged-optics-cpo-technology-stands-in-2026/)
- LPO/XPO: [Arista OFC 2026](https://events.arista.com/ofc-2026) / [Arista 800G FAQ](https://www.arista.com/assets/data/pdf/Datasheets/Arista-800G_Optics_FAQ.pdf)
