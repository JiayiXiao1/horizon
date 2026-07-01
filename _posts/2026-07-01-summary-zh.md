---
layout: default
title: "Horizon Summary: 2026-07-01 (ZH)"
date: 2026-07-01
lang: zh
---

> From 37 items, 16 important content pieces were selected

---

1. [vLLM v0.24.0 新增 MiniMax-M3 支持与 DeepSeek-V4 优化](#item-1) ⭐️ 9.0/10
2. [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](#item-2) ⭐️ 9.0/10
3. [Anthropic 发布 Claude Sonnet 5，代理能力最强](#item-3) ⭐️ 9.0/10
4. [Claude Code 隐写标记请求](#item-4) ⭐️ 8.0/10
5. [Anthropic 推出 Claude Science 用于科学数据分析](#item-5) ⭐️ 8.0/10
6. [通过 WebAssembly 将 Kubernetes 移植到浏览器](#item-6) ⭐️ 8.0/10
7. [shot-scraper video：AI 代理录制演示视频](#item-7) ⭐️ 8.0/10
8. [Ornith-1.0：开源自脚手架 LLM，专为智能体编程打造](#item-8) ⭐️ 8.0/10
9. [华为开源盘古 2.0，含 505B 和 92B 两个版本](#item-9) ⭐️ 8.0/10
10. [Anthropic 发布 Claude Sonnet 4.6，性能大幅提升](#item-10) ⭐️ 8.0/10
11. [特斯拉监督版 FSD 在中国上线](#item-11) ⭐️ 8.0/10
12. [Google DeepMind 发布 Nano Banana 2 Lite](#item-12) ⭐️ 7.0/10
13. [Anthropic 获美政府批准，恢复向关键基础设施部署 Mythos 5](#item-13) ⭐️ 7.0/10
14. [存储芯片涨价引发手机厂商减产](#item-14) ⭐️ 7.0/10
15. [英国拟放宽苹果和谷歌应用商店支付规则](#item-15) ⭐️ 7.0/10
16. [Claude Desktop Linux 测试版上线，支持 Ubuntu 与 Debian](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 新增 MiniMax-M3 支持与 DeepSeek-V4 优化](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM v0.24.0 版本由 256 位贡献者提交了 571 次代码，新增了对 MiniMax-M3 多模态模型的支持，并对 DeepSeek-V4 进行了重大优化，包括 FlashInfer 稀疏索引缓存和预填充分块规划改进。 此版本显著扩展了 vLLM 的模型支持范围和推理性能，使 MiniMax-M3 和 DeepSeek-V4 等前沿开源模型的用户受益。优化降低了延迟并提高了吞吐量，使大规模 LLM 服务更加高效。 关键技术亮点包括集成了用于专家并行（EP）的 DeepEP v2、用于工具调用/推理的新流式解析器引擎，以及新增了用于扩散 LLM 的 DiffusionGemma。Rust 前端现在支持 API 密钥认证和 CORS，设备选择机制已改为使用 'device_ids' 参数，而非设置 CUDA_VISIBLE_DEVICES。

github · khluu · Jun 29, 19:41

**背景**: vLLM 是一个高性能的开源 LLM 推理和服务库，以其高效的内存管理和快速解码而广泛使用。MiniMax-M3 是一个多模态视觉语言模型，支持 100 万 token 的上下文窗口；DeepSeek-V4 是一个强大的开源权重模型，具有流形约束超连接（mHC）等架构创新。FlashInfer 是一个内核库，为 LLM 服务提供高效的注意力实现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://build.nvidia.com/minimaxai/minimax-m3/modelcard">minimax-m3 Model by Minimaxai | NVIDIA NIM</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#DeepSeek-V4`, `#MiniMax-M3`, `#open source`

---

<a id="item-2"></a>
## [美国解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制](https://twitter.com/AnthropicAI/status/2072106151890809341) ⭐️ 9.0/10

美国商务部已解除对 Anthropic 的 Claude Fable 5 和 Mythos 5 的出口管制，允许这些先进 AI 模型出口到国际。该决定是在 Anthropic 同意主动检测并解决与模型相关的安全风险之后做出的。 这一政策变化标志着 AI 监管的重大转变，可能影响美中竞争和全球 AI 市场。它还引发了对企业依赖前沿模型以及出口管制有效性的担忧。 Claude Fable 5 是一款已确保安全可供普遍使用的 Mythos 级模型，而 Mythos 5 则是一款专注于网络安全的模型，目前仅限经过审查的合作伙伴使用。这些模型于 2026 年 6 月 9 日在包括 AWS、Google Cloud 和 Microsoft Foundry 在内的多个平台上可用。

hackernews · Pragmata · Jun 30, 23:55 · [社区讨论](https://news.ycombinator.com/item?id=48740771)

**背景**: 对先进 AI 模型的出口管制旨在防止敏感技术落入对手手中，尤其是中国。Anthropic 的 Claude 模型是最强大的 AI 系统之一，其发布一直受到安全和滥用问题的关注。解除管制表明在安全与商业利益之间进行了重新评估。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude Platform Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀疑和担忧：一些人认为损害已经造成，企业无法依赖美国的前沿模型；另一些人指出，中国模型已证明无需大量资本支出就能具备竞争力。还有人批评政府的行动是作秀，安全措施早已存在。

**标签**: `#AI regulation`, `#export controls`, `#Anthropic`, `#US-China competition`, `#frontier models`

---

<a id="item-3"></a>
## [Anthropic 发布 Claude Sonnet 5，代理能力最强](https://t.me/zaihuapd/42280) ⭐️ 9.0/10

Anthropic 于 2026 年 6 月 30 日发布了 Claude Sonnet 5，称其是迄今代理能力最强的 Sonnet 模型，能够规划、使用浏览器和终端等工具并自主运行。该模型即日起面向所有套餐开放，Free 和 Pro 用户将默认使用该模型。 Claude Sonnet 5 以更低的价格提供了接近 Opus 级别的代理能力，使开发者和企业更容易获得先进的 AI 代理功能。此次发布标志着 AI 模型向更自主、能使用工具并独立处理复杂任务的趋势发展。 Claude Sonnet 5 在推理、工具使用、编码和知识工作方面优于 Sonnet 4.6，性能接近 Opus 4.8。定价为每百万输入 token 2 美元、输出 token 10 美元（截至 2026 年 8 月 31 日），比 Opus 4.8（5 美元/25 美元）更便宜。

telegram · zaihuapd · Jul 1, 01:12

**背景**: Anthropic 的 Claude 模型系列包括 Haiku（最快）、Sonnet（平衡）和 Opus（最强）。Sonnet 模型旨在平衡速度和能力，而 Opus 追求最高性能。代理型 AI 指能够自主规划并使用外部工具执行多步骤任务的模型，而不仅仅是生成文本回复。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-5">Introducing Claude Sonnet 5 \ Anthropic</a></li>
<li><a href="https://www.mejba.me/blog/claude-sonnet-5-agentic-coding">Claude Sonnet 5 Changes Everything About Agentic Coding</a></li>
<li><a href="https://www.digitalapplied.com/blog/claude-sonnet-5-agentic-coding-near-opus-price-2026">Claude Sonnet 5 : Near-Opus Agentic Coding at Sonnet Price</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些用户质疑其性价比，指出在更高努力级别下 Opus 的单位成本表现更好；而另一些用户则欣赏其速度和代理能力。一位用户的基准测试显示 Sonnet 5 在速度上表现良好，但在常识问答和组合工具调用任务上存在弱点。

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#agent`

---

<a id="item-4"></a>
## [Claude Code 隐写标记请求](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 8.0/10

Anthropic 的 Claude Code 工具使用隐写术在发出的请求中嵌入隐藏标识符，很可能用于检测中国公司未经授权进行模型蒸馏的行为。 这种做法引发了对 AI 开发者工具透明度和信任的严重担忧，因为用户可能不知道他们的请求包含可用于跟踪或执法的隐藏标记。 该隐写技术是通过逆向工程发现的；隐藏数据以用户不可见但 Anthropic 服务器可提取的方式嵌入。

hackernews · kirushik · Jun 30, 15:44 · [社区讨论](https://news.ycombinator.com/item?id=48734373)

**背景**: 隐写术是将信息隐藏在其他信息或物理对象中的做法。在 AI 领域，它可用于在模型输入或输出中隐藏数据。Claude Code 是 Anthropic 于 2025 年发布的一款智能编码工具，允许开发者通过终端中的自然语言委托编码任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic coding tool that lives in your terminal, understands your codebase, and helps you code faster by executing routine tasks, explaining complex code, and handling git workflows - all through natural language commands. · GitHub</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：一些人批评缺乏透明度，而另一些人则淡化严重性，认为其意图显然是防止中国公司进行模型蒸馏。少数用户表达了对 Anthropic 的不信任，并建议使用 Codex CLI 等开源替代品。

**标签**: `#steganography`, `#AI ethics`, `#Anthropic`, `#developer tools`, `#privacy`

---

<a id="item-5"></a>
## [Anthropic 推出 Claude Science 用于科学数据分析](https://claude.com/product/claude-science) ⭐️ 8.0/10

Anthropic 推出了 Claude Science，这是一个基于本地服务器的 AI 工作台，可集成数据库和高性能计算 (HPC) 集群，用于科学数据分析。 该工具使研究人员能够在安全环境中本地运行 AI 驱动的数据分析，弥合了先进 AI 能力与无法迁移到云的敏感科学数据之间的差距。 Claude Science 运行一个带有基于 Web 的 UI 的本地服务器，使其能够连接到机构集群和数据库，同时将数据保留在本地。它支持 pandas 等工具进行数据处理，并生成可审计的工件。

hackernews · lebovic · Jun 30, 17:07 · [社区讨论](https://news.ycombinator.com/item?id=48735770)

**背景**: 科学研究通常涉及敏感或专有数据，出于安全或合规原因无法在云端 AI 服务上处理。传统数据分析工作流程要求研究人员手动编码并管理计算资源。Claude Science 旨在提供一个 AI 助手，直接在研究人员的本地或机构计算环境中工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-science-ai-workbench">Claude Science, an AI workbench for scientists, is now available</a></li>
<li><a href="https://grokipedia.com/page/Claude_for_Life_Sciences">Claude for Life Sciences</a></li>
<li><a href="https://aithinkerlab.com/run-claude-ai-locally/">Can You Run Claude Locally in 2026? Real Answer + Workarounds</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调该工具的架构（本地服务器 + Web UI）是安全环境的关键差异化因素，一位评论者指出它与 HPC 集群的集成。一些用户发现它对特定任务（如设计生物农药）有用，而另一些用户则质疑其相对于现有工具（如 Claude Code 与 org-mode）的价值。

**标签**: `#AI`, `#data science`, `#Anthropic`, `#scientific computing`, `#HPC`

---

<a id="item-6"></a>
## [通过 WebAssembly 将 Kubernetes 移植到浏览器](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser) ⭐️ 8.0/10

ngrok 发布了一个名为“Wébernetes”的演示，通过 WebAssembly 在浏览器中完整运行 Kubernetes 集群，可通过 webernetes-demo.ngrok.app 访问。 这使得无需任何本地设置即可进行交互式 Kubernetes 学习和测试，降低了新手的入门门槛，并提供了安全的实验环境。 该项目在 GitHub 上以 ngrok/webernetes 开源，演示使用编译为 WebAssembly 的 k3s 运行单节点集群。

hackernews · peterdemin · Jun 30, 20:48 · [社区讨论](https://news.ycombinator.com/item?id=48738985)

**背景**: Kubernetes 是一个容器编排平台，通常需要机器集群来运行。WebAssembly（Wasm）是一种二进制指令格式，可在浏览器中以接近原生的速度运行。将 Kubernetes 移植到 Wasm 使其能在没有传统操作系统支持的环境中运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cncf.io/blog/2024/03/12/webassembly-on-kubernetes-from-containers-to-wasm-part-01/">WebAssembly on Kubernetes: from containers to Wasm (part 01) | CNCF</a></li>
<li><a href="https://ngrok.com/blog/ngrok-k8s">Introducing the ngrok Kubernetes Operator | ngrok blog</a></li>
<li><a href="https://github.com/ngrok/ngrok-operator">GitHub - ngrok/ngrok-operator: The official ngrok Kubernetes Operator · GitHub</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该项目的教育价值，认为它可以取代 Katacoda 等平台进行概念学习。一位评论者强调，将 AI 生成的代码与真实 Kubernetes 行为进行测试的工作流程是一个关键见解。

**标签**: `#Kubernetes`, `#WebAssembly`, `#Browser`, `#Education`, `#DevOps`

---

<a id="item-7"></a>
## [shot-scraper video：AI 代理录制演示视频](https://simonwillison.net/2026/Jun/30/shot-scraper-video/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 shot-scraper 1.10，新增了“shot-scraper video”命令，该命令使用 Playwright 根据 YAML 故事板文件录制 Web 应用程序操作的 WebM 视频。 该工具使 AI 编码代理能够自动生成其工作的可验证视频演示，解决了代理生成代码中信任和验证的关键需求。 故事板文件指定了服务器设置、视口、光标可见性、等待条件、JavaScript 覆盖（例如剪贴板模拟）以及一系列场景，包含暂停、点击和输入等操作。

rss · Simon Willison · Jun 30, 16:54

**背景**: shot-scraper 是一个使用 Playwright 对网页进行截图的命令行工具。新的 video 命令将其扩展到录制功能，使开发者和 AI 代理能够创建可重现的 Web 交互演示。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://shot-scraper.datasette.io/en/stable/video.html">Recording videos - shot - scraper</a></li>
<li><a href="https://simonwillison.net/2026/Jun/30/shot-scraper-video/">Have your agent record video demos of its work with shot - scraper ...</a></li>
<li><a href="https://www.remio.ai/post/shot-scraper-video-lets-ai-agents-record-demo-videos">Shot - scraper Video Lets AI Agents Record Demo Videos</a></li>

</ul>
</details>

**标签**: `#developer-tools`, `#automation`, `#testing`, `#playwright`, `#ai-agents`

---

<a id="item-8"></a>
## [Ornith-1.0：开源自脚手架 LLM，专为智能体编程打造](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce 发布了 Ornith-1.0，这是一个采用 MIT 许可证的新开源权重 LLM 系列，参数规模从 9B 到 397B 不等，在编码基准测试中达到了同类开源模型的最优性能。 Ornith-1.0 的自脚手架能力使其能够自主规划、编写、测试和调试代码，推动了智能体编程的发展并减少了人工干预。其 MIT 开源许可证促进了广泛采用和进一步研究。 该模型系列包括 9B Dense、31B Dense、35B MoE 和 397B MoE 变体，基于 Gemma 4 和 Qwen 3.5（均为 Apache 2.0 许可）。它支持高达 262k 的上下文长度，并兼容 vLLM 部署。

rss · Simon Willison · Jun 29, 16:17

**背景**: 智能体编程是指 AI 代理在最少人工输入下自主规划、编写、测试和修改代码。传统的编码助手需要逐步指导，而像 Ornith-1.0 这样的智能体模型可以独立处理复杂任务。Ornith-1.0 通过强化学习后训练学习自己的代理脚手架，这是一种称为自脚手架的新方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding | DeepReinforce Blog | Jun. 2026</a></li>
<li><a href="https://www.marktechpost.com/2026/06/25/deepreinforce-releases-ornith-1-0-an-open-source-coding-model-family-that-learns-its-own-rl-scaffolds/">DeepReinforce Releases Ornith-1.0: An Open-Source Coding Model Family That Learns Its Own RL Scaffolds - MarkTechPost</a></li>

</ul>
</details>

**标签**: `#LLM`, `#open-source`, `#coding`, `#agentic`, `#AI`

---

<a id="item-9"></a>
## [华为开源盘古 2.0，含 505B 和 92B 两个版本](https://t.me/zaihuapd/42259) ⭐️ 8.0/10

在 2026 年华为开发者大会上，华为宣布开源 openPangu 2.0 模型，包含 505B 总参数的 Pro 版和 92B 总参数的 Flash 版，支持 512K 上下文长度。公司计划从 6 月 30 日起陆续开源七大组件。 此次发布标志着开源 AI 生态的一个重要里程碑，华为旨在将盘古从中国领先模型推向世界领先。该大规模开源模型针对昇腾芯片和鸿蒙系统优化，可能加速全球 AI 应用和竞争。 Pro 版总参数为 505B，激活参数未公开；Flash 版总参数 92B，激活参数 6B。该模型更亲和昇腾算力，并适配鸿蒙系统。

telegram · zaihuapd · Jun 30, 06:01

**背景**: 华为早在 2021 年就发布了盘古大模型，早于 ChatGPT 引发的全球 AI 热潮。openPangu 2.0 基于华为昇腾 AI 芯片构建，旨在提供 GPT-4 等专有模型的开源替代方案。其 512K 上下文窗口可处理超长文档或对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/huawei-launches-openpangu-2-0-with-50-5b-parameters-and-512k-context">Huawei Launches OpenPangu 2 . 0 with 50.5 Billion... | KuCoin</a></li>
<li><a href="https://news.aibase.com/news/29268">Huawei openPangu 2 . 0 Launches Two Versions: Accelerating the...</a></li>
<li><a href="https://www.aimadetools.com/blog/best-chinese-open-source-ai-models-june-2026/">Best Chinese Open -Source AI Models June 2026: Pangu , DeepSeek...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Open Source`, `#Large Language Model`, `#Huawei`, `#Deep Learning`

---

<a id="item-10"></a>
## [Anthropic 发布 Claude Sonnet 4.6，性能大幅提升](https://t.me/zaihuapd/42277) ⭐️ 8.0/10

Anthropic 发布了 Claude Sonnet 4.6，在编程、计算机使用、长文本推理和智能体规划方面进行了全面升级。该模型现已作为 Free 和 Pro 用户的默认版本，并提供 1M token 上下文窗口。 此次发布显著提升了 AI 执行复杂编程任务和与计算机界面交互的能力，使其对开发者和知识工作者更加有用。1M token 上下文窗口使其能够处理超长文档和复杂的智能体工作流。 Claude Sonnet 4.6 在 OSWorld 基准测试中表现出显著进步，该模型通过查看截图并决定点击、输入等操作。该模型已通过 API 和主流云平台上线，定价与前代相同。

telegram · zaihuapd · Jun 30, 17:58

**背景**: Anthropic 的 Claude 模型是专为安全且强大的 AI 辅助而设计的大型语言模型。计算机使用功能允许模型通过解释截图并执行操作来直接与图形用户界面交互，从而实现通常需要人类鼠标和键盘输入的任务自动化。OSWorld 基准测试评估 AI 智能体在跨多个应用程序的真实计算机任务上的表现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>
<li><a href="https://cobusgreyling.substack.com/p/claude-sonnet-46-and-computer-use">Claude Sonnet 4.6 & Computer Use</a></li>
<li><a href="https://os-world.github.io/">OSWorld : Benchmarking Multimodal Agents for Open-Ended Tasks in...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#model release`

---

<a id="item-11"></a>
## [特斯拉监督版 FSD 在中国上线](https://t.me/zaihuapd/42281) ⭐️ 8.0/10

特斯拉在社交媒体平台 X 上宣布，其监督版全自动驾驶（FSD）系统现已在中国可用，标志着其先进驾驶辅助技术正式进入中国市场。 此次扩张意义重大，因为中国是全球最大的汽车市场，也是自动驾驶技术的关键战场，可能提升特斯拉的收入和相对于比亚迪、小鹏等本土竞争对手的竞争地位。 据报道，中国的监督版 FSD 相比美国版本功能有限，因为特斯拉只能使用本地数据进行训练并面临监管限制，预计其定价将与美国每月 99 美元的订阅价格类似。

telegram · zaihuapd · Jul 1, 01:22

**背景**: 特斯拉的 FSD 是一套需要驾驶员主动监督的先进驾驶辅助功能。该系统已开发多年，并逐步在特定市场推出。中国对自动驾驶数据有严格规定，要求外国公司本地存储和处理数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving ( Supervised ) | Tesla</a></li>
<li><a href="https://www.teslarati.com/tesla-china-expects-fsd-approval-end-of-2024-musk/">Tesla China FSD approval expected by end of 2024: Musk</a></li>
<li><a href="https://www.notebookcheck.net/Tesla-brings-half-baked-FSD-to-full-price-customers-in-China-as-it-can-only-use-local-data-for-training.967429.0.html">Tesla brings half-baked FSD to full-price customers in China as it can...</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#FSD`, `#autonomous driving`, `#China`, `#EV`

---

<a id="item-12"></a>
## [Google DeepMind 发布 Nano Banana 2 Lite](https://deepmind.google/models/gemini-image/flash-lite/) ⭐️ 7.0/10

Google DeepMind 发布了 Nano Banana 2 Lite，这是 Nano Banana 2 图像生成模型的蒸馏版本，推理速度更快且文本渲染能力提升，但仅限 Google One 订阅用户使用。 此次发布通过更快的速度使高质量图像生成更易于消费者使用，但 Google One 账户要求可能限制其普及，尤其是对 Workspace 用户。 Nano Banana 2 Lite 生成图像时间不到 5 秒，而基础模型约需 30 秒，但不支持编程控制宽高比，且处理高度精细提示的能力不如基础模型。

hackernews · minimaxir · Jun 30, 16:48 · [社区讨论](https://news.ycombinator.com/item?id=48735444)

**背景**: 模型蒸馏是一种技术，通过训练一个更小、更快的“学生”模型来模仿更大的“教师”模型，从而在降低计算成本的同时保留大部分质量。Google DeepMind 的 Nano Banana 系列专注于面向消费者应用的高效图像生成。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bentoml.com/blog/a-guide-to-open-source-image-generation-models">The Best Open-Source Image Generation Models in 2026</a></li>
<li><a href="https://blog.segmind.com/distilledstable-diffusion-models/">A Comprehensive Guide to Distilled Stable Diffusion Models</a></li>

</ul>
</details>

**社区讨论**: 社区评论反应不一：一些用户称赞速度和文本渲染改进，而另一些用户则批评 Google One 账户限制，并对房地产经纪人使用 AI 生成图像进行欺骗表示不满。还有用户指出对比图表中未包含 ChatGPT。

**标签**: `#AI`, `#image generation`, `#Google DeepMind`, `#model release`

---

<a id="item-13"></a>
## [Anthropic 获美政府批准，恢复向关键基础设施部署 Mythos 5](https://t.me/zaihuapd/42260) ⭐️ 7.0/10

2026 年 6 月 27 日，美国政府通知 Anthropic，其最强的网络安全模型 Mythos 5 可重新部署给运营和守卫关键基础设施的组织，此前该部署自 6 月 12 日起被暂停。 这一批准标志着政府政策转向允许先进 AI 模型用于关键基础设施防御，可能为未来高风险安全场景中的 AI 部署开创先例。 Anthropic 正在迅速为这些组织恢复访问，同时继续与政府协商，争取扩大 Mythos 5 的适用范围，并推动 Fable 5 模型的批准。Mythos 5 是一款专注于网络安全的模型，旨在发现软件漏洞。

telegram · zaihuapd · Jun 30, 07:04

**背景**: Claude Mythos 是 Anthropic 开发的大型语言模型，用于发现软件漏洞。出于安全和滥用担忧，Anthropic 此前未公开发布该模型。政府的暂停和随后的批准反映了在 AI 能力与安全风险之间寻求平衡的持续辩论。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#Anthropic`, `#government policy`, `#critical infrastructure`

---

<a id="item-14"></a>
## [存储芯片涨价引发手机厂商减产](https://t.me/zaihuapd/42265) ⭐️ 7.0/10

受存储芯片价格持续上涨影响，小米、OPPO、vivo 和传音等主要手机厂商已将 2026 年生产目标下调 15-20%，调整重点集中在中低端及海外机型。 这可能引发智能手机行业下滑，TrendForce 预测 2026 年产量将下降 7%，终端售价可能被迫上涨，影响整个供应链。 小米和 OPPO 订单下调超 20%，vivo 下调近 15%，传音亦调低目标。砍单主要针对成本敏感的中低端及海外机型，表明厂商正在消化部分成本压力。

telegram · zaihuapd · Jun 30, 08:44

**背景**: 存储芯片（包括 DRAM 和 NAND 闪存）是智能手机的关键部件。由于供应紧张以及 AI 和数据中心需求增加，其价格持续上涨，挤压了手机厂商的利润空间。

**标签**: `#storage chips`, `#smartphone industry`, `#supply chain`, `#price hike`, `#TrendForce`

---

<a id="item-15"></a>
## [英国拟放宽苹果和谷歌应用商店支付规则](https://www.reuters.com/world/uk-regulator-proposes-easing-apple-google-app-store-payment-rules-2026-06-30/) ⭐️ 7.0/10

2026 年 6 月 30 日，英国竞争与市场管理局（CMA）提议允许应用开发者将用户引导至苹果和谷歌应用商店之外的支付选项，并对这种引导收取的费用设定上限，以确保公平合理。 该提案可能大幅降低苹果和谷歌向开发者收取的 15-30%佣金，从而降低消费者成本并促进移动生态系统的竞争。 CMA 还考虑要求苹果开放用于非接触式支付的 NFC 技术，允许第三方支付服务在 iOS 应用内使用。该提案是英国新数字市场制度下咨询的一部分，最终决定预计于 2026 年晚些时候做出。

telegram · zaihuapd · Jun 30, 12:12

**背景**: CMA 是英国主要的竞争监管机构，负责促进市场竞争。2025 年，根据英国新的数字市场制度，苹果和谷歌被认定在移动生态中具有“战略市场地位”，这赋予 CMA 施加行为要求的权力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Competition_and_Markets_Authority">Competition and Markets Authority - Wikipedia</a></li>
<li><a href="https://www.gov.uk/government/organisations/competition-and-markets-authority">Competition and Markets Authority - GOV. UK</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lfZ2FEZ0R4RUJ3YkI0ZFZFWXd5Z0FQAQ?hl=en-GB&gl=GB&ceid=GB:en">Google News - CMA on Google's market status - Overview</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#app store`, `#regulation`, `#Apple`, `#Google`

---

<a id="item-16"></a>
## [Claude Desktop Linux 测试版上线，支持 Ubuntu 与 Debian](https://x.com/ClaudeDevs/status/2071988881717871065) ⭐️ 7.0/10

Anthropic 于 6 月 30 日发布了 Claude Desktop 的 Linux 测试版，为 Ubuntu 和 Debian 系统提供原生桌面支持。付费用户现在可以直接在桌面上使用 Claude Code、Claude Cowork 和聊天功能。 此次扩展将完整的桌面体验带给 Linux 用户，而 Linux 用户是之前依赖浏览器或终端访问的开发者和高级用户的关键群体。这巩固了 Claude 作为跨操作系统的多功能 AI 平台的地位。 该测试版最初仅支持 Ubuntu 和 Debian 发行版，并向所有付费计划开放。功能包括用于 AI 辅助编程的 Claude Code、用于非技术任务的 Claude Cowork 以及标准聊天界面。

telegram · zaihuapd · Jun 30, 17:12

**背景**: Claude 是 Anthropic 开发的一系列大型语言模型，采用宪法 AI 训练以确保伦理合规。此前，Linux 用户只能通过网页浏览器或终端与 Claude 交互；此桌面客户端提供了原生的集成体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://grokipedia.com/page/Claude_Cowork">Claude Cowork</a></li>

</ul>
</details>

**标签**: `#Claude`, `#Linux`, `#Desktop`, `#AI`, `#Ubuntu`

---