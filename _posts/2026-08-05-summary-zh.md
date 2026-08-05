---
layout: default
title: "Horizon Summary: 2026-08-05 (ZH)"
date: 2026-08-05
lang: zh
---

> From 38 items, 21 important content pieces were selected

---

1. [Keyv 及相关 npm 包在活跃的 Shai-Hulud 供应链攻击中被入侵](#item-1) ⭐️ 9.0/10
2. [Mistral 推出 Shieldstral：3B 开源多模态审核模型](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash 在单个 AMD MI300X 上运行，速度超 150 tok/s](#item-3) ⭐️ 8.0/10
4. [Oxide Computer 完成 4.45 亿美元 D 轮融资](#item-4) ⭐️ 8.0/10
5. [MiniMax-H3 通过 MLX 移植在苹果芯片上运行](#item-5) ⭐️ 8.0/10
6. [华为提出韬定律，欲取代摩尔定律](#item-6) ⭐️ 8.0/10
7. [Cloudflare 弃用第三方安全工具，用每月 58 美元的 AI 处理漏洞赏金](#item-7) ⭐️ 8.0/10
8. [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](#item-8) ⭐️ 8.0/10
9. [我国首部 L3/L4 自动驾驶强制性国标报批](#item-9) ⭐️ 8.0/10
10. [新色彩空间简化多样化肤色的生成](#item-10) ⭐️ 7.0/10
11. [斯蒂芬·沃尔夫拉姆对亡妻伊莉斯·考利的深情悼念](#item-11) ⭐️ 7.0/10
12. [Waymo 在达拉斯向所有人开放无人驾驶打车服务](#item-12) ⭐️ 7.0/10
13. [联邦快递的合法邮件加剧钓鱼混淆](#item-13) ⭐️ 7.0/10
14. [LLM 0.32 新增推理轨迹、服务端工具与智能日志](#item-14) ⭐️ 7.0/10
15. [不要做“肉代理”：阅读、理解并验证 AI 输出](#item-15) ⭐️ 7.0/10
16. [LLM 让开源代码修改变得切实可行](#item-16) ⭐️ 7.0/10
17. [苹果批准微软请求，欧盟用户将可在 iPhone 与 Windows 间共享剪贴板](#item-17) ⭐️ 7.0/10
18. [俄罗斯要求苹果设备自 2025 年 9 月起支持第三方应用商店](#item-18) ⭐️ 7.0/10
19. [美国 FCC 禁止进口新款中国机器人和逆变器](#item-19) ⭐️ 7.0/10
20. [3D 打印仿生海绵体在猪模型中恢复勃起功能](#item-20) ⭐️ 7.0/10
21. [英伟达 CEO：美国应使用优秀的中国开源 AI 模型](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Keyv 及相关 npm 包在活跃的 Shai-Hulud 供应链攻击中被入侵](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

一场活跃的 npm 供应链攻击已入侵流行的 Keyv 包及相关包，自复制蠕虫“Shai-Hulud”已污染数百个包。攻击仍在进行中，并引发了社区关于缓解策略的紧急讨论。 此次攻击影响了 JavaScript 生态系统中广泛使用的包，可能危及许多项目的开发者和 CI 凭据。它凸显了 npm 依赖系统的脆弱性，并强调了加强供应链安全措施的必要性。 Shai-Hulud 蠕虫已入侵超过 500 个包，包括 79 个包名下的 353 个版本，并窃取凭据，同时保留仓库钩子。该攻击利用了预安装/后安装钩子，社区现在呼吁限制或移除这些钩子。

hackernews · cimi_ · Aug 4, 11:01 · [社区讨论](https://news.ycombinator.com/item?id=49166874)

**背景**: Keyv 是一个简单的 Node.js 键值存储库，支持多种后端，在 npm 生态系统中广泛使用。此类供应链攻击通过恶意安装脚本等方式入侵合法包以分发恶意软件，并可能在软件供应链中产生连锁效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code ...</a></li>
<li><a href="https://unit42.paloaltonetworks.com/npm-supply-chain-attack/">"Shai-Hulud" Worm Compromises npm Ecosystem in Supply Chain Attack (Updated November 26)</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>

</ul>
</details>

**社区讨论**: 社区成员对此次攻击表示担忧，有人呼吁暂停新增预安装/后安装钩子，也有人建议使用 devcontainers 进行隔离。还提到了 Packj 等工具用于检测供应链攻击，一些用户寻求实用方法来检查其 node_modules 是否被入侵。

**标签**: `#security`, `#supply-chain`, `#npm`, `#open-source`, `#malware`

---

<a id="item-2"></a>
## [Mistral 推出 Shieldstral：3B 开源多模态审核模型](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral AI 于 2026 年 8 月 4 日发布了 Shieldstral，这是一个 3B 参数的开源多模态安全分类器。它在推理时使用自然语言策略问题来评判文本和图像，性能优于其 7 倍大小的模型。 此次发布为内容审核提供了一种经济高效且灵活的解决方案，可能使较小的平台能够实施强大的安全措施。其基于提示的策略允许无需重新训练即可定制，这可能改变 AI 生态系统中审核的部署方式。 Shieldstral 支持提示审核、响应审核、提示-响应对分类、拒绝检测以及跨文本和图像输入的安全过滤。它根据自然语言策略问题返回是/否分类，并已在 Hugging Face 上提供。

hackernews · riadsila · Aug 4, 16:36 · [社区讨论](https://news.ycombinator.com/item?id=49171268)

**背景**: 内容审核对于 AI 应用防止有害输出至关重要。传统的审核模型依赖固定的危害类别，而 Shieldstral 的方法在推理时使用自然语言策略，提供了更大的灵活性。Mistral 还为开发者提供了审核 API 和自定义护栏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://docs.mistral.ai/models/model-cards/shieldstral-1-0">Shieldstral 1.0 - docs.mistral.ai</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral's Shieldstral Packs Policy-Adaptive Safety Screening Into 3B ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论对该模型的灵活性表现出兴趣，有人质疑它是否能处理超出典型大科技审核风格的任意规则集。一些用户对现实世界的边缘情况持怀疑态度，而另一些人则将其视为其项目中内容审核的实用解决方案。

**标签**: `#AI`, `#content moderation`, `#Mistral`, `#open-weights`, `#multimodal`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash 在单个 AMD MI300X 上运行，速度超 150 tok/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

一份新指南展示了在单个 AMD MI300X GPU 上运行 DeepSeek V4 Flash，在完整权重和 256k 上下文窗口下实现每秒超过 150 个 token 的速度。 这很重要，因为它表明大型 MoE 模型可以在单个高端 GPU 上高效运行，可能降低硬件成本，使先进 LLM 对研究人员和小型组织更易获取。 MI300X 拥有 192GB HBM3 内存，这对于容纳 284B 参数模型至关重要。指南指出一个权衡：上下文窗口从原始的 1M token 减少到 256k，尽管这对许多用例仍然实用。

hackernews · zhoutong · Aug 4, 10:00 · [社区讨论](https://news.ycombinator.com/item?id=49166386)

**背景**: DeepSeek V4 Flash 是一个混合专家（MoE）语言模型，总参数 284B，但每个 token 仅激活 13B，因此推理效率高。AMD MI300X 是一款数据中心 GPU，配备 192GB HBM3 内存，专为大型 AI 工作负载设计。在单个 GPU 上运行如此大的模型需要精细的内存管理和优化技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash · Hugging Face</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>
<li><a href="https://lenovopress.lenovo.com/lp1943-thinksystem-amd-mi300x-192gb-750w-8-gpu-board">ThinkSystem AMD MI300X 192GB 750W 8-GPU Board Product Guide > Lenovo Press</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 MI300X 通常以 8-GPU 板卡形式出售，而非单卡，并建议 MI350P 作为具有 144GB 内存的 PCIe 替代品。还有人提到了 DwarfStar 等先前工作，并对上下文窗口的权衡提出疑问，但大多数人认为 256k 上下文是实用的折中方案。

**标签**: `#DeepSeek`, `#AMD MI300X`, `#LLM inference`, `#quantization`, `#hardware`

---

<a id="item-4"></a>
## [Oxide Computer 完成 4.45 亿美元 D 轮融资](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

根据美国证券交易委员会（SEC）的 Form D 文件，Oxide Computer 已完成 4.45 亿美元的 D 轮融资。此前该公司已完成 A 轮 4400 万美元、B 轮 1 亿美元和 C 轮 2 亿美元的融资。 这一重大融资里程碑凸显了投资者对 Oxide 构建云规模硬件和软件愿景的信心。这可能加速公司的产品开发和市场采用，有望颠覆传统的服务器和云基础设施市场。 该融资通过 SEC 的 Form D 文件披露，表明这是一次私募配售。公司尚未公开宣布本轮融资，投资者和估值细节尚未披露。社区评论既表达了对产品可用性和销售响应速度的兴奋，也表达了怀疑。

hackernews · depr · Aug 4, 20:13 · [社区讨论](https://news.ycombinator.com/item?id=49174407)

**背景**: Oxide Computer 是一家专注于构建本地云基础设施的硬件初创公司，提供集计算、存储和网络于一体的机架级系统。该公司由 Bryan Cantrill 和 Adam Leventhal 共同创立，他们曾在 Sun Microsystems 和 Joyent 工作。其产品旨在提供比传统云提供商更易于管理和更具成本效益的替代方案。

**社区讨论**: 社区情绪复杂：一些人对公司的进展和产品概念表示兴奋，而另一些人则质疑 Oxide 是否真的出货硬件，并指出销售响应不佳。一位评论者提到填写了销售表格但从未收到回复，尽管他们在 AWS 上花费巨大。总体而言，人们对团队表示钦佩，但对执行持怀疑态度。

**标签**: `#funding`, `#hardware`, `#startup`, `#Oxide Computer`

---

<a id="item-5"></a>
## [MiniMax-H3 通过 MLX 移植在苹果芯片上运行](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

Simon Willison 演示了通过 MLX 移植版 PipeNetwork/minimax-h3-mlx 在苹果芯片上运行 MiniMax 的新型全模态模型 MiniMax-H3。他在自己的 M5 Max MacBook Pro 上成功根据文本提示生成了带音频的 15 秒视频片段。 这使得开发者能够在苹果芯片上本地运行最先进的全模态生成模型，减少对云端 API 的依赖，并支持离线实验。这凸显了 MLX 移植生态系统的不断壮大，使先进 AI 模型对苹果开发者社区更加可及。 该模型需要下载约 115 GB 的模型文件，在 M5 Max 上生成视频耗时不到 45 分钟。由于未提供音频提示指导，生成的音频被描述为“奇怪的类似语音的垃圾”，但提示指南提供了获得更好结果的技巧。

rss · Simon Willison · Aug 4, 19:10

**背景**: MiniMax-H3 是一个通用的全模态生成系统，可接受文本、图像、音频和视频输入，并能生成最长 15 秒、最高 2K 分辨率、带原生立体声的视频片段。MLX 是 Apple 推出的数组框架，专为在苹果芯片上进行高效机器学习而设计，此移植版利用它来在本地运行模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and ...</a></li>
<li><a href="https://kylon.io/blog/minimax-h3-guide-2026">MiniMax H3 Guide: Open-Weight Multimodal Video, API, and License</a></li>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>

</ul>
</details>

**标签**: `#MLX`, `#MiniMax-H3`, `#omni-modal`, `#Apple Silicon`, `#video generation`

---

<a id="item-6"></a>
## [华为提出韬定律，欲取代摩尔定律](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

在 2026 年于上海举行的 IEEE 国际电路与系统研讨会（ISCAS）上，华为海思总裁何庭波发布了“韬（τ）定律”，提出以时间缩微替代几何缩微作为半导体演进的新原则。华为声称过去六年已据此设计并量产 381 款芯片，今年秋季将推出采用逻辑折叠技术的新麒麟手机芯片。 这一发布意义重大，因为它提出了一种后摩尔范式，可能将半导体进步延伸到物理极限之外，从而重塑行业格局。同时，这也标志着华为战略性地绕开 EUV 限制，力争在 2031 年前实现等效 1.4 纳米制程的晶体管密度，可能改变芯片领域的竞争态势。 韬定律的核心是通过降低时间常数（τ）实现器件、电路、芯片到系统的多层级协同优化。华为预计，到 2031 年，基于该定律的芯片晶体管密度将达到等效 1.4 纳米制程水平，并声称比传统缩微方式密度提高 55%。逻辑折叠架构将晶体管级逻辑折叠成垂直层，需要新的设计工具，例如北京大学开发的 3D 芯片设计工具。

telegram · zaihuapd · Aug 4, 08:04

**背景**: 摩尔定律预测晶体管密度大约每两年翻一番，但由于几何缩微面临挑战，正接近物理极限。时间缩微通过优化时间常数而非物理尺寸，提供了一种替代方案。华为的提议是探索后摩尔计算范式的更广泛趋势的一部分，并借助中国在出口管制下推动半导体自给自足的努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/huawei-claims-sanctions-busting-breakthrough-with-1-4nm-class-chips-by-2031-claims-55-percent-higher-transistor-density-firm-claims-new-logicfolding-chip-architecture-can-bypass-euv-restrictions-introduces-tau-scaling-law-to-replace-moores-law">Huawei claims sanctions-busting breakthrough with 1.4nm-class chips by 2031, claims 55% higher transistor density — firm claims new LogicFolding chip architecture can bypass EUV restrictions, introduces 'Tau Scaling Law' to replace Moore's Law | Tom's Hardware</a></li>
<li><a href="https://qz.com/huawei-logicfolding-chip-design-tau-scaling-052626">Huawei LogicFolding chip design aims to match 1.4nm by 2031</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#Huawei`, `#Moore's Law`, `#chip design`, `#technology`

---

<a id="item-7"></a>
## [Cloudflare 弃用第三方安全工具，用每月 58 美元的 AI 处理漏洞赏金](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare 首席安全官 Grant Bourzikas 在悉尼的一次会议上透露，公司已使用 Anthropic 的 Claude Sonnet 模型自动化处理漏洞赏金报告，每月仅花费 58 美元，而如果使用安全专用模型 Mythos，同样的工作每月约需 20 万美元。Cloudflare 还构建了 200 多个自主安全代理，几乎用自研应用（部分由 AI 辅助编写）取代了所有第三方安全工具。 这展示了通过 AI 自动化在安全运营中实现显著的成本降低和效率提升，可能重塑企业处理安全工具的方式。同时，这也凸显了 AI 在安全领域日益重要的作用，但 Cloudflare 的谨慎建议表明，这种策略可能并不普遍适用。 成本对比鲜明：Claude Sonnet 每月 58 美元，而安全专用模型 Mythos 每月 20 万美元。Cloudflare 的首席安全官建议其他公司不要效仿，指出并非每家银行都该自己开发所有软件。此外，首席战略官将公司裁员 1100 人归因于 AI 驱动的自动化，并提到计划充当 AI 公司与出版商之间的中介，通过微支付实现内容付费。

telegram · zaihuapd · Aug 4, 09:24

**背景**: Cloudflare 是一家主要的网络基础设施和安全公司。漏洞赏金计划奖励安全研究人员发现并报告漏洞。像 Claude Sonnet 这样的 AI 模型可用于对这些报告进行分流，通过去重和评估其价值。Mythos 是 Anthropic 的高级 AI 模型，具有强大的安全能力，但运行成本要高得多。Cloudflare 的举措反映了利用 AI 自动化安全运营的更广泛趋势，但其规模和工程专业知识并不典型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600">Cloudflare has mostly ditched third party security tools, suggests not trying that at home</a></li>
<li><a href="https://www.contrastsecurity.com/glossary/mythos-ai">What Is Mythos AI? Autonomous Exploits and AppSec Defense | Contrast Security</a></li>
<li><a href="https://www.endorlabs.com/learn/what-is-mythos-and-why-it-matters-for-software-security">What Is Mythos and Why It Matters for Software Security | Blog | Endor Labs</a></li>

</ul>
</details>

**标签**: `#AI`, `#security`, `#Cloudflare`, `#automation`, `#vulnerability management`

---

<a id="item-8"></a>
## [谷歌为 Anthropic 搭建 2000 亿美元华尔街融资机器](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

谷歌悄然搭建了一个约 2000 亿美元的庞大融资架构，向 Anthropic 交付超过 1500 亿美元的 AI 芯片。该架构涉及博通、阿波罗、黑石和摩根士丹利等合作伙伴，采用厂商融资模式来分散风险。 这是历史上最大的基础设施融资交易之一，使 Anthropic 在缺乏信用评级的情况下仍能扩展其 AI 算力。它为 AI 公司如何在不将巨额硬件资产压在自身资产负债表上的情况下获取大规模算力开创了先例。 今年 6 月，特殊目的载体 Compute SPV 完成了首批交易，购入约 350 亿美元硬件，约合 1 吉瓦算力和 100 万颗 TPU。该模式借鉴了波音和 GE 推销飞机和发动机的厂商融资玩法，谷歌担保数据中心，博通购买并协助融资芯片，阿波罗和黑石购买硬件后回租给 Anthropic。

telegram · zaihuapd · Aug 4, 10:52

**背景**: 厂商融资是一种卖方为买方提供贷款的信贷安排，常用于促进大额采购。在此案例中，谷歌及其合作伙伴采用类似模式，将建设 AI 基础设施的财务风险分散到多个参与方，避免任何单一公司将全部成本压在资产负债表上。TPU（张量处理单元）是谷歌自研的 AI 芯片，专为加速机器学习工作负载而设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nucleuscommercialfinance.com/finance-glossary/vendor-finance/">Vendor Finance | What is Vendor Finance for Business?</a></li>
<li><a href="https://aiwiki.ai/wiki/tpu_chip">TPU Chip | AI Wiki</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#finance`, `#chips`

---

<a id="item-9"></a>
## [我国首部 L3/L4 自动驾驶强制性国标报批](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

工信部已完成《智能网联汽车自动驾驶系统安全要求》强制性国家标准报批稿，并于 6 月 17 日起公示，建议 2027 年 7 月 1 日实施。这是我国首部针对 L3 和 L4 级自动驾驶的强制性标准。 该标准标志着监管从“概念松绑”转向“安全硬约束”，要求车企通过 Safety Case 机制系统性论证安全性。这将对中国自动驾驶行业产生重大影响，影响车辆设计、营销和合规策略。 该标准适用于搭载 L3 或 L4 级系统的 M 类和 N 类车辆，不适用于自动泊车系统。对于 L3 级，要求具备驾驶人接管能力监测功能；对于 L4 级，包含自主风险处置的具体要求，并考虑乘客站立等情况。

telegram · zaihuapd · Aug 4, 13:06

**背景**: 自动驾驶等级从 L0 到 L5，L3 为有条件自动驾驶，驾驶员需随时准备接管；L4 为高度自动驾驶，系统可在多数情况下无需驾驶员干预。中国一直在制定智能网联汽车相关法规，该标准是建立更高级别自动化强制性安全要求的关键一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://chedongxi.com/p/370544.html">车企营销不能再“乱吹”了！ 自 动 驾 驶 国标出台，明年7月实施 - 车东西</a></li>
<li><a href="https://www.ithome.com/0/985/665.htm">ithome.com/0/985/665.htm</a></li>

</ul>
</details>

**标签**: `#autonomous driving`, `#regulation`, `#China`, `#safety standard`, `#L3/L4`

---

<a id="item-10"></a>
## [新色彩空间简化多样化肤色的生成](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

作者介绍了一种自定义色彩空间和算法，用于生成多样化且逼真的肤色，并提供了交互式演示和详细说明。该项目包含一个 JavaScript 颜色选择器和一个 Python 程序化生成算法。 这解决了数字艺术和游戏开发中的一个实际难题，即选择逼真的肤色往往很困难。该方法可以简化工作流程，并激发更多面向人类应用的色彩科学研究。 该色彩空间是通过对数据拟合函数构建的，而非使用 PCA，作者承认方法学“不太可靠”且有改进空间。页面包含“未来工作”部分和各种 JavaScript 演示。

hackernews · automatoney · Aug 4, 15:16 · [社区讨论](https://news.ycombinator.com/item?id=49170165)

**背景**: 由于人类感知和光照的影响，数字媒体中的肤色表示非常复杂。传统的色彩空间如 RGB 或 HSV 对肤色并不直观，而现有的方法如 Pantone 肤色色卡并未被引用。该项目旨在为此目的创建一个专用空间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>

</ul>
</details>

**社区讨论**: 评论称赞了该工作的优雅性和函数拟合方法，同时指出肤色建模的复杂性。有人建议参考 Pantone 肤色色卡，并提到肤色在 Oklab 色彩空间中形成月牙形，这与文章一致。一位评论者观察到生成的颜色中带有绿色、蓝色和紫色，质疑其合理性。

**标签**: `#color science`, `#procedural generation`, `#digital art`, `#skin tone`, `#algorithm`

---

<a id="item-11"></a>
## [斯蒂芬·沃尔夫拉姆对亡妻伊莉斯·考利的深情悼念](https://writings.stephenwolfram.com/2026/08/in-memory-of-my-wife-elise-cawley-1961-2026-with-thanks-for-36-wonderful-years/) ⭐️ 7.0/10

斯蒂芬·沃尔夫拉姆发表了一篇深情的个人悼文，纪念他去世的妻子伊莉斯·考利（1961–2026），回顾了他们共同度过的 36 年，并对彼此相伴的人生表达了感激之情。 这篇悼文让科技界得以罕见地窥见一位知名人物的私人生活，促进了共情与联结。它凸显了创新背后的人性一面，并与许多经历过失去的人产生共鸣。 这篇悼文以其惊人的细节著称，暗示沃尔夫拉姆可能记有日记或拥有非凡的记忆力。社区评论称赞其真诚与情感深度，超越了他平时的写作风格。

hackernews · jdcampolargo · Aug 4, 18:51 · [社区讨论](https://news.ycombinator.com/item?id=49173165)

**背景**: 斯蒂芬·沃尔夫拉姆是著名的计算机科学家、物理学家，也是 Mathematica 和 Wolfram Alpha 的创造者。伊莉斯·考利是他的妻子，两人相伴 36 年，她的离世促使他写下这篇个人反思，并引发了社区的广泛关注。

**社区讨论**: 社区评论表达了深切的同情和敬佩，许多人指出这篇悼文的情感力量和真诚。一些人分享了个人失去亲人的经历，另一些人则强调这篇文章超越了沃尔夫拉姆平时的写作风格。

**标签**: `#tribute`, `#Stephen Wolfram`, `#personal`, `#community`, `#obituary`

---

<a id="item-12"></a>
## [Waymo 在达拉斯向所有人开放无人驾驶打车服务](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo 已正式在德克萨斯州达拉斯向公众开放其无人驾驶打车服务，标志着这家自动驾驶汽车公司又一次重大城市扩张。该服务现已在达拉斯地区向所有用户开放，此前已在其他城市推出。 此次扩张意义重大，因为它将自动驾驶打车服务带到了美国最大、最依赖汽车的大都市区之一，可能重塑城市出行方式，减少对私家车的依赖。这也表明 Waymo 在自动驾驶汽车行业持续扩大规模并保持竞争优势。 达拉斯以低密度、高扩张和有限的公共交通而闻名，这对自动驾驶汽车来说是一个具有挑战性的环境。该服务可能面临极端天气条件（如高温和突然的天气变化）的考验，这可能影响车辆的耐用性和传感器可靠性。

hackernews · xnx · Aug 4, 18:29 · [社区讨论](https://news.ycombinator.com/item?id=49172836)

**背景**: Waymo 是 Alphabet Inc.的子公司，运营着全球首个自动驾驶打车服务，已提供超过 2000 万次出行，满意度达 93%。该公司一直在向多个城市扩张，包括旧金山、凤凰城和洛杉矶，并计划于 2026 年在伦敦推出服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride - Hail</a></li>
<li><a href="https://manufacturingcurated.com/automotive-and-aerospace/waymos-driverless-robotaxis-dallas-expansion-by-2026/">Waymo's Driverless Robotaxis: Dallas Expansion by 2026?</a></li>
<li><a href="https://www.roadtoautonomy.com/waymo-drives-autonomously-dallas/">Waymo Drives Autonomously into Dallas | The Road to Autonomy</a></li>

</ul>
</details>

**社区讨论**: 社区评论展现了多元观点：一些人认为无人驾驶汽车通过降低交通成本，是一种有效的经济适用房政策；另一些人则担心对当地经济的影响，例如资金流出本地经济。许多用户报告了使用 Waymo 的积极体验，指出其与人类驾驶员相比更安全、更可预测，但也有人提到偶尔发生车辆卡住的情况。

**标签**: `#autonomous vehicles`, `#Waymo`, `#transportation`, `#urban planning`, `#AI`

---

<a id="item-13"></a>
## [联邦快递的合法邮件加剧钓鱼混淆](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

Troy Hunt 的文章指出，联邦快递的合法邮件做法（如发送带有附件的未经请求的海关通知）使用户更难区分真实通信与钓鱼诈骗。文章通过真实案例说明了电子邮件安全面临的持续挑战。 这很重要，因为它表明即使是信誉良好的公司也会无意中让用户接受危险的邮件行为，从而增加整体对钓鱼攻击的脆弱性。这凸显了改进邮件认证标准和用户教育以对抗社会工程攻击的必要性。 文章提到联邦快递通过普通电子邮件发送带有 PDF 附件的海关通知，这与常见的钓鱼手法相似。社区评论还提到其他组织（如 IRS）的类似问题，以及 .xyz 等新通用顶级域名的泛滥使域名信任变得更加复杂。

hackernews · stymaar · Aug 4, 21:09 · [社区讨论](https://news.ycombinator.com/item?id=49175192)

**背景**: 钓鱼是一种社会工程攻击，攻击者冒充合法实体诱骗受害者泄露敏感信息或点击恶意链接。电子邮件仍然是主要攻击途径，超过 70% 的数据泄露始于钓鱼或社会工程攻击。像联邦快递这样的公司经常发送格式不佳的合法邮件，攻击者模仿这些邮件，使用户难以分辨真假。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.mailguard.com.au/blog/dont-fall-for-this-fraudulent-fedex-phishing-email">Don’t fall for this fraudulent FedEx phishing email</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6334892/">Email fraud: The search for psychological predictors of susceptibility ...</a></li>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-social-engineering">What is Social Engineering ? - Meaning</a></li>

</ul>
</details>

**社区讨论**: 社区评论分享了个人在联邦快递和其他组织的经历，强调合法邮件看起来像钓鱼邮件所造成的困惑。一些用户指出验证 c.gle 等域名的困难，另一些用户则指出新通用顶级域名加剧了问题。总体情绪是对当前电子邮件安全实践的不满。

**标签**: `#phishing`, `#security`, `#email`, `#FedEx`, `#social engineering`

---

<a id="item-14"></a>
## [LLM 0.32 新增推理轨迹、服务端工具与智能日志](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 7.0/10

LLM 0.32 于 2026 年 8 月 4 日发布，为推理模型引入了可见的推理轨迹，支持来自 OpenAI 和 Anthropic 等服务端的工具，重新设计了内容可寻址的 SQLite 日志，并支持 GPT-5.6 模型系列，默认模型改为 GPT-5.6 Luna。此外，新增了 'llm openai endpoint' 命令，可对任何兼容 OpenAI 的端点执行一次性提示。 此次更新显著增强了 LLM CLI 工具，通过支持推理轨迹和服务端工具，与当前 AI 趋势保持一致，这对于构建智能体应用至关重要。它改善了依赖 LLM 与各种模型交互的开发者和高级用户的体验，可能提高采用率和生产力。 推理轨迹默认显示到标准错误输出，可通过 -R/--hide-reasoning 标志禁用。服务端工具包括 OpenAI 的 CodeInterpreter 和 WebSearch，以及 Anthropic 的 WebSearch、WebFetch、CodeExecution 和 AnthropicMCP，可通过命令行标志使用。内容可寻址的 SQLite 日志经过重新设计，以提高存储和检索效率。

rss · Simon Willison · Aug 4, 23:58

**背景**: LLM 是 Simon Willison 开发的命令行工具，用于与大型语言模型交互。它支持多种提供商和插件，允许用户运行提示并集成工具。OpenAI Responses API 于 2025 年 3 月发布，通过结合聊天补全和高级工具调用功能，简化了智能体应用的开发。内容可寻址存储（CAS）是一种基于内容而非位置检索数据的方法，可以提高效率和去重能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://llm.datasette.io/en/stable/usage.html">Usage - LLM</a></li>
<li><a href="https://simonwillison.net/2025/May/27/llm-tools/">Large Language Models can run tools in your terminal with LLM 0.26</a></li>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>

</ul>
</details>

**标签**: `#LLM`, `#CLI`, `#AI`, `#OpenAI`, `#release`

---

<a id="item-15"></a>
## [不要做“肉代理”：阅读、理解并验证 AI 输出](https://simonwillison.net/2026/Aug/3/dont-be-a-meat-proxy/#atom-everything) ⭐️ 7.0/10

Niklas Gruhn 创造了“肉代理”一词，用来形容那些盲目转发 AI 输出而不加理解的人。他敦促用户阅读、理解、验证 AI 回复，并用自己语言重写。 该术语揭示了一种常见的 AI 误用，削弱了专业价值和信任。它鼓励更审慎地整合 AI，促进沟通中的责任感和质量。 该术语由 Niklas Gruhn 在 2026 年 8 月 3 日的博客文章中提出，并由 Simon Willison 重点推荐。建议强调，投入个人努力是完成必要验证步骤的“证明”。

rss · Simon Willison · Aug 3, 23:45

**背景**: 大型语言模型（LLM）生成的文本可能流畅，但可能包含错误或偏见。不加验证地复制 AI 输出可能传播错误信息，降低人类专业知识的价值。“肉代理”一词类比于仅转发数据而不处理的代理服务器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/3/dont-be-a-meat-proxy/">Don't be a meat proxy | Simon Willison’s Weblog</a></li>
<li><a href="https://www.remio.ai/post/simon-willison-says-dont-be-a-meat-proxy-for-ai">Simon Willison Says Don't Be a Meat Proxy for AI</a></li>
<li><a href="https://techplanet.today/post/the-meat-proxy-problem-why-blindly-forwarding-ai-output-undermines-professional-value">The Meat Proxy Problem: Why Blindly Forwarding AI ... | TechPlanet</a></li>

</ul>
</details>

**社区讨论**: Lobste.rs 上的讨论验证了这一概念，有人指出该术语可能被滥用来羞辱初级员工或非母语者。其他人强调应将其用于诊断工作流程，而非指责个人。

**标签**: `#AI`, `#LLMs`, `#AI ethics`, `#productivity`, `#definitions`

---

<a id="item-16"></a>
## [LLM 让开源代码修改变得切实可行](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 7.0/10

西蒙·威利森认为，LLM 降低了检查和修改开源代码的摩擦，使开源理想更加切实可行。他描述了使用 Claude 和 Codex 以最少的时间投入来克隆、构建和理解项目。 这一转变可能使代码贡献和定制民主化，让更多开发者能够参与开源项目。它可能加速创新并扩大软件开发的参与度。 威利森指出，以前让软件编译是一个主要障碍，但现在他将其视为零时间投入，委托给 AI 工具。他承认自己尚未习惯性地修改软件，但看到了明确的前进道路。

rss · Simon Willison · Aug 3, 15:30

**背景**: 开源软件赋予用户检查和修改代码的自由，但实践中，理解和构建项目所需的时间限制了只有少数专家能做到。LLM 可以协助导航代码库、解释功能并自动化构建过程，从而降低入门门槛。

**社区讨论**: Hacker News 的讨论可能包括对 LLM 在开源参与中实际益处的认同，一些用户分享了自己的经验，另一些则表达了对过度依赖 AI 的担忧。总体情绪似乎是积极的，认识到增加参与度的潜力。

**标签**: `#open source`, `#LLMs`, `#developer tools`, `#workflow`

---

<a id="item-17"></a>
## [苹果批准微软请求，欧盟用户将可在 iPhone 与 Windows 间共享剪贴板](https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu) ⭐️ 7.0/10

苹果已批准微软的互操作性请求，将开发 iPhone 与 Windows PC 之间的跨设备剪贴板共享功能，预计 2027 年秋季随 iOS 28 面向欧盟用户推出。届时用户无需第三方应用，即可在一台设备上复制、在另一台设备上粘贴。 这标志着在欧盟《数字市场法案》（DMA）推动下，跨平台互操作性迈出重要一步，可能改善用户工作流程并减少对第三方解决方案的依赖。这也可能为其他大型科技生态系统之间的互操作性请求开创先例。 微软于 2026 年 3 月 25 日提交请求，6 月 26 日获批。苹果的实现将使用 AccessorySetupKit 框架进行一次性配对授权，类似于 iOS 26.5 中的配件通知框架。该功能最初仅面向欧盟，但苹果未排除未来推广至全球的可能性。

telegram · zaihuapd · Aug 4, 03:15

**背景**: 欧盟《数字市场法案》（DMA）要求指定的“守门人”（如苹果）允许第三方访问与其自身服务相同的操作系统硬件和软件功能。DMA 第 6(7)条特别要求此类功能的互操作性。AccessorySetupKit 是苹果在 WWDC24 上推出的框架，为应用提供了一种简化且注重隐私的方式来设置和管理蓝牙及 Wi-Fi 配件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/developer-portal/interoperability_en">Interoperability - Digital Markets Act (DMA) - European Commission</a></li>
<li><a href="https://developer-mdn.apple.com/videos/play/wwdc2024/10203/">Meet AccessorySetupKit - WWDC24 - Videos - Apple Developer</a></li>
<li><a href="https://www.macworld.com/article/3205820/apple-is-finally-making-copy-paste-work-between-iphones-and-pcs.html">The feature is currently scheduled as part of iOS 28 in the EU.</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Microsoft`, `#iOS`, `#Interoperability`, `#DMA`

---

<a id="item-18"></a>
## [俄罗斯要求苹果设备自 2025 年 9 月起支持第三方应用商店](https://t.me/zaihuapd/42963) ⭐️ 7.0/10

俄罗斯国家杜马通过新法案，要求自 2025 年 9 月 1 日起，包括 iPhone 和 iPad 在内的苹果设备必须允许用户安装 RuStore 等第三方应用商店。该法律禁止苹果和谷歌设置安装限制或障碍。 该法规挑战了苹果和谷歌对应用分发的控制，可能为其他国家强制要求第三方应用商店开创先例。这可能对应用商店垄断产生重大影响，并迫使平台持有者在俄罗斯改变其商业模式。 该法律还禁止制造商限制第三方软件的安装和更新、封锁替代软件功能、强制开发者定价或限制支付方式。RuStore 是由 VK 在俄罗斯数字发展部支持下创建的俄罗斯应用商店，自 2023 年起预装在安卓设备上。

telegram · zaihuapd · Aug 4, 05:25

**背景**: 自 2019 年俄罗斯通过法律要求设备制造商提供国内应用以来，俄罗斯一直在推动在售设备上安装国内应用。苹果与俄罗斯当局一直处于缓慢升级的争端中，俄罗斯因苹果未能预装 RuStore 和 MAX messenger 等国家支持的应用而对苹果提起反垄断诉讼。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/03/russia-escalates-dispute-with-apple-over-mandatory-app-preinstallation/">Russia escalates dispute with Apple over mandatory app ... - 9to5Mac</a></li>
<li><a href="https://www.msn.com/en-us/news/other/russia-wants-its-apps-on-your-iphone-and-now-it-s-hauling-apple-into-court/ar-AA29nHlM">Russia wants its apps on your iPhone — and now it’s hauling Apple ...</a></li>
<li><a href="https://www.rustore.ru/en">RuStore is the official app store for Android and Harmony OS</a></li>

</ul>
</details>

**标签**: `#regulation`, `#app store`, `#Apple`, `#Russia`, `#policy`

---

<a id="item-19"></a>
## [美国 FCC 禁止进口新款中国机器人和逆变器](https://t.me/zaihuapd/42970) ⭐️ 7.0/10

7 月 28 日，美国联邦通信委员会（FCC）公布措施，禁止进口来自中国的新款人形机器人、四足机器人和联网电力逆变器，该措施自发布起立即生效，适用于尚未推出的型号。 此举标志着美中科技脱钩进一步升级，直接影响机器人及 AI 基础设施供应链。这可能迫使企业寻找替代供应商，并为更广泛限制中国科技产品开创先例。 该禁令仅适用于尚未上市的型号，且 FCC 预计将豁免许多非中国供应商。但该机构仍有权撤销已获准在美国销售型号的授权。

telegram · zaihuapd · Aug 4, 11:29

**背景**: FCC 是美国独立的通信和技术监管机构。逆变器将直流电转换为交流电，常用于太阳能和电池系统；联网逆变器可接入网络，存在潜在网络安全风险。人形机器人和四足机器人是先进机器人产品，常用于工业和研究领域。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kizpow.com/xingyezixun/2568.html">kizpow.com/xingyezixun/2568.html</a></li>
<li><a href="https://ouluwind.com/baike/569.html">ouluwind.com/baike/569.html</a></li>

</ul>
</details>

**标签**: `#US-China`, `#robotics`, `#regulation`, `#AI`, `#supply chain`

---

<a id="item-20"></a>
## [3D 打印仿生海绵体在猪模型中恢复勃起功能](https://doi.org/10.1016/j.biomaterials.2026.124491) ⭐️ 7.0/10

一项发表在《Biomaterials》上的研究利用 3D 打印技术制造了具有正弦腔隙结构的水凝胶仿生海绵体，并植入脐带来源的间充质干细胞，在猪模型中成功恢复了勃起功能。 这代表了勃起功能障碍（ED）再生医学领域的重大进展，为从根本上修复受损组织提供了可能，有望替代仅缓解症状的传统疗法。若成功转化到人类，可能惠及全球数百万 ED 患者，尤其是严重阴茎损伤者。 该研究利用单细胞测序揭示了机制：干细胞促进内皮细胞分化以重建血管网络，减少 TGF-β分泌以抑制内皮-间质转化，并通过激活抗炎因子 IL-10 调节免疫环境。该仿生结构可在体外流体压力下模拟阴茎勃起过程。

telegram · zaihuapd · Aug 4, 13:52

**背景**: 勃起功能障碍（ED）是男性难以获得或维持勃起的常见疾病。传统治疗包括口服药物、注射或手术，但往往只能缓解症状，而非修复潜在的结构损伤。海绵体是阴茎中在勃起时充血的勃起组织。3D 生物打印是一种利用生物墨水逐层构建三维结构的技术，常与活细胞结合，用于制造组织样构造物以进行再生医学治疗。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/42546581/">Development and mechanistic investigation of 3 D - printed biomimetic ...</a></li>
<li><a href="https://www.livescience.com/health/scientists-invent-3d-printed-penis-implant-to-restore-erections-and-it-works-in-rabbits-and-pigs">Scientists invent 3 D - printed penis implant to restore... | Live Science</a></li>
<li><a href="https://www.dailymail.com/sciencetech/article-14472861/3D-printed-PENIS-used-cure-erectile-dysfunction.html">Scientists create the world's first 3 D - printed PENIS... | Daily Mail Online</a></li>

</ul>
</details>

**标签**: `#3D printing`, `#biomedical engineering`, `#stem cells`, `#erectile dysfunction`, `#regenerative medicine`

---

<a id="item-21"></a>
## [英伟达 CEO：美国应使用优秀的中国开源 AI 模型](https://t.me/zaihuapd/42977) ⭐️ 7.0/10

英伟达 CEO 黄仁勋在采访中表示，中国开源 AI 模型“非常优秀”，美国企业“绝对”应该获准使用。他还反对以国家安全为由全面限制开源模型。 黄仁勋的言论在 AI 行业具有重要影响力，可能影响美国关于开源 AI 和中美科技竞争的政策讨论。他的立场可能鼓励更开放的合作，并影响 AI 芯片和硬件的市场动态。 黄仁勋认为中国公司将美国公司挤出市场的可能性为零，更便宜甚至免费的 AI 会扩大用户规模，增加对芯片、硬件和数据中心的需求。他建议通过安全沙箱控制下载的中国模型，并针对具体的隐私或合同违规行为处理知识产权争议，而非全面限制。

telegram · zaihuapd · Aug 4, 15:22

**背景**: 开源 AI 模型，如中国的 DeepSeek，因其性能和可访问性而受到全球关注。安全沙箱是一种隔离环境，允许程序在不影响宿主系统的情况下运行，可用于安全测试和控制 AI 模型。关于开源 AI 与国家安全的辩论日益激烈，一些美国政策制定者呼吁限制中国模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://juejin.cn/post/7223305855922995257">juejin.cn/post/7223305855922995257</a></li>
<li><a href="https://gonglue.us/254636">留给 开 源 模 型 的时间，只剩 6 个月了 – 美 国 攻略</a></li>

</ul>
</details>

**标签**: `#AI`, `#开源模型`, `#黄仁勋`, `#产业政策`, `#中美科技`

---