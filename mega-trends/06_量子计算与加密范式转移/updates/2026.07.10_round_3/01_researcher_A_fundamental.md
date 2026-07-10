# 基本面研究员报告 — #06 量子计算（Round 3，07.10）

> 硬件/技术里程碑视角 | 06.05 → 07.10（约 5 周）| 供 PM + CIO + 魔鬼辩护人审阅

---

## 一、Delta 摘要表（★ 排序）

| ★ | 事件 | 日期 | 来源 | 对投资论点的影响 |
|---|------|------|------|-----------------|
| ★★★★★ | **IBM 完成量子模拟实用案例**：与大学合作创造此前不存在的分子并用量子计算验证其奇异性质；3/26 提出"对自然基准"而非速度基准的新范式 | 2026-03-05 / 03-26 | [newsroom.ibm.com](https://newsroom.ibm.com/2026-03-05-ibm-and-university-researchers-create-a-never-before-seen-molecule-and-prove-its-exotic-nature-with-quantum-computing) | 量子优势**尚未正式确认**（速度意义上），但实用案例从零到一的突破；CEO Krishna 仍预测 2026 年底前实现 |
| ★★★★★ | **Quantinuum Helios 发表 Nature 论文**：98 物理量子比特 QCCD 离子阱处理器，50 个纠错逻辑量子比特（优于盈亏平衡），双比特门保真度 99.921%，单比特门 99.9975% | 2026（Nature s41586-026-10676-4） | [Nature](https://www.nature.com/articles/s41586-026-10676-4) | 离子阱路线获同行评审验证；纠错编码比 ~2:1（色码）为业界最佳 |
| ★★★★★ | **CHIPS 法案 $20.13 亿意向书签署**：商务部 5/21 与 9 家公司签约（IBM/Rigetti/GlobalFoundries 等），结构为拨款+政府少数股权 | 2026-05-21 | [NIST](https://www.nist.gov/news-events/news/2026/05/department-commerce-announces-letters-intent-9-companies-2-billion) / [WSJ](https://www.wsj.com/tech/quantum-computing-grants-ibm-rigetti-globalfoundries-7382e6be) | 美国国家战略级资金落地；政府持股结构罕见（表明国家安全属性） |
| ★★★★ | **Atom Computing 首次在中性原子上实现完整 toric code 纠错** | 2026-06-03 | [Quantum Insider](https://thequantuminsider.com/2026/06/03/atom-computing-reveals-quantum-error-correction-with-toric-code/) | 中性原子路线获关键验证；与 Microsoft Azure Quantum 合作（24 逻辑量子比特纪录）；~1200 物理量子比特系统 |
| ★★★★ | **Microsoft Majorana 2 发布**：声称拓扑量子比特寿命 >20 秒，但 Majorana 1 仍未独立验证 | 2026-06-02 | [Quantum Insider](https://thequantuminsider.com/2026/06/02/microsoft-reports-advances-in-majorana-2-following-debate-over-last-years-topological-claims/) | 拓扑路线**被边缘化**的最强信号：物理学家在 Global Physics Summit 公开质疑；"落后数年" |
| ★★★★ | **Quantinuum IPO 后 5 周稳定在发行价以上**：QNT ~$74-76（7/8-9），较 $60 发行价 +25% | 2026-07-08 | [StockTitan](https://www.stocktitan.net/overview/QNT/) | R2 升级条件 3（3 个月稳定）已完成 5/12 周，进展良好 |
| ★★★★ | **IonQ Q1 出售首台 256 量子比特系统** + 光子互连里程碑（远程纠缠验证）+ ABQ-Net 量子网络上线（2/24，全美首个开放接入纠缠网络） | 2026-Q1 / 02-24 | [IonQ](https://www.ionq.com/news/ionq-achieves-key-photonic-interconnect-milestone-demonstrating-networked-quantum-systems-using-entanglement) | 收入增速与量子网络商业化双线推进；R2 升级条件 2（200%+）在轨 |
| ★★★ | **D-Wave "RSA-2048 因式分解" 被广泛质疑**：Wang 2025 仅处理特殊结构整数（~90 bit），非通用 RSA-2048；专家维持 10+ 年远 | 2025-2026 | [Homeland Security Today](https://www.hstoday.us/subject-matter-areas/cybersecurity/no-chinese-did-not-crack-rsa-with-quantum-yet/) / [Hacker News](https://news.ycombinator.com/item?id=43952396) | Q-Day 恐慌情景概率维持低位（10%）；RSA 时间表不变 |
| ★★★ | **QuEra 目标 2026 年实现 100 逻辑量子比特**；中性原子路线获 IEEE Spectrum 认定为"2026 大跃进" | 2026 | [QuEra Roadmap](https://www.quera.com/press-releases/quera-computing-releases-a-groundbreaking-roadmap-for-advanced-error-corrected-quantum-computers-pioneering-the-next-frontier-in-quantum-innovation-0) / [IEEE Spectrum](https://spectrum.ieee.org/neutral-atom-quantum-computing) | 中性原子路线成第四条可信路径 |
| ★★★ | **NIST PQC 第二轮补充签名算法**：9 个候选，更新规格截止 8/14/2026；FIPS 206（FALCON）开发中 | 2026 H2 进行中 | [NIST CSRC](https://csrc.nist.gov/projects/post-quantum-cryptography/post-quantum-cryptography-standardization) / [PostQuantum](https://postquantum.com/security-pqc/nist-third-round-pqc-signatures/) | 确定性层（PQC 迁移）受益时间表不变 |
| ★★★ | **Regev 算法正式发表于 JACM**：渐近优于 Shor；Ragavan 改进（空间高效+噪声鲁棒）；实验验证对特定合数优于 Shor | 2025 (JACM) | [JACM](https://dl.acm.org/doi/10.1145/3708471) / [arXiv:2502.09772](https://arxiv.org/html/2502.09772v1) | 理论改进但不改变近期 RSA 时间表（仍需容错量子硬件） |
| ★★★ | **Gil Kalai 维持怀疑立场**：3/10 博文回应 Aaronson；双方同意实验精度已足以近期内经验性解决可扩展性争论 | 2026-03-10 | [Kalai Blog](https://gilkalai.wordpress.com/2026/03/10/scott-aaronsons-view-of-my-view-about-quantum-computing/) | 学术怀疑未消退；IBM 2029 延迟风险仍存 |
| ★★ | **PsiQuantum Omega 光量子芯片组**（可制造）+ 目标 2026-27 实现 50-100 光子量子比特原型 + 百万量子比特目标 2027 | 2025-02 / 2026 | [PsiQuantum](https://www.psiquantum.com/technology) / [PostQuantum](https://postquantum.com/quantum-computing-companies/psiquantum/) | 光量子路线获资本持续但百万量子比特目标激进 |
| ★★ | **中国光量子计算机接入天衍量子云平台**（6/25）；天衍-504 + 祖冲之 3.0 对标 IBM/Google | 2026-06-25 | [NCSTI](https://en.ncsti.gov.cn/Latest/news/202606/t20260625_250267.html) / [CSIS](https://www.csis.org/analysis/understanding-chinas-quest-quantum-advancement) | 中美量子竞赛叙事持续；中国多路线并行（超导+光量子） |

---

## 二、技术里程碑更新表

### 2.1 逻辑量子比特推进（核心指标）

| 平台 | 路线 | 逻辑量子比特 | 物理量子比特 | 编码比 | 纠错码 | 状态/来源 |
|------|------|-------------|-------------|--------|--------|-----------|
| **Quantinuum Helios** | 离子阱 QCCD | **50**（纠错检出，优于盈亏平衡） | 98 | ~2:1 | 色码 | [Nature 2026](https://www.nature.com/articles/s41586-026-10676-4) 独立同行评审 |
| **Quantinuum H2 + Microsoft 虚拟化** | 离子阱 | **~94**（可靠逻辑量子比特，R2 基线） | — | — | qubit virtualization | [Microsoft Blog 2024-04](https://blogs.microsoft.com/blog/2024/04/03/advancing-science-microsoft-and-quantinuum-demonstrate-the-most-reliable-logical-qubits-on-record-with-an-error-rate-800x-better-than-physical-qubits/) |
| **Google Willow** | 超导 | 距离-5 / 距离-7 表面码记忆（below-threshold） | — | — | 表面码 | [Nature 2025](https://www.nature.com/articles/s41586-024-08449-y)（被引 1211 次）|
| **Atom Computing + Microsoft** | 中性原子 | **24**（纠缠逻辑量子比特纪录，2024-11） | ~1200 | ~50:1 | toric code（2026-06 首次完整演示） | [Azure Blog](https://azure.microsoft.com/en-us/blog/quantum/2024/11/19/microsoft-and-atom-computing-offer-a-commercial-quantum-machine-with-the-largest-number-of-entangled-logical-qubits-on-record/) |
| **QuEra** | 中性原子 | 目标 **100**（2026） | — | — | Gottesman 2016 方案 | [QuEra Roadmap](https://www.quera.com/press-releases/quera-computing-releases-a-groundbreaking-roadmap-for-advanced-error-corrected-quantum-computers-pioneering-the-next-frontier-in-quantum-innovation-0) |
| **IonQ** | 离子阱 | AQ ~256（Tempo 目标）；已售首台 256 物理量子比特系统 | 256+ | — | — | [IonQ Roadmap](https://www.ionq.com/roadmap) |
| **IBM Nighthawk** | 超导 | 物理量子比特导向（2026 目标 7500 门 / 3 耦合模块 / 360 量子比特） | 120（单芯片） | — | 误差缓解（非完整纠错） | [IBM Tech Atlas](https://www.ibm.com/roadmaps/quantum/2026/) |
| **Microsoft Majorana 2** | 拓扑 | 声称拓扑量子比特寿命 >20 秒 | 8（Majorana 1） | — | 拓扑保护（未验证） | [Quantum Insider 2026-06-02](https://thequantuminsider.com/2026/06/02/microsoft-reports-advances-in-majorana-2-following-debate-over-last-years-topological-claims/) **独立验证缺失** |

**关键判断**：
- R2 基线"94 逻辑量子比特（Quantinuum）"指的是 H2 + Microsoft qubit virtualization 系统（软件层增强），而非专用硬件
- Helios 的 50 逻辑量子比特（98 物理，色码，Nature 同行评审）是**专用硬件**的独立验证基准
- 向 1000（药物发现阈值）：**无任何平台接近**。QuEra 2026 目标 100 已是前沿
- 编码比差距巨大：Helios ~2:1（离子阱优势）vs Atom Computing ~50:1（中性原子仍需优化）

### 2.2 纠错码进展

| 纠错方案 | 平台 | 突破 | 验证状态 |
|----------|------|------|----------|
| 色码（color code） | Quantinuum Helios | 2:1 编码比，优于盈亏平衡 | ✅ Nature 同行评审 |
| 表面码 below-threshold | Google Willow | 距离-5/7，增加物理量子比特→逻辑错误率下降 | ✅ Nature 同行评审（被引 1211）|
| 动态表面码 | Google Research | 新纠错路径 | 研究阶段 |
| Toric code | Atom Computing | 中性原子首次完整演示 | ✅ 2026-06 公布 |
| Gottesman 2016 方案 | QuEra | 重复丢失修正 | arXiv 预印本 |
| 拓扑保护 | Microsoft Majorana | 声称 >20 秒寿命 | ❌ **未独立验证** |

### 2.3 门保真度对比

| 平台 | 单比特门 | 双比特门 | 备注 |
|------|---------|---------|------|
| Quantinuum Helios | 99.9975% | 99.921% | 全连通，离子阱 |
| Quantinuum H-Series | — | 99.9%（"三个 9"） | 全连通 |
| Oxford（实验记录） | — | 99.999985%（0.000015% 错误率） | 世界纪录（实验性非商用） |

---

## 三、PQ 投资时钟位置更新

### R2 基线：PQ1（7-8 点钟，早期商业化萌芽期）

### R3 判断：**维持 PQ1，但向 8 点钟方向移动（PQ1+）**

**移动依据（向 PQ2 推动）**：
1. Helios Nature 论文 = 离子阱路线获同行评审的硬件级纠错验证
2. Atom Computing toric code + Microsoft 合作 = 中性原子路线从探索→竞争
3. CHIPS $20.13 亿签约 = 国家级资金从承诺→意向书落地
4. Quantinuum IPO 稳定 = 公开市场对纯量子标的的定价能力初步建立
5. IBM 实用案例（分子模拟）= 从理论→首个真实物理对象模拟

**未达 PQ2（8-9 点钟）的阻碍**：
1. **无确认的量子优势**（速度意义）：IBM 3 月分子模拟是实用案例但非速度优势；CEO 仍"预测年底前"
2. **逻辑量子比特仍 50-100 区间**：距 1000（药物发现）和百万（RSA 破解）仍远
3. **路线未收敛**：4 条路线仍活跃（超导/离子阱/中性原子/光量子），仅拓扑被边缘化
4. **Majorana 未验证**：拓扑路线的关键承诺仍未兑现
5. **IonQ Q2 财报未出**（~8/12）：收入增速可持续性未确认

---

## 四、路线收敛度评估

### 5 条路线状态（R3）

| 路线 | 代表玩家 | R3 状态 | 资本集中度 | 收敛信号 |
|------|---------|---------|-----------|---------|
| **超导** | IBM, Google | 领先，below-threshold 已验证 | 高（CHIPS + IBM/Google 内部） | — |
| **离子阱** | Quantinuum, IonQ | 强势，Helios Nature + IonQ 商业化 | 高（IPO + CHIPS） | — |
| **中性原子** | Atom Computing, QuEra, Pasqal | **突破年**，toric code + 100 目标 | 快速上升（Microsoft 合作） | ↑ 获资本集中 |
| **光量子** | PsiQuantum, Quandela | 持续，Omega 芯片组 + 百万目标 | 中（多十亿级私人投资） | — |
| **拓扑** | Microsoft | **被边缘化**，Majorana 未验证 | 孤立（仅 Microsoft） | ↓ 边缘化 |

### 收敛判断：**部分收敛（1/5 路线被边缘化）**

- R2 升级条件 4 要求"至少 1-2 条技术路线被市场淘汰"
- **拓扑路线**被边缘化的信号强烈：
  - Majorana 1（2025-02）被物理学家在 Global Physics Summit 公开质疑
  - Majorana 2（2026-06）声称 >20 秒寿命但**仍无独立验证**
  - PostQuantum 评为"落后数年"
  - Microsoft 自身转向与 Atom Computing（中性原子）合作 = **实质上承认拓扑路线不足以单独支撑商业化**
- **但**：仅 1 条路线被边缘化，4 条仍活跃（超导/离子阱/中性原子/光量子）
- **中性原子**同时获得资本集中（Atom Computing + Microsoft + QuEra），这是收敛的另一面信号

**结论**：R2 升级条件 4（1-2 条路线淘汰）**部分达成**（1 条边缘化，需第二条确认）。若 PsiQuantum 2026-27 原型未达预期，光量子可能成为第二条被边缘化路线。

---

## 五、IBM 2029 延迟概率更新判断

### R2 基线：50% 延迟概率（建模 2029(30%)/2031(40%)/2033+(30%)）

### R3 判断：**下调至 40-45%**（即 IBM 2029 按期概率从 50% 升至 55-60%）

**下调延迟概率的因素（利好按期）**：
1. **Below-threshold 纠错已被同行评审验证**（Google Willow Nature，被引 1211 次）—— 这是可扩展性的**物理基础**已确认
2. **Helios 色码 2:1 编码比** —— 证明高效纠错在专用硬件上可行（非仅理论）
3. **IBM Nighthawk 按计划推进**（2026 目标 7500 门 / 360 量子比特），未见延迟报告
4. **IBM 3 月分子模拟** —— 从理论→实用案例的零到一突破
5. **误差率从 0.1%（2023）→0.000015%（2026，Oxford 记录）** —— 物理层面持续改善

**维持延迟风险的因素（利好延迟）**：
1. **Gil Kalai 仍维持怀疑**（3/10 博文）——噪声论证未被实验推翻，但双方同意近期可经验性裁决
2. **无确认的量子优势**（速度意义）—— CEO 仍"预测"而非"已实现"
3. **从 50-100 逻辑量子比特到百万级**（Starling 目标）的工程跳跃巨大
4. **Majorana 拓扑路线受挫** —— 若拓扑最终失败，IBM 的超导路线需独自承担全部压力
5. **纠错解码器的实时性能** —— 规模化后解码延迟是已知工程瓶颈

**更新建模**：2029(35%)/2031(40%)/2033+(25%) —— 略微向 2029 倾斜，但仍保守

---

## 六、对升级 4 条件的技术评估

| 升级条件 | R2 状态 | R3 状态 | 达成度 | 关键证据 |
|----------|---------|---------|--------|---------|
| **1. IBM 2026 验证量子优势** | 未兑现 | **部分在轨** | 40% | 3 月分子模拟是实用案例但非速度优势；CEO 仍预测年底前；需 Nature/Science 独立论文确认速度优势 |
| **2. IonQ Q2-Q3 收入增速 200%+** | 待验证 | **在轨** | 60% | Q1 出售首台 256 量子比特系统；光子互连里程碑；ABQ-Net 上线；Q2 财报 ~8/12 待出 |
| **3. Quantinuum IPO 3 个月稳定在发行价以上** | 待验证 | **进展良好** | 5/12 周（42%）| QNT ~$74-76（7/8），较 $60 发行价 +25%；无破发迹象；交易量正常 |
| **4. 至少 1-2 条技术路线被淘汰** | 未达成 | **部分达成** | 50% | 拓扑路线被边缘化（Majorana 未验证 + Microsoft 转向中性原子）；需第二条确认 |

### 综合评估

- **4 条件中 0 条完全达成，3 条部分在轨，1 条进展良好**
- 预计升级窗口仍为 **2026 Q4 - 2027 Q1**（与 R2 判断一致）
- 若 IBM Q4 前发布确认量子优势论文 + IonQ Q2 维持高增速 + Quantinuum 9 月稳定 3 月 → 可触发升级
- 最大风险：IBM 量子优势若年底仍未确认 → 升级推迟至 2027 Q2+

---

## 七、经典 vs 量子边界更新

### 7.1 Regev 算法

- **正式发表于 JACM 2025**（Journal of the ACM）：渐近优于 Shor，用高维格密码技术增强
- **Ragavan 改进**（2023，被 JACM 2025 引用）：空间高效 + 噪声鲁棒，降低量子硬件要求
- **实验验证**（arXiv:2502.09772，2025-02）：对特定合数实际优于 Shor
- **对 RSA 时间表影响**：**不改变近期时间表**。Regev/Ragavan 降低的是渐近复杂度和空间需求，但仍需**容错量子计算机**（百万级物理量子比特）。Gidney & Ekerå 2021 基准（20M 量子比特 / 8 小时破解 RSA-2048）仍是主流估计

### 7.2 D-Wave RSA-2048 声明

- Wang 2025（Tsinghua Science and Technology，被引 13）声称 D-Wave 首次因式分解 RSA-2048
- **广泛质疑**：
  - 仅处理**特殊结构整数**（因子仅差 2 bit），非通用 RSA-2048
  - 实际验证仅 ~90-bit
  - 使用量子退火（annealing）非 Shor 算法（门级量子计算）
  - Homeland Security Today："No, Chinese Did Not Crack RSA With Quantum (Yet)"
- **结论**：Q-Day 恐慌情景概率维持 R2 的 10%；RSA 破解时间表不变

### 7.3 经典模拟追赶

- JUPITER 等超算持续推进经典模拟边界
- AI 加速经典模拟（神经网络解码器等）是活跃研究方向
- 但经典模拟只能模拟小规模量子电路（~50-100 量子比特），无法替代规模化量子硬件

---

## 八、学术怀疑更新

### Gil Kalai vs Scott Aaronson（2026-03-10 博文交锋）

- Kalai 在 3/10 博文中直接回应 Aaronson 对其怀疑立场的表述
- **核心分歧不变**：Kalai 认为噪声本质上禁止大规模量子计算；Aaronson 认为不禁止
- **新共识**：双方同意实验精度已提升到足以**近期内经验性裁决**争论
- **对投资的启示**：可扩展性争论进入"可证伪窗口"——若 2027-2028 年 IBM Starling 原型或 Helios 后继者达到 1000+ 逻辑量子比特，Kalai 立场将被实验推翻；反之若持续卡在 100-200，Kalai 立场获支撑

### Oded Regev

- Regev 算法发表于 JACM 2025（见 7.1）
- 未发表对可扩展性的直接评论，但其算法改进间接降低了硬件门槛（利好可扩展性）

---

## 九、PQC 标准进展

### 已 finalized（2024-08）

| FIPS | 算法 | 用途 |
|------|------|------|
| FIPS 203 | ML-KEM（CRYSTALS-Kyber） | 密钥封装 |
| FIPS 204 | ML-DSA（CRYSTALS-Dilithium） | 数字签名 |
| FIPS 205 | SLH-DSA（SPHINCS+） | 数字签名（哈希基） |

### 进行中（R3 窗口）

| 项目 | 状态 | 预期 |
|------|------|------|
| **FIPS 206（FALCON）** | 开发中 | 2026 H2 预期但**未发布** |
| **Additional Digital Signature Schemes Round 2** | 9 个候选，更新规格截止 2026-08-14 | NIST 预计修改较小；finalization 可能 2027 |
| **Round 3 候选** | NIST 已选 9 个第三轮候选 | 标准化继续推进 |

**判断**：PQC 标准化按预期推进，无延迟也无加速。确定性层（PANW/CRWD/NET/GOOGL）的投资逻辑不受影响。Google 2029 / NSA CNSA 2.0 2030 / NIST 2035 截止日期维持不变。

---

## 十、关键区分：厂商宣称 vs 独立验证

| 声明 | 来源 | 验证状态 | 可信度 |
|------|------|---------|--------|
| Helios 50 逻辑量子比特 / 99.921% 双比特门 | Quantinuum | ✅ Nature 同行评审 | **高** |
| Willow below-threshold 表面码 | Google | ✅ Nature 同行评审（被引 1211） | **高** |
| H2 + Microsoft 94 可靠逻辑量子比特 | Quantinuum/Microsoft | ⚠️ 联合发布，部分同行评审 | **中高** |
| Atom Computing 24 逻辑量子比特 + toric code | Atom Computing/Microsoft | ⚠️ 联合发布，未经独立第三方复现 | **中** |
| Majorana 2 拓扑量子比特 >20 秒寿命 | Microsoft | ❌ **未独立验证**，物理学家公开质疑 | **低** |
| IonQ 256 量子比特系统已售 | IonQ | ⚠️ 厂商宣称，商业交易未公开审计 | **中** |
| IBM 2026 量子优势 | IBM（CEO 预测） | ❌ **未实现**，仅分子模拟实用案例 | **待验证** |
| D-Wave RSA-2048 因式分解 | Wang 2025 | ❌ **广泛质疑**，仅特殊结构整数 | **低** |
| QuEra 2026 年 100 逻辑量子比特 | QuEra（路线图目标） | ❌ 未实现（目标） | **待验证** |

---

## 十一、来源链接索引

### 一级来源（同行评审 / 官方）

1. [Quantinuum Helios Nature 论文 (2026)](https://www.nature.com/articles/s41586-026-10676-4) — 98 量子比特离子阱 QCCD，50 逻辑量子比特
2. [Google Willow Nature 论文 (2025)](https://www.nature.com/articles/s41586-024-08449-y) — Below-threshold 表面码（被引 1211）
3. [NIST/D Commerce CHIPS $20.13 亿意向书 (2026-05-21)](https://www.nist.gov/news-events/news/2026/05/department-commerce-announces-letters-intent-9-companies-2-billion)
4. [IBM Newsroom 分子模拟 (2026-03-05)](https://newsroom.ibm.com/2026-03-05-ibm-and-university-researchers-create-a-never-before-seen-molecule-and-prove-its-exotic-nature-with-quantum-computing)
5. [IBM Quantum Blog 量子优势时代](https://www.ibm.com/quantum/blog/quantum-advantage-era)
6. [IBM Tech Atlas 量子路线图 2026](https://www.ibm.com/roadmaps/quantum/2026/)
7. [NIST CSRC PQC 标准化](https://csrc.nist.gov/projects/post-quantum-cryptography/post-quantum-cryptography-standardization)
8. [Regev 算法 JACM 2025](https://dl.acm.org/doi/10.1145/3708471)
9. [Kalai 博文回应 Aaronson (2026-03-10)](https://gilkalai.wordpress.com/2026/03/10/scott-aaronsons-view-of-my-view-about-quantum-computing/)

### 二级来源（行业媒体 / 厂商）

10. [Quantinuum Helios 博客](https://www.quantinuum.com/blog/introducing-helios-the-most-accurate-quantum-computer-in-the-world)
11. [Quantinuum H-Series 56 物理量子比特](https://www.quantinuum.com/blog/quantinuums-h-series-hits-56-physical-qubits-that-are-all-to-all-connected-and-departs-the-era-of-classical-simulation)
12. [Atom Computing toric code (2026-06-03)](https://thequantuminsider.com/2026/06/03/atom-computing-reveals-quantum-error-correction-with-toric-code/)
13. [Microsoft Majorana 2 (2026-06-02)](https://thequantuminsider.com/2026/06/02/microsoft-reports-advances-in-majorana-2-following-debate-over-last-years-topological-claims/)
14. [IonQ 光子互连里程碑](https://www.ionq.com/news/ionq-achieves-key-photonic-interconnect-milestone-demonstrating-networked-quantum-systems-using-entanglement)
15. [IonQ Roadmap](https://www.ionq.com/roadmap)
16. [Quantinuum IPO 定价公告](https://www.quantinuum.com/press-releases/quantinuum-announces-pricing-of-upsized-initial-public-offering)
17. [StockTitan QNT 概览](https://www.stocktitan.net/overview/QNT/)
18. [WSJ CHIPS 量子拨款](https://www.wsj.com/tech/quantum-computing-grants-ibm-rigetti-globalfoundries-7382e6be)
19. [QuEra 100 逻辑量子比特路线图](https://www.quera.com/press-releases/quera-computing-releases-a-groundbreaking-roadmap-for-advanced-error-corrected-quantum-computers-pioneering-the-next-frontier-in-quantum-innovation-0)
20. [IEEE Spectrum 中性原子 2026 大跃进](https://spectrum.ieee.org/neutral-atom-quantum-computing)
21. [Science News Microsoft 拓扑量子比特质疑](https://www.sciencenews.org/article/microsoft-topological-quantum-majorana)
22. [Homeland Security Today D-Wave RSA 质疑](https://www.hstoday.us/subject-matter-areas/cybersecurity/no-chinese-did-not-crack-rsa-with-quantum-yet/)
23. [Wang 2025 D-Wave RSA-2048 原始论文](https://www.sciopen.com/article/10.26599/TST.2024.9010028)
24. [Ragavan Regev 改进 (ePrint 2023/1501)](https://eprint.iacr.org/2023/1501)
25. [Regev 实验实现 (arXiv:2502.09772)](https://arxiv.org/html/2502.09772v1)
26. [CSIS 中国量子分析](https://www.csis.org/analysis/understanding-chinas-quest-quantum-advancement)
27. [NCSTI 中国光量子接入天衍云 (2026-06-25)](https://en.ncsti.gov.cn/Latest/news/202606/t20260625_250267.html)
28. [PsiQuantum Omega / 技术页](https://www.psiquantum.com/technology)
29. [Microsoft + Atom Computing 24 逻辑量子比特 (Azure Blog 2024-11)](https://azure.microsoft.com/en-us/blog/quantum/2024/11/19/microsoft-and-atom-computing-offer-a-commercial-quantum-machine-with-the-largest-number-of-entangled-logical-qubits-on-record/)
30. [Forbes IBM 量子优势 2026 目标](https://www.forbes.com/sites/moorinsights/2025/12/05/ibm-targets-quantum-advantage-by-2026-with-new-processors-and-tools/)

---

> **研究员结论**：R3 窗口（06.05→07.10）技术进展扎实但无范式级突破。Helios Nature 论文 + Atom Computing toric code + CHIPS $20.13 亿落地 = 三项可验证的实质性进展。但 IBM 量子优势仍未确认、逻辑量子比特仍在 50-100 区间、路线仅部分收敛（拓扑边缘化）。PQ 时钟维持 PQ1+（向 8 点钟移动但未达 PQ2）。升级 4 条件 0/4 完全达成，预计 2026 Q4-2027 Q1 触发窗口不变。IBM 2029 延迟概率从 50% 微调至 40-45%（below-threshold 物理基础已确认，但工程跳跃仍大）。
