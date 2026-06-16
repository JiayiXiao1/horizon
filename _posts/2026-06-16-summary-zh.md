---
layout: default
title: "Horizon Summary: 2026-06-16 (ZH)"
date: 2026-06-16
lang: zh
---

> From 37 items, 17 important content pieces were selected

---

1. [LinkedIn 求职陷阱：npm 后门攻击开发者](#item-1) ⭐️ 9.0/10
2. [哪吒监控高危路径穿越漏洞（CVSS 9.1）](#item-2) ⭐️ 9.0/10
3. [vLLM v0.23.0 优化 DeepSeek-V4 并扩展 Model Runner V2](#item-3) ⭐️ 8.0/10
4. [智能灯泡中隐藏的禁书图书馆](#item-4) ⭐️ 8.0/10
5. [Iroh 1.0：点对点网络库发布](#item-5) ⭐️ 8.0/10
6. [Hetzner 云服务器价格最高涨 3 倍](#item-6) ⭐️ 8.0/10
7. [福克斯以 220 亿美元收购 Roku](#item-7) ⭐️ 8.0/10
8. [Salesforce 以 36 亿美元收购 Fin](#item-8) ⭐️ 8.0/10
9. [AI 为何尚未且不会取代软件工程师](#item-9) ⭐️ 8.0/10
10. [美国政府以安全为由要求 Anthropic 禁用两款 AI 模型](#item-10) ⭐️ 8.0/10
11. [Rio 3.5 模型被曝套壳中国开源模型](#item-11) ⭐️ 8.0/10
12. [本地模型替代云端编程助手](#item-12) ⭐️ 7.0/10
13. [《指挥官基恩》引擎白皮书发布](#item-13) ⭐️ 7.0/10
14. [铜转运药物恢复记忆并清除阿尔茨海默病蛋白](#item-14) ⭐️ 7.0/10
15. [性格冲突导致 Anthropic 模型下线](#item-15) ⭐️ 7.0/10
16. [字节跳动洽购天数智芯 AI 芯片，考虑百度昆仑芯](#item-16) ⭐️ 7.0/10
17. [消费者起诉 Anthropic 夸大 AI 订阅用量](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [LinkedIn 求职陷阱：npm 后门攻击开发者](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 9.0/10

一名开发者发现，LinkedIn 上的虚假招聘人员发送的 GitHub 仓库中隐藏了后门，该后门利用 npm 的自动脚本执行功能，在安装依赖时运行恶意代码。 这种新颖的社会工程攻击针对求职面试中的开发者，利用信任过程，若成功可能导致广泛的供应链入侵，已有多个受害者报告。 后门隐藏在注释掉的测试代码中，通过 npm 的'prepare'脚本执行，该脚本在'npm install'后自动运行。载荷与远程服务器通信以接收命令。

hackernews · lwhsiao · Jun 15, 20:00 · [社区讨论](https://news.ycombinator.com/item?id=48546294)

**背景**: npm 是 Node.js 的包管理器，允许包定义在安装时自动运行的脚本（如'prepare'）。此功能虽然方便，但可能被滥用来执行任意代码。针对开发者的社会工程攻击有所增加，虚假招聘是常见手段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.to/trknhr/lessons-from-the-spring-2026-oss-incidents-hardening-npm-pnpm-and-github-actions-against-1jnp">Lessons from the Spring 2026 OSS Incidents: Hardening npm , pnpm...</a></li>
<li><a href="https://docs.bswen.com/blog/2026-03-31-axios-supply-chain-attack/">What Happened in the Axios npm Supply Chain Attack? | BSWEN</a></li>

</ul>
</details>

**社区讨论**: 评论者表示担忧，认为这种攻击与正常的面试任务非常接近，有人报告已多次遇到类似尝试。尽管已举报，但 GitHub 和 LinkedIn 未删除恶意内容，引发不满。

**标签**: `#supply chain attack`, `#social engineering`, `#npm`, `#cybersecurity`, `#LinkedIn`

---

<a id="item-2"></a>
## [哪吒监控高危路径穿越漏洞（CVSS 9.1）](https://github.com/nezhahq/nezha/security/advisories/GHSA-5c25-7vpj-9mqh) ⭐️ 9.0/10

哪吒监控（Nezha）v2.0.13 以下版本被披露存在严重路径穿越漏洞（CVE-2026-53519，CVSS 9.1），未经身份验证的攻击者可读取任意文件（如 config.yaml）并获取 JWT 密钥。 哪吒监控被广泛用于服务器监控，该漏洞可能导致仪表盘及关联代理完全沦陷，因为 JWT 密钥可被用于伪造身份认证令牌。 该漏洞位于仪表盘的 NoRoute 处理程序中，任何以 /dashboard 开头的 URL 都被视为管理前端资源请求，从而允许通过 /dashboard../data/config.yaml 等序列进行路径穿越。利用无需身份验证。

telegram · zaihuapd · Jun 15, 09:25

**背景**: 哪吒监控是一款开源、轻量的服务器监控与运维工具，由仪表盘（服务端）和安装在受监控主机上的代理组成。JWT（JSON Web Token）常用于身份认证；若密钥泄露，攻击者可伪造有效令牌获得未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.thehackerwire.com/nezha-monitoring-unauthenticated-file-read-cve-2026-53519/">Nezha Monitoring Unauthenticated File Read (CVE-2026-53519) – TheHackerWire</a></li>
<li><a href="https://cve.threatint.eu/CVE/CVE-2026-53519">CVE-2026-53519 | THREATINT</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#nezha`, `#path traversal`, `#open source`

---

<a id="item-3"></a>
## [vLLM v0.23.0 优化 DeepSeek-V4 并扩展 Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 为 DeepSeek-V4 引入了重大优化，包括解耦的稀疏 MLA 元数据、TRTLLM-gen 注意力内核以及 Mega-MoE 的 EPLB 支持，同时将 Model Runner V2 (MRv2) 默认扩展到 Llama 和 Mistral 密集模型。 这些改进显著提升了两个最重要模型系列——DeepSeek-V4 和 Llama/Mistral——的推理性能和效率，使 vLLM 成为生产部署中更具吸引力的开源推理引擎。 该版本包含来自 200 位贡献者的 408 次提交，新增了对 Step-3.7-Flash 和 Gemma 4 Unified 等模型的支持，并引入了具有流式生成和动态 LoRA 端点的 Rust 前端。

github · khluu · Jun 15, 05:27

**背景**: vLLM 是一个高性能的开源 LLM 推理和服务库，在 AI 社区中被广泛使用。Model Runner V2 (MRv2) 是对 vLLM 执行核心的彻底重写，旨在更加模块化和高效。DeepSeek-V4 是一个具有稀疏混合专家 (MoE) 架构的大型语言模型，其 MLA（多头潜在注意力）机制是其效率的关键。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vllm-website-5zwgmvte0-inferact-inc.vercel.app/blog/mrv2">Model Runner V 2 : A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse_mla - vLLM Documentation</a></li>
<li><a href="https://nvidia.github.io/TensorRT-LLM/features/attention.html">Multi-Head, Multi-Query, and Group-Query Attention — TensorRT LLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#open source`, `#AI infrastructure`

---

<a id="item-4"></a>
## [智能灯泡中隐藏的禁书图书馆](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 8.0/10

一位开发者利用开源固件 Tasmota，将禁书图书馆嵌入到一个 Wi-Fi 智能灯泡中，使附近的人可以通过灯泡的 Wi-Fi 网络访问这些书籍。 该项目创造性地将物联网黑客技术与言论自由倡导相结合，展示了如何将日常设备重新利用以规避审查并保持信息获取渠道。 该灯泡运行一个 Web 服务器，当连接到其 Wi-Fi 网络时，可提供禁书的 EPUB 文件；存储空间限制约为 2 MB，因此只能存储少量书籍。

hackernews · sohkamyung · Jun 15, 22:37 · [社区讨论](https://news.ycombinator.com/item?id=48547985)

**背景**: Tasmota 是一种开源固件，可替换许多基于 ESP8266 的智能设备的原始固件，让用户完全控制设备。该项目受 PirateBox 和 LibraryBox 启发，它们将 Wi-Fi 接入点转变为离线文件共享中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.richardosgood.com/posts/banned-book-library/">Banned Book Library | Rick's Blog</a></li>
<li><a href="https://github.com/ct-Open-Source/tuya-convert/issues/830">Merkury MI-BW904-999W, Merkury Innovations A21 Smart Light Bulb ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_books_banned_by_governments">List of books banned by governments - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该项目的创造力和政治声明，一些人将其与 PirateBox 和网状网络相提并论。一位用户指出“禁书”列表可能受媒体叙事影响，但总体情绪是积极的。

**标签**: `#censorship`, `#IoT`, `#free speech`, `#hacking`, `#privacy`

---

<a id="item-5"></a>
## [Iroh 1.0：点对点网络库发布](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 作为一个点对点网络库发布，它允许应用实例之间轻松、安全地连接，无需用户账户，并且现在支持自定义传输层。 这通过提供“应用层的 Tailscale”方法简化了分布式应用开发，减少了对中心化基础设施和用户账户管理的需求。 Iroh 底层使用 QUIC 多路径，并原生支持 IPv4、IPv6 和中继传输，新的自定义传输 API 允许集成 WebRTC、BLE 或 Tor 等协议。

hackernews · chadfowler · Jun 15, 15:13 · [社区讨论](https://news.ycombinator.com/item?id=48542480)

**背景**: Iroh 是一个基于 Rust 的点对点库，构建在 QUIC 之上，使用中继和打洞技术。对等点通过 NodeId 连接，在握手期间验证以提供端到端加密和认证。这类似于 Tailscale 的工作方式，但位于应用层，意味着开发者可以直接将 Iroh 嵌入到他们的应用中，无需用户拥有单独的账户或 VPN 软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.iroh.computer/docs/overview">A high-level description of what iroh is</a></li>
<li><a href="https://www.iroh.computer/blog/tor-custom-transport">Use iroh with Tor for anonymous connections - Iroh</a></li>

</ul>
</details>

**社区讨论**: 社区讨论将 Iroh 描述为“应用层的 Tailscale”，开发者询问自定义传输支持（WebRTC、BLE、LoRa），并指出需要更清晰的文档说明拨号密钥和中继使用。一些用户质疑 Iroh 解决的问题，而另一些用户则赞扬向去中心化网络的迈进。

**标签**: `#networking`, `#peer-to-peer`, `#rust`, `#library`, `#release`

---

<a id="item-6"></a>
## [Hetzner 云服务器价格最高涨 3 倍](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner 宣布对其云服务器进行重大价格调整，部分实例价格涨幅高达 3 倍，新服务器立即生效，现有服务器从 2025 年 2 月 1 日起执行。 作为欧洲主要云服务商的大幅涨价，反映了 AI 驱动的需求对硬件成本的广泛影响，可能迫使开发者和企业重新考虑云支出或寻找替代方案。 大多数云产品涨幅在 30-43%之间，但某些实例如 CX22 从每月€3.49 涨至€10.49，涨幅达 200%。超额流量价格保持不变。

hackernews · tuhtah · Jun 15, 13:19 · [社区讨论](https://news.ycombinator.com/item?id=48540844)

**背景**: Hetzner 是一家受欢迎的德国托管服务商，以价格实惠的专用服务器和云服务著称。此次涨价归因于 AI 需求推动的硬件成本上升，导致 RAM 和 SSD 竞争加剧，以及全球供应链限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lowendtalk.com/discussion/200033/hetzner-black-friday-price-increase-surprise">Hetzner Black Friday Price Increase Surprise — LowEndTalk</a></li>
<li><a href="https://microage.ca/winnipeg/whats-driving-the-surge-in-hardware-prices/">What’s Driving the Surge in Hardware Prices – MB – Manitoba</a></li>

</ul>
</details>

**社区讨论**: 社区反应普遍负面，用户对 3 倍涨幅感到震惊并质疑其合理性。部分评论者指出硬件成本确实上涨，另一些人则推荐 GTHost 等替代方案，或与超大规模云服务商进行比较。

**标签**: `#cloud computing`, `#pricing`, `#Hetzner`, `#hardware costs`, `#AI infrastructure`

---

<a id="item-7"></a>
## [福克斯以 220 亿美元收购 Roku](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

福克斯公司已同意以约 220 亿美元收购 Roku，这是近年来流媒体行业最大的收购案之一。 这笔交易可能重塑电视硬件格局，让一家大型内容提供商直接控制美国 30%-50%家庭使用的平台，引发对内容中立性和反垄断问题的担忧。 为获得反垄断批准，福克斯已承诺保持 Roku 平台对 Netflix、Disney+和 Max 等竞争对手开放。消息公布后，福克斯股价下跌 15%。

hackernews · thm · Jun 15, 12:50 · [社区讨论](https://news.ycombinator.com/item?id=48540499)

**背景**: Roku 是领先的流媒体硬件和软件平台，以其服务无关的架构著称，允许用户访问各种流媒体应用而不偏向任何特定内容提供商。福克斯是一家大型媒体集团，拥有 Fox News、Fox Sports 和福克斯广播网络。此次收购是 Lachlan Murdoch 巩固控制权后福克斯的首笔重大交易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://easternherald.com/2026/06/15/fox-corporation-roku-22-billion-acquisition-antitrust-open-platform/">Fox Buys Roku for $22 Billion — and Its Biggest Problem Is Its Own...</a></li>
<li><a href="https://www.usatoday.com/story/money/business/2026/06/15/fox-roku-22b-streaming-deal/90557322007/">Fox to acquire Roku for $22B in streaming push</a></li>

</ul>
</details>

**社区讨论**: 社区情绪普遍悲观，用户对福克斯控制 Roku 硬件以及平台可能失去中立性表示担忧。一些用户已开始转向 Nvidia Shield 等替代品，以避免广告和内容偏见。

**标签**: `#acquisition`, `#streaming`, `#media`, `#antitrust`, `#Roku`

---

<a id="item-8"></a>
## [Salesforce 以 36 亿美元收购 Fin](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 8.0/10

Salesforce 已签署最终协议，以 36 亿美元收购 AI 客服初创公司 Fin（前身为 Intercom）。 此次收购加剧了 AI 代理领域的竞争，尤其是针对 Salesforce 前联席 CEO Bret Taylor 创立的 Sierra（估值 158 亿美元），并表明 Salesforce 致力于将 AI 代理嵌入其 CRM 生态系统。 Fin 按解决次数而非 token 收费，并能从历史对话中学习；它已处理 Intercom 76%的客服请求。这笔交易发生在 Fin 一个月前从 Intercom 更名之后。

hackernews · colesantiago · Jun 15, 12:08 · [社区讨论](https://news.ycombinator.com/item?id=48540126)

**背景**: Fin 是一个 AI 驱动的客服代理，可自动回复和升级问题。Salesforce 一直在开发自己的 AI 代理平台 Agentforce，允许在 Salesforce 生态系统中构建和部署自定义 AI 代理。此次收购有助于 Salesforce 与 Sierra、Decagon 等独立 AI 客服初创公司竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fin.ai/">Fin . The highest performing Customer Agent</a></li>
<li><a href="https://www.salesforce.com/agentforce/">Agentforce: The AI Agent Platform | Salesforce</a></li>
<li><a href="https://www.linkedin.com/pulse/1-12m-year-startup-inside-jayanthan-swamy-hj2xc">$1 to $12M in a year: a startup inside a Startup</a></li>

</ul>
</details>

**社区讨论**: 社区看法不一：有人称赞执行良好的 AI 客服代理（如 Starlink），也有人担心 AI 会编造借口。评论者注意到与 Sierra 和 Decagon 的竞争格局，部分人质疑帮助台 SaaS 对非企业客户的长期可行性。

**标签**: `#acquisition`, `#AI`, `#customer support`, `#Salesforce`, `#startup`

---

<a id="item-9"></a>
## [AI 为何尚未且不会取代软件工程师](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表文章，认为 AI 尚未且不会取代软件工程师，并引用纽约州 WARN 法案申报数据：在披露要求实施的第一年，没有一家公司报告与 AI 相关的裁员。 这一基于证据的反驳挑战了“AI 将导致软件工程大规模失业”的主流叙事，而软件工程被认为是最易受 AI 冲击的职业之一。该观点为工程师提供了信心，并为关于 AI 对劳动力影响的公共讨论提供了依据。 作者指出软件工程中 AI 无法自动化的三个真正瓶颈：决定构建什么、对交付物进行验证并承担责任，以及对代码库、业务和环境的深度人类理解。他们指出 AI 加快了编码速度，但并未触及这些核心活动。

rss · Simon Willison · Jun 14, 23:54

**背景**: 《工人调整和再培训通知法案》（WARN Act）要求雇主在发生大规模裁员前提前通知。2025 年 3 月，纽约州在其 WARN 申报表中增加了 AI 披露复选框，成为美国首个这样做的州。第一年有超过 160 家公司提交了通知，但没有一家勾选 AI 相关选项。Arvind Narayanan 和 Sayash Kapoor 是普林斯顿大学的 AI 学者，也是《AI Snake Oil》一书的作者，该书对 AI 炒作进行了批判性审视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arvind_Narayanan">Arvind Narayanan - Wikipedia</a></li>
<li><a href="https://engineering.princeton.edu/news/2025/01/13/ai-snake-oil-conversation-princeton-ai-experts-arvind-narayanan-and-sayash-kapoor">‘AI Snake Oil’: A conversation with Princeton AI experts Arvind Narayanan and Sayash Kapoor - Princeton Engineering</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#job displacement`, `#labor economics`

---

<a id="item-10"></a>
## [美国政府以安全为由要求 Anthropic 禁用两款 AI 模型](https://t.me/zaihuapd/41960) ⭐️ 8.0/10

美国商务部向 Anthropic 发出出口管制指令，要求其暂停任何外国公民在美国境内外访问 Fable 5 和 Mythos 5 AI 模型。作为回应，Anthropic 已关闭这两款模型对所有客户的访问，包括其外籍员工。 这标志着政府在 AI 模型访问方面的干预显著升级，为基于国家安全的出口管制树立了先例。它可能重塑 AI 公司全球部署模型的方式，并可能导致整个行业面临更严格的监管。 据报道，该指令源于对模型可能被越狱并带来安全风险的担忧。Anthropic 表示，其他 Claude 模型不受影响，公司正在争取尽快恢复访问。

telegram · zaihuapd · Jun 15, 08:55

**背景**: Fable 5 和 Mythos 5 是 Anthropic 最先进的 AI 模型，其中 Mythos 5 是顶级模型。美国政府越来越多地使用出口管制来限制敏感技术（尤其是 AI）向外国实体扩散。此举之前已有针对其他 AI 公司的类似措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/13/anthropic-disable-advanced-ai-models-us-government-order">Anthropic to disable its most advanced AI models after US order...</a></li>
<li><a href="https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/">Anthropic disables Fable and Mythos AI models following... | Fortune</a></li>
<li><a href="https://www.aljazeera.com/news/2026/6/13/us-orders-anthropic-to-disable-ai-models-for-all-foreign-nationals">US orders Anthropic to disable AI models for all foreign... | Al Jazeera</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export controls`, `#national security`, `#Anthropic`, `#AI safety`

---

<a id="item-11"></a>
## [Rio 3.5 模型被曝套壳中国开源模型](https://mp.weixin.qq.com/s/0oYevRBT8PPxG5hudOXxug) ⭐️ 8.0/10

此前被捧为开源 SOTA 的 Rio 3.5 模型被揭露为套壳模型，实为 Nex 和 Qwen 的混合产物，随后被下架，Rio 团队致歉。 该事件暴露了开源 AI 社区中严重的模型抄袭问题，损害了信任，并凸显了对声称的创新进行更好验证的必要性。 Nex 团队发现，去掉系统提示后，Rio 3.5 有 79% 的概率自称 Nex，权重分析显示共线性超过 0.98，混合比例约为 0.57 的 Nex 和 0.43 的 Qwen。

telegram · zaihuapd · Jun 15, 12:39

**背景**: Rio 3.5 是一个 3970 亿参数的混合专家模型，声称由里约热内卢市开发。Nex-N2-Pro 是中国 AI 实验室 Nex-AGI 于 2026 年 6 月初发布的开源模型，基于阿里巴巴的 Qwen3.5 构建。此次争议之前已有类似事件，如 Cursor 的 Composer 2 被曝实际为 Kimi，斯坦福团队的 Llama3-V 被指抄袭清华面壁的 MiniCPM-Llama3-V 2.5。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://iset-news.online/article/rio-de-janeiro-built-an-ai-model-that-beat-deepseek-but-was-based-on-someone-elses-work-nPTNdp">Rio de Janeiro Built an AI Model That Beat... — ISET-NEWS</a></li>
<li><a href="https://dev.to/jamilxt/rio-de-janeiros-homegrown-ai-was-someone-elses-model-with-a-new-name-jcb">Rio de Janeiro's 'Homegrown' AI Was Someone Else's Model Wit...</a></li>
<li><a href="https://huggingface.co/nex-agi/Nex-N2-Pro">nex -agi/ Nex -N2-Pro · Hugging Face</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#plagiarism`, `#model controversy`, `#LLM`

---

<a id="item-12"></a>
## [本地模型替代云端编程助手](https://news.ycombinator.com/item?id=48542100) ⭐️ 7.0/10

Hacker News 用户报告已完全用本地模型（如 Qwen3.6 和 Gemma）替代 Claude 和 GPT 等云端编程助手，在消费级硬件上实现高达每秒 150 token 的速度。 这一转变表明本地模型现已可用于日常编程，在保护隐私和节省成本的同时，对许多任务不牺牲性能，可能减少对昂贵云订阅的依赖。 用户报告使用 llama.cpp 搭配 Qwen3.6-35B-A3B-MTP 在双 RTX 3090 或 128GB RAM 的 Mac Studio 上运行，质量与 8-12 个月前的前沿模型相当。

hackernews · cloudking · Jun 15, 14:46

**背景**: 本地 LLM 在用户自己的硬件上运行，避免云成本和数据隐私问题。Ollama、llama.cpp 和 VSCode 的 Continue 扩展等工具简化了本地编程助手的设置。每秒 token 数（tok/s）衡量推理速度；150 tok/s 对本地模型来说算快。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/data-science-collective/how-to-build-your-own-llm-coding-assistant-with-qwen2-5-coder-b26aaadf071d">How to Build Your Own LLM Coding Assistant With... | Medium</a></li>
<li><a href="https://vasilkoff.com/blog/vscodium-and-ollama">VSCodium + Ollama: Local LLM Coding Setup Guide</a></li>
<li><a href="https://www.packetswitch.co.uk/using-the-continue-vscode-extension-and-local-llms-for-improved-coding/">How to Use Continue and Local LLMs for Better Coding in VSCode?</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为本地模型对大多数日常编程任务足够好，尽管不如顶级云模型聪明。一些人强调隐私和成本节省的重要性，另一些人则指出需要双 RTX 3090 等强大硬件。

**标签**: `#local LLM`, `#coding assistant`, `#privacy`, `#open source`

---

<a id="item-13"></a>
## [《指挥官基恩》引擎白皮书发布](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

一篇详细分析《指挥官基恩》游戏引擎的白皮书已发布，重点介绍了其在早期 PC 硬件上实现平滑滚动的技术创新。 这篇深度分析揭示了 id Software 使用的开创性技术，为后来定义行业的游戏如《德军总部 3D》和《毁灭战士》奠定了基础。 白皮书涵盖了自适应瓦片刷新（ATR）技术，该技术利用 EGA 的 CRTC 并行读取四个字节，从而在当时的有限硬件上实现了平滑滚动。

hackernews · mfiguiere · Jun 15, 17:52 · [社区讨论](https://news.ycombinator.com/item?id=48544781)

**背景**: 《指挥官基恩》是 id Software 在 1990 年代初期开发的一系列横向卷轴平台游戏。当时，PC 图形硬件（EGA）缺乏硬件精灵支持，使得平滑滚动成为一个重大挑战。自适应瓦片刷新技术是一种巧妙的软件解决方案，它在 VRAM 中构建虚拟屏幕并实现平滑滚动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Commander_Keen">Commander Keen - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Enhanced_Graphics_Adapter">Enhanced Graphics Adapter - Wikipedia</a></li>
<li><a href="https://ohtldr.com/summary/commander-keens-adaptive-tile-refresh/">Commander Keen ’s adaptive tile refresh – Oh TL;DR</a></li>

</ul>
</details>

**社区讨论**: 评论者对白皮书表示赞赏，有人推荐书籍《毁灭战士大师》以了解历史背景，还有人指出需要将 PC 硬件与 SNES 等主机进行比较才能理解这一成就。一位用户还提到了类似的分析如 Cosmodoc。

**标签**: `#game engine`, `#retro computing`, `#id Software`, `#technical deep-dive`

---

<a id="item-14"></a>
## [铜转运药物恢复记忆并清除阿尔茨海默病蛋白](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins) ⭐️ 7.0/10

莫纳什大学的研究人员发现，一种铜转运药物能够在阿尔茨海默病小鼠模型中恢复记忆并清除有毒的β-淀粉样蛋白。该药物已针对其他疾病进行过安全性评估，可能有助于快速推进人体试验。 这代表了阿尔茨海默病治疗的潜在突破，因为目前针对β-淀粉样蛋白的疗法在临床试验中大多失败。如果在人体中成功，可能为全球数百万患者提供新的治疗途径。 该药物通过恢复大脑中的铜稳态来促进β-淀粉样蛋白斑块的清除。然而，该研究仍处于临床前阶段，且对阿尔茨海默病的β-淀粉样蛋白假说仍存在质疑。

hackernews · bookofjoe · Jun 15, 14:48 · [社区讨论](https://news.ycombinator.com/item?id=48542132)

**背景**: 阿尔茨海默病以大脑中β-淀粉样蛋白斑块的积累为特征，这一标志物驱动了数十年的药物开发。然而，许多靶向β-淀粉样蛋白的药物未能显示出临床益处，引发了关于β-淀粉样蛋白是疾病原因还是结果的争论。铜失调也被认为与阿尔茨海默病病理有关，因此铜转运成为新的治疗靶点。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48542132">Copper transport drug restores memory and clears... | Hacker News</a></li>
<li><a href="https://vue-hackernews-ssr-5cavbdjcta-ew.a.run.app/item/48542132">Vue HN 2.0 | Copper transport drug restores memory and clears toxic...</a></li>
<li><a href="https://colab.ws/articles/10.1007/s00249-007-0235-2">Copper transport and Alzheimer ’ s disease | CoLab</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了谨慎乐观但也存在质疑。一些用户指出靶向β-淀粉样蛋白的疗法历史记录不佳，而另一些人则认为β-淀粉样蛋白斑块是真实存在的，可能仍然相关。一位评论者强调该药物仅在老鼠身上测试过，还需要人体试验。

**标签**: `#Alzheimer's`, `#copper transport`, `#amyloid-beta`, `#drug discovery`, `#neuroscience`

---

<a id="item-15"></a>
## [性格冲突导致 Anthropic 模型下线](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

Axios 报道称，Anthropic 与美国政府之间的性格冲突和幕后紧张关系导致了一项出口管制指令，迫使 Anthropic 为所有用户禁用其高级 AI 模型 Fable 和 Mythos。 这一事件凸显了人际动态和治理问题如何直接影响 AI 部署和国家安全政策，可能影响 Anthropic 的 IPO 前景以及更广泛的 AI 行业与监管机构的关系。 文章引用了熟悉政府和 Anthropic 的消息人士，指出一次“潜在的狭窄、非通用越狱”触发了政府回应，并且完美的越狱抵抗可能是不可能的。

rss · Simon Willison · Jun 15, 14:57

**背景**: Anthropic 是一家 AI 安全公司，开发了 Fable 和 Mythos 等高级模型。2026 年 6 月，美国政府发布出口管制指令，以国家安全为由要求 Anthropic 暂停向外国公民提供这些模型的访问权限。该公司遵守指令，为所有用户禁用了这些模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/13/anthropic-disable-advanced-ai-models-us-government-order">Anthropic to disable its most advanced AI models after US order...</a></li>
<li><a href="https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/">Anthropic disables Fable and Mythos AI models following... | Fortune</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 博客上的社区讨论对政府的理由表示怀疑，并指出 Anthropic 红队负责人的政治经验。评论者还质疑 Anthropic 是否解决了 2023 年的通用越狱攻击。

**标签**: `#Anthropic`, `#AI governance`, `#export controls`, `#policy`, `#AI safety`

---

<a id="item-16"></a>
## [字节跳动洽购天数智芯 AI 芯片，考虑百度昆仑芯](https://www.reuters.com/world/china/bytedance-talks-with-chinas-iluvatar-corex-purchase-ai-chips-sources-say-2026-06-15/) ⭐️ 7.0/10

字节跳动正与上海芯片公司天数智芯洽谈采购至少 5 万颗 AI 芯片，主要用于推理任务，并同时考虑引入百度昆仑芯。若交易达成，天数智芯将成为字节跳动继华为、寒武纪之后的第三大国产 GPU 供应商。 此举表明字节跳动在美国出口限制下战略性地减少对英伟达的依赖，并凸显中国本土 AI 芯片生态的日益成熟。该消息导致天数智芯股价上涨 12%。 这些芯片主要用于 AI 推理任务，而非训练。字节跳动还在评估百度昆仑芯作为额外选项。天数智芯开发用于 AI 的 GPGPU，而百度的昆仑 M100 和 M300 计划于 2026 和 2027 年推出。

telegram · zaihuapd · Jun 15, 06:53

**背景**: 字节跳动是 TikTok 的母公司，也是全球最大的 AI 芯片消耗者之一，主要使用英伟达 GPU。然而，美国出口管制限制了英伟达向中国销售先进芯片，促使中国科技公司寻求本土替代方案。天数智芯是一家总部位于上海的 AI 芯片初创公司，而百度的昆仑芯是自研 AI 加速器。华为和寒武纪已是字节跳动的主要国产 GPU 供应商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iluvatar_CoreX">Iluvatar CoreX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kunlunxin">Kunlunxin - Wikipedia</a></li>
<li><a href="https://www.chinadaily.com.cn/a/202511/14/WS69166bfba310d6866eb29629.html">Baidu unveils new Kunlun chips - Chinadaily.com.cn</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#ByteDance`, `#China tech`, `#semiconductors`, `#geopolitics`

---

<a id="item-17"></a>
## [消费者起诉 Anthropic 夸大 AI 订阅用量](https://www.wsj.com/tech/ai/anthropic-sued-over-limits-on-its-200-a-month-ai-plans-e2a109e4) ⭐️ 7.0/10

华盛顿特区消费者 Karl Kahn 对 Anthropic 提起集体诉讼，指控其每月 100 美元的 Max 5x 和每月 200 美元的 Max 20x 订阅计划未能提供宣传中的使用限额。 这是对 AI 订阅透明度最早的重大法律挑战之一，可能迫使公司明确披露使用上限，并在限额误导时向客户退款。 诉讼引用 Anthropic 在 2025 年 7 月的一封邮件作为证据，并要求为自 2024 年 4 月以来购买这些计划的用户退款。Anthropic 的帮助中心称 Max 计划每次会话提供 Pro 版 5 倍或 20 倍的使用量，但用户反映实际限额不明确且更低。

telegram · zaihuapd · Jun 15, 14:17

**背景**: Anthropic 提供 Claude Pro（每月 20 美元）和更高级别的 Max 计划（每月 100 美元和 200 美元），承诺提供 5 倍或 20 倍的使用量。然而，用户抱怨实际使用限额模糊且通常低于宣传，导致困惑和不满。这起诉讼凸显了消费者对 AI 订阅定价和透明度日益增长的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/11049741-what-is-the-max-plan">What is the Max plan? | Claude Help Center</a></li>
<li><a href="https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-pro-or-max-plan">Using Claude Code with your Pro or Max Plan | Anthropic Help Center</a></li>
<li><a href="https://blog.laozhang.ai/en/posts/claude-daily-limit">Claude Daily Limit in 2026: What Free, Pro, and Max Actually Reset</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#lawsuit`, `#AI subscription`, `#consumer protection`, `#transparency`

---