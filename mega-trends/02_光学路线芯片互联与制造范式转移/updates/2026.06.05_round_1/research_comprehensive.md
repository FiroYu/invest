# 课题#02「光学路线芯片互联与制造范式转移」— 综合研究报告 (Round 1)

> **分析日期**: 2026年6月5日
> **研究轮次**: Round 1（综合研究）
> **上次评级**: 有条件通过
> **研究方法**: 2026年5-6月最新行业动态搜索 + 已有README交叉验证

---

## 一、执行摘要

**一句话判断：光学互联范式转移已从「即将发生」升级为「已经发生」。2026年4月TSMC COUPE平台正式进入量产，NVIDIA已开始出货CPO交换机，产业临界点已被突破。**

本次研究在2026年5-6月最新行业动态基础上确认：TSMC COUPE（Compact Universal Photonic Engine）硅光子平台已于2026年4月正式量产，首代产品1.6Tbps OSFP光引擎，NVIDIA和Broadcom为第一批发货客户。NVIDIA在2026年3月向Coherent和Lumentum合计投资$40亿，并宣布Spectrum-X/Quantum-X CPO交换机2026H2出货，Feynman架构（2028）将集成NVLink CPO。这一系列里程碑标志着光学互联从「实验室→商业化」的关键过渡已完成。

**核心矛盾变化：** 上次评级时核心关注是「CPO能否量产」。本轮确认：量产已启动。新的核心矛盾转向——(1) 先进封装产能瓶颈（SoIC/CoWoS被GPU、HBM和光子学三方争夺），(2) CPO测试良率仍是量产规模化的最大障碍，(3) 铜-光共存格局至少持续到2028年。

---

## 二、2026年5-6月最新关键动态

### 2.1 TSMC COUPE量产正式启动 ★★★

**事件：** 2026年4月1日，TSMC在SEMI硅光子产业联盟会议上正式宣布COUPE平台从开发阶段迈入商业量产。COO Kevin Zhang在2026年5月Technology Symposium Hsinchu场次将COUPE定位为「AI芯片下一步的关键词」。

| 关键参数 | 详情 |
|---------|------|
| 封装方案 | SoIC-X face-to-face混合键合，将EIC直接堆叠在PIC上方 |
| 首代速率 | 1.6 Tbps双向（8路200G PAM4 per side） |
| 连接标准 | OSFP连接器 |
| 第二代 | 2027年集成至CoWoS，目标6.4 Tbps主板级 |
| 第三代 | 目标12.8 Tbps处理器封装内 |
| SoIC产能 | 2026年底目标30,000-40,000片/月 |
| COUPE on Substrate | 2026H2量产（将COUPE扩展至基板级） |

**关键瓶颈：** 先进封装产能正在成为比芯片制程更稀缺的资源。光子学（COUPE）与GPU（CoWoS-S/R）和HBM（CoWoS-L）三方争夺SoIC和CoWoS产线。光子学现在是「另一个排队抢TSMC先进封装产能的客户」。

**来源：** TSMC 2026 Technology Symposium; TrendForce (2026.05.18); NewMaxx/Borecraft (2026.06.01); Machine Herald (2026.04.07)

### 2.2 NVIDIA：$40亿光子学投资 + CPO交换机开始出货 ★★★

**事件链：**

1. **2026年3月**：NVIDIA向Coherent Corp和Lumentum Holdings各投资$20亿（合计$40亿），并签署多年采购协议以保证优先获取先进激光和光学组件。时机选择正值OFC 2026之前，信号明确。

2. **GTC 2026**：Jensen Huang提前约5年加速光学路线图。推出：
   - **Spectrum-X Photonics**（以太网CPO交换机）
   - **Quantum-X Photonics**（InfiniBand CPO交换机）
   - 每台交换机400 Tb/s聚合吞吐量
   - 两台交换机均基于TSMC COUPE技术，2026H2出货

3. **2026年5月**：与Corning深化合作，Corning在德州和北卡罗来纳州新建三座光纤工厂，创造3000+就业岗位。

4. **Feynman架构（2028）**：NVLink CPO交换机将集成到Feynman架构中，单域扩展到1,152 GPU封装。但NVLink仍提供铜缆选项（Kyber）——铜光共存。

**关键洞察：** NVIDIA当前CPO战略是「scale-out用光（交换机），scale-up保持铜」。NVLink域内仍用铜缆（<1米），机架间用CPO。这种「铜光共存」框架被Jensen和Broadcom CEO Hock Tan共同确认至少持续到2028年。

**来源：** CNBC (2026.03.02); Supercomputing.news; Counterpoint Research (2026.04.02); HPCwire (2026.04.20); TrendForce (2026.05.18)

### 2.3 Broadcom (AVGO)：CPO第二客户，铜光共存鼓吹者 ★★

**定位：** TSMC COUPE的第二大早期客户，将CPO附加到Tomahawk交换机ASIC上。

**CEO Hock Tan立场：** 公开强调铜缆在机架内（超短距）到2028年前仍可行，随着单通道速率向400G攀升，铜缆在成本/可靠性上保持优势。这是一种「现实主义」立场——Broadcom同时是铜缆SerDes（Tomahawk）和CPO的最大供应商之一，两面下注。

**技术路线：** 采用MZM（Mach-Zehnder Modulator）多波长架构（vs NVIDIA的单波长MRM路线）。早期CPO架构采用WL-FO（晶圆级扇出）封装，PIC和EIC分离制造后由SPIL（矽品）负责RDL互连——但RDL PI层的均匀性对信号完整性构成瓶颈。

**来源：** OFC50/SEMIVISION (2025.04.26); SDxCentral (2026.03); TrendForce (2026.05.18)

### 2.4 Marvell (MRVL)：3D硅光子引擎 ★★★

**里程碑：** 在OFC 2024发布业界首个支持200Gbps电/光接口的3D SiPho Engine，在OFC 2026进一步展示进展。

| 关键参数 | 详情 |
|---------|------|
| 引擎规格 | 6.4T 3D SiPho Engine，32通道×200Gbps I/O |
| 集成组件 | Ge光电探测器、调制器(MRM/MZM)、TIA、Driver、SiN/Si波导 |
| 性能提升 | 2×总带宽、2× I/O带宽密度、30%更低每比特能耗 |
| 架构愿景 | CPO + XPU计算die + HBM堆叠在同一基板上 |

**差异化策略：** Marvell是全球最完整的PAM4 DSP + TIA/driver + 光引擎一体化供应商。其CPO策略深度绑定定制化AI加速器（XPU）架构，通过光学I/O实现「数据搬运速度是电信号的100倍」。

**来源：** Marvell Investor PR; SEMIVISION OFC50 (2025.04.26); PhotonCap (2026.05)

### 2.5 Lumentum (LITE) & Coherent (COHR)：NVIDIA战略投资重塑格局 ★★★

**Lumentum ($20亿投资)**：激光源、光放大器、PIC。长距离电信+数据中心互联双重敞口。高功率激光源对更高速率光链路至关重要。

**Coherent ($20亿投资)**：2022年II-VI与原Coherent合并后的综合实体。InP激光器、硅光子收发器、数据中心互联光组件。硅光子平台直接服务于AI数据中心部署。

**竞争影响：** NVIDIA $40亿投资（非收购，是股权投资）赋予其对两家最大的纯光子学供应商的董事会影响力和供应链优先级。其他光子学公司（Marvell、Broadcom、Intel硅光子部门、初创公司群）现在面临一个现实：两家关键组件供应商与最大的GPU客户有优先关系。

**来源：** CNBC (2026.03.02); Supercomputing.news; Forbes (2026.03.04)

### 2.6 CPO测试：量产最大瓶颈 ★★★

**核心问题：** CPO测试是目前量产规模化的最大障碍，行业缺乏统一标准，流程大量依赖人工。

**四个测试阶段：**

| 阶段 | 内容 | 关键性 |
|------|------|:------:|
| (1) PIC晶圆级测试 (OWAT) | DC电学+光学（功率、损耗、暗电流） | ⭐⭐⭐ 最核心 |
| (2) EIC-PIC晶圆级测试 | 调制功能、高速测试、S参数 | ⭐⭐ |
| (3) OE级测试 | 全流程校准，确认KGOE（已知良好光引擎） | ⭐⭐⭐ |
| (4) 先进封装模块级测试 | 全系统功能验证 | ⭐⭐ |

**OWAT痛点：** 单模光纤芯截面~78.5μm² vs 光波导截面~0.099μm²（差800倍），需要纳米级对准精度。单个PIC 100%检测平均耗时>100秒，目前大量依赖人工操作。

**设备供应链格局：**

| 联盟 | ATE供应商 | 探针伙伴 | 关键产品 |
|------|----------|---------|---------|
| Advantest+FormFactor | 爱德万 | FormFactor | V93000-Triton光子测试系统（UFO Probe Card，CalVue实时对准） |
| Teradyne+ficonTEC | 泰瑞达 | ficonTEC（已被中国罗博特科收购） | 首套300mm双面晶圆探针测试系统（WLT-D2，50nm精度） |
| Keysight+FormFactor | — | — | N778x偏振合成器+PIC晶圆测试方案 |
| Chroma | — | — | SLT领导者，正在开发CPO测试设备 |
| Enlitech+iST | — | — | Night Jar SiPh芯片测试平台（高光谱成像） |

**投资含义：** CPO测试设备市场正在形成一个独立的高增长细分。随着CPO芯片陆续量产后，半导体测试设备资本支出占比将进一步提升。

**来源：** TrendForce Insights (2026.04.24); Digitimes (2026.04.13)

### 2.7 竞争格局更新

| 玩家 | 状态 | 技术路线 | 时间线 |
|------|------|---------|--------|
| **TSMC** | 2026年4月量产COUPE | SoIC-X混合键合 | Gen1→Gen2(2027)→Gen3 |
| **NVIDIA** | CPO交换机2026H2出货 | 单波长MRM (DR4) | 2028 Feynman=NVLink CPO |
| **Broadcom** | Tomahawk CPO量产 | 多波长MZM (FR4) | 与TSMC COUPE并行 |
| **Marvell** | 6.4T 3D引擎演示中 | 多客户评估阶段 | CPO+XPU+HBM集成 |
| **Samsung** | 落后TSMC 3年 | 光引擎2027，CPO Turnkey 2029 | 强调HBM+代工+封装+SiPh垂直整合 |
| **AMD** | $2.8亿台湾SiPh研发中心 | 靠近TSMC封装厂 | 未公布CPO具体时间线 |
| **Intel** | 自有硅光子部门 | 存在但非核心叙事 | 较慢 |
| **Ayar Labs** | 2025年12月首个COUPE光互联演示 | TeraPHY产品线 | NVIDIA/AMD/Intel投资 |
| **Foxconn** | CPO交换机Q3 2026量产 | 系统级整合 | 2026 Capex +30% |

### 2.8 开放标准 vs 专有路线

**Open CPX MSA**（2026年3月OFC正式启动）：Ciena、Coherent、Marvell、Molex、Samtec、TeraHop等定义光引擎封装/热管理/电接口规范。**NVIDIA和Broadcom缺席**——暗示两大CPO消费巨头倾向专有方案（类似NVLink/CUDA的封闭生态策略）。

**OCI（Optical Compute Interconnect）标准**：在OFC 2026推出，用于GPU与CPO模块的连接标准。

**来源：** BusinessWire (2026.03.12); Supercomputing.news

---

## 三、假设验证（与README核心论点交叉检验）

| README核心论点 | 验证结果 | 2026.06最新证据 | 置信度 |
|---------------|:------:|----------------|:------:|
| H1: 2026年是CPO量产元年 | ✅ **成立/强化** | TSMC COUPE 4月量产，NVIDIA/Broadcom确认出货 | 5/5 |
| H2: 铜在200G/lane以上物理失效 | ✅ **成立/强化** | 224G铜<1米，NVIDIA/Hock Tan确认此为铜的边界 | 5/5 |
| H3: CPO良率是瓶颈 | ✅ **成立/强化** | 测试是最大障碍（>100秒/PIC+无统一标准+人工依赖） | 5/5 |
| H4: 可插拔光模块短期内性价比优于CPO | ⚠️ **部分成立但趋势改变** | 可插拔仍是主流，但NVIDIA/TSMC正在加速CPO替代（提前5年） | 4/5 |
| H5: 光子计算距商业化尚远 | ✅ **成立** | 本轮搜索未见光子计算商业突破，Lightmatter/Celestial AI仍处早期 | 3/5 |

---

## 四、核心争议更新

### 4.1 争议1：铜光替代速度——「更快」 vs 「共存更久」

**本轮新证据：**

- **加速方（铜死得更快）**：NVIDIA提前5年光学路线图，$40亿投资锁死供应链。Ayar Labs+Alchip演示首个COUPE光学互联方案。Foxconn CPO交换机Q3量产。Open CPX MSA标准化加速。
- **减速方（铜活得更久）**：Jensen Huang和Hock Tan**同时**确认铜缆在机架内到2028年前仍可行。NVIDIA Feynman架构同时保留铜缆（Kyber）和CPO（Kyber CPO）两个scale-up选项。超短距铜链路（<0.5米）在400G/lane仍具成本优势。

**综合判断：** 铜不会「突然死亡」，而是从外向内逐步退缩——scale-out网络已开始光化（2026交换机CPO），scale-up域内（GPU-GPU）铜缆维持到2028年，之后光进铜退加速。TrendForce预测CPO在AI数据中心光模块渗透率2030年达35%，意味着65%仍为可插拔——**长期共存格局**。

### 4.2 争议2：CPO的维护性 vs 可插拔的便利性

**可插拔优势：** 模块故障→拔插替换，成熟供应链，标准化竞争充分。
**CPO劣势：** 光引擎故障→可能需要更换整个交换机/GPU封装，故障成本极高。

**本轮洞察：** NVIDIA选择CPO用于scale-out（交换机，数百到数千条链路，效率优势压倒可维护性顾虑），但在GPU scale-up（NVLink）暂不使用CPO。这本身就是对该争议的实践性回答——**在哪里用CPO取决于效率增益 vs 维护成本的权衡点**。

### 4.3 争议3：封闭生态 vs 开放标准

NVIDIA和Broadcom缺席Open CPX MSA是强烈信号。NVIDIA $40亿投资锁死Coherent/Lumentum供应链，等于说「我们用自己的标准」。这可能导致CPO市场分裂为：(1) NVIDIA专有生态（NVLink CPO），(2) Broadcom专有生态（Tomahawk CPO），(3) 开放生态（OCI + Open CPX MSA 为其他厂商服务）。

---

## 五、关键指标更新

| 指标 | README原值 (2026.05) | 本轮更新 (2026.06) | 变化 | 判断 |
|------|---------------------|-------------------|:----:|------|
| 光模块速率主流 | 800G → 1.6T过渡 | 1.6T成为CPO标准速率 | ↑ 加速 | COUPE首代即1.6T |
| CPO渗透率 (AI DC) | ~0% | 2026H2开始出货 | — | 仍处量产元年 |
| 硅光子光模块占比 | ~30% | 加速提升 | ↑ | 硅光子路线被确认 |
| 铜缆单通道速率极限 | 200G/lane | **224G已确认极限**（<1米） | 确认 | 产业共识形成 |
| NVIDIA CPO时间线 | 未知 | GTC 2026确认2026H2→2028 Feynman | ★ 决定性确认 | |
| CPO渗透率2030E | 未明确 | **35%** (TrendForce) | 新数据点 | |

---

## 六、风险矩阵更新

### 新增/强化风险

| # | 风险 | 严重程度 | 概率 | 来源 |
|---|------|:------:|:----:|------|
| R1 | **TSMC先进封装产能瓶颈**：SoIC/CoWoS被GPU/HBM/光子学三方争夺，COUPE产能可能受限 | 🔴 高 | 40-50% | NewMaxx (2026.06.01) |
| R2 | **CPO测试良率限制量产规模**：无统一标准+人工依赖+100秒/PIC，可能延迟爬坡速度 | 🔴 高 | 50-60% | TrendForce (2026.04.24) |
| R3 | **ABF基板2027年供应紧张**：AI GPU/ASIC/CPO三重需求叠加，高端基板可能再现短缺 | 🟠 中高 | 35-45% | TrendForce (2026.05.18) |
| R4 | **NVIDIA供应商锁定挤压非投资企业**：Coherent/Lumentum获NVIDIA优先权，其他光子学公司面临不公平竞争 | 🟡 中 | 20-30% | Supercomputing.news |
| R5 | **Samsung CPO 2029晚但垂直整合差异化**：若HBM+代工+SiPh一体化路线被验证，可能后发制人 | 🟡 中 | 15-25% | TrendForce (2026.04.01) |

---

## 七、情景分析

### Bull Case (35%)
- TSMC COUPE产能爬坡超预期 → 2027年CPO出货量突破百万级
- NVIDIA Feynman 2028年全面CPO化（scale-up+scale-out）
- 测试自动化突破（Advantest/Teradyne方案成熟）→ 单PIC检测降至<10秒
- 硅光子占光模块比例2028年突破50%
- CPO渗透率2030年超预期达40%+

**标的影响：** TSMC +30-40%, NVIDIA +20-30%, Coherent/Lumentum +50%+, 设备商(Advantest/Teradyne) +30-50%

### Base Case (45%)
- TSMC COUPE稳步爬坡，2026年出货量数万级 → 2027年十万级
- NVIDIA CPO交换机2026H2顺利出货，但量不大
- 铜光共存格局持续到2028-2029年
- CPO 2030年渗透率约30-35%（符合TrendForce）
- 测试自动化渐进改进

**标的影响：** TSMC +15-20%, Coherent/Lumentum +20-30%, 设备商 +15-25%

### Bear Case (20%)
- CPO测试良率问题未解决 → 量产爬坡大幅延迟
- AI CapEx在2027年见顶 → CPO需求骤降
- 铜缆在224G以上通过AEC/CPC技术实现突破 → 光替代时间线推迟
- Samsung后发制人 → TSMC COUPE份额被蚕食
- 开放式CPO标准碎片化 → 生态恶化

**标的影响：** 光子学相关标的 -30-50%, 但TSMC整体基本面受限于AI放缓而非光学本身

---

## 八、投资机会映射

### 第一梯队（确定性最高）

| 标的 | 逻辑 | 风险 | 时间框架 |
|------|------|------|---------|
| **TSMC** | COUPE垄断者，先进封装产能的守门人 | 整体AI CapEx周期风险 | 长期核心 |
| **NVIDIA** | CPO最大推动者和消费者 | 估值偏高 | 中长期 |

### 第二梯队（CPO直接受益）

| 标的 | 逻辑 | 风险 | 时间框架 |
|------|------|------|---------|
| **Broadcom (AVGO)** | Tomahawk CPO + 定制ASIC双驱动 | 铜缆业务自相蚕食 | 中长期 |
| **Marvell (MRVL)** | 最完整光互联PAM4 DSP+引擎一体化 | 客户集中风险 | 中长期 |
| **Coherent (COHR)** | NVIDIA投资+硅光子收发器 | 单一客户依赖 | 中短期 |
| **Lumentum (LITE)** | NVIDIA投资+激光源关键供应商 | 单一客户依赖 | 中短期 |

### 第三梯队（CPO生态/设备）

| 标的 | 逻辑 | 风险 | 时间框架 |
|------|------|------|---------|
| **Advantest** | CPO测试ATE领导者(V93000-Triton) | 日本股票流动性 | 中长期 |
| **Teradyne** | CPO测试第二玩家(UltraFLEXplus+ficonTEC) | ficonTEC中国所有权风险 | 中长期 |
| **Corning (GLW)** | NVIDIA光纤供应商，新建3座工厂 | 传统玻璃业务拖累 | 中长期 |
| **FormFactor** | 光学探针/对准系统供应商 | 细分市场规模有限 | 中期 |

### 第四梯队（长期关注/期权性质）

| 标的 | 逻辑 | 风险 | 时间框架 |
|------|------|------|---------|
| **Ayar Labs** (未上市) | COUPE光学互联方案先驱 | 估值不明，NVIDIA/AMD/Intel投资 | 长期跟踪 |
| **Lightmatter** (未上市) | 光子AI加速器Nature论文 | 大规模商业化尚需3-5年 | 长期跟踪 |
| **Celestial AI** (未上市) | 光子互联架构 | 早期阶段 | 长期跟踪 |
| **Samsung** | 2029年CPO Turnkey | 落后3年，但垂直整合独特 | 长期关注 |

---

## 九、与相邻课题的传导关系

| 关联课题 | 传导路径 | 方向 | 强度 |
|---------|---------|:----:|:----:|
| #01 AI架构范式转移(JEPA vs LLM) | AI训练集群规模↑→互联瓶颈→光学需求↑ | 正 | 强 |
| #11 先进制程GAA | TSMC先进封装产能被多方争夺→COUPE供给受限 | 负（竞争） | 中 |
| #17 AI推理经济与定制芯片 | 定制ASIC(Broadcom/Marvell)集成CPO→差异化优势 | 正 | 中 |
| #21 铜铝超级周期 | 铜缆被光替代→长期铜需求减少（但2028年前影响小） | 负（长期） | 弱 |

---

## 十、方法论备注

- **搜索源**: anysearch batch_search（5组关键词并行搜索）+ anysearch extract（9篇深度文章提取）
- **信息截止时间**: 2026年6月5日
- **搜索关键词**: silicon photonics 2026, CPO co-packaged optics, TSMC COUPE, NVIDIA optical interconnect, LITE MRVL AVGO silicon photonics
- **核心来源**: TrendForce, DIGITIMES, NewMaxx/Borecraft, Machine Herald, Supercomputing.news, Counterpoint Research, SEMIVISION/OFC50, HPCwire
- **未覆盖维度**: 中国硅光子产业链（中际旭创/光迅科技/华工科技/源杰科技等）的最新动态，中国厂商在可插拔光模块的主导地位如何影响CPO转型路径
- **建议Round 2补充**: (1) 中国光模块产业链CPO布局调研，(2) TSMC COUPE产能具体数字追踪，(3) CPO测试良率的最新进展，(4) OFC 2026后各厂商的CPO路标对比表
