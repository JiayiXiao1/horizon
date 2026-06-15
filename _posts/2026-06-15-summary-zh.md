---
layout: default
title: "Horizon Summary: 2026-06-15 (ZH)"
date: 2026-06-15
lang: zh
---

> From 34 items, 17 important content pieces were selected

---

1. [Pyodide 314.0 支持直接将 WASM 轮子发布到 PyPI](#item-1) ⭐️ 9.0/10
2. [里约热内卢自称自研的大语言模型被揭露为加权合并模型](#item-2) ⭐️ 8.0/10
3. [Jane Street 谈形式化方法与 AI 代码](#item-3) ⭐️ 8.0/10
4. [JavaScript 的诞生与消亡（2014）演讲](#item-4) ⭐️ 8.0/10
5. [数据表明 AI 尚未取代软件工程师](#item-5) ⭐️ 8.0/10
6. [2026 年第一季度美国超 75 个数据中心项目被阻，总值 1300 亿美元](#item-6) ⭐️ 8.0/10
7. [华为开源盘古 2.0 模型，剑指全球第一](#item-7) ⭐️ 8.0/10
8. [美国政府要求 Anthropic 封禁两款 AI 模型](#item-8) ⭐️ 8.0/10
9. [全球地下真菌网络首张地图公布](#item-9) ⭐️ 8.0/10
10. [Adobe 过于严格的 EPUB 验证导致 Kobo 误报错误](#item-10) ⭐️ 7.0/10
11. [本地 ML 在 M1 Max 上索引 669GB GoPro 视频](#item-11) ⭐️ 7.0/10
12. [如何赚到十亿美元](#item-12) ⭐️ 7.0/10
13. [数据显示并非所有人都在广泛使用 AI](#item-13) ⭐️ 7.0/10
14. [将 SQLite 结果列映射回源表](#item-14) ⭐️ 7.0/10
15. [OpenRouter Fusion Router：半价实现 Claude 级智能](#item-15) ⭐️ 7.0/10
16. [克鲁格曼：马斯克是“人形庞氏骗局”，SpaceX 上市让普通投资者被迫买单](#item-16) ⭐️ 7.0/10
17. [澳大利亚青少年社交媒体禁令执行四个月成效不彰](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 支持直接将 WASM 轮子发布到 PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 允许 Python 包维护者使用 PEP 783 中定义的新 pyemscripten 平台标签，直接将 WebAssembly (WASM) 轮子发布到 PyPI。此前，Pyodide 维护者必须手动构建和托管超过 300 个包。 这消除了浏览器中 Python 的一个主要瓶颈，使更广泛的 Python 生态系统能够无需人工干预即可为 Pyodide 分发包。它显著减轻了 Pyodide 维护者的维护负担，并加速了新包的可用性。 该功能由 4 月 21 日合并到 PyPI 的 warehouse 仓库的 PR 支持。Simon Willison 通过发布 luau-wasm 包演示了该工作流程，该包可通过 micropip install 在 Pyodide 中安装。

rss · Simon Willison · Jun 13, 23:55

**背景**: Pyodide 是一个基于 WebAssembly 的浏览器和 Node.js 的 Python 发行版。PEP 783 为编译为 WebAssembly 的二进制 Python 包定义了 pyemscripten 平台标签。此前，分发此类包需要 Pyodide 维护者手动托管和维护。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging - Python Enhancement Proposals</a></li>

</ul>
</details>

**社区讨论**: 文章引用的 Hacker News 讨论显示出高度参与和积极情绪，许多用户对消除这一长期限制表示兴奋。一些评论者注意到更复杂的 Python 包在浏览器中运行的潜力。

**标签**: `#Pyodide`, `#WebAssembly`, `#Python`, `#PyPI`, `#package distribution`

---

<a id="item-2"></a>
## [里约热内卢自称自研的大语言模型被揭露为加权合并模型](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

一项调查揭露，里约热内卢自称自研的大语言模型 Rio-3.5-Open-397B 实际上是大约 60% 的 Nex-N2 Pro 和 40% 的 Qwen3.5-397B-A17B 的加权合并，并未进行额外训练。 这引发了对人工智能开发中透明度和归属问题的严重质疑，尤其是对于声称自主研发的公共部门项目。同时，它也凸显了模型合并这一日益增长的做法，这种做法可能模糊原创工作与衍生模型之间的界限。 Rio 模型中的每个权重张量在所有 60 层中，以数千个标准差的程度，都是 Nex 和 Qwen 的 0.6/0.4 混合。该模型被宣传为 Qwen3.5 的微调版本，但发布的版本并未应用任何蒸馏或训练。

hackernews · unrvl22 · Jun 14, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48528371)

**背景**: 模型合并是一种将两个或多个预训练模型的权重组合成一个模型的技术，无需额外训练，通常使用线性插值或 SLERP 等方法。它可以提高多任务性能，但当合并后的模型被呈现为原创作品时，会引发归属问题。里约热内卢市政府通过其 IT 公司 IplanRIO 发布了该模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2212.09849">[2212.09849] Dataless Knowledge Fusion by Merging Weights of Language Models</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**社区讨论**: 评论者就未披露是故意还是误解展开了辩论，一些人指出声称的改进可能来自未包含在上传模型中的策略蒸馏。其他人对缺乏适当归属表示失望，而少数人则对简单的权重线性组合能够在不降低性能的情况下提升表现感到惊讶。

**标签**: `#LLM`, `#open-source`, `#AI ethics`, `#model merging`, `#transparency`

---

<a id="item-3"></a>
## [Jane Street 谈形式化方法与 AI 代码](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street 发布了一篇博客文章，讨论形式化方法在编程中日益增长的重要性，尤其是在 AI 生成代码日益普及的背景下。文章强调形式化验证如何帮助应对验证瓶颈并提升代码质量。 这一讨论意义重大，因为它触及了现代软件工程中的一个关键挑战：确保 AI 生成代码的正确性。形式化方法可能将人类开发者的角色从编写代码转变为验证代码，从而可能改变软件开发生命周期。 这篇博客是 Jane Street 关于形式化方法系列文章的一部分，该公司以使用 OCaml 而闻名。文章指出，在使用 AI 代理编程时，类型已经很有价值，而更强大的证明技术可能带来更大的好处。

hackernews · eatonphil · Jun 14, 12:35 · [社区讨论](https://news.ycombinator.com/item?id=48526633)

**背景**: 形式化方法是基于数学的技术，用于规范、开发和验证软件与硬件系统。它们使用逻辑、类型理论和自动定理证明来确保正确性。Jane Street 是一家量化交易公司，长期以来一直倡导在生产中使用 OCaml 和形式化验证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1">Jane Street Blog - Formal methods and the future of programming</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>
<li><a href="https://users.ece.cmu.edu/~koopman/des_s99/formal_methods/">Formal Methods - Electrical and Computer Engineering</a></li>

</ul>
</details>

**社区讨论**: 社区评论反映了经验与怀疑的混合。一位评论者回忆了早期的证明自动化工具，如 Boyer-Moore 证明器；另一位指出形式化规范可能感觉像是用不同方式编写测试。还有一位评论者强调了形式化方法在帮助非英语母语者验证 AI 生成代码方面的潜力。

**标签**: `#formal methods`, `#programming`, `#verification`, `#AI`, `#software engineering`

---

<a id="item-4"></a>
## [JavaScript 的诞生与消亡（2014）演讲](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

Gary Bernhardt 在 2014 年 PyCon 上的演讲幽默地预测了 JavaScript 将演变为编译目标，并最终被 WebAssembly 和 TypeScript 取代，这一预测在很大程度上已成为现实。 该演讲的先见之明已被证实，影响了开发者对 JavaScript 角色及 Web 开发未来的思考。 演讲追溯了 JavaScript 从 1995 年到 2035 年的历史，融合了喜剧与严肃分析，并正确预见了 asm.js（后来的 WebAssembly）以及编译到 JS 的语言的兴起。

hackernews · subset · Jun 14, 12:38 · [社区讨论](https://news.ycombinator.com/item?id=48526661)

**背景**: JavaScript 于 1995 年诞生，最初是浏览器的简单脚本语言，但后来成为 Web 开发的主导语言。然而，其局限性催生了 TypeScript 等编译到 JS 的语言以及 WebAssembly 等替代运行时，使得其他语言也能在浏览器中运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript">The Birth & Death of JavaScript</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly/Guides/Rust_to_Wasm">Compiling from Rust to WebAssembly - WebAssembly | MDN</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该演讲的准确性，指出 JavaScript 确实成为了编译目标，WebAssembly 实现了预测。一些人还提到 Bernhardt 早期的“Wat”演讲是经典之作。

**标签**: `#JavaScript`, `#WebAssembly`, `#Programming Languages`, `#Tech Talk`, `#Prediction`

---

<a id="item-5"></a>
## [数据表明 AI 尚未取代软件工程师](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan 和 Sayash Kapoor 发表文章，认为数据不支持 AI 将导致软件工程大规模裁员的说法，并引用纽约 WARN 法案文件：第一年超过 160 家公司提交了通知，但没有一家勾选 AI 披露框。 这一基于证据的反驳挑战了 AI 导致失业的主流叙事，尤其是在被认为最易受自动化影响的行业中，并表明其他行业可能更有缓冲余地。 作者指出了软件工程中难以自动化的三个真正瓶颈：决定和明确要构建什么、验证并对交付物负责，以及对代码库、业务和环境的深度人类理解。

rss · Simon Willison · Jun 14, 23:54

**背景**: WARN 法案要求公司在大规模裁员前提前 60 天通知。2025 年 3 月，纽约成为美国第一个在 WARN 文件中添加 AI 披露复选框的州，询问技术创新或自动化是否导致了裁员。尽管普遍存在担忧，但第一年内没有公司勾选该框。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>
<li><a href="https://opentools.ai/news/new-yorks-ai-layoff-disclosure-law-0-compliance-shocking-revelations">New York's AI Layoff Disclosure Law: 0 Compliance, Shocking Revelations! | AI News</a></li>
<li><a href="https://www.softwareseni.com/why-ai-layoff-disclosure-laws-are-not-working-and-what-would-actually-fix-them/">Why AI Layoff Disclosure Laws Are Not Working and What Would Actually Fix Them - SoftwareSeni</a></li>

</ul>
</details>

**标签**: `#AI`, `#software engineering`, `#employment`, `#job displacement`, `#evidence-based`

---

<a id="item-6"></a>
## [2026 年第一季度美国超 75 个数据中心项目被阻，总值 1300 亿美元](https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs) ⭐️ 8.0/10

2026 年第一季度，美国全国至少有 75 个数据中心建设项目被阻止或推迟，总价值约 1300 亿美元，数量已与 2025 年全年持平。草根反对组织在三个月内从 396 个激增至 833 个，遍布 49 个州。 这一波反对浪潮标志着公众和政治情绪对数据中心扩张的重大转变，源于对能源成本飙升、水资源消耗和环境影响的担忧。它可能减缓人工智能基础设施的建设，并迫使行业采取更可持续的做法。 被阻项目总值约 1300 亿美元，活跃的草根反对组织达到 833 个，遍布 49 个州。各州议会提出了大量监管法案，部分联邦议员也提出了暂停数据中心建设的立法提案。

telegram · zaihuapd · Jun 14, 03:03

**背景**: 数据中心消耗大量电力和水资源，其快速扩张引发了对电网压力、电价上涨和环境退化的担忧。在美国，数据中心电力需求预计将大幅增长，促使地方和州层面出现两党反对。支持者认为担忧被夸大，数据中心能带来经济效益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs">More than 75 data center build-outs worth $130 billion have been successfully blocked in the first three months of 2026 — bipartisan opposition mounts nationwide over fears of soaring power and water costs | Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/06/130-billion-in-data-center-projects-blocked-by-protests-so-far-this-year/">$130 billion in data center projects blocked by protests so far this year - Ars Technica</a></li>
<li><a href="https://www.carbon-direct.com/insights/data-centers-and-their-energy-use-trends-in-state-capitals">Data centers and their energy use: Trends in state capitals | Carbon Direct</a></li>

</ul>
</details>

**标签**: `#data centers`, `#energy policy`, `#AI infrastructure`, `#regulation`, `#environment`

---

<a id="item-7"></a>
## [华为开源盘古 2.0 模型，剑指全球第一](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

在华为开发者大会 2026 上，华为宣布开源 openPangu 2.0 模型，包含 505B 参数的 Pro 版和 92B 参数的 Flash 版，支持 512K 上下文窗口。公司计划从 6 月 30 日起陆续开源预训练代码等七大组件。 此次发布标志着华为 AI 战略的重大进展，以完全开源、国产自研的大模型挑战 GPT-4 和 Llama 等全球领先者。它通过提供基于华为昇腾芯片和鸿蒙系统的高性能替代方案，强化了中国 AI 生态系统。 505B Pro 模型是全球最大的开源大语言模型之一，而 92B Flash 版本提供了更高效的选项。512K 上下文窗口可处理极长文档，如整本书籍或大型代码库。该模型针对华为昇腾 AI 芯片和鸿蒙系统进行了优化。

telegram · zaihuapd · Jun 14, 08:05

**背景**: 像 GPT-4 这样的大语言模型已经改变了 AI 领域，但大多数领先模型由美国公司开发，且需要昂贵的 NVIDIA GPU。华为的昇腾芯片是国产替代方案，openPangu 2.0 被设计为在该硬件上高效运行。512K 上下文窗口远大于典型模型（如 GPT-4 的 128K），使模型能一次性处理更多信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thamizhelango.medium.com/mindspore-zhipu-ai-huawei-ascend-how-china-built-a-frontier-ai-model-without-a-single-nvidia-68403d92cedb">MindSpore, Zhipu AI & Huawei Ascend : How China Built... | Medium</a></li>
<li><a href="https://www.bitrue.com/blog/huawei-ascend-ai-chip-specs-2025">Huawei Ascend AI Chips : Specifications, Models, and Performance in...</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1eplndh/what_is_the_current_largest_context_window_for_an/">What is the current largest context window for an open LLM? : r/LocalLLaMA - Reddit</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#large language model`, `#Huawei`, `#Pangu`

---

<a id="item-8"></a>
## [美国政府要求 Anthropic 封禁两款 AI 模型](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

美国政府以国家安全为由向 Anthropic 发出出口管制指令，要求该公司限制所有客户（包括外国员工）访问其 Fable 5 和 Mythos 5 AI 模型。Anthropic 已遵守指令，关闭了这两款模型的访问权限，其他 Claude 模型不受影响。 这标志着政府对先进 AI 模型的干预显著升级，为 AI 能力的出口管制开创了先例。它影响了依赖这些模型的企业和研究人员，并凸显了 AI 创新与国家安全之间日益紧张的局势。 该指令专门针对 Fable 5 和 Mythos 5，商务部担心模型被越狱后可能带来安全风险。Anthropic 表示正在尽快恢复访问，但目前所有客户（包括外国员工）均被封锁。

telegram · zaihuapd · Jun 14, 09:06

**背景**: Anthropic 的 Mythos 系列模型（包括 Mythos 5）专为高级网络安全任务设计，例如发现软件漏洞。Fable 5 是该系列中更安全、面向公众发布的版本。美国政府越来越多地使用出口管制来限制先进 AI 技术的获取，特别是防止对手获得相关能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.euronews.com/my-europe/2026/06/14/us-export-controls-on-anthropic-should-not-be-discriminatory-eu-commission-warns">US export controls on Anthropic 'should not be... | Euronews</a></li>
<li><a href="https://www.americanactionforum.org/insight/ai-export-controls-balancing-national-security-and-ai-innovation/">AI Export Controls : Balancing National Security and AI Innovation...</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#export control`, `#national security`, `#Anthropic`, `#AI safety`

---

<a id="item-9"></a>
## [全球地下真菌网络首张地图公布](https://insideclimatenews.org/news/11062026/earths-massive-underground-fungal-networks/) ⭐️ 8.0/10

地下网络保护协会（SPUN）的科学家首次绘制出全球丛枝菌根真菌网络地图，估计其总长度达 110 千万亿公里，总质量约为全人类体重的 5 倍。 这张地图揭示了地下真菌网络的巨大规模和碳储存能力，它们每年封存约 10 亿吨碳，凸显了其在减缓气候变化和维护生态系统健康中的关键作用。 地图显示，农田中的真菌密度仅为野生生态系统的一半，而拥有全球约 40%丛枝菌根真菌生物量的野生草原，正以森林 4 倍的速度转为农田。

telegram · zaihuapd · Jun 14, 14:58

**背景**: 丛枝菌根真菌与约 80%的陆生植物形成共生关系，延伸植物根系并帮助它们吸收水分和养分。这些真菌通过其庞大的地下网络储存碳，对气候调节具有重要意义。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.sciencenet.cn/htmlnews/2023/4/498730.shtm">地上地下搭起“通讯 网 ” 植物间交流无处不在—新闻—科学 网</a></li>
<li><a href="https://madechango.com/study-guide/view/2108">Threads of underground fungal networks are long enough to reach...</a></li>

</ul>
</details>

**标签**: `#ecology`, `#climate change`, `#mycology`, `#carbon sequestration`, `#research`

---

<a id="item-10"></a>
## [Adobe 过于严格的 EPUB 验证导致 Kobo 误报错误](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/) ⭐️ 7.0/10

一篇技术深度分析揭示，Adobe 的 EPUB 验证工具（基于 RMSDK）过于严格，将有效的 EPUB 文件标记为错误，导致 Kobo 设备上出现显示问题。 此问题影响依赖 Adobe 验证的 Kobo 用户，导致挫败感和时间浪费，同时也凸显了 Adobe 软件质量和 QA 实践的更广泛问题。 文章解释称，Adobe 的 RMSDK（Reader Mobile SDK）执行比 EPUB 标准更严格的规则，导致误报。解决方法包括使用 kepubify 或 PineNote 等替代设备。

hackernews · sohkamyung · Jun 14, 22:54 · [社区讨论](https://news.ycombinator.com/item?id=48533848)

**背景**: EPUB 是一种广泛使用的开放电子书标准。Adobe 的 RMSDK 是一种专有渲染引擎，被包括 Kobo 在内的许多电子阅读器使用。EPUBCheck 等验证工具检查是否符合标准，但 Adobe 的实现增加了额外检查，可能拒绝有效文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.epubconversion.com/epub-validator/">Free ePub validator | ePub checker | validate ePub format ebooks</a></li>
<li><a href="https://hmdpublishing.com/education/tools/epub-validator">Free EPUB Validator & Fixer Online — Check EPUB 2.0 & 3.0 Files</a></li>

</ul>
</details>

**社区讨论**: 评论者指出 Adobe 历来 QA 不佳，以 Flash 为例。一些人建议使用 kepubify 将 EPUB 转换为 Kobo 的原生格式，另一些人则推荐 PineNote 设备以获得更开放的软件。

**标签**: `#ePub`, `#Adobe`, `#Kobo`, `#ebooks`, `#software quality`

---

<a id="item-11"></a>
## [本地 ML 在 M1 Max 上索引 669GB GoPro 视频](https://news.ycombinator.com/item?id=48528029) ⭐️ 7.0/10

一位开发者使用开源机器学习模型在 M1 Max MacBook 上索引了 628 个 GoPro 视频（共 669 GB，超过 15 小时的素材），实现了搜索功能并自动将精彩片段编译到达芬奇时间线。 这表明强大的本地 AI 视频索引现在可以在消费级硬件上实现，提供了云服务无法比拟的隐私和离线能力，并为内容创作者和档案管理员开辟了新的工作流程。 该流水线以每秒 1 帧的速度处理，总共分析了 57,537 帧，总计算时间为 67 小时 40 分钟。它使用开源 ML 模型进行场景检测和语义搜索，并将选定的片段直接输出到达芬奇。

hackernews · iliashad · Jun 14, 15:13

**背景**: 传统上，视频索引需要手动标记或昂贵的云 AI 服务。本项目使用的本地 ML 模型完全在用户机器上运行，保护隐私并避免重复费用。M1 Max 的统一内存和神经网络引擎显著加速了这些工作负载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Machine_learning">Machine learning - Wikipedia</a></li>
<li><a href="https://www.creativeainews.com/blog/framedex-local-video-indexing-gemma-4-claude-code-2026/">Framedex: Local Video Indexing with Gemma 4 and Claude</a></li>
<li><a href="https://github.com/bryanrandell/DaVinci-Resolve-Timeline-Utility">GitHub - bryanrandell/ DaVinci - Resolve - Timeline -Utility: Switch quickly...</a></li>

</ul>
</details>

**社区讨论**: 评论者提到了类似项目（如 Framedex），并指出达芬奇 Resolve 21 已经内置了 AI 索引功能（IntelliSearch），但仅限于 Studio 版本。一些人质疑本地处理 67 小时与使用云加速的实用性，而另一些人则对本地 AI 视频工具表示热情。

**标签**: `#machine learning`, `#video indexing`, `#local AI`, `#GoPro`, `#M1 Max`

---

<a id="item-12"></a>
## [如何赚到十亿美元](https://paulgraham.com/earn.html) ⭐️ 7.0/10

保罗·格雷厄姆发表了一篇文章，认为赚到十亿美元需要大规模创造价值，通常通过解决实际问题的科技初创公司来实现。 这篇文章引发了关于极端财富创造的伦理和机制的讨论，影响了企业家和公众对十亿美元财富的看法。 该文章在 Hacker News 上获得了 452 个点赞和 1372 条评论，讨论质量参差不齐，包括关于财富攫取和道德语义的深刻反驳。

hackernews · kingstoned · Jun 14, 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48526360)

**背景**: 保罗·格雷厄姆是著名风险投资家和散文家，Y Combinator 的联合创始人。他的文章常探讨初创公司动态和财富创造。在此语境中，“赚取”一词存在争议，批评者认为十亿美元财富往往涉及攫取而非纯粹的价值创造。

**社区讨论**: 评论呈现分歧：一些人捍卫格雷厄姆的价值创造论点，而另一些人则认为十亿美元财富本质上涉及剥削或对“赚取”一词的语义操纵。少数用户幽默地计算极端增长场景以说明这一概念。

**标签**: `#wealth creation`, `#startups`, `#entrepreneurship`, `#economics`, `#Paul Graham`

---

<a id="item-13"></a>
## [数据显示并非所有人都在广泛使用 AI](https://gabrielweinberg.com/p/people-are-consuming-ai-like-they) ⭐️ 7.0/10

一篇文章指出，尽管 AI 功能强大，但许多人并未广泛使用它，引用数据显示超过 50%的受访者每周使用 AI 不到一次。 这挑战了主流的 AI 炒作叙事，揭示了感知与实际采用之间的差距，对产品设计、工作场所政策和投资策略具有影响。 文章利用调查数据和个人轶事表明，AI 的使用并非普遍，许多人仍然依赖传统方法或很少使用 AI。

hackernews · yegg · Jun 14, 14:44 · [社区讨论](https://news.ycombinator.com/item?id=48527700)

**背景**: 自 2022 年底 ChatGPT 发布以来，人们普遍猜测 AI 正在迅速改变工作和日常生活。然而，实际采用数据往往落后于炒作，许多用户仍然对如何有效整合 AI 持怀疑或不确定态度。

**社区讨论**: 评论者分享了不同的体验：有些人认为 AI 在监督下很有帮助，另一些人则感到使用 AI 的压力或担心被落下。一个关键见解是，AI 的采用可能更多通过现有软件中的嵌入式功能增长，而非独立的聊天界面。

**标签**: `#AI adoption`, `#technology trends`, `#workplace`, `#LLMs`, `#skepticism`

---

<a id="item-14"></a>
## [将 SQLite 结果列映射回源表](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 7.0/10

Simon Willison 探索了将 SQL 查询结果列程序化映射回其源 table.column 的方法，使用 Claude Code (Opus 4.8) 通过 APSW、ctypes 和 EXPLAIN 分析找到了解决方案。 这项技术可以使 Datasette 为任意 SQL 查询结果添加列来源信息，从而改善用户对数据的理解和调试能力。 解决方案包括使用 APSW 库、通过 ctypes 访问 SQLite 的 sqlite3_column_table_name() C 函数，以及解析 EXPLAIN 输出来推断列来源。

rss · Simon Willison · Jun 13, 23:05

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的工具。列来源指的是识别每个结果列来自哪个表和列，SQLite 的 Python 接口本身并不直接提供此信息。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/">Research: Mapping SQLite result columns back to their source `table.column`</a></li>
<li><a href="https://docs.datasette.io/en/stable/sql_queries.html">Running SQL queries - Datasette documentation</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#Datasette`, `#SQL`, `#AI-assisted development`, `#column provenance`

---

<a id="item-15"></a>
## [OpenRouter Fusion Router：半价实现 Claude 级智能](https://x.com/i/status/2065856853989270011) ⭐️ 7.0/10

OpenRouter 推出了 Fusion Router（openrouter/fusion），这是一个多模型协商系统，通过并行调用模型和共识分析，以大约一半的成本实现了与 Claude Fable 相当的智能水平。 这一创新可能大幅降低高质量 AI 推理的成本，使开发者和企业更容易获得先进智能，并可能重塑整个行业的 LLM 路由策略。 Fusion Router 的工作方式是：主模型在必要时调用一组模型并行作答，然后由裁判模型比较它们的回答，生成结构化分析（共识、矛盾等）。成本约为单次完成的 4-5 倍，且内部调用不会递归触发。

telegram · zaihuapd · Jun 14, 01:21

**背景**: OpenRouter 是一个提供统一访问各种大语言模型（LLM）的平台。Fusion Router 通过启用多模型协商扩展了这一功能，多个模型协作生成更可靠的答案。这种方法类似于机器学习中的集成方法，但应用于 LLM 推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/docs/guides/routing/routers/fusion-router">Fusion Router | Multi-model AI... | OpenRouter | Documentation</a></li>
<li><a href="https://openrouter.ai/docs/guides/features/plugins/fusion">Fusion | Multi-model AI Analysis with... | OpenRouter | Documentation</a></li>
<li><a href="https://writingmate.ai/models/openrouter/fusion">OpenRouter : Fusion - AI Model Details | Writingmate</a></li>

</ul>
</details>

**标签**: `#LLM`, `#OpenRouter`, `#model routing`, `#AI inference`, `#multi-model`

---

<a id="item-16"></a>
## [克鲁格曼：马斯克是“人形庞氏骗局”，SpaceX 上市让普通投资者被迫买单](https://paulkrugman.substack.com/p/elon-musk-human-ponzi-scheme) ⭐️ 7.0/10

诺贝尔经济学奖得主保罗·克鲁格曼发表评论文章，认为埃隆·马斯克未能兑现的承诺构成了“人形庞氏骗局”，而 SpaceX 以 1.77 万亿美元估值上市，加上指数规则调整，将迫使普通投资者通过指数基金被动买入。 这位知名经济学家的批评凸显了被动投资和高调私营公司估值可能造成的市场扭曲，可能影响公众对指数基金机制以及远见企业家问责制的讨论。 据报道，SpaceX 去年收入仅 187 亿美元且仍处于亏损状态，但其 IPO 估值高达 1.77 万亿美元。纳斯达克 100 和富时罗素等指数提供商近期修改规则，允许 SpaceX 快速纳入成分股，这意味着追踪指数的基金必须买入其股票。

telegram · zaihuapd · Jun 14, 04:52

**背景**: 庞氏骗局是一种欺诈性投资模式，用新投资者的资金支付早期投资者的回报，而非来自合法利润。指数基金被动跟踪市场指数，当一只股票被纳入主要指数时，所有跟踪该指数的基金都必须买入，无论价格高低。这种机制可能推高估值，迫使普通投资者持有被高估的股票。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8tx0ZbKkemQ">tech.ifeng.com/c/8tx0ZbKkemQ</a></li>
<li><a href="https://money.udn.com/money/story/5599/9556737">被 動 基 金 搶進 SpaceX ... | 經濟日報</a></li>
<li><a href="https://xueqiu.com/6943090400/381595097?scene=1036&share_uid=6943090400">xueqiu.com/6943090400/381595097?scene=1036&share_uid...</a></li>

</ul>
</details>

**标签**: `#Elon Musk`, `#SpaceX`, `#Ponzi scheme`, `#index funds`, `#tech criticism`

---

<a id="item-17"></a>
## [澳大利亚青少年社交媒体禁令执行四个月成效不彰](https://t.me/zaihuapd/41955) ⭐️ 7.0/10

Molly Rose Foundation 的调查显示，澳大利亚针对 16 岁以下青少年的社交媒体禁令生效四个月后，61% 的 12 至 15 岁受访者仍拥有活跃账号，其中 TikTok、YouTube 和 Instagram 保留了超过 52% 的原有未成年用户。 这揭示了澳大利亚社交媒体监管的重大执行漏洞，凸显了基于年龄的限制措施的困难以及加强平台问责的必要性，对全球类似政策具有借鉴意义。 约 60% 的受访青少年反映平台未采取任何注销或限制措施，许多人还使用 VPN 绕过禁令，削弱了法律的有效性。

telegram · zaihuapd · Jun 15, 01:02

**背景**: 澳大利亚于 2024 年通过法律，禁止 16 岁以下儿童访问社交媒体，旨在保护未成年人免受网络伤害。Molly Rose Foundation 是在 14 岁少女 Molly Russell 因社交媒体内容自杀后成立的，致力于推动更安全的网络环境。VPN 通过隐藏用户 IP 地址来绕过地理限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Molly_Rose_Foundation">Molly Rose Foundation</a></li>
<li><a href="https://www.alwaysvpn.com/guides/where-vpns-illegal-banned">Where Are VPNs Illegal or Banned ? | AlwaysVPN</a></li>

</ul>
</details>

**标签**: `#social media regulation`, `#Australia`, `#teen online safety`, `#platform governance`, `#VPN`

---