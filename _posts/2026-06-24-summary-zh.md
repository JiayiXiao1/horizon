---
layout: default
title: "Horizon Summary: 2026-06-24 (ZH)"
date: 2026-06-24
lang: zh
---

> From 32 items, 21 important content pieces were selected

---

1. [FFmpeg 严重漏洞允许通过恶意视频远程执行代码](#item-1) ⭐️ 9.0/10
2. [中国灵晟超算时隔八年登顶 TOP500](#item-2) ⭐️ 9.0/10
3. [所见即所得的 TikZ 编辑器，支持源码同步](#item-3) ⭐️ 8.0/10
4. [即将到来的循环：AI 代理重塑软件开发](#item-4) ⭐️ 8.0/10
5. [Unlimited OCR：长文档解析的恒定内存方案](#item-5) ⭐️ 8.0/10
6. [谷歌因非官方 Workspace CLI 解雇员工](#item-6) ⭐️ 8.0/10
7. [提示注入即角色混淆：LLM 优先考虑风格而非内容](#item-7) ⭐️ 8.0/10
8. [Moebius 0.2B 图像修复模型通过 WebGPU 移植到浏览器](#item-8) ⭐️ 8.0/10
9. [OpenAI 将制作 AI 动画电影《Critterz》，成本不到 3000 万美元](#item-9) ⭐️ 8.0/10
10. [Valve 发布 Steam Machine 游戏主机，起售价 1049 美元](#item-10) ⭐️ 8.0/10
11. [美国人形机器人依赖中国零部件](#item-11) ⭐️ 8.0/10
12. [SpaceX 猎鹰重型火箭将于 2028 年发射欧洲火星车](#item-12) ⭐️ 8.0/10
13. [FUTO Swipe：新滑行输入模型发布](#item-13) ⭐️ 7.0/10
14. [Swift Package Index 被苹果收购](#item-14) ⭐️ 7.0/10
15. [维生素 D 益处真实但仅限于缺乏者](#item-15) ⭐️ 7.0/10
16. [加州 AB 2047 法案要求 3D 打印机内置枪支检测功能](#item-16) ⭐️ 7.0/10
17. [Datasette 1.0a35 新增创建/修改表界面](#item-17) ⭐️ 7.0/10
18. [中国高校大规模撤销外语专业](#item-18) ⭐️ 7.0/10
19. [三星发布 UFS 5.0，带宽 10.8 GB/s，面向端侧 AI](#item-19) ⭐️ 7.0/10
20. [不精准洗牌需 14 次才能随机化一副牌](#item-20) ⭐️ 7.0/10
21. [LastPass 因合作伙伴 Klue 遭入侵导致客服数据泄露](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [FFmpeg 严重漏洞允许通过恶意视频远程执行代码](https://cybernews.com/security/critical-ffmpeg-vulnerability-enables-complete-compromise/) ⭐️ 9.0/10

在 FFmpeg 的 MagicYUV 解码器中发现了严重远程代码执行漏洞 CVE-2026-8461（代号 PixelSmash），攻击者通过播放或存储一个 50 KB 的恶意视频文件即可完全控制系统。FFmpeg 已发布 8.1.2 版本修复该问题。 FFmpeg 是使用最广泛的媒体处理库，嵌入在 VLC、Jellyfin、Kodi、OBS 和 Nextcloud 等应用中，影响数十亿设备，包括桌面、服务器、NAS 和 IoT 设备。该漏洞可实现无痕迹的静默攻击，因此立即更新至关重要。 该漏洞是 libavcodec 中 MagicYUV 解码器的堆越界写入问题，CVSS 评分为 8.8。不仅播放视频会触发，自动生成缩略图或媒体库扫描也可能中招，影响所有使用 FFmpeg 的平台。

telegram · zaihuapd · Jun 23, 15:00

**背景**: FFmpeg 是一个免费开源的多媒体框架，几乎所有视频播放器、流媒体服务和媒体服务器都使用它来解码、编码和处理音视频。MagicYUV 是一种无损视频编解码器，专为高速编辑设计，但 FFmpeg 中的解码器存在越界写入漏洞，可被利用执行代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://jfrog.com/blog/pixelsmash-critical-ffmpeg-vulnerability-turns-media-files-into-weapons/">CVE - 2026 - 8461 Turns Video into a Host for Remote Code Execution</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/ffmpeg-fixes-pixelsmash-flaw-in-widely-used-video-decoder/">FFmpeg fixes PixelSmash flaw in widely used video decoder</a></li>

</ul>
</details>

**标签**: `#ffmpeg`, `#vulnerability`, `#remote code execution`, `#security`, `#cve`

---

<a id="item-2"></a>
## [中国灵晟超算时隔八年登顶 TOP500](https://news.mydrivers.com/1/1131/1131573.htm) ⭐️ 9.0/10

6 月 23 日，部署于深圳国家超算中心的灵晟超算以 2.198 ExaFLOPS 的 HPL 性能位列 TOP500 榜首，成为全球首台纯 CPU 设计突破 2 ExaFLOPS 的系统。 这标志着中国时隔八年重返超算榜首，展示了国产 CPU 技术的重大进步和国家科技自主可控能力，尤其是在美国 GPU 出口限制的背景下。 灵晟采用 40960 颗 LX2 处理器，每颗含 304 个 Armv9 核心，主频 1.55 GHz，总计 245 万个核心。它还在 HPCG 基准测试中位居首位，在 HPL-MxP 混合精度测试中排名第四。

telegram · zaihuapd · Jun 23, 15:30

**背景**: TOP500 榜单基于高性能 Linpack（HPL）基准测试对全球最强超算进行排名，该测试衡量双精度浮点性能。此前榜首是美国使用 GPU 加速器的 El Capitan。灵晟的成就引人注目，因为它完全依赖 CPU，避免了对受美国出口管制的高级 GPU 的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.hpcwire.com/2026/04/28/china-unveils-2-exaflop-all-cpu-lineshine-supercomputer/">China Unveils 2 Exaflop, All-CPU 'LineShine' Supercomputer - HPCwire</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/china-bypasses-us-gpu-bans-with-1-54-exaflops-lineshine-supercomputer-cpu-only-monster-packs-2-4-million-huawei-designed-armv9-cores">China bypasses US GPU bans with 1.54-exaflops 'LineShine' supercomputer — CPU-only monster packs 2.4 million Huawei-designed Armv9 cores | Tom's Hardware</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/supercomputers/chinas-lineshine-supercomputer-dethrones-us-el-capitan-secures-first-place-in-top-500-list-first-machine-in-the-rankings-to-sustain-more-than-2-exaflops-of-double-precision-performance-using-only-cpus">China's LineShine supercomputer dethrones US' El Capitan, secures first place in Top 500 list — first machine in the rankings to sustain more than 2 ExaFLOPS of double-precision performance using only CPUs | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#supercomputing`, `#TOP500`, `#HPC`, `#China`, `#LineShine`

---

<a id="item-3"></a>
## [所见即所得的 TikZ 编辑器，支持源码同步](https://tikz.dev/editor/) ⭐️ 8.0/10

一款开源的所见即所得 TikZ 编辑器已发布，用户可通过拖拽和调整元素来编辑 TikZ 图形，源代码与渲染图形保持同步。该编辑器几乎完全由 Codex 编码代理构建。 该工具解决了学术界和 LaTeX 用户手动编写 TikZ 图形的一大痛点，大幅减少了调整坐标和重新编译的时间。同时，它也展示了 AI 编码代理如何能够构建出原本因过于繁琐而难以实现的复杂软件。 该编辑器解析 TikZ 代码并追踪每个对象的精确源码位置，拖拽时仅覆盖坐标中的数字，而不改变其他代码结构。它还包含从 SVG、PPTX 和 IPE 到 TikZ 的转换器，并重新实现了 LaTeX 的连字符和换行算法以支持多行节点。

hackernews · DominikPeters · Jun 23, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48645437)

**背景**: TikZ 是一个强大的 LaTeX 宏包，用于以编程方式创建矢量图形，广泛应用于学术论文中。传统上，用户通过编写 \draw 等命令并反复编译来调整位置，非常耗时。所见即所得（WYSIWYG）编辑器允许直接进行可视化操作，但现有工具很少能将可视化编辑与实时源代码同步结合起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PGF/TikZ">PGF/TikZ - Wikipedia</a></li>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://en.wikipedia.org/wiki/WYSIWYG_editor">WYSIWYG editor</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞该项目解决了实际需求，有用户表示自己学生时代就想要这样的工具。但也有批评指出生成的 TikZ 代码不必要地使用了绝对坐标，建议改进。还有人将其与 quiver.app 等专业工具比较，并询问是否支持 Typst 的 cetz 包。

**标签**: `#LaTeX`, `#TikZ`, `#editor`, `#academic tools`, `#open source`

---

<a id="item-4"></a>
## [即将到来的循环：AI 代理重塑软件开发](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Flask 框架的创建者 Armin Ronacher 认为，AI 编码代理引入了一个新的“循环”，开发者需要投入更多时间预先编写规范并与代理迭代，从而将开发范式转向一种更生物性的、类似生命体与代码的关系。 这种范式转变可能从根本上改变软件的设计和维护方式，更强调规范编写和迭代优化而非直接编码，影响所有采用 AI 编码代理的开发者。 Ronacher 指出，虽然代理可以快速生成代码，但它们需要清晰详细的规范才能产生高质量结果，而开发者通常需要多次迭代来完善规范和输出。文章强调，这个循环反映了通过反复失败尝试来理解问题的过程。

hackernews · ingve · Jun 23, 11:06 · [社区讨论](https://news.ycombinator.com/item?id=48643180)

**背景**: Armin Ronacher 是知名的开源开发者，以创建 Flask Web 框架和 Jinja 模板引擎而闻名。AI 编码代理（例如基于大型语言模型的工具）可以根据自然语言提示生成代码，但通常难以处理复杂或模糊的需求。“循环”指的是开发者在使用这些工具时经历的规范编写、代理执行和优化的迭代周期。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Armin_Ronacher">Armin Ronacher</a></li>
<li><a href="https://tosea.ai/blog/loop-engineering-ai-agents-complete-guide-2026">What Is Loop Engineering? A Complete Guide from Prompt... | Tosea. ai</a></li>
<li><a href="https://digg.com/tech/mumvj4el">Geoffrey Litt argues AI coding agents struggle with UI because...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍同意 Ronacher 的观点，指出他们遇到的瓶颈是规范编写而非代码生成。一些人观察到，当开发者清楚自己想要什么时，循环最为有效，代理在获得精确规范后可以表现出色。其他人则强调范式正在转向将软件视为需要培育而非直接控制的活生物体。

**标签**: `#AI agents`, `#software development`, `#paradigm shift`, `#specification`, `#programming`

---

<a id="item-5"></a>
## [Unlimited OCR：长文档解析的恒定内存方案](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

百度研究人员推出了 Unlimited OCR，该方法用因果参考滑动窗口注意力（R-SWA）替代标准注意力，使 KV 缓存内存不随输出长度增长，从而无需逐页分块即可一次性解析整个文档。 这一突破消除了端到端 OCR 处理长文档的主要瓶颈，使得单次处理整本书籍或报告而不耗尽 GPU 内存成为可能，有望显著提升数字化、归档和文档分析工作流的效率。 该方法在保持或提升解析任务精度的同时实现了恒定内存使用，论文可在 arXiv（2606.23050）上获取。实现代码已在百度组织的 GitHub 上开源。

hackernews · ingve · Jun 23, 11:35 · [社区讨论](https://news.ycombinator.com/item?id=48643426)

**背景**: 在基于 Transformer 的 OCR 模型中，键值（KV）缓存存储过去的 token 表示以避免重复计算，但其内存占用随输出长度线性增长，导致长文档出现内存不足错误。传统的解决方法是把文档分页处理，但这可能丢失上下文并降低精度。Unlimited OCR 的 R-SWA 机制将注意力限制在固定大小的滑动窗口内，从而消除了线性内存增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pandaily.com/baidu-unlimited-ocr-constant-kv-cache-jun2026">Baidu Unveils Unlimited-OCR: Constant KV Cache Delivers SOTA Performance on Long Documents - Pandaily</a></li>
<li><a href="https://www.xugj520.cn/en/archives/unlimited-ocr-constant-memory.html">Unlimited OCR: One-Shot Long-Horizon Document Parsing with Constant Memory | Efficient Coder</a></li>
<li><a href="https://arxiv.org/html/2606.23050v1">Unlimited OCR Works Welcome the Era of One-shot Long-horizon Parsing</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区称赞这是一项巧妙的架构技巧，用户提到了乐谱识别等应用，并对团队致谢 DeepSeek-OCR 和 PaddleOCR 表示赞赏。还有人指出项目名称源自《Fate/stay night》的梗。

**标签**: `#OCR`, `#AI`, `#memory optimization`, `#deep learning`, `#open source`

---

<a id="item-6"></a>
## [谷歌因非官方 Workspace CLI 解雇员工](https://twitter.com/JPoehnelt/status/2069482265953087602) ⭐️ 8.0/10

谷歌员工 Justin Poehnelt 因创建并发布一个可能被误认为是官方产品的非官方 Google Workspace CLI 工具而被解雇。 这一事件凸显了员工创新与企业官僚主义之间的紧张关系，引发了对开源政策以及大型科技公司副业项目风险的质疑。 该工具以 Poehnelt 的个人账户发布，在 GitHub 上大受欢迎，但违反了谷歌禁止发布可能被误认为官方产品的政策。Poehnelt 可能在解雇前已收到警告。

hackernews · justinwp · Jun 23, 18:13 · [社区讨论](https://news.ycombinator.com/item?id=48649011)

**背景**: 谷歌曾有因内部工具政策违规而解雇员工的历史，例如 2019 年一名员工因修改安全工具被解雇。公司曾鼓励副业项目的“20%时间”政策已被缩减。Google Workspace CLI (gws) 现在是官方工具，但 Poehnelt 的非官方版本早于它。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Google_Workspace_CLI">Google Workspace CLI</a></li>
<li><a href="https://github.com/googleworkspace/cli">GitHub - googleworkspace/cli: Google Workspace CLI — one command-line tool for Drive, Gmail, Calendar, Sheets, Docs, Chat, Admin, and more. Dynamically built from Google Discovery Service. Includes AI agent skills.</a></li>
<li><a href="https://www.theverge.com/2019/12/17/21024472/google-employee-fired-labor-rights-notification-tool">Google employee says she was fired for sending internal pop-ups about labor rights | The Verge</a></li>

</ul>
</details>

**社区讨论**: 评论意见分歧：一些人批评 Poehnelt 缺乏判断力，发布可能被误认为官方产品的工具；另一些人则认为这是官僚主义过度干预的案例，引用了 Pournelle 的官僚铁律。一些前谷歌员工指出，以个人账户发布项目很常见，但警告此案越过了界限。

**标签**: `#Google`, `#CLI`, `#Open Source`, `#Corporate Policy`, `#Bureaucracy`

---

<a id="item-7"></a>
## [提示注入即角色混淆：LLM 优先考虑风格而非内容](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Charles Ye、Jasmine Cui 和 Dylan Hadfield-Menell 的研究表明，LLM 无法可靠地区分特权文本（如系统提示）和不可信的用户输入，因为它们优先考虑文本风格而非内容，从而导致有效的越狱攻击。 这一发现揭示了 LLM 安全性的根本缺陷，表明当前针对提示注入的防御措施本质上是脆弱的，可能需要模型在角色感知方式上进行范式转变。 研究人员引入了“去风格化”——重写文本使其看起来不像角色标签中的预期格式——这使数据集中的攻击成功率从 61% 降至 10%，尽管对人类来说含义保持不变。

rss · Simon Willison · Jun 22, 23:59

**背景**: 提示注入是一种网络安全攻击，恶意输入导致 LLM 产生意外行为，通常绕过安全护栏。LLM 被训练为遵循指令，但难以区分开发者定义的提示和用户输入，尤其是当风格模仿内部角色标签（如 <system> 或 <assistant>）时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://arxiv.org/html/2603.12277v2">Prompt Injection as Role Confusion</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的讨论中，人们赞赏博客风格的写作，并担忧角色混淆使提示注入成为“永无止境的打地鼠游戏”。一些评论者质疑当前架构是否能实现真正的角色感知。

**标签**: `#prompt injection`, `#LLM security`, `#role confusion`, `#jailbreak`, `#AI safety`

---

<a id="item-8"></a>
## [Moebius 0.2B 图像修复模型通过 WebGPU 移植到浏览器](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison 成功将 Moebius 0.2B 轻量级图像修复模型移植到浏览器中，完全通过 WebGPU 运行，在线演示位于 simonw.github.io/moebius-web/。移植过程使用了 Claude Code 和基于 WebGPU 后端的 ONNX Runtime Web。 这使得高级图像修复功能无需专用 GPU 即可使用，用户只需在支持 WebGPU 的浏览器中直接运行模型。这展示了在客户端运行复杂 AI 模型的可行性日益增强，有助于降低服务器成本并提升隐私保护。 原始 Moebius 模型需要 PyTorch 和 NVIDIA CUDA，但浏览器移植版使用 ONNX Runtime Web 和 WebGPU 后端进行推理。该模型仅有 0.2B 参数，但在修复基准测试中性能可与 FLUX.1 等 10B+ 模型媲美。

rss · Simon Willison · Jun 22, 23:43

**背景**: 图像修复是指用合理的内容填充图像中缺失或移除的区域。Moebius 是一个轻量级框架，仅用 0.2B 参数即可实现高质量修复，挑战了大型基础模型必不可少的观念。WebGPU 是一种现代浏览器 API，可直接在浏览器中实现 GPU 加速计算和 AI 推理，并于 2026 年成为 W3C 推荐标准。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.19195">[2606.19195] Moebius: 0.2B Lightweight Image Inpainting ...</a></li>
<li><a href="https://github.com/hustvl/Moebius">GitHub - hustvl/Moebius: [ECCV 2026] Moebius: 0.2B ...</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius: 0.2B Lightweight Image Inpainting Framework with 10B ...</a></li>

</ul>
</details>

**社区讨论**: 文章引用的 Hacker News 讨论可能赞扬了实际的移植工作以及使用 Claude Code 进行代理编程。一些评论者可能讨论了基于浏览器与服务器端推理之间的权衡，或者其他模型类似移植的潜力。

**标签**: `#image inpainting`, `#WebGPU`, `#browser AI`, `#model porting`, `#machine learning`

---

<a id="item-9"></a>
## [OpenAI 将制作 AI 动画电影《Critterz》，成本不到 3000 万美元](https://t.me/zaihuapd/42125) ⭐️ 8.0/10

OpenAI 正支持制作一部名为《Critterz》的动画长片，该片将主要使用 OpenAI 自家的 AI 工具（包括 GPT-5）完成。影片预算不到 3000 万美元，制作周期仅为 9 个月，远低于传统动画电影。 这标志着 OpenAI 首次涉足长片电影制作，展示了生成式 AI 大幅降低动画行业成本和制作时间的潜力。如果成功，可能颠覆传统动画工作流程，加速 AI 在创意产业的应用。 该片计划在戛纳电影节首映，并于 2026 年在全球影院上映。OpenAI 的 GPT-5 将在制作过程中发挥关键作用，该模型在多种任务上具备博士级能力。

telegram · zaihuapd · Jun 23, 03:11

**背景**: 传统动画电影通常成本超过 1 亿美元，制作周期为 3-5 年。OpenAI 的 GPT-5 相比前代模型有显著提升，在编程、写作和视觉感知方面具备最先进的性能，使其适合电影制作等复杂创意任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5">GPT-5 - Wikipedia</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5/">Introducing GPT-5 | OpenAI</a></li>
<li><a href="https://openai.com/gpt-5/">GPT-5 is here | OpenAI</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI filmmaking`, `#animation`, `#GPT-5`, `#generative AI`

---

<a id="item-10"></a>
## [Valve 发布 Steam Machine 游戏主机，起售价 1049 美元](https://store.steampowered.com/hardware/steammachine) ⭐️ 8.0/10

Valve 发布了新款 Steam Machine，这是一款运行 SteamOS 3 的紧凑型游戏主机，起售价 1049 美元，声称性能是 Steam Deck 的 6 倍以上。 这标志着 Valve 在十年后重返主机市场，可能提供一种高性能、类似 PC 的游戏体验，以客厅设备的形式挑战传统主机和 PC 游戏。 Steam Machine 是一个小型立方体设备，设计用于连接电视或显示器，附带 Steam Controller 无线适配器，并具有可自定义的 LED 灯条，可显示游戏下载进度。

telegram · zaihuapd · Jun 23, 04:53

**背景**: Steam Machine 最初于 2015 年发布，但由于市场反响不佳，于 2018 年停产。新款型号运行基于 Arch Linux 的 SteamOS 3，并包含用于 Windows 游戏兼容性的 Proton。Steam Deck 是 Valve 于 2022 年发布的手持游戏 PC，取得了巨大成功，新款 Steam Machine 似乎借助了这一成功，以更强大的家用主机形态出现。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Steam_Machine">Steam Machine</a></li>
<li><a href="https://en.wikipedia.org/wiki/SteamOS">SteamOS</a></li>
<li><a href="https://store.steampowered.com/steamos/">SteamOS</a></li>

</ul>
</details>

**标签**: `#gaming`, `#hardware`, `#Valve`, `#SteamOS`, `#console`

---

<a id="item-11"></a>
## [美国人形机器人依赖中国零部件](https://t.me/zaihuapd/42129) ⭐️ 8.0/10

《华尔街日报》报道称，美国人形机器人在电机、关节、磁体和传感器等关键零部件上越来越依赖中国供应链。迪士尼的“奥拉夫”机器人使用了中国宇树科技的部件，特斯拉也正与中国供应商合作推进 Optimus 的量产准备。 这种依赖凸显了重要的地缘政治和产业趋势：美国机器人公司依靠中国制造获取成本优势。这引发了对供应链安全和竞争力的担忧，促使美国议员提出法案评估风险。 中国 2025 年推出了 28 款人形机器人，数量接近美国企业的 3 倍。摩根士丹利估算，中国供应链最多可将制造成本压低三分之二。

telegram · zaihuapd · Jun 23, 07:47

**背景**: 人形机器人需要电机、关节和传感器等复杂部件来实现运动和交互。中国凭借其制造规模和成本效率已成为这些部件的主要生产国。特斯拉和迪士尼等美国公司正利用中国供应商来加速开发并降低成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.163.com/dy/article/JO7AAQTE051100B9.html">m.163.com/dy/article/JO7AAQTE051100B9.html</a></li>
<li><a href="https://cloud.tencent.com/developer/news/4070576">机构：特斯拉Optimus V3推动人形机器人产业发展，超10家中国供应商已...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1988193930685223756">人形机器人关键零部件：电机全景解析 - 知乎</a></li>

</ul>
</details>

**标签**: `#humanoid robots`, `#supply chain`, `#US-China tech competition`, `#robotics`, `#manufacturing`

---

<a id="item-12"></a>
## [SpaceX 猎鹰重型火箭将于 2028 年发射欧洲火星车](https://t.me/zaihuapd/42133) ⭐️ 8.0/10

美国宇航局周四确认，已选定 SpaceX 的猎鹰重型火箭于 2028 年底从肯尼迪航天中心发射欧洲航天局的罗莎琳德·富兰克林号火星车。该任务旨在寻找火星地表下过去或现在存在生命的迹象。 这一里程碑结束了 ExoMars 计划二十多年的延误和预算问题，为欧洲首辆深钻火星车确定了发射工具。NASA、ESA 和 SpaceX 之间的合作加强了火星探索领域的国际联系，并利用了猎鹰重型火箭成熟的重型运载能力。 罗莎琳德·富兰克林号火星车设计可钻入火星地表下两米深处，比以往任何火星车都深，以采集样本进行生物特征分析。NASA 将提供关键硬件，包括发射服务、下降模块的制动系统以及放射性同位素加热单元。

telegram · zaihuapd · Jun 23, 10:47

**背景**: 罗莎琳德·富兰克林号火星车原为 ExoMars 计划的一部分，由 ESA 建造，俄罗斯航天局曾参与，但合作因俄乌冲突而终止。NASA 介入提供发射和关键部件，任务现定于 2028 年由猎鹰重型火箭发射。猎鹰重型是一种超重型运载火箭，由三个猎鹰 9 号芯级组成，能够将大型载荷送往火星。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rosalind_Franklin_(rover)">Rosalind Franklin (rover)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Falcon_Heavy">Falcon Heavy - Wikipedia Falcon Heavy - SpaceX Images SpaceX Falcon Heavy — 12+ Flights, Specs, Payload & Mission ... SpaceX launch vehicles - Wikipedia Falcon Heavy & Starman - YouTube Starship's Twelfth Flight Test - SpaceX Falcon Heavy Compendium - ElonX.net</a></li>
<li><a href="https://arstechnica.com/space/2026/04/after-a-saga-of-broken-promises-a-european-rover-finally-has-a-ride-to-mars/">After a saga of broken promises, a European rover ... - Ars Technica</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Mars mission`, `#NASA`, `#ESA`, `#space exploration`

---

<a id="item-13"></a>
## [FUTO Swipe：新滑行输入模型发布](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO 发布了 FUTO Swipe，这是为其注重隐私的键盘开发的新滑行输入模型，该模型基于用户贡献的数据进行训练，旨在与 Gboard 的准确性相媲美。 这解决了注重隐私的用户此前为了离线功能而不得不牺牲滑行输入质量的主要痛点，可能推动移动键盘领域转向开源、尊重隐私的替代方案。 滑行输入库采用 GPLv3 许可，而 Android 键盘应用则使用单独的 FUTO 许可。该模型可在 Hugging Face 上获取，并基于选择加入的用户数据进行训练。

hackernews · futohq · Jun 23, 17:50 · [社区讨论](https://news.ycombinator.com/item?id=48648619)

**背景**: 滑行输入允许用户通过在字母上滑动手指来输入单词，依赖神经网络模型预测目标单词。FUTO 键盘是一款完全离线、开源的 Android 键盘，优先考虑隐私，但其滑行准确性落后于 Gboard。这个新模型旨在缩小这一差距。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://keyboard.futo.org/">FUTO Keyboard</a></li>
<li><a href="https://huggingface.co/models?other=swipe-typing">Models – Hugging Face</a></li>
<li><a href="https://play.google.com/store/apps/details?id=org.futo.inputmethod.latin.playstore&hl=en_US">FUTO Keyboard - Apps on Google Play</a></li>

</ul>
</details>

**社区讨论**: 用户报告称新模型感觉与 Gboard 一样好，有些人已完全转为使用它。然而，仍存在随机大写和缺乏上下文感知建议等问题。一位评论者指出滑行输入库（GPLv3）与键盘应用（FUTO 许可）之间的许可差异。

**标签**: `#mobile keyboard`, `#swipe typing`, `#machine learning`, `#open source`, `#privacy`

---

<a id="item-14"></a>
## [Swift Package Index 被苹果收购](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 7.0/10

苹果已收购 Swift Package Index（SPI），这是一个由社区维护的 Swift 包搜索引擎。SPI 团队将加入苹果，致力于改进 Swift 包生态系统。 此次收购表明苹果加大对 Swift 包生态系统的投入，但也引发了对索引未来开放性和治理的担忧。社区担心苹果可能施加限制，或将自身利益置于社区需求之上。 SPI 团队明确提到开发者身份验证是未来方向，这引发了不安。该索引目前仅支持 GitHub 仓库，一些社区成员认为这是创建替代方案的机会。

hackernews · JDevlieghere · Jun 23, 18:00 · [社区讨论](https://news.ycombinator.com/item?id=48648779)

**背景**: Swift Package Index 是一个由社区运行的搜索引擎，帮助开发者发现 Swift 包并检查它们与各种平台的兼容性。它的创建是为了解决 Swift（苹果用于 iOS、macOS 等平台的编程语言）缺乏中央包注册表的问题。其他生态系统如 JavaScript 的 npm 或 Python 的 PyPI 都有常见的包注册表，而 Swift 一直依赖去中心化解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sesamedisk.com/apple-joins-swift-package-index/">What Happened: Apple Joins Swift Package Index - Sesame Disk</a></li>
<li><a href="https://www.swift.org/packages/">Packages | Swift .org</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：有人为 SPI 团队的成功感到高兴，也有人对苹果在开源和开发者服务方面的记录持怀疑态度。担忧包括可能对索引包进行监管以及关注开发者身份验证。

**标签**: `#Swift`, `#Apple`, `#Package Management`, `#Open Source`, `#Ecosystem`

---

<a id="item-15"></a>
## [维生素 D 益处真实但仅限于缺乏者](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

一项对维生素 D 研究的批判性综述得出结论，益处确实存在，但主要针对严重缺乏者，反驳了过度宣传和完全否定两种极端观点。 这一细致入微的分析有助于澄清关于维生素 D 补充剂的持续争论，为公共卫生建议和个人决策提供指导。 该综述指出，许多研究未能测量基线维生素 D 水平，且益处最显著的是那些水平低于 30 nmol/L 的人群。

hackernews · surprisetalk · Jun 23, 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48647486)

**背景**: 维生素 D 是一种脂溶性维生素，对骨骼健康和免疫功能至关重要。在日照有限的地区缺乏很常见，补充剂的使用存在广泛争议。

**社区讨论**: 评论者称赞了这种平衡的分析，一些人指出维生素 K2 可能有助于吸收，且个体剂量不同。其他人则指出了早期研究中的方法论缺陷。

**标签**: `#nutrition`, `#vitamin D`, `#health research`, `#evidence-based medicine`

---

<a id="item-16"></a>
## [加州 AB 2047 法案要求 3D 打印机内置枪支检测功能](https://www.the3dprintingnerd.com/ab2047) ⭐️ 7.0/10

加州议会 2025 年提出的 AB 2047 法案要求，到 2028 年 7 月 1 日，所有在该州销售的 3D 打印机必须配备枪支蓝图检测软件，并禁止使用开源替代方案。 若该法案通过，将为美国 3D 打印技术监管树立先例，可能扼杀教育和小企业的创新，同时引发关于审查制度和技术可行性的严重担忧。 该法案要求制造商为每种打印机型号提交证明，确认已配备枪支蓝图检测算法，并明确禁止使用绕过该要求的开源固件。

hackernews · Buildstarted · Jun 23, 22:12 · [社区讨论](https://news.ycombinator.com/item?id=48652184)

**背景**: 3D 打印机可用于制造塑料枪支部件，包括所谓的无序列号“幽灵枪”。加州此前已通过限制 3D 打印枪支的法律，但 AB 2047 是首个要求打印机内置检测技术的法案。批评者认为，此类软件在技术上不可行，因为 3D 打印机读取的是几何数据而非意图，且很容易被规避。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260AB2047">Bill Text - AB-2047 Firearms: 3-dimensional printing blocking technology.</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/dangers-californias-legislation-censor-3d-printing">The Dangers of California’s Legislation to Censor 3D Printing</a></li>
<li><a href="https://www.techspot.com/news/112594-california-assembly-passes-bill-requiring-gun-blocking-software.html">California passes bill requiring gun-blocking software in 3D ...</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了强烈反对，用户将其类比为失败的内容过滤系统，并指出有动机的个人可以轻松绕过这些限制。有人猜测该法案由布隆伯格支持的游说团体资助，另一些人则质疑 3D 打印武器的实际威胁，认为它们在统计上属于异常值。

**标签**: `#3D printing`, `#regulation`, `#California law`, `#education`, `#technology policy`

---

<a id="item-17"></a>
## [Datasette 1.0a35 新增创建/修改表界面](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 引入了新的“创建表”和“修改表”界面，均基于 JSON API，用户可以通过 Web 界面或编程方式定义列、主键、约束等。 此版本是 Datasette 1.0 的重要里程碑，通过 UI 和 API 实现模式管理，大幅扩展了其作为数据探索和发布工具的能力，而此前只能通过 SQLite 命令完成。 “创建表”API 支持定义列、主键、自定义列类型、NOT NULL 约束、字面默认值、表达式默认值和单列外键。“修改表”API 支持添加、重命名、重新排序和删除列，以及更改列类型、默认值、约束、主键、外键和重命名表。

rss · Simon Willison · Jun 23, 21:34

**背景**: Datasette 是一个用于探索和发布表格数据的开源工具，提供 Web 界面和 JSON API 来查询 SQLite 数据库。在此版本之前，创建或修改表模式需要直接使用 SQLite 命令或外部工具，限制了 Datasette 作为全功能数据库管理界面的可用性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#open-source`, `#data-exploration`, `#release`

---

<a id="item-18"></a>
## [中国高校大规模撤销外语专业](https://t.me/zaihuapd/42130) ⭐️ 7.0/10

包括对外经济贸易大学和北京语言大学在内的多所中国高校宣布停止日语笔译、意大利语口译等硕士招生。济南大学停招了朝鲜语、德语等 9 个本科专业，沈阳航空航天大学在 2024 年暂停了英语等 10 个专业的招生。 这一趋势反映了高等教育优先级的重大转变，受招生下降、就业市场需求变化以及人工智能对语言职业的影响驱动。它影响到成千上万的学生和教师，并标志着中国对语言教育的广泛重新评估。 2018 年至 2022 年间，全国 109 所高校撤销了 28 个外语相关专业，其中日语、英语和朝鲜语是撤销最多的专业。这些削减涵盖本科和研究生层次，并涉及知名院校。

telegram · zaihuapd · Jun 23, 08:32

**背景**: 中国的外语专业因高考分数线下降、人工智能翻译工具的竞争以及就业前景有限而面临兴趣下降。许多学生现在更倾向于将语言技能与商业或法律等其他领域结合，导致向跨学科项目的转变。这一趋势并非中国独有；韩国和其他国家也观察到了类似的下降。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.163.com/dy/article/KOJ0A7UJ0519E3QB.html">m.163.com/dy/article/KOJ0A7UJ0519E3QB.html</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_28451132">多校官宣：外语专业，停招_澎湃号·湃客_澎湃新闻-The Paper</a></li>
<li><a href="https://news.qq.com/rain/a/20240929A05YTL00">多所高校保研结果出炉：小语种本科生跨专业保研是“人才流失”吗？_腾讯新闻</a></li>

</ul>
</details>

**标签**: `#higher education`, `#foreign language`, `#China`, `#academic trends`, `#policy`

---

<a id="item-19"></a>
## [三星发布 UFS 5.0，带宽 10.8 GB/s，面向端侧 AI](https://news.samsung.com/global/samsung-unveils-industrys-fastest-ufs-5-0-solution-for-next-gen-on-device-ai-applications) ⭐️ 7.0/10

三星宣布推出 UFS 5.0，这是业界最快的通用闪存存储解决方案，顺序读取速度高达 10.8 GB/s，顺序写入速度高达 9.5 GB/s，计划于 2026 年第四季度量产。 这一突破使带宽相比 UFS 4.1 提升一倍以上，为旗舰手机、XR 头显和 AI 可穿戴设备中的端侧 AI 应用提供更快的数据加载速度，这对 AI 处理向边缘设备迁移至关重要。 UFS 5.0 基于最新的 JEDEC 嵌入式存储接口标准，提供最高 1 TB 容量，相比三星 UFS 4.1 功耗效率提升超过 40%，封装尺寸缩小 16.7%。

telegram · zaihuapd · Jun 23, 09:17

**背景**: 通用闪存存储（UFS）是一种广泛应用于移动设备的高性能存储标准。端侧 AI 指直接在设备上运行人工智能模型而非云端，需要快速数据访问以实现实时处理。JEDEC 是制定 UFS 规范的标准组织。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.samsung.com/global/samsung-unveils-industrys-fastest-ufs-5-0-solution-for-next-gen-on-device-ai-applications">Samsung Unveils Industry’s Fastest UFS 5.0 Solution for Next-Gen On-Device AI Applications</a></li>
<li><a href="https://semiconductor.samsung.com/estorage/ufs/ufs-5-0/">UFS 5.0 | Universal Flash Storage | Samsung Semiconductor Global</a></li>
<li><a href="https://www.sammobile.com/2026/06/23/samsung-worlds-fastest-ufs-5-0-storage-chip-announced-debut-galaxy-s27/">Samsung unveils UFS 5.0 storage chip, could debut with... - SamMobile</a></li>

</ul>
</details>

**标签**: `#storage`, `#Samsung`, `#UFS`, `#AI`, `#hardware`

---

<a id="item-20"></a>
## [不精准洗牌需 14 次才能随机化一副牌](https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/) ⭐️ 7.0/10

新研究扩展了 1992 年的经典结论——7 次完美鸽尾式洗牌足以随机化一副 52 张牌——表明在现实的不精准洗牌条件下，大约需要 14 次洗牌。 这一发现完善了我们对现实场景中随机化的理解，对概率论、算法设计以及任何依赖随机排列的领域都有影响。 研究人员为每张牌分配二进制条形码，追踪其在洗牌过程中的路径，并识别出残留有序的“冷点”，证明即使是不精准的洗牌也存在截止现象。不过，当前模型仍假设牌是一张张交错落下，而非成沓掉落。

telegram · zaihuapd · Jun 23, 16:04

**背景**: Gilbert–Shannon–Reeds 模型是鸽尾式洗牌的标准数学模型，假设一副牌被分成大致相等的两叠，然后交错合并。截止现象描述了随着洗牌次数增加，从有序到随机的急剧转变。Bayer 和 Diaconis 在 1992 年的经典工作表明，在理想条件下，7 次完美的鸽尾式洗牌足以随机化一副 52 张牌。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/">Seven Perfect Shuffles Randomize a Deck of Cards . | Quanta Magazine</a></li>
<li><a href="https://nadialafreniere.github.io/Snapshot_cutoff_first_submission_english.pdf">Cutoff phenomenon : Surprising behaviour in card shuffling and other...</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#probability`, `#randomization`, `#card shuffling`

---

<a id="item-21"></a>
## [LastPass 因合作伙伴 Klue 遭入侵导致客服数据泄露](https://techcrunch.com/2026/06/23/password-manager-maker-lastpass-says-hackers-stole-customer-support-case-data-during-klue-breach/) ⭐️ 7.0/10

LastPass 披露，其合作伙伴 Klue 遭 Icarus 组织入侵（2026 年 6 月 12 日），导致客户支持案例数据和个人信息被盗。 此事件凸显了第三方集成的连锁风险，尤其对于拥有超过 3300 万用户的密码管理器而言，尽管密码库本身未受影响。 被盗数据包括姓名、电话号码、电子邮件地址、物理地址、支持案例记录和销售相关数据。LastPass 表示其自身基础设施和密码库未被攻破。

telegram · zaihuapd · Jun 24, 00:49

**背景**: LastPass 在 2022 年曾遭遇严重数据泄露，攻击者窃取了加密的密码库，最终导致 2450 万美元的集体诉讼和解。Klue 入侵事件是一次基于 OAuth 的供应链攻击，被攻破的集成凭证使攻击者能够访问多家公司的 Salesforce 数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/22/klue-hack-results-in-data-breach-at-several-cybersecurity-firms/">Klue hack results in data breach at several cybersecurity... | TechCrunch</a></li>
<li><a href="https://cybersecuritynews.com/klue-hack-cybersecurity-companies/">Klue Hack Leads to Data Breach Across Multiple Cybersecurity...</a></li>
<li><a href="https://en.wikipedia.org/wiki/LastPass_2022_data_breach">LastPass 2022 data breach</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#LastPass`, `#password manager`

---