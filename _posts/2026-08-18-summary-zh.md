---
layout: default
title: "Horizon Summary: 2026-08-18 (ZH)"
date: 2026-08-18
lang: zh
---

> From 38 items, 22 important content pieces were selected

---

1. [Mojo 编程语言以 Apache 2 协议开源](#item-1) ⭐️ 9.0/10
2. [Turbovec：Google TurboQuant 的 Rust 向量搜索实现](#item-2) ⭐️ 8.0/10
3. [内存价格一年暴涨 500%，128GB DDR5 售价达 3399 美元](#item-3) ⭐️ 8.0/10
4. [Linux 7.3 提升 VRAM 超卖性能](#item-4) ⭐️ 8.0/10
5. [Qwen 3.8 27B 在智能指数上媲美 GPT-5.6](#item-5) ⭐️ 8.0/10
6. [AirTag 追踪稀有书籍货运至亚马逊 AI 训练设施](#item-6) ⭐️ 8.0/10
7. [中国要求政府机构提前卸载定制版 Windows 10](#item-7) ⭐️ 8.0/10
8. [亚马逊搜索广告：对消费者的隐性税](#item-8) ⭐️ 7.0/10
9. [火车当平板扫描仪：创意狭缝扫描摄影](#item-9) ⭐️ 7.0/10
10. [Cursor 推出 Origin，面向 AI 代理的 GitHub 替代品](#item-10) ⭐️ 7.0/10
11. [用 20 美元工具修复变砖的 Framework 笔记本](#item-11) ⭐️ 7.0/10
12. [基于 O'Reilly 书籍的 Polars 速查表发布](#item-12) ⭐️ 7.0/10
13. [数据中心废热使周边气温升高 0.8°C](#item-13) ⭐️ 7.0/10
14. [耶鲁研究：全民健康覆盖每年可节省 1 万亿美元并挽救 11.4 万生命](#item-14) ⭐️ 7.0/10
15. [意大利因苹果滥用 App Store 主导地位罚款 1.15 亿美元](#item-15) ⭐️ 7.0/10
16. [宇树科技科创板 IPO 进入询价阶段，拟募资 42 亿元](#item-16) ⭐️ 7.0/10
17. [苹果带摄像头 AirPods 进入设计验证测试](#item-17) ⭐️ 7.0/10
18. [iOS 27 Beta 5 为 Apple 智能中国版预埋设备端处理机制](#item-18) ⭐️ 7.0/10
19. [企业微信 5.0.10 开放 CLI 与 MCP，支持 AI Agent 集成](#item-19) ⭐️ 7.0/10
20. [中国对境外保单收益征收 20%税，汇丰保诚股价大跌](#item-20) ⭐️ 7.0/10
21. [国产 AI 芯片 2026 年将占中国市场近 90%](#item-21) ⭐️ 7.0/10
22. [Telegram 申请 .gram 域名，为用户提供个性化二级域名](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Mojo 编程语言以 Apache 2 协议开源](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular 已将 Mojo 编程语言及其编译器和工具链以宽松的 Apache 2.0 许可证开源，紧随其 1.0 版本的发布。这兑现了 2023 年 5 月做出的开源承诺。 此次开源对 AI/ML 社区来说是一个重要里程碑，因为 Mojo 旨在结合类似 Python 的语法与系统级性能和 GPU 支持。这可能会加速其采用，促进社区贡献，并扩大围绕该语言的生态系统。 Mojo 基于 MLIR 编译器框架构建，能够针对 CPU、GPU、TPU 和其他加速器。最初成为 Python 超集的目标已于 2025 年 8 月放弃，Mojo 现在是一种独立的语言，尽管它保留了受 Python 启发的语法。

rss · Simon Willison · Aug 18, 21:39

**背景**: Mojo 是由 Modular 公司开发的系统编程语言，于 2023 年 5 月首次发布。它旨在结合 Python 的易用性与 C/C++ 和 Rust 的性能，利用 MLIR 实现高级编译器优化。Apache 2.0 许可证是一种宽松的开源许可证，允许用户以最少的限制使用、修改和分发代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language) - Wikipedia</a></li>
<li><a href="https://www.apache.org/licenses/LICENSE-2.0">Apache License, Version 2.0 | Apache Software Foundation</a></li>
<li><a href="https://pypi.org/project/mojo-compiler/">mojo-compiler · PyPI</a></li>

</ul>
</details>

**社区讨论**: Lobste.rs 上的社区讨论普遍对开源表示兴奋和赞同，一些人注意到偏离 Python 超集兼容性的转变。还有关于对 AI 开发的影响以及与其他语言（如 Rust 和 Julia）的比较的讨论。

**标签**: `#Mojo`, `#open source`, `#programming language`, `#AI/ML`, `#compiler`

---

<a id="item-2"></a>
## [Turbovec：Google TurboQuant 的 Rust 向量搜索实现](https://github.com/RyanCodrai/turbovec) ⭐️ 8.0/10

Turbovec 是一个新的 Rust 库，实现了 Google 的 TurboQuant 算法，用于高效的向量搜索，承诺在大规模索引中显著节省内存并提升速度。据报道，它仅用 4GB 内存即可处理 1000 万篇文档，从而加快反向索引构建并使开发过程更顺畅。 这很重要，因为它将最先进的量化技术引入 Rust 生态系统，可能为本地、隐私优先的应用甚至通过 WASM 在浏览器中使用提供更高效、更易用的向量搜索。这也凸显了将研究中的先进算法应用于实用开源工具的趋势。 Turbovec 使用 Rust 构建，旨在兼容类似 FAISS 的工作流，社区对 SQLite 绑定和 WASM 编译感兴趣。然而，一些评论者指出 FAISS 已不再是 SOTA，且像 Qdrant 这样的成熟解决方案已集成 TurboQuant，质疑该库的新颖性和采用准备度。

hackernews · fittingopposite · Aug 18, 18:07 · [社区讨论](https://news.ycombinator.com/item?id=49349898)

**背景**: TurboQuant 是 Google Research 提出的向量量化算法，将在 ICLR 2026 上展示，可将嵌入向量压缩 5-8 倍，同时保持 95% 以上的召回率。它采用两阶段过程：首先优化 MSE 的向量量化器，然后对残差应用 1 位量化器以实现无偏内积估计。该算法旨在减少大型语言模型和向量搜索引擎的内存开销，在 NVIDIA H100 GPU 上可实现至少 6 倍的内存减少和高达 8 倍的注意力计算加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/TurboQuant">TurboQuant - Wikipedia</a></li>
<li><a href="https://research.google/blog/turboquant-redefining-ai-efficiency-with-extreme-compression/">TurboQuant: Redefining AI efficiency with extreme compression</a></li>
<li><a href="https://arxiv.org/abs/2504.19874">[2504.19874] TurboQuant: Online Vector Quantization with Near ... TurboQuant: Redefining AI efficiency with extreme compression GitHub - Firmamento-Technologies/TurboQuant: Near-optimal ... TurboQuant: Online Vector Quantization with Near-optimal ... TurboQuant - Wikipedia GitHub - RecursiveIntell/turbo-quant: Rust implementation of ... TurboQuant: 3-Bit KV Cache via PolarQuant + QJL (ICLR 2026)</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人对内存节省和本地/WASM 使用的潜力感到兴奋，而另一些人则质疑其新颖性，因为 FAISS 已不再是 SOTA，且 Qdrant 已集成 TurboQuant。还有人要求提供更易读的文档以促进采用。

**标签**: `#vector search`, `#Rust`, `#quantization`, `#ANN`, `#TurboQuant`

---

<a id="item-3"></a>
## [内存价格一年暴涨 500%，128GB DDR5 售价达 3399 美元](https://www.tomshardware.com/pc-components/ram/memory-prices-climb-500-percent-in-12-months-up-to-10x-the-lowest-ever-tracked-prices-128gb-of-ddr5-now-usd3-399) ⭐️ 8.0/10

过去 12 个月内存价格暴涨 500%，128GB DDR5 套件现价超过 3399 美元，是最低记录价格的 10 倍。此次涨价归因于 AI 驱动的需求和供应限制。 此次价格暴涨对消费者、PC 组装者和整个电子行业产生重大影响，可能使许多人无法负担内存升级。这也引发了对永久性涨价以及 AI 需求对硬件市场影响的担忧。 价格上涨不仅影响 DDR5，还波及 DDR4，由于对旧平台需求增加，DDR4 价格已上涨 120-180%。显示器面板制造商也因组件成本上升而提价，表明电子产品价格呈普遍上涨趋势。

hackernews · haunter · Aug 17, 17:52 · [社区讨论](https://news.ycombinator.com/item?id=49334960)

**背景**: 内存价格受供需动态影响，AI 数据中心消耗了大量 DRAM 和 NAND 产能，导致消费级、PC 和企业级市场出现短缺和价格飙升。历史上，内存价格具有周期性，但当前涨势由持续的 AI 需求驱动，可能导致更持久的涨价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/ram/memory-prices-climb-500-percent-in-12-months-up-to-10x-the-lowest-ever-tracked-prices-128gb-of-ddr5-now-usd3-399">Memory prices climb 500% in 12 months, up to... | Tom's Hardware</a></li>
<li><a href="https://www.ftcelectronics.com/news/ddr5-prices-remain-on-the-rise-ai-demand-and-supply-constraints-continue-to-reshape-the-memory-marke">DDR 5 Prices Continue to Rise as AI Demand Keeps Supply Tight</a></li>
<li><a href="https://www.aroged.com/2026/08/17/rammageddon-has-arrived-ram-prices-have-soared-to-crazy-heights-128-gb-ddr5-costs-3399/">RAMmageddon has arrived: RAM prices have soared to... - Aroged</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了沮丧和怀疑，用户计划推迟硬件升级，并质疑制造商是否利用 AI 需求抬高价格。一些人分享了被建议尽早购买内存的经历，而另一些人则担心涨价的持久性以及对需要更换内存的用户的影响。

**标签**: `#hardware`, `#memory prices`, `#DDR5`, `#market trends`, `#AI demand`

---

<a id="item-4"></a>
## [Linux 7.3 提升 VRAM 超卖性能](https://pixelcluster.dev/VRAM-Overcommit/) ⭐️ 8.0/10

Linux 内核 7.3 引入了针对 VRAM 超卖场景的性能改进，使系统在视频内存耗尽时能更优雅地处理。由 Valve Linux 图形团队的 Natalie Vock 编写的补丁已合并到上游，并计划在 Linux 7.3 中发布。 这一改进对 Linux 游戏和 GPU 密集型工作负载意义重大，尤其是在 VRAM 有限的系统上。它减少了 VRAM 耗尽时的性能损失，使 Linux 成为依赖 GPU 的游戏玩家和专业人士更可行的平台。 内核补丁专注于改进驱逐策略以及 GPU 驱动与内存子系统之间的协调。这项工作是为完善 VRAM 管理而持续努力的一部分，未来的内核可能会在这些更改的基础上进一步发展。

hackernews · flaburgan · Aug 18, 07:51 · [社区讨论](https://news.ycombinator.com/item?id=49342719)

**背景**: VRAM（视频随机存取存储器）是 GPU 上用于存储纹理、帧缓冲和其他图形数据的专用内存。当 VRAM 满时，系统必须将数据驱逐到系统 RAM，这可能导致显著的性能下降。Linux 内核 7.3 包含改进驱逐处理方式的补丁，减少了性能影响。该工作是 Linux 内核中更广泛的 DRM（直接渲染管理器）内存管理子系统的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.osnews.com/story/145846/beyond-the-limits-of-physical-vram/">Beyond the limits of physical VRAM – OSnews</a></li>
<li><a href="https://pixelcluster.dev/VRAM-Overcommit/">VRAM Management Part 2: Beyond the Limits of Physical VRAM | pixelcluster's GPU blog</a></li>
<li><a href="https://www.phoronix.com/news/Linux-7.3-Improving-vRAM-Mgmt">Linux 7.3 To Land Initial Code Improving vRAM Management , More...</a></li>

</ul>
</details>

**社区讨论**: 社区普遍对这一改进持积极态度，用户对即将发布的版本表示兴奋。一些使用 Nvidia 硬件的用户指出，Nvidia 不支持分页，这限制了改进的收益。还有关于内核在内存分配中的角色以及碎片整理潜力的讨论，以及对开发者工作的赞赏。

**标签**: `#Linux kernel`, `#VRAM`, `#memory management`, `#performance`, `#open source`

---

<a id="item-5"></a>
## [Qwen 3.8 27B 在智能指数上媲美 GPT-5.6](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

阿里巴巴的开源模型 Qwen 3.8 27B（270 亿参数）在 Artificial Analysis 智能指数上获得 52 分，与 GPT-5.6 Luna（max）持平，仅比 GLM-5.2（753B）和 DeepSeek V4 Pro（1.7T）低 1 分。 这一里程碑表明，小型高效的开源模型能够与规模大得多的专有模型相抗衡，可能使高性能 AI 更加普及，并减少对庞大计算资源的依赖。 Artificial Analysis 智能指数汇总了涵盖数学、科学、编码和推理的九项挑战性评估。Qwen 3.8 27B 采用 Apache 2.0 许可证，支持视觉，专为高效通用文本生成和智能体工作负载而设计。

rss · Simon Willison · Aug 17, 23:58

**背景**: Artificial Analysis 智能指数是一个综合基准，用于全面衡量 AI 能力。Qwen 3.8 27B 是阿里巴巴 Qwen 系列的一部分，该系列以发布功能强大的开源模型而闻名。其前代 Qwen 3.6 27B 已经令人印象深刻，新模型延续了这一趋势，并展现出卓越的效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://simonwillison.net/2026/Aug/16/qwen-38-27b/">Qwen 3.8 27B is excellent, but it defaults to wildly ...</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（通过链接引用）可能强调该模型的效率和开源特性，用户对能在本地运行如此强大的模型表示兴奋。一些人可能会讨论该指数的有效性或与其他基准的比较。

**标签**: `#AI`, `#LLMs`, `#Qwen`, `#open-source`, `#model-efficiency`

---

<a id="item-6"></a>
## [AirTag 追踪稀有书籍货运至亚马逊 AI 训练设施](https://simonwillison.net/2026/Aug/17/we-tracked-a-shipment-of-rare-books-it-ended-at-an-amazon-ai-tra/) ⭐️ 8.0/10

404 Media 在稀有书籍中藏入 Apple AirTag，追踪了从 Biblio 卖家发出的大约 1000 本书的订单，该订单被送至拉斯维加斯亚马逊 LAS8 设施的 VGT3 区域。亚马逊员工的在线论坛讨论证实，VGT3 对大量书籍进行破坏性扫描以用于 AI 训练。 这项调查提供了具体证据，证明来自匿名、对价格不敏感的客户的大宗书籍订单确实被用于 AI 训练数据，证实了书商界长期以来的怀疑。它凸显了围绕未经许可使用受版权保护的书籍训练 AI 模型的持续版权和伦理争议。 这本书被送至亚马逊 LAS8 设施的 VGT3 区域，入口处展示了一个恐龙持书的标志，象征破坏性扫描。AirTag 追踪依赖 Apple 的 Find My 网络，该网络利用附近的 Apple 设备报告位置，而非 GPS。

rss · Simon Willison · Aug 17, 15:21

**背景**: 一段时间以来，书商报告收到来自匿名客户的大宗订单，这些客户对价格不敏感，被广泛怀疑是 AI 公司为获取训练数据而扫描书籍。2025 年 6 月，Simon Willison 报道了 Anthropic 的书籍扫描活动。AirTag 是小型蓝牙追踪器，利用 Apple 的 Find My 网络定位物品，而 Biblio 是二手和稀有书籍的市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AirTag">AirTag - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Biblio.com">Biblio.com - Wikipedia</a></li>
<li><a href="https://www.biblio.com/company/about-biblio">About Biblio Booksearch and Marketplace - Biblio</a></li>

</ul>
</details>

**标签**: `#AI training data`, `#copyright`, `#investigative journalism`, `#Amazon`, `#books`

---

<a id="item-7"></a>
## [中国要求政府机构提前卸载定制版 Windows 10](https://www.bloomberg.com/news/articles/2026-08-18/china-axing-microsoft-windows-from-state-agencies-ahead-of-plan) ⭐️ 8.0/10

中国国家安全部已要求部分政府机构卸载定制版 Windows 10（神州网信政府版），比原定 2027 年 2 月的停用日期提前数月，理由是数据安全担忧。 此举表明数据安全审查加强，并加速中国减少对外国技术的依赖，可能影响微软的政府业务和全球科技供应链。 定制版 Windows 10 由微软与中国电子科技集团合资的 C&M Information Technologies 开发，原定于 2027 年 2 月退役。微软表示未发现影响该产品的安全事件，且该产品仍在定期获得安全更新。

telegram · zaihuapd · Aug 18, 06:22

**背景**: 定制版 Windows 10，即“Windows 10 神州网信政府版”，是为满足中国政府安全需求而开发，此前因后门担忧，Windows 8 被禁止用于政府电脑。此次提前停用反映了中国持续减少对外国软件的依赖并应对数据安全风险的努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.zaobao.com.sg/news/china/story20260819-9539834">中国据悉提前停用政府机构定制款Windows 10 | 联合早报</a></li>
<li><a href="https://www.chaincatcher.com/article/2283501">中国据报提前停用政府定制版 Windows 10 操作系统，原支持计划提前终止｜中国, Windows 10 - ChainCatcher</a></li>
<li><a href="https://www.gate.com/zh/news/detail/china-accelerates-removal-of-government-customized-windows-10-pulling-23530316">中国加速淘汰政府定制版 Windows 10，将停用日期提前数月</a></li>

</ul>
</details>

**标签**: `#China`, `#Microsoft`, `#Windows 10`, `#data security`, `#government policy`

---

<a id="item-8"></a>
## [亚马逊搜索广告：对消费者的隐性税](https://seths.blog/2026/08/the-amazon-tax/) ⭐️ 7.0/10

Seth Godin 的文章认为，亚马逊的赞助搜索结果对消费者而言是一种“税”，优先展示付费广告而非更优产品。讨论中提到了潜在的法律行动，包括商标侵权和欺诈指控。 这一批评凸显了广告对电商平台日益增长的影响，影响消费者信任和购买决策。它引发了对亚马逊市场公平性和透明度的质疑，可能促使监管审查和广告实践的变革。 文章指出，亚马逊的 A9 算法将销售速度作为主要排名因素，赞助广告可以提升自然排名。社区成员建议按“畅销榜”排序以避开广告，并讨论了新产品在没有广告的情况下难以突围的问题。

hackernews · herbertl · Aug 18, 13:22 · [社区讨论](https://news.ycombinator.com/item?id=49345263)

**背景**: 亚马逊市场是一个占主导地位的电商平台，赞助产品通常出现在搜索结果顶部。广告已成为亚马逊的重要收入来源，其 A9 算法优先考虑销售速度高的产品，而广告驱动的销售可以影响这一指标。这引发了广告可能掩盖更相关或更高质量产品的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://salesduo.com/blog/amazon-ad-types-guide/">Amazon Ad Types & Formats: The Complete 2026 Guide (All 4 Explained)</a></li>
<li><a href="https://www.adbadger.com/blog/amazon-advertising-what-does-sponsored-mean-on-amazon/">What Does "Sponsored" Mean on Amazon? A Complete Guide | Ad Badger</a></li>
<li><a href="https://www.brookings.edu/articles/what-is-a-digital-ad-tax/">What is a digital ad tax? | Brookings</a></li>

</ul>
</details>

**社区讨论**: 社区讨论大多批评亚马逊的广告做法，有人建议对商标侵权和欺诈采取法律行动。其他人指出广告是常见的商业模式，但亚马逊的主导地位使其问题更大。一些用户分享了实用技巧，如按“畅销榜”排序以避开广告，并讨论了新卖家面临的挑战。

**标签**: `#Amazon`, `#advertising`, `#e-commerce`, `#consumer behavior`, `#economics`

---

<a id="item-9"></a>
## [火车当平板扫描仪：创意狭缝扫描摄影](https://philo.gay/linecam/) ⭐️ 7.0/10

一个创意项目利用火车的移动和固定相机产生平板扫描仪效果，连续捕捉风景图像。该项目在 philo.gay/linecam/ 上有详细介绍，并在 Hacker News 上获得了 378 分和 58 条评论的显著社区关注。 该项目展示了一个巧妙且低成本的技巧，重新利用日常技术（火车和相机）来创造独特的艺术图像。它与创客和摄影社区产生共鸣，激发类似的实验，并凸显了技术与艺术的交汇点。 该技术本质上是狭缝扫描摄影，火车的运动提供了扫描移动。根据火车速度，生成的图像具有独特的拉伸或压缩外观，进行中的扫描本身也被视为艺术作品。

hackernews · otherayden · Aug 18, 12:43 · [社区讨论](https://news.ycombinator.com/item?id=49344825)

**背景**: 狭缝扫描摄影是一种技术，通过使用窄缝将移动图像曝光到传感器或胶片上，从而创建场景的时间扭曲表示。在这个项目中，火车的运动充当扫描机制，固定相机捕捉连续的像素线，这些像素线被拼接在一起形成最终图像。这种方法类似于平板扫描仪的工作原理，即传感器在文档上移动以逐行捕获图像。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=49344825">Using the railway network as a flatbed scanner | Hacker News</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映出强烈的热情和共同经验。几位用户提到他们做过的类似项目，例如 2008 年与 Ward Cunningham 一起进行的狭缝扫描设置，以及手动拼接帧的动画技术。其他人分享了诸如 slitscan.space 之类的工具，并表示受到启发尝试类似的实验，其中一位用户提议在锯木厂进行木纹直播。

**标签**: `#computer vision`, `#creative coding`, `#hardware hack`, `#photography`, `#side project`

---

<a id="item-10"></a>
## [Cursor 推出 Origin，面向 AI 代理的 GitHub 替代品](https://cursor.com/changelog/origin-code-hosting) ⭐️ 7.0/10

Cursor 推出了 Origin，这是一个专为 AI 代理设计的全新 Git 托管和代码审查平台，目前对付费计划开放早期测试版。该平台于 2026 年 6 月 16 日在 Compile 活动上发布，由 Graphite 背后的团队打造。 Origin 标志着 Cursor 从 AI 代码编辑扩展到代码托管领域的重要一步，可能挑战 GitHub 的主导地位。同时，它也引发了关于中心化和信任的讨论，尤其是考虑到 Cursor 归 Elon Musk 所有，这引发了开发者对数据隐私和控制的担忧。 Origin 被描述为“代理时代的 Git 锻造厂”，是首个从一开始就围绕 AI 代理设计的托管平台。目前处于早期测试阶段，对 Cursor 付费计划开放，并提供更广泛访问的等待名单。

hackernews · tomasreimers · Aug 17, 17:02 · [社区讨论](https://news.ycombinator.com/item?id=49334209)

**背景**: 像 GitHub 和 GitLab 这样的 Git 托管平台是用于存储和协作代码的中心化服务。去中心化替代方案如 Radicle 和联邦式 Forgejo 提供了更多控制和抗审查能力。Cursor 以其 AI 驱动的代码编辑器而闻名，现在通过 Origin 进入这一领域，旨在将 AI 代理更深入地集成到开发工作流中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cursor.com/origin">Cursor · Origin</a></li>
<li><a href="https://apidog.com/blog/cursor-origin/">What Is Cursor Origin ? The Git Hosting Platform Built for AI Agents...</a></li>
<li><a href="https://www.learncursor.dev/learn/cursor-origin">Cursor Origin : Git Hosting Built for AI Agents · Learn Cursor</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀疑和担忧，用户质疑使用 Musk 拥有的平台进行代码托管的明智性，并提到隐私和信任问题。一些人建议使用去中心化替代方案，如 Radicle 或 Forgejo，而另一些人则对 GitHub 的现状表示遗憾。Origin 的开发者 Tomas 表示愿意回答问题，这表明团队有一定程度的参与。

**标签**: `#code hosting`, `#GitHub alternative`, `#Cursor`, `#decentralization`, `#Musk`

---

<a id="item-11"></a>
## [用 20 美元工具修复变砖的 Framework 笔记本](https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/) ⭐️ 7.0/10

一名用户仅用价值 20 美元的工具成功修复了因 BIOS 更新失败而变砖的 AMD 7040 系列 Framework 13 笔记本电脑。修复过程涉及使用编程器直接刷写 BIOS 芯片，而 Framework 官方并未提供此操作文档。 这凸显了 BIOS 更新失败的普遍问题以及制造商在恢复支持方面的缺失，引发了关于责任和维修权的讨论。它强调了文档和低成本维修选项对消费者的重要性，可能影响行业实践和消费者权益讨论。 作者使用了 CH341A 编程器和 SOIC-8 夹子，花费约 20 美元，直接刷写 BIOS 芯片。修复对象是 AMD 7040 系列 Framework 13，作者指出 Framework 未提供官方恢复文档，尽管维修协会强调文档是维修权的重要支柱。

hackernews · jp_sc · Aug 18, 13:18 · [社区讨论](https://news.ycombinator.com/item?id=49345220)

**背景**: BIOS 更新对安全性和稳定性至关重要，但失败可能导致设备“变砖”，无法使用。许多制造商缺乏官方恢复流程，迫使用户寻求第三方解决方案或丢弃设备。维修权运动倡导制造商提供文档和零件以支持维修。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://quantum5.ca/2026/08/16/fixing-bricked-amd-7040-series-framework-13-laptop-with-20-tools/">Fixing a bricked AMD 7040 series Framework 13” laptop with $20 tools</a></li>
<li><a href="https://community.frame.work/t/solved-framework-unresponsive-after-bios-update/75181">[Solved] - Framework Unresponsive After BIOS Update</a></li>
<li><a href="https://blog.adafruit.com/2026/08/18/fixing-a-bricked-framework-laptop/">Fixing a bricked Framework laptop - Adafruit Industries</a></li>

</ul>
</details>

**社区讨论**: 评论者对制造商表示不满，分享了类似经历，并呼吁采取法律行动或延长保修期。一些人后悔购买 Framework，因为零件市场缺乏且库存问题，而另一些人则强调 BIOS 更新失败的普遍性以及需要更好的支持。

**标签**: `#hardware`, `#repair`, `#BIOS`, `#Framework`, `#consumer rights`

---

<a id="item-12"></a>
## [基于 O'Reilly 书籍的 Polars 速查表发布](https://opensource.posit.co/resources/cheatsheets/polars/) ⭐️ 7.0/10

《Python Polars：权威指南》的作者将这本近 500 页的书籍压缩成了一份两页的速查表，提供 PDF 和无障碍 HTML 两种版本。该速查表为常见的 Polars 操作提供了快速参考。 这份速查表为数据从业者提供了实用资源，可能降低采用 Polars 的门槛。Polars 是一个高性能的 DataFrame 库，解决了 pandas 的局限性。这反映了社区对 Polars 作为数据分析现代替代品的兴趣日益增长。 该速查表是“高度有损”压缩，省略了书中的许多细节，但旨在涵盖最常用的操作。除了 PDF 版本外，还提供了无障碍 HTML 版本，作者欢迎就遗漏的操作或组织方式提供反馈。

hackernews · jeroenjanssens · Aug 18, 13:38 · [社区讨论](https://news.ycombinator.com/item?id=49345476)

**背景**: Polars 是一个用于 Python 的 DataFrame 库，旨在提高速度和效率，利用 Rust 和惰性求值在大数据集上优于 pandas。它作为 pandas 的现代替代品而广受欢迎，pandas 在处理大数据时常常面临性能和内存问题。该速查表基于 O'Reilly 书籍《Python Polars：权威指南》，该书是 Polars 库的全面参考。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacamp.com/tutorial/python-polars-tutorial-complete-guide-for-beginners">Python Polars Tutorial: A Complete Guide for Beginners | DataCamp</a></li>
<li><a href="https://realpython.com/polars-python/">Python Polars: A Lightning-Fast DataFrame Library – Real Python</a></li>
<li><a href="https://docs.pola.rs/user-guide/getting-started/">Getting started - Polars user guide</a></li>

</ul>
</details>

**社区讨论**: 社区反应总体积极，用户在看到速查表后表示有兴趣尝试 Polars，尤其是那些来自 R 或 data.table 背景的用户。一些用户指出了小烦恼，例如'pl.col()'语法的冗长，而另一些用户则表示他们已经转向 DuckDB。总体而言，讨论突出了速查表的实用性以及 Polars 与其他数据工具之间的持续比较。

**标签**: `#Polars`, `#Python`, `#Data Analysis`, `#Cheatsheet`, `#Data Science`

---

<a id="item-13"></a>
## [数据中心废热使周边气温升高 0.8°C](https://asmedigitalcollection.asme.org/sustainablebuildings/article/7/2/024501/1233035/Data-Center-Waste-Heat-as-an-Emerging-Urban) ⭐️ 7.0/10

发表在 ASME《可持续建筑杂志》上的现场测量显示，数据中心使下风向邻近地区的气温升高约 0.8°C，影响范围延伸至设施外约 500 米。 这一实证证据量化了数据中心的局部热影响，随着 AI 和云计算推动数据中心快速扩张，这一影响日益重要。它凸显了一个日益严重的环境问题，可能影响城市规划和可持续性法规。 研究测得迎风侧平均气温约为 42.7°C，而在园区东边界下风向升至 43.5°C。观测到的约 0.8°C 的升温延伸至下风向约 500 米处，但搜索窗口为 500-1000 米。

hackernews · cwwc · Aug 18, 17:24 · [社区讨论](https://news.ycombinator.com/item?id=49349147)

**背景**: 数据中心消耗大量电力，其中大部分转化为必须散发的热量。这些废热可能加剧城市热岛效应，即城市地区比周边农村地区更热。以往研究多关注废热回收用于区域供暖，但直接测量局部温度影响的研究很少。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencedirect.com/science/article/pii/S1364032123006342">Waste heat recoveries in data centers: A review - ScienceDirect</a></li>
<li><a href="https://en.wikipedia.org/wiki/Urban_heat_island">Urban heat island - Wikipedia</a></li>
<li><a href="https://www.businesstoday.in/technology/story/ai-data-centres-are-heating-the-planet-and-millions-may-feel-it-523363-2026-03-31">AI data centres are heating the planet and millions... - BusinessToday</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论呈现两极分化：一些评论者对问题的严重性表示怀疑，而另一些人则感叹缺乏客观辩论。少数人指出测得的升温幅度较小且局部化，还有人质疑为何数据中心比炼油厂等其他污染行业更受关注。

**标签**: `#data centers`, `#environmental impact`, `#urban heat`, `#sustainability`, `#research`

---

<a id="item-14"></a>
## [耶鲁研究：全民健康覆盖每年可节省 1 万亿美元并挽救 11.4 万生命](https://ysph.yale.edu/news-article/universal-health-coverage-could-save-one-trillion-dollars-and-114000-lives-every-year/) ⭐️ 7.0/10

耶鲁大学的一项研究估计，在美国实施全民健康覆盖每年可节省 1 万亿美元并挽救 11.4 万人的生命。该研究结果于近期发布，引发了广泛讨论。 这项研究为长期争论的政策提供了具体的经济和生命价值估算，可能影响公众舆论和关于医疗改革的政策讨论。它凸显了系统性变革的潜在益处，对政策制定者、医疗服务提供者和公众都有影响。 1 万亿美元的数字来自 1.3 万亿美元的成本节省减去为更多人提供保险而增加的 3040 亿美元支出。节省来自五个方面：降低药品价格、按医疗保险水平向提供者支付、减少行政开销、减少欺诈性账单以及减少可避免的急诊和住院。

hackernews · karakoram · Aug 17, 15:49 · [社区讨论](https://news.ycombinator.com/item?id=49332981)

**背景**: 全民健康覆盖（UHC）意味着所有人都能获得所需的医疗服务而不遭受经济困难。美国医疗体系在发达国家中独特，依赖私人保险且成本高昂，这引发了关于改革的持续辩论。这项研究通过量化潜在的节省和挽救的生命，为证据基础增添了内容。

**社区讨论**: 社区评论对研究的假设和政治可行性表示怀疑。一些人认为，从低效中获利的强大利益集团会抵制变革，而另一些人则呼吁首先实现透明的定价。少数人指出，类似的研究在 ACA 之前也出现过，但面临强烈反对，这表明此类提议可能更像是竞选口号而非可实现的政策。

**标签**: `#healthcare`, `#policy`, `#economics`, `#US`

---

<a id="item-15"></a>
## [意大利因苹果滥用 App Store 主导地位罚款 1.15 亿美元](https://t.me/zaihuapd/43243) ⭐️ 7.0/10

意大利反垄断机构 AGCM 因苹果通过其应用跟踪透明度（ATT）政策滥用 App Store 中的主导地位，对其处以 1.15 亿美元罚款。苹果强烈反对该决定，称监管机构忽视了 ATT 带来的隐私保护好处。 该裁决凸显了监管机构对苹果 App Store 做法及其隐私政策的日益关注，可能影响全球其他反垄断案件。它强调了隐私措施与数字市场竞争公平性之间的紧张关系。 AGCM 指控苹果单方面对开发者施加 ATT 规则，要求他们显示跟踪提示，而苹果自身的应用却无需显示。该机构表示，该政策与苹果声称的隐私目标不成比例，损害了商业伙伴的利益。

telegram · zaihuapd · Aug 17, 12:50

**背景**: 应用跟踪透明度（ATT）由苹果于 2021 年 4 月在 iOS 14.5 中引入，要求应用在跨其他应用和网站跟踪用户前征求用户许可。该政策一直存在争议，批评者认为它虽然有利于用户隐私，但给了苹果不公平的优势。意大利反垄断机构 AGCM 以在数字市场执行竞争规则而闻名，此前曾因类似滥用行为对亚马逊处以罚款。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://apiko.com/blog/app-tracking-transparency-what-data-do-apps-collect-why/">App Tracking Transparency : what Data do Apps Collect and why</a></li>
<li><a href="https://developer.apple.com/documentation/apptrackingtransparency">App Tracking Transparency | Apple Developer Documentation</a></li>
<li><a href="https://www.linkedin.com/pulse/amazon-fined-italian-antitrust-authority-end-digital-carmelo-cennamo">Amazon fined by the Italian Antitrust Authority . Is this the end of...</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Apple`, `#App Store`, `#privacy`, `#regulation`

---

<a id="item-16"></a>
## [宇树科技科创板 IPO 进入询价阶段，拟募资 42 亿元](https://t.me/zaihuapd/43244) ⭐️ 7.0/10

2026 年 8 月 5 日，宇树科技科创板 IPO 进入初步询价阶段，询价时间为 9:30 至 15:00。公司拟募资 42.02 亿元，发行新股 4044.64 万股，占发行后总股本的 10%，市场预估发行价约 104 元/股，对应市值将超过 400 亿元。 此次 IPO 是宇树科技作为中国最知名的机器人独角兽之一的重要里程碑，反映了投资者对机器人和 AI 公司日益增长的兴趣。成功上市可能为仿人机器人的进一步研发和商业化提供大量资金，可能加速行业发展。 网上、网下申购将于 8 月 10 日开启，8 月 12 日缴款截止。招股书显示，宇树科技 2025 年营收 16.99 亿元、净利润 2.78 亿元；公司预计 2026 年上半年营收为 10.52 亿至 11.28 亿元。

telegram · zaihuapd · Aug 17, 13:20

**背景**: 科创板是上海证券交易所的科技创新板，采用注册制，类似于纳斯达克，面向科技公司。宇树科技是领先的机器人公司，以四足机器人和仿人机器人（如 H1 和 R1）闻名，并为其 R1 仿人机器人部署了 NVIDIA 全栈机器人技术。IPO 询价阶段是注册制流程中的关键步骤，机构投资者提交指示性价格以确定最终发行价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.unitree.com/">Unitree Robotics | Robot Dog_Quadruped_Humanoid Robotics Company</a></li>
<li><a href="https://eu.36kr.com/zh/p/3419294583000457">eu.36kr.com/zh/p/3419294583000457</a></li>
<li><a href="https://m.gelonghui.com/p/6095164">云深处 IPO ：“ 机 器狗”起家，喝得上 机 器人“热汤”吗</a></li>

</ul>
</details>

**标签**: `#IPO`, `#Unitree`, `#robotics`, `#finance`, `#STAR Market`

---

<a id="item-17"></a>
## [苹果带摄像头 AirPods 进入设计验证测试](https://t.me/zaihuapd/43247) ⭐️ 7.0/10

据彭博社报道，苹果带摄像头的 AirPods 已进入设计验证测试（DVT）阶段，原型机接近定型。摄像头位于左右耳机，用于为 Siri 提供视觉信息，而非用于拍照或录像。 这标志着苹果在推出集成 AI 和计算机视觉的新型可穿戴设备方面迈出了重要一步，有望增强 Siri 的上下文感知能力。这反映了苹果将 AI 功能融入日常设备的整体战略，但 Siri 的 AI 质量延迟可能导致上市时间推迟。 该产品原定最早于今年上半年发售，但因新版 Siri 延迟而推后。如果苹果对视觉 AI 功能的质量仍不满意，上市时间还可能继续后移。摄像头不用于拍照或录像。

telegram · zaihuapd · Aug 18, 02:00

**背景**: 设计验证测试（DVT）是硬件开发中的一个阶段，在量产前对设计进行最终确定并验证其是否符合规格。它位于工程验证测试（EVT）之后、生产验证测试（PVT）之前。据传，苹果带摄像头的 AirPods 旨在为 Siri 提供视觉信息，使其能够识别物体或周围环境，从而在日常场景中更加实用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Engineering_validation_test">Engineering validation test - Wikipedia</a></li>
<li><a href="https://embeddedartistry.com/fieldmanual-terms/design-validation-test/">Design Validation and Test [DVT] - Embedded Artistry</a></li>
<li><a href="https://superintelligencenews.com/ai-fields/large-language-models/camera-airpods-apples-siri-gamble-explained/">Camera AirPods : Apple ’s Siri gamble explained</a></li>

</ul>
</details>

**标签**: `#Apple`, `#AirPods`, `#wearables`, `#AI`, `#hardware`

---

<a id="item-18"></a>
## [iOS 27 Beta 5 为 Apple 智能中国版预埋设备端处理机制](https://t.me/zaihuapd/43248) ⭐️ 7.0/10

iOS 27 beta 5 被发现已预埋中国版 Apple 智能的相关说明，强调用户请求全部在设备端处理，不会发送给苹果或安全机制提供商。这表明 Apple 智能在中国的落地已进入适配阶段。 这一进展意义重大，表明苹果正在积极调整其 AI 套件以符合中国法规，同时保持其注重隐私的策略。这可能为 Apple 智能在中国的正式推出铺平道路，影响数百万 iPhone 用户及该地区的 AI 生态系统。 预埋文案提到，根据法律要求，苹果会收集匿名的安全结果并以聚合形式共享，安全机制也将自动下载更新。这表明将涉及本地安全合作伙伴，很可能是阿里巴巴的通义千问，据报道该模型已被选为中国版模型。

telegram · zaihuapd · Aug 18, 02:16

**背景**: Apple 智能是苹果的 AI 功能套件，在其他地区依赖 OpenAI 的 ChatGPT 等模型。然而，ChatGPT 在中国大陆被屏蔽，因此苹果需要获得许可的本地模型。报道称，阿里巴巴的通义千问已获得中国网信办批准，苹果在阿里巴巴的帮助下训练了自己的 AI 模型，以遵守当地内容和数据规则。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.remio.ai/post/apple-intelligence-china-approval-clears-a-path-for-qwen-integration-but-the-launch-is-not-finished">Apple Intelligence China Approval Clears a Path for Qwen Integration...</a></li>
<li><a href="https://www.theverge.com/ai-artificial-intelligence/980160/apple-intelligence-china-custom-ai-model-alibaba">Apple trained its own AI model for China with help from... | The Verge</a></li>
<li><a href="https://felloai.com/apple-intelligence-china/">Apple Intelligence in China: Powered by Alibaba's Qwen</a></li>

</ul>
</details>

**标签**: `#Apple`, `#iOS`, `#AI`, `#Privacy`, `#China`

---

<a id="item-19"></a>
## [企业微信 5.0.10 开放 CLI 与 MCP，支持 AI Agent 集成](https://mp.weixin.qq.com/s/uJf57P15-FQL_u6jLHiGYA) ⭐️ 7.0/10

企业微信 5.0.10 版本面向所有企业开放了 CLI 与 MCP 能力，使 WorkBuddy、DeepSeek Harness 和企业自建 Agent 可以直接调用 10 大核心办公模块。该更新还包含权限隔离、关键操作人工审批、限时授权和完整审计等安全功能。 此次更新意义重大，因为企业微信是中国广泛使用的企业平台，通过 MCP 和 CLI 等标准协议让 AI Agent 接入其核心办公模块，有望简化工作流程并提高生产力。同时，这也为企业软件采用开放的 AI 集成标准并保持安全控制树立了先例。 这 10 大办公模块包括文档和表格读取、数据分析，以及生成提案 PPT 或经营看板。安全模型支持人与 AI 的权限隔离、关键操作的人工审批、限时授权和完整审计日志。

telegram · zaihuapd · Aug 18, 06:22

**背景**: 模型上下文协议（MCP）是 Anthropic 于 2024 年 11 月推出的开放标准，用于将 AI 模型连接到外部工具和数据源，并已成为 AI Agent 集成的事实标准。CLI（命令行界面）提供了一种可脚本化的方式让软件与系统交互，常用于企业自动化。企业微信（WeCom）是腾讯的企业通讯与协作平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://learn.microsoft.com/en-us/azure/developer/ai/intro-agents-mcp">Build Agents using Model Context Protocol on Azure</a></li>
<li><a href="https://dev.to/x4nent/complete-guide-to-mcp-model-context-protocol-in-2026-architecture-implementation-and-4a11">Complete Guide to MCP (Model Context Protocol) in 2026 ...</a></li>
<li><a href="https://github.com/loonghao/wecom-bot-mcp-server">GitHub - loonghao/wecom-bot-mcp-server: A Python server ...</a></li>

</ul>
</details>

**标签**: `#WeChat Work`, `#MCP`, `#AI integration`, `#enterprise software`, `#CLI`

---

<a id="item-20"></a>
## [中国对境外保单收益征收 20%税，汇丰保诚股价大跌](https://t.me/zaihuapd/43253) ⭐️ 7.0/10

据财新报道，中国税务机关已开始对境外保单收益（包括香港保单）征收 20%的个人所得税。此举导致汇丰、保诚和渣打股价大幅下跌，其中保诚在伦敦一度下跌 13%。 这一监管举措对跨境保险和金融市场产生重大影响，尤其冲击依赖中国大陆访客赴港购险的保诚、友邦等保险公司。此举表明中国对境外资产的税收征管趋严，可能重塑投资流向和离岸保险行业。 该税项适用于香港保单收益，包括股息派发及预缴保费利息，北京和杭州已开始执行。6 月初已有部分银行暂停为中国大陆客户开立可用于海外投资的香港账户，投行富瑞称该消息引发保诚“投资者恐慌”。

telegram · zaihuapd · Aug 18, 07:30

**背景**: 中国个人所得税法要求居民对全球所得纳税，包括利息、股息及境外投资收益。然而，对境外保单收益的征管历来较为宽松，许多大陆居民赴港购买保险以获取更高回报和更广保障。此次执法填补了这一漏洞，与更广泛的境外资产监控和征税努力一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://t.me/KatyushaUnion/8544">肃反委员会 – Telegram</a></li>
<li><a href="https://shanghai.chinatax.gov.cn/xwdt/ztzl/zcgll/grsdsggzl/rdwt/202004/P020200402600133658053.pdf">shanghai.chinatax.gov.cn/xwdt/ztzl/zcgll/grsdsggzl/rdwt/202004...</a></li>
<li><a href="https://m.haiwaimoney.com/h-nd-3940.html">一文读懂： 香 港 保 险要不要交 税</a></li>

</ul>
</details>

**标签**: `#China`, `#taxation`, `#insurance`, `#financial markets`, `#regulation`

---

<a id="item-21"></a>
## [国产 AI 芯片 2026 年将占中国市场近 90%](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinas-homegrown-ai-accelerators-to-supply-90-percent-of-the-countrys-domestic-market-analysts-suggest-cambricon-and-huawei-expected-to-be-the-biggest-winners-in-the-shift-away-from-nvidia-and-amd) ⭐️ 7.0/10

TrendForce 预测，到 2026 年，中国本土 AI 加速器将占据国内市场的近 90%，高于去年的 45%。寒武纪和华为预计将成为最大受益者，其中华为在 2025 年已出货 81.2 万颗，占据 20.3%的市场份额。 这一转变标志着中国在 AI 芯片领域显著减少对英伟达和 AMD 的依赖，反映了其在美国出口管制下推动半导体自给自足的努力。这可能会重塑全球 AI 芯片市场，并影响主要参与者的竞争格局。 2025 年，英伟达以 220 万颗的出货量占据中国市场的 55%，而华为出货 81.2 万颗。为实现 2026 年的目标，中国需要在一年内将高端 AI 芯片产量提升 2.2 倍至约 196 万颗，这引发了关于产能能否跟上的疑问。

telegram · zaihuapd · Aug 18, 13:03

**背景**: 中国一直在加速发展本土半导体产业，以减少对外国技术的依赖，尤其是在美国对先进 AI 芯片实施出口管制之后。寒武纪常被比作英伟达，专注于 AI 芯片和 GPGPU，近期实现盈利，收入激增 4400%，凸显了中国 AI 芯片独立战略的成功。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://insights.trendforce.com/p/china-high-end-ai-chip-autonomy">China's Aggressive Push for High-End AI Chip Autonomy</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cambricon_Technologies">Cambricon Technologies - Wikipedia</a></li>
<li><a href="https://hellochinatech.com/p/cambricon-china-ai-chip-turning-point">Cambricon and China’s AI Chip Turning Point: From Losses to ...</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#China`, `#Huawei`, `#Cambricon`, `#semiconductor industry`

---

<a id="item-22"></a>
## [Telegram 申请 .gram 域名，为用户提供个性化二级域名](https://t.me/zaihuapd/43262) ⭐️ 7.0/10

Telegram 已向 ICANN 申请 .gram 顶级域名。若获批，其 10 亿用户可获得如 durov.gram 的个性化二级域名，并可通过单个提示词创建由 Telegram 托管的互动网站。 此举可能使 Telegram 对新的域名空间拥有重大控制权，可能改变用户建立网络身份和托管内容的方式。这也凸显了平台申请自有顶级域名以增强用户参与度和生态整合的趋势。 该申请需遵循 ICANN 严格的新 gTLD 流程，包括财务和法律承诺。作为 TLD 运营商，Telegram 将控制注册局并制定二级域名政策，但需遵守与 ICANN 的合同。

telegram · zaihuapd · Aug 18, 17:44

**背景**: ICANN 管理全球域名系统，并定期开放新通用顶级域名（gTLD）的申请轮次。TLD 运营商控制扩展名下的注册局，从而决定二级地址的政策。这与 .com 或 .org 的运营方式类似，但对社区型或品牌特定域名具有更大的灵活性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://domainnamewire.com/2026/08/18/telegram-gram-top-level-domain/">Telegram applies for .gram top level domain name</a></li>
<li><a href="https://thearabianpost.com/telegram-seeks-gram-domain-for-user-web-identities/">Telegram seeks .gram domain for user web identities</a></li>
<li><a href="https://x.com/durov/status/2089770867576172804">Pavel Durov on X: "Telegram has applied for the .gram domain ...</a></li>

</ul>
</details>

**标签**: `#Telegram`, `#domain`, `#ICANN`, `#web`, `#announcement`

---