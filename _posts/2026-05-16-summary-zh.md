---
layout: default
title: "Horizon Summary: 2026-05-16 (ZH)"
date: 2026-05-16
lang: zh
---

> From 38 items, 17 important content pieces were selected

---

1. [Zulip 转型为非营利基金会](#item-1) ⭐️ 9.0/10
2. [Pixel 10 零点击漏洞链披露](#item-2) ⭐️ 9.0/10
3. [首个公开的 M5 macOS 内核漏洞利用在 5 天内完成](#item-3) ⭐️ 9.0/10
4. [vLLM v0.21.0：破坏性变更、KV 卸载、推测解码](#item-4) ⭐️ 8.0/10
5. [Mitchell Hashimoto 警告企业陷入“AI 精神病”](#item-5) ⭐️ 8.0/10
6. [美国司法部要求苹果和谷歌披露 10 万多名应用用户信息](#item-6) ⭐️ 8.0/10
7. [ABC 新闻移除所有 FiveThirtyEight 文章](#item-7) ⭐️ 8.0/10
8. [OCaml 上太空：OxCaml 栈注解大幅降低 GC 延迟](#item-8) ⭐️ 8.0/10
9. [arXiv 对未核查 LLM 内容实施一年禁投](#item-9) ⭐️ 8.0/10
10. [特朗普与习近平讨论 AI 护栏及英伟达 H200 芯片](#item-10) ⭐️ 8.0/10
11. [加州法案要求停服游戏提供补丁或退款](#item-11) ⭐️ 7.0/10
12. [Radicle：基于 Git 的去中心化代码协作平台](#item-12) ⭐️ 7.0/10
13. [ChatGPT Android 版拆解发现 Codex 远程桌面功能](#item-13) ⭐️ 7.0/10
14. [中国与波音磋商多达 500 架 737 MAX 订单](#item-14) ⭐️ 7.0/10
15. [加州集体诉讼指控 OpenAI 向 Meta 和 Google 分享用户数据](#item-15) ⭐️ 7.0/10
16. [支付宝回应支付功能关闭后仍被扣款 184 万元捐赠](#item-16) ⭐️ 7.0/10
17. [苹果与 OpenAI 合作出现裂痕，OpenAI 考虑法律行动](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Zulip 转型为非营利基金会](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 9.0/10

Zulip 核心团队（包括创始人 Tim Abbott）将离职加入 Anthropic，公司被捐赠给新成立的独立非营利组织 Zulip 基金会。 这一治理转型确保了 Zulip 的长期独立性和可信度，回应了社区对商业压力和数据隐私的担忧，并为开源可持续性树立了先例。 公告于周五下午发布，一些社区成员指出这是敏感新闻的典型发布时间。此举发生在 Bun 被风投公司收购后不久，引发了对比但存在关键差异。

hackernews · boramalper · May 15, 18:37 · [社区讨论](https://news.ycombinator.com/item?id=48152168)

**背景**: Zulip 是一个开源团队聊天平台，以其独特的基于主题的线程功能而闻名，结合了电子邮件和聊天的优点。它创建于 2012 年，是 Slack 的热门替代品。Anthropic 是一家由前 OpenAI 研究人员创立的 AI 安全公司，以开发 Claude 语言模型而闻名。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zulip">Zulip - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://zulip.com/">Zulip — organized team chat</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：许多人对核心团队的离开感到难过，但对基金会的潜力感到兴奋。一些人将其与 Bun 的收购相提并论，但另一些人认为这不同，因为 Zulip 被捐赠给了非营利组织。周五下午的发布时间引发了质疑。

**标签**: `#open source`, `#nonprofit`, `#governance`, `#Zulip`, `#community`

---

<a id="item-2"></a>
## [Pixel 10 零点击漏洞链披露](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 9.0/10

Google Project Zero 披露了针对 Pixel 10 的完整零点击漏洞链，展示了从 Dolby 音频解码漏洞到内核控制的远程代码执行。 该漏洞链凸显了 AI 驱动的消息分析带来的攻击面扩大（在用户交互前解码媒体），并强调了对这类功能进行严格安全审查的必要性。 该链利用了 CVE-2025-54957（一个影响所有 Android 设备、直至 2026 年 1 月才修补的 Dolby 音频漏洞）以及 Pixel 10 VPU 中的一个视频驱动漏洞来实现内核提权。

hackernews · happyhardcore · May 15, 13:39 · [社区讨论](https://news.ycombinator.com/item?id=48148460)

**背景**: 零点击漏洞无需用户交互，因此极其危险。现代手机的 AI 功能通常会预处理消息（例如解码音频）以实现搜索和分析，无意中扩大了攻击面。Project Zero 是谷歌的精英安全团队，负责发现并披露关键漏洞。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://projectzero.google/2026/05/pixel-10-exploit.html">A 0-click exploit chain for the Pixel 10: When a Door Closes ...</a></li>
<li><a href="https://cyberpress.org/zero-click-exploit-chain-for-pixel-10/">Google Project Zero Reveals Zero-Click Exploit Chain for Pixel 10</a></li>
<li><a href="https://gbhackers.com/pixel-10-zero-click-exploit-chain/">Google Project Zero Details Pixel 10 Zero-Click Exploit Chain</a></li>

</ul>
</details>

**社区讨论**: 评论者对 AI 功能扩大攻击面表示担忧，有人指出这是重蹈覆辙。其他人讨论了厂商的响应时间，对谷歌在 90 天内修补表示赞赏，但担心其他 Android OEM。还有人质疑近期为何缺少 iPhone 越狱。

**标签**: `#security`, `#exploit`, `#mobile`, `#Android`, `#0-click`

---

<a id="item-3"></a>
## [首个公开的 M5 macOS 内核漏洞利用在 5 天内完成](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif 与 Mythos Preview 合作，在短短五天内创建了首个公开的 Apple M5 macOS 内核内存破坏漏洞利用，绕过了 Apple 的 MIE 硬件保护。 该漏洞利用表明，即使是最先进的 Apple MIE 内存保护，在 AI 辅助下也能被迅速绕过，凸显了网络安全格局的重大转变。 该利用链针对 M5 硬件上的 macOS 26.4.1，利用两个漏洞和正常系统调用，从非特权用户提升至 root shell，完整的 55 页技术报告将在 Apple 修复后发布。

telegram · zaihuapd · May 15, 02:15

**背景**: Apple M5 芯片配备了内存完整性强制（MIE），这是一种基于硬件和软件的内存安全系统，使用 ARM 的增强内存标记扩展（EMTE）。Apple 花费五年时间开发 MIE，以大幅增加内存破坏漏洞利用的难度。Mythos Preview 是 Anthropic 最先进的边界 AI 模型，专为网络安全研究设计。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://security.apple.com/blog/memory-integrity-enforcement/">Memory Integrity Enforcement: A complete vision for memory safety in Apple devices - Apple Security Research</a></li>

</ul>
</details>

**标签**: `#Apple M5`, `#kernel exploit`, `#macOS security`, `#AI-assisted hacking`, `#MIE bypass`

---

<a id="item-4"></a>
## [vLLM v0.21.0：破坏性变更、KV 卸载、推测解码](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 弃用了 transformers v4，要求 C++20，将 KV 卸载与混合内存分配器集成，增加了带有思考预算的推测解码，并为 Blackwell GPU 引入了 TOKENSPEED_MLA 后端。 此版本强制迁移到 transformers v5 和现代 C++ 标准，同时提高了推理模型的内存效率和推测解码能力，对大型语言模型的开发者和用户产生重大影响。 KV 卸载子系统现在使用 HMA，支持滑动窗口和多连接器功能。推测解码尊重推理/思考预算，新的 MLA 后端针对 Blackwell GPU 上的 DeepSeek-R1/Kimi-K25。

github · khluu · May 15, 08:44

**背景**: vLLM 是一个高吞吐量、内存高效的大型语言模型推理引擎。KV 缓存卸载将键值缓存从 GPU 移动到 CPU 内存，以减轻 GPU 内存压力。推测解码使用草稿模型预测 token，由目标模型验证，从而在不改变输出分布的情况下加速推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/issues/11382">[RFC]: Hybrid Memory Allocator · Issue #11382 · vllm -project/ vllm</a></li>
<li><a href="https://github.com/lightseekorg/tokenspeed/tree/main">GitHub - lightseekorg/tokenspeed: TokenSpeed is a speed-of ...</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#transformers`, `#speculative decoding`, `#GPU`

---

<a id="item-5"></a>
## [Mitchell Hashimoto 警告企业陷入“AI 精神病”](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Vagrant 和 Terraform 的创建者 Mitchell Hashimoto 在社交媒体上警告，许多公司正因盲目信任 AI 生成的代码和决策而陷入“AI 精神病”，导致系统不稳定和不可持续的做法。 这一批评凸显了软件行业中日益增长的风险：在没有适当监督的情况下过度依赖 AI 可能会降低代码质量和系统可靠性，从而造成长期的技术债务和运营危机。 Hashimoto 的帖子引发了 288 条评论的讨论，有人认为只要人类验证输出，使用 AI 生成代码是可以的，而另一些人则警告纯 AI 编写的系统可能变得难以理解且不稳定。

hackernews · reasonableklout · May 15, 20:26 · [社区讨论](https://news.ycombinator.com/item?id=48153379)

**背景**: “AI 精神病”最初指的是一种心理健康现象，即个体因与聊天机器人互动而出现精神病。在此语境中，Hashimoto 用这个比喻来描述那些不加批判地信任 AI 输出、导致糟糕工程决策的公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chatbot_psychosis">Chatbot psychosis - Wikipedia</a></li>
<li><a href="https://itsfoss.com/news/mitchell-hashimoto-vouch/">Mitchell Hashimoto Launches 'Vouch' to Fight AI Slop in Open Source Ecosystem</a></li>
<li><a href="https://newsletter.pragmaticengineer.com/p/mitchell-hashimoto">Mitchell Hashimoto’s new way of writing code</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意 Hashimoto 的观点，分享了 AI 生成代码导致问题的例子。一些人指出，AI 救援咨询可能成为一种新的高价值服务，而另一些人则指出，真正的问题是将决策外包给 AI，而不是将 AI 作为工具使用。

**标签**: `#AI`, `#software engineering`, `#AI risks`, `#code quality`, `#industry critique`

---

<a id="item-6"></a>
## [美国司法部要求苹果和谷歌披露 10 万多名应用用户信息](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/) ⭐️ 8.0/10

美国司法部要求苹果、谷歌和亚马逊提供超过 10 万名下载了 EZ Lynk 的 Auto Agent 应用的用户身份、地址和购买历史，作为排放打击行动的一部分。 此案为政府对应用商店用户的监控树立了重要先例，引发了关于权力越界和应用分发中心化的严重隐私和法律担忧。 EZ Lynk 否认其应用主要用于排放作弊，声称它还可用于性能监控和软件升级。司法部的请求涉及至少 10 万名用户，使持续多年的法律斗争升级。

hackernews · tencentshill · May 15, 17:28 · [社区讨论](https://news.ycombinator.com/item?id=48151383)

**背景**: EZ Lynk 的 Auto Agent 应用允许用户修改车辆发动机控制单元（ECU），可能禁用排放控制系统。《清洁空气法》禁止篡改排放系统，司法部正在调查此类工具的广泛使用。苹果和谷歌等应用商店作为集中分发点，成为法律要求的对象。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/">U.S. DOJ demands Apple and Google unmask over 100,000 users ...</a></li>
<li><a href="https://9to5mac.com/2026/05/15/doj-reportedly-demands-apple-and-google-identify-over-100000-users-of-car-app/">DOJ reportedly demands Apple and Google identify over 100,000 ...</a></li>
<li><a href="https://www.forbes.com/sites/thomasbrewster/2026/05/14/government-demands-apple-and-google-identify-over-100000-users-of-car-app/">The DOJ Is Demanding Apple And Google Identify Over 100,000 ...</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：一些人认为该应用用于非法排放篡改，用户应受审查；另一些人担心这为更广泛的监控（如针对禁用 GPS 追踪的汽车改装）开创先例。多位用户强调集中式应用分发的风险，并建议使用 F-Droid 等匿名替代方案。

**标签**: `#privacy`, `#legal`, `#app stores`, `#surveillance`, `#automotive`

---

<a id="item-7"></a>
## [ABC 新闻移除所有 FiveThirtyEight 文章](https://twitter.com/baseballot/status/2055309076209492208) ⭐️ 8.0/10

ABC 新闻已移除 FiveThirtyEight 的所有文章，实际上将该数据新闻品牌的整个档案从网络上删除。 此举抹去了大量数据驱动新闻和可视化内容，可能损害公众获取有价值分析的途径，并引发对品牌管理不善和知识产权纠纷的担忧。 FiveThirtyEight 创始人 Nate Silver 声称 ABC 拒绝将 IP 卖回给他，理由是他批评了他们的品牌管理。移除内容包括备受赞誉的关于枪支死亡、p-hacking 和肠道微生物组的交互式可视化作品。

hackernews · cmsparks · May 15, 19:07 · [社区讨论](https://news.ycombinator.com/item?id=48152553)

**背景**: FiveThirtyEight 是由 Nate Silver 于 2008 年创立的数据新闻网站，以对政治、体育和科学的统计分析而闻名。ABC 新闻于 2013 年收购该品牌，但在裁员和选举年之外盈利能力下降后，该网站逐渐被边缘化。

**社区讨论**: 社区评论对高质量可视化内容的丢失表示遗憾，并批评 ABC 的管理。一些人猜测 Nate Silver 可能低价回购该品牌，如果他成功，将使 ABC 难堪。

**标签**: `#data journalism`, `#media`, `#FiveThirtyEight`, `#ABC News`, `#content removal`

---

<a id="item-8"></a>
## [OCaml 上太空：OxCaml 栈注解大幅降低 GC 延迟](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 8.0/10

一篇博客文章披露，OCaml 被用于卫星载荷软件，而 OxCaml 编译器的 exclave 栈注解显著降低了垃圾回收压力和延迟，将每数据包的 p99.9 延迟从 29 纳秒降至 9 纳秒，并在处理 2500 万个数据包的过程中完全消除了次要 GC。 这表明，通过使用先进的编译器技术来控制内存分配，像 OCaml 这样的高级垃圾收集语言可以适用于实时、资源受限的环境（如太空）。这为传统上由 C/C++ 主导的领域带来了更安全、更高效的系统编程可能性。 性能提升来自 OxCaml 的 exclave 栈注解，它允许开发者指定某些值应在栈上而非堆上分配，从而减少 GC 压力。卫星载荷软件还使用了 SystemD 服务、DBus 以及 CCSDS 到 DBus 的桥接，并对数据采用对称密钥加密。

hackernews · yminsky · May 15, 10:55 · [社区讨论](https://news.ycombinator.com/item?id=48147058)

**背景**: OCaml 是一种通用高级编程语言，带有自动管理内存的垃圾回收器。在低延迟或实时系统中，GC 暂停可能成为问题。OxCaml 是 OCaml 的一个性能优化分支，引入了栈分配注解，使开发者能够为关键路径绕过 GC，类似于 Rust 的所有权机制，但采用可选用的实用主义方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://oxcaml.org/documentation/stack-allocation/reference/">OxCaml | Stack allocation | Reference</a></li>
<li><a href="https://github.com/oxcaml/oxcaml">GitHub - oxcaml/oxcaml: OCaml - Oxidized! · GitHub</a></li>
<li><a href="https://www.dra27.uk/blog/platform/2025/05/07/oxcaml-toes.html">Dipping toes into OxCaml | Notes from the Windows corner</a></li>

</ul>
</details>

**社区讨论**: 社区成员分享了第一手经验：一位评论者指出他们可能是最早在 2016 年将 OCaml 送上太空的人（GHGSat-D）。另一位强调，关键优势在于默认拥有 GC，同时能通过栈注解减少堆分配。一些人讨论了为低延迟场景改造 GC 语言的难度，而另一些人则批评 CCSDS 重新发明轮子。

**标签**: `#OCaml`, `#space`, `#garbage collection`, `#systems programming`, `#low-latency`

---

<a id="item-9"></a>
## [arXiv 对未核查 LLM 内容实施一年禁投](https://x.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv 宣布一项政策，对提交含有未核查 LLM 生成内容（如幻觉引用或占位数据）的论文作者实施一年禁投。该处罚适用于那些明显显示未经验证 AI 输出的投稿。 该政策直接解决了 LLM 生成内容日益破坏预印本库学术诚信的问题。它为其他平台树立了先例，并强化了作者无论内容如何生成都应对投稿负全责的原则。 该禁令适用于幻觉引用、LLM 元注释以及诸如“表格数据仅为示例，请替换为真实实验数据”等占位数据。禁投结束后，作者需先让论文被可信的同行评审会议或期刊接收，才能重新提交到 arXiv。

telegram · zaihuapd · May 15, 04:30

**背景**: arXiv 是一个广泛使用的开放获取预印本库，研究人员在同行评审前在此分享论文。近期，人们越来越担心作者使用大型语言模型（LLM）生成内容而未进行适当核查，导致出现虚构引用和无意义数据。此次政策更新旨在通过追究作者责任来维护该库的诚信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://arxiv.org/">arXiv .org e- Print archive</a></li>

</ul>
</details>

**标签**: `#arXiv`, `#LLM`, `#academic integrity`, `#policy`, `#AI ethics`

---

<a id="item-10"></a>
## [特朗普与习近平讨论 AI 护栏及英伟达 H200 芯片](https://www.bloomberg.com/news/articles/2026-05-15/trump-says-he-discussed-ai-guardrails-nvidia-s-chips-with-xi) ⭐️ 8.0/10

美国总统特朗普在访华期间与习近平主席讨论了 AI 护栏及英伟达 H200 芯片出口问题，并指出尽管美国已批准，但中国选择不购买 H200。 此次高层讨论凸显了围绕 AI 芯片供应链的地缘政治紧张局势，对全球 AI 发展和美中科技竞争具有重要影响。 美国已允许英伟达向中国客户供应 H200，但北京尚未批准采购，迄今无一交付。中国此前曾拒绝进口性能较低的 H20 芯片。

telegram · zaihuapd · May 15, 15:13

**背景**: AI 护栏是确保 AI 系统负责任地运行并在规定边界内的安全机制。英伟达 H200 是一款面向生成式 AI 和高性能计算工作负载的高端 GPU。讨论还涉及 Anthropic 的 Mythos 模型引发的全球网络安全担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-guardrails">What are AI guardrails? - IBM</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H 200 GPU | NVIDIA</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms - The New York Times</a></li>

</ul>
</details>

**标签**: `#AI`, `#US-China`, `#semiconductors`, `#geopolitics`, `#Nvidia`

---

<a id="item-11"></a>
## [加州法案要求停服游戏提供补丁或退款](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/) ⭐️ 7.0/10

加州一项法案提出，当游戏公司关闭服务器时，必须发布补丁使在线游戏可离线运行，或提供退款；关键委员会投票即将举行。 该立法可能为游戏数字保存和消费者权益开创先例，迫使发行商改变处理停服游戏的方式，影响数百万玩家。 该法案豁免纯订阅制游戏，可能促使发行商转向订阅模式以规避合规要求。同时要求服务器关闭前提前 60 天通知。

hackernews · Lihh27 · May 15, 19:48 · [社区讨论](https://news.ycombinator.com/item?id=48152994)

**背景**: 许多在线游戏在服务器关闭后变得无法游玩，即使玩家已预先购买，因为它们依赖远程验证或多人在线基础设施。消费者权益组织如“Stop Killing Games”一直推动立法要求提供离线模式或退款，以保护数字所有权。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stopkillinggames.com/">Stop Killing Games — They Kill Games . We Fight Back.</a></li>
<li><a href="https://gaminghq.eu/2026/03/04/law-offline-mode-digital-games-preservation/">Growing Calls for Laws Requiring Offline Versions of Purchased Games</a></li>

</ul>
</details>

**社区讨论**: 评论者意见分歧：有人支持开源服务器代码让社区自建服务器，也有人警告法案可能增加开发者的成本和风险，可能加速向订阅制转型，或使发行商对推出在线游戏更加谨慎。

**标签**: `#gaming`, `#legislation`, `#digital preservation`, `#online services`, `#consumer protection`

---

<a id="item-12"></a>
## [Radicle：基于 Git 的去中心化代码协作平台](https://radicle.dev/) ⭐️ 7.0/10

Radicle 是一个基于 Git 的开源、点对点代码协作平台，旨在成为 GitHub 等中心化代码托管平台的去中心化替代方案。它支持公共和私有仓库，私有仓库仅对授权节点可见。 Radicle 解决了开发者社区日益关注的抗审查和数据自主控制问题。其本地优先、点对点的设计可能重塑开发者协作方式，减少对中心化服务的依赖。 Radicle 的私有仓库在静态时未加密，而是依赖选择性复制，因此对网络不可见，但可能因漏洞或配置错误而泄露。该项目使用自定义许可证（非 AGPL），有人认为这可能允许 SaaS 公司采用并扩展该平台。

hackernews · KolmogorovComp · May 15, 12:07 · [社区讨论](https://news.ycombinator.com/item?id=48147603)

**背景**: 传统的代码托管平台如 GitHub 和 GitLab 是中心化的，意味着单一实体控制访问并可能施加审查。Radicle 使用点对点网络，每个用户保留对其数据和交互的控制，通过加密签名确保真实性。这种方法是去中心化基础设施更广泛运动的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://radicle.dev/">Radicle: the sovereign forge</a></li>
<li><a href="https://radicle.dev/guides/protocol">Radicle Protocol Guide</a></li>
<li><a href="https://radicle.dev/guides/user">The Radicle forge is an open source, peer-to-peer code collaboration...</a></li>

</ul>
</details>

**社区讨论**: 评论者担心私有仓库的安全性，指出缺乏静态加密使其容易意外泄露。还有人批评非 AGPL 许可证，担心它可能使 SaaS 公司能够采用并扩展 Radicle。一些用户则称赞其本地优先设计，并认为它对代理工作流很有用。

**标签**: `#decentralization`, `#git`, `#code forge`, `#open source`, `#peer-to-peer`

---

<a id="item-13"></a>
## [ChatGPT Android 版拆解发现 Codex 远程桌面功能](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

对 ChatGPT Android 版 1.2026.125 的 APK 拆解发现，OpenAI 正在为 Codex 开发手机远程桌面控制功能，用户可通过手机查找和重连远程会话。 该功能将使开发者能够通过移动设备远程管理 Codex 编码会话，大幅提升工作流程的灵活性和生产力。 该功能仍在开发中，尚无可用预览，正式上线时间也未公布。用户需要在手机和桌面端登录同一账号。

telegram · zaihuapd · May 14, 21:48

**背景**: Codex 是 OpenAI 推出的一套 AI 驱动的编码代理，可自动化软件工程任务。近期 OpenAI 已将 Codex 引入 ChatGPT 移动应用，此次拆解表明其正在进一步集成远程桌面功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/work-with-codex-from-anywhere/">Work with Codex from anywhere | OpenAI</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pjcXUtTUVSSEx2bW8yTG4wMUh5Z0FQAQ?hl=en-NG&gl=NG&ceid=NG:en">Google News - OpenAI adds Codex coding tool to ChatGPT mobile...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#remote desktop`, `#Android`

---

<a id="item-14"></a>
## [中国与波音磋商多达 500 架 737 MAX 订单](https://t.me/zaihuapd/41389) ⭐️ 7.0/10

中国正与波音磋商采购多达 500 架 737 MAX 飞机，这将是近十年来中国首次向波音下达重大订单。该交易预计将在本月底至下月初特朗普总统访华期间公布。 这一潜在订单标志着中美贸易紧张局势的缓和，可能显著增加波音的订单积压，尤其是在 737 MAX 经历波折之后。这也凸显了中国日益增长的航空市场及其将飞机采购作为外交工具的战略运用。 该交易包括多达 500 架 737 MAX 飞机，另外还洽谈了约 100 架 787 和 777X 宽体机，可能稍后单独宣布。协议尚未最终敲定，宣布方式以及是否形成具有约束力的正式承诺仍在协商中。

telegram · zaihuapd · May 15, 01:09

**背景**: 波音 737 MAX 是一款窄体客机系列，在 2019 年 3 月至 2020 年 11 月期间因两起与 MCAS 系统相关的致命坠机事故而在全球停飞。中国是首个停飞 MAX 的国家，并迟迟未批准其复飞，中国航空公司直到 2024 年初才恢复 MAX 运营。777X 是一款具有折叠翼尖的长程宽体喷气机，目前处于飞行测试阶段，预计 2027 年投入运营。787 Dreamliner 是一款复合材料结构宽体飞机，于 2011 年投入运营。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_777X">Boeing 777X - Wikipedia Images 777X - The Boeing Company Confirmed: Boeing 777X To Enter Service In 2027 After 7-Year ... Top Stories Lufthansa’s 1st Boeing 777X is now in flight testing Why The Boeing 777X Is Worth Waiting And Waiting And ... - Forbes Boeing 777X Set for 2027 Debut After Costly Delays and ... Boeing 777X: Everything You Need To Know - Dj's Aviation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_787_Dreamliner">Boeing 787 Dreamliner - Wikipedia Images 787 Dreamliner - The Boeing Company Boeing 787: 5 Things To Know Before Your First Flight On The ... Boeing 787 Overview and Seat Map - Airportix Boeing 787 Seat Map 2026: 106 Layouts from 57+ | Flight Seatmap All About Boeing 787 Dreamliner: Design, Features, Crashes ... Boeing 787 - Aviation Week</a></li>

</ul>
</details>

**标签**: `#Boeing`, `#China`, `#aviation`, `#trade`, `#737 MAX`

---

<a id="item-15"></a>
## [加州集体诉讼指控 OpenAI 向 Meta 和 Google 分享用户数据](https://futurism.com/artificial-intelligence/openai-personal-information-meta-google) ⭐️ 7.0/10

在加州提起的一项集体诉讼指控 OpenAI 未经适当同意，通过 Meta Pixel 和 Google Analytics 跟踪工具，将用户的聊天查询、邮箱地址和用户 ID 分享给 Meta 和 Google。 这起诉讼凸显了主要 AI 公司如何处理用户数据的重大隐私问题，可能影响数百万用户，并为 AI 行业的数据共享实践树立先例。 诉讼指控 OpenAI 违反了《加州隐私侵犯法》和《电子通信隐私法》，OpenAI 尚未回应置评请求。

telegram · zaihuapd · May 15, 03:45

**背景**: Meta Pixel 是一种 JavaScript 跟踪代码，用于监控用户在网站上的行为；Google Analytics 是一种网络分析服务，用于跟踪和报告网站流量。这两种工具常用于广告和分析，但可能将个人数据传输到各自的平台。《加州隐私侵犯法》禁止未经同意的窃听和电子窃听。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Meta_Pixel">Meta Pixel</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Analytics">Google Analytics</a></li>
<li><a href="https://taulersmith.com/california-invasion-of-privacy-act">California Invasion of Privacy Act | Tauler Smith LLP</a></li>

</ul>
</details>

**标签**: `#privacy`, `#lawsuit`, `#OpenAI`, `#data sharing`, `#AI ethics`

---

<a id="item-16"></a>
## [支付宝回应支付功能关闭后仍被扣款 184 万元捐赠](https://m.thepaper.cn/newsDetail_forward_33181083) ⭐️ 7.0/10

支付宝于 2026 年 5 月 15 日回应称，已向警方寻求帮助，此前一名用户反映其支付宝账户在关闭支付功能三年后，仍被扣款 184 万元用于公益捐赠。 这一事件引发了对支付系统安全和授权完整性的严重担忧，可能影响用户对数字支付平台及公益捐赠机制的信任。 该用户账户被扣款 6 次，捐赠给中国乡村发展基金会，其中单笔最大金额为 184 万元。银行调查发现，虽然一般支付功能已关闭，但公益捐赠功能仍可正常使用。

telegram · zaihuapd · May 15, 07:00

**背景**: 支付宝是中国领先的数字支付平台，广泛用于在线交易和公益捐赠。中国乡村发展基金会是一家全国性大型慈善组织。此案凸显了支付授权系统中的潜在漏洞，即特定功能可能在一般功能关闭后仍保持激活状态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260515A03G4Y00">支付宝回应关闭支付功能后仍被扣款捐赠184万：不排除涉嫌违法犯罪的可...</a></li>
<li><a href="https://www.163.com/dy/article/KSVGFA460550B6IS.html">支付宝最新回应“关闭支付功能后被扣捐赠184万”：系正常执行支付指令，...</a></li>
<li><a href="https://finance.sina.com.cn/wm/2026-05-15/doc-inhxyccf9379617.shtml">“关闭支付功能后，仍被扣款捐赠184万”，支付宝最新回应：不排除涉嫌违...</a></li>

</ul>
</details>

**标签**: `#security`, `#payment systems`, `#Alipay`, `#fraud`, `#China`

---

<a id="item-17"></a>
## [苹果与 OpenAI 合作出现裂痕，OpenAI 考虑法律行动](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 7.0/10

苹果与 OpenAI 为期两年的合作关系出现紧张，OpenAI 指责苹果未能充分推广 ChatGPT 集成，导致订阅转化率远低于预期，目前正在探索法律选项，可能发出正式违约通知。 这一争端可能重塑 AI 模型在消费设备中的集成方式，因为苹果计划在 iOS 27 中向 Claude 和 Gemini 等第三方模型开放 Siri，可能终结 ChatGPT 的独家地位，影响整个 AI 生态系统。 OpenAI 已聘请外部律师研究法律选项，可能很快发出正式违约通知。苹果也对 OpenAI 的隐私标准、硬件业务和挖角工程师感到不满，并计划在 6 月 WWDC 上展示 iOS 27 对第三方 AI 模型的支持。

telegram · zaihuapd · May 15, 12:59

**背景**: 苹果与 OpenAI 于 2024 年宣布合作，将 ChatGPT 集成到 Siri 和其他 Apple Intelligence 功能中。该协议预计为双方带来数十亿美元的订阅收入，但集成被批评为隐蔽且功能受限，多数用户仍使用独立的 ChatGPT 应用。苹果现在转向多模型策略，iOS 27 将允许用户选择多种 AI 助手。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight">OpenAI - Apple Partnership Frays, Setting Up Possible... - Bloomberg</a></li>
<li><a href="https://techcrunch.com/2026/05/14/openai-is-reportedly-preparing-legal-action-against-apple-it-wouldnt-be-the-first-partner-to-feel-burned/">OpenAI is reportedly preparing legal action against Apple ; it...</a></li>
<li><a href="https://apple.gadgethacks.com/news/ios-27-siri-third-party-ai-assistants-explained-apples-strategy/">iOS 27 Siri Third-Party AI Assistants Explained: Apple's ...</a></li>

</ul>
</details>

**标签**: `#Apple`, `#OpenAI`, `#AI partnerships`, `#legal dispute`, `#ChatGPT`

---