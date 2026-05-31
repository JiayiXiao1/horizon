---
layout: default
title: "Horizon Summary: 2026-05-31 (ZH)"
date: 2026-05-31
lang: zh
---

> From 36 items, 18 important content pieces were selected

---

1. [vLLM v0.22.0：DeepSeek V4 强化、MRv2、Rust 前端](#item-1) ⭐️ 8.0/10
2. [微软将永久授权 Office 降级为只读模式](#item-2) ⭐️ 8.0/10
3. [领域专长才是真正的竞争优势](#item-3) ⭐️ 8.0/10
4. [埃森哲以 12 亿美元收购 Ookla，强化网络 AI 能力](#item-4) ⭐️ 8.0/10
5. [Zig ELF 链接器进展迈向 C 语言替代](#item-5) ⭐️ 8.0/10
6. [OpenRouter 完成 1.13 亿美元 B 轮融资](#item-6) ⭐️ 8.0/10
7. [Anthropic 详解 Claude 跨产品沙箱技术](#item-7) ⭐️ 8.0/10
8. [通过 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](#item-8) ⭐️ 8.0/10
9. [蓝色起源新格伦火箭静态点火测试爆炸](#item-9) ⭐️ 8.0/10
10. [SpaceX 获 41.6 亿美元美军卫星合同](#item-10) ⭐️ 8.0/10
11. [华为提出“韬定律”：以时间缩微替代几何缩微](#item-11) ⭐️ 8.0/10
12. [Voxel Space 算法详解](#item-12) ⭐️ 7.0/10
13. [Openrsync：OpenBSD 的安全 rsync 实现](#item-13) ⭐️ 7.0/10
14. [教宗利奥首道通谕批判技术救世主义](#item-14) ⭐️ 7.0/10
15. [Chad Whitacre 因 AI 退出科技行业](#item-15) ⭐️ 7.0/10
16. [Datasette 1.0a31 新增写入查询和存储查询功能](#item-16) ⭐️ 7.0/10
17. [骑手过剩：2000 万骑手仅需 400 万](#item-17) ⭐️ 7.0/10
18. [Codex 现已支持跨设备远程控制](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.22.0：DeepSeek V4 强化、MRv2、Rust 前端](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 8.0/10

vLLM v0.22.0 对 DeepSeek V4 进行了重大强化，推动 Model Runner V2 走向默认，并增加了实验性的 Rust 前端。该版本包含来自 230 位贡献者的 459 次提交。 此版本显著增强了对 DeepSeek V4 和 Qwen3 等前沿模型的支持，而 Model Runner V2 则提供了更简洁、更高效的推理核心。实验性的 Rust 前端可能为生产部署带来更好的性能和安全性。 DeepSeek V4 获得了 NVFP4 融合 MoE 支持、CUDA graph 完整/分段模式以及 MTP 推测解码。Model Runner V2 现在会自动为 Qwen3 密集模型选择，并在存在 KV 连接器时回退到 MRv1。

github · khluu · May 29, 10:28

**背景**: vLLM 是一个高吞吐量、内存高效的大型语言模型推理引擎。Model Runner V2 是对核心执行路径的彻底重写，旨在更加模块化和高效。NVFP4 是 NVIDIA 的一种 4 位浮点格式，可在保持精度的同时减少内存使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/v0.10.2/api/vllm/model_executor/layers/quantization/utils/nvfp4_moe_support.html">nvfp4_moe_support - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>

</ul>
</details>

**标签**: `#LLM inference`, `#vLLM`, `#DeepSeek`, `#open source`, `#performance`

---

<a id="item-2"></a>
## [微软将永久授权 Office 降级为只读模式](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

微软宣布，自 2026 年 7 月 13 日起，由于需要安全证书更新而旧版本无法支持，永久授权的 Office 2019 和 2021 for Mac 将切换为只读模式。 此举实质上撤销了之前购买的永久授权的核心功能，破坏了传统上对无限期离线使用的承诺，并推动用户转向 Microsoft 365 订阅。 只读模式允许用户打开和阅读文件，但禁止编辑、打印或创建新文档。该变更适用于 Mac 上的 Word、Excel、PowerPoint、Outlook 和 OneNote。

hackernews · antipurist · May 30, 23:26 · [社区讨论](https://news.ycombinator.com/item?id=48341578)

**背景**: 永久授权允许用户一次性购买后无限期使用软件，而订阅则需要持续付费。微软一直在从永久授权转向基于订阅的 Microsoft 365，此举被视为朝该方向迈出的又一步。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cpl.thalesgroup.com/software-monetization/perpetual-vs-subscription-licenses">Perpetual License vs. Subscription Model: Long-Term Effects on Revenue</a></li>
<li><a href="https://talk.tidbits.com/t/office-2019-switching-to-view-only-mode-what-to-do/33495">Office 2019 switching to view-only mode—what to do?</a></li>
<li><a href="https://learn.microsoft.com/en-us/answers/questions/5637995/i-bought-office-but-excel-and-word-shows-view-only">I bought office but excel and word shows view only</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈反对，用户称这一变更非法，并指出盗版版本可能更尊重原始合同。一些人推测加速的时间线是由 AI 实验室在代理中使用离线 Office 所驱动，促使微软推动订阅许可。

**标签**: `#Microsoft`, `#licensing`, `#software`, `#Office`, `#consumer rights`

---

<a id="item-3"></a>
## [领域专长才是真正的竞争优势](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 8.0/10

一篇博客文章认为，领域专长而非 AI 熟练度才是软件开发中真正的护城河，挑战了围绕 AI 辅助编程的热潮。 这一观点重新定义了 AI 在软件工程中的角色辩论，表明即使 AI 工具不断改进，深厚的领域知识仍将不可替代。 文章提到了“氛围编程”——一种开发者不加仔细审查就接受 AI 生成代码的做法——并认为缺乏软件工程技能的领域专家仍然需要传统工程师来构建健壮的系统。

hackernews · aaronbrethorst · May 30, 20:40 · [社区讨论](https://news.ycombinator.com/item?id=48340411)

**背景**: “氛围编程”由 Andrej Karpathy 于 2025 年提出，是一种 AI 辅助开发方法，用户通过提示描述项目并接受生成的代码而不进行深入审查。这引发了关于 AI 是否减少了对传统软件工程技能需求的辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://grokipedia.com/page/Vibe_coding">Vibe coding</a></li>

</ul>
</details>

**社区讨论**: 评论者对优秀开发者标准的不断变化表示怀疑，一些人指出领域专家仍然需要软件工程师来修复糟糕的数据库设计等问题。另一些人则认为软件本身就是一个领域，通才仍然有价值。

**标签**: `#AI`, `#software engineering`, `#domain expertise`, `#vibe coding`

---

<a id="item-4"></a>
## [埃森哲以 12 亿美元收购 Ookla，强化网络 AI 能力](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

埃森哲已同意以 12 亿美元收购 Ookla（Speedtest、Downdetector、Ekahau 和 RootMetrics 的母公司），以增强其面向企业的网络智能和数据驱动 AI 服务。 此次收购使埃森哲获得 Ookla 每月超过 2.5 亿次消费者发起测试的庞大数据集，从而能为电信运营商和企业提供更深入的洞察，以优化 5G 和 Wi-Fi 网络。这也表明网络数据作为 AI 驱动咨询和服务的关键资产，其价值日益增长。 Ookla 的数据平台除了消费者发起的测试外，还包括受控的驾车、步行和嵌入式测试选项。埃森哲此前通过收购网络测试公司 Umlaut，已在该领域成为竞争对手。

hackernews · Garbage · May 30, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48337987)

**背景**: Ookla 最知名的产品是 Speedtest.net（用于测量互联网连接性能的流行工具）和 Downdetector（实时追踪服务中断情况）。该公司的主要收入来自向电信运营商出售聚合的网络性能数据，运营商每年支付六位数费用以获取改善基础设施的洞察。埃森哲是一家全球 IT 服务和咨询公司，一直在大力投资 AI，包括承诺投入 30 亿美元用于生成式 AI。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ookla.com/speedtest-intelligence">Speedtest Intelligence ® Global Performance Metrics | Ookla</a></li>
<li><a href="https://en.wikipedia.org/wiki/Downdetector">Downdetector - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，这笔交易本质上是一次数据收购，因为 Ookla 的真正价值在于向电信运营商销售网络智能，而非面向消费者的 Speedtest 或 Downdetector。一些人担心，Downdetector 被一家与它所监控的公司有合作的咨询公司收购后，其独立性会受到影响。

**标签**: `#acquisition`, `#network intelligence`, `#data monetization`, `#telecom`, `#AI`

---

<a id="item-5"></a>
## [Zig ELF 链接器进展迈向 C 语言替代](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

Zig 最新开发日志显示，新的 ELF 链接器已能构建启用了 LLVM 和 LLD 库的自托管 Zig 编译器，标志着链接器开发的一个重要里程碑。 这一改进使 Zig 更接近成为具有快速迭代速度的完整 C 语言替代品，可能使开发者获得类似 C 的性能，同时开发周期像 JavaScript 或 Python 一样快。 该链接器支持增量链接，可加速开发构建，但可能与发布构建中常用的链接时优化（LTO）互斥。

hackernews · kristoff_it · May 30, 17:29 · [社区讨论](https://news.ycombinator.com/item?id=48338673)

**背景**: ELF 链接器将编译后的目标文件组合成可执行文件或共享库。Zig 正在开发自己的链接器以取代传统的 GNU ld 或 LLVM 的 lld，旨在实现更快的编译速度和与构建系统的更好集成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/?2026-05-30">Devlog Zig Programming Language</a></li>
<li><a href="https://hn.nuxt.dev/item/48338673">Nuxt HN | Zig ELF Linker Improvements Devlog</a></li>
<li><a href="https://ziggit.dev/t/devlog-elf-linker-improvements/15808">Devlog ELF Linker Improvements - Media - Ziggit</a></li>

</ul>
</details>

**社区讨论**: 社区成员热情高涨，一位用户指出 Zig 的链接器进展使其成为快速迭代的可行 C 语言替代品。另一位用户表示很高兴选择 Zig 而非 Rust 作为转译目标，称赞其优越的构建系统设计。

**标签**: `#Zig`, `#linker`, `#systems programming`, `#compiler`, `#programming languages`

---

<a id="item-6"></a>
## [OpenRouter 完成 1.13 亿美元 B 轮融资](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter 宣布完成 1.13 亿美元的 B 轮融资，巩固了其作为低摩擦、带计费控制的多个 LLM 提供商访问代理层的关键地位。 这笔融资验证了 OpenRouter 在 AI 基础设施栈中的地位，使开发者无需管理多个 API 集成即可轻松试验和切换模型，这在 LLM 生态日益多样化的今天愈发重要。 OpenRouter 对 API 调用收取 5% 的附加费，一些用户认为考虑到统一访问和计费上限（许多模型提供商仍缺乏此功能）的便利性，这个费用是可以接受的。

hackernews · freeCandy · May 30, 17:27 · [社区讨论](https://news.ycombinator.com/item?id=48338660)

**背景**: OpenRouter 是一项代理服务，通过单一 API 端点即可访问来自不同提供商的数百个 LLM，包括开源和专有模型。它通过处理认证、计费和路由来简化开发者体验，并提供计费上限和可观测性等功能。该公司旨在减少 AI 构建者的摩擦，支持跨模型实验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/enterprise">Enterprise AI Infrastructure Made Simple | OpenRouter</a></li>
<li><a href="https://github.com/pmbstyle/openrouter-proxy">GitHub - pmbstyle/ openrouter - proxy : Nodejs OpenRouter proxy ...</a></li>

</ul>
</details>

**社区讨论**: 社区成员普遍称赞 OpenRouter 减少了 API 摩擦并支持轻松进行模型实验，但有人质疑一旦模型格局稳定后其长期价值。联合创始人澄清公司仍由创始人领导，专注于为开发者构建产品。

**标签**: `#AI Infrastructure`, `#Funding`, `#LLM APIs`, `#OpenRouter`, `#Developer Tools`

---

<a id="item-7"></a>
## [Anthropic 详解 Claude 跨产品沙箱技术](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了一份详细的技术概述，介绍了用于在 Claude.ai、Claude Code 和 Cowork 中隔离 Claude 的沙箱技术，包括 gVisor、Seatbelt、Bubblewrap 和完整虚拟机隔离。 这份文档通过提供具体的实现细节，填补了沙箱产品中常见的信任缺口，对 AI 安全和企业采用代理型 AI 工具至关重要。 Claude.ai 使用 gVisor，Claude Code 在 macOS 上使用 Seatbelt、在 Linux 上使用 Bubblewrap，而 Claude Cowork 运行完整虚拟机（macOS 上使用 Apple 的 Virtualization 框架，Windows 上使用 HCS）。文章还披露了一个之前遗漏的通过 api.anthropic.com/v1/files 的数据外泄途径。

rss · Simon Willison · May 30, 21:36

**背景**: 沙箱是一种安全技术，通过隔离应用程序或进程来限制其被攻破后可能造成的损害。gVisor 是 Google 开发的容器沙箱，在用户空间实现 Linux 系统调用以增强安全性。Seatbelt 是 macOS 内置的沙箱框架，Bubblewrap 是 Flatpak 等使用的轻量级 Linux 沙箱工具。这些工具有助于防止 AI 代理访问敏感数据或执行未经授权的操作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged sandboxing tool used by Flatpak and similar projects · GitHub</a></li>
<li><a href="https://github.com/bkircher/seatbelt">GitHub - bkircher/ seatbelt : Simple macOS Seatbelt wrapper that runs...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#sandboxing`, `#Anthropic`, `#Claude`, `#security`

---

<a id="item-8"></a>
## [通过 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison 展示了一种使用 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用的方法，使得生成的 HTML 中的 JavaScript 能够被执行。这种方法克服了之前基于 Web Worker 的方法中<script>标签无法执行的限制。 这项技术使得像 Datasette 这样的全功能 Python Web 应用能够在浏览器中完全运行并支持 JavaScript，扩展了基于浏览器的 Python 应用的能力。它使得依赖 JavaScript 的插件和功能能够在 Datasette Lite 及类似项目中正常工作。 该实现使用服务工作者拦截网络请求，并提供由 Pyodide 中运行的 Python ASGI 应用生成的响应。Simon Willison 使用 Claude Opus 4.8 帮助原型设计解决方案，并提供了基本 ASGI 应用和 Datasette 1.0a31 的演示。

rss · Simon Willison · May 30, 21:02

**背景**: Pyodide 是 CPython 到 WebAssembly 的移植，使得 Python 能够在浏览器中运行。ASGI（异步服务器网关接口）是异步 Python Web 服务器和应用程序的规范。服务工作者是在浏览器后台运行的脚本，可以拦截网络请求，充当可编程代理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers">Using Service Workers - Web APIs | MDN - MDN Web Docs</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WebAssembly`, `#ASGI`, `#Service Workers`, `#Datasette`

---

<a id="item-9"></a>
## [蓝色起源新格伦火箭静态点火测试爆炸](https://arstechnica.com/space/2026/05/blue-origins-new-glenn-rocket-just-exploded-during-a-static-fire-test/) ⭐️ 8.0/10

2026 年 5 月 28 日，蓝色起源的新格伦火箭在卡纳维拉尔角进行静态点火测试时发生爆炸，火箭被毁，发射台受损。爆炸发生在七台 BE-4 甲烷发动机点火过程中，导致火箭完全报废，地面基础设施严重损毁。 此次事故严重影响了 NASA 的阿尔忒弥斯登月计划，因为蓝色起源承担了月球着陆器和月球车的发射任务。同时，这也推迟了亚马逊的 Kuiper 卫星互联网星座项目，因为 NG-4 任务原计划部署 48 颗 Kuiper 卫星。 爆炸发生在 NG-4 任务的静态点火测试期间，该任务原计划发射 48 颗亚马逊 Kuiper 宽带卫星。无人员伤亡报告，但发射台的闪电防护塔倒塌，地面基础设施严重受损。

telegram · zaihuapd · May 29, 11:08

**背景**: 新格伦是蓝色起源的重型轨道火箭，由七台 BE-4 发动机提供动力，使用液化天然气（甲烷）和液氧。BE-4 是一种富氧分级燃烧发动机，是美国制造的首款此类发动机。Kuiper 项目（现已更名为 Amazon Leo）是亚马逊的卫星互联网星座，旨在与 Starlink 竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nasaspaceflight.com/2026/05/blue-origin-new-glenn-explodes/">Blue Origin's New Glenn explodes during Static Fire test at ...</a></li>
<li><a href="https://aviationweek.com/space/launch-vehicles-propulsion/new-glenn-explodes-during-static-test-fire">New Glenn Explodes During Static Test Fire | Aviation Week</a></li>
<li><a href="https://en.wikipedia.org/wiki/BE-4">BE-4 - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Blue Origin`, `#New Glenn`, `#rocket explosion`, `#NASA Artemis`, `#space industry`

---

<a id="item-10"></a>
## [SpaceX 获 41.6 亿美元美军卫星合同](https://www.bloomberg.com/news/articles/2026-05-29/spacex-wins-4-billion-contract-for-us-golden-dome-satellites) ⭐️ 8.0/10

SpaceX 获得美国太空军 41.6 亿美元合同，将建设低地球轨道卫星网络，用于追踪飞机、巡航导弹等空中威胁，作为 Golden Dome 防御系统的一部分。 这份合同标志着 SpaceX 在国家安全太空项目中的角色显著扩大，也表明商业航天能力在军事导弹追踪与防御领域日益重要。 该卫星星座将整合天基传感器、通信系统和地面处理能力，以减少现有地面雷达和飞机监测的盲区。SpaceX 此前已参与 Golden Dome 的天基拦截器原型开发，并加入了该计划底层软件系统的多公司联盟。

telegram · zaihuapd · May 30, 01:53

**背景**: Golden Dome 是美国总统特朗普于 2025 年 5 月宣布的多层导弹防御系统，旨在保护美国免受远程和高超音速导弹的威胁。其名称借鉴了以色列的 Iron Dome，但规模预计大得多。该系统计划利用天基传感器和拦截器实现全球覆盖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spacenews.com/space-force-awards-spacex-4-16-billion-to-build-satellite-network-for-airborne-target-tracking/">Space Force awards SpaceX $4.16 billion to build satellite ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Golden_Dome_(missile_defense_system)">Golden Dome (missile defense system) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#defense`, `#satellite`, `#missile tracking`, `#Golden Dome`

---

<a id="item-11"></a>
## [华为提出“韬定律”：以时间缩微替代几何缩微](https://t.me/zaihuapd/41648) ⭐️ 8.0/10

在 2026 年上海国际电路与系统研讨会（ISCAS）上，华为发表了“韬定律”（τ定律），这是一种以时间缩微替代传统几何缩微的半导体演进新原则。过去六年，华为已据此设计量产了 381 款芯片，并计划今年秋季推出采用逻辑折叠技术的新麒麟芯片。 韬定律通过降低时间常数而非缩小晶体管尺寸，为逼近物理极限的摩尔定律提供了潜在替代路径。这有望在不依赖极紫外（EUV）光刻技术的情况下持续提升芯片性能，惠及整个半导体行业，尤其对面临出口限制的中国企业意义重大。 该定律以希腊字母τ（tau）命名，τ在电路理论中代表时间常数。华为的逻辑折叠技术通过垂直堆叠多层有源硅，在物理上“折叠”关键路径，减少水平走线和 RC 延迟。华为预计，到 2031 年基于该定律的芯片晶体管密度可达 1.4 纳米制程同等水平。

telegram · zaihuapd · May 30, 02:18

**背景**: 摩尔定律——芯片上晶体管数量大约每两年翻一番的观察——数十年来推动了半导体进步，但如今因物理和经济限制而放缓。几何缩微（缩小晶体管尺寸）一直是提升性能的主要方法，但需要越来越昂贵的光刻工具（如 EUV）。韬定律提出了一种替代方案：在器件、电路、芯片和系统层面系统性降低时间常数τ，从而在不完全依赖光刻缩微的情况下实现性能提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://baike.baidu.com/item/韬定律/67839953">韬定律 - 百度百科</a></li>
<li><a href="https://baike.baidu.com/item/逻辑折叠技术/67870423">逻辑折叠技术 - 百度百科</a></li>
<li><a href="https://www.huxiu.com/article/4861353.html">华为提出韬定律挑战摩尔定律，芯片设计新路径浮出水面</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#Moore's Law`, `#Huawei`, `#chip design`, `#scaling`

---

<a id="item-12"></a>
## [Voxel Space 算法详解](https://s-macke.github.io/VoxelSpace/) ⭐️ 7.0/10

一篇关于 1992 年游戏《Comanche》中使用的 Voxel Space 渲染算法的详细技术说明已发布，包含交互式演示和源代码。 这次深入解析保留了一种在有限硬件上实现逼真地形的、具有历史意义的 2.5D 渲染技术，启发了现代实现和复古游戏开发。 该算法使用高度图和颜色图通过光线投射渲染地形，但并非真正的体素渲染；它是一个 2.5D 引擎，缺乏完整的 3D 自由度。

hackernews · davikr · May 30, 14:25 · [社区讨论](https://news.ycombinator.com/item?id=48336564)

**背景**: Voxel Space 是 NovaLogic 为 1992 年直升机模拟游戏《Comanche: Maximum Overkill》开发的专有引擎。它完全用汇编语言编写，采用基于高度图的光线投射技术渲染平滑、有机的地形，在当时与基于多边形的游戏相比令人印象深刻。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://s-macke.github.io/VoxelSpace/">Voxel Space | VoxelSpace</a></li>
<li><a href="https://github.com/s-macke/VoxelSpace">GitHub - s-macke/VoxelSpace: Terrain rendering algorithm in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comanche_(video_game_series)">Comanche (video game series) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者指出该算法在技术上是一种高度图光线投射器，而非真正的体素渲染。一位用户分享了最小化测试的实用类比，其他人则分享了在 C++和 AGS 引擎中的现代移植和实现链接。

**标签**: `#rendering`, `#retro-gaming`, `#algorithms`, `#voxels`

---

<a id="item-13"></a>
## [Openrsync：OpenBSD 的安全 rsync 实现](https://github.com/kristapsdz/openrsync) ⭐️ 7.0/10

OpenBSD 团队发布了 openrsync，这是对广泛使用的 rsync 文件同步工具的重写，重点在于安全性和正确性。 这很重要，因为 rsync 是系统管理和文件传输的关键工具，而 openrsync 旨在通过利用 OpenBSD 的 pledge 和 unveil 等安全特性来减少漏洞，为面向网络的操作提供更安全的替代方案。 Openrsync 尚未完全替代 rsync；用户报告了某些标志和行为的问题，例如 --rsync-path 选项未按预期工作。该项目目前正在作为 RPKI 验证器的一部分进行开发。

hackernews · sph · May 30, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48334854)

**背景**: Rsync 是一种通过比较修改时间和大小来高效传输和同步文件的实用程序。原生的 rsync 协议不加密数据，因此仅适用于受信任的网络。OpenBSD 的 pledge 和 unveil 是安全机制，分别限制进程能力和文件系统访问，以限制潜在漏洞的影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.openbsdhandbook.com/rsync/">rsync | OpenBSD Handbook</a></li>
<li><a href="https://hn.nuxt.dev/item/48334854">Nuxt HN | Openrsync: An implementation of rsync , by the OpenBSD ...</a></li>
<li><a href="https://docs.ircnow.org/openbsd/openrsync/">openrsync</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了实际使用经验，指出其随时间有所改进，但也指出了如标志支持不完整等限制。一些用户表示希望一旦成熟就完全使用 openrsync，而另一些用户则提到了 Go 语言的替代实现。还有关于 pledge 和 unveil 对安全性的重要性的讨论，以及这些特性在 Linux 等其他平台上是否可用。

**标签**: `#rsync`, `#OpenBSD`, `#security`, `#file synchronization`, `#open source`

---

<a id="item-14"></a>
## [教宗利奥首道通谕批判技术救世主义](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 7.0/10

教宗利奥十四世发布了首道通谕《崇高人性》，批判技术救世主义，并警告通过人工智能集中权力的危险。 这道通谕为关于人工智能伦理与控制的全球辩论增添了强有力的宗教声音，挑战了仅靠技术就能解决人类问题的叙事。 这道名为《崇高人性》的通谕英文版约 42,300 字，以人工智能为核心议题，呼吁保护人类尊严与自主性。

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [社区讨论](https://news.ycombinator.com/item?id=48334710)

**背景**: 技术救世主义是一种认为技术将带来乌托邦未来或拯救人类的信念。教宗利奥的通谕延续了天主教社会训导的传统，该传统经常涉及当代伦理问题。梵蒂冈此前已参与人工智能伦理讨论，包括举办相关会议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ncronline.org/vatican/vatican-news/pope-leo-calls-disarm-ai-major-document-warns-technologic-threats-humanity">Pope Leo calls to 'disarm' AI in major document, warns of technologic threats to humanity | National Catholic Reporter</a></li>
<li><a href="https://www.vaticannews.va/en/pope/news/2026-05/pope-leo-xiv-encyclical-magnifica-humanitas-ai.html">Pope Leo’s ‘Magnifica humanitas’: AI must serve humanity not concentrate power - Vatican News</a></li>
<li><a href="https://www.nytimes.com/2026/05/25/world/europe/pope-leo-encyclical.html">Pope Leo Warns of Risks From A.I. in 42,300-Word Encyclical - The New York Times</a></li>

</ul>
</details>

**社区讨论**: 社区评论突出了关于谁应控制技术的辩论，一些人指出像 Sam Altman 和 Dario Amodei 这样的科技 CEO 表现出“AI 精神病”。其他人则引用 Peter Thiel 关于敌基督的观点，将技术救世主义与宗教概念联系起来。

**标签**: `#AI ethics`, `#religion and technology`, `#technology control`, `#Vatican`, `#technological messianism`

---

<a id="item-15"></a>
## [Chad Whitacre 因 AI 退出科技行业](https://simonwillison.net/2026/May/30/retiring-from-tech-to-live-offline/#atom-everything) ⭐️ 7.0/10

Sentry 创始人 Chad Whitacre 宣布退出科技和开源领域，计划过一种受阿米什人启发的离线生活。他将 AI 称为压垮他的最后一根稻草，形容其为侵入他思想的“另一个人”。 这位知名开源人物的个人决定凸显了人们对 AI 影响心理健康和生活方式的日益不安。它可能激励他人重新审视自己与技术的关系，并加速关于数字戒断和 AI 伦理的讨论。 Whitacre 的退休伴随着一封打字机打印并扫描的信件和一篇视频文章。他此前曾尝试过 Claude Code 和 Opus 4.5 等 AI 工具，这些体验让他感到既陶醉又不安。

rss · Simon Willison · May 30, 19:39

**背景**: Sentinelese 人是北哨兵岛上一个未接触的土著群体，他们暴力排斥外来者。阿米什人是一个基督教派别，以选择性拒绝现代技术以保护其生活方式而闻名。Whitacre 将这些群体与他退出科技的愿望相类比，目标是过一种拒绝 AI 和 doomscrolling、但接受汽车和电力的“新阿米什”生活方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sentinelese">Sentinelese - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amish_way_of_life">Amish way of life - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上对这篇文章的评论褒贬不一，有人对 Whitacre 的立场表示同情，也有人质疑他计划的可行性。几位评论者指出，通过在线平台宣布离线退休具有讽刺意味。

**标签**: `#AI impact`, `#tech career`, `#open source`, `#digital detox`, `#personal essay`

---

<a id="item-16"></a>
## [Datasette 1.0a31 新增写入查询和存储查询功能](https://simonwillison.net/2026/May/29/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a31 允许拥有相应权限的用户执行写入查询（INSERT/UPDATE/DELETE）并保存存储查询（原“canned queries”已更名）。 此版本将 Datasette 从只读探索工具转变为功能完整的数据库应用平台，使用户能够编辑数据并在实例内共享可复用的查询。 写入查询通过新界面执行，提供模板化的 INSERT/UPDATE/DELETE 语句，权限粒度精细（例如，create-table 权限独立）。存储查询可私有保存或与实例其他成员共享。

rss · Simon Willison · May 29, 03:32

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具。此前仅支持只读查询。此 alpha 版本标志着向 Datasette 1.0 迈出的重要一步，新增了之前仅通过 datasette-write 等插件提供的写入功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/sql-write-queries/">SQL write queries and stored queries in Datasette ... - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/May/29/datasette/">Release: datasette 1.0a31 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#release`, `#sql`, `#database`, `#open-source`

---

<a id="item-17"></a>
## [骑手过剩：2000 万骑手仅需 400 万](https://m.sohu.com/a/1029514455_122135404) ⭐️ 7.0/10

中国即时配送行业骑手已接近 2000 万人，但支撑日均约 1.1 亿订单实际只需约 400 万熟练骑手，超过 1600 万人成为冗余运力。 骑手严重过剩凸显了零工经济中劳动力市场的扭曲和经济低效，导致骑手之间激烈竞争，以及美团、京东、阿里巴巴等平台巨额亏损。 始于 2025 年 2 月的补贴大战新增骑手超过 800 万人，同时平台合计亏损数十亿：美团 2025 年净亏损 234 亿元，京东新业务亏损 466 亿元，阿里即时零售亏损 870 亿元。

telegram · zaihuapd · May 30, 09:52

**背景**: 美团、京东、阿里巴巴等即时配送平台从 2025 年初开始激烈补贴大战，通过巨额优惠吸引用户和骑手，导致骑手数量激增远超实际需求。随着补贴退潮，订单量未能同步增长，造成运力过剩和骑手间激烈竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KU6JGDUE0556N7I6.html">外卖大战退潮后，2000万骑手挤在路上，1600万是“冗余运力”|单量|扩张...</a></li>
<li><a href="https://www.sohu.com/a/962694058_121385340">三大平台外卖大战：每分钟“烧钱”40万，谁在为“非理性买单”？_补贴_利...</a></li>
<li><a href="https://www.bcbay.com/news/2026/05/30/1020516.html">中国外卖大战后骑手过剩 需400万人涌进2000万人-新闻中心-温哥华港湾...</a></li>

</ul>
</details>

**标签**: `#gig economy`, `#labor market`, `#platform economics`, `#delivery industry`, `#China`

---

<a id="item-18"></a>
## [Codex 现已支持跨设备远程控制](https://developers.openai.com/codex/changelog#codex-2026-05-28-app) ⭐️ 7.0/10

OpenAI 的 Codex 现在允许用户从 iOS、Android 或 Mac 设备远程控制 Windows 上的 Codex 实例，并实时查看进度。此次更新还引入了增强的协作功能，包括本地项目和工作树中的线程协调，以及覆盖对话内容和 Git 分支名称的扩展搜索。 此次更新显著提升了 Codex 对于跨设备工作的开发者的实用性，实现了无缝的远程编码和监控。扩展的搜索和线程协调功能使得管理复杂项目和检索上下文更加容易，从而提高了使用 Codex 作为 AI 编码助手的团队的生产力。 远程控制要求 Codex 在 Windows 主机上运行，控制设备可以是 Mac、iPhone 或 Android 手机（通过 ChatGPT 移动应用）。新的线程协调允许在工作树中添加独立的后台线程以实现灵活的多任务处理，个人资料页面现在显示详细的使用统计和词元活动。

telegram · zaihuapd · May 30, 10:37

**背景**: Codex 是 OpenAI 开发的 AI 编码助手，能够理解和生成代码、自动化任务并与桌面应用交互。此前，Codex 仅限于在单个设备上本地使用；此次更新将其扩展到远程和移动访问，使其对于需要从不同地点或设备工作的开发者更加灵活。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/work-with-codex-from-anywhere/">Work with Codex from anywhere | OpenAI</a></li>
<li><a href="https://developers.openai.com/codex/remote-connections">Remote connections – Codex | OpenAI Developers</a></li>
<li><a href="https://developers.openai.com/codex/app/worktrees">Worktrees – Codex app | OpenAI Developers</a></li>

</ul>
</details>

**标签**: `#Codex`, `#remote control`, `#AI coding assistant`, `#collaboration`, `#search`

---