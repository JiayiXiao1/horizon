---
layout: default
title: "Horizon Summary: 2026-07-17 (ZH)"
date: 2026-07-17
lang: zh
---

> From 37 items, 19 important content pieces were selected

---

1. [Firefox 通过 WebAssembly 在另一个浏览器中运行](#item-1) ⭐️ 9.0/10
2. [Linus Torvalds 宣称 Linux 不反 AI](#item-2) ⭐️ 9.0/10
3. [Kimi 发布 2.8 万亿参数开源模型 K3](#item-3) ⭐️ 9.0/10
4. [Thinking Machines Lab 发布开源权重 Inkling 模型](#item-4) ⭐️ 8.0/10
5. [xAI 在隐私争议后开源 Grok Build](#item-5) ⭐️ 8.0/10
6. [Claude web_fetch 工具绕过漏洞导致数据泄露](#item-6) ⭐️ 8.0/10
7. [长鑫存储 2026 年 DRAM 产能将逼近美光](#item-7) ⭐️ 8.0/10
8. [日本购入 2.75 万块英伟达 Rubin 芯片打造机器人 AI](#item-8) ⭐️ 8.0/10
9. [台积电再投千亿美元赴美，Q2 利润飙升 77%](#item-9) ⭐️ 8.0/10
10. [微软 Comic Chat 开源，30 年后重见天日](#item-10) ⭐️ 7.0/10
11. [一加停止在美欧推出新产品](#item-11) ⭐️ 7.0/10
12. [交互式线性代数书籍获社区好评](#item-12) ⭐️ 7.0/10
13. [从 Rust 到 Zig 重写编译器：速度与控制双赢](#item-13) ⭐️ 7.0/10
14. [LLM 批评有理，但我仍在使用](#item-14) ⭐️ 7.0/10
15. [GPT-5.6 Codex 漏洞可删除用户文件](#item-15) ⭐️ 7.0/10
16. [知网将下架以 DeepSeek 为作者的论文](#item-16) ⭐️ 7.0/10
17. [美国 ITC 对 DRAM 设备启动 337 调查](#item-17) ⭐️ 7.0/10
18. [欧盟拟要求安卓向竞争对手 AI 助手开放](#item-18) ⭐️ 7.0/10
19. [1Password 集成 Claude，实现安全 AI 登录](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Firefox 通过 WebAssembly 在另一个浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter 已将完整的 Firefox 浏览器（Gecko 引擎）编译为 WebAssembly，使其能够在另一个浏览器标签页中运行。该项目使用了 AI 辅助开发，借助 Claude Opus 和 Fable，估计花费了 25,000 美元的 AI 代币。 这是一项突破性的技术成就，展示了在另一个浏览器中运行像浏览器这样完整复杂应用的可行性。它为沙盒浏览、跨浏览器测试以及基于 Web 的新型虚拟化开辟了可能性。 所有网络流量都通过 Wisp 协议经 WebSocket 代理到 Puter 的服务器，因为浏览器中的 WebAssembly 代码无法打开原始网络连接。该项目支持端到端加密，通过检查 WebSocket 消息已得到验证。

rss · Simon Willison · Jul 16, 23:34

**背景**: WebAssembly (Wasm) 是一种低级二进制指令格式，能在现代浏览器中以接近原生的速度运行。传统上，浏览器是 Web 应用的运行时，但将浏览器本身编译为 Wasm 会将宿主浏览器转变为类似虚拟机管理程序的环境。Wisp 协议是一种低开销协议，用于通过单个 WebSocket 连接代理多个 TCP/UDP 套接字，在此设置中对网络功能至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/wisp-protocol: Wisp is a low-overhead, easy to implement protocol for proxying multiple TCP/UDP sockets over a single websocket. · GitHub</a></li>
<li><a href="https://developer.puter.com/labs/firefox-wasm/">Firefox in WebAssembly - developer.puter.com</a></li>
<li><a href="https://github.com/HeyPuter/firefox-wasm">HeyPuter/firefox-wasm: Firefox in WebAssembly - GitHub</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论非常热烈，许多评论者对该技术壮举印象深刻。一些人担心代理流量的成本和演示服务器的可扩展性，团队不得不扩展服务器以应对负载。

**标签**: `#WebAssembly`, `#Firefox`, `#browser engineering`, `#AI-assisted development`, `#Wisp protocol`

---

<a id="item-2"></a>
## [Linus Torvalds 宣称 Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 9.0/10

Linux 创始人 Linus Torvalds 在 Linux Media 邮件列表中声明，Linux 不是一个反 AI 的项目，AI 是一个明显有用的工具，并邀请不同意的人 fork 内核或离开。 这位开源关键人物的强力支持标志着 Linux 社区对 AI 立场的重大转变，可能加速 AI 在内核开发中的整合，并影响其他开源项目。 Torvalds 强调 AI 的有用性已毋庸置疑，尽管他承认 AI 还有其他未解决的问题，比如其经济影响。该声明是在 Linux Media 邮件列表中针对内核开发中关于 AI 的持续辩论而发表的。

rss · Simon Willison · Jul 16, 13:26

**背景**: Linux 内核是 Linux 操作系统的核心，由 Linus Torvalds 和全球开发者社区维护。最近，开源社区内部就 AI 在软件开发中的作用展开了辩论，一些项目采取了反 AI 政策。Torvalds 的声明直接回应了这一争议，断言 AI 工具在 Linux 开发中受到欢迎。

**标签**: `#Linux`, `#AI`, `#Open Source`, `#Linus Torvalds`, `#Kernel Development`

---

<a id="item-3"></a>
## [Kimi 发布 2.8 万亿参数开源模型 K3](https://t.me/zaihuapd/42619) ⭐️ 9.0/10

Kimi AI 发布了开源大语言模型 K3，总参数量达 2.8 万亿，采用稀疏混合专家架构，包含 896 个专家，每个 token 激活 16 个专家。该模型支持最高 100 万 token 的上下文，综合性能仅次于 Claude Fable 5 和 GPT-5.6 Sol。 K3 代表了开源 AI 领域的重大突破，性能可与顶级闭源模型媲美，有望让前沿智能更易获取。其创新的架构（包括 Kimi Delta Attention 和 Attention Residuals）可能影响未来模型设计，并减少对密集计算的依赖。 K3 采用 Kimi Delta Attention（KDA）线性注意力机制，通过细粒度门控实现高效长上下文处理，并引入 Attention Residuals 缓解深层 Transformer 中的隐状态稀释问题。模型定价为每百万输入 token 3 美元、每百万输出 token 15 美元，与 Anthropic 的 Sonnet 系列相当。

telegram · zaihuapd · Jul 17, 00:02

**背景**: 大型语言模型通常采用密集架构，每个输入激活所有参数，计算成本高昂。混合专家（MoE）模型通过每个 token 仅激活部分参数来解决这一问题，从而在不按比例增加计算量的情况下扩大总参数量。Kimi Delta Attention 是一种线性注意力变体，其计算量随序列长度线性增长，而非标准注意力的二次增长，因此适合长上下文。Attention Residuals 允许模型有选择地关注较早的层，从而提高训练和推理效率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">Kimi Linear: An Expressive, Efficient Attention Architecture</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出 K3 的定价相对于其他中国模型较高，但如果性能确实能与前沿模型媲美，则定价合理。部分讨论聚焦于中国实验室将 AI 智能商品化的战略意义，另一些用户分享了基准测试结果，显示 K3 优于 Opus 4.8，并与 Sol 和 Fable 竞争。

**标签**: `#AI`, `#large language model`, `#open-source`, `#Kimi`, `#Mixture of Experts`

---

<a id="item-4"></a>
## [Thinking Machines Lab 发布开源权重 Inkling 模型](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，这是一个开放权重的混合专家多模态模型，总参数量 975B（活跃参数 41B），采用 Apache-2.0 许可，在 45 万亿个文本、图像、音频和视频 token 上训练而成。 此次发布增强了美国开放权重生态系统，为中国开源模型提供了有竞争力的替代方案，其 Apache-2.0 许可鼓励广泛采用和定制。 模型卡内容明显稀疏，训练数据文档极少，Thinking Machines Lab 承认 Inkling 并非前沿模型，而是通过其 Tinker 平台进行微调的强大基础模型。更小的 276B（活跃参数 12B）变体 Inkling-Small 已承诺但尚未发布。

rss · Simon Willison · Jul 16, 15:35

**背景**: 混合专家（MoE）模型使用多个专门的子网络（专家）和门控机制，每次输入仅激活部分专家，从而在保持较低推理计算成本的同时实现更大的总参数量。开放权重模型公开训练好的参数，允许用户运行、微调和研究，不同于封闭模型。Apache-2.0 是一种宽松的开源许可，允许自由使用、修改和分发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>

</ul>
</details>

**标签**: `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#AI model release`

---

<a id="item-5"></a>
## [xAI 在隐私争议后开源 Grok Build](https://simonwillison.net/2026/Jul/15/grok-build/#atom-everything) ⭐️ 8.0/10

xAI 在发现其 CLI 工具会上传整个目录（包括 SSH 密钥和密码数据库）到云端后，已将整个 Grok Build 代码库以 Apache 2.0 许可证开源。该公司还删除了所有先前保留的用户数据，并禁用了默认数据保留。 此事件凸显了 AI 驱动的开发者工具中关键的隐私风险，而开源举措是重建信任的重要一步。在宽松许可证下发布 844,530 行 Rust 代码也为开源社区提供了宝贵资源。 Grok Build 代码库包含 844,530 行 Rust 代码，其中仅约 3% 为供应商代码，并包含一个自包含的 Mermaid 图表终端渲染器。该仓库只有一个提交，因此无法看到开发历史。

rss · Simon Willison · Jul 15, 23:59

**背景**: Grok CLI 工具由 xAI 开发，是一个连接到 xAI 的 Grok API 的对话式 AI 命令行界面。Apache 2.0 许可证是一种宽松的开源许可证，允许用户自由使用、修改和分发软件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apache_License">Apache License</a></li>
<li><a href="https://github.com/superagent-ai/grok-cli">GitHub - superagent-ai/grok-cli: An open-source coding agent ...</a></li>

</ul>
</details>

**社区讨论**: 社区对隐私侵犯表达了强烈不满，一名用户报告称在其主目录中运行该工具会上传包括 SSH 密钥和密码管理器数据在内的个人文件。作为回应，Elon Musk 表示所有上传的用户数据将被完全删除，随后 xAI 开源了代码库。

**标签**: `#AI`, `#privacy`, `#open source`, `#security`, `#xAI`

---

<a id="item-6"></a>
## [Claude web_fetch 工具绕过漏洞导致数据泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

研究员 Ayush Paul 发现了一种提示注入攻击，绕过了 Anthropic 在 Claude 的 web_fetch 工具中基于 URL 的保护机制，通过诱骗模型访问一系列攻击者控制的 URL，从而窃取用户的姓名、所在城市和雇主等隐私数据。 该漏洞破坏了 Claude web_fetch 工具的核心安全设计，表明即使采用确定性 URL 限制，仍可通过间接提示注入绕过，对用户隐私和 AI 助手的信任构成严重威胁。 该攻击利用了一个漏洞：web_fetch 可以访问之前获取的页面中嵌入的 URL，从而允许蜜罐站点引导模型通过一系列链接，将数据通过 URL 参数泄露。Anthropic 已内部发现该问题，并通过移除 web_fetch 访问获取内容中链接的能力来修复漏洞。

rss · Simon Willison · Jul 15, 14:21

**背景**: 提示注入攻击利用了大语言模型无法区分可信指令与不可信用户或网页内容的弱点。在“致命三重奏”场景中，拥有私有数据访问权限和网页获取工具的 LLM 可能被网页中嵌入的恶意指令欺骗，从而泄露数据。Anthropic 曾试图通过限制 web_fetch 仅能访问用户明确提供或由配套 web_search 工具返回的 URL 来缓解此问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://docs.claude.com/en/docs/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Docs</a></li>
<li><a href="https://cdn.openai.com/pdf/dd8e7875-e606-42b4-80a1-f824e4e11cf4/prevent-url-data-exfil.pdf">Preventing URL-Based Data Exfiltration in Language-Model Agents Adrian Spânu</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论强调了该攻击的巧妙性以及分层防御的重要性，一些评论者指出，只要 LLM 能够访问外部内容，类似的绕过方式就可能持续存在。其他人则就 Anthropic 因内部已发现而不支付漏洞赏金的决定是否合理展开了辩论。

**标签**: `#AI safety`, `#prompt injection`, `#security vulnerability`, `#Claude`, `#data exfiltration`

---

<a id="item-7"></a>
## [长鑫存储 2026 年 DRAM 产能将逼近美光](https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer) ⭐️ 8.0/10

根据 Citrini Research 的预测，中国长鑫存储有望在 2026 年底达到约 35 万片/月的 DRAM 产能，仅比美光的 37.5 万片/月少 2.5 万片，届时中国可能成为全球第二大 DRAM 生产国。 这一快速产能扩张可能重塑全球内存供应链，减少对韩国和美国供应商的依赖，并有助于在 2030 年预计 25%的全球供应缺口背景下稳定 DRAM 价格。 该预测还包括其他中国企业（如昇维旭、晋华集成和 XMC）的贡献，到 2026 年中国 DRAM 总产能可能达到 60 万片/月（不含三星、SK 海力士在华工厂）。然而，美国的 MATCH 法案可能限制先进浸没式 DUV 光刻设备的出口，构成关键瓶颈。

telegram · zaihuapd · Jul 16, 02:30

**背景**: DRAM（动态随机存取存储器）是一种用于计算机、服务器和消费电子产品的易失性存储器。目前，全球 DRAM 市场由三星、SK 海力士和美光三大厂商主导。中国一直在努力实现半导体自给自足，长鑫存储是其领先的 DRAM 制造商。DUV（深紫外）光刻是芯片电路刻蚀的关键工艺，先进的浸没式 DUV 设备对于在竞争节点上生产 DRAM 至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/dram/cxmt-close-to-matching-microns-memory-capacity-in-2026-research-claims-would-put-china-on-track-to-become-worlds-second-largest-dram-producer">CXMT close to matching Micron's memory capacity in 2026, research claims — would put China on track to become world's second-largest DRAM producer | Tom's Hardware</a></li>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/congress-moves-to-strip-commerce-of-chip-export-discretion-with-the-match-act">Congress moves to strip the DoC of chip-export discretion with the MATCH Act — DUV lithography machines among those targeted in chipmaking tool crackdown | Tom's Hardware</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#semiconductors`, `#China`, `#memory industry`, `#geopolitics`

---

<a id="item-8"></a>
## [日本购入 2.75 万块英伟达 Rubin 芯片打造机器人 AI](https://www.bloomberg.com/news/articles/2026-07-16/japan-to-buy-nvidia-rubin-chips-to-build-sovereign-ai-for-robots) ⭐️ 8.0/10

日本计划购入 27,500 块英伟达下一代 Rubin 芯片，由新成立的 Noetra 公司牵头建设大型数据中心，开发面向机器人的本土基础 AI 模型，并获得政府 3873 亿日元（约 24 亿美元）拨款。 这标志着日本在机器人领域推动主权 AI 的重大政府支持举措，旨在减少对外国技术的依赖，并力争到 2040 年占据全球机器人市场 30%以上的份额。 Noetra 由软银、丰田支持的 Preferred Networks、NEC、本田和索尼等企业参与组建，计划在 2027 年 3 月前发布首个 AI 模型，并在数年内推出机器人专用版本。

telegram · zaihuapd · Jul 16, 10:59

**背景**: 英伟达 Rubin 平台于 2024 年发布，是以天体物理学家 Vera Rubin 命名的下一代 AI 超级芯片架构，包含六款芯片（Vera CPU、Rubin GPU、NVLink 6 交换机等），旨在大幅缩短训练时间并降低推理成本。主权 AI 指国家自主开发和控制 AI 基础设施与模型的能力，以减少对外部势力的依赖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rubin_(microarchitecture)">Rubin (microarchitecture) - Wikipedia</a></li>
<li><a href="https://developer.nvidia.com/blog/inside-the-nvidia-rubin-platform-six-new-chips-one-ai-supercomputer/">Inside the NVIDIA Vera Rubin Platform: Six New Chips, One AI ...</a></li>
<li><a href="https://robotsbeat.com/japan-nvidia-noetra-physical-ai-factory-frontia-rubin-gpus/">Japan and NVIDIA Launch World's First National... | RobotsBeat</a></li>

</ul>
</details>

**标签**: `#AI`, `#Robotics`, `#Nvidia`, `#Japan`, `#Sovereign AI`

---

<a id="item-9"></a>
## [台积电再投千亿美元赴美，Q2 利润飙升 77%](https://www.reuters.com/world/asia-pacific/tsmcs-second-quarter-profit-seen-hitting-record-ai-boom-2026-07-15/) ⭐️ 8.0/10

台积电宣布再向亚利桑那州工厂投资 1000 亿美元，使在美总投资规模达到 2650 亿美元。同时，受 AI 需求驱动，公司公布 2026 年第二季度净利润达 7066 亿新台币（约 220 亿美元），同比增长 77%，创历史新高。 这一巨额投资凸显了台积电在地缘政治紧张局势下对美国芯片制造的承诺，并强调了 AI 热潮持续推动半导体需求。这也标志着全球半导体供应链的重大转变，台积电正在向台湾以外扩张。 台积电将 2026 年资本支出预测上调至 600 亿至 640 亿美元，并预计全年美元营收增长略超 40%。亚利桑那州目前有 8 座工厂在建或规划中，未来可能再增 4 座。

telegram · zaihuapd · Jul 16, 12:29

**背景**: 台积电是全球最大的半导体代工厂，为苹果、英伟达和 AMD 等公司生产芯片。美国政府通过《芯片法案》鼓励芯片制造回流，以减少对台湾的依赖，因为存在地缘政治风险。台积电的亚利桑那项目最初遭遇延迟，第二座工厂推迟至 2027 年投产。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://laoyaoba.com/html/share/news/855650?source=app_android_v2">含泪“走出去” 台 积 电 成立“海外办”意味着什么</a></li>
<li><a href="https://m.elecfans.com/article/2379846.html">台 积 电 ：美国 亚 利 桑 那 州 第二座晶圆 厂 投产时间推迟至2027...</a></li>
<li><a href="https://m.gelonghui.com/p/465904">台 积 电 要赴美建3nm 厂 ，或再投数百亿美元</a></li>

</ul>
</details>

**标签**: `#TSMC`, `#semiconductors`, `#AI`, `#investment`, `#manufacturing`

---

<a id="item-10"></a>
## [微软 Comic Chat 开源，30 年后重见天日](https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/) ⭐️ 7.0/10

2026 年 7 月 16 日，微软将 1990 年代的图形化 IRC 客户端 Comic Chat（后更名为 Microsoft Chat）开源，该软件能将文本对话自动转化为漫画形式。源代码现已托管在 GitHub 上。 此次开源保留了一段早期互联网的趣味历史，也彰显了微软对开源的承诺。同时，它重新唤起了人们对那个充满实验精神的网络时代的怀念——像 Comic Chat 这样的产品曾不断突破创意边界。 Comic Chat 最初于 1996 年随 Internet Explorer 3.0 发布，后来被捆绑在 Windows 98 中。它让世界认识了 Comic Sans 字体，并通过自定义命令扩展了 IRC 协议，用于控制角色外观和表情。

hackernews · jervant · Jul 16, 16:06 · [社区讨论](https://news.ycombinator.com/item?id=48936426)

**背景**: IRC（互联网中继聊天）是一种基于文本的聊天协议，在 1990 年代和 2000 年代初期广泛用于群组通信。Comic Chat 是一个图形化客户端，能自动将 IRC 对话渲染成漫画面板，包含插画角色、对话气泡和表情，使聊天更加有趣和易用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Microsoft_Comic_Chat">Microsoft Comic Chat</a></li>
<li><a href="https://opensource.microsoft.com/blog/2026/07/16/microsoft-comic-chat-is-now-open-source/">Microsoft Comic Chat is now open source</a></li>

</ul>
</details>

**社区讨论**: 社区反响极为积极且充满怀旧情绪。评论者分享了个人故事，例如 Comic Chat 如何启发了一个创业项目，并指出尽管它因扩展 IRC 协议而曾遭诟病，但仍是备受喜爱的互联网历史片段。

**标签**: `#open source`, `#microsoft`, `#irc`, `#retro computing`, `#nostalgia`

---

<a id="item-11"></a>
## [一加停止在美欧推出新产品](https://community.oneplus.com/thread/2170715118587871237) ⭐️ 7.0/10

一加决定停止在欧洲和北美推出新产品，但将继续为现有设备提供软件更新和安全补丁。 这标志着从关键市场的重大撤退，可能影响一加在西方市场的品牌影响力和用户基础。 该决定并不意味着完全停止运营；现有设备仍将获得支持。一加由 OPPO 支持，后者可能继续在这些地区运营。

hackernews · pilililo2 · Jul 16, 10:14 · [社区讨论](https://news.ycombinator.com/item?id=48932539)

**背景**: 一加最初以“不将就”品牌著称，提供高规格、价格实惠、接近原生安卓且解锁引导加载程序的手机。随着时间的推移，它转向更主流的策略，引发了早期发烧友社区的批评。

**社区讨论**: 社区评论表达了失望和怀旧之情，前员工提到 996 工作文化和人员空心化。用户指出，虽然近期一加手机电池续航出色，但公司已失去其黑客友好的精神。

**标签**: `#OnePlus`, `#smartphones`, `#business strategy`, `#market exit`, `#community discussion`

---

<a id="item-12"></a>
## [交互式线性代数书籍获社区好评](https://immersivemath.com/ila/) ⭐️ 7.0/10

一本带有交互式图形的沉浸式线性代数书籍已在线发布，读者可以直接在浏览器中操作 3D 可视化内容。 该资源使抽象的线性代数概念更加直观，有望改善数学教育，并激发其他学科类似交互式教科书的创作。 该书涵盖向量、矩阵和特征值等主题，交互式图形会随用户调整参数实时更新。

hackernews · srean · Jul 16, 15:32 · [社区讨论](https://news.ycombinator.com/item?id=48935951)

**背景**: 线性代数是计算机图形学、机器学习和工程等领域的基础。传统教科书依赖静态图表，可能使空间概念难以理解。交互式图形通过让学习者直观探索关系来弥补这一差距。

**社区讨论**: 评论者表达了强烈的热情，希望统计学、概率论和机器人学也有类似的交互式书籍。有人指出，LLM 现在使创建此类插图更容易，并建议添加“解释此内容”弹出窗口以增强交互性。

**标签**: `#linear algebra`, `#interactive learning`, `#education`, `#mathematics`

---

<a id="item-13"></a>
## [从 Rust 到 Zig 重写编译器：速度与控制双赢](https://rtfeldman.com/rust-to-zig) ⭐️ 7.0/10

Richard Feldman 发表了一篇详细博文，描述将 Roc 编译器从 Rust 重写为 Zig 的进展，指出 Zig 在内存控制、交叉编译和增量构建性能方面的优势是主要动因。 这次重写凸显了 Zig 作为系统编程语言的吸引力日益增强，特别是在编译器开发领域，手动内存管理和快速迭代周期至关重要。同时，它也引发了关于语言设计中安全性与控制力之间权衡的讨论。 博文指出，生成机器码的编译器在二进制修补等任务中常需不安全操作，而 Zig 通过显式分配器控制和 ReleaseSafe 模式下的运行时安全检查来处理。但社区成员质疑 Zig 的运行时检查是否能完全捕获 use-after-free 错误。

hackernews · jorangreef · Jul 16, 11:39 · [社区讨论](https://news.ycombinator.com/item?id=48933149)

**背景**: Rust 和 Zig 都是现代系统编程语言，但在内存安全上采取不同策略：Rust 通过借用检查器在编译时强制安全，而 Zig 赋予程序员完全的手动控制权并辅以可选的运行时检查。编译器是复杂的程序，常需底层内存操作，因此成为检验语言权衡的绝佳案例。Roc 编译器是由同一位作者开发的函数式语言编译器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://piembsystech.com/memory-management-in-zig-programming-language/">Memory Management in Zig Programming Language</a></li>
<li><a href="https://zig.guide/build-system/cross-compilation/">Cross-compilation - zig.guide</a></li>
<li><a href="https://deepwiki.com/ziglang/zig/3.3-incremental-compilation">Incremental Compilation | ziglang/zig | DeepWiki</a></li>

</ul>
</details>

**社区讨论**: 社区评论褒贬不一：Steve Klabnik 认为生成机器码本身并不需要不安全操作，而其他人则称赞 Zig 的增量构建是杀手级特性。一些人担心 Zig 的运行时安全检查可能无法完全防止 use-after-free 漏洞，并质疑 Rust 未来能否在增量构建速度上赶上 Zig。

**标签**: `#Rust`, `#Zig`, `#compilers`, `#memory safety`, `#systems programming`

---

<a id="item-14"></a>
## [LLM 批评有理，但我仍在使用](https://www.theocharis.dev/blog/llm-critics-are-right-i-use-llms-anyway/) ⭐️ 7.0/10

作者承认对 LLM 的合理批评，如潜在的认知萎缩和过度依赖，但认为有意识地使用能提升软件工程中的生产力和思考能力。 这种细致入微的观点很重要，因为它回应了关于 AI 工具对人类技能长期影响的日益激烈的辩论，影响开发者及知识工作者如何将 LLM 融入工作流程。 作者分享了一个月内花费近 1 万美元购买 token 的个人经历，凸显了重度使用 LLM 的高昂成本，而社区评论指出 LLM 在开源项目中生成了低质量的 PR。

hackernews · JeremyTheo · Jul 16, 11:59 · [社区讨论](https://news.ycombinator.com/item?id=48933310)

**背景**: LLM（大型语言模型）如 GPT-4 是能生成类人文本的 AI 系统，广泛应用于软件工程的代码生成、调试和文档编写。批评者警告过度依赖可能导致技能萎缩、批判性思维减弱以及高能耗带来的环境成本。

**社区讨论**: 社区评论表达了对认知萎缩的担忧，将 LLM 成瘾与智能手机成瘾相比较，并指出高 token 成本和开源项目中低质量 PR 等实际问题，有人考虑屏蔽 AI 生成的贡献。

**标签**: `#LLM`, `#software engineering`, `#productivity`, `#critical thinking`, `#AI tools`

---

<a id="item-15"></a>
## [GPT-5.6 Codex 漏洞可删除用户文件](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 7.0/10

GPT-5.6 的 Codex 存在一个漏洞：在启用完全访问模式且未使用沙箱保护时，模型可能错误地删除 $HOME 目录而非临时目录，从而导致用户文件被意外删除。 该漏洞凸显了 AI 编程代理在拥有无限制文件系统访问权限时的关键安全风险，并强调了使用沙箱保护和自动审查功能以防止数据丢失的必要性。 该漏洞发生在启用完全访问模式、关闭沙箱保护和自动审查的情况下；模型尝试通过覆盖 $HOME 环境变量来设置临时目录，但错误地删除了 $HOME 目录。

rss · Simon Willison · Jul 16, 17:45

**背景**: 像 Codex 这样的 AI 编程代理可以自主读取、写入和执行用户机器上的代码。完全访问模式赋予代理广泛的权限，而沙箱保护则将其操作限制在安全环境中。$HOME 环境变量通常指向用户的主目录，其中包含个人文件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://explainx.ai/blog/openai-codex-gpt-5-6-home-deletion-full-access-july-2026">Codex GPT - 5 . 6 $HOME Deletion — Full Access | explainx.ai</a></li>
<li><a href="https://amux.io/guides/ai-agent-sandboxing/">AI Agent Sandboxing in 2026: Docker, E2B, Firecracker... — amux</a></li>
<li><a href="https://deepnoodle.ai/blog/sandboxing-ai-coding-agents">The Deep Noodle Blog | Sandboxing AI Coding Agents</a></li>

</ul>
</details>

**标签**: `#codex`, `#ai-safety`, `#gpt-5.6`, `#bug`, `#coding-agents`

---

<a id="item-16"></a>
## [知网将下架以 DeepSeek 为作者的论文](https://www.zaobao.com.sg/news/china/story20260716-9371836) ⭐️ 7.0/10

中国最大的学术期刊平台知网宣布，将下架将 DeepSeek、Gemini 等 AI 工具列为作者的论文，并明确不接受 AI 工具作为论文署名作者。 这一政策为中国学术诚信树立了明确先例，应对了学术出版中日益增长的 AI 生成内容趋势，并厘清了法律和伦理责任。 知网表示，AI 不具备民事主体资格，无法承担学术核查、整改和追责等责任。在研究或写作中使用 AI 的作者应在研究方法或致谢中加以说明。

telegram · zaihuapd · Jul 16, 07:45

**背景**: DeepSeek 是一家中国 AI 公司，开发了如 DeepSeek-V3（671B 参数）等大型语言模型。近期，一些期刊开始将 AI 工具列为合著者，引发了关于作者责任和学术伦理的担忧。知网的举措符合中国现行法律，包括《民法典》和《著作权法》，这些法律要求作者必须是自然人或法人实体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://finance.sina.com.cn/wm/2026-07-15/doc-inihxaeu7895922.shtml">知网声明：AI署名作者的论文一律下架_新浪财经_新浪网</a></li>
<li><a href="https://finance.sina.cn/2026-07-15/detail-inihxaeu7895922.d.html?vt=4&cid=76729&node_id=76729">知网声明：AI署名作者的论文一律下架|DeepSeek|科研|人工智能|学术|红线_手机新浪网</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2026-07-15/doc-inihxaey1127935.shtml">严禁AI当论文作者！知网：对将DeepSeek等署名的论文已做下架处理_新浪科技_新浪网</a></li>

</ul>
</details>

**标签**: `#AI ethics`, `#academic publishing`, `#China`, `#DeepSeek`, `#authorship policy`

---

<a id="item-17"></a>
## [美国 ITC 对 DRAM 设备启动 337 调查](https://www.cls.cn/detail/2428105) ⭐️ 7.0/10

2026 年 7 月 15 日，美国国际贸易委员会投票决定对特定 DRAM 设备及其下游产品启动 337 调查（调查编码 337-TA-1511），该调查基于 Netlist 提出的专利侵权投诉。被调查方包括三星、谷歌、英伟达、博通和超微电脑等。 这项调查可能扰乱 AI 服务器和数据中心使用的 DDR5 DIMM 及 HBM 供应，进而推高云服务和 AI 硬件的成本。涉案公司均为科技巨头，凸显了半导体和 AI 行业面临的高风险。 投诉具体涉及 DDR5 DIMM、高带宽内存（HBM），以及使用这些组件的服务器、计算和存储系统。Netlist 是一家规模较小的半导体公司，与谷歌等公司存在长期专利纠纷。

telegram · zaihuapd · Jul 16, 08:34

**背景**: 《1930 年关税法》第 337 条授权美国国际贸易委员会调查进口贸易中的不公平行为，包括专利侵权。若认定违规，委员会可发布排除令，禁止侵权产品进入美国市场。DRAM 是一种为处理器临时存储数据的存储芯片，而 HBM 是其高带宽变体，常用于 AI 加速器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.usitc.gov/press_room/us337.htm">Understanding Investigations Of Intellectual Property Infringement And Other Unfair Practices In Import Trade (Section 337) | United States International Trade Commission</a></li>
<li><a href="https://www.reuters.com/world/asia-pacific/us-probes-samsung-alleged-infringement-netlists-memory-chip-patents-2026-07-16/">US probes Samsung for alleged infringement of Netlist's ...</a></li>
<li><a href="https://www.linkedin.com/pulse/netlist-google-patent-war-16-year-odyssey-over-912-billions-wallach-vpt2e">The Netlist (NLST) -Google Patent War: A 16-Year ... - LinkedIn</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#337 Investigation`, `#Patent Infringement`, `#AI Hardware`, `#Supply Chain`

---

<a id="item-18"></a>
## [欧盟拟要求安卓向竞争对手 AI 助手开放](https://t.me/zaihuapd/42615) ⭐️ 7.0/10

欧盟正在根据《数字市场法案》起草指导方针，要求谷歌向 ChatGPT、Claude 等竞争对手的 AI 助手提供与自家 Gemini 助手相同的安卓系统级访问权限。 此举可能通过降低第三方服务在安卓上的门槛来重塑 AI 助手市场的竞争格局，增加用户选择，但也引发了谷歌对安全和隐私的担忧。 相关要求仍处于草案阶段，发布时间可能推迟；谷歌担心这种开放可能影响用户安全和隐私。

telegram · zaihuapd · Jul 16, 13:19

**背景**: 《数字市场法案》（DMA）是欧盟旨在遏制大型在线平台反竞争行为的法规。安卓是全球最流行的移动操作系统，谷歌的 Gemini AI 助手享有锁屏交互、应用集成等系统功能的特权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/eu-google-android-ai-search-data-digital-markets-act">EU forces Google to open Android under Digital Markets Act</a></li>
<li><a href="https://www.linkedin.com/posts/africa-is-home-global_the-european-union-is-pressing-google-to-activity-7455124646502236160-dgv3">EU Pressures Google to Open Android to Rival AI Assistants | LinkedIn</a></li>
<li><a href="https://au.news.yahoo.com/eu-tells-google-external-ai-154157242.html">The EU tells Google to give external AI assistants the same access to...</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#antitrust`, `#Google`

---

<a id="item-19"></a>
## [1Password 集成 Claude，实现安全 AI 登录](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 7.0/10

1Password 推出了与 Claude 的 Mac 端集成，允许 AI 代理代表用户登录网站，而密码和二次验证码不会进入 Claude 的上下文、记忆或 Anthropic 的系统。 该集成解决了 AI 代理使用中的一个关键安全问题，即凭证不进入 AI 上下文，通过用户审批和会话限权实现自动登录，可能为安全的 AI 与密码管理器交互树立新标准。 凭证通过安全通道直接注入目标网页，用户需通过生物识别逐条审批登录请求；若自动填充提交失败，已填内容会被立即擦除。该功能面向 Mac 的商业、家庭及个人版用户，需同时安装 1Password 与 Claude 的桌面及浏览器扩展。

telegram · zaihuapd · Jul 16, 15:54

**背景**: 像 1Password 这样的密码管理器可以安全存储凭证并自动填充登录表单，但通常需要用户手动操作。像 Claude 这样的 AI 代理可以自动化任务，但如果访问明文密码则存在风险。该集成利用 1Password 的安全凭证注入和生物识别审批，将自动化与安全性结合起来。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.1password.dev/cli/reference/commands/inject">inject - 1Password Developer</a></li>
<li><a href="https://1password.com/blog/securing-mcp-servers-with-1password-stop-credential-exposure-in-your-agent">Securing MCP servers with 1Password: Stop credential exposure ...</a></li>
<li><a href="https://support.claude.com/en/articles/10065433-install-claude-desktop">Install Claude Desktop | Claude Help Center</a></li>

</ul>
</details>

**标签**: `#password management`, `#AI integration`, `#security`, `#Claude`, `#1Password`

---