# 基本面研究员（研究员A）独立研究报告

> 课题: #17 AI推理经济与定制芯片范式转移
> 分析日期: 2026-09-03
> 角色: fundamental（估值、财务建模、行业对比）
> 信息截止: 2026-09-03（捕获窗口 2026.07.10 → 09.03）

---

## 一、核心发现（Top 3）

1. **NVDA Q2 FY2027 全面碾压并给出 FY2028 +70% 供给受限指引，但 Forward PE 已升破 R3 合理区间**。总营收 $96.2B（vs $91B 指引，+106% YoY/+18% QoQ），DC 收入 $89.0B（+117% YoY，处于 street 区间 $83.5-91.5B 上沿），非 GAAP 毛利率 75.0%；Q3 指引 $108B ±2%（毛利率降至 ~74%，且不假设任何中国 DC 计算收入）；Vera Rubin 已全面量产，约占 Q3 DC 收入 20%；管理层明确 FY2028 营收增长约 70%"supply-constrained outlook"。股价 $224.41（9/3），Forward PE ~24.2x——高于 R3 裁定的 20-22x "justified cheap" 带，PEG ~0.48-0.56 仍是全市场最低档。基本面更强、估值更贵，entry band（$195-210）已失效。

2. **四大 Hyperscaler 2026 CapEx 集体上调至 ~$733B（+~70% YoY），但 2027"首次正式指引"并未发生——全部为方向性表态，且 FCF/融资结构恶化速度超预期**。GOOGL $195-205B / AMZN $220B / META $130-145B / MSFT 季度 CapEx 将 >$50B；2027 街道预期 $1.09-1.4T（Wells Fargo +27% 上调至 $1.092T；Morgan Stanley $1.4T）。代价：Alphabet 季度 FCF **-$5.9B**（史上首次转负）、Meta 季度 FCF 仅 **$784M**（-91% YoY）并单季发债 $24.9B；Barclays 测算 2027 CapEx 将占五大 Hyperscaler OCF 的 ~90%（2023 年为 40%）；Bridgewater 测算 2027 AI 融资需求 $612B > 全市场 IG+HY 净发行 $470B。**H5 从"有条件成立"滑向"融资依赖临界"**。

3. **租金与 Token 价格数据线出现方向性分化：GPU 租金上涨、Token 价格暴跌**——"二级市场过剩"未再现。H100 neocloud 指数 ~$2.43-2.63/hr（K4 阈值 $1.5 远未触发，1 年期合约价从 $1.70→$2.35 且 Q3 再涨 20-22%）；B200 on-demand 中位 ~$6.79/hr。同时混合 Token 价格 10 周内 -43%（$2.04→$1.16/1M，5/31-8/8），"性能恒定年降 ~10x"继续成立但总量支出仍因用量扩张而上升。推理经济学"量价剪刀差"是本轮最健康的信号：单价通缩未伴随收入通缩。

---

## 二、详细分析

### 2.1 NVDA — Q2 FY2027（8/26，D1 必查项）

| 指标 | 实际 | 对照 | 判定 |
|---|---|---|---|
| 总营收 | $96.2B | 指引 $91B / street $92.2B | 超指引 ~$5.2B |
| DC 收入 | $89.0B（+117% YoY，+18% QoQ） | street $83.5-91.5B | 上沿附近 |
| 非 GAAP EPS | ~$2.22 | consensus 超预期 | Beat |
| 非 GAAP 毛利率 | 75.0% | Q3 指引 ~74% ±50bp | Rubin 爬坡正常稀释 |
| Q3 FY27 指引 | $108B ±2 | 隐含 +~12% QoQ | 再创纪录 |

- **Rubin**：Vera Rubin "now in full production"（官方新闻稿），Q3 约占 DC 收入 20%（≈$20B 量级）；每 GW 收入机会 Hopper $18B → Blackwell $25B → Rubin 进一步提升（WisdomTree 8/28-9/2 测算）。**双两芯方案确认**：Rubin Ultra 四芯因 CoWoS-L 基板翘曲取消，改双 die（TSMC N3P + CoWoS-L），2027 发布——与 R3 裁定一致，无新恶化；黄仁勋亲赴台积电锁定 Vera Rubin 产能（平台六芯片推动 CoWoS 向 130k wpm 扩张）。
- **中国**：Q3 指引不假设任何中国 DC 计算收入——地缘下行被显式剥离，指引质量高。
- **估值**：$224.41（9/3），Forward PE 24.2x（GuruFocus/Yahoo 口径一致；trailing ~27.5x，较 10 年均值 -42%）。R3 为 $202.78/20-22x → 8 周 +10.7%，PE 扩张 ~2-4 个点。Seeking Alpha 9/2 文章以"0.48x PEG"论证仍便宜；同日另一篇标题直指"losing market share"。**我的裁定：24x 配 +70% FY28 指引 = PEG <0.5，估值仍非主要风险，但 R3 入场带 $195-210 已过，追高性价比下降。**

### 2.2 Hyperscaler Q2 — 2026 执行与 2027 指引（D2 必查项）

| 公司 | 财报日 | 2026 CapEx | Q2 CapEx | Q2 FCF | 2027 表态 |
|---|---|---|---|---|---|
| GOOGL | 7/22 | $195-205B（自 $180-190B 上调） | $44.9B（~2x YoY） | **-$5.9B** | 方向性"更高"，采购承诺超上年 |
| META | 7/29 | $130-145B（上调下限） | $31.08B（+83%） | **$784M**（-91%） | "significantly increase" |
| AMZN | 7/30 | $220B（自 $200B 上调，vs 2025 $125B +76%） | ~$53B | 压缩 | "产能到 2027 都跟不上需求"（Jassy） |
| MSFT | 7/29(FY26Q4) | ~$190B 日历年 + 补充 | $41B | 压缩 | 季度 CapEx 持续 >$50B；street FY27 ~$220B |

- 四大合计 2026 ~**$733B**（Mohit Agrawal 汇总；含 Oracle 口径 $750-803B）。**D2 结论：2027 正式量化指引均未给出**，全部为方向性措辞——正式数字要到 Q3/Q4 财报，这是下一个验证窗口。
- 需求侧支撑真实：Azure +43%（加速，年化首破 $100B）、Google Cloud $24.8B +82%、backlog $514B（单季 +$50B）、AWS $42.2B +37% @39.4% OPM、MSFT 调整后 EPS $4.74 大超 $4.24。
- **融资结构（本轮最大 delta）**：Meta 单季发债 $24.9B；Oracle $25B 八档 IG 债获创纪录需求（2026 计划 $45-50B，债/股各半）；2026 全年 AI 相关债券发行预估 $279-570B（JPMAM $279B / Vanguard $300-570B），2027 还需 $220-300B；BNY 警告累计 $1.5T 波浪推宽利差。**AI IG 债从 R3 的 $121B 已膨胀 2-4 倍**，K11 未触发（Oracle 认购创纪录、无利差失控证据）但密度在快速上升。

### 2.3 AVGO — Q3 FY2026（9/2，D4）

- 营收 $29.59B（+86-88% YoY，超自身指引 $29.4B）；调整后 EPS $3.32 vs $3.24；**AI 半导体收入 ~$16.7B（+221% YoY，翻三倍）**。
- Q4 指引 $34.8B（+93% YoY，含 AI ~$21.7B）vs street $35.03B——差 $230M，股价跌 ~5%（高预期陷阱，非基本面恶化）。
- FY2026 AI 收入上调至 **~$58B（+186%）**（原 $56B）；FY2027 "significantly over $100B"（3 月口径）维持。合同簿：OpenAI 10GW 合作（2025.10），**Nexus 2026 底投产、2027 合同承诺 1.3GW**；Anthropic FY27 ~3GW 需求；Google 下一代 + Meta XPU 加速。VMware 软化被 AI 掩盖（非 AI 部分需盯）。
- 基本面结论：H1 的最强微观验证；$100B+ FY27 AI 收入 = 对 NVDA 的实质分流，但 TAM 扩张快于分流，二者同涨。

### 2.4 ASIC vs GPU 份额（H1 数据更新）

- 收入口径：NVDA 2026 年占 AI 加速器市场 **~80-85%**（2023 年 ~92%）——收入份额缓降。
- 单位口径：R3 的 95%→62-66% 无新季度数据直接复核，方向由三重证据支持：①AVGO AI 收入 +221%；②Google TPU 已迭代至第 8 代（8t 算力 ~3x Ironwood、8i 每美元性能 +80%，Ironwood 降为上代）；③Microsoft Maia 200（1/26 发布，自称 FP8 超 Ironwood/Trainium3）+ Trainium3 量产年。**ASIC 是增长最快的处理器类别**（多源），ASIC 服务器出货占比 27.8%（R3 基线）趋势向上。
- 结构判断：份额侵蚀是"份额稀释"而非"份额丢失"——NVDA FY27 DC 收入仍 +117%。H1 继续成立且强化。

### 2.5 TSMC — CoWoS 与资本开支（D11，H2/H4）

- Q2 2026 营收 NT$1.27T（~$40.2B，+36% YoY，超指引上限）；2026 CapEx 上调至 **$60-64B**。
- **CoWoS 售罄至 2026 年底，交期延伸入 2027**；产能路线：CoWoS ~35k wpm（2024 末）→ **~130k wpm（2026 末目标）**；先进封装整体 675k（2025）→ 1.275M（2026）→ **2.31M wpm（2027）**（io-fund）。
- 2027 年 1 月起先进制程+先进封装**涨价至多 10%**（Nikkei 7/21）——瓶颈方的定价权确认。
- H4（2027H2 缓解）：供给翻倍是事实，但需求端同步翻倍（NVDA 六芯片平台、Rubin Ultra 双 die、ASIC 四线扩产）；Rubin Ultra 因封装约束维持双 die（TrendForce 4/1）。**缓解可见、宽松未证**。

### 2.6 GOOGL / MRVL / CoreWeave（K4/K11 canary）

- **GOOGL**：$333-342（~ATH，市值 $4.08T），trailing ~16.8x（受一次性收益扭曲），Forward ~22-25x。Cloud OI $8.8B（>3x YoY）证明 TPU 自用+外销的盈利模型跑通。FCF 转负是估值核心矛盾：市场 7/22 用下跌投票 CapEx。TPU 优先内部 AGI 研发，外部分配受限——Ironwood/8 系对 NVDA 的替代在收入端已可观测（Cloud +82% 加速）。
- **MRVL**（8/27，Q2 FY27）：营收 $2.739B（+37%，纪录，超指引中值 $39M），EPS $0.94 vs $0.93；FY27 上调至 ~$12B（+45%，原 $11.5B）；Q3 指引略超共识 ~$3.03B。**股价仍跌 >2%**：未上调长期展望 + Google 客户集中焦虑（Stifel 测算 Google 定制芯片 7 年 ~$120B）。10/6 Investor Day 是下一个催化。维持小仓位观察仓定位。
- **CoreWeave**（8/11，Q2）：营收 $2.575B（+112% YoY），净亏损 $626M（-24% 利润率，好于预期的 -$1.49 EPS）；backlog **$104B（+246%）**另有季末后 >$25B 新签；FY26 收入指引上调至 $12.4-13.2B。**利息费用 $640M/季（YoY $267M），指引 ~$860M/季**；单季举债 >$10B（无担保+可转债，结构向无担保迁移）；Q2 CapEx $9.4B。股价上涨。**K4/K11 判定：违约触发否；债务机器全速运转但市场仍愿接——canary 活着，呼吸声更粗。**

### 2.7 租金与 Token 价格数据线（D5/D6）

- **H100**：neocloud 指数 $2.43-2.63/hr（SDH100RT ~$2.53）；spot/社区 $1.33-1.99（Vast.ai $1.33 最低）；hyperscaler on-demand 均值 $7.89。1 年期合约 $1.70（2025.10）→ $2.35（2026.3）→ Q3 +20-22%。**K4（<$1.5 持续两周）远离触发**——R3 的"spot $0.79-1.40"更接近可中断现货低沿，中位口径实际走强。
- **B200**：on-demand 中位 ~$6.79（$3.75-9.86 区间），新世代紧俏结构不变。
- **Token**：混合价 10 周 -43%（$2.04→$1.16/1M）；前沿指数较 2023.3 基点 -84%；K5（任两家同季 >50%）未确认单一厂商腰斩，但市场混合价单季 -43% 已属"早期预警上限"；总量推理支出仍上升（用量>单价）。K12：支出指数未获得公开连续序列，待验证，但方向（量补价）成立。

---

## 三、假设验证

| 假设 | 判断 | 证据 | 置信度(1-5) |
|---|---|---|:---:|
| H1 ASIC 推理份额 2028 增至 30-40% | **成立（强化）** | AVGO AI +221%、FY27 >$100B；TPU 8t/8i 迭代；Maia 200/Trainium3 量产；NVDA 收入份额 92%→80-85% | 4 |
| H2 CoWoS 瓶颈持续至 2027 | **成立（强化）** | CoWoS 售罄至 26 年底、交期入 2027；TSMC 涨价 10%；Rubin Ultra 因封装约束改双 die | 4 |
| H3 推理成本年降 ~10x | **成立** | Token 混合价 10 周 -43%；恒定性能年降 ~10x 多源；但总支出量升价降 | 4 |
| H4 CoWoS 扩产 2027H2 缓解 | **待验证（偏紧）** | 先进封装 27 年 2.31M wpm 翻倍，但需求同步翻倍；Rubin 双 die 上限仍在 | 3 |
| H5 CapEx 可持续至 2027 | **有条件成立（融资依赖加深）** | 2026 全部上调至 ~$733B；2027 方向性全升、street $1.09-1.4T；但 GOOGL/META FCF 转负/近零、AI 债 $279-570B、2027 占 OCF ~90% | 4 |

**退场标准快照**：K2 未触发（全部上调）；K4 远离触发（租金上涨）；K5 早期预警（混合价 -43%/10 周，接近但未确认双厂商 >50%）；K6 远离触发（+117%）；K9 部分触发（Meta Compute 已官宣未定价未上线，Anthropic 租站 $1.25B/年；第二家跟进未证实，NVDA 回租 neocloud 二源确认未获得——待验证）；K10 未获得 Q2 折旧表述变化（待验证）；K11 预警未触发（Oracle IG 创纪录认购）；K12 待验证（量价剪刀差健康）。

---

## 四、情景分析

| 情景 | 概率 | 核心驱动 | 组合预期回报 |
|------|:----:|---------|:-----------:|
| Bull | 25% | FY28 +70% 兑现 + 2027 CapEx 落地 $1.2T+ + Rubin 爬坡干净 + AVGO FY27 AI >$120B；NVDA 重估 28-30x | +25% |
| Base | 50% | 执行延续但 PE 停在 22-24x；2027 CapEx +15-25%（方向性转正式）；FCF 负值常态化但债市照单全收 | +9% |
| Bear | 25% | 2027 融资缺口显性化（$612B > 净发行）或某家 2027 指引仅 +10-15%；Meta Compute 上线+API 通缩压垮 neocloud 传导；NVDA 降 16-18x | -22% |
| **加权** | | | **+5.3%** |

（分标的 Base：NVDA +10% / AVGO +9% / GOOGL +10% / MRVL +3%；Bull：+30/+22/+18/+15%；Bear：-25/-20/-15/-18%）

---

## 五、时间维度

- **短期(1-3月)**：MSFT/GOOGL/META Q3 财报（10 月底）给出 2027 首批半量化口径；MRVL Investor Day（10/6）；FOMC 9/16；Rubin 出货爬坡数据；AVGO 高预期消化。**2027 正式指引是最大单一催化剂。**
- **中期(3-12月)**：Nexus 2026 底投产→2027 1.3GW 兑现；Rubin Ultra 双 die 2027 发布；AI 债 $220-300B 增发测试市场容量；CoWoS 2.31M wpm 扩产 vs 需求赛跑；Meta Compute 是否定价上线（K9）。
- **长期(1-3年)**：ASIC 份额 30-40% 路径验证；2027 CapEx/OCF ~90% 的可持续性边界；推理量价剪刀差能否维持"通缩不通缩收入"；四芯→双 die 后 NVDA 每美元算力路线图重置。

---

## 六、基本面排名（研究员A 视角）

| 排名 | 标的 | 一句话理由 | 操作倾向 |
|:---:|---|---|---|
| 1 | NVDA | Beat+大超指引+FY28 +70% 可见性，PEG <0.5；唯价格已越过 R3 入场带 | 持有/回调加仓，勿追高 |
| 2 | AVGO | AI +221%、FY27 >$100B、合同簿 13GW+；-5% 提供更好入场 | 持有/逢跌加仓 |
| 3 | GOOGL | Cloud +82% 加速+backlog $514B+最便宜头部 AI 资产；FCF 转负是主要瑕疵 | 持有 |
| 3.5 | TSM（关联） | 售罄+涨价 10%+CapEx 上调，瓶颈定价权 | 关联配置 |
| 4 | MRVL | 基本面 beat-raise 但缺长期展望上修，Google 集中度焦虑 | 0-3% 观察，10/6 前不加 |

---

## 七、数据来源

| # | 数据点 | 来源 | 时间 | 可靠性 |
|---|--------|------|------|:------:|
| 1 | NVDA Q2 FY27 营收/DC/Rubin 量产/Q3 指引 | NVIDIA 官方新闻稿 nvidianews | 2026-08-26 | 高 |
| 2 | NVDA FY28 +70%/供给受限、中国零假设 | Q2 FY27 电话会转录（q4cdn PDF） | 2026-08-26 | 高 |
| 3 | NVDA $224.41、Forward PE 24.2 | GuruFocus / Yahoo Finance | 2026-09-03 | 高 |
| 4 | Rubin Ultra 双 die/CoWoS-L 翘曲 | Tom's Hardware / TrendForce / Wccftech | 2026-03~07 | 中高 |
| 5 | 四大 2026 CapEx ~$733B 及分项 | Mohit Agrawal(LinkedIn)/digitalapplied/CNBC | 2026-07-28~31 | 中高 |
| 6 | GOOGL Q2（backlog $514B、FCF -$5.9B、$195-205B） | SEC 8-K/CNBC/Fierce Network | 2026-07-22 | 高 |
| 7 | META Q2（FCF $784M、发债 $24.9B） | Meta IR/SEC/Fortune/CNBC | 2026-07-29 | 高 |
| 8 | AMZN $220B、产能紧到 2027、AWS +37% | Amazon IR/CNBC/mlq.ai | 2026-07-30 | 高 |
| 9 | MSFT FY26Q4（Azure +43%、季度 CapEx >$50B） | Microsoft IR/CNBC/Morningstar | 2026-07-29 | 高 |
| 10 | 2027 无正式指引、street $1.09-1.4T、90% OCF | 2027 guidance 分析/Barclays/WF/MS via 汇总 | 2026-08 | 中 |
| 11 | AVGO Q3 FY26 全套 + OpenAI 1.3GW/Nexus | CNBC/Broadcom IR/Baptista/AlphaSense | 2026-09-02 | 高 |
| 12 | CoWoS 售罄/130k wpm/$60-64B/涨价 10% | VanEck/AI Weekly/io-fund/Nikkei via LinkedIn | 2026-07~08 | 中高 |
| 13 | NVDA 份额 80-85%（收入口径） | Silicon Analysts/Presenc/Kaiso | 2026 | 中 |
| 14 | TPU 8t/8i、Maia 200、Ironwood 代际 | Google blog/Microsoft blog/CNBC | 2026-01~07 | 高 |
| 15 | MRVL Q2 FY27 与股价反应 | Marvell IR/Reuters/IBD | 2026-08-27 | 高 |
| 16 | CRWV Q2（$2.575B、利息 $640M、backlog $104B） | CoreWeave IR/SEC/CNBC | 2026-08-11 | 高 |
| 17 | H100 ~$2.5/B200 ~$6.8 租金、合约价上行 | SiliconData/GetDeploying/RunPod/Tech-Insider | 2026-08~09 | 中高 |
| 18 | Token 混合价 -43%/10 周 | alicantetechvies/BenchLM/TokenPriceIndex | 2026-08-08 | 中 |
| 19 | AI 债 $279-570B、Oracle $25B、$612B vs $470B | Vanguard/JPMAM/FT/Bridgewater via Reddit 汇总 | 2026-08 | 中 |
| 20 | Meta Compute 未定价、Anthropic 租站 $1.25B | Bloomberg/Axe Compute | 2026-07-01~08 | 中高 |

> 方法论备注：anysearch MCP 首批配额耗尽后回退 WebSearch（web_search_prime 后端）。未覆盖：K10 折旧年限 Q2 表述（未检索到变化，标待验证）；K12 连续月度支出指数（公开序列缺失）；NVDA 财报当日单日股价反应精确值（待验证）。
