---
layout: default
title: "Horizon Summary: 2026-05-18 (ZH)"
date: 2026-05-18
lang: zh
---

> From 33 items, 15 important content pieces were selected

---

1. [SGLang v0.5.12 全面支持 DeepSeek V4 推理](#item-1) ⭐️ 9.0/10
2. [Semble：为 AI 代理节省 98%令牌的代码搜索工具](#item-2) ⭐️ 8.0/10
3. [原生与 Web：iOS 文本渲染之争](#item-3) ⭐️ 8.0/10
4. [GDS 反对 NHS 退出开源](#item-4) ⭐️ 8.0/10
5. [OpenClaw 开发者单月消耗 130 万美元 OpenAI API Token](#item-5) ⭐️ 8.0/10
6. [将 80 美元安卓平板改造成 Debian 工作站](#item-6) ⭐️ 7.0/10
7. [AI 不会加速软件流程](#item-7) ⭐️ 7.0/10
8. [特斯拉太阳能屋顶被降级，转向传统面板](#item-8) ⭐️ 7.0/10
9. [Mozilla 捍卫 VPN 反对英国年龄验证提案](#item-9) ⭐️ 7.0/10
10. [AI 是技术，不是产品](#item-10) ⭐️ 7.0/10
11. [苹果芯片运行 LLM 成本高于 OpenRouter](#item-11) ⭐️ 7.0/10
12. [马耳他向全体公民免费提供 ChatGPT Plus](#item-12) ⭐️ 7.0/10
13. [欧盟将对 TikTok 和 Meta 的成瘾设计采取行动](#item-13) ⭐️ 7.0/10
14. [GitHub Copilot 桌面应用进入技术预览](#item-14) ⭐️ 7.0/10
15. [长鑫科技提交 IPO 申请，营收暴增 719%](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.12 全面支持 DeepSeek V4 推理](https://github.com/sgl-project/sglang/releases/tag/v0.5.12) ⭐️ 9.0/10

SGLang v0.5.12 版本为 DeepSeek V4 提供了全面的推理支持，包括张量并行、专家并行、上下文并行和数据并行注意力，以及针对 MegaMoE 优化的 DeepGemm 和 FlashMLA 内核。同时还新增了对 Intern-S2-Preview、MiniCPM-V 4.6 和 Gemma 4 MTP 等模型的支持。 该版本通过先进的并行策略和内核优化，显著提升了 DeepSeek V4（一个重要的大型语言模型）的服务效率和可扩展性，降低了 AI 推理的延迟并提高了吞吐量，惠及更广泛的 AI/ML 社区。 关键技术新增包括用于将非活跃 KV 缓存卸载到 CPU 内存的 HiSparse、速度更快且精度损失可忽略的 W4A4 MegaMoE 内核，以及适用于所有 Nvidia GPU 的统一 Docker 标签。该版本还引入了基于 Blackwell GPU 的 TokenSpeed MLA 注意力后端，支持 FP8 KV 缓存。

github · Fridge003 · May 16, 18:23

**背景**: SGLang 是一个开源的大型语言模型推理引擎，旨在提供高性能和灵活性。DeepSeek V4 是一个先进的 MoE（混合专家）模型，需要复杂的并行策略和内核优化才能高效推理。张量并行和专家并行等技术将计算分布到多个 GPU 上，而 DeepGemm 和 FlashMLA 是专门加速矩阵运算和注意力机制的优化内核。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/DeepGEMM: DeepGEMM: clean and efficient ...</a></li>

</ul>
</details>

**标签**: `#DeepSeek V4`, `#inference`, `#SGLang`, `#LLM`, `#kernel optimization`

---

<a id="item-2"></a>
## [Semble：为 AI 代理节省 98%令牌的代码搜索工具](https://github.com/MinishLab/semble) ⭐️ 8.0/10

Semble 是一个开源代码搜索工具，结合了静态 Model2Vec 嵌入和 BM25，在 CPU 上运行时比 grep 节省 98% 的令牌。它能在约 250ms 内索引典型仓库，查询仅需约 1.5ms，达到 137M 参数 transformer 模型 99% 的检索质量。 这显著降低了像 Claude Code 这样的 AI 代理在大型代码库中导航时的令牌成本，解决了基于代理的代码搜索中的关键低效问题。其仅需 CPU 运行和零配置设置，无需 GPU 或 API 密钥即可使用。 Semble 使用来自 Model2Vec 的 potion-code-16M 静态模型，结合 BM25，通过倒数排名融合（RRF）融合，并使用代码感知信号重新排序。在涵盖 63 个仓库和 19 种语言的约 1250 个查询/文档对的基准测试中，它达到了 0.854 NDCG@10。

hackernews · Bibabomas · May 17, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48169874)

**背景**: AI 代理在找不到相关代码时通常会回退到 grep，这会读取整个文件并消耗大量令牌。现有的替代方案如基于 transformer 的嵌入在 CPU 上运行缓慢，或需要 GPU/API 密钥。Model2Vec 是一种将句子 transformer 转换为小型静态嵌入模型的技术，可将模型大小减少多达 50 倍，速度提高 500 倍，且性能损失极小。BM25 是信息检索中使用的经典概率排序函数。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MinishLab/model2vec">GitHub - MinishLab/model2vec: Fast State-of-the-Art Static ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Okapi_BM25">Okapi BM25 - Wikipedia</a></li>
<li><a href="https://minish.ai/packages/model2vec/introduction/">Model2Vec | Minish</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了概率搜索与确定性 grep 的对比问题，以及代理是否信任非 grep 工具的结果。其他人将 Semble 与 LSP 进行比较，并建议语义搜索也可能有益于人类开发者。

**标签**: `#code search`, `#AI agents`, `#embeddings`, `#open source`, `#efficiency`

---

<a id="item-3"></a>
## [原生与 Web：iOS 文本渲染之争](https://justsitandgrin.im/posts/native-all-the-way-until-you-need-text/) ⭐️ 8.0/10

一位开发者分享了构建高性能 iOS 文本编辑器的经验，发现虽然 TextKit 2 能以低于 8 毫秒的速度处理 5000 行文件的按键重排，但复杂的 Markdown 渲染最终让他们选择 WebKit 作为实用方案。 这篇文章凸显了文本密集型应用中原生与 Web 渲染之间的持续张力，挑战了原生始终优于 Web 视图的假设，尤其是在浏览器引擎日益成熟而 SwiftUI 仍存在性能差距的情况下。 作者用《白鲸记》测试了 TextKit 2，可见范围渲染速度比全文样式快 25 倍，但发现 WebKit 在处理内联图片和双向文本等丰富 Markdown 功能时更实用。

hackernews · dive · May 17, 11:49 · [社区讨论](https://news.ycombinator.com/item?id=48168058)

**背景**: TextKit 2 是苹果在 iOS 15 中引入的现代文本引擎，旨在比 TextKit 1 提供更好的性能和灵活性。WebKit 虽然常与网页浏览器关联，但它本身是 macOS/iOS 的原生框架，能高效渲染 HTML 和 CSS。争论的焦点在于：对于复杂渲染任务，是使用原生框架还是依赖 WebKit。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.apple.com/videos/play/wwdc2021/10061/">Meet TextKit 2 - WWDC21 - Videos - Apple Developer</a></li>
<li><a href="https://developer.apple.com/videos/play/wwdc2022/10090/">What's new in TextKit and text views - WWDC22 - Videos - Apple Developer</a></li>
<li><a href="https://news.ycombinator.com/item?id=48168455">If you're on macOS, WebKit is a native OS framework. | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 评论者讨论了权衡：有人认为在 macOS 上 WebKit 是原生框架，适合 Markdown 渲染；另一些人指出 SwiftUI 仍有性能问题，且存在成熟的 SwiftUI Markdown 渲染器。一位开发者分享了他们使用 TextKit 2 处理大文件的积极体验。

**标签**: `#text rendering`, `#native vs web`, `#iOS development`, `#performance`, `#SwiftUI`

---

<a id="item-4"></a>
## [GDS 反对 NHS 退出开源](https://simonwillison.net/2026/May/17/gds-weighs-in/#atom-everything) ⭐️ 8.0/10

英国政府数字服务局（GDS）于 2026 年 5 月 14 日发布指南，建议公共部门组织默认保持开源仓库公开，直接反对 NHS 最近因 Project Glasswing 报告的安全漏洞而关闭其 GitHub 仓库的决定。 英国两大政府机构之间的公开分歧凸显了公共部门软件中开放与安全之间的关键政策辩论，对政府 IT 的透明度、成本和复用具有深远影响。 GDS 的指南题为《AI、开放代码与公共部门漏洞风险》，强调将仓库设为私有会增加交付和政策成本，同时降低复用和审查。Terence Eden 将此解读为公务员体系内罕见的公开升级，比喻为“被邀请参加没有饼干的会议”。

rss · Simon Willison · May 17, 15:59

**背景**: NHS 在通过 Project Glasswing（Anthropic 主导的利用先进 AI 的网络安全倡议）报告漏洞后，决定关闭其公共 GitHub 仓库。GDS 作为政府数字中心，通常倡导开源以促进透明度和效率。这一事件标志着两个组织之间的重大政策分歧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.gov.uk/government/organisations/government-digital-service">Government Digital Service - GOV.UK</a></li>
<li><a href="https://shkspr.mobi/blog/2026/05/nhs-goes-to-war-against-open-source/">NHS Goes To War Against Open Source</a></li>
<li><a href="https://www.theregister.com/2026/05/05/nhs_to_closesource_hundreds_of_repos/">NHS to close-source hundreds of GitHub repos over AI, security concerns</a></li>

</ul>
</details>

**社区讨论**: 文章未提供评论，但 Terence Eden 博客及其他渠道的更广泛社区讨论显示，许多人支持 GDS 的立场，批评 NHS 的反应过度，损害了开源的好处。

**标签**: `#open source`, `#government policy`, `#security`, `#public sector`

---

<a id="item-5"></a>
## [OpenClaw 开发者单月消耗 130 万美元 OpenAI API Token](https://www.tomshardware.com/tech-industry/artificial-intelligence/openclaw-creator-burns-through-1-3-million-in-openai-api-tokens-in-a-single-month) ⭐️ 8.0/10

OpenClaw 开发者 Peter Steinberger 披露，其团队在 30 天内消耗了价值 130 万美元的 OpenAI API Token，涉及 6030 亿个 Token 和 760 万次请求，由约 100 个 Codex 代理产生。 此案例凸显了大规模 AI 代理自动化的巨大运营成本，对 AI 开发的经济性和自主编码代理的可持续性具有重要影响。 高额费用主要由 Codex 的“快速模式”计费驱动；若禁用该模式，原始 API 成本将降至约 30 万美元。账单还显示使用了 2026 年 4 月 23 日版本的 GPT-5.5 模型。

telegram · zaihuapd · May 17, 13:38

**背景**: OpenClaw 是一个免费开源的自主 AI 代理，通过大型语言模型执行任务，并以消息平台作为主要界面。Codex 是 OpenAI 推出的 AI 编码代理，用于辅助软件开发任务。GPT-5.5 是 OpenAI 于 2026 年 4 月 23 日发布的大型语言模型，以其先进的编码能力著称。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw</a></li>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**标签**: `#AI`, `#OpenAI`, `#API costs`, `#Codex`, `#automation`

---

<a id="item-6"></a>
## [将 80 美元安卓平板改造成 Debian 工作站](https://github.com/tech4bot/rk3562deb) ⭐️ 7.0/10

一位开发者在 GitHub 上发布指南，展示如何将一台 80 美元的 RK3562 安卓平板电脑改造成可用的 Debian Linux 工作站，并利用 AI 辅助逆向工程实现硬件支持。 该项目展示了将廉价、易得的硬件改造为 Linux 系统的潜力，降低了爱好者和开发者的入门门槛。同时，它也凸显了 AI 如何加速逆向工程，使设备破解更加便捷。 该平板采用瑞芯微 RK3562 四核处理器和 4GB 内存，多任务能力有限，但足以运行轻量级桌面环境或基于终端的工作流。指南包含启动 Debian 并使大部分设备正常工作的步骤。

hackernews · tech4bot · May 17, 13:16 · [社区讨论](https://news.ycombinator.com/item?id=48168668)

**背景**: RK3562 是瑞芯微推出的一款低功耗四核应用处理器，常用于廉价安卓平板。AI 辅助逆向工程利用机器学习自动分析硬件和软件，从而更轻松地将操作系统移植到新设备上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rockchips.net/product/rk3562/">RK3562 - Rockchips.net</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_reverse_engineering">AI-assisted reverse engineering - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一项目表示热情，有人指出 4GB 内存足以完成轻量级任务，如基于终端的开发或 VAX 模拟。还有人询问如何利用 AI 进行逆向工程的学习资源，另有人警告此类突破可能导致廉价平板价格上涨。

**标签**: `#Linux`, `#Embedded Systems`, `#Hardware Hacking`, `#Debian`, `#AI-assisted Reverse Engineering`

---

<a id="item-7"></a>
## [AI 不会加速软件流程](https://frederickvanbrabant.com/blog/2026-05-15-i-dont-think-ai-will-make-your-processes-go-faster/) ⭐️ 7.0/10

Frederick Van Brabant 认为，AI 不会加速软件开发流程，因为主要瓶颈是不清晰的需求，而 AI 在没有人类输入的情况下无法解决这一问题。 这挑战了当前认为 AI 将大幅提升软件生产力的主流观点，强调诸如需求模糊等基本的人为问题仍然至关重要。 文章指出，软件开发人员长期以来一直寻求详细的问题描述，但模糊的功能请求是常态；AI 在没有人类干预的情况下无法澄清这些需求。

hackernews · TheEdonian · May 17, 12:13 · [社区讨论](https://news.ycombinator.com/item?id=48168221)

**背景**: 在软件工程中，需求收集通常是最耗时且容易出错的阶段。像 LLM 这样的 AI 工具可以快速生成代码，但仍然依赖于精确的规范来产生正确的输出。

**社区讨论**: 评论者大多同意需求是瓶颈，一些人指出 AI 仍然可以在构思、文档和部署方面提供帮助。其他人则认为 AI 对于超出自身专业领域的任务更具变革性。

**标签**: `#AI`, `#software engineering`, `#productivity`, `#requirements`

---

<a id="item-8"></a>
## [特斯拉太阳能屋顶被降级，转向传统面板](https://electrek.co/2026/05/14/tesla-solar-roof-promise-vs-reality-pivot-panels/) ⭐️ 7.0/10

特斯拉正从太阳能屋顶产品转向传统太阳能电池板，由于成本高昂和经济性差，太阳能屋顶实际上已被搁置。 这一战略转变表明，特斯拉雄心勃勃的一体化太阳能屋顶方案未能实现大众市场可行性，可能重塑住宅太阳能市场并影响消费者选择。 特斯拉太阳能屋顶平均成本约 10.6 万美元（税前），而传统屋顶更换加常规太阳能电池板约 6 万美元，投资回收期为 15-25 年，而面板为 7-12 年。

hackernews · celsoazevedo · May 17, 04:09 · [社区讨论](https://news.ycombinator.com/item?id=48165980)

**背景**: 特斯拉太阳能屋顶作为高端产品推出，将太阳能电池集成到屋顶瓦片中，旨在替代传统屋顶同时发电。然而，与传统太阳能电池板相比，高昂的安装成本和复杂的物流阻碍了其普及，传统面板更便宜且安装更简单。

**社区讨论**: 评论者对产品衰落表示失望，指出其美观性，但一致认为经济性从未奏效。有人猜测太阳能屋顶最初是为了在特斯拉财务困难时提振股价。

**标签**: `#Tesla`, `#solar energy`, `#renewable energy`, `#business strategy`, `#clean tech`

---

<a id="item-9"></a>
## [Mozilla 捍卫 VPN 反对英国年龄验证提案](https://blog.mozilla.org/netpolicy/2026/05/15/mozilla-to-uk-regulators-vpns-are-essential-privacy-and-security-tools-and-should-not-be-undermined/) ⭐️ 7.0/10

Mozilla 已向英国政府关于在线内容年龄验证的咨询提交回应，认为 VPN 是必要的隐私和安全工具，不应被削弱。 这很重要，因为英国提出的 VPN 年龄验证要求可能为削弱在线隐私和安全开创全球先例，影响数百万依赖 VPN 保护的用户。 这份名为《在网络世界中成长》的咨询文件在第 30 页左右埋藏了一个关于对 VPN 进行年龄验证的具体问题。Mozilla 的回应强调，监管机构应追究平台对在线伤害的责任，而非针对 VPN。

hackernews · WithinReason · May 17, 06:17 · [社区讨论](https://news.ycombinator.com/item?id=48166459)

**背景**: VPN（虚拟专用网络）加密互联网流量并隐藏用户的 IP 地址，提供在线隐私和安全。英国政府一直在探索年龄验证措施以保护儿童免受有害内容侵害，但批评者认为，要求 VPN 进行年龄验证会损害其核心隐私功能，并可能导致监控。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.mozilla.org/netpolicy/2026/05/15/mozilla-to-uk-regulators-vpns-are-essential-privacy-and-security-tools-and-should-not-be-undermined/">Mozilla to UK regulators: VPNs are essential privacy and security tools and should not be undermined – Open Policy & Advocacy</a></li>
<li><a href="https://www.youtube.com/watch?v=uzmR4nt1rpE">UK Proposes 24/7 Phone Surveillance & VPN Age Verification</a></li>
<li><a href="https://outbyte.com/blog/the-uk-debates-age-checks-for-vpns-will-it-protect-kids-or-destroy-adult-privacy/">The UK Debates Age Checks for VPNs : Will It... - Outbyte Official Blog</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，澳大利亚政府出人意料地推荐使用 VPN，一位用户提到 Mozilla 的回应是针对特定的英国咨询。另一位用户质疑谷歌是否发表了类似声明，还有评论引用乔治·奥威尔的《1984》作为对英国数字政策的警告。

**标签**: `#privacy`, `#VPN`, `#UK regulation`, `#digital rights`, `#Mozilla`

---

<a id="item-10"></a>
## [AI 是技术，不是产品](https://daringfireball.net/2026/05/ai_is_technology_not_a_product) ⭐️ 7.0/10

一篇文章认为，AI 应被视为增强产品（如 Siri）的基础技术，而非独立产品，并与“Dropbox 是功能”的辩论相类比。 这一观点挑战了当前的 AI 热潮，敦促公司专注于将 AI 集成到以用户为中心的产品中，而非将其作为独立产品营销，这可能重塑整个科技行业的产品策略。 文章引用了苹果以客户为中心的方法以及 iTunes Ping 失败的历史例子，说明技术必须服务于明确的用户需求。它还呼应了早期的“Dropbox 是功能”论点，暗示 AI 公司可能难以建立可持续的生态系统。

hackernews · ch_sm · May 17, 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48168626)

**背景**: 关于 AI 是产品还是技术的辩论，反映了科技界早期的讨论，例如“Dropbox 是功能”的论点，即云存储被视为一种商品而非独立产品。苹果历来专注于将技术融入精致的用户体验，正如史蒂夫·乔布斯强调从客户体验出发逆向工作。

**社区讨论**: 评论者大多同意文章观点，指出苹果理想的 AI 实现是让 Siri 无缝工作而不让人觉得是 AI。一位评论者引用史蒂夫·乔布斯从客户体验出发逆向工作的哲学，另一位则直接类比“Dropbox 是功能”的论点，警告 AI 公司若没有硬件集成则可能变得可有可无。

**标签**: `#AI`, `#product design`, `#Apple`, `#technology strategy`

---

<a id="item-11"></a>
## [苹果芯片运行 LLM 成本高于 OpenRouter](https://www.williamangel.net/blog/2026/05/17/offline-llm-energy-use.html) ⭐️ 7.0/10

William Angel 的一篇博客文章比较了在苹果芯片硬件上运行大型语言模型与使用 OpenRouter 等云 API 的成本，结论是本地推理更昂贵。该分析考虑了硬件折旧、电费和 token 吞吐量。 这挑战了本地推理更便宜的普遍假设，对在设备端和云端 AI 之间做决策的开发者和企业有影响。该争论还凸显了云提供商可能定价过低，长期不可持续。 作者估计，即使在乐观假设下（50W 功耗、40 tokens/秒、10 年寿命），MacBook Pro Max 的成本也只与 OpenRouter 的 Gemma4 31b 定价（每百万 token 约 38-50 美分）相当。然而，该分析将电费向上取整，并假设全天候专用运行，可能不符合实际情况。

hackernews · datadrivenangel · May 17, 12:09 · [社区讨论](https://news.ycombinator.com/item?id=48168198)

**背景**: 在苹果芯片（如 M4 Max）上本地运行 LLM 因隐私和离线使用而受欢迎，但硬件成本很高。OpenRouter 等云 API 聚合多种模型并按 token 收费，通常由风险投资补贴。这种比较对两种 AI 推理方式都相关。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.williamangel.net/blog/2026/05/17/offline-llm-energy-use.html">Apple Silicon costs more than OpenRouter</a></li>
<li><a href="https://openrouter.ai/pricing">Pricing - OpenRouter</a></li>
<li><a href="https://www.compute-market.com/blog/mac-mini-m4-for-ai-apple-silicon-2026">Mac Mini M4 for AI 2026 — LLM Benchmarks & Review | Compute Market</a></li>

</ul>
</details>

**社区讨论**: 评论者批评了方法论：bastawhiz 指出取整误差和不切实际的 24/7 使用假设；applfanboysbgon 指出分析忽略了笔记本电脑的双重使用价值；dijit 认为云 API 亏本销售，使比较不公平。其他人建议使用更高效的模型如 Qwen3.6 27B 以获得更好的速度和成本。

**标签**: `#LLM`, `#Apple Silicon`, `#cost analysis`, `#inference`, `#cloud vs local`

---

<a id="item-12"></a>
## [马耳他向全体公民免费提供 ChatGPT Plus](https://openai.com/index/malta-chatgpt-plus-partnership/) ⭐️ 7.0/10

OpenAI 与马耳他政府宣布国家级合作，公民完成马耳他大学开发的 AI 素养课程后，可免费获得一年 ChatGPT Plus 订阅。 这是 ChatGPT Plus 首次国家级合作，为全球政府主导的 AI 普及和教育计划树立了先例。 该项目名为“AI for All”，将于 2026 年 5 月启动，由马耳他数字创新局管理，后续将扩展至海外公民。

telegram · zaihuapd · May 16, 10:40

**背景**: 马耳他于 2019 年推出国家 AI 战略，旨在推动 AI 采用和创新。马耳他数字创新局（MDIA）负责监督数字创新和 AI 治理。此次合作将 AI 访问与强制性教育相结合，以促进负责任的使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://gagadget.com/en/710697-malta-is-giving-citizens-free-chatgpt-plus-if-they-take-an-ai-class-first/">Malta is giving citizens free ChatGPT Plus — if they take an AI class first</a></li>
<li><a href="https://de.euronews.com/next/2026/05/16/malta-burger-erhalten-chatgpt-plus-gratis-uber-nationales-ki-programm">Malta : Bürger erhalten ChatGPT Plus gratis über... | Euronews</a></li>
<li><a href="https://mdia.gov.mt/">Malta Digital Innovation Authority</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#AI policy`, `#education`, `#partnership`

---

<a id="item-13"></a>
## [欧盟将对 TikTok 和 Meta 的成瘾设计采取行动](https://unwire.hk/2026/05/16/eu-tiktok-meta-addictive-design-child-protection/life-tech/social-network/) ⭐️ 7.0/10

欧盟委员会主席冯德莱恩在丹麦峰会上宣布，欧盟将对 TikTok 和 Meta（Instagram、Facebook）的成瘾设计功能以及 13 岁年龄限制执行不力采取行动，法律建议预计在 2026 年夏季前就绪。 这标志着欧盟根据《数字服务法》对平台设计监管的重大升级，可能迫使主要社交媒体公司全球范围内重新设计核心参与功能，并为其他司法管辖区树立先例。 欧盟已初步裁定 TikTok 的成瘾设计和 Meta 的年龄核实机制违反《数字服务法》，并已推出开源匿名年龄核实应用。澳大利亚已禁止 16 岁以下使用社交媒体，多国跟进立法。

telegram · zaihuapd · May 16, 14:33

**背景**: 《数字服务法》（DSA）是欧盟一项里程碑式的法规，对大型在线平台施加了更严格的义务，以应对非法内容、系统性风险和用户安全。成瘾设计指无限滚动、自动播放和推送通知等功能，旨在最大化用户参与度和在平台上的停留时间。年龄验证已成为政府保护未成年人上网的关键焦点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://digital-strategy.ec.europa.eu/en/news/commission-preliminarily-finds-tiktoks-addictive-design-breach-digital-services-act">Commission preliminarily finds TikTok's addictive design in ...</a></li>
<li><a href="https://www.technobezz.com/news/eu-plans-new-rules-targeting-addictive-design-on-tiktok-and-meta-to-protect-children">EU Plans New Rules Targeting Addictive Design on TikTok and ...</a></li>
<li><a href="https://www.freevacy.com/news/politico/von-der-leyen-hints-social-media-ban-and-age-verification-possible-by-summer/7372">Von der Leyen hints social media ban and age verification possible...</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#addictive design`, `#TikTok`, `#Meta`, `#Digital Services Act`

---

<a id="item-14"></a>
## [GitHub Copilot 桌面应用进入技术预览](https://github.blog/changelog/2026-05-14-github-copilot-app-is-now-available-in-technical-preview/) ⭐️ 7.0/10

GitHub Copilot 桌面应用现已进入技术预览，用户可以直接从 issue、PR、提示词或历史会话启动隔离的开发会话，在应用内查看变更差异、运行测试、创建 PR，并支持 Agent Merge 自动处理 review 评论和合并。 此次更新将 Copilot 从代码补全工具转变为完整的开发环境，使开发者无需离开应用即可执行复杂工作流。它显著减少了上下文切换，并自动处理合并冲突等繁琐任务，从而提升了 Copilot Pro 和 Pro+ 订阅者的生产力。 技术预览版立即面向 Copilot Pro 和 Pro+ 订阅者开放，Business 和 Enterprise 用户将在本周内陆续获得访问权限，但需要组织管理员在策略中开启预览和 CLI 权限。Agent Merge 功能此前于 2026 年 4 月作为云代理功能推出，用于自动处理 review。

telegram · zaihuapd · May 16, 15:07

**背景**: GitHub Copilot 是由 GitHub 和 OpenAI 开发的 AI 代码补全与编程助手，集成在 VS Code、JetBrains 等主流 IDE 中。新的桌面应用将 Copilot 的能力从内联建议扩展到隔离环境，支持运行测试、查看差异、管理 PR 等任务。Agent Merge 是一项利用云端代理自动解决合并冲突和处理 review 评论的功能，可减少手动操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-04-13-fix-merge-conflicts-in-three-clicks-with-copilot-cloud-agent/">Fix merge conflicts in three clicks with Copilot cloud agent - GitHub Changelog</a></li>
<li><a href="https://github.blog/changelog/2026-03-26-ask-copilot-to-resolve-merge-conflicts-on-pull-requests/">Ask @copilot to resolve merge conflicts on pull requests - GitHub Changelog</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot - Wikipedia</a></li>

</ul>
</details>

**标签**: `#GitHub Copilot`, `#AI coding assistant`, `#developer tools`, `#technical preview`

---

<a id="item-15"></a>
## [长鑫科技提交 IPO 申请，营收暴增 719%](https://api3.cls.cn/share/article/2373399?os=android&amp;sv=8.7.8&amp;app=cailianpress) ⭐️ 7.0/10

长鑫科技（CXMT）已向上交所科创板提交 IPO 申请，披露 2026 年一季度营收 508 亿元（同比增长 719.13%），净利润 330.1 亿元，扭亏为盈。公司同时预计 2026 年上半年营收为 1100 亿至 1200 亿元。 此次 IPO 申请凸显了在 AI 需求驱动的全球内存短缺背景下，中国本土 DRAM 产业的快速增长。若成功上市，将为长鑫科技提供重要融资渠道，助力其扩大产能并与三星、SK 海力士、美光竞争。 公司 2026 年一季度归母净利润为 247.6 亿元，扣非归母净利润为 263.4 亿元。上半年业绩指引显示持续强劲势头，营收同比增长 612%至 677%。

telegram · zaihuapd · May 17, 11:05

**背景**: DRAM（动态随机存取存储器）是一种半导体存储器，广泛用作计算机和服务器的内存。全球 DRAM 市场目前由三星、SK 海力士和美光三巨头主导。长鑫科技是中国领先的 DRAM 制造商，其在科创板（中国版纳斯达克）上市将是中国半导体自主化进程中的一个里程碑。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random-access memory - Wikipedia</a></li>
<li><a href="https://baike.kuaiji.com/v231914478.html">扣非归母净利润 (财会术语) - 会计百科</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#IPO`, `#DRAM`, `#China tech`, `#finance`

---