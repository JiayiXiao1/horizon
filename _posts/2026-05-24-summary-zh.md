---
layout: default
title: "Horizon Summary: 2026-05-24 (ZH)"
date: 2026-05-24
lang: zh
---

> From 31 items, 16 important content pieces were selected

---

1. [80386 微码被反汇编并分析](#item-1) ⭐️ 9.0/10
2. [Anthropic 的 Project Glasswing：AI 发现逾万高危漏洞](#item-2) ⭐️ 9.0/10
3. [苹果开源 corecrypto，附量子安全算法形式化验证](#item-3) ⭐️ 9.0/10
4. [微软财报意外披露 OpenAI 单季度巨亏 1150 亿美元](#item-4) ⭐️ 9.0/10
5. [特朗普政府终止大多数绿卡申请人的身份调整](#item-5) ⭐️ 8.0/10
6. [SpaceX 首次试飞 Starship V3 火箭](#item-6) ⭐️ 8.0/10
7. [从第一性原理优化深度学习](#item-7) ⭐️ 8.0/10
8. [AI 内存需求推高消费电子价格](#item-8) ⭐️ 8.0/10
9. [中国八部门联合整治非法跨境证券交易](#item-9) ⭐️ 8.0/10
10. [Cloudflare 全球故障 25 分钟，影响 28% HTTP 流量](#item-10) ⭐️ 8.0/10
11. [微软大规模推广 Claude Code，鼓励非技术员工使用 AI 编程](#item-11) ⭐️ 8.0/10
12. [海盗船采用长鑫芯片，DDR5 价格或下调](#item-12) ⭐️ 8.0/10
13. [对 HTML <dl>元素的批评引发语义 HTML 讨论](#item-13) ⭐️ 7.0/10
14. [FTC 对 Cox Media Group 虚假 AI“主动监听”广告处以罚款](#item-14) ⭐️ 7.0/10
15. [腾讯收购喜马拉雅获批，附条件放弃独家版权](#item-15) ⭐️ 7.0/10
16. [我国日均词元调用量两年增超千倍，突破 140 万亿](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [80386 微码被反汇编并分析](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 9.0/10

Reenigne 基于 Ken Shirriff 提供的高分辨率微码 ROM 图像，发布了 80386 微码的详细反汇编与分析。 这项逆向工程揭示了 80386 如何在微架构层面实现复杂的 x86 指令，为复古计算爱好者和 CPU 架构研究者提供了宝贵的见解。 反汇编覆盖了整个微码 ROM，记录了执行 MOV、ADD 和内存分段等指令的微操作。这项工作建立在 reenigne 早期 8086 微码反汇编的基础上。

hackernews · nand2mario · May 23, 12:11 · [社区讨论](https://news.ycombinator.com/item?id=48247004)

**背景**: 微码是控制 CPU 内部硬件的低级指令层，将复杂的机器指令翻译成更简单的微操作。80386 于 1985 年发布，是英特尔首款 32 位 x86 处理器，也是 CPU 设计的里程碑。逆向其微码有助于揭示经典处理器的内部工作原理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 Microcode Disassembled - Reenigne blog</a></li>
<li><a href="https://nand2mario.github.io/posts/2026/z386/">z386: An Open-Source 80386 Built Around Original Microcode</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microarchitecture">Microarchitecture - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区对这项逆向工程表示惊叹和赞赏。评论包括关于从芯片图像中提取微码过程的技术问题、对开源 z386 等相关项目的引用，以及关于微编程的进一步阅读推荐。

**标签**: `#reverse engineering`, `#microcode`, `#80386`, `#CPU architecture`, `#retrocomputing`

---

<a id="item-2"></a>
## [Anthropic 的 Project Glasswing：AI 发现逾万高危漏洞](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic 公布了 Project Glasswing 的初期成果，其 Claude Mythos Preview 模型在一个月内从关键软件和数千个开源项目中发现了超过一万个高危或严重漏洞，经审查的漏洞中 90.6% 为真阳性。 这表明 AI 现在能够以远超人类能力的规模和速度发现漏洞，将瓶颈从发现转移到验证和修补，这对软件安全和开源生态系统具有重大影响。 该模型扫描了数千个开源项目，发现 6202 个高危漏洞，其中 1752 个经过审查，真阳性率为 90.6%。Cloudflare 等合作伙伴报告漏洞发现速度提高了十倍。

telegram · zaihuapd · May 23, 03:16

**背景**: Project Glasswing 是 Anthropic 发起的一项全行业网络安全倡议，与 Claude Mythos Preview 的受限预览版同时推出。Claude Mythos Preview 是一个不向公众开放的前沿通用模型，能够自主发现和利用漏洞，既带来了安全收益也引发了担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/04/08/anthropic-claude-mythos-preview-identify-vulnerabilities/">Anthropic's new AI model finds and exploits... - Help Net Security</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-latest-ai-model-identifies-thousands-of-zero-day-vulnerabilities-in-every-major-operating-system-and-every-major-web-browser-claude-mythos-preview-sparks-race-to-fix-critical-bugs-some-unpatched-for-decades">Anthropic's latest AI model identifies 'thousands of... | Tom's H...</a></li>

</ul>
</details>

**标签**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#Anthropic`, `#open source`

---

<a id="item-3"></a>
## [苹果开源 corecrypto，附量子安全算法形式化验证](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 9.0/10

苹果开源了 corecrypto 密码库，其中包含量子安全算法 ML-KEM 和 ML-DSA 的实现，并提供了端到端的形式化验证证明，从数学上保证这些实现与 NIST 标准严格一致。 这是密码学保障的一个重要里程碑，因为形式化验证为将在超过 25 亿台活跃苹果设备上运行的代码提供了最高级别的正确性信心，从而保护未来通信免受量子计算机攻击。 形式化证明覆盖了 C 代码和手工优化的 ARM64 汇编，苹果还公开了其定制验证工具和 Isabelle 理论库，供独立专家评估。

telegram · zaihuapd · May 23, 04:49

**背景**: ML-KEM（原 Kyber）和 ML-DSA（原 Dilithium）是 NIST 于 2024 年标准化的后量子密码算法，旨在抵御未来量子计算机的攻击。形式化验证使用数学证明来确保软件实现与其规范完全一致，从而消除整类错误。苹果的 corecrypto 库为 iOS、macOS 及其他苹果平台提供基础加密运算。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kyber">ML - KEM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isabelle_(proof_assistant)">Isabelle (proof assistant) - Wikipedia</a></li>

</ul>
</details>

**标签**: `#cryptography`, `#formal verification`, `#quantum-safe`, `#open source`, `#Apple`

---

<a id="item-4"></a>
## [微软财报意外披露 OpenAI 单季度巨亏 1150 亿美元](https://t.me/zaihuapd/41537) ⭐️ 9.0/10

微软最新财报意外披露，根据其权益法投资核算，OpenAI 单季度净亏损约 1150 亿美元，这一亏损规模几乎是 OpenAI 2025 年上半年 43 亿美元营收的三倍。 这一披露凸显了前沿人工智能研究的极高资本密集度，引发了对 AI 开发财务可持续性的质疑。同时也突显了微软等主要投资者面临的巨大财务风险，微软已向 OpenAI 投入 130 亿美元。 微软持有 OpenAI 约 27% 的股权，1150 亿美元的亏损是根据微软净利润减少 31 亿美元推算得出。若按税前损失和微软实际持股比例 32.5% 计算，亏损可能超过 1200 亿美元。

telegram · zaihuapd · May 23, 07:40

**背景**: 权益法会计要求投资者按持股比例确认被投资方的损益。OpenAI 的巨额亏损主要源于维持大模型领先地位所需的巨大资本支出，包括 GPU 集群等算力基础设施。其订阅和 API 服务的收入未能跟上这些成本的增长。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.qbitai.com/2025/11/347840.html">微软独家：OpenAI最新季度净亏损115亿美元</a></li>
<li><a href="https://www.zhihu.com/question/1967900167182181978">媒体曝 OpenAI 单季度亏损 120 亿美元，具体情况如何？目前 OpenAI 发展面临哪些问题？ - 知乎</a></li>
<li><a href="https://www.ifanr.com/1653377">OpenAI 再不上市，财务窟窿就要把巨头们拖垮了 | 爱范儿</a></li>

</ul>
</details>

**社区讨论**: 知乎等平台上的社区评论对亏损规模表示震惊，许多人指出 OpenAI 的支出不可持续，并对当前 AI 投资模式的长期可行性提出质疑。一些评论者认为 OpenAI 可能需要上市或寻求额外融资来覆盖其现金消耗。

**标签**: `#OpenAI`, `#Microsoft`, `#AI Economics`, `#Financial Disclosure`, `#Artificial Intelligence`

---

<a id="item-5"></a>
## [特朗普政府终止大多数绿卡申请人的身份调整](https://www.nytimes.com/2026/05/22/us/politics/green-card-changes-trump.html) ⭐️ 8.0/10

2026 年 5 月 22 日，特朗普政府宣布，大多数绿卡申请人必须离开美国，通过海外领事程序申请，除非在特殊情况下，否则不再允许在美国境内调整身份。 这项政策严重扰乱了数十万合法移民的生活，尤其是 H-1B 技术工人，他们现在面临与家人和工作的长期分离，可能导致人才流失，损害美国科技行业。 USCIS 备忘录（PM-602-0199）规定，身份调整仅在特殊情况下才会获批，实际上要求大多数申请人使用领事处理程序，这可能导致在美国海外领事馆等待多年。

hackernews · tlhunter · May 22, 21:27 · [社区讨论](https://news.ycombinator.com/item?id=48241890)

**背景**: 身份调整（AOS）长期以来允许已在美国持临时签证的移民在不离境的情况下申请绿卡。而领事处理程序则要求申请人返回母国或第三国，在美国大使馆或领事馆进行面谈。这一改变颠覆了数十年的标准做法，给申请人带来了巨大的不确定性和困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.uscis.gov/newsroom/news-releases/us-citizenship-and-immigration-services-will-grant-adjustment-of-status-only-in-extraordinary">U.S. Citizenship and Immigration Services Will Grant ‘Adjustment of Status’ Only in Extraordinary Circumstances | USCIS</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了震惊和愤怒，称该政策疯狂且鲁莽。许多人指出了实际困境：在美国出生的孩子需要签证才能离境、领事馆多年积压、以及可能被困海外的风险。一些最近获得绿卡的人感到庆幸，但也对未来入籍申请感到担忧。

**标签**: `#immigration`, `#US policy`, `#tech workers`, `#green card`, `#H-1B`

---

<a id="item-6"></a>
## [SpaceX 首次试飞 Starship V3 火箭](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 8.0/10

SpaceX 于 2026 年 5 月 22 日从德克萨斯州的 Starbase 发射了首枚 Starship V3 原型机。上级成功精准着陆，但 Super Heavy 助推器在返回过程中出现发动机故障，飞船发动机舱也显示出损坏迹象。 这次试飞标志着 SpaceX 在迭代开发世界最强大火箭过程中的关键里程碑，使其更接近完全可重复使用和运营能力。飞船成功着陆和隔热罩性能改进显示了重大进展，而助推器问题则凸显了尚存的挑战。 上升过程中，Super Heavy 助推器的一台发动机提前关机。助推器的回推燃烧失败，着陆燃烧导致偏离目标的硬溅落。Starship 上级在级分离后不久失去一台发动机，发动机舱出现可见的红光和喷气，但仍精确着陆在目标点。

hackernews · busymom0 · May 22, 23:41 · [社区讨论](https://news.ycombinator.com/item?id=48242959)

**背景**: Starship 是 SpaceX 正在开发的两级完全可重复使用的超重型运载火箭。它由 Super Heavy 助推器和 Starship 飞船组成，两者均使用燃烧液态甲烷和液氧的 Raptor 发动机。V3 版本比之前的迭代更大、更强大，旨在最终将宇航员和货物运送到月球、火星及更远的地方。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starship_prototypes">Starship prototypes</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://arstechnica.com/space/2026/05/spacexs-starship-v3-still-a-work-in-progress-mostly-successful-on-first-flight/">SpaceX's Starship V3—still a work in progress—mostly... - Ars Technica</a></li>

</ul>
</details>

**社区讨论**: 社区评论赞扬了飞船成功着陆和隔热罩的改进，一位用户指出再入过程中没有可见的热点。然而，对助推器未能完成返回感到失望，一些人还对发动机舱损坏表示担忧。总体情绪是积极的，赞赏 SpaceX 的快速迭代方法。

**标签**: `#SpaceX`, `#Starship`, `#rocket launch`, `#space exploration`, `#engineering`

---

<a id="item-7"></a>
## [从第一性原理优化深度学习](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

一篇全面的博客文章通过将效率分解为计算、内存和开销三个组成部分，解释了如何优化深度学习系统以实现最大硬件利用率。 这篇文章提供了基础性理解，帮助从业者识别瓶颈并进行针对性优化，这在深度学习模型规模和复杂性不断增长的背景下至关重要。 文章采用第一性原理方法，指出在 Python 执行一次 FLOP 的时间内，A100 GPU 可以完成 975 万次 FLOP，凸显了高级代码与硬件能力之间的巨大差距。

hackernews · tosh · May 23, 11:50 · [社区讨论](https://news.ycombinator.com/item?id=48246889)

**背景**: 深度学习训练和推理常因 Python 开销、数据传输和次优内核配置而导致硬件利用率低下。理解计算受限、内存受限和开销受限这三种状态，使开发者能够优先进行最有效的优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://horace.io/brrr_intro.html">Making Deep Learning go Brrrr From First Principles</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞这篇文章是经典之作，并强调了 NVIDIA 在 TFLOPs、带宽和互连方面的持续领先。其他人则指出性能可移植性的复杂性——模型在不同运行时和硬件上表现各异，并表达了对生产系统故障模式的兴趣。

**标签**: `#deep learning`, `#performance optimization`, `#NVIDIA`, `#ML systems`, `#GPU computing`

---

<a id="item-8"></a>
## [AI 内存需求推高消费电子价格](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 8.0/10

内存制造商正将晶圆产能从 DDR 和 LPDDR 重新分配给 AI 数据中心所需的 HBM，导致消费级内存短缺和价格上涨，尤其影响 100 美元以下的智能手机。 这一转变意味着智能手机、笔记本电脑和游戏机等消费电子产品将在未来几年内变得更贵，对非洲和南亚的低收入市场影响尤为严重。 HBM 每 GB 消耗的晶圆产能是 DDR 或 LPDDR 的三倍以上，其分配比例预计从 2%上升到 2026 年底的 20%。内存公司故意控制产能以维持利润。

rss · Simon Willison · May 22, 22:01

**背景**: DRAM 内存主要有三种类型：DDR（用于台式机/服务器）、LPDDR（用于移动/低功耗设备）和 HBM（用于 GPU 的高带宽内存）。它们都在相同的晶圆生产线上制造，因此增加 HBM 产量会减少其他类型的产能。内存行业仅由三家公司（三星、SK 海力士、美光）主导，它们在经历过去的繁荣-萧条周期后学会了避免过度投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://semiwiki.com/wikis/semiconductor-ip-wikis/ddr-vs-lpddr-vs-hbm-wiki/">DDR vs. LPDDR vs. HBM Wiki - SemiWiki</a></li>

</ul>
</details>

**标签**: `#memory`, `#AI`, `#hardware`, `#market analysis`, `#supply chain`

---

<a id="item-9"></a>
## [中国八部门联合整治非法跨境证券交易](https://t.me/zaihuapd/41525) ⭐️ 8.0/10

中国八部门联合印发整治方案，严厉打击非法跨境证券、期货和基金经营活动，只允许存量投资者在两年集中整治期内单向卖出并转出资金。证监会已对老虎证券、富途控股和长桥的非法跨境展业行为立案调查。 此次整治标志着对跨境证券交易的监管大幅收紧，将影响数百万使用境外平台的中国投资者，可能重塑金融科技行业格局，迫使相关平台合规或退出中国市场。 富途控股拟被罚款 185 亿元，老虎证券子公司被罚没约 41.1 亿元。整治对象不仅包括境外平台，还包括协助非法跨境展业的境内关联方、中介以及提供开户通道和营销引流的信息平台和自媒体。

telegram · zaihuapd · May 22, 13:55

**背景**: 许多中国投资者使用富途、老虎等境外券商交易港股和美股，这种行为在中国证券法下并不完全合法。证监会此前多次警告，但执法力度有限。新方案明确了整治时间表和处罚措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml">m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml</a></li>
<li><a href="https://m.jiemian.com/article/14471841.html">m.jiemian.com/article/14471841.html</a></li>
<li><a href="https://www.21jingji.com/article/20260523/herald/e7eb58bb6994d891f986fd9d06c85b1d.html">中国 证 监会拟对 富 途 罚 款18.5亿， 老 虎 证 券 罚 没4.112亿 - 21经济网</a></li>

</ul>
</details>

**标签**: `#regulation`, `#China`, `#cross-border trading`, `#securities`, `#fintech`

---

<a id="item-10"></a>
## [Cloudflare 全球故障 25 分钟，影响 28% HTTP 流量](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

2025 年 12 月 5 日 08:47 UTC，Cloudflare 发生全球性故障，持续约 25 分钟，影响约 28%的 HTTP 流量。故障源于为修复 Next.js 安全漏洞（CVE-2025-55182）而更新的 WAF 托管规则集。 此次故障凸显了集中式 Web 基础设施的脆弱性，因为 Cloudflare 保护着全球互联网流量的很大一部分。该事件还揭示了大规模部署安全补丁而未经充分测试的风险。 故障主要影响使用旧版 FL1 代理和 Cloudflare 托管规则集的客户。有问题的 WAF 更新旨在缓解 CVE-2025-55182，这是 React Server Components 中的一个严重未认证远程代码执行漏洞，通过 Next.js 被利用。

telegram · zaihuapd · May 22, 16:15

**背景**: Cloudflare 是一家主要的 CDN 和 Web 安全提供商，处理全球 HTTP 流量的很大一部分。其 Web 应用防火墙（WAF）使用托管规则集来阻止恶意请求。漏洞 CVE-2025-55182（又称 React2Shell）允许攻击者在运行 React Server Components 的服务器上无需认证即可执行任意代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/waf/managed-rules/">Managed Rules · Cloudflare Web Application Firewall ( WAF ) docs</a></li>
<li><a href="https://react.dev/blog/2025/12/03/critical-security-vulnerability-in-react-server-components">Critical Security Vulnerability in React Server Components – React</a></li>
<li><a href="https://medium.com/@pnadheem/your-next-js-app-might-be-fine-until-one-weird-request-hits-it-react2shell-cve-2025-55182-3a6d0ed214e0">Your Next . js App Might Be “Fine”… Until One Weird Request... | Medium</a></li>

</ul>
</details>

**标签**: `#Cloudflare`, `#outage`, `#WAF`, `#Next.js`, `#security`

---

<a id="item-11"></a>
## [微软大规模推广 Claude Code，鼓励非技术员工使用 AI 编程](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

微软正在其核心工程团队（包括 CoreAI 团队以及负责 Windows、Microsoft 365 和 Outlook 的团队）中广泛部署 Anthropic 的 Claude Code，并鼓励非技术员工使用它进行原型设计。工程师现在需要同时使用 Claude Code 和 GitHub Copilot，并提供对比反馈。 此举标志着微软 AI 辅助开发策略的重大转变——它在使用自家 GitHub Copilot 的同时，也采用了竞争对手的工具，这可能会影响整个行业的实践。同时，它降低了非技术员工参与软件原型设计的门槛，有望加速公司内部的创新。 Claude Code 是 Anthropic 开发的 AI 编程代理，可在终端或 IDE 中运行；而 GitHub Copilot 是微软自家的 AI 结对编程工具。要求工程师对比这两种工具，表明微软正在评估它们在不同任务中的表现优劣。

telegram · zaihuapd · May 23, 06:05

**背景**: Claude Code 是 Anthropic 的 Claude 模型系列的一部分，该系列采用宪法 AI（constitutional AI）技术以确保伦理合规。GitHub Copilot 由 GitHub 和 OpenAI 开发，是一款广泛使用的代码补全工具，集成于主流 IDE 中。微软在自家工具之外还采用竞争对手的工具，反映了 AI 辅助开发领域快速演变的格局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#Microsoft`, `#Claude Code`, `#GitHub Copilot`, `#software engineering`

---

<a id="item-12"></a>
## [海盗船采用长鑫芯片，DDR5 价格或下调](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

美商海盗船已开始在其 DDR5 内存模组中使用中国厂商长鑫存储（CXMT）的芯片，6000 MT/s 规格的产品已上市。 这一转变使 DRAM 供应链更加多元化，随着中国产能扩张，DDR5 价格有望下降，尤其是在 AI 对 HBM 的需求挤压消费级 DRAM 供应的背景下。 基于长鑫芯片的 DDR5 模组运行在 6000 MT/s，性能与国际主流产品一致。长鑫存储在 2026 年第一季度业绩强劲，并计划年内上市。

telegram · zaihuapd · May 23, 11:17

**背景**: DRAM 是一种用于计算机和服务器的内存。全球 DRAM 市场由三星、SK 海力士和美光三大巨头主导。近期，这些公司已将产能转向 AI 所需的高带宽内存（HBM），导致消费级 DDR5 供应减少。长鑫存储是一家中国 DRAM 制造商，正在扩大产能以填补市场空缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>

</ul>
</details>

**标签**: `#DDR5`, `#DRAM`, `#Corsair`, `#CXMT`, `#supply chain`

---

<a id="item-13"></a>
## [对 HTML <dl>元素的批评引发语义 HTML 讨论](https://benmyers.dev/blog/on-the-dl/) ⭐️ 7.0/10

Ben Myers 发表了一篇对 HTML <dl>元素的详细批评，认为其设计和用法在现代 Web 开发中存在缺陷。该文章在 Hacker News 上引发了大量讨论，获得 106 条评论和 346 个点赞。 这篇批评挑战了语义 HTML（Web 可访问性和 SEO 的基石）的实用价值。这场辩论凸显了理论语义与现实开发需求之间的张力，影响开发者如何选择标记方式。 <dl>元素没有隐式 ARIA 角色，且在没有显式角色的情况下不允许使用 aria-label。开发者经常发现<dl>对于复杂布局过于僵化，例如需要多个包装器或部分之间的分隔线。

hackernews · ravenical · May 23, 13:03 · [社区讨论](https://news.ycombinator.com/item?id=48247325)

**背景**: 语义 HTML 使用传达内容结构含义的元素，提高可访问性和 SEO。<dl>元素最初设计用于定义列表（如词汇表），但现在用于各种键值对展示。批评者认为其限制使其在现代 Web 界面中不实用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://frontman.sh/glossary/semantic-html/">Semantic HTML | Frontman Glossary</a></li>
<li><a href="https://www.codecademy.com/resources/blog/semantic-html/">codecademy.com/resources/blog/ semantic - html</a></li>
<li><a href="https://academi.dev/html-semantics-and-accessibility/">HTML Semantics and Accessibility Explained: Building... | Academi</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了不同观点：一些人同意语义 HTML 设计不佳且不实用，而另一些人则为其历史根源和可访问性优势辩护。一位评论者指出<dl>在 Web 出现之前就已使用，引用了 1985 年的 IBM 手册。

**标签**: `#HTML`, `#semantic web`, `#accessibility`, `#web development`

---

<a id="item-14"></a>
## [FTC 对 Cox Media Group 虚假 AI“主动监听”广告处以罚款](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

FTC 宣布，Cox Media Group、MindSift 和 1010 Digital Works 将支付近 100 万美元，以和解他们虚假营销“主动监听”AI 服务的指控，该服务声称能通过监听智能设备对话来投放广告。 这一执法行动为打击虚假 AI 营销声明树立了先例，强化了公司不能夸大 AI 能力来销售服务，尤其是涉及侵犯消费者隐私的监控服务。 FTC 发现，“主动监听”服务实际上并未监听对话或使用语音数据，而是以加价方式转售数据经纪商的电子邮件列表。FTC 还指出，在服务条款中隐藏选择同意并不构成充分同意。

rss · Simon Willison · May 22, 04:48

**背景**: 2024 年，Cox Media Group 营销了一项“主动监听”服务，声称智能设备通过监听对话捕获实时意图数据。这助长了手机通过麦克风监听用户以投放广告的阴谋论。FTC 的行动驳斥了这些说法，表明该服务只是转售的电子邮件列表。

**标签**: `#FTC`, `#AI`, `#privacy`, `#regulation`, `#marketing`

---

<a id="item-15"></a>
## [腾讯收购喜马拉雅获批，附条件放弃独家版权](https://mp.weixin.qq.com/s/xnx31SOS6NMozZXnHeaaQg) ⭐️ 7.0/10

国家市场监管总局批准腾讯收购喜马拉雅，要求腾讯放弃在线音频版权独家授权，并在限期内解除现有独家合同。 这一决定打破了喜马拉雅的独家内容壁垒，使竞争平台能够获取相同音频内容，可能重塑中国在线音频市场的竞争格局，并提升用户跨平台收听的便利性。 腾讯不得达成或变相达成在线音频版权独家授权，并需逐步解除现有独家合同。腾讯表示将配合解除独家合同，后续寻求非独家合作。

telegram · zaihuapd · May 22, 10:33

**背景**: 喜马拉雅是中国领先的在线音频平台，以拥有大量独家内容（如有声书和播客）而闻名。独家版权协议一直是其关键竞争优势，但也成为用户跨平台获取内容的障碍。监管机构的附加条件旨在促进公平竞争和消费者选择。

**标签**: `#antitrust`, `#China`, `#online audio`, `#acquisition`, `#regulation`

---

<a id="item-16"></a>
## [我国日均词元调用量两年增超千倍，突破 140 万亿](https://t.me/zaihuapd/41542) ⭐️ 7.0/10

国家数据局披露，我国日均词元（Token）调用量在 2025 年 3 月突破 140 万亿，而 2024 年初仅为 1000 亿，两年增长超千倍。 这一爆炸性增长表明中国人工智能商业化进程加速，围绕词元定价和结算的数据市场正在形成，可能推动 AI 在各行业的广泛应用。 词元是大模型处理信息的最小单元，其调用量是衡量 AI 使用量的关键指标。该数据由国家数据局披露，具有官方权威性。

telegram · zaihuapd · May 23, 14:36

**背景**: 词元是大语言模型处理文本的基本单元，可以是单词、子词或字符。词元经济是指围绕词元的计量、定价和交易形成的新体系，支撑 AI 商业化服务。中国数据要素市场化配置改革旨在促进数据作为生产要素的流通和定价。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/docs/transformers/zh/main_classes/tokenizer">Tokenizer - Hugging Face</a></li>
<li><a href="https://www.moomoo.com/news/post/70293298/china-galaxy-securities-operators-introduction-of-token-based-plans-opens">China Galaxy Securities: Operators' Introduction of Token-Based Plans ...</a></li>
<li><a href="https://qwen.readthedocs.io/zh-cn/latest/getting_started/concepts.html">核心概念 - Qwen</a></li>

</ul>
</details>

**标签**: `#AI`, `#China`, `#token economy`, `#data market`, `#industry growth`

---