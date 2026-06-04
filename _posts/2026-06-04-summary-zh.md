---
layout: default
title: "Horizon Summary: 2026-06-04 (ZH)"
date: 2026-06-04
lang: zh
---

> From 35 items, 19 important content pieces were selected

---

1. [Elixir v1.20 引入渐进类型系统](#item-1) ⭐️ 9.0/10
2. [蓝牙音箱被黑，通过 USB 注入按键](#item-2) ⭐️ 9.0/10
3. [HTTP/2 炸弹攻击可远程瘫痪主流服务器](#item-3) ⭐️ 9.0/10
4. [谷歌发布 Gemma 4 12B，无编码器多模态模型](#item-4) ⭐️ 8.0/10
5. [特德·姜：人工智能没有意识](#item-5) ⭐️ 8.0/10
6. [DaVinci Resolve 21 新增照片管理和动态图形功能](#item-6) ⭐️ 8.0/10
7. [Uber 将每款 AI 工具的月代币支出上限设为 1500 美元](#item-7) ⭐️ 8.0/10
8. [Let's Encrypt 计划迁移至后量子证书](#item-8) ⭐️ 8.0/10
9. [乐鑫 ESP32-S31：集成 SIMD 指令和 BitScrambler 的 RISC-V 芯片](#item-9) ⭐️ 8.0/10
10. [数学家警告 AI 快速进展的风险](#item-10) ⭐️ 8.0/10
11. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash](#item-11) ⭐️ 8.0/10
12. [SpaceX 拟以每股 135 美元 IPO，筹资 750 亿美元](#item-12) ⭐️ 8.0/10
13. [谷歌允许网站退出 AI 搜索结果](#item-13) ⭐️ 8.0/10
14. [开发者分享抗 NMDA 受体脑炎诊断经历](#item-14) ⭐️ 7.0/10
15. [原始 PlayStation 架构深度解析](#item-15) ⭐️ 7.0/10
16. [何时字节优化真正重要：AoS 与 SoA 对比](#item-16) ⭐️ 7.0/10
17. [3 月 4 日 GFW 大规模封禁代理服务](#item-17) ⭐️ 7.0/10
18. [千问向第三方 Agent 和 Skill 全面开放平台](#item-18) ⭐️ 7.0/10
19. [美国教师工会呼吁限制小学 AI 与屏幕使用](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Elixir v1.20 引入渐进类型系统](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20 于 2026 年 6 月 3 日发布，引入了渐进类型系统，允许开发者选择性地为代码添加类型注解以进行静态类型检查，同时保持完全动态类型的兼容性。 这标志着 Elixir 的范式转变，满足了社区长期以来对静态类型的需求，并可能吸引那些因缺乏类型安全而此前避免使用该语言的开发者。 渐进类型系统作为可选功能实现，现有的无类型代码仍然完全有效。初始版本专注于核心类型检查，更高级的功能计划在后续版本中推出。

hackernews · cloud8421 · Jun 3, 19:02 · [社区讨论](https://news.ycombinator.com/item?id=48388324)

**背景**: 渐进类型系统允许程序部分动态类型化、部分静态类型化，通过类型注解的有无来控制。Elixir 此前依赖 Dialyzer 进行可选的静态分析，但 v1.20 将原生类型检查直接集成到编译器中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing - Wikipedia</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>
<li><a href="https://www.ituonline.com/tech-definitions/what-is-gradual-typing/">What Is Gradual Typing ? - ITU Online IT Training</a></li>

</ul>
</details>

**社区讨论**: 社区普遍持积极态度，许多长期使用 Elixir 的开发者表示兴奋。一些用户将新系统与 Dialyzer 的成功类型方法进行比较，而另一些则讨论渐进类型对性能的影响及其对无类型与有类型语言争论的影响。

**标签**: `#Elixir`, `#gradual typing`, `#functional programming`, `#programming languages`, `#type systems`

---

<a id="item-2"></a>
## [蓝牙音箱被黑，通过 USB 注入按键](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 9.0/10

一名研究人员展示了一种新型攻击方式，通过蓝牙无线重写 Creative Sound Blaster Katana V2X 音箱的固件，将其变成 USB 键盘，从而向连接的 PC 注入按键。 这种攻击绕过了传统安全措施，因为音箱是受信任的 USB 设备，且重写固件无需认证或用户交互，使其成为隐蔽的按键注入攻击向量。 该音箱的蓝牙固件更新过程缺乏有效认证，允许写入任意固件。研究人员在固件中添加了 USB HID 键盘描述符，使音箱能够模拟键盘。

hackernews · xx_ns · Jun 3, 10:53 · [社区讨论](https://news.ycombinator.com/item?id=48382310)

**背景**: 按键注入攻击（如使用 USB Rubber Ducky 设备）利用了操作系统对人机交互设备（HID）的信任。BadUSB 攻击涉及重编程 USB 设备的固件以充当键盘。这项研究将这一概念扩展到可通过无线方式重编程的外设。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.opswat.com/blog/the-danger-of-a-usb-device-and-keystroke-injection-attack">The Danger of a USB Device and Keystroke Injection Attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/BadUSB_attack">BadUSB attack</a></li>

</ul>
</details>

**社区讨论**: 评论者批评 Creative 公司否认该漏洞构成网络安全风险，并指出供应链中可能存在蠕虫传播。一些人指出攻击需要蓝牙物理接近，但另一些人认为缺乏认证是严重缺陷。

**标签**: `#security`, `#firmware`, `#bluetooth`, `#badusb`, `#hardware hacking`

---

<a id="item-3"></a>
## [HTTP/2 炸弹攻击可远程瘫痪主流服务器](https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb) ⭐️ 9.0/10

研究人员披露了一种名为 HTTP/2 炸弹的新型远程拒绝服务攻击，该攻击利用 HPACK 压缩和慢速连接占用，以极低带宽瘫痪 NGINX、Apache、IIS、Envoy 和 Pingora 等主流服务器。 该攻击可在一台机器和 100 Mbps 连接下在数秒内瘫痪主流服务器，对互联网基础设施构成严重威胁。它暴露了 HTTP/2 实现的脆弱性，凸显了紧急修补的必要性。 100 Mbps 家用网络可在数秒内让部分服务器不可用；Apache httpd 和 Envoy 单个客户端约 20 秒可占住 32 GB 内存。NGINX 已在 1.29.8+ 修复，Apache 在 mod_http2 v2.0.41 修复，而 IIS、Envoy 和 Pingora 暂无补丁。

telegram · zaihuapd · Jun 3, 15:00

**背景**: HTTP/2 使用 HPACK 压缩来减少头部开销，但可能被滥用，将小输入放大为大量内存分配。Slowloris 是一种经典攻击，通过保持大量不完整请求的连接来耗尽服务器资源。HTTP/2 炸弹结合了这两种技术：一个字节的线缆数据触发大量头部分配，同时慢速发送保持连接存活，导致内存耗尽。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb">Codex Discovered a Hidden HTTP / 2 Bomb - Calif</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-http-2-bomb-dos-attack-crashes-web-servers-in-under-a-minute/">New ' HTTP / 2 Bomb ' DoS attack crashes web servers in under a minute</a></li>
<li><a href="https://blog.cloudflare.com/hpack-the-silent-killer-feature-of-http-2/">HPACK: the silent killer (feature) of HTTP/2</a></li>

</ul>
</details>

**标签**: `#security`, `#HTTP/2`, `#DoS`, `#web servers`, `#vulnerability`

---

<a id="item-4"></a>
## [谷歌发布 Gemma 4 12B，无编码器多模态模型](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 8.0/10

Google DeepMind 于 2026 年 6 月 3 日发布了 Gemma 4 12B，这是一个开放权重的多模态模型，用轻量级嵌入模块取代了传统的视觉编码器，使视觉和音频输入能够直接集成到语言模型中。 这种无编码器架构降低了延迟和内存使用，使模型能够在配备 16GB VRAM 的消费级笔记本电脑上运行，同时性能接近更大的 26B 模型。这为开发者和研究人员普及了先进的多模态 AI。 该模型使用一个 35M 参数的嵌入层（单次矩阵乘法、位置嵌入和归一化），而不是像 SigLIP 这样的专用视觉编码器。它支持文本、图像和音频输入，并在 Hugging Face 上提供预训练和指令微调版本。

hackernews · rvz · Jun 3, 16:04 · [社区讨论](https://news.ycombinator.com/item?id=48385906)

**背景**: 传统的多模态模型使用单独的编码器（例如用于视觉的 SigLIP）将非文本输入转换为语言模型的表示，这增加了延迟和内存开销。Gemma 4 12B 的无编码器设计直接在语言模型中处理所有模态，简化了架构并提高了效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/">Introducing Gemma 4 12 B</a></li>
<li><a href="https://huggingface.co/google/gemma-4-12B">google/ gemma - 4 - 12 B · Hugging Face</a></li>
<li><a href="https://techstartups.com/2026/06/03/google-deepmind-launches-gemma-4-12b-bringing-frontier-ai-model-to-everyday-laptops/">Google launches Gemma 4 12B, bringing frontier AI model to ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些用户报告在编码基准测试中表现尚可，尽管存在轻微语法错误；而另一些用户则质疑 35M 嵌入层的鲁棒性，并指出图像处理质量较差。此外，关于谷歌发布开放模型的战略动机也存在争议。

**标签**: `#multimodal`, `#encoder-free`, `#Gemma`, `#Google`, `#AI`

---

<a id="item-5"></a>
## [特德·姜：人工智能没有意识](https://www.theatlantic.com/philosophy/2026/06/no-artificial-intelligence-is-not-conscious/687378/) ⭐️ 8.0/10

特德·姜在《大西洋月刊》发表文章，认为大型语言模型（LLM）没有意识，强调类人行为与主观体验之间的区别。 这篇文章重新点燃了关于人工智能意识的辩论，影响了公众讨论和人工智能伦理，尤其是在 LLM 日益融入社会的背景下。 姜认为 LLM 只是下一个词预测器，没有主观体验，而真正的意识需要身体和感官器官。

hackernews · lordleft · Jun 3, 17:51 · [社区讨论](https://news.ycombinator.com/item?id=48387270)

**背景**: 像 GPT-4 这样的大型语言模型（LLM）通过基于训练数据中的模式预测下一个词来生成文本。它们可以产生类人回应，但缺乏理解或意识。自人工智能出现以来，关于 AI 是否能有意识的争论就一直存在。

**社区讨论**: 评论者意见不一：一些人同意 LLM 缺乏意识，而另一些人则认为如果 AI 表现得像有意识，就应该被当作有意识来对待。少数人强调无论是否有意识，AI 对齐和伦理都很重要。

**标签**: `#AI consciousness`, `#philosophy`, `#LLMs`, `#ethics`, `#Ted Chiang`

---

<a id="item-6"></a>
## [DaVinci Resolve 21 新增照片管理和动态图形功能](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design 发布了 DaVinci Resolve 21，新增了专门用于静态图像编辑和管理的照片页面，以及增强的动态图形工具和 AI 功能，如 IntelliSearch 和去老化。 此次更新使 DaVinci Resolve 成为 Adobe Lightroom 和 After Effects 的直接竞争对手，可能颠覆摄影师和动态设计师的现有工作流程。AI 工具的加入也提高了视频编辑的效率。 照片页面包含来自视频侧的高级调色工具、带有 Resolve FX 和 Fusion FX 的效果库，以及用于基于内容搜索图像的 IntelliSearch。动态图形增强利用了 Fusion 页面的节点式工作流程。

hackernews · pentagrama · Jun 3, 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48384482)

**背景**: DaVinci Resolve 是一款专业的视频编辑、调色、视觉特效和音频后期制作软件。它传统上专注于视频，但版本 21 扩展到照片管理和动态图形领域，挑战了 Lightroom 和 After Effects 等专业工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/whatsnew">DaVinci Resolve – What’s New | Blackmagic Design</a></li>
<li><a href="https://documents.blackmagicdesign.com/SupportNotes/DaVinci_Resolve_21_New_Features_Guide.pdf?_v=1776322810000">DaVinci Resolve 21 New Features Guide</a></li>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/fusion">DaVinci Resolve – Fusion | Blackmagic Design</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户称赞照片管理和动态图形新增功能即使没有 AI 功能也意义重大。一些人对 AI 营销炒作感到厌倦，但承认新 AI 工具对编辑工作流程的实际好处。

**标签**: `#video editing`, `#photo management`, `#motion graphics`, `#AI`, `#professional tools`

---

<a id="item-7"></a>
## [Uber 将每款 AI 工具的月代币支出上限设为 1500 美元](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

Uber 在四个月内花光了 2026 年的人工智能预算后，将员工使用 Claude Code 和 Cursor 等 AI 编码工具的月支出上限设为每款工具 1500 美元。该政策仅适用于代理型编码软件，并于近几个月内实施。 这标志着企业 AI 工具使用首次面临重大现实约束，凸显了消耗大量代币的编码代理不可持续的成本动态。这表明即使是资金充足的公司也必须控制 AI 支出，可能影响整个行业的采用和定价策略。 1500 美元的上限适用于每款 AI 编码工具，这意味着同时使用 Cursor 和 Claude Code 的工程师每月最多可花费 3000 美元。以软件工程师年薪中位数 33 万美元计算，该上限约占每位工程师总薪酬的 11%。

rss · Simon Willison · Jun 3, 12:01 · [社区讨论](https://news.ycombinator.com/item?id=48383056)

**背景**: 像 Claude Code 和 Cursor 这样的 AI 编码代理使用大型语言模型自主编写和编辑代码，消耗代币（处理的文本单位），成本取决于模型大小和使用量。Uber 的 2026 年 AI 预算是在 2025 年制定的，当时这些工具尚未爆发式流行，导致迅速超支。个人订阅者通常享受补贴价格，而企业则需支付完整的 API 费率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**社区讨论**: 评论者就 AI 编码工具是昙花一现还是持久变革展开了辩论。一些人认为，更小、更便宜的模型足以完成大多数任务，而大型模型仍会产生混乱的代码，需要大量审查。另一些人则指出，这些工具被迅速采用且每席位支出高昂，证明了其真实价值。还有人质疑，面对 DeepSeek 等中国模型的竞争，AI 提供商是否会维持对个人的补贴定价。

**标签**: `#AI`, `#cost management`, `#coding agents`, `#Uber`, `#LLM economics`

---

<a id="item-8"></a>
## [Let's Encrypt 计划迁移至后量子证书](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 8.0/10

Let's Encrypt 宣布计划采用 Merkle Tree 证书（MTC）迁移至后量子证书，以防范未来量子计算机的攻击。 作为主要的证书颁发机构，Let's Encrypt 的迁移将显著影响 Web PKI 生态系统，推动行业向量子安全密码学发展，并防范“先收集、后解密”的威胁。 在常见情况下，MTC 比当前的 X.509 证书更小，因为它将单个签名、公钥和包含证明合并在一起。这一迁移还使透明度成为颁发本身的属性，简化了证书透明度。

hackernews · SGran · Jun 3, 15:06 · [社区讨论](https://news.ycombinator.com/item?id=48385114)

**背景**: 后量子密码学（PQC）旨在开发能够抵御量子计算机攻击的算法，量子计算机可能利用 Shor 算法破解当前的公钥系统（如 RSA 和 ECDSA）。证书透明度（CT）是一种记录所有颁发证书以检测错误颁发的标准，但当前的 CT 存在包含证明等复杂性。Let's Encrypt 是一个免费、自动化的证书颁发机构，颁发了大量网络证书。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://en.wikipedia.org/wiki/Certificate_Transparency">Certificate Transparency</a></li>

</ul>
</details>

**社区讨论**: 评论者提出了对当前证书透明度存在缺陷以及验证包含证明的挑战的担忧。一些人指出了从 ed25519 等成熟算法迁移的实际困难，而另一些人则称赞 MTC 减少了握手大小并简化了透明度。

**标签**: `#post-quantum cryptography`, `#Let's Encrypt`, `#TLS/SSL`, `#certificate transparency`, `#infrastructure`

---

<a id="item-9"></a>
## [乐鑫 ESP32-S31：集成 SIMD 指令和 BitScrambler 的 RISC-V 芯片](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 8.0/10

乐鑫发布了 ESP32-S31，这是一款双核 32 位 RISC-V 微控制器，主频高达 320 MHz，具备 SIMD 指令和用于灵活数据转换的 BitScrambler 外设。 采用带 SIMD 的 RISC-V 内核使得 Rust 等现代工具链可以无缝使用，降低了嵌入式开发的门槛，并扩展了高性能物联网应用的生态系统。 ESP32-S31 包含 60 个 GPIO，支持 Wi-Fi 6 和千兆以太网，其 BitScrambler 外设可在 DMA 传输期间转换数据，类似于树莓派 Pico 的 PIO。

hackernews · volemo · Jun 3, 16:10 · [社区讨论](https://news.ycombinator.com/item?id=48385965)

**背景**: 乐鑫的 ESP32 系列传统上使用 Tensilica Xtensa 内核。转向 RISC-V 代表了向开放标准 ISA 的迈进，简化了工具链支持并促进了更广泛的社区贡献。SIMD 指令允许并行处理数据，而 BitScrambler 则将位级操作从 CPU 中卸载。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.espressif.com/en/products/socs/esp32-s31">ESP32-S31 Dual-Core RISC-V + Multi-Protocol SoC</a></li>
<li><a href="https://docs.espressif.com/projects/esp-idf/en/stable/esp32p4/api-reference/peripherals/bitscrambler.html">BitScrambler Driver - ESP32-P4 - — ESP-IDF Programming Guide...</a></li>
<li><a href="https://hackaday.com/2026/04/08/espressifs-new-esp32-s31-dual-core-risc-v-with-wifi-6-and-gbit-ethernet/">Espressif’s New ESP32-S31: Dual-Core RISC-V With ... - Hackaday</a></li>

</ul>
</details>

**社区讨论**: 社区对转向 RISC-V 感到兴奋，指出这通过简单的目标三元组简化了 Rust 开发。一些用户对命名感到困惑，因为 ESP32 品牌现在涵盖了许多不同的架构。BitScrambler 被与树莓派 Pico 的 PIO 进行了有利比较。

**标签**: `#ESP32`, `#RISC-V`, `#embedded systems`, `#Rust`, `#hardware`

---

<a id="item-10"></a>
## [数学家警告 AI 快速进展的风险](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

一群数学家就 AI 在数学领域的快速进展发出警告，强调了对证明验证和归属问题的风险。 这一警告凸显了核心数学实践可能受到的冲击，引发了关于人类推理在该领域未来角色的辩论。 数学家们认为，AI 生成和验证证明的能力可能削弱人类监督和适当的归属，尽管一些人看到了人机协作的潜力。

hackernews · pseudolus · Jun 3, 10:05 · [社区讨论](https://news.ycombinator.com/item?id=48382052)

**背景**: 数学传统上依赖人类进行证明验证和归属。大型语言模型（LLM）的最新进展使 AI 能够协助生成和检查证明，引发了对该学科长期影响的担忧。

**社区讨论**: 社区评论表达了不同观点：一些人强调 AI 的“长尾愚蠢”并类比艺术和象棋领域的早期颠覆，而另一些人则担心人类数学家未来变得无关紧要。

**标签**: `#AI`, `#mathematics`, `#research`, `#LLMs`, `#disruption`

---

<a id="item-11"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软宣布了两款新的大语言模型：MAI-Thinking-1，一个拥有 1 万亿参数、35 亿活跃参数的推理模型；以及 MAI-Code-1-Flash，一个拥有 1370 亿参数、50 亿活跃参数的代码模型，后者正在向 VS Code 中的 GitHub Copilot 用户推出。 这些模型展示了微软利用混合专家（MoE）架构推动高效、高性能 AI 的努力，MAI-Thinking-1 声称在盲测中优于 Sonnet 4.6。MAI-Code-1-Flash 在 GitHub Copilot 中的部署可能显著影响开发者生产力和代码生成成本。 这两个模型均基于 MoE 架构，通过大总参数和低活跃参数实现高效。微软声称它们是在干净、商业许可的数据上训练的，没有从第三方模型蒸馏，但技术论文显示训练数据包括专有网络爬取和 Common Crawl，与其他主要 LLM 类似。

rss · Simon Willison · Jun 2, 22:21

**背景**: 混合专家（MoE）是一种机器学习技术，每个输入只激活多个专用子网络（专家），使模型能够扩展参数而不成比例增加计算成本。MAI-Thinking-1 是专为复杂问题解决设计的推理模型，而 MAI-Code-1-Flash 则针对代码生成任务进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI - Thinking - 1 | Microsoft AI</a></li>
<li><a href="https://microsoft.ai/news/introducingmai-code-1-flash/">Introducing MAI-Code-1-Flash | Microsoft AI</a></li>
<li><a href="https://github.blog/changelog/2026-06-02-mai-code-1-flash-is-now-available-for-github-copilot/">MAI-Code-1-Flash is now available for GitHub Copilot</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Microsoft`, `#AI`, `#code generation`, `#reasoning`

---

<a id="item-12"></a>
## [SpaceX 拟以每股 135 美元 IPO，筹资 750 亿美元](https://www.reuters.com/business/media-telecom/spacex-plans-raise-75-billion-ipo-135-per-share-source-says-2026-06-03/) ⭐️ 8.0/10

SpaceX 计划以每股 135 美元的固定价格发行 5.556 亿股，筹资 750 亿美元，预计于 2026 年 6 月 12 日在纳斯达克上市，股票代码为 SPCX。 这将成为史上最大规模的 IPO，可能引发 OpenAI 和 Anthropic 等 AI 公司的巨型 IPO 浪潮，并为 SpaceX 提供资金以扩展 AI 计算和星链网络。 固定价 IPO 极为罕见，因为在路演前就锁定了发行价；细节仍可能调整。SpaceX 去年营收 187 亿美元，但净亏损 49 亿美元，仅星链盈利。

telegram · zaihuapd · Jun 3, 09:01

**背景**: IPO（首次公开募股）是指私人公司首次向公众出售股票。固定价 IPO 是提前设定股价，而非通过簿记建档过程。星链（Starlink）是 SpaceX 运营的卫星互联网星座，为偏远地区提供宽带服务。路演是公司高管向潜在投资者展示公司价值以吸引兴趣的营销活动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://www.zhihu.com/question/19602940">IPO 之前的「路演」具体是怎样的过程？ - 知乎</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#IPO`, `#finance`, `#AI`, `#Starlink`

---

<a id="item-13"></a>
## [谷歌允许网站退出 AI 搜索结果](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 8.0/10

谷歌在 Search Console 中新增一个开关，允许网站所有者选择不显示在 AI 概览和 AI 模式中，且不影响其常规搜索排名和 Discover 流量。 这使发布商能更好地控制其内容在搜索生成式 AI 中的使用方式，回应了关于流量下降和缺乏归属的担忧。它为搜索引擎如何平衡 AI 功能与发布商权益树立了先例。 该退出功能目前正在英国网站中测试，随后将向全球推广。谷歌还在 Search Console 中引入了生成式 AI 搜索统计数据，展示展示量、页面表现和地域数据。

telegram · zaihuapd · Jun 3, 12:00

**背景**: AI 概览是出现在部分谷歌搜索结果顶部的 AI 生成摘要，提供快速答案，用户无需点击进入网站。自推出以来，许多发布商报告流量大幅下降，因此呼吁获得更多控制权。新的退出功能是在英国监管机构裁定和网络出版行业压力日益增大的背景下推出的。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/">Google will let sites opt-out of AI Mode and Overviews in Search</a></li>
<li><a href="https://www.androidheadlines.com/2026/06/google-ai-search-opt-out-publisher-control.html">Google Launches Opt Out for AI Search Overviews and AI Mode</a></li>
<li><a href="https://mashable.com/tech/google-will-allow-websites-to-opt-out-of-ai-overviews">Google will allow websites to opt out of AI overviews</a></li>

</ul>
</details>

**标签**: `#Google`, `#AI`, `#SEO`, `#Search Console`, `#Web Publishing`

---

<a id="item-14"></a>
## [开发者分享抗 NMDA 受体脑炎诊断经历](https://burntsushi.net/encephalitis/) ⭐️ 7.0/10

软件开发者 Andrew Gallant（burntsushi）公开分享了他被诊断为抗 NMDA 受体脑炎的经历，这是一种罕见的自身免疫性脑部疾病，他详细描述了可怕的症状以及获得正确诊断的挑战。 这一亲身经历凸显了罕见的自身免疫性脑炎常被误诊为精神疾病的问题，强调了提高认识和改进诊断工具的必要性。同时，它也强调了生物医学研究在发现严重神经系统症状的可治疗病因方面的关键作用。 抗 NMDA 受体脑炎于 2007 年首次被描述，由抗体攻击大脑中的 NMDA 受体引起。约 80%的患者为女性，约半数病例与肿瘤相关，最常见的是卵巢畸胎瘤。

hackernews · Tomte · Jun 3, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48384355)

**背景**: 抗 NMDA 受体脑炎是一种罕见的自身免疫性疾病，身体的免疫系统产生抗体攻击大脑中的 NMDA 受体，导致炎症。早期症状常类似精神疾病（如精神分裂症），导致频繁误诊。治疗包括免疫抑制和切除肿瘤（如果存在），早期干预可显著改善预后。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anti-NMDA_receptor_encephalitis">Anti-NMDA receptor encephalitis</a></li>
<li><a href="https://www.ncbi.nlm.nih.gov/books/NBK578203/">Autoimmune Encephalitis - StatPearls - NCBI Bookshelf</a></li>
<li><a href="https://www.med.upenn.edu/autoimmuneneurology/nmdar-encephalitis.html">Anti-NMDAR Encephalitis | Center for Autoimmune Neurology ...</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了深切同情，并分享了自身免疫性疾病被误诊的类似经历。一位神经科医生指出，该病非常罕见，容易被误诊为精神疾病，但称赞了治疗作者的优秀神经科中心。其他人则强调了持续进行生物医学研究以发现此类疾病可逆治疗方法的重要性。

**标签**: `#autoimmune disease`, `#medical misdiagnosis`, `#neuroscience`, `#personal story`

---

<a id="item-15"></a>
## [原始 PlayStation 架构深度解析](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 7.0/10

Rodrigo Copetti 发布了对原始 PlayStation 的详细架构分析，涵盖其 MIPS R3000A CPU、GTE、GPU 和 SPU 音频系统。 该分析为复古计算爱好者和模拟器开发者提供了宝贵的见解，帮助他们理解定义 PlayStation 游戏的硬件特性。 文章解释了 GTE 在 3D 几何和光照中的作用、GPU 的基于瓦片的渲染，以及具有 512 KB 专用 RAM 的 24 通道 ADPCM 音频的 SPU。

hackernews · gregsadetsky · Jun 3, 10:24 · [社区讨论](https://news.ycombinator.com/item?id=48382142)

**背景**: 原始 PlayStation 于 1994 年发布，使用 33.8688 MHz 的 MIPS R3000A CPU 和自定义 GPU 进行 3D 图形处理。其架构在当时是独特的，具有独立的几何变换引擎 (GTE) 用于矢量数学，以及音频处理单元 (SPU) 用于音频。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>
<li><a href="https://www.copetti.org/writings/consoles/playstation/">PlayStation Architecture | A Practical Analysis</a></li>
<li><a href="https://psx-spx.consoledev.net/soundprocessingunitspu/">Sound Processing Unit (SPU) - PlayStation Specifications ...</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞了文章的深度和网站设计，同时指出这是 2019 年的重发。一位开发者分享了《合金装备》PC 移植版中使用的内存映射技巧，另一位则询问 PS1 网页模拟器的推荐。

**标签**: `#PlayStation`, `#console architecture`, `#retro computing`, `#hardware`

---

<a id="item-16"></a>
## [何时字节优化真正重要：AoS 与 SoA 对比](https://fzakaria.com/2026/06/01/every-byte-matters) ⭐️ 7.0/10

一篇文章指出，“每个字节都重要”这一口号常常具有误导性，并以数组结构体（AoS）与结构体数组（SoA）的内存布局选择为例，说明何时字节级优化才真正有价值。 这一讨论帮助开发者理解何时值得投入精力进行内存优化，避免在无法提升性能的微优化上浪费时间，同时指出在哪些场景下改变布局能带来显著收益。 文章指出，读取单个字节微不足道，但读取 100 万个字节（例如遍历 100 万个怪物）时优化就至关重要。文章还提到 JVM 对象头（当前 12 字节，即将降至 8 字节）会带来开销，而 Project Valhalla 旨在某些情况下消除对象头。

hackernews · ingve · Jun 3, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48382382)

**背景**: 数组结构体（AoS）将每个对象的字段连续存储，而结构体数组（SoA）将每个字段存储在单独的数组中。当遍历多个对象的同一字段时，SoA 可以改善缓存局部性和 SIMD 向量化。JVM 为每个对象增加了额外开销（对象头+填充），使得内存布局决策在 Java 中比在手动控制内存的语言中影响更大。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AoS_and_SoA">AoS and SoA - Wikipedia</a></li>
<li><a href="https://www.reddit.com/r/bigquery/comments/1fbzy55/array_of_structs_vs_struct_of_arrays/">r/bigquery on Reddit: ARRAY of STRUCTS vs STRUCT of ARRAYS</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为“每个字节都重要”取决于具体场景。有人指出 JVM 的开销使优化更困难，但提到即将到来的改进，如减少对象头和 Project Valhalla。还有人分享了在资源受限环境中每个比特都至关重要的历史经验。

**标签**: `#memory optimization`, `#data structures`, `#JVM`, `#performance`, `#systems programming`

---

<a id="item-17"></a>
## [3 月 4 日 GFW 大规模封禁代理服务](https://t.me/zaihuapd/41740) ⭐️ 7.0/10

3 月 4 日，中国国家防火墙（GFW）开始封禁热门代理服务商的 IP 段，严重影响了 Vless 和 AnyTLS 协议，而非 TLS 加密协议似乎受影响较小。 此次大规模封禁严重影响了依赖代理服务访问受限内容的用户，并凸显了 GFW 针对 Vless 和 AnyTLS 等新型加密协议的封禁能力在持续演进。 此次封禁对 Vless 协议影响较深，较新的 AnyTLS 协议似乎也被大量阻断，但缺乏统计数据佐证。非 TLS 加密类型似乎受影响较小，但实际影响范围尚不清楚。

telegram · zaihuapd · Jun 3, 11:15

**背景**: 中国国家防火墙（GFW）是一套审查和监控系统，用于屏蔽国外网站并减缓跨境流量。Vless 是 Xray 中使用的无状态轻量传输协议，而 AnyTLS 是一种较新的协议，旨在缓解 TLS-in-TLS 指纹识别问题。GFW 此前曾封禁 Shadowsocks 和 VMess 等协议，此次事件表明其封禁能力已扩展至新型加密方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xtls.github.io/en/development/protocols/vless.html">VLESS Protocol | Project X</a></li>
<li><a href="https://github.com/anytls/anytls-go/blob/main/docs/protocol.md">anytls-go/docs/protocol.md at main - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Great_Firewall">Great Firewall - Wikipedia</a></li>

</ul>
</details>

**标签**: `#GFW`, `#proxy`, `#encryption`, `#censorship`, `#Vless`

---

<a id="item-18"></a>
## [千问向第三方 Agent 和 Skill 全面开放平台](https://www.stcn.com/article/detail/3941333.html) ⭐️ 7.0/10

千问 APP 宣布将向第三方 Agent 和 Skill 全面开放，所有企业都可在千问上运营自己的品牌 Agent。首批测试企业包括瑞幸咖啡、肯德基、蜜雪冰城和东方航空等。 此举使千问成为潜在的 AI 超级应用，通过支持丰富的专用 Agent 和 Skill 生态系统，类似于微信的小程序模式。这可能加速企业在客服、点单等任务中采用 AI Agent。 该平台支持 Skill（可复用的工具模板）和企业可定制的品牌 Agent。首批企业正在测试 Agent 服务，并将陆续上线。

telegram · zaihuapd · Jun 3, 12:15

**背景**: 千问是阿里旗下的大语言模型和 AI 助手平台。Agent 是能自主执行任务的 AI 系统，Skill 是为 Agent 配备特定能力的可复用工具模板。向第三方开放平台允许企业在千问内创建自己的品牌 AI Agent，类似于微信承载小程序的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260603A07TGS00">向第三方Agent全面开放，千问正在打造AI时代真正入口</a></li>
<li><a href="https://www.ithome.com/0/959/289.htm">阿里千问向第三方 Agent、Skill 全面开放，肯德基、瑞幸、蜜雪冰城、...</a></li>
<li><a href="https://help.aliyun.com/zh/model-studio/web-search-agent-guide">千问联网检索Agent-大模型服务平台百炼 (Model Studio)-阿里云帮助中...</a></li>

</ul>
</details>

**标签**: `#AI`, `#platform`, `#agents`, `#enterprise`

---

<a id="item-19"></a>
## [美国教师工会呼吁限制小学 AI 与屏幕使用](https://www.aft.org/press-release/devices-down-eyes-hands-weingarten-calls-screen-bans-ai-limits-active-learning-major) ⭐️ 7.0/10

美国教师联合会（AFT）主席兰迪·温加滕提议在幼儿园至二年级禁止屏幕使用，在小学阶段停止使用面向学生的 AI 工具，并禁止 16 岁以下青少年使用社交聊天机器人。 作为代表 160 万成员的主要美国教师工会，AFT 的立场可能影响教育政策和学校技术应用，可能重塑 AI 和数字工具在早期儿童教育中的整合方式。 这项名为“放下设备，亲手实践”的计划还呼吁对科技公司征收“科技税”以资助公共教育，并建立不接受行业资助的独立研究机构，以研究数字技术对儿童的长期影响。

telegram · zaihuapd · Jun 3, 13:30

**背景**: 美国教师联合会（AFT）是美国第二大教师工会，成立于 1916 年，隶属于 AFL-CIO。人们对儿童使用 AI 聊天机器人寻求友谊和治疗日益担忧，研究表明存在对心理健康危机回应不足等风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/American_Federation_of_Teachers">American Federation of Teachers</a></li>

</ul>
</details>

**标签**: `#education`, `#AI policy`, `#screen time`, `#children`, `#teachers union`

---