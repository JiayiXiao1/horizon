---
layout: default
title: "Horizon Summary: 2026-06-01 (ZH)"
date: 2026-06-01
lang: zh
---

> From 37 items, 11 important content pieces were selected

---

1. [VideoLAN 发布开源 AV2 解码器 Dav2d](#item-1) ⭐️ 9.0/10
2. [Cloudflare Turnstile 要求 WebGL 指纹识别，引发隐私担忧](#item-2) ⭐️ 8.0/10
3. [可重启序列：Linux 中的无锁并发机制](#item-3) ⭐️ 8.0/10
4. [Anthropic 详解 Claude 产品中的沙箱技术](#item-4) ⭐️ 8.0/10
5. [通过 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](#item-5) ⭐️ 8.0/10
6. [FROST 攻击：网站通过 SSD 计时窥探用户](#item-6) ⭐️ 8.0/10
7. [1 位 Bonsai Image 4B 实现本地图像生成](#item-7) ⭐️ 7.0/10
8. [AI 工具作为 ADHD 放大器：一位开发者的反思](#item-8) ⭐️ 7.0/10
9. [Chad Whitacre 因 AI 退出科技行业](#item-9) ⭐️ 7.0/10
10. [中国外卖行业骑手过剩达 5 倍](#item-10) ⭐️ 7.0/10
11. [Codex 现已支持跨设备远程控制与增强搜索](#item-11) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [VideoLAN 发布开源 AV2 解码器 Dav2d](https://jbkempf.com/blog/2026/dav2d/) ⭐️ 9.0/10

VideoLAN 宣布了 dav2d，这是一个新的基于 CPU 的开源 AV2 视频解码器，并指出 AV2 解码的复杂度大约是 AV1 的五倍。 Dav2d 是 AV2 采用的关键一步，因为软件解码器可以在硬件解码器可用之前实现播放和测试，而其性能挑战凸显了针对特定架构优化的必要性。 Dav2d 目前专注于正确性，计划针对 x86、ARM 和 RISC-V 架构进行性能优化；AV2 预计在相同质量下比 AV1 降低约 30% 的码率。

hackernews · captain_bender · May 31, 11:44 · [社区讨论](https://news.ycombinator.com/item?id=48344961)

**背景**: AV2 是 AV1 的继任者，由开放媒体联盟（AOMedia）开发的开放、免版税视频编码格式。它于 2026 年 5 月正式发布，旨在为流媒体、广播以及 AR/VR 等新兴应用提供更高的压缩效率。参考编码器 AVM 1.0.0 于 2026 年初发布，但像 dav2d 这样的软件解码器对于实际使用至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.phoronix.com/news/Dav2d-Open-Source-AV2-Decode">VideoLAN Publishes Dav2d For Open-Source AV2 Decoder - Phoronix</a></li>
<li><a href="https://videocardz.com/newz/videolan-publishes-dav2d-an-early-cpu-decoder-for-av2-video-codec">VideoLAN publishes dav2d, an early CPU decoder for AV2 video codec - VideoCardz.com</a></li>
<li><a href="https://en.wikipedia.org/wiki/AV2_(video_coding_format)">AV2 (video coding format)</a></li>

</ul>
</details>

**社区讨论**: 社区评论既表达了兴奋也表达了担忧：有人质疑 25% 的体积缩减是否值得淘汰 AV1 硬件解码器，而另一些人则指出 AV2 解码基准测试将很有揭示性。还有关于编解码器设计哲学的讨论，即对解码进行描述性规定而非对编码进行规定性规定。

**标签**: `#video codec`, `#AV2`, `#decoder`, `#open source`, `#performance`

---

<a id="item-2"></a>
## [Cloudflare Turnstile 要求 WebGL 指纹识别，引发隐私担忧](https://hacktivis.me/articles/cloudflare-turnstile-webgl-fingerprinting) ⭐️ 8.0/10

Cloudflare 的 Turnstile（一种 CAPTCHA 替代方案）现在要求进行 WebGL 指纹识别以区分人类和机器人，最近的一项分析揭示了这一点。这一变化使用户即使在启用了 Firefox 的 resistFingerprinting 等隐私保护措施时，也会暴露于浏览器指纹识别之下。 这一发展凸显了机器人检测与用户隐私之间不断升级的军备竞赛，因为像 Turnstile 这样广泛使用的服务采用了可能削弱隐私工具的指纹识别技术。它影响了数百万使用 Turnstile 的网站，并引发了关于安全与隐私之间权衡的质疑。 WebGL 指纹识别利用设备图形硬件的独特渲染特性来创建持久标识符，可用于跨会话跟踪用户。Cloudflare 的 Turnstile 现在需要此功能，可能会在阻止或伪造 WebGL 的浏览器或配置上失效。

hackernews · HypnoticOcelot · May 31, 14:13 · [社区讨论](https://news.ycombinator.com/item?id=48345840)

**背景**: WebGL 指纹识别是一种利用 WebGL API 从设备显卡和驱动程序中提取唯一签名的方法。Cloudflare Turnstile 是一种注重隐私的传统 CAPTCHA 替代方案，旨在无需交互式挑战即可验证用户。机器人检测军备竞赛导致了越来越侵入性的方法，指纹识别已成为常用工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://browserleaks.com/webgl">WebGL Browser Report - WebGL Fingerprinting - BrowserLeaks</a></li>
<li><a href="https://www.cloudflare.com/products/turnstile/">Cloudflare Turnstile - Easy CAPTCHA Alternative</a></li>
<li><a href="https://dev.to/agenthustler/headless-browser-detection-how-sites-know-youre-a-bot-47g">Headless Browser Detection : How Sites Know You're a Bot</a></li>

</ul>
</details>

**社区讨论**: 评论者对隐私影响表示不满，一些人指出即使 Firefox 的严格隐私模式也无法阻止 WebGL 指纹识别。其他人则为指纹识别作为机器人检测的必要之恶辩护，而一位用户警告称，这场军备竞赛可能将互联网变成围墙花园。

**标签**: `#privacy`, `#fingerprinting`, `#cloudflare`, `#webgl`, `#bot-detection`

---

<a id="item-3"></a>
## [可重启序列：Linux 中的无锁并发机制](https://justine.lol/rseq/) ⭐️ 8.0/10

文章解释了可重启序列（rseq），这是一种 Linux 内核机制，允许用户空间代码定义临界区，如果被抢占，内核将重新执行该临界区，从而在许多情况下消除了对互斥锁和原子操作的需求。 rseq 通过减少锁和原子操作的开销，显著提高了并发程序的性能，特别是在多核系统上，并且已在 TCMalloc 等生产系统中使用。 rseq 机制的工作原理是让内核检查被抢占线程的程序计数器；如果它落在已注册的临界区内，内核会将程序计数器重置到该区域的起始位置，从而无需硬件锁即可保证原子性。

hackernews · grappler · May 31, 14:38 · [社区讨论](https://news.ycombinator.com/item?id=48346019)

**背景**: 传统的并发控制使用互斥锁或原子操作来保护共享数据，但这些操作开销较大。可重启序列通过利用内核支持在被抢占时重试临界区，提供了一种轻量级替代方案。该特性最初由 Paul Turner 和 Andrew Hunter 于 2013 年提出，并合入 Linux 内核 4.18。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.efficios.com/blog/2019/02/08/linux-restartable-sequences/">The 5-year journey to bring restartable sequences to Linux - EfficiOS</a></li>
<li><a href="https://google.github.io/tcmalloc/rseq.html">Restartable Sequence Mechanism for TCMalloc | tcmalloc</a></li>
<li><a href="http://www.gnu.org/software/libc/manual//html_node/Restartable-Sequences.html">Restartable Sequences (The GNU C Library)</a></li>

</ul>
</details>

**社区讨论**: 评论者提到了 librseq 库，可以更轻松地使用 rseq 而无需汇编代码；也有人批评文章关于昂贵工作站的语气。历史背景被提及，指出类似技术约 25 年前就已存在。

**标签**: `#Linux`, `#concurrency`, `#kernel`, `#performance`, `#rseq`

---

<a id="item-4"></a>
## [Anthropic 详解 Claude 产品中的沙箱技术](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic 发布了一份详细的技术概述，介绍了 Claude.ai、Claude Code 和 Claude Cowork 中使用的沙箱技术，包括 gVisor、Seatbelt、Bubblewrap 和完整虚拟机。 这份文档通过提供透明度，解决了沙箱工具信任度普遍不足的问题，帮助开发者和用户理解保护 AI 代理的安全边界。 Claude.ai 使用 gVisor，Claude Code 在 macOS 上使用 Seatbelt、在 Linux 上使用 Bubblewrap，Claude Cowork 则通过 Apple 的 Virtualization framework 或 Windows 上的 HCS 运行完整虚拟机。文章还披露了过去的风险，如 api.anthropic.com/v1/files 数据泄露途径。

rss · Simon Willison · May 30, 21:36

**背景**: 沙箱技术将 AI 代理与主机系统隔离，以防止恶意行为。gVisor 是 Google 开发的容器沙箱，在用户空间实现 Linux 系统调用。Seatbelt 是 macOS 内置的沙箱，Bubblewrap 是 Flatpak 使用的轻量级 Linux 沙箱。这些工具限制文件系统、网络和进程的访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/ bubblewrap : Low-level unprivileged sandboxing...</a></li>
<li><a href="https://github.com/bkircher/seatbelt">GitHub - bkircher/ seatbelt : Simple macOS Seatbelt wrapper that runs...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#sandboxing`, `#Anthropic`, `#Claude`, `#security`

---

<a id="item-5"></a>
## [通过 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison 展示了通过 Pyodide 和服务工作者在浏览器中运行 Python ASGI 应用的方法，使得 Datasette Lite 能够完整执行 JavaScript。他使用 Claude Opus 4.8 生成了这一解决方案，克服了之前 Web Worker 方法无法执行<script>标签的限制。 这种方法使得完整的 Python ASGI Web 应用能够在浏览器中运行，包括支持依赖 JavaScript 的插件和功能。它极大地扩展了基于浏览器的 Python 工具（如 Datasette Lite）的能力，使其在实际应用中更加实用。 该解决方案使用服务工作者拦截网络请求，并通过 Pyodide 运行 Python ASGI 应用，从而允许<script>标签中的 JavaScript 正常执行。Simon Willison 提供了两个演示：一个基本的 ASGI FastCGI 演示和一个运行 Datasette 1.0a31 的演示。

rss · Simon Willison · May 30, 21:02

**背景**: Pyodide 是一个基于 WebAssembly 的浏览器 Python 发行版，允许 Python 代码直接在浏览器中运行而无需服务器。ASGI（异步服务器网关接口）是构建异步 Python Web 应用的标准。Datasette Lite 是 Datasette 数据探索工具的浏览器版本，通过 Pyodide 在浏览器中运行。此前，Datasette Lite 使用 Web Worker 运行 Python，但这种方法无法执行 HTML 页面中嵌入的 JavaScript，导致部分插件失效。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://asgi.readthedocs.io/en/latest/introduction.html">Introduction — ASGI 3.0 documentation</a></li>
<li><a href="https://github.com/simonw/datasette-lite">GitHub - simonw/datasette-lite: Datasette running in your browser using WebAssembly and Pyodide · GitHub</a></li>

</ul>
</details>

**标签**: `#Pyodide`, `#WebAssembly`, `#ASGI`, `#Python`, `#Service Workers`

---

<a id="item-6"></a>
## [FROST 攻击：网站通过 SSD 计时窥探用户](https://futurism.com/future-society/websites-spying-solid-state-drive) ⭐️ 8.0/10

研究人员披露了一种名为 FROST 的无交互侧信道攻击，恶意网站可通过浏览器的 Origin Private File System (OPFS) API 测量 SSD 读写计时，从而推断用户活动。 该攻击在识别访问的网站和运行的应用时准确率达 88-96%，无需安装软件或用户交互，对网络用户隐私构成重大威胁，并凸显了一类新的基于浏览器的侧信道漏洞。 该攻击在 Mac 和 Linux 系统上测试，网站识别准确率为 88.95%，应用识别准确率为 95.83%；研究人员指出 Windows 并非免疫。用完网页后及时关闭标签页可降低风险。

telegram · zaihuapd · May 31, 01:55

**背景**: Origin Private File System (OPFS) 是一种浏览器 API，提供对网站源私有的低级逐字节文件访问。以往的基于 SSD 的侧信道攻击需要在设备上运行原生软件；FROST 首次将此类攻击完全移至浏览器中，通过利用 OPFS 读取操作期间 SSD 争用导致的计时差异来实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arstechnica.com/security/2026/05/websites-have-a-new-way-to-spy-on-visitors-analyzing-their-ssd-activity/">Websites have a new way to spy on visitors: Analyzing their SSD activity</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/05/29/website-tracking-ssd-activity-research/">Websites can spy on user activity by analyzing SSD ... - Help Net Security</a></li>
<li><a href="https://hannesweissteiner.com/pdfs/frost.pdf">FROST : Fingerprinting Remotely using</a></li>

</ul>
</details>

**标签**: `#security`, `#side-channel attack`, `#SSD`, `#privacy`, `#web browser`

---

<a id="item-7"></a>
## [1 位 Bonsai Image 4B 实现本地图像生成](https://prismml.com/news/bonsai-image-4b) ⭐️ 7.0/10

PrismML 发布了 Bonsai Image 4B，这是一个 1 位量化的扩散 Transformer 模型，可在手机和笔记本电脑等本地设备上生成图像，模型大小仅为 930 MB。 这一突破使得在消费级硬件上无需依赖云端即可实现高质量图像生成，降低了成本和隐私担忧，并为边缘 AI 应用开辟了新的可能性。 Bonsai Image 4B 在 iPhone 17 Pro Max 上生成 512x512 图像需 9.4 秒，在 Mac M4 Pro 上约需 6 秒，相比全精度 FLUX.2 模型实现了高达 5.6 倍的加速。

hackernews · modinfo · May 31, 15:04 · [社区讨论](https://news.ycombinator.com/item?id=48346257)

**背景**: 模型量化通过降低神经网络权重的精度（例如从 16 位降至 1 位）来缩小模型大小并加速推理。扩散 Transformer 是一类通过迭代去噪将随机噪声转化为图像的生成模型。1 位量化对图像生成尤其具有挑战性，因为视觉质量对权重精度高度敏感。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.banandre.com/blog/prismml-bonsai-image-4b-1-bit-webgpu-local-image-generation">Your Browser Just Became an Image Generation Engine... - Banandre</a></li>
<li><a href="https://digg.com/ai/cyontmtp">PrismML releases Bonsai Image 4B, a 930 MB 1 - bit diffusion...</a></li>
<li><a href="https://prismml.com/news/bonsai-image-4b">PrismML — Introducing 1-bit and Ternary Bonsai Image 4 B : Image ...</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人对本地 AI 硬件升级取代订阅感到兴奋，而另一些人质疑这是否解决了真正的瓶颈（生成时间 vs. 内存）。少数人讨论了逼真假图像的伦理问题以及 1 位抖动图像生成的潜力。

**标签**: `#image generation`, `#model quantization`, `#edge AI`, `#local inference`

---

<a id="item-8"></a>
## [AI 工具作为 ADHD 放大器：一位开发者的反思](https://simonwillison.net/2026/May/31/the-solution-might-be-cancelling-my-ai-subscription/#atom-everything) ⭐️ 7.0/10

David Wilson 发表了一篇博客文章，认为 AI 编码工具是“热核级 ADHD 放大器”，导致项目被放弃和时间浪费，并建议取消订阅作为解决方案。 这一批评引起了许多开发者的共鸣，他们发现使用 AI 工具时注意力下降、项目碎片化加剧，引发了关于生成式 AI 时代生产力和注意力的重要讨论。 Wilson 列出了超过 16 个用 AI 工具启动的项目，指出大多数并非有意为之且未完成。他将自己的经历与 Hacker News 上患有 ADHD 的评论者形成对比，后者报告说 AI 帮助他们实现超专注并完成项目。

rss · Simon Willison · May 31, 16:31

**背景**: ADHD（注意力缺陷多动障碍）是一种神经发育状况，表现为注意力不集中、多动和冲动。AI 编码代理可以快速生成代码、测试和文档，降低了启动新项目的门槛，但也容易导致项目被放弃。这场辩论凸显了 AI 提高生产力与可能分散注意力之间的张力。

**社区讨论**: Hacker News 的讨论出现了分歧：一些 ADHD 用户发现 AI 帮助他们完成项目并保持专注，而另一些人则赞同 Wilson 关于分心和项目放弃的担忧。一位评论者将 AI 描述为“心灵的慰藉”，使其能够保持收件箱清零并参与跨团队工作。

**标签**: `#AI`, `#productivity`, `#attention`, `#developer experience`

---

<a id="item-9"></a>
## [Chad Whitacre 因 AI 退出科技行业](https://simonwillison.net/2026/May/30/retiring-from-tech-to-live-offline/#atom-everything) ⭐️ 7.0/10

知名开源人物 Chad Whitacre 宣布退出科技行业，计划过一种离线的新阿米什式生活，称 AI 是压垮他的最后一根稻草。他分享了一封打字机打印的信件和一段视频来解释他的决定。 这是一位受人尊敬的社区成员采取的具体、高调的行动，反映了人们对 AI 对科技文化和个人福祉影响的日益不安。这可能会激励其他人重新审视自己与技术的关系。 Whitacre 此前曾尝试使用 Claude Code 和 Opus 4.5，形容那种体验就像脑子里有另一个“人”。他计划保留 1980 年代水平的技术（汽车、电力），但拒绝 AI 和末日刷屏。

rss · Simon Willison · May 30, 19:39

**背景**: Sentinelese 人是北哨兵岛上的一个原住民部落，他们暴力拒绝外界接触，以保护其传统生活方式。阿米什人以根据社区价值观选择性采用技术而闻名。Whitacre 将两者作为自己退出现代科技的类比。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sentinelese">Sentinelese - Wikipedia</a></li>
<li><a href="https://groups.etown.edu/amishstudies/cultural-practices/technology/">Technology – Amish Studies</a></li>

</ul>
</details>

**标签**: `#AI`, `#tech culture`, `#retirement`, `#open source`, `#digital minimalism`

---

<a id="item-10"></a>
## [中国外卖行业骑手过剩达 5 倍](https://m.sohu.com/a/1029514455_122135404) ⭐️ 7.0/10

全国即时配送骑手已接近 2000 万人，但支撑日均约 1.1 亿单实际只需要约 400 万熟练骑手，超过 1600 万人成为冗余运力。 这种巨大的劳动力过剩揭示了美团、京东、阿里等平台补贴驱动扩张战导致的严重低效和浪费，造成数十亿亏损，引发对零工经济模式可持续性的担忧。 补贴大战始于 2025 年 2 月，京东、淘宝闪购和美团累计投入超千亿补贴，新增骑手超过 800 万人。2025 年美团净亏损 234 亿元，京东新业务亏损 466 亿元，阿里即时零售亏损 870 亿元。

telegram · zaihuapd · May 30, 09:52

**背景**: 中国外卖行业经历了爆炸性增长，平台通过补贴激烈争夺消费者和骑手。然而，随着补贴退潮，订单量未同步增长，部分市场出现超过 5 名骑手争抢 1 单的情况。维持庞大骑手队伍的高固定成本加上低订单密度，加剧了平台亏损。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.cyol.com/gb/articles/2025-07/19/content_BbOzVPslYb.html">饿了么 美 团 京 东 被约谈背后：外卖之战为何打得如此激烈</a></li>
<li><a href="https://www.jjckb.cn/20250704/da12c895ae7849409ebbbc93277d12ed/c.html">展望即时零售：第三方即配接棒电商快递向千亿市值迈进-经济参考网 _ 新华社《经济参考报》官方网站</a></li>

</ul>
</details>

**标签**: `#gig economy`, `#platform economics`, `#China tech`, `#labor market`

---

<a id="item-11"></a>
## [Codex 现已支持跨设备远程控制与增强搜索](https://developers.openai.com/codex/changelog#codex-2026-05-28-app) ⭐️ 7.0/10

OpenAI 的 Codex 现在允许用户从 iOS、Android 或 Mac 设备远程控制 Windows 上运行的 Codex 会话，并实时查看进度。此外，该应用还引入了本地项目的线程协调功能，并扩展了对话历史和 Git 分支名称的搜索范围。 此次更新通过支持远程操作和多任务处理，显著提升了开发者工作流的灵活性，对于跨设备和跨地点协作的团队尤为有价值。增强的搜索功能帮助开发者快速定位相关上下文，提高了复杂项目中的生产力。 远程控制功能要求 Windows 版 Codex 应用正在运行且可访问；对于 ChatGPT 工作区用户，管理员可能需要启用远程控制访问权限。线程协调允许用户通过函数调用生成独立的后台线程，从而实现并行任务执行。

telegram · zaihuapd · May 30, 10:37

**背景**: Codex 是 OpenAI 推出的 AI 编程助手，可与开发环境集成，帮助编写、调试和管理代码。新的远程控制功能建立在 Codex 现有的计算机使用能力之上，使其能够观察并操作 Windows 上的桌面应用。线程协调和扩展搜索是持续改进的一部分，旨在使 Codex 成为更强大的协作工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/codex/remote-connections">Remote connections – Codex | OpenAI Developers</a></li>
<li><a href="https://developers.openai.com/codex/app/features">Features – Codex app | OpenAI Developers</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#remote control`, `#collaboration`, `#developer tools`

---