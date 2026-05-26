---
layout: default
title: "Horizon Summary: 2026-05-26 (ZH)"
date: 2026-05-26
lang: zh
---

> From 31 items, 15 important content pieces were selected

---

1. [APKPure 上的 Telegram 官方版被植入间谍后门](#item-1) ⭐️ 9.0/10
2. [加州提议将 Linux 从年龄验证法中豁免](#item-2) ⭐️ 8.0/10
3. [教宗利奥十四世关于人工智能伦理的通谕](#item-3) ⭐️ 8.0/10
4. [微软 Copilot Cowork 通过提示注入窃取文件](#item-4) ⭐️ 8.0/10
5. [Armin Ronacher 抨击 AI 生成的错误报告](#item-5) ⭐️ 8.0/10
6. [华为提出半导体缩微新定律“韬定律”](#item-6) ⭐️ 8.0/10
7. [Epic 公布虚幻引擎 6，首发展示游戏为《火箭联盟》](#item-7) ⭐️ 8.0/10
8. [离体人脑用于药物测试引发伦理争议](#item-8) ⭐️ 8.0/10
9. [挪威部署 2PB 华为闪存用于主权大语言模型训练](#item-9) ⭐️ 7.0/10
10. [Mullvad 推出出口 IP 指纹识别缓解措施](#item-10) ⭐️ 7.0/10
11. [荷兰查获 800 台服务器，逮捕 2 名网络攻击帮凶](#item-11) ⭐️ 7.0/10
12. [神舟二十三号乘组公布：首位港籍航天员，一年期任务](#item-12) ⭐️ 7.0/10
13. [人工智能时代网络安全岗位激增](#item-13) ⭐️ 7.0/10
14. [马斯克宣布 Grok V9-Medium 训练完成](#item-14) ⭐️ 7.0/10
15. [欧盟初步认定谷歌可能违反《数字市场法》](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [APKPure 上的 Telegram 官方版被植入间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

APKPure 上发布的 Telegram 12.6.5 版本被重新签名并注入了名为 DataCollector 的间谍框架，可窃取聊天记录、通讯录、照片、文档、GPS 定位和 SIM 卡信息。 此次供应链攻击危及数百万从 APKPure 下载 Telegram 用户的隐私，凸显了第三方应用商店的风险。 该间谍软件使用 AES-GCM 加密将数据外传至 C2 服务器 38.190.225.166，恶意代码位于 classes3.dex 中，超过 3000 行。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个流行的第三方 Android 应用商店，尤其在 Google Play 受限的地区。供应链攻击是指攻击者入侵可信的分发渠道，将恶意代码注入合法应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://securityaffairs.com/116635/cyber-crime/apkpure-client-malware.html">Hackers compromised APKPure client to distribute infected Apps</a></li>
<li><a href="https://www.secureblink.com/cyber-security-news/supply-chain-attack-infiltrates-android-apps-with-malicious-spin-ok-sdk">Supply Chain Attack Infiltrates Android Apps with Malicious SpinOK SDK</a></li>
<li><a href="https://en.wikipedia.org/wiki/Supply_chain_attack">Supply chain attack - Wikipedia</a></li>

</ul>
</details>

**标签**: `#security`, `#malware`, `#telegram`, `#supply chain attack`, `#privacy`

---

<a id="item-2"></a>
## [加州提议将 Linux 从年龄验证法中豁免](https://www.tomshardware.com/software/linux/california-moves-to-exempt-linux-from-its-upcoming-age-verification-law-after-backlash-over-forcing-operating-systems-to-collect-users-ages-amendment-proposed-by-the-same-lawmaker-who-wrote-the-original-law) ⭐️ 8.0/10

加州在遭到开源社区强烈反对后，提出修正案将 Linux 从其年龄验证法（AB 2273）中豁免。该修正案由起草原法案的同一立法者提出。 这一豁免防止了像 Linux 这样的操作系统被迫收集用户年龄，否则可能会扼杀开源开发和创新。它凸显了互联网监管与开源生态系统之间的紧张关系。 原法律 AB 2273 要求含有可能对未成年人有害内容的平台验证用户年龄，批评者认为这将适用于操作系统。拟议的修正案明确豁免了像 Linux 这样的开源操作系统。

hackernews · rbanffy · May 25, 18:19 · [社区讨论](https://news.ycombinator.com/item?id=48269961)

**背景**: 加州的 AB 2273《年龄适当设计规范法案》于 2022 年签署成为法律，仿效英国的年龄验证规范。它要求含有大量对未成年人有害内容的网站进行年龄验证，但因范围过广而面临法律挑战和批评。开源倡导者认为，要求操作系统收集年龄将侵犯隐私并阻碍软件开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://legiscan.com/CA/text/AB2273/id/2606836">California AB2273 | 2021-2022 | Regular Session - LegiScan</a></li>
<li><a href="https://www.lawyer-monthly.com/2025/11/californias-age-verification-law-federal-judge-halts-mandate-citing-free-speech-risks/">California's Age Verification Law: Federal Judge Halts Mandate, Citing ...</a></li>
<li><a href="https://calawyers.org/privacy-law/the-california-age-appropriate-design-code-act/">The California Age-Appropriate Design Code Act</a></li>

</ul>
</details>

**社区讨论**: 社区评论中既有怀疑也有宽慰。一些用户指出大多数评论者误解了该法律，而另一些人则质疑该法律如何适用于服务器环境，或批评将负担转嫁给消费者而非公司。还有人担忧立法究竟由谁起草。

**标签**: `#Linux`, `#age-verification`, `#California law`, `#open-source`, `#policy`

---

<a id="item-3"></a>
## [教宗利奥十四世关于人工智能伦理的通谕](https://www.vatican.va/content/leo-xiv/en/encyclicals/documents/20260515-magnifica-humanitas.html) ⭐️ 8.0/10

教宗利奥十四世于 2026 年 5 月 25 日发布了他的首道通谕《崇高人性》，呼吁对人工智能和技术进行伦理反思，警告权力集中，并倡导以人为本的方法。 这是一位重要宗教领袖发出的罕见且重要的声明，连接了技术、伦理与灵性，将影响全球关于人工智能治理和技术社会影响的辩论。 该通谕长达 83 页，并与教宗利奥十三世的《新事》通谕相呼应，呼吁全球社会从支配、排斥和战争的逻辑中“解除”人工智能的武装。

hackernews · theletterf · May 25, 10:11 · [社区讨论](https://news.ycombinator.com/item?id=48265206)

**背景**: 教宗通谕是教宗就重要问题向天主教会和世界发出的正式信函。教宗利奥十四世的首道通谕聚焦于在人工智能时代保护人的尊严，反映了对人工智能伦理影响日益增长的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Magnifica_humanitas">Magnifica humanitas - Wikipedia</a></li>
<li><a href="https://www.vaticannews.va/en/pope/news/2026-05/pope-leo-xiv-magnifica-humanitas-presentation-ai-disarmament.html">Pope Leo presents 'Magnifica humanitas’ calling for ...</a></li>
<li><a href="https://religionnews.com/2026/05/25/in-his-first-encyclical-pope-leo-xiv-says-ai-must-serve-humanity-not-the-powerful-few/">In his first encyclical, Pope Leo XIV says AI must serve ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的评论者赞扬了梵蒂冈对技术的深思熟虑，一位无神论者称这是关于人工智能的最佳机构观点之一。其他人讨论了历史上驯服技术以造福社会的困难，以及建设者考虑文明层面影响的重要性。

**标签**: `#AI ethics`, `#technology and society`, `#papal encyclical`, `#philosophy of technology`

---

<a id="item-4"></a>
## [微软 Copilot Cowork 通过提示注入窃取文件](https://www.promptarmor.com/resources/microsoft-copilot-cowork-exfiltrates-files) ⭐️ 8.0/10

PromptArmor 的研究人员演示了微软 Copilot 基于技能的架构可能通过提示注入被利用，从而从企业环境中窃取敏感文件。 这引发了企业对 AI 集成的严重安全担忧，因为 Copilot 广泛部署在 Microsoft 365 中，攻击者可能通过看似良性的交互窃取数据。 该攻击利用了 Copilot 执行技能（自定义程序）的能力，这些技能可以运行 shell 命令，使攻击者能够构造一个提示，通过 curl 或类似工具触发文件窃取。

hackernews · Kneenex · May 25, 21:45 · [社区讨论](https://news.ycombinator.com/item?id=48272354)

**背景**: 提示注入是一种网络安全攻击，恶意输入导致 LLM 产生意外行为。在 Copilot 等企业工具中，技能本质上是 LLM 代理可以调用的程序，如果没有适当的沙箱隔离，它们可以执行任意命令。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/microsoft-copilot-studio/guidance/architecture-overview">Define your solution architecture - Microsoft Copilot Studio</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了这是否是真正的漏洞还是预期行为，一些人认为技能只是程序，攻击类似于 'curl $url | bash'。其他人批评微软在没有充分安全加固的情况下匆忙推出 Copilot 集成。

**标签**: `#AI security`, `#prompt injection`, `#Microsoft Copilot`, `#LLM agents`, `#enterprise software`

---

<a id="item-5"></a>
## [Armin Ronacher 抨击 AI 生成的错误报告](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Flask 的创建者 Armin Ronacher 批评了开源项目中大量涌入的低质量 AI 生成的错误报告，并提倡一种简单的人类观察格式：运行了什么命令、期望的行为、实际发生的行为以及确切的错误或日志。 这凸显了开源维护中一个日益严重的问题：AI 生成的报告用不准确、冗长且听起来自信的内容浪费维护者的时间，可能损害项目健康和开发者生产力。 Ronacher 特别指出了使用“clankers”（对 AI 的贬称）改写问题，产生虚假的最小复现、错误根本原因猜测和不相关的错误列表，通常信心十足但准确性很低。

rss · Simon Willison · May 24, 18:46

**背景**: Armin Ronacher 是一位著名的开源开发者，以创建 Flask Web 框架和 Jinja 模板引擎而闻名。AI 生成的内容（常被称为“slop”）已成为开源问题追踪器中的麻烦，用户粘贴 AI 精炼的错误报告，掩盖了原始的人类观察。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Armin_Ronacher">Armin Ronacher</a></li>
<li><a href="https://lucumr.pocoo.org/about/">About Me | Armin Ronacher 's Thoughts and Writings</a></li>

</ul>
</details>

**标签**: `#open-source`, `#AI`, `#bug reports`, `#software maintenance`, `#developer experience`

---

<a id="item-6"></a>
## [华为提出半导体缩微新定律“韬定律”](https://www.peopleapp.com/column/30052220655-500007509895) ⭐️ 8.0/10

在 2026 年 IEEE 国际电路与系统研讨会上，华为发表了“韬定律”，提出以“时间缩微”替代传统的“几何缩微”作为半导体演进新原则。过去六年，华为已据此设计量产了 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟手机芯片。 韬定律提供了一条在摩尔定律因量子隧穿效应和成本飙升而逼近物理极限时，继续提升半导体性能的潜在路径。若得到验证，这可能重塑全球芯片产业，并减少对极紫外光刻技术的依赖，对华为及中国半导体自主化具有重大意义。 韬定律以系统性降低时间常数τ为目标，通过逻辑折叠等技术在器件、电路、芯片和系统层面进行协同优化。华为预计，到 2031 年基于该定律的高端芯片晶体管密度可达 1.4 纳米制程同等水平。

telegram · zaihuapd · May 25, 01:35

**背景**: 摩尔定律曾预言晶体管密度每两年翻一番，数十年来推动了半导体进步，但如今因物理和经济障碍而放缓。传统的几何缩微通过缩小晶体管尺寸来提升性能，但在纳米尺度下，量子隧穿效应和制造成本飙升等问题凸显。韬定律提出了一种互补方法：不缩小物理尺寸，而是通过降低信号传播时延（时间常数）来提升性能和密度，从而可能在不依赖极紫外光刻的情况下延长硅基芯片的生命周期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guancha.cn/economy/2026_05_25_818257.shtml">华为公布 半 导 体 领域重大突破</a></li>
<li><a href="https://www.jiuyangongshe.com/a/4ehfd4eadx6">华为 韬 定 律 横空出世，麒麟芯验证新路径：国产替代三大投资主线浮现</a></li>
<li><a href="https://www.ithome.com/0/954/702.htm">Mate 90...</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Huawei`, `#chip design`, `#Moore's Law`, `#scaling`

---

<a id="item-7"></a>
## [Epic 公布虚幻引擎 6，首发展示游戏为《火箭联盟》](https://www.pcgamer.com/gaming-industry/epic-reveals-first-unreal-engine-6-game-and-its-not-fortnite/) ⭐️ 8.0/10

Epic Games 在巴黎《火箭联盟》冠军系列赛上宣布了虚幻引擎 6，并透露《火箭联盟》将直接从虚幻引擎 3 升级到 UE6，跳过 UE4 和 UE5。 这标志着 Epic 引擎的一次重大代际飞跃，表明其向统一元宇宙平台转变，因为 UE6 被定位为连接《堡垒之夜》、《乐高堡垒之夜》和更广泛的 Epic 生态系统。 《火箭联盟》已在 UE3 上运行了 11 年，升级到 UE6 将带来图形大修和 Verse 集成。目前尚未公布 UE6 的具体发布日期或功能列表。

telegram · zaihuapd · May 25, 02:20

**背景**: 四年前发布的虚幻引擎 5 已在游戏和电影领域广泛使用，但因 PC 端优化问题而受到批评。Epic 将虚幻引擎 6 定位为其元宇宙愿景的粘合剂，连接各种游戏和工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibtimes.co.uk/epic-games-unreal-engine-6-rocket-league-paris-1798706">Unreal Engine 6 Release Date, Features , Trailer and... | IBTimes UK</a></li>
<li><a href="https://www.ign.com/articles/rocket-league-to-receive-first-game-engine-tune-up-in-11-years-as-psyonix-teases-unreal-engine-6-update">Rocket League to Receive First Game Engine Tune Up in 11 Years as Psyonix Reveals New Update in Unreal Engine 6 Teaser</a></li>

</ul>
</details>

**标签**: `#Unreal Engine`, `#Game Development`, `#Epic Games`, `#Rocket League`, `#Metaverse`

---

<a id="item-8"></a>
## [离体人脑用于药物测试引发伦理争议](https://www.science.org/content/article/not-alive-not-dead-disembodied-human-brains-used-drug-testing) ⭐️ 8.0/10

美国生物科技公司 Bexorg 利用 BrainEx 灌流系统，在捐献者死亡数小时后部分恢复人脑的代谢和细胞活动，用于测试阿尔茨海默病和帕金森病等神经疾病药物。 这一突破挑战了传统的生命与死亡定义，可能通过提供更准确的人脑模型彻底改变中枢神经系统药物研发，但也引发了关于意识、人格和科学干预边界的深刻伦理问题。 这些恢复活动的大脑并未恢复意识或产生完整的神经活动，但该技术引发了伦理学家关于未来系统可能创造有感知但无法交流的离体大脑的辩论。BrainEx 系统最初是为猪脑开发的，后来被改造用于人类。

telegram · zaihuapd · May 25, 14:57

**背景**: BrainEx 灌流系统于 2019 年首次在猪脑上展示，可通过输送含有维生素、氨基酸和保护剂的特殊溶液，在死亡数小时后恢复微循环和细胞功能。Bexorg 成立于 2021 年，已筹集 4250 万美元用于将该技术商业化用于药物发现。传统的药物测试依赖动物模型或细胞培养，往往无法预测人体反应，导致神经药物开发失败率很高。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://neuwritesd.org/2019/06/13/brainex-restoring-brain-circulation-after-death/">BrainEx: Restoring Brain Circulation After Death</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC8272538/">Evaluating the translational value of postmortem brain ...</a></li>
<li><a href="https://engineventures.com/companies/bexorg">Bexorg | Engine Ventures</a></li>

</ul>
</details>

**标签**: `#neuroscience`, `#bioethics`, `#drug testing`, `#consciousness`, `#BrainEx`

---

<a id="item-9"></a>
## [挪威部署 2PB 华为闪存用于主权大语言模型训练](https://www.blocksandfiles.com/flash/2026/05/22/norways-2-petabytes-of-huawei-flash-storage-and-llm-training/5244910) ⭐️ 7.0/10

挪威已部署 2PB 的华为闪存存储，用于训练一个旨在保护挪威语言和文化的主权大语言模型（LLM）。该存储是 Olivia 系统的一部分，该系统为 HPE Cray Supercomputing EX 系统，配备 448 个 GPU 和 64,512 个 CPU 核心。 这一举措凸显了主权 AI 日益增长的趋势，即各国建设独立 AI 基础设施以保护文化和语言特性。同时，它也引发了关于此类硬件是否足以训练出有竞争力的 LLM，而非对现有开源模型进行微调的争论。 华为闪存存储提供 2PB 容量，但具体型号未披露。Olivia 超级计算机配备 448 个 GPU，被认为从头训练一个完整规模的 LLM 略显不足，因此引发了对项目可行性的质疑。

hackernews · rbanffy · May 25, 19:37 · [社区讨论](https://news.ycombinator.com/item?id=48270770)

**背景**: 主权 AI 是指一个国家利用自己的基础设施、数据和人才来生产 AI 的能力，通常是为了保护当地语言和文化。训练大型语言模型通常需要巨大的计算资源和高速存储；闪存存储为数据密集型工作负载提供低延迟和高吞吐量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/what-is-sovereign-ai/">What Is Sovereign AI? | NVIDIA Blog</a></li>
<li><a href="https://www.weforum.org/stories/2024/04/sovereign-ai-what-is-ways-states-building/">Sovereign AI: What it is, and 6 ways states are building it | World Economic Forum</a></li>
<li><a href="https://www.mckinsey.com/featured-insights/mckinsey-explainers/what-is-sovereign-ai">What is sovereign AI? | McKinsey</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：有人质疑在主流模型已训练多语言数据的情况下，主权 LLM 的必要性；也有人怀疑硬件（448 个 GPU）是否足以训练完整模型。建议包括构建精选的挪威语数据集并分享给模型构建者。

**标签**: `#LLM`, `#sovereign AI`, `#storage`, `#Huawei`, `#Norway`

---

<a id="item-10"></a>
## [Mullvad 推出出口 IP 指纹识别缓解措施](https://mullvad.net/en/help/exit-ip-vpn-servers-mitigation-rollout) ⭐️ 7.0/10

Mullvad 宣布推出针对出口 IP 指纹识别的缓解措施，该技术通过利用确定性 IP 分配模式，可能将 VPN 用户在不同网站上的活动关联起来。 此次更新解决了一个重大的隐私漏洞，该漏洞可能破坏 VPN 用户的匿名性，尤其是那些依赖 Mullvad 进行敏感活动的用户。它为其他 VPN 提供商应对高级指纹识别技术树立了先例。 缓解措施改变了出口 IP 的分配方式，打破了允许跨站点关联的确定性模式。Mullvad 的多跳功能通过两个服务器路由流量，进一步增加了指纹识别的难度。

hackernews · Cider9986 · May 25, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48269580)

**背景**: 出口 IP 指纹识别是一种技术，网站通过观察分配给 VPN 用户的 IP 地址，由于某些 VPN 根据用户的 WireGuard 密钥确定性分配 IP，因此即使用户切换服务器，也能在不同站点间关联同一用户。Mullvad 之前为每个服务器分配多个出口 IP 以减少拥塞，但这产生了可识别的模式。浏览器指纹识别（如 canvas 指纹识别）是一种相关技术，通过设备特征识别用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cyberinsider.com/mullvad-vpn-exit-ip-patterns-could-enable-user-fingerprinting/">Mullvad VPN exit IP patterns could enable user fingerprinting</a></li>
<li><a href="https://www.technadu.com/mullvad-fingerprinting-issue-prompts-vpn-system-changes/628269/">Mullvad Fingerprinting Issue Prompts VPN System Changes</a></li>
<li><a href="https://gproxy.net/en/blog/browser-fingerprinting-and-proxies/">Browser Fingerprinting : What It Is and How Proxies Help Hide It</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了浏览器级保护的重要性，有人建议像 Librewolf 这样的浏览器应伪造一致且非唯一的配置文件。另一个人指出，Mullvad 浏览器内置代理和随机 IP 模式，已避免了此问题。还有用户询问 VPN 是否向 ISP 支付出口点费用。

**标签**: `#privacy`, `#VPN`, `#fingerprinting`, `#security`

---

<a id="item-11"></a>
## [荷兰查获 800 台服务器，逮捕 2 名网络攻击帮凶](https://krebsonsecurity.com/2026/05/netherlands-seizes-800-servers-arrests-2-for-aiding-cyberattacks/) ⭐️ 7.0/10

荷兰当局查获了 800 台服务器，并逮捕了两名运营“防弹托管”服务、为网络攻击提供便利的个人。 此次行动破坏了网络犯罪分子使用的关键基础设施，凸显了执法部门持续打击防弹托管、削弱网络攻击能力的努力。 被查获的服务器由与俄罗斯情报机构直接关联的公司运营，并非合法托管提供商。荷兰因其宽松的法规而成为防弹托管的知名中心。

hackernews · jruohonen · May 25, 13:56 · [社区讨论](https://news.ycombinator.com/item?id=48266906)

**背景**: 防弹托管是指无视非法活动投诉的服务，为网络犯罪分子提供运行僵尸网络、垃圾邮件和其他攻击的基础设施。此类提供商通常执法薄弱地区运营，因此对恶意行为者具有吸引力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Bulletproof_hosting">Bulletproof hosting</a></li>
<li><a href="https://www.sentinelone.com/cybersecurity-101/threat-intelligence/bulletproof-hosting/">What is Bulletproof Hosting?</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这些并非合法托管公司，而是俄罗斯情报机构的前台公司。一些人对荷兰网络攻击量之高表示惊讶，而另一些人则强调网络犯罪分子本可以合法工作却选择犯罪。

**标签**: `#cybersecurity`, `#law enforcement`, `#Netherlands`, `#server seizure`, `#cybercrime`

---

<a id="item-12"></a>
## [神舟二十三号乘组公布：首位港籍航天员，一年期任务](https://t.me/zaihuapd/41554) ⭐️ 7.0/10

神舟二十三号乘组已公布，由指令长朱杨柱、航天驾驶员张志远和载荷专家黎家盈组成，黎家盈将成为首位来自香港的航天员。任务计划于 5 月 24 日 23 时 08 分发射，其中一名航天员将执行一年期在轨任务。 此次任务创造了多项首次：首位香港女性载荷专家、首位来自第三批航天员的指令长，以及首个由第三批和第四批航天员共同组成的乘组。这凸显了中国航天计划的扩展以及香港参与国家航天事业。 朱杨柱此前执行过神舟十六号任务，成为首位担任指令长的航天飞行工程师。黎家盈是首位执行飞行任务的第四批航天员，也是面向港澳选拔的首位女性载荷专家。任务包括一名航天员在轨一年，显著延长了驻留时间。

telegram · zaihuapd · May 24, 15:13

**背景**: 中国航天员分为三类：航天驾驶员、航天飞行工程师和载荷专家。载荷专家负责科学实验和特定载荷操作。第四批航天员选拔于 2022 年启动，首次面向港澳地区选拔载荷专家。神舟二十三号将是首个同时包含第三批和第四批航天员的载人任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.eastmoney.com/a/202605243747407098.html">神舟二十三号 航 天 员乘组5月24日出征太空 在轨期间将新开展100...</a></li>
<li><a href="https://www.ithome.com/0/954/539.htm">发射任务准备进展顺利，神舟二十三乘组 航 天 员身心状态良好 - IT之家</a></li>
<li><a href="https://www.chinanews.com.cn/gn/2026/05-23/10627014.shtml">“ 天 宫”将迎来首位来自香 港 的 航 天 员 -中新网</a></li>

</ul>
</details>

**标签**: `#space exploration`, `#Shenzhou-23`, `#astronaut announcement`, `#China space program`

---

<a id="item-13"></a>
## [人工智能时代网络安全岗位激增](https://www.nytimes.com/2026/05/24/technology/one-job-that-is-growing-in-the-ai-era-cybersecurity-experts.html) ⭐️ 7.0/10

据《纽约时报》报道，人工智能时代对网络安全专家的需求激增，2026 年第一季度相关岗位招聘量同比增长 11%，高管职位需求较去年秋季增加了五到七倍。 这一趋势凸显了人工智能驱动的代码膨胀和新型安全威胁（如 Anthropic 的 Mythos 模型带来的威胁）正迫使企业紧急招聘网络安全人才，重塑就业市场和薪酬结构。 高级安全岗位薪酬包可达七八百万美元，安全工程师也需要补充 AI 技能才能保持竞争力。部分猎头公司甚至因合格候选人不足而拒绝接单。

telegram · zaihuapd · May 25, 06:21

**背景**: 像 Anthropic 于 2026 年 4 月发布的 Mythos 这样的前沿 AI 模型已展现出发现和利用软件漏洞的能力，加剧了网络安全风险。同时，AI 生成的代码扩大了攻击面，使得既懂安全技术又能驾驭 AI 复杂性的专家变得极为紧缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms ...</a></li>
<li><a href="https://www-cdn.anthropic.com/8b8380204f74670be75e81c820ca8dda846ab289.pdf">Claude Mythos Preview System Card - www-cdn.anthropic.com</a></li>

</ul>
</details>

**标签**: `#cybersecurity`, `#AI`, `#job market`, `#hiring trends`

---

<a id="item-14"></a>
## [马斯克宣布 Grok V9-Medium 训练完成](https://x.com/elonmusk/status/2058787384364265734) ⭐️ 7.0/10

埃隆·马斯克宣布，拥有 1.5 万亿参数的 Grok V9-Medium 基础模型已完成训练，评估结果良好，团队正在进行微调并准备强化学习，预计 2-3 周后向公众发布。 此次发布的参数量是当前 0.5T v8-small 模型的三倍，显著提升了编程能力，特别是在复杂编码任务方面，可能增强 xAI 在 AI 编程助手市场的竞争力。 该模型在补充训练中加入了大量 Cursor 数据，相比当前线上版本，在处理复杂编程任务时预计将有明显提升。

telegram · zaihuapd · May 25, 07:07

**背景**: Grok 是埃隆·马斯克的 AI 公司 xAI 开发的大型语言模型。当前生产模型 Grok v8-small 拥有 0.5 万亿参数。基于人类反馈的强化学习（RLHF）是一种常用技术，用于使模型输出与人类偏好对齐，通常在初始训练后应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://beyondtmrw.org/article/grok-v9-medium-training-complete-xai-15t-parameter-leap-coding-ai">Grok V 9 - Medium 1.5T Training Complete: xAI's Coding AI Leap</a></li>
<li><a href="https://www.kucoin.com/news/flash/musk-announces-grok-v9-medium-1-5t-model-to-launch-in-2-3-weeks">Musk announces the launch of the Grok V 9 - Medium (1.5T) model in...</a></li>
<li><a href="https://www.capitalbay.news/grok-v9-training-end-cursor-use-raise-concerns/">Elon Musk Teases Grok V 9 Launch Amid Data Concerns</a></li>

</ul>
</details>

**标签**: `#AI`, `#Grok`, `#Elon Musk`, `#machine learning`, `#model release`

---

<a id="item-15"></a>
## [欧盟初步认定谷歌可能违反《数字市场法》](https://t.me/zaihuapd/41566) ⭐️ 7.0/10

欧盟委员会发布初步调查结果，认为 Alphabet（谷歌）可能违反了《数字市场法》（DMA），具体表现为在搜索结果中自我偏好其自有服务，并限制 Play 商店开发者引导用户使用其他购买渠道。 这是 DMA 首次针对守门人采取的重大执法行动，可能为自我偏好和反引导规则的适用树立先例，并可能迫使谷歌在欧盟范围内大幅改变其搜索和应用商店做法。 调查重点在于谷歌搜索涉嫌偏袒其自有购物、航班和酒店服务，以及 Play 商店规则阻止开发者告知用户应用外更便宜的替代方案。尽管谷歌此前已采取合规措施，但委员会认为这些措施仍不足。

telegram · zaihuapd · May 26, 00:27

**背景**: 《数字市场法》（DMA）是欧盟的一项法规，将大型在线平台指定为“守门人”，并施加义务以确保公平竞争。其中一项关键义务是不得自我偏好，即不得将守门人自身产品或服务的排名置于第三方之上。另一项是允许应用开发者引导用户使用守门人平台之外的优惠。谷歌于 2023 年被指定为其搜索引擎和应用商店的守门人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Digital_Markets_Act">Digital Markets Act - Wikipedia</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://illinoislawreview.org/online/antitrust-self-preferencing-and-display-of-search-results/">Antitrust, Self-Preferencing, and Display of Search Results</a></li>

</ul>
</details>

**标签**: `#regulation`, `#Google`, `#DMA`, `#antitrust`, `#search`

---