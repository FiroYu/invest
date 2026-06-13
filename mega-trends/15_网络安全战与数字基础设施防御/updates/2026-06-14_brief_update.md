# 网络安全战与数字基础设施防御 动态更新 2026-06-14

## 关键进展

1. **Miasma供应链蠕虫源码泄露GitHub，衍生"Hades"攻击浪潮** - 继6月1日Miasma蠕虫攻破Red Hat @redhat-cloud-services官方npm包（32个包、~95个恶意版本、11.6万周下载量、0个CVE）之后，攻击工具包的**完整源码于6月11日前后通过被攻破的开发者账号泄露至GitHub公开仓库**。多个安全厂商（SafeDep、TechJack、Rescana、Security Boulevard）在6月11–13日密集预警：泄露后的工具包已被武器化为代号为**"Hades"的新攻击浪潮**，攻击面从npm扩展至**PyPI、RubyGems及CI/CD流水线**，注入恶意代码并窃取GitHub令牌、云平台凭据与本地密钥。（SafeDep / TechJack Solutions / Rescana ThreatsDay Bulletin / Security Boulevard，6月11–13日）

2. **Shai-Hulud V2演进：AI扫描器规避能力确认** - Zscaler ThreatLabz 2025年11月首次披露的Shai-Hulud V2软件供应链攻击活动持续演进。安全分析（Security Boulevard，6月13日）确认该系列（Miasma → Hades）已具备**规避主流AI代码扫描器**的能力——传统签名/哈希检测和AI语义扫描双重失效。这标志着供应链攻击进入"AI对抗AI"阶段：攻击侧同样在使用AI生成多态、低熵的恶意代码以绕过防御。（Security Boulevard，6月13日）

3. **同期高密度事件集群** - 6月11日Rescana ThreatsDay Bulletin同一窗口内还记录：针对**AI Agent的成功钓鱼攻击**（冒充工具调用诱导Agent泄露凭据）、Anthropic发布**Claude Code GitHub Action高危补丁**、以及Palo Alto GlobalProtect VPN认证绕过漏洞被在野利用（超4万台服务器被控）、cPanel大规模利用（4万+服务器）。供应链蠕虫+AI Agent攻击+开发工具链漏洞在同一周叠加，显示攻击面正沿"AI原生开发栈"快速扩散。（Rescana / Innovate Cybersecurity，6月1–13日）

## 影响评估

- **对该议题的影响**：本次升级是议题核心论点——"网络安全战从外周防御转向数字基础设施（供应链/开发工具链/AI Agent）内生威胁"——的**强实证**。三重变化值得重视：
  1. **攻击工业化**：Miasma源码公开=供应链蠕虫工具民主化，未来将出现大量派生变种（如同勒索软件即服务RaaS对勒索赛道的影响）。防御侧的边际成本将系统性上升。
  2. **AI Agent成新攻击面**：针对AI Agent的成功钓鱼首次被批量记录，叠加Claude Code官方Action漏洞。随着企业Agent部署放量，**Agent凭据/权限管理**将成为下一个安全支出爆发点（利好CIEM/Agent安全赛道）。
  3. **AI扫描器规避**：攻防双方都在用AI，单纯依赖AI检测的安全产品（部分NGS/SASE厂商卖点）面临质疑，**"人在回路"+供应链完整性证明（如Sigstore/产物溯源）**的价值凸显。

- **投资含义**：
  - **利好**：PANW（NGS ARR加速，6/5已记录）、CRWD、Snyk/Semgrep/Chainguard等供应链安全与SCA厂商、AI Agent安全新锐。
  - **承压/需观察**：过度依赖"AI自动检测"叙事的纯检测类工具；开源生态治理成本上升对云厂商CI/CD负担。
  - **指标跟踪**：6/5 update中PANW NGS ARR（59-60%增长）与CRWD指引仍是主线，本次事件是**需求侧催化剂验证**而非基本面拐点。

## 信源

- [Inside the Miasma Software Supply Chain Attack Toolkit - SafeDep](https://safedep.io/inside-the-miasma-supply-chain-attack-toolkit/)
- [Miasma Supply Chain Worm Toolkit Leak Fuels Hades Campaign - TechJack Solutions](https://techjacksolutions.com/scc-intel/miasma-supply-chain-worm-toolkit-leak-fuels-hades-campaign-against-open-source-registries-and-ci-cd-pipelines/)
- [ThreatsDay Bulletin June 2026: Miasma Supply Chain Worm Leak - Rescana](https://www.rescana.com/post/threatsday-bulletin-june-2026-miasma-supply-chain-worm-leak-claude-code-github-action-vulnerability-ai-agent-phishing-to)
- [Shai-Hulud Campaign Evolution: Miasma, Hades, and AI Scanner Evasion - Security Boulevard](https://securityboulevard.com/2026/06/shai-hulud-campaign-evolution-miasma-hades-and-ai-scanner-evasion/)
- [The Miasma worm's path of destruction - Cloudsmith](https://cloudsmith.com/blog/miasma-worms-path-of-destruction)
- [Open Source Package Registries / GitHub / CI/CD Vulnerability Rollup 2026-06-11 - TechJack Solutions](https://techjacksolutions.com/scc-vendor-rollup/open-source-package-registries-github-ci-cd-vulnerability-rollup-2026-06-11/)
- [Preinstall to persistence: Inside the Red Hat npm Miasma campaign - Microsoft Security Blog](https://www.microsoft.com/en-us/security/blog/2026/06/02/preinstall-persistence-inside-red-hat-npm-miasma-credential-stealing-campaign/)
