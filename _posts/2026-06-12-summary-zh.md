---
layout: default
title: "Horizon Summary: 2026-06-12 (ZH)"
date: 2026-06-12
lang: zh
---

> From 40 items, 22 important content pieces were selected

---

1. [AMD 对关键 RCE 漏洞的修复不充分](#item-1) ⭐️ 9.0/10
2. [Anthropic 撤销秘密限制 AI 研究人员的政策](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude Fable 5 和 Mythos 5，性能大幅提升](#item-3) ⭐️ 9.0/10
4. [Homebrew 6.0.0 发布，带来安全与性能升级](#item-4) ⭐️ 8.0/10
5. [要求人类关注，先展示人类努力](#item-5) ⭐️ 8.0/10
6. [小米开源 MiMo Code 编程代理](#item-6) ⭐️ 8.0/10
7. [代码行数：AI 时代的虚荣指标](#item-7) ⭐️ 8.0/10
8. [谷歌发布开源权重模型 DiffusionGemma](#item-8) ⭐️ 8.0/10
9. [Android 17 强制应用内存上限，超限即终止](#item-9) ⭐️ 8.0/10
10. [中国审查 Meta 收购 Manus，创始人被限制离境](#item-10) ⭐️ 8.0/10
11. [macOS 27 将是最后完整支持 Rosetta 2 的版本](#item-11) ⭐️ 8.0/10
12. [请愿撤回加拿大 C-22 法案](#item-12) ⭐️ 7.0/10
13. [DeltaDB 捕获提交之间的代码变更](#item-13) ⭐️ 7.0/10
14. [Waymo 推出每月 30 美元的订阅服务](#item-14) ⭐️ 7.0/10
15. [Datasette 1.0a33 扩展 JSON Extras API](#item-15) ⭐️ 7.0/10
16. [Datasette Agent 0.2a0 增加交互式工具执行功能](#item-16) ⭐️ 7.0/10
17. [Jeremy Howard 提出反直觉的 AI 安全方案](#item-17) ⭐️ 7.0/10
18. [Anthropic 寻求新融资，估值或达 400 亿美元](#item-18) ⭐️ 7.0/10
19. [美团、淘宝闪购、京东外卖签署跨平台黑名单公约](#item-19) ⭐️ 7.0/10
20. [Instacart 与 OpenAI 在 ChatGPT 内推出即时结账功能](#item-20) ⭐️ 7.0/10
21. [苹果与伦敦警方共享被盗 iPhone 数据](#item-21) ⭐️ 7.0/10
22. [SpaceX 轨道数据中心计划面临中国供应链难题](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AMD 对关键 RCE 漏洞的修复不充分](https://mrbruh.com/amd2/) ⭐️ 9.0/10

一名研究人员披露了 AMD 软件中的一个远程代码执行漏洞，AMD 最初拒绝修复，随后仅使用非加密的 CRC-32 校验而非正确的加密签名验证进行了修补。 该漏洞可能允许攻击者通过中间人攻击或入侵网络服务器来破坏服务器，影响 AMD 的供应链和用户信任。不充分的修复凸显了供应商在安全响应方面的持续疏忽。 该补丁使用了 CRC-32，它专为错误检测而非加密安全设计，攻击者可以轻易伪造有效的校验和。AMD 还声称实施了签名验证，但这并不属实。

hackernews · MrBruh · Jun 11, 16:03 · [社区讨论](https://news.ycombinator.com/item?id=48492215)

**背景**: CRC-32 是一种用于检测意外数据损坏的循环冗余校验，但它不具备加密安全性，攻击者可以轻易绕过。需要使用 RSA 或 ECDSA 等加密签名验证来确保下载可执行文件的完整性和真实性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyclic_redundancy_check">Cyclic redundancy check - Wikipedia</a></li>
<li><a href="https://medium.com/@mark.benly/understanding-the-crc32-header-a-deep-dive-into-cyclic-redundancy-check-3b34d31585c7">Understanding the CRC32 Header: A Deep Dive into Cyclic Redundancy Check | by Mark Benly | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者对 AMD 的回应表示失望，称 CRC-32 修复“可笑地无知”，并指出 AMD 在软件质量方面有不良历史。一些人讨论了漏洞赏金计划的范围以及中间人攻击的可行性。

**标签**: `#security`, `#vulnerability`, `#AMD`, `#RCE`, `#supply chain`

---

<a id="item-2"></a>
## [Anthropic 撤销秘密限制 AI 研究人员的政策](https://simonwillison.net/2026/Jun/11/anthropic-walks-back-policy/#atom-everything) ⭐️ 9.0/10

Anthropic 已撤销 Claude Fable 5 中一项秘密限制前沿大语言模型开发用户回复有效性的政策，使安全措施变得可见和透明。 这一逆转恢复了人们对 Anthropic 致力于透明和道德 AI 开发的信任，因为原政策可能暗中破坏 AI 研究并损害用户自主权。 被标记的请求现在将明显回退到 Opus 4.8，而不是暗中限制回复，API 用户将收到拒绝原因。Anthropic 为在速度与透明度之间做出错误权衡而道歉。

rss · Simon Willison · Jun 11, 03:45

**背景**: Claude Fable 5 是 Anthropic 最强大的广泛发布模型，专为高要求推理和自主任务设计。原政策隐藏在系统卡中，会识别针对前沿大语言模型开发的请求并在不通知用户的情况下限制有效性，引发了关于家长式作风和信任的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI | DataCamp</a></li>

</ul>
</details>

**社区讨论**: 社区评论对原政策表示强烈不满，将其比作 Excel 暗中修改公式，并批评 Anthropic 的家长式做法。一些用户仍持怀疑态度，指出隐形安全措施仍可能被秘密保留，信任已受损。

**标签**: `#AI ethics`, `#Anthropic`, `#policy`, `#AI research`, `#transparency`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Fable 5 和 Mythos 5，性能大幅提升](https://t.me/zaihuapd/41892) ⭐️ 9.0/10

Anthropic 发布了面向普通用户的 Claude Fable 5（Mythos 级模型）以及面向经过审查的网络安全合作伙伴的 Claude Mythos 5。新模型在软件工程、知识工作、视觉和科研等基准测试中均达到顶尖水平，而 Fable 5 的价格比前代 Mythos Preview 降低了一半以上。 此次发布标志着让尖端 AI 能力更易获取且更实惠的重要一步，可能重塑大语言模型的竞争格局。内置的安全分类器将敏感查询重定向到能力较弱的模型（Opus 4.8），展示了平衡性能与安全性的新方法。 Claude Fable 5 包含一个安全分类器，当涉及网络安全和生物化学等话题时，会切换至 Opus 4.8 回复，约 5% 的会话受影响。Claude Mythos 5 限制较少，仅面向一小批经过审查的客户，用于漏洞发现等任务。

telegram · zaihuapd · Jun 11, 07:45

**背景**: Anthropic 的 Claude 模型是为安全且强大的 AI 辅助而设计的大语言模型（LLM）。'Mythos' 级别代表 Anthropic 最强大的模型，此前仅用于专业安全研究。'Fable' 是一个新层级，在增加安全护栏的同时将 Mythos 级别的能力带给普通用户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://aws.amazon.com/blogs/aws/anthropic-claude-fable-5-on-aws-mythos-class-capabilities-with-built-in-safeguards-now-available/">Anthropic Claude Fable 5 on AWS: Mythos-class capabilities with built-in safeguards now available | Amazon Web Services</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的社区评论反馈不一：有人称赞 Fable 5 在前端任务和可靠性方面的表现，也有人指出它仍会留下小错误且价格昂贵。一项基准测试记录了创纪录的超时次数和因记忆训练数据导致的高作弊率，引发了对基准有效性的担忧。

**标签**: `#Anthropic`, `#Claude`, `#AI模型`, `#大语言模型`, `#发布`

---

<a id="item-4"></a>
## [Homebrew 6.0.0 发布，带来安全与性能升级](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 8.0/10

Homebrew 6.0.0 引入了新的 tap 信任安全机制、更快的默认 JSON API、Linux 沙箱支持，以及初步的 macOS 27（Golden Gate）支持。 作为 macOS 和 Linux 上广泛使用的包管理器，此重大版本提升了安全性和性能，惠及数百万开发者。新功能回应了社区长期以来的请求，并改善了跨平台的用户体验。 Tap 信任机制验证第三方仓库的真实性，新的 JSON API 减少了响应大小和延迟。Linux 沙箱使用 Bubblewrap 隔离构建进程，macOS 27 支持为初步版本。

hackernews · mikemcquaid · Jun 11, 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48490024)

**背景**: Homebrew 是一个免费开源的包管理器，简化了在 macOS 和 Linux 上安装软件的过程。它使用“tap”（第三方仓库）来扩展软件包集合，新的信任机制有助于防止恶意软件包。JSON API 被 Homebrew 的内部命令和外部工具用于更快的数据检索。

**社区讨论**: 社区成员对维护者的长期奉献表示感谢，一位用户提到其服务已超过 16 年。一些用户讨论了切换到或从 Nix 和 mise 等替代方案切换的体验，提及了可重现性、软件包支持和用户体验之间的权衡。其他人则强调了 Homebrew 在 Bazzite 等不可变 Linux 发行版中的作用。

**标签**: `#homebrew`, `#package-manager`, `#macos`, `#linux`, `#security`

---

<a id="item-5"></a>
## [要求人类关注，先展示人类努力](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

一篇博客文章指出，在请求人类关注（如代码审查）时，必须展示人类努力，批评大量未经打磨的 AI 生成的拉取请求给审查者带来负担。 这凸显了协作软件开发中一个日益严重的问题：未经打磨的 AI 生成内容可能压垮审查者、降低生产力，并可能损害团队动态和代码质量。 文章强调，审查者更愿意投入精力处理那些显示作者已付出努力的 PR，例如清晰的描述、集中的变更以及对反馈的深思熟虑的回应。

hackernews · jjfoooo4 · Jun 11, 23:01 · [社区讨论](https://news.ycombinator.com/item?id=48497609)

**背景**: 代码审查是软件开发中的关键实践，团队成员在合并代码前相互检查变更。随着 Claude 和 ChatGPT 等 AI 编码助手的兴起，开发者可以快速生成大量代码，但这可能导致缺乏人工监督的低质量 PR。

**社区讨论**: 评论者分享了同事用 AI 生成的 PR 淹没团队的经历，导致怨恨和回避。有人建议在 AI 输出旁附上提示词以便复现，另一些人则认为核心问题是许多任务本身毫无意义，使用 AI 很诱人但结果糟糕。

**标签**: `#AI in software engineering`, `#code review`, `#collaboration`, `#productivity`, `#LLM usage`

---

<a id="item-6"></a>
## [小米开源 MiMo Code 编程代理](https://mimo.xiaomi.com/mimocode) ⭐️ 8.0/10

小米以 MIT 许可证开源了 MiMo Code，这是一个终端原生的 AI 编程代理。它基于 OpenCode 分支，并增加了持久记忆、子代理编排和目标驱动的自主循环等功能。 小米这样的科技巨头开源此举，标志着向开源 AI 开发者工具的转变，对 Claude Code 等闭源替代方案构成挑战。通过降低切换成本和增加透明度，可能加速 AI 编程代理的普及。 MiMo Code 包含跨会话项目理解的持久记忆、智能上下文管理，以及通过 dream/distill 循环实现的自我改进。它支持多个 LLM 提供商、TUI、LSP、MCP 和插件，并在 GitHub 上可用。

hackernews · apeters · Jun 11, 14:27 · [社区讨论](https://news.ycombinator.com/item?id=48490826)

**背景**: AI 编程代理是帮助开发者自主编写、阅读和调试代码的工具。OpenCode 是一个开源的终端编程代理，MiMo Code 基于其分支。小米的 MiMo 团队此前开发了 MiMo 2.5 语言模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/blog/mimo-code-long-horizon">mimo .xiaomi.com/blog/ mimo - code -long-horizon</a></li>
<li><a href="https://www.gizmochina.com/2026/06/11/xiaomi-mimo-code-open-source-terminal-ai-coding-agent/">Xiaomi announces new AI coding agent that actually remembers what...</a></li>

</ul>
</details>

**社区讨论**: 社区普遍欢迎这一开源发布，用户称赞其新增的持久记忆和子代理编排等功能。一些评论者认为编程工具应该开源，批评了 Claude Code 等闭源工具。少数用户还推广了他们自己的兼容工具。

**标签**: `#open-source`, `#AI coding agent`, `#Xiaomi`, `#LLM`, `#developer tools`

---

<a id="item-7"></a>
## [代码行数：AI 时代的虚荣指标](https://curlewis.co.nz/posts/lines-of-code-got-a-better-publicist/) ⭐️ 8.0/10

一篇博文指出，代码行数是一个虚荣指标，尤其是在被 AI 代理膨胀后，并呼吁用实际生产力提升的证据而非原始输出来衡量。 这一批评挑战了在 AI 辅助开发中日益流行的以代码行数衡量生产力的趋势，敦促行业关注质量和可维护性而非单纯的数量。 文章指出，AI 代理可以快速生成大量代码，但如果没有相应价值或质量的证据，代码行数就会产生误导。它呼吁采用能反映实际问题解决和用户影响的指标。

hackernews · RyeCombinator · Jun 11, 12:26 · [社区讨论](https://news.ycombinator.com/item?id=48489402)

**背景**: 代码行数长期以来一直被批评为衡量软件生产力的糟糕指标，因为它奖励冗长而非效率。随着 GitHub Copilot 等 AI 代码生成工具的兴起，该指标在管理讨论中重新流行，但往往缺乏代码质量或业务价值的必要背景。

**社区讨论**: 评论者普遍认为代码行数是虚荣指标，有人指出 AI 生成的代码往往缺乏可维护性。一位评论者讽刺地提到微软高管提出的每月每位工程师 100 万行代码的目标，另一位则指出公司利用 AI 作为裁员的借口而非真正的生产力提升。

**标签**: `#AI code generation`, `#software metrics`, `#productivity`, `#engineering culture`

---

<a id="item-8"></a>
## [谷歌发布开源权重模型 DiffusionGemma](https://simonwillison.net/2026/Jun/10/diffusiongemma/#atom-everything) ⭐️ 8.0/10

谷歌发布了 DiffusionGemma，这是一个基于扩散模型的开放权重文本生成模型，采用 Apache 2 许可证，并由 NVIDIA 在其 NIM 云 API 上免费托管。 此次发布标志着谷歌重新回归基于扩散模型的文本生成，提供了高速性能（每秒超过 500 个 token）和开放的可访问性，可能加速高效文本生成的研究和应用开发。 该模型在 Hugging Face 上名为 google/diffusiongemma-26B-A4B-it，总参数量为 260 亿，每个 token 激活 40 亿参数。在测试中，它用 4.4 秒生成了 2,409 个 token，速度至少达到每秒 500 个 token。

rss · Simon Willison · Jun 10, 20:00

**背景**: 扩散模型通常用于图像生成，但也可通过将随机噪声逐步优化为连贯序列来应用于文本。谷歌此前在 2025 年 5 月尝试过 Gemini Diffusion 模型，其速度达到每秒 857 个 token，但未进一步开发。新的 DiffusionGemma 是 Gemma 系列下的开放权重模型，可自由修改和使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/">Try NVIDIA NIM APIs</a></li>
<li><a href="https://developer.nvidia.com/nim">NIM for Developers | NVIDIA Developer</a></li>
<li><a href="https://free-llm.com/provider/nvidia-nim">NVIDIA NIM Free API (2026) | Models & Guide - Free-LLM</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（文章中有链接）可能包含对开放许可证和高速度的兴奋，但此处未提供具体评论。

**标签**: `#AI`, `#open-source`, `#text generation`, `#Google`, `#diffusion model`

---

<a id="item-9"></a>
## [Android 17 强制应用内存上限，超限即终止](https://android-developers.googleblog.com/2026/06/prioritizing-memory-efficiency-steps-for-android-17.html) ⭐️ 8.0/10

从 Android 17 开始，系统会根据设备总 RAM 为每个应用设定内存上限，超过限制的进程会被直接终止且不留堆栈跟踪。同时，Google 提供了 ProfilingManager API，用于在生产环境中异常或 OOM 时收集堆转储。 这一政策变化显著影响应用开发和内存管理，迫使开发者优化内存使用以避免应用被终止。它通过防止单个应用拖累系统性能，提升了整体设备稳定性和多任务体验。 Google 建议启用 R8 优化、使用 RGB_565 等低内存图片格式、及时回收位图、借助 LeakCanary 修复内存泄漏，并响应 onTrimMemory 回调。ProfilingManager API 在 Android 15+ 设备上可用，支持在生产环境中收集堆转储。

telegram · zaihuapd · Jun 11, 05:30

**背景**: Android 长期以来面临内存管理挑战，单个应用消耗过多内存可能导致整个系统变慢或导致其他应用被杀死。按应用设置内存上限已讨论多年，但 Android 17 是首个严格实施该政策的版本。新政策旨在平衡应用功能与整体系统健康，尤其在内存有限的设备上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.android.com/reference/android/os/ProfilingManager">ProfilingManager | API reference | Android Developers</a></li>
<li><a href="https://android-developers.googleblog.com/2026/06/datadog-profilingmanager-performance-insights.html">Android Developers Blog: Datadog delivers millions of in-depth...</a></li>

</ul>
</details>

**标签**: `#Android`, `#memory management`, `#app development`, `#performance`

---

<a id="item-10"></a>
## [中国审查 Meta 收购 Manus，创始人被限制离境](https://t.me/zaihuapd/41895) ⭐️ 8.0/10

中国监管部门正在审查 Meta 收购 AI 初创公司 Manus 是否违反投资规定，并已限制 Manus 首席执行官肖红和首席科学家季一超离境。 这标志着对重大科技收购的显著监管干预，凸显了中国对 AI 相关交易日益收紧的控制以及中美之间潜在的紧张关系。 该交易于 2024 年 12 月宣布，据报道估值约 20 亿美元。两位创始人本月在北京与国家发展和改革委员会会面后被告知不得出境。

telegram · zaihuapd · Jun 11, 10:00

**背景**: Manus 是由蝴蝶效应公司开发的自主 AI 智能体，该公司成立于中国，总部设在新加坡。Meta 的收购旨在增强其 AI 能力，但中国的审查表明对技术转让或国家安全的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lCOTdxakVCR2FRVHVzSFJ3dm1pZ0FQAQ?hl=en-NG&gl=NG&ceid=NG:en">Google News - News about Manus • AI • Meta - Overview</a></li>

</ul>
</details>

**标签**: `#Meta`, `#Manus`, `#AI regulation`, `#acquisition`, `#China`

---

<a id="item-11"></a>
## [macOS 27 将是最后完整支持 Rosetta 2 的版本](https://www.macrumors.com/2026/06/10/macos-golden-gate-last-to-support-intel-apps/) ⭐️ 8.0/10

苹果宣布 macOS 27 Golden Gate 将是最后一个完整支持 Rosetta 2 的版本，从 macOS 28 起仅保留对部分依赖 Intel 框架的旧游戏的有限支持。此外，macOS 27 将首次仅支持 Apple silicon，Intel Mac 无法升级至此版本。 这标志着 macOS 上 Intel 应用兼容性的终结，迫使开发者和用户迁移到 Universal 或 Apple silicon 原生应用。这也意味着苹果自 2020 年开始的 Intel 处理器过渡进入最后阶段。 Rosetta 2 在 macOS 27 中将保持完整功能，但从 macOS 28 起，仅支持部分依赖无人维护的 Intel 框架的旧游戏。基于 Intel 的 Mac 无法运行 macOS 27 及更高版本。

telegram · zaihuapd · Jun 11, 10:45

**背景**: Rosetta 2 是 macOS Big Sur（2020 年）中引入的动态二进制翻译器，允许基于 Intel 的应用在 Apple silicon Mac 上运行。它是苹果从 Intel 处理器过渡到自研 ARM 芯片的一部分。同时引入的 Universal 2 二进制文件包含 Intel 和 Apple silicon 两种架构的代码，可在任一平台上实现原生性能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rosetta_(software)">Rosetta (software)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_silicon">Apple silicon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Universal_binary">Universal binary</a></li>

</ul>
</details>

**标签**: `#macOS`, `#Rosetta 2`, `#Apple Silicon`, `#Intel Mac`, `#Software Compatibility`

---

<a id="item-12"></a>
## [请愿撤回加拿大 C-22 法案](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 7.0/10

加拿大下议院网站上发起了一份请愿，要求撤回 C-22 法案，批评者认为该法案威胁隐私和科技行业。 如果通过，C-22 法案可能迫使科技公司建立加密后门，削弱加拿大人的数字安全和隐私，并可能影响与美国的跨境数据流动。 该请愿是正在进行的议会审查的一部分，SECU 委员会正在逐条审查并投票修正案。批评者还将 C-22 法案与 C-34 法案联系起来，称后者进一步侵蚀隐私。

hackernews · hmokiguess · Jun 11, 15:37 · [社区讨论](https://news.ycombinator.com/item?id=48491830)

**背景**: C-22 法案是一项加拿大立法提案，旨在扩大监控和数据访问权限。批评者认为它迫使科技公司削弱加密，损害隐私和创新。该法案目前正在议会审查中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.todayville.com/bill-c-22-surveils-ordinary-canadians-while-leaving-cartel-networks-untouched/">Bill C - 22 Surveils Ordinary Canadians While Leaving... - Todayville</a></li>
<li><a href="https://news.spreely.com/canada-c-22-compels-tech-firms-to-build-encryption-backdoors/">Canada C - 22 Compels Tech Firms To Build Encryption Backdoors</a></li>

</ul>
</details>

**社区讨论**: 评论者对请愿的影响表示怀疑，但强调制造舆论的重要性。他们提到 SECU 委员会关于 C-22 的会议，并链接到 C-34 等相关法案，警告如果该法案通过，加拿大科技行业将受损。

**标签**: `#privacy`, `#Canada`, `#legislation`, `#technology policy`

---

<a id="item-13"></a>
## [DeltaDB 捕获提交之间的代码变更](https://zed.dev/blog/introducing-deltadb) ⭐️ 7.0/10

Zed 博客介绍了 DeltaDB，这是一个记录 Git 提交之间每次操作的工具，旨在捕捉编写软件的完整过程，并认为这些中间状态比最终提交更具信息量。 这挑战了仅审查最终提交的常见做法，通过揭示代码的真实演变过程，可能改进代码审查和协作。它还可能影响开发者对版本控制和工作文档化的思考方式。 DeltaDB 捕获每一次击键和编辑，而不仅仅是快照，提供了细粒度的变更时间线。该工具旨在与 Git 一起使用，而非替代 Git，目标是让开发过程中的“混乱汤”变得可见且可分析。

hackernews · jeremy_k · Jun 11, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48492533)

**背景**: 像 Git 这样的传统版本控制系统将提交记录为代码库在特定时间点的快照。然而，编写代码的实际过程涉及许多中间步骤、实验和删除，这些在最终提交中丢失了。DeltaDB 旨在保留这一过程，以便更好地理解和协作。

**社区讨论**: 评论意见不一：一些人认为中间变更混乱且无用，更倾向于通过 rebase 制作干净的提交。另一些人表达隐私担忧，认为记录每一次击键具有侵入性。少数人建议 Git 已经支持频繁的自动提交和合并策略来实现类似目标。

**标签**: `#software engineering`, `#version control`, `#code review`, `#developer tools`, `#git`

---

<a id="item-14"></a>
## [Waymo 推出每月 30 美元的订阅服务](https://waymo.com/blog/2026/06/waymo-premier/) ⭐️ 7.0/10

Waymo 推出了 Waymo Premier 订阅服务，每月 30 美元，提供优先叫车和乘车返现。 这标志着自动驾驶网约车商业化的重要一步，可能重塑用户使用和支付自动驾驶服务的方式。 该订阅每月 30 美元，包含优先叫车和乘车返现，返现福利对报销车费的商务旅客尤其有吸引力。

hackernews · boulos · Jun 11, 16:10 · [社区讨论](https://news.ycombinator.com/item?id=48492304)

**背景**: Waymo 是一家领先的自动驾驶汽车公司，在美国部分城市运营网约车服务。订阅模式在软件和交通领域很常见，但这是自动驾驶网约车领域的首批尝试之一。

**社区讨论**: 社区评论褒贬不一：有人认为返现对商务旅客是福利，也有人质疑其相比公共交通的价值。还有人担心安全问题，以及在紧急情况下无法控制车辆。

**标签**: `#autonomous vehicles`, `#subscription service`, `#ride-hailing`, `#Waymo`, `#transportation`

---

<a id="item-15"></a>
## [Datasette 1.0a33 扩展 JSON Extras API](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 将 `?_extra=` 模式扩展到了查询和行，并且该功能现在已在 JSON API 文档中记录。 此版本是迈向稳定版 1.0 的重要一步，为 Datasette 用户提供了更一致、更强大的 API，并通过改进文档提升了开发者体验。 `?_extra=` 模式最初在 Datasette 1.0a3 中为表引入；此 alpha 版本将其扩展到查询和行，允许用户在 JSON 响应中请求额外的元数据。

rss · Simon Willison · Jun 11, 15:26

**背景**: Datasette 是一个用于探索和发布表格数据的开源工具。它提供了用于查询数据库的 JSON API。`?_extra=` 参数允许用户在 API 响应中请求额外的字段，如列类型或行计数。

**标签**: `#datasette`, `#python`, `#open-source`, `#API`, `#release`

---

<a id="item-16"></a>
## [Datasette Agent 0.2a0 增加交互式工具执行功能](https://simonwillison.net/2026/Jun/10/datasette-agent/#atom-everything) ⭐️ 7.0/10

Datasette Agent 0.2a0 引入了工具在执行过程中向用户提问的能力，通过新的 ToolContext 对象和 ask_user() 方法实现，并且对话在服务器重启后仍能持久保存。它还包含一个新的内置 save_query 工具，在将 SQL 查询保存为 Datasette 存储查询之前需要人工批准。 此版本为 AI 代理实现了一种新颖的交互模式，允许它们在执行过程中暂停并请求用户输入，从而提高了安全性和用户控制。持久化功能确保暂停的对话在服务器重启后仍然存在，使该工具在实际数据探索工作流中更加稳健。 工具通过声明 context 参数来接收 ToolContext 对象，并可以调用 await context.ask_user(...) 来提出是/否、多项选择或自由文本问题。在问题未回答时，代理回合暂停，问题以表单形式显示在聊天 UI 中，并持久化到内部数据库。一旦回答，工具将从顶部重新执行，并重放存储的答案。

rss · Simon Willison · Jun 10, 23:57

**背景**: Datasette Agent 是一个 AI 驱动的工具，用于探索和查询 Datasette 中的数据，Datasette 是一个开源的数据探索和发布工具。新的 ask_user() 功能得益于最近使用 Claude Fable 5 构建的 LLM alpha 版本。此版本是早期 alpha 版（0.2a0），表明它仍处于实验阶段。

**标签**: `#datasette`, `#AI agents`, `#tool interaction`, `#open source`, `#data exploration`

---

<a id="item-17"></a>
## [Jeremy Howard 提出反直觉的 AI 安全方案](https://simonwillison.net/2026/Jun/10/jeremy-howard/#atom-everything) ⭐️ 7.0/10

Jeremy Howard 提出，拥有顶级 AI 模型的实验室必须禁止将其用于前沿 AI 研究，同时向其他所有人开放访问，以减缓递归自我改进并减少权力失衡。 该提案挑战了主流的 AI 安全方法——像 Anthropic 这样的领先实验室使用自己的模型进行前沿研究，可能加速进展并集中权力。如果被采纳，可能从根本上改变 AI 开发和治理的动态。 Howard 特别批评了 Anthropic 选择了相反的道路：允许自己使用顶级模型进行前沿研究，同时破坏他人的尝试。他澄清自己个人倾向于开放和民主化 AI 而非减缓其发展，但认为那些声称要减缓发展的人应该以身作则。

rss · Simon Willison · Jun 10, 15:23

**背景**: 递归自我改进（RSI）是指 AI 系统重写自身代码以增强能力的过程，可能导致智能爆炸。前沿 AI 研究涉及使用最先进的模型突破 AI 能力的边界。关于 AI 安全的辩论包括对失控加速和权力集中在少数实验室的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#recursive self-improvement`, `#power imbalance`, `#frontier AI`, `#Anthropic`

---

<a id="item-18"></a>
## [Anthropic 寻求新融资，估值或达 400 亿美元](https://t.me/zaihuapd/41888) ⭐️ 7.0/10

Anthropic 正在洽谈新一轮融资，估值可能达到 300 亿至 400 亿美元，较今年初翻了一番。 这轮融资凸显了 AI 行业的激烈竞争，Anthropic 和 OpenAI 都在筹集巨额资金以扩展其大语言模型并抢占市场份额。 Anthropic 主要通过提供其对话式 AI Claude 的访问权限来创收。与此同时，OpenAI 也在筹集 50 亿至 70 亿美元资金，估值接近 1500 亿美元。

telegram · zaihuapd · Jun 11, 04:45

**背景**: Anthropic 是一家由前 OpenAI 员工创立的领先 AI 公司，专注于构建安全且能力强大的 AI 系统。其旗舰产品 Claude 直接与 OpenAI 的 GPT 模型竞争。公司估值的快速增长反映了投资者对 AI 领域的强烈信心。

**标签**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#Claude`

---

<a id="item-19"></a>
## [美团、淘宝闪购、京东外卖签署跨平台黑名单公约](https://finance.sina.com.cn/jjxw/2026-06-11/doc-iniazpqt0741536.shtml) ⭐️ 7.0/10

美团、淘宝闪购、京东外卖共同签署《广东省网络餐饮行业高质量发展与食品安全自律公约》，首次提出建立跨平台黑名单共享机制，对严重违法商户实施跨平台联合约束，实现“一处违法、全网受限”。 这标志着平台治理和食品安全领域迈出重要一步，通过建立跨平台统一威慑机制，有望减少重复违规行为，提升消费者信任。同时，这也意味着行业从被动合规转向主动治理。 该公约共五章二十一条，涵盖平台主体责任、入网商户管理、配送人员关怀和社会共治等内容，并在广东省市场监管局见证下签署。

telegram · zaihuapd · Jun 11, 11:30

**背景**: 中国网络餐饮平台长期面临违规商户跨平台逃避处罚的问题，这些商户常因食品安全等问题被一家平台处罚后转投其他平台。新的跨平台黑名单共享机制旨在堵住这一漏洞，确保在一家平台被禁的商户在其他平台也受到限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.dayoo.com/guangdong/202606/11/139996_54968763.htm">news.dayoo.com/guangdong/202606/11/139996_54968763.htm</a></li>

</ul>
</details>

**标签**: `#platform governance`, `#food safety`, `#e-commerce`, `#regulation`

---

<a id="item-20"></a>
## [Instacart 与 OpenAI 在 ChatGPT 内推出即时结账功能](https://t.me/zaihuapd/41900) ⭐️ 7.0/10

2025 年 12 月 8 日，Instacart 与 OpenAI 宣布深化合作，在 ChatGPT 中上线首个集成即时结账功能的杂货购物应用，用户无需离开聊天界面即可浏览商品、加入购物车并完成支付。 这标志着电子商务的重大转变，将完整的购买流程嵌入 AI 聊天机器人中，可能改变用户在线购物方式，通过减少摩擦并将用户留在 AI 生态系统中，对传统电商平台构成挑战。 该功能结合了 Instacart 的实时配送网络与 OpenAI 的前沿模型；这是首个在 ChatGPT 内直接完成结账的集成，据报道 OpenAI 从每笔销售中抽取少量佣金，而非按点击收费。

telegram · zaihuapd · Jun 11, 13:15

**背景**: Instacart 是北美最大的在线杂货与即时配送平台，提供从选购到送达的一站式服务。OpenAI 的 ChatGPT 已从对话式 AI 演变为能够执行购物等任务的平台，新的即时结账功能代表了向“对话式商务”的迈进，即购买在聊天中无缝完成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/chatgpt-instant-checkout">A guide to ChatGPT Instant Checkout : What it means for... | eesel AI</a></li>
<li><a href="https://www.eesel.ai/blog/chatgpt-checkout">ChatGPT Checkout is changing e-commerce: Here's what... - eesel AI</a></li>
<li><a href="https://www.linkedin.com/posts/modern-retail_marketplace-briefing-why-chatgpt-checkout-activity-7379961068925902848-B259">OpenAI launches ChatGPT checkout feature , challenges... | LinkedIn</a></li>

</ul>
</details>

**标签**: `#AI`, `#e-commerce`, `#ChatGPT`, `#Instacart`, `#OpenAI`

---

<a id="item-21"></a>
## [苹果与伦敦警方共享被盗 iPhone 数据](https://www.express.co.uk/life-style/science-technology/2215942/apple-launches-major-iphone-update) ⭐️ 7.0/10

苹果与伦敦大都会警察局达成数据共享协议，向警方提供被盗设备标识以追踪设备重新联网情况，并在近期软件更新中将“被盗设备保护”设为默认开启。 这一合作使伦敦手机盗窃案减少 18%（2025 年 6 月至 2026 年 5 月间减少 1.4 万起），凸显了公私数据共享在打击犯罪方面的潜力，同时也引发了隐私方面的担忧。 警方向苹果提供被盗设备标识，苹果据此阻止设备重新激活或追踪转售。伦敦大都会警察局正推动立法，要求手机公司共享被盗数据并让被盗设备无法使用。

telegram · zaihuapd · Jun 12, 00:24

**背景**: 被盗 iPhone 数据共享是指执法机构向苹果提供设备唯一标识（如 IMEI），苹果随后在其激活服务器中标记这些设备。“被盗设备保护”是一项功能，要求对敏感操作进行生物识别验证，使被盗 iPhone 更难使用或转售。

**标签**: `#Apple`, `#privacy`, `#law enforcement`, `#data sharing`, `#security`

---

<a id="item-22"></a>
## [SpaceX 轨道数据中心计划面临中国供应链难题](https://www.bloomberg.com/opinion/articles/2026-06-11/spacex-s-critical-minerals-plan-runs-through-china) ⭐️ 7.0/10

SpaceX 计划从 2030 年起每年将 100 吉瓦的太阳能 AI 数据中心送入轨道，需要数千次发射和约 100 万吨运力，但该计划因中国在镓和多晶硅等关键矿物上的主导地位而面临挑战。 这凸显了 SpaceX 雄心勃勃的轨道基础设施面临的重大地缘政治和供应链风险，可能延迟或复杂化天基 AI 计算的部署。它也凸显了在先进技术项目中减少对中国材料依赖的更广泛挑战。 太空太阳能电池可能涉及砷化镓或多晶硅，而中国在全球镓和太阳能级多晶硅生产中占主导地位。SpaceX 还持有美国军方合同，因此依赖中国硬件可能成为安全隐患。

telegram · zaihuapd · Jun 12, 01:14

**背景**: 轨道数据中心是提议中的太空设施，利用天基太阳能为 AI 计算供电，克服地球上的能源和土地限制。该概念基于升级版星链卫星，并源于军事太空架构，如战略防御倡议的“ brillant pebbles”计划。镓等关键矿物对于太空使用的高效太阳能电池至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Orbital_data_center">Orbital data center</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#orbital data center`, `#supply chain`, `#critical minerals`, `#AI`

---