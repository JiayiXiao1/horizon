---
layout: default
title: "Horizon Summary: 2026-05-15 (ZH)"
date: 2026-05-15
lang: zh
---

> From 36 items, 17 important content pieces were selected

---

1. [首个公开的苹果 M5 内核漏洞利用](#item-1) ⭐️ 9.0/10
2. [Bun 从 Zig 重写为 Rust，已合并](#item-2) ⭐️ 9.0/10
3. [潜伏 18 年的 NGINX 远程代码执行漏洞（CVE-2026-42945）威胁全球数亿服务器](#item-3) ⭐️ 9.0/10
4. [DeepSeek 会话隔离漏洞泄露用户对话](#item-4) ⭐️ 9.0/10
5. [vLLM v0.21.0：KV 卸载、Blackwell 后端、重大变更](#item-5) ⭐️ 8.0/10
6. [移除 2024 款 RAV4 混合动力车的调制解调器和 GPS](#item-6) ⭐️ 8.0/10
7. [RTX 5090 外接显卡搭配 M4 MacBook Air：游戏与 LLM 性能提升](#item-7) ⭐️ 8.0/10
8. [arXiv 对 AI 幻觉参考文献作者实施一年禁令](#item-8) ⭐️ 8.0/10
9. [Anthropic 与 SpaceX 达成大规模 GPU 算力合作](#item-9) ⭐️ 8.0/10
10. [美国放行 H200 对华销售，英伟达寻求突破](#item-10) ⭐️ 8.0/10
11. [京东上线 AI 硬件专区，上架受制裁 NVIDIA GPU](#item-11) ⭐️ 8.0/10
12. [Codex 现已在 ChatGPT 移动应用中免费提供](#item-12) ⭐️ 7.0/10
13. [MIT 校长就资金与人才管道危机发表讲话](#item-13) ⭐️ 7.0/10
14. [CSP 允许列表实验：动态域名白名单](#item-14) ⭐️ 7.0/10
15. [发达国家肥胖率趋稳，中低收入国家仍在上升](#item-15) ⭐️ 7.0/10
16. [ChatGPT 安卓版拆解发现 Codex 远程桌面功能](#item-16) ⭐️ 7.0/10
17. [中国与波音磋商至多 500 架 737 MAX 订单](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [首个公开的苹果 M5 内核漏洞利用](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

一个安全研究团队发布了首个针对苹果 M5 芯片的内核内存破坏漏洞利用，并附有一份 55 页的技术报告。 该漏洞利用表明，即使苹果最新的 M5 芯片配备了 MTE 等先进缓解措施，仍可能被攻破，凸显了持续存在的安全挑战，并可能影响漏洞赏金估值。 该漏洞利用在一周内攻破了最佳防护，报告详细说明了漏洞如何绕过内存标签扩展（MTE）。在苹果漏洞赏金平台上，该漏洞利用估值约为 10 万美元，但如果包装得当，可能达到 150 万美元。

hackernews · quadrige · May 14, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48139219)

**背景**: 苹果 M5 是苹果最新的基于 ARM 的 SoC，采用第三代 3 纳米工艺，配备带有神经加速器的 10 核 GPU。内核内存破坏漏洞利用针对操作系统核心以获取更高权限，而 MTE 是一种旨在检测内存安全错误的硬件缓解措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://www.apple.com/newsroom/2025/10/apple-unleashes-m5-the-next-big-leap-in-ai-performance-for-apple-silicon/">Apple unleashes M5, the next big leap in AI performance for Apple silicon - Apple</a></li>

</ul>
</details>

**社区讨论**: 评论者反应不一：有人称赞这一技术成就并期待报告，也有人质疑漏洞如何绕过 MTE。关于漏洞赏金价值的讨论中，估值从 10 万美元到 150 万美元不等。一条讽刺评论暗示苹果可能捏造漏洞以炒作 Mythos，还有用户后悔专门为 MIE 购买了 M5。

**标签**: `#macOS`, `#kernel exploit`, `#Apple M5`, `#security`, `#memory corruption`

---

<a id="item-2"></a>
## [Bun 从 Zig 重写为 Rust，已合并](https://github.com/oven-sh/bun/pull/30412) ⭐️ 9.0/10

Bun 的核心已从 Zig 重写为 Rust，生成了超过 100 万行 Rust 代码，该拉取请求已合并到主分支。 此次重写标志着广泛使用的 JavaScript 运行时 Bun 的重大架构转变，有望提高内存安全性和性能，同时减少释放后使用和双重释放等错误。 重写大约花费了一周的积极编码时间，但之前进行了大量准备，包括将 Zig 惯用法详细映射到 Rust 等效项。代码库现在包含超过 100 万行 Rust，在 736 个文件中约有 10,428 个 unsafe 块。

hackernews · Chaoses · May 14, 08:15 · [社区讨论](https://news.ycombinator.com/item?id=48132488)

**背景**: Bun 是一个快速的全能 JavaScript 运行时，包含打包器、转译器、任务运行器和 npm 客户端。它最初用 Zig 编写，Zig 是一种专注于健壮性和最优性的系统编程语言。Rust 是另一种以无需垃圾回收的内存安全性而闻名的系统语言。此次重写将 Bun 从 Zig 迁移到 Rust，利用 Rust 的所有权模型来防止常见的内存错误。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了 Zig 和 Rust 惯用法之间令人印象深刻的准备和映射，一些人指出代码库大小接近 Rust 编译器。有人对大量 unsafe 块表示担忧，但 Bun 维护者解释说，Rust 消除了 Zig 版本中常见的许多内存错误。

**标签**: `#Bun`, `#Rust`, `#JavaScript Runtime`, `#Software Rewrite`, `#Systems Programming`

---

<a id="item-3"></a>
## [潜伏 18 年的 NGINX 远程代码执行漏洞（CVE-2026-42945）威胁全球数亿服务器](https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability) ⭐️ 9.0/10

2026 年 5 月 13 日披露了 NGINX 重写模块中一个自 2008 年就存在的严重堆缓冲区溢出漏洞（CVE-2026-42945，CVSS 9.2），影响 0.6.27 至 1.30.0 所有版本及多个企业级产品。修复版本已发布在 NGINX 1.31.0 和 1.30.1 中。 该漏洞允许未经身份验证的攻击者在 NGINX 工作进程上远程执行代码，可能危及云原生环境、Kubernetes Ingress 和 API 网关中使用的数十亿台服务器。18 年的潜伏期凸显了在遗留 C 代码中检测细微内存安全漏洞的难度。 该漏洞源于 NGINX 两遍脚本引擎的状态不一致：包含'?'的重写后`is_args`标志未重置，导致第一遍分配缓冲区空间不足，而第二遍写入转义字符（如'+'扩展为 3 字节）。利用需要特定配置，即同时使用`rewrite`和`set`指令且包含未命名捕获组。

telegram · zaihuapd · May 14, 02:41

**背景**: NGINX 是一款广泛使用的开源 Web 服务器和反向代理，常部署为 Kubernetes Ingress 控制器或 API 网关。重写模块使用两遍引擎处理 URL 重写：第一遍计算缓冲区大小，第二遍拷贝数据。当大小计算低估实际写入数据量时，就会发生堆缓冲区溢出，攻击者可能覆盖相邻内存并执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability">NGINX Rift: Achieving NGINX Remote Code Execution via... | depthfirst</a></li>
<li><a href="https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html">18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/18-year-old-nginx-vulnerability-allows-dos-potential-rce/">18-year-old NGINX vulnerability allows DoS, potential RCE</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，已发布的利用代码禁用了 ASLR，但研究人员声称存在可靠的绕过方法。一些用户建议使用命名捕获组作为缓解措施，而另一些用户则讨论在启用 ASLR 的实际部署中利用的可行性。

**标签**: `#security`, `#nginx`, `#vulnerability`, `#rce`, `#cve`

---

<a id="item-4"></a>
## [DeepSeek 会话隔离漏洞泄露用户对话](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 9.0/10

DeepSeek 对话系统存在会话隔离漏洞，攻击者在空对话中输入未闭合的 <think 字符串即可获取其他用户的对话片段。 该漏洞可能泄露代码、密钥和隐私等敏感用户数据，影响广泛使用的 AI 聊天机器人 DeepSeek 的 Web 和 API 用户。 攻击方式是在全新的空对话中发送未闭合的 <think 字符串，导致模型返回其他用户的对话历史片段。报告者 cancat2024 于 2026 年 5 月 11 日负责任地披露了该漏洞。

telegram · zaihuapd · May 14, 13:15

**背景**: DeepSeek 是由中国公司 DeepSeek 开发的生成式 AI 聊天机器人，于 2025 年 1 月发布。会话隔离是一种安全机制，确保每个用户的数据相互独立；该机制失效会导致跨用户数据泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(chatbot)">DeepSeek (chatbot) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，第三方部署也存在此问题，表明这可能是模型幻觉而非纯粹的隔离缺陷。

**标签**: `#security`, `#vulnerability`, `#AI`, `#DeepSeek`, `#data leak`

---

<a id="item-5"></a>
## [vLLM v0.21.0：KV 卸载、Blackwell 后端、重大变更](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 引入了带混合内存分配器的 KV 缓存卸载、面向 NVIDIA Blackwell GPU 的新 TOKENSPEED_MLA 注意力后端，以及尊重思考预算的推测解码。同时弃用了 transformers v4 并将 C++构建要求提升至 C++20。 这些特性显著提升了大型语言模型的内存效率和推理速度，尤其是在 Blackwell 硬件上。重大变更可能要求用户更新构建环境和模型加载代码。 带 HMA 的 KV 卸载支持滑动窗口组和通过 MooncakeStoreConnector 的分布式卸载。TOKENSPEED_MLA 后端针对 Blackwell GPU 上的 DeepSeek-R1 和 Kimi-K25 模型进行了优化。推测解码现在能在设置思考预算时正确限制推理 token 数量。

github · khluu · May 14, 23:15

**背景**: vLLM 是一个高吞吐量的 LLM 推理引擎，通过管理 KV 缓存来减少内存使用。KV 缓存在 GPU 内存不足时将数据卸载到 CPU 内存。推测解码使用较小的草稿模型加速生成 token，但之前忽略了推理模型的思考预算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/hybrid_kv_cache_manager/">Hybrid KV Cache Manager - vLLM</a></li>
<li><a href="https://vllm-project.github.io/2026/01/08/kv-offloading-connector.html">Inside vLLM’s New KV Offloading Connector: Smarter Memory ...</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/39573">[Bug]: Thinking token budget not enforced with MTP ... - GitHub</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#breaking changes`, `#speculative decoding`

---

<a id="item-6"></a>
## [移除 2024 款 RAV4 混合动力车的调制解调器和 GPS](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

一篇详细指南发布，指导如何从 2024 款 RAV4 混合动力车上物理移除数据通信模块（DCM）和内置 GPS，以阻止遥测数据收集。 这使车主能够直接控制车辆的数据隐私，绕过企业的选择退出政策，并凸显了联网汽车功能与用户隐私之间日益紧张的关系。 移除调制解调器后，蓝牙配对仍允许车辆使用手机网络发送遥测数据；建议改用有线 USB CarPlay，但 CarPlay 本身也会收集车辆数据。

hackernews · arkadiyt · May 14, 17:08 · [社区讨论](https://news.ycombinator.com/item?id=48138136)

**背景**: 像 RAV4 这样的现代车辆配备了远程信息处理单元，持续向制造商传输驾驶数据。丰田的 Safety Connect 及类似服务会收集位置、速度等指标，如果车主选择加入，这些数据常会与保险公司等第三方共享。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/">Removing the Modem and GPS from my 2024 RAV4 Hybrid</a></li>
<li><a href="https://www.cryptogon.com/?p=75142">cryptogon.com » “Removing the Modem and GPS from my 2024 RAV4 ...</a></li>
<li><a href="https://conzit.com/post/taking-control-disabling-data-tracking-in-2024-rav4-hybrid">Taking Control: Disabling Data Tracking in 2024 RAV4 Hybrid</a></li>

</ul>
</details>

**社区讨论**: 评论者提到了替代方法，如移除福特 Maverick 的保险丝，并讨论了丰田是否仅在车主选择加入时才与保险公司共享数据。一些人对丰田否认影响 CarPlay 导航的 GPS 问题表示失望。

**标签**: `#privacy`, `#automotive`, `#telematics`, `#hardware hacking`, `#data ownership`

---

<a id="item-7"></a>
## [RTX 5090 外接显卡搭配 M4 MacBook Air：游戏与 LLM 性能提升](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

一位开发者通过 Thunderbolt 将 NVIDIA RTX 5090 外接显卡成功连接到 M4 MacBook Air，实现了可玩的游戏体验和大幅提升的 LLM 推理速度。该方案通过自定义 Linux 虚拟机与 GPU 直通技术，绕过了苹果官方对 Apple Silicon 外接显卡的不支持限制。 这一突破表明外接显卡可以在 Apple Silicon 上工作，有望扩展 Mac 的游戏和 AI 能力。同时，它为 Mac 用户提供了一条实用路径，使其能够使用高端 NVIDIA GPU 进行 LLM 推理，解决了苹果统一内存的提示处理瓶颈。 该方案使用带有 GPU 直通的 Linux 虚拟机，由于 macOS 限制，GPU 内存仅限 1.5 GB 窗口。游戏基准测试显示可玩的帧率，LLM 提示处理速度相比原生 Apple Silicon 大幅提升。

hackernews · allenleee · May 14, 15:47 · [社区讨论](https://news.ycombinator.com/item?id=48137145)

**背景**: Apple Silicon Mac 将 CPU 和 GPU 集成在单一芯片上并采用统一内存，这对许多任务有利，但阻止了外接显卡支持。外接显卡仅在 Intel 版 Mac 上获得官方支持，且仅限 AMD GPU。NVIDIA GPU 从未在 macOS 上获得官方支持。该项目使用自定义 Linux 虚拟机绕过这些限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.aimadetools.com/blog/llm-inference-apple-silicon/">LLM Inference on Apple Silicon — M4 Performance Guide (2026)</a></li>
<li><a href="https://egpu.io/setup-guide-external-graphics-card-mac/">The Beginner’s External Graphics Card Setup Guide for Mac | eGPU.io</a></li>

</ul>
</details>

**社区讨论**: 社区对这一技术成就印象深刻，许多人指出 LLM 推理改进是最实用的好处。一些评论者对苹果缺乏官方外接显卡支持表示失望，而另一些人则建议使用 Vulkan 转换层等替代方案来玩游戏。

**标签**: `#eGPU`, `#Mac gaming`, `#LLM inference`, `#Apple Silicon`, `#RTX 5090`

---

<a id="item-8"></a>
## [arXiv 对 AI 幻觉参考文献作者实施一年禁令](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv 推出新政策，对提交包含 AI 幻觉参考文献的论文的作者实施一年禁令，之后要求后续提交必须先被知名同行评审场所接受。 该政策直接应对学术出版中日益严重的 AI 生成不准确性问题，强化了学术交流的诚信和信任。 禁令持续一年，之后作者必须让论文被知名同行评审场所接受后才能发布到 arXiv。据报道，该政策已于本周开始执行。

hackernews · gjuggler · May 14, 20:39 · [社区讨论](https://news.ycombinator.com/item?id=48140922)

**背景**: AI 幻觉指的是大型语言模型生成听起来合理但虚假的信息，包括引用不存在的论文。这已成为学术出版中的一个重要问题，研究发现顶级会议如 NeurIPS 接受的论文中也存在幻觉引用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://byteiota.com/arxiv-bans-authors-1-year-for-ai-hallucinated-citations/">arXiv Bans Authors 1 Year for AI-Hallucinated Citations</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC13051339/">Hallucinated citations produced by generative artificial ...</a></li>
<li><a href="https://spylab.ai/blog/hallucinations/">Trends in LLM-Generated Citations on arXiv - SPY Lab</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多表示支持，一位用户称该政策“对科学非常有益”，另一位表示如果作者不仔细检查 LLM 输出，就不值得阅读。一些人警告在采取不利行动前需要仔细审查，而另一些人则指出 LLM 爱好者对该政策感到愤怒。

**标签**: `#arXiv`, `#academic integrity`, `#AI-generated content`, `#hallucinations`, `#policy`

---

<a id="item-9"></a>
## [Anthropic 与 SpaceX 达成大规模 GPU 算力合作](https://t.me/zaihuapd/41371) ⭐️ 8.0/10

Anthropic 宣布与 SpaceX 达成合作，将使用 xAI 的 Colossus 1 数据中心全部算力，一个月内获得超过 300 兆瓦电力和逾 22 万块 NVIDIA GPU。因此，Claude Code 的 Pro 和 Max 套餐速率限制翻倍，Claude Opus 的 API 速率限制也显著提高。 这笔交易大幅扩展了 Anthropic 的计算能力，使 Claude 的模型训练和推理更快，直接惠及依赖 Claude Code 和 Claude API 的开发者与企业。这也标志着 AI 行业基础设施扩展的趋势，获取大规模 GPU 集群成为关键竞争优势。 Colossus 1 数据中心由 xAI 在田纳西州孟菲斯建造，是目前世界上最大的 AI 超级计算机。该合作使 Anthropic 独家获得其全部 300 兆瓦容量和超过 22 万块 NVIDIA GPU，并立即提升了 Claude 的服务限制。

telegram · zaihuapd · May 14, 00:57

**背景**: Anthropic 开发了 Claude 系列大语言模型，包括 Claude Code（一个智能编码工具）和 Claude Opus（最强模型）。Colossus 1 是由 xAI 建造的超级计算机，归 SpaceX 和 Elon Musk 所有，主要用于训练 Grok 聊天机器人。此次合作为 Anthropic 提供了大规模计算资源以扩展其 AI 服务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.datacenterdynamics.com/en/news/anthropic-to-use-all-of-spacex-xais-colossus-1-data-center-compute/">Anthropic to use all of SpaceX-xAI's Colossus 1 data center ...</a></li>
<li><a href="https://greyjournal.net/news/anthropic-spacex-colossus-deal/">Anthropic Rents All of SpaceX’s Colossus 1 Data Center</a></li>

</ul>
</details>

**标签**: `#Anthropic`, `#SpaceX`, `#AI Infrastructure`, `#Claude`, `#GPU`

---

<a id="item-10"></a>
## [美国放行 H200 对华销售，英伟达寻求突破](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 8.0/10

美国商务部已批准向约 10 家中国企业销售英伟达 H200 芯片，包括阿里巴巴和腾讯，单一客户最多可购买 7.5 万颗。 这一批准标志着美国对华先进 AI 芯片出口管制可能发生转变，影响全球 AI 硬件供应链以及美国芯片出口与中国国产 AI 芯片发展之间的平衡。 尽管获得批准，但尚未有任何交付完成，中国企业在北京方面的指导下持谨慎态度。英伟达 CEO 黄仁勋访华被视为推动交易落地的重要尝试。

telegram · zaihuapd · May 14, 08:57

**背景**: H200 是英伟达基于 Hopper 架构的最新 GPU，配备 141 GB HBM3e 内存和 4.8 TB/s 带宽，容量几乎是 H100 的两倍。美国此前实施严格出口管制，限制中国获取先进 AI 芯片，旨在遏制其 AI 和国防发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.runpod.io/articles/guides/nvidia-h200-gpu">Nvidia H200 GPU: Specs, VRAM, Price, and AI Performance</a></li>
<li><a href="https://www.linkedin.com/pulse/us-tightens-export-controls-ai-chips-china-dusan-simic-urqvf">US Tightens Export Controls on AI Chips to China</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#AI hardware`, `#US-China trade`, `#NVIDIA`, `#export controls`

---

<a id="item-11"></a>
## [京东上线 AI 硬件专区，上架受制裁 NVIDIA GPU](https://u.jd.com/HaDkFMa) ⭐️ 8.0/10

京东开设了“AI 硬件京东自营专区”，首批上架了 NVIDIA GeForce RTX 5090 32G 涡轮版、RTX PRO 6000 Blackwell 工作站版以及 H100 等 GPU，这些产品此前因出口限制而暂停对华销售。 此举大幅提升了中国获取高端 AI 硬件的渠道，可能推动本土 AI 发展，并绕开此前的出口管制。这标志着硬件可用性的转变，可能影响全球 AI 供应链。 RTX 5090 涡轮版为全球统一规格，无性能阉割；RTX PRO 6000 配备 96GB GDDR7 ECC 显存，面向专业渲染和数据中心。H100 此前因制裁而暂停对华出口。

telegram · zaihuapd · May 14, 15:15

**背景**: 美国政府对中国实施了先进 AI 芯片的出口限制，包括 NVIDIA 的 H100 和 A100 GPU，以限制中国的 AI 能力。京东是中国主要的电商平台，其自营专区确保产品正品和可靠供应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/">GeForce RTX 50 Series Graphics Cards | NVIDIA</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/professional-desktop-gpus/rtx-pro-6000/">NVIDIA RTX PRO 6000 Blackwell Workstation Edition</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h100/">H 100 GPU | NVIDIA</a></li>

</ul>
</details>

**标签**: `#AI hardware`, `#NVIDIA`, `#export restrictions`, `#China`, `#GPU`

---

<a id="item-12"></a>
## [Codex 现已在 ChatGPT 移动应用中免费提供](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 7.0/10

OpenAI 已将其 AI 编程代理 Codex 免费集成到 ChatGPT 移动应用中，使用户能够随时随地进行代码编写和调试。 此次扩展将强大的 AI 辅助编程功能带到移动设备，有望提升开发者生产力，并使编程辅助惠及更广泛的用户群体。 Codex 包含在 ChatGPT 的免费套餐中，但用户交互数据可能用于训练。移动端体验可能受限于屏幕尺寸和缺乏键盘，导致与桌面端相比效果参差不齐。

hackernews · mikeevans · May 14, 20:06 · [社区讨论](https://news.ycombinator.com/item?id=48140529)

**背景**: Codex 是 OpenAI 推出的一套 AI 驱动编程代理，可自动化软件工程任务。它可通过 CLI、桌面应用或现在的 ChatGPT 移动应用使用，支持远程控制和本地执行等功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/openai/codex/releases">Releases · openai / codex</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai / codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**社区讨论**: 社区成员对 Codex 免费感到惊讶，有人指出它包含在免费套餐中。用户反映移动端因屏幕和输入限制效果参差不齐，部分人希望更好地集成本地文件和提供 Linux 支持。

**标签**: `#AI`, `#code generation`, `#mobile app`, `#OpenAI`, `#developer tools`

---

<a id="item-13"></a>
## [MIT 校长就资金与人才管道危机发表讲话](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 7.0/10

MIT 校长 Sally Kornbluth 发布视频讲话，探讨研究资金和人才管道面临的挑战，指出学术界普遍存在的幻灭感。 这一讲话标志着学术界面临系统性危机——资金减少和职业前景黯淡正迫使博士毕业生离开科研岗位，可能削弱美国的科学领导地位。 理科博士平均耗时六年，工作艰辛且薪酬微薄，尽管最初怀有学术志向，但大多数应届毕业生正考虑离开学术界。

hackernews · dmayo · May 14, 14:51 · [社区讨论](https://news.ycombinator.com/item?id=48136262)

**背景**: 美国科研体系高度依赖联邦拨款和稳定的博士人才输送。然而，资金停滞、成本上升以及就业市场紧缩导致早期职业研究人员的不满情绪日益增长，威胁到学术研究的长期健康发展。

**社区讨论**: 评论者表达了多元观点：有人指出学术模式已破裂并面临代际重置，也有人认为博士进入工业界并非浪费。少数人提到中国在教育领域的崛起构成了竞争挑战。

**标签**: `#academia`, `#research funding`, `#talent pipeline`, `#higher education`

---

<a id="item-14"></a>
## [CSP 允许列表实验：动态域名白名单](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一个实验，通过在沙箱 iframe 中拦截 fetch 错误并提示用户批准，动态地将域名添加到内容安全策略（CSP）允许列表中。 这种方法提供了一种用户友好的方式来管理 CSP 限制而不破坏功能，可能通过减少对过于宽松策略的需求来改进 Web 安全实践。 该实验在沙箱 iframe 内使用自定义 fetch() 来捕获 CSP 违规，然后将被阻止的源传递给父窗口，父窗口显示一个对话框，询问用户是否将该域名添加到允许列表并刷新页面。

rss · Simon Willison · May 13, 04:50

**背景**: 内容安全策略（CSP）是一种浏览器安全机制，限制页面可以加载的资源，有助于防止跨站脚本（XSS）攻击。传统上，CSP 策略是静态的，当需要新的源时需要手动更新，这可能导致策略过于宽松或功能损坏。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/13/csp-allow/">Tool: CSP Allow-list Experiment - simonwillison.net</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP">Content Security Policy (CSP) - HTTP | MDN - MDN Web Docs</a></li>

</ul>
</details>

**标签**: `#CSP`, `#web security`, `#sandbox`, `#iframe`, `#experiment`

---

<a id="item-15"></a>
## [发达国家肥胖率趋稳，中低收入国家仍在上升](https://www.nature.com/articles/s41586-026-10383-0) ⭐️ 7.0/10

一项覆盖 200 个国家、2.32 亿人的大规模研究发现，高收入国家儿童青少年肥胖率自 1990 年代起增速放缓，2000 年后大多趋于稳定，意大利、葡萄牙、法国等国甚至出现小幅下降；而中低收入国家的肥胖率仍在持续稳定或加速上升。 这项研究揭示了全球肥胖趋势的转变，表明富裕国家的社会经济和政策因素可能遏制了肥胖流行，而较贫穷国家正面临日益加重的负担。研究结果强调，中低收入国家需要采取有针对性的干预措施，以防止进一步的健康和经济影响。 该研究分析了 1980 年至 2024 年的数据，覆盖 200 个国家和 2.32 亿人。在一些高收入国家，成人肥胖率在最初上升后也趋于平稳，而中低收入国家的肥胖率在某些情况下已超过富裕国家。

telegram · zaihuapd · May 14, 09:45

**背景**: 肥胖是糖尿病、心脏病和某些癌症等慢性疾病的主要风险因素。研究认为，受社会、经济和技术变化影响的食物可得性、负担能力和使用方式等因素可能帮助高收入国家遏制了肥胖上升，但低收入地区尚未取得类似进展。

**标签**: `#public health`, `#obesity`, `#global health`, `#epidemiology`

---

<a id="item-16"></a>
## [ChatGPT 安卓版拆解发现 Codex 远程桌面功能](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

对 ChatGPT 安卓版 1.2026.125 的 APK 拆解发现，OpenAI 正在为 Codex 开发远程桌面控制功能，允许用户通过手机查找和重连远程会话。 该功能将极大扩展 Codex 的实用性，使开发者能够通过移动设备远程管理编码任务，有望提高生产力并让 AI 辅助开发更加便捷。 该功能仍在开发中，尚无可用预览，且要求桌面端登录与移动设备相同的账号。官方发布日期尚未公布。

telegram · zaihuapd · May 14, 21:48

**背景**: OpenAI Codex 是一款旨在自动化软件工程任务的 AI 代理，例如构建功能和重构代码。APK 拆解是指反编译安卓应用的安装文件以检查其代码和资源，通常能揭示尚未公开的即将推出的功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex">OpenAI Codex - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#Android`, `#remote desktop`, `#AI`

---

<a id="item-17"></a>
## [中国与波音磋商至多 500 架 737 MAX 订单](https://t.me/zaihuapd/41389) ⭐️ 7.0/10

中国与波音正在磋商一笔至多 500 架波音 737 MAX 的潜在订单，这将是近十年来中国首次向波音下达重大飞机订单，预计在特朗普访华期间公布。 这笔交易将标志着中美贸易紧张局势的重大缓和，并为波音 737 MAX 项目带来重大提振，该项目此前面临安全和生产挑战。 谈判还包括约 100 架波音 787 和 777X 宽体机，但可能稍后单独宣布。交易尚未最终敲定，宣布方式及是否形成具有约束力的正式承诺仍在协商中。

telegram · zaihuapd · May 15, 01:09

**背景**: 波音 737 MAX 是一款窄体客机系列，在 2019 年 3 月至 2020 年 11 月期间因两起与 MCAS 系统相关的致命坠机事故而全球停飞。中国是首个停飞 MAX 的国家，并因中美贸易紧张局势而放缓了交付和订单。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Boeing`, `#China`, `#aviation`, `#trade`, `#737 MAX`

---