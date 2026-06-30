---
layout: default
title: "Horizon Summary: 2026-06-30 (ZH)"
date: 2026-06-30
lang: zh
---

> From 33 items, 16 important content pieces were selected

---

1. [最高法院裁定地理围栏搜查令需受第四修正案保护](#item-1) ⭐️ 9.0/10
2. [vLLM v0.24.0 新增 MiniMax-M3 支持与 DeepSeek-V4 优化](#item-2) ⭐️ 8.0/10
3. [火箭实验室以 80 亿美元收购铱星](#item-3) ⭐️ 8.0/10
4. [将 Game Boy 指令 JIT 编译为 WASM 性能超越原生解释器](#item-4) ⭐️ 8.0/10
5. [CUDA 内核启动过程深度解析](#item-5) ⭐️ 8.0/10
6. [桑迪亚国家实验室 SA3000：1970 年代的抗辐射 8085 CPU](#item-6) ⭐️ 8.0/10
7. [Ornith-1.0：开源权重 LLM 系列实现编程 SOTA](#item-7) ⭐️ 8.0/10
8. [Jon Udell：邀请智能体加入，而非被排除在外](#item-8) ⭐️ 8.0/10
9. [三星与 SK 海力士宣布大规模 AI 投资计划](#item-9) ⭐️ 8.0/10
10. [算法误判删除普朗克 1940 年代论文](#item-10) ⭐️ 8.0/10
11. [长鑫存储与腾讯签近 30 亿美元 DRAM 供应协议](#item-11) ⭐️ 8.0/10
12. [提议的.self 顶级域名旨在促进自托管](#item-12) ⭐️ 7.0/10
13. [Qwen 3.6 27B：本地开发的最佳选择？](#item-13) ⭐️ 7.0/10
14. [因藏匿 zine 被判 30 年引发言论自由警报](#item-14) ⭐️ 7.0/10
15. [欧洲 ISP 要求版权方为过度屏蔽承担责任](#item-15) ⭐️ 7.0/10
16. [中国加强个人境外股票收益征税监管](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [最高法院裁定地理围栏搜查令需受第四修正案保护](https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision) ⭐️ 9.0/10

美国最高法院裁定，地理围栏搜查令（强制谷歌等科技公司提供特定区域内所有设备位置数据的命令）构成第四修正案意义上的搜查，必须基于相当理由获得搜查令。大法官埃琳娜·卡根撰写了多数意见，认为即使身处公共场所，个人对其聚合位置数据也享有合理的隐私期待。 这项里程碑式的裁决极大地限制了执法部门在没有个别嫌疑的情况下进行大规模数字监控的能力，加强了数百万智能手机用户的隐私保护。它为第四修正案如何适用于数字时代新兴监控技术树立了关键先例。 该案源于一起银行抢劫调查，谷歌提供了案发地点附近 19 台设备的位置数据。法院驳回了政府关于个人在公共场所没有隐私期待的主张，强调了地理围栏搜索的全面性和回溯性。

hackernews · cdrnsf · Jun 29, 15:54 · [社区讨论](https://news.ycombinator.com/item?id=48720924)

**背景**: 地理围栏搜查令，也称为反向位置搜查令，允许执法部门在特定时间段内搜索公司数据库中特定地理区域内的所有移动设备。谷歌的 Sensorvault 数据库存储了数十亿设备的历史位置数据，一直是此类搜查令的主要目标。第四修正案保护公民免受不合理的搜查和扣押，法院一直在努力将其应用于数字监控技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/us-news/2026/jun/29/supreme-court-geofence-warrants-case-decision">US supreme court rules geofence warrants require constitutional privacy protections | US supreme court | The Guardian</a></li>
<li><a href="https://en.wikipedia.org/wiki/Geofence_warrant">Geofence warrant</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一裁决表示强烈支持，有人强调法院在意见中使用了事实来源。其他人讨论了该裁决对 Flock 自动车牌识别器等监控工具的影响，质疑这些工具现在是否需要搜查令。还有评论者指出，即使没有手机数据，也可以通过其他方式识别嫌疑人，并引用了 Paula Broadwell 案。

**标签**: `#privacy`, `#supreme court`, `#geofence warrants`, `#fourth amendment`, `#digital surveillance`

---

<a id="item-2"></a>
## [vLLM v0.24.0 新增 MiniMax-M3 支持与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 8.0/10

vLLM v0.24.0 已发布，新增对 MiniMax-M3 模型的支持，并对 DeepSeek-V4 进行了大量优化，包括 FlashInfer 稀疏索引缓存和预填充分块规划改进。本次发布包含来自 256 位贡献者的 571 次提交。 此版本显著扩展了 vLLM 的模型支持范围和推理效率，通过支持 MiniMax-M3 和 DeepSeek-V4 等前沿模型，使 AI 社区能够更快、更经济地部署这些模型。针对 DeepSeek-V4 的优化（如 FlashInfer 稀疏索引缓存）可将首 token 延迟降低 2-4%。 MiniMax-M3 支持包括通过 MSA 实现的 BF16/FP8 索引器、MXFP4 支持以及 FP8 稀疏 GQA，并进行了广泛的 AMD/ROCm 调优。DeepSeek-V4 优化还包括用于低延迟的集群协作 topK 内核和连续的逐块 KV 分配。

github · khluu · Jun 29, 19:41

**背景**: vLLM 是一个开源的高吞吐量 LLM 推理引擎，广泛用于服务大型语言模型。MiniMax-M3 是一个具有 1M 上下文和原生多模态的前沿模型，采用 MiniMax 稀疏注意力（MSA）架构。DeepSeek-V4 是一个 671B 参数的 MoE 模型，针对效率和国产芯片进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-m3">MiniMax M3: Frontier Coding, 1M Context, Native Multimodality — All in One Model - MiniMax Research | MiniMax</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>
<li><a href="https://github.com/flashinfer-ai/flashinfer">GitHub - flashinfer -ai/ flashinfer : FlashInfer : Kernel Library for LLM...</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#DeepSeek-V4`, `#MiniMax-M3`, `#GPU optimization`

---

<a id="item-3"></a>
## [火箭实验室以 80 亿美元收购铱星](https://investors.rocketlabcorp.com/news-releases/news-release-details/rocket-lab-acquire-iridium-historic-deal-creating-fully) ⭐️ 8.0/10

火箭实验室于 2025 年 6 月 29 日宣布，将以现金加股票方式收购铱星通信，交易价值约 80 亿美元，每股报价 54 美元。该交易已获双方董事会一致批准，预计 2027 年年中完成，尚需股东和监管批准。 这项历史性收购将火箭实验室的发射和航天器制造能力与铱星的全球低轨卫星网络及 L 波段频谱相结合，打造一家完全整合的太空公司，可能效仿 SpaceX 的 Starlink 战略。它为火箭实验室提供了稳定的发射需求基线，对冲市场波动，并使其成为重要的端到端太空服务提供商。 火箭实验室已获得 36 亿美元的过桥贷款承诺。铱星星座由 66 颗活跃的低轨卫星组成，具备星间链路，提供全球语音和数据服务，其卫星位于约 780 公里高度的极地轨道，并非典型的低轨轨道。

hackernews · everfrustrated · Jun 29, 14:09 · [社区讨论](https://news.ycombinator.com/item?id=48719485)

**背景**: 火箭实验室是一家端到端的太空公司，提供发射服务（Electron 火箭）、航天器制造和卫星组件。铱星通信运营着唯一真正的全球卫星网络，最初于 1998 年发射，经历了破产重组，并通过 SpaceX 的 Falcon 9 火箭进行了升级。此次收购类似于 SpaceX 利用 Starlink 为其 Falcon 9 火箭保证基础发射量的策略。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iridium_satellite_constellation">Iridium satellite constellation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Iridium_Communications">Iridium Communications - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Rocket_Lab">Rocket Lab - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了与 SpaceX Starlink 策略的相似之处，用户指出火箭实验室可以利用铱星保证最低发射量，并将星座替换纳入其订单簿。一些人表达了对太空垃圾和太空商业化的担忧，而另一些人则质疑技术适配性，因为铱星的极地轨道与典型低轨不同，可能无法由 Electron 火箭到达。

**标签**: `#space`, `#acquisition`, `#satellite`, `#Rocket Lab`, `#Iridium`

---

<a id="item-4"></a>
## [将 Game Boy 指令 JIT 编译为 WASM 性能超越原生解释器](https://humphri.es/blog/WATaBoy/) ⭐️ 8.0/10

一篇博客文章展示了将 Game Boy 模拟器指令即时编译为 WebAssembly（WASM）可以超越原生解释器，通过利用浏览器的 JIT 引擎实现更高性能。 这种方法为在受 JIT 限制的平台（如 iOS）上运行模拟器提供了新途径，因为浏览器允许 WASM JIT。它可能使更多设备实现高性能模拟。 该项目名为 WATaBoy，在运行时将 Game Boy CPU 指令编译为 WASM 模块。据报道，Firefox 比 Chrome/Safari 慢 25%，可能是由于不同的 WASM JIT 实现。

hackernews · energeticbark · Jun 29, 15:02 · [社区讨论](https://news.ycombinator.com/item?id=48720190)

**背景**: 模拟器传统上使用解释执行或原生 JIT 编译。原生 JIT 在 iOS 上常被禁止，但浏览器可以对 WASM 进行 JIT 编译。该项目通过生成 WASM 而非原生代码来利用这一点，绕过平台限制同时享受 JIT 加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sysprog21/jitboy">GitHub - sysprog21/jitboy: A Game Boy emulator with dynamic recompilation (JIT) · GitHub</a></li>
<li><a href="https://rodrigodd.github.io/2023/09/02/gameroy-jit.html">GameRoy: JIT compilation in High-Accuracy Game Boy Emulation | Rodrigodd</a></li>
<li><a href="https://8bitworkshop.com/docs/posts/2021/webassembly-vs-javascript-emulator-performance.html">Emulator Performance: WebAssembly vs. JavaScript — 8bitworkshop documentation</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，使用 JavaScript 的 eval()是一种简单的 JIT 方法，而苹果对浏览器的 JIT 例外使该技术在 iOS 上可行。一位评论者称赞该项目对本科生来说令人印象深刻，另一位则强调 WASM 开销（约 20%）远小于解释器开销（约 1000%）。

**标签**: `#JIT compilation`, `#WebAssembly`, `#emulation`, `#Game Boy`, `#performance`

---

<a id="item-5"></a>
## [CUDA 内核启动过程深度解析](https://fergusfinn.com/blog/what-happens-when-you-run-a-gpu-kernel/) ⭐️ 8.0/10

Fergus Finn 发表了一篇技术博客，详细讲解了从 CPU 驱动交互到 GPU 执行的 CUDA 内核启动全过程。 这篇文章填补了常见 CUDA 教程的空白，解释了通常被忽略的底层步骤，帮助开发者优化内核启动并理解 GPU 硬件行为。 文章涵盖了门铃机制、队列管理描述符（QMD）以及线程束资格判断，将 CUDA 语法与实际 GPU 提交联系起来。

hackernews · mezark · Jun 29, 13:11 · [社区讨论](https://news.ycombinator.com/item?id=48718863)

**背景**: CUDA 是 NVIDIA 的并行计算平台，允许开发者在 GPU 上运行代码。内核启动涉及 CPU 驱动准备命令和数据，然后通过门铃寄存器发送到 GPU。GPU 调度器随后将工作分配给流多处理器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.geeksforgeeks.org/cpp/launching-a-kernel-in-cuda/">Launching a Kernel | CUDA - GeeksforGeeks</a></li>
<li><a href="https://enccs.github.io/cuda/2.02_HelloGPU/">Launching the GPU kernel — CUDA training materials documentation</a></li>
<li><a href="https://medium.com/@snshyam/cuda-deep-dive-what-happens-when-you-launch-a-kernel-034e23624932">🚀 CUDA Deep Dive: What Happens When You Launch a Kernel? | by Shyam SN | Medium</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞文章清晰解释了 CPU 到 GPU 的路径，特别是门铃和 QMD 部分。有人指出 NVIDIA 的开源 GPU 文档可以补充这些信息，并讨论了开源内核优化库挑战专有解决方案的可能性。

**标签**: `#CUDA`, `#GPU`, `#systems programming`, `#HPC`, `#NVIDIA`

---

<a id="item-6"></a>
## [桑迪亚国家实验室 SA3000：1970 年代的抗辐射 8085 CPU](https://www.cpushack.com/2026/06/03/sandia-national-labs-sa3000-8085-cpu/) ⭐️ 8.0/10

CPU Shack 上的一篇文章详细介绍了桑迪亚国家实验室的 SA3000，这是一款在 1970 年代末至 1980 年代初开发的抗辐射 8085 CPU，能够承受高达 3×10⁶ rad 的辐射，性能仅下降 40%。 这款历史 CPU 突显了早期政府在内部抗辐射芯片设计上的投入，这一能力至今对太空和国防系统仍至关重要。社区评论将其与现代抗辐射 POWER 架构 CPU（如 BAE RAD5545）联系起来，展示了该技术的演进。 SA3000 采用 n-on-n+外延衬底以实现闩锁控制，晶体管周围设有保护环，并使用硬化氧化物。它在桑迪亚自己的 IC 工厂制造，封装由 Fairchild 和 Allied Signal 处理。

hackernews · rbanffy · Jun 29, 10:20 · [社区讨论](https://news.ycombinator.com/item?id=48717287)

**背景**: 抗辐射处理是使电子设备抵抗电离辐射的过程，对太空和核环境至关重要。Intel 8085 是 1977 年推出的 8 位微处理器，广泛用于嵌入式系统。桑迪亚国家实验室是美国政府专注于国家安全的研究实验室。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Radiation_hardening">Radiation hardening - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Intel_8085">Intel 8085 - Wikipedia</a></li>
<li><a href="https://www.baesystems.com/en-us/article/next-generation-radiation-hardened-computer-for-space">Next-generation radiation - hardened computer for space</a></li>

</ul>
</details>

**社区讨论**: 评论者赞扬了政府的内部能力，并提到了现代抗辐射 CPU 如 MOOG BRE440 和 BAE RAD5500/5545，它们采用 IBM POWER 架构。有人对核武器依赖如此古老的 CPU 表示惊讶，而其他人则解释了诸如“n-on-n+外延衬底”等术语。

**标签**: `#radiation-hardened`, `#CPU`, `#history`, `#embedded systems`, `#government technology`

---

<a id="item-7"></a>
## [Ornith-1.0：开源权重 LLM 系列实现编程 SOTA](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0 系列开源权重 LLM（9B 到 397B），采用 MIT 许可证，在编程基准测试中达到了同类开源模型的最优性能。 此次发布为开发者提供了一个强大且许可宽松的模型系列，用于智能体编程任务，可能加速 AI 辅助软件开发，减少对专有模型的依赖。 该模型系列包括 9B Dense、31B Dense、35B MoE 和 397B MoE 变体，基于预训练的 Gemma 4 和 Qwen 3.5 构建，两者均采用 Apache 2.0 许可证。早期用户报告显示其在智能体编程工作流中表现强劲，例如导航代码库和执行工具调用。

rss · Simon Willison · Jun 29, 16:17

**背景**: 智能体编程是指使用 AI 代理辅助软件开发任务，如代码生成、调试和测试。混合专家（MoE）模型使用多个专门的子网络和门控机制来高效处理多样化的输入，从而以较低的计算成本实现更大的模型容量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self - Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agentic_coding">Agentic coding</a></li>
<li><a href="https://ai.plainenglish.io/mixture-of-experts-moe-models-in-ai-4bcbcdecccf8">Mixture - of - Experts ( MoE ) Models in AI | by DhanushKumar | Artificial...</a></li>

</ul>
</details>

**社区讨论**: 在 Simon Willison 的博客上，初步反响积极，作者指出其在智能体编程任务中表现强劲，推理速度快（103 tokens/秒）。未提及重大批评或分歧。

**标签**: `#LLM`, `#open-source`, `#coding`, `#AI`, `#model release`

---

<a id="item-8"></a>
## [Jon Udell：邀请智能体加入，而非被排除在外](https://simonwillison.net/2026/Jun/28/jon-udell/#atom-everything) ⭐️ 8.0/10

Jon Udell 主张在人类保持控制的前提下进行智能体辅助开发，邀请智能体加入循环而非被排除在外，并警告避免由 AI 智能体生成不可审查的拉取请求。 这重新定义了人机协作的叙事，强调在 AI 辅助软件开发中的人类主导权和工程纪律，随着 AI 智能体在编码工作流中日益普及，这一点至关重要。 Udell 特别批评了智能体生成包含数千行 LLM 编写代码的不可审查 PR 的做法，并倡导一种协作流程，其中智能体提供协助，但由人类审查和批准变更。

rss · Simon Willison · Jun 28, 21:57

**背景**: 智能体辅助开发利用 AI 智能体自动化软件工程的部分环节，但如果管理不当，可能导致大量不透明的代码变更。'人在循环中'这一术语常暗示机器在控制，Udell 通过翻转叙事来挑战这一观点，坚持人类作为主要决策者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.jonudell.net/2026/06/28/doctor-it-hurts-when-agents-create-unreviewable-prs-dont-do-that/">“Doctor, it hurts when agents create unreviewable PRs .” “Don’t do that.”</a></li>
<li><a href="https://golabstech.com/solutions/agent-assisted-development">Agent - Assisted Development | Golabs AI-Orchestrated Engineering</a></li>
<li><a href="https://www.linkedin.com/pulse/i-tried-agent-assisted-development-smooth-ride-deji-akomolafe-jxxfc">I Tried Agent - Assisted Development . It Was Not the Smooth Ride...</a></li>

</ul>
</details>

**标签**: `#agentic-software-development`, `#human-in-the-loop`, `#AI-agents`, `#software-engineering`

---

<a id="item-9"></a>
## [三星与 SK 海力士宣布大规模 AI 投资计划](https://t.me/zaihuapd/42235) ⭐️ 8.0/10

三星和 SK 海力士将于 2026 年 6 月 29 日的国家简报会上宣布大规模 AI 投资计划，其中三星计划十年内投入 6480 亿美元，创韩国历史之最。 这些投资标志着行业向 AI 基础设施的重大转变，可能重塑全球半导体供应链并加速 AI 应用。 三星的计划包括 300 万亿韩元用于芯片工厂建设，而 SK 海力士计划到 2030 年将 DRAM 晶圆产能翻倍，并通过美国上市筹资 290 亿美元。

telegram · zaihuapd · Jun 29, 07:00

**背景**: 物理 AI 指能够与现实世界交互的 AI 系统，结合感知、推理和行动。HBM（高带宽存储器）对 AI 加速器至关重要，SK 海力士是领先的 HBM 供应商。三星是全球最大的存储芯片制造商，但在 HBM 技术上面临挑战。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.asiaeconomynews.com/page200.html?article_id=1754">6480亿美元砸向本土 三星用韩国史上最大投资押注芯片与AI赛道</a></li>
<li><a href="https://www.ithome.com/0/960/576.htm">SK 海力士最新计划：2030-2031 年 DRAM 晶圆产能实现翻倍，月产量达百...</a></li>
<li><a href="https://xueqiu.com/7113191878/391960620">物理 AI 全面深度分析（定义 + 五大受益赛道 + 全产业链上市公司 + 上...</a></li>

</ul>
</details>

**标签**: `#AI`, `#semiconductors`, `#investment`, `#Samsung`, `#SK Hynix`

---

<a id="item-10"></a>
## [算法误判删除普朗克 1940 年代论文](https://arstechnica.com/science/2026/06/why-did-this-journal-retract-two-1940s-papers-by-max-planck/) ⭐️ 8.0/10

马克斯·普朗克在 1940 年代发表的两篇论文被《自然科学》期刊撤稿并彻底删除，很可能是自动检测系统误将其识别为违规内容。 这一事件凸显了学术出版中缺乏历史背景的算法内容审核的危险性，可能抹去重要的科学遗产，并削弱对自动化系统的信任。 与通常保留原文并附撤稿声明的做法不同，这些论文被完全删除，只留下标注“因违规而撤回”的空白页面。期刊主编此前不知情，推测是自动系统的错误操作。

telegram · zaihuapd · Jun 29, 08:46

**背景**: 马克斯·普朗克（1858–1947）是量子物理学的奠基人。《自然科学》是一本历史悠久的德国科学期刊。自动检测系统越来越多地被用于检测抄袭或伦理违规，但它们可能缺乏评估历史论文所需的细微判断，这些论文可能使用不同的引用规范或包含过时的术语。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://retractionwatch.com/">Retraction Watch – Tracking retractions as a window into the ...</a></li>
<li><a href="https://www.hanspub.org/journal/OJNS.html">自然科学杂志_物质科学杂志_数理科学期刊_汉斯出版社</a></li>

</ul>
</details>

**标签**: `#academic publishing`, `#algorithmic bias`, `#content moderation`, `#history of science`, `#AI ethics`

---

<a id="item-11"></a>
## [长鑫存储与腾讯签近 30 亿美元 DRAM 供应协议](https://www.reuters.com/world/china/chinas-cxmt-wins-3-billion-memory-supply-deal-with-tencent-sources-say-2026-06-29/) ⭐️ 8.0/10

长鑫存储（CXMT）与腾讯签署了一项价值超过 200 亿元人民币（约 29.4 亿美元）的多年期 DRAM 供应协议，涵盖数年服务器内存芯片供货。 这笔交易标志着中国本土内存产业的重要里程碑：作为国内领先的 DRAM 制造商，长鑫存储从科技巨头腾讯获得巨额订单，有助于减少 AI 和云计算基础设施对外国供应商（如三星和 SK 海力士）的依赖。 据消息人士称，该协议期限为三到五年。据报道，长鑫存储还在与其他中国互联网公司（包括阿里云、字节跳动和小米）进行类似交易的谈判。

telegram · zaihuapd · Jun 29, 09:31

**背景**: DRAM（动态随机存取内存）是一种易失性存储器，广泛用于服务器、PC 和 AI 加速器中的临时数据存储。长鑫存储是中国最大的 DRAM 制造商，近期已开始量产先进的 DDR5 内存，缩小了与全球领先者三星和 SK 海力士的差距。这笔交易反映了在美国出口管制持续背景下，中国推动半导体自主化的努力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://cnnews.chosun.com/client/news/viw.asp?nNewsNumb=20241262105">中国尖端DRAM也实现了量产…追击到了三星和海力士眼前</a></li>
<li><a href="https://cloud.tencent.com/developer/article/2574397">TrendForce：DRAM 市场与技术概览 2025-2026 - 腾讯云</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#DRAM`, `#China tech`, `#AI infrastructure`, `#supply chain`

---

<a id="item-12"></a>
## [提议的.self 顶级域名旨在促进自托管](https://hccf.onmy.cloud/2026/06/21/reclaiming-our-digital-selves-hccfs-vision-for-a-human-centered-top-level-domain/) ⭐️ 7.0/10

一项名为.self 的新顶级域名（TLD）提案已发布，旨在通过为每人提供一个免费域名并采用基于声誉的治理来管理滥用行为，从而支持自托管。 如果实施，.self 可能降低自托管门槛，让个人对自己的在线存在拥有更多控制权，减少对中心化平台的依赖，但面临防止滥用和运营资金方面的重大挑战。 该提案包括每人一个免费域名、基于声誉的系统以防止抢注和滥用，以及允许因不活跃而事后移除域名的治理模型。然而，在没有注册费的情况下运营 TLD 的资金来源仍不明确。

hackernews · HumanCCF · Jun 29, 19:49 · [社区讨论](https://news.ycombinator.com/item?id=48724230)

**背景**: 自托管是指在自己的服务器上运行和维护网站或服务，而不是使用托管或 SaaS 提供商。像.com 和.org 这样的顶级域名通常由收取费用的注册机构管理。一个带有基于声誉治理的免费 TLD 是一种新颖的方法，旨在鼓励自托管同时减少滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Self-hosting_(network)">Self-hosting (network) - Wikipedia</a></li>
<li><a href="https://github.com/awesome-selfhosted/awesome-selfhosted">GitHub - awesome-selfhosted/awesome-selfhosted: A list of ...</a></li>
<li><a href="https://www.sup.org/books/title?id=20267">Reputation-Based Governance | Stanford University Press</a></li>

</ul>
</details>

**社区讨论**: 社区评论对滥用表示担忧，引用.tk TLD 的历史，其中诈骗者导致广泛封锁。其他人质疑在没有身份验证的情况下防止抢注的可行性以及免费 TLD 的财务可持续性。一些人建议查看微软的 Vega 项目以获取身份解决方案。

**标签**: `#DNS`, `#self-hosting`, `#TLD`, `#decentralization`, `#identity`

---

<a id="item-13"></a>
## [Qwen 3.6 27B：本地开发的最佳选择？](https://quesma.com/blog/qwen-36-is-awesome/) ⭐️ 7.0/10

Qwen 3.6 27B 是一个拥有 270 亿参数的稠密多模态模型，已作为开源权重模型发布，针对本地开发进行了优化，在稳定性和实际应用方面有所改进。 该模型为希望在本地运行强大 LLM 的开发者提供了一个强有力的选择，在性能和资源需求之间取得了平衡，这对于隐私敏感或离线编码任务至关重要。 该模型需要强大的硬件支持，社区报告建议至少需要 32GB 显存或配备 128GB 内存的高端 Mac，并且在负载下可能会产生热量和噪音。

hackernews · stared · Jun 29, 17:05 · [社区讨论](https://news.ycombinator.com/item?id=48721903)

**背景**: 本地 LLM 允许开发者在自己的机器上运行 AI 模型，无需将数据发送到外部服务器，从而提供隐私和离线能力。Qwen 是阿里巴巴的一系列开源权重模型，27B 变体是一个稠密模型（所有参数均激活），在规模和性能之间取得了平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://github.com/QwenLM/Qwen3-Coder">GitHub - QwenLM/Qwen3-Coder: Qwen3-Coder is the code version ...</a></li>
<li><a href="https://ollama.com/library/qwen3-coder">qwen3-coder - ollama.com</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，Qwen3-Coder:30b 在编码任务上可能更快速、更准确，一些用户还警告了笔记本电脑上的散热和噪音等硬件限制。其他人则质疑这些基准测试是否反映了在现有代码库上进行实际编码的情况。

**标签**: `#local-llm`, `#qwen`, `#ai-development`, `#hardware`, `#machine-learning`

---

<a id="item-14"></a>
## [因藏匿 zine 被判 30 年引发言论自由警报](https://theintercept.com/2026/06/26/daniel-sanchez-estrada-zines-prairieland-free-speech/) ⭐️ 7.0/10

Daniel Sanchez-Estrada 因藏匿联邦搜查令所寻找的 zine 被判处 30 年监禁，该搜查令与一起 Antifa 抗议活动有关，其中一名联邦探员被枪击。这一判决引发了严重的言论自由担忧，因为这些 zine 此前已公开发表，且与枪击事件无直接关联。 此案为言论自由树立了一个令人不安的先例，将藏匿已发表材料的行为视为篡改证据，可能抑制政治敏感 zine 的传播。它还凸显了与抗议相关的指控可能带来的严厉惩罚，即使对于未直接参与暴力的人也是如此。 搜查令针对的是抗议者向 ICE 设施发射烟花后的文件，一名团伙成员据称射中了一名急救人员的颈部。Sanchez-Estrada 并非枪手，但因藏匿他认为可能将他人与犯罪联系起来的 zine 而被定罪，最终在可能的 75 年刑期中被判处 30 年。

hackernews · xrd · Jun 28, 21:42 · [社区讨论](https://news.ycombinator.com/item?id=48711981)

**背景**: Zine 是一种非商业性、通常自制的小众出版物，历史上被边缘化社区用来绕过主流媒体。篡改证据涉及隐藏或改变与刑事调查相关的证据，可能面临严厉处罚。在此案中，这些 zine 被视为与抗议相关的犯罪活动的证据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zine">Zine - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者意见不一：一些人认为在搜查令下藏匿 zine 明显是篡改证据，而另一些人则质疑 zine 本身是何种犯罪的证据，并指出它们已经发表。许多人表示担忧，认为 30 年刑期过于严厉，为言论自由树立了危险先例，一些人希望未来能得到赦免。

**标签**: `#free speech`, `#legal`, `#civil liberties`, `#protest`, `#sentencing`

---

<a id="item-15"></a>
## [欧洲 ISP 要求版权方为过度屏蔽承担责任](https://torrentfreak.com/european-isps-want-rightsholders-held-accountable-for-overblocking-damage/) ⭐️ 7.0/10

欧洲互联网服务提供商正在推动立法，要求版权方对过度屏蔽合法内容所造成的损害承担法律和经济责任，从而改变当前的责任平衡。 这可能从根本上改变在线版权执法的模式，降低审查风险，保护互联网用户对合法内容的访问，同时可能增加版权方的成本。 该提案针对的是过度屏蔽行为，即 ISP 因过于宽泛的下架请求或自动过滤而删除或屏蔽实际上并未侵权的内容。这一辩论与美国 DMCA 系统中的类似担忧相呼应。

hackernews · Brajeshwar · Jun 29, 16:07 · [社区讨论](https://news.ycombinator.com/item?id=48721072)

**背景**: 过度屏蔽是指由于过于激进的版权或其他规则执法，无意中屏蔽了合法内容。ISP 目前面临快速处理下架通知的压力，往往导致过度屏蔽，而受影响方几乎没有追索权。版权方通常不会因错误下架而受到处罚。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://de.wikipedia.org/wiki/Overblocking">Overblocking – Wikipedia</a></li>
<li><a href="https://www.netscout.com/what-is/overblocking">What is Overblocking? | NETSCOUT</a></li>
<li><a href="https://cyber.harvard.edu/property99/liability/main.html">ISP Liability for Copyright Infringement</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持这一举措，并引用了西班牙足球联赛期间 La Liga 干扰互联网等现实案例。一些人担心时机可能有利于寻求更容易获取数据的 AI 模型训练公司，而非保护用户权利。

**标签**: `#ISP`, `#copyright`, `#censorship`, `#internet governance`, `#EU policy`

---

<a id="item-16"></a>
## [中国加强个人境外股票收益征税监管](https://t.me/zaihuapd/42236) ⭐️ 7.0/10

中国税务部门正加强对个人境外股票收益的征税监管，要求按年度盈亏净额缴纳 20%的税款，亏损不得跨年结转，并利用 CRS 数据精准发现未申报行为。 此举对持有境外股票的中国投资者影响重大，增加了合规成本和税负，并标志着全球税务信息共享趋势的加强。 20%的税率适用于一个日历年内境外股票交易的净收益，但亏损不得结转至以后年度抵扣。中国已参与 CRS，该机制自动交换各司法管辖区间的金融账户信息。

telegram · zaihuapd · Jun 29, 08:01

**背景**: 根据中国个人所得税法，境外股票收益被归类为“财产转让所得”，适用 20%的税率。CRS（共同申报准则）是经合组织（OECD）推出的一项倡议，旨在促进各国之间自动交换金融账户信息，帮助税务机关识别未申报的境外资产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.shui5.cn/article/7f/85570.html">shui5.cn/article/7f/85570.html</a></li>
<li><a href="https://chenlitong.blog.caixin.com/archives/193957">CRS 已经开始打捞锦鲤，您的钱恐怕藏不住了-家族治理与传承-财新网</a></li>
<li><a href="https://xueqiu.com/7899180198/294107984">聊聊 境 外 投资 所 得 税 问题 经过 交 流后重新修改编辑，感谢JJacky123...</a></li>

</ul>
</details>

**标签**: `#tax regulation`, `#China`, `#overseas investment`, `#CRS`, `#personal finance`

---