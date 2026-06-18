---
layout: default
title: "Horizon Summary: 2026-06-18 (ZH)"
date: 2026-06-18
lang: zh
---

> From 44 items, 25 important content pieces were selected

---

1. [GLM-5.2：领先的开源权重大模型发布](#item-1) ⭐️ 9.0/10
2. [哪吒监控高危路径穿越漏洞（CVSS 9.1）](#item-2) ⭐️ 9.0/10
3. [Epic Games 推出开源版本控制系统 Lore](#item-3) ⭐️ 8.0/10
4. [泄露文件显示 OpenAI 每年亏损数十亿美元](#item-4) ⭐️ 8.0/10
5. [美国科学陷入危机：资金、签证、人才流失](#item-5) ⭐️ 8.0/10
6. [Adam 推出 CADAM：开源 AI CAD 工具，文本生成模型](#item-6) ⭐️ 8.0/10
7. [Tesco 因 Broadcom 定价迁移 4 万工作负载离开 VMware](#item-7) ⭐️ 8.0/10
8. [RFC 10008 标准化 HTTP QUERY 方法](#item-8) ⭐️ 8.0/10
9. [Charity Majors：AI 要求更强的工程纪律](#item-9) ⭐️ 8.0/10
10. [AI 模型出口管制损害美国网络防御](#item-10) ⭐️ 8.0/10
11. [GitHub Copilot 2026 年 6 月起改为按用量计费](#item-11) ⭐️ 8.0/10
12. [中国将科创板 IPO 标准扩展至 AI 与硬科技](#item-12) ⭐️ 8.0/10
13. [微软借 OpenAI 模型在华扩张 AI 业务](#item-13) ⭐️ 8.0/10
14. [美国推迟将 DeepSeek 及百余家中国公司列入黑名单](#item-14) ⭐️ 7.0/10
15. [在 EC2 上运行 Firecracker 虚拟机，浏览器启动不到 1 秒](#item-15) ⭐️ 7.0/10
16. [AI 模型在“最后特工生存”游戏基准测试中一决高下](#item-16) ⭐️ 7.0/10
17. [大众汽车屏蔽 GrapheneOS 用户使用其应用](#item-17) ⭐️ 7.0/10
18. [MicroUI：用 ANSI C 编写的微型即时模式 GUI 库](#item-18) ⭐️ 7.0/10
19. [Photobucket 要求支付 5 美元才能取回你的照片](#item-19) ⭐️ 7.0/10
20. [Datasette 1.0a34 新增行级增删改界面](#item-20) ⭐️ 7.0/10
21. [Georgi Gerganov 认可 Qwen3.6-27B 用于本地编程](#item-21) ⭐️ 7.0/10
22. [Anthropic 企业 AI 市场份额首超 OpenAI](#item-22) ⭐️ 7.0/10
23. [微信支付推出 AI 专属卡，每笔消费需本人授权](#item-23) ⭐️ 7.0/10
24. [运营商词元套餐成本高昂，开发者直呼用不起](#item-24) ⭐️ 7.0/10
25. [OpenAI Codex 现支持自定义第三方模型提供者](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GLM-5.2：领先的开源权重大模型发布](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai 于 2026 年 6 月 16 日发布了 GLM-5.2，这是一个 753B 参数的混合专家（MoE）开源权重大模型，具有 40B 活跃参数和 100 万 token 的上下文窗口，采用 MIT 许可证。 GLM-5.2 是首个在 Artificial Analysis 智能指数中排名第一的开源权重模型，超越了 MiniMax-M3 和 DeepSeek V4 Pro，并在 Code Arena WebDev 排行榜上位列第二，以极低的成本挑战了闭源模型。 该模型在智能指数上每个任务使用 43k 输出 token，高于竞争对手，并通过 OpenRouter 以输入 $1.40/M、输出 $4.40/M 的价格提供。该模型仅支持文本输入；Z.ai 的视觉模型 GLM-5V-Turbo 仍为闭源。

rss · Simon Willison · Jun 17, 23:58

**背景**: 混合专家（MoE）是一种架构，每个 token 仅激活部分参数，从而使大模型更高效。GLM-5.2 的 100 万 token 上下文窗口允许处理非常长的文档，例如整个代码库或书籍。开源权重模型是指模型参数公开可用，允许研究人员和开发者本地运行或微调。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.datacamp.com/blog/glm-5-2">GLM - 5 . 2 : Features, Setup, and Model Switching Guide | DataCamp</a></li>
<li><a href="https://lushbinary.com/blog/glm-5-2-developer-guide-1m-context-coding-plan/">GLM 5 . 2 Developer Guide: 1M Context & MoE | Lushbinary</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞 GLM-5.2 的性能和低成本，有人指出其以极低价格媲美 Opus 4.7 等闭源模型。但也有用户对推理效率表示担忧，称一个简单的数学求值器任务耗时 15 分钟、消耗 45k token。还有人指出该模型相比同类模型更消耗 token。

**标签**: `#LLM`, `#open-weights`, `#GLM-5.2`, `#AI`, `#benchmark`

---

<a id="item-2"></a>
## [哪吒监控高危路径穿越漏洞（CVSS 9.1）](https://t.me/zaihuapd/42001) ⭐️ 9.0/10

哪吒监控（Nezha）v2.0.13 以下版本被披露存在严重未授权路径穿越漏洞（CVE-2026-53519，CVSS 9.1），攻击者可读取配置文件并获取 JWT 密钥。 该漏洞影响广泛使用的开源监控工具，未授权攻击者可窃取 JWT 密钥从而危及整个监控基础设施，可能导致系统完全被控。 攻击者通过构造类似 /dashboard../data/config.yaml 的 GET 请求利用漏洞，利用前缀混淆逻辑绕过认证。用户应立即升级至 v2.0.13 或更高版本。

telegram · zaihuapd · Jun 17, 01:25

**背景**: 哪吒监控是一款流行的开源轻量级服务器监控与告警系统。路径穿越漏洞允许攻击者访问预期目录之外的文件。JWT 密钥用于签名认证令牌，一旦泄露，攻击者可伪造令牌并获得未授权访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tjsky.net/news/1664">哪吒探针爆致命 漏 洞 （ CVE - 2026 - 53519 ）大批 MJJ... | 秋风于渭水</a></li>
<li><a href="https://nezha.io/">哪 吒 监 控 Nezha Monitoring</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#open-source`, `#monitoring`, `#path-traversal`

---

<a id="item-3"></a>
## [Epic Games 推出开源版本控制系统 Lore](https://lore.org/) ⭐️ 8.0/10

Epic Games 宣布了 Lore，一个专为可扩展性设计的开源版本控制系统，旨在与 Perforce 竞争游戏开发市场。 Lore 解决了游戏开发中的一个主要痛点——处理大型二进制文件和文件锁定——而 Git 在这方面表现不佳，它可能提供一个免费、开源的替代方案来取代专有的 Perforce。 Lore 针对结合代码与大型二进制资产（如纹理、3D 模型和音频文件）的项目进行了优化，并包含为艺术家提供的独占文件锁定等功能。

hackernews · regnerba · Jun 17, 14:30 · [社区讨论](https://news.ycombinator.com/item?id=48571081)

**背景**: 版本控制系统（VCS）跟踪文件随时间的变化。Git 在代码方面很流行，但对大型二进制文件效率低下；Perforce 是游戏开发中的行业标准，但它是专有的且复杂。Lore 旨在结合 Git 的开放性和 Perforce 的可扩展性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">Lore is a next-generation, open source revision control system</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System</a></li>
<li><a href="https://dev.epicgames.com/documentation/unreal-engine/lore-version-control-in-unreal-engine?lang=en-US">Lore Version Control in Unreal Engine - Epic Dev</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区普遍认为 Lore 是 Perforce 的有力挑战者，尤其适用于 Unreal Engine 开发。一些评论者指出 Git 的用户界面不友好和 Perforce 的复杂性，而另一些人则质疑 Lore 能否达到 Perforce 的成熟度和生态系统。

**标签**: `#version control`, `#game development`, `#open source`, `#scalability`, `#Perforce`

---

<a id="item-4"></a>
## [泄露文件显示 OpenAI 每年亏损数十亿美元](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

泄露的财务文件显示，尽管收入快速增长，但由于极高的运营成本和巨额研发支出，OpenAI 每年亏损数十亿美元。 这一发现引发了对 OpenAI 商业模式可持续性以及整个 AI 行业盈利路径的严重质疑，影响投资者、竞争对手和客户。 文件显示，销售、一般及行政费用占收入的 55%，非常高，而研发成本更是天文数字，表明即使收入增长，盈利仍遥不可及。

hackernews · greenchair · Jun 17, 21:31 · [社区讨论](https://news.ycombinator.com/item?id=48577208)

**背景**: OpenAI 是一家领先的人工智能研究和部署公司，以 ChatGPT 和 GPT-4 闻名。作为初创公司，它优先考虑快速增长和前沿研究而非短期盈利，但这些泄露突显了该战略的财务压力。

**社区讨论**: 社区评论存在分歧：一些人认为由于高运营成本和研发支出，亏损不可持续；而另一些人则指出收入快速增长，如果成本得到控制，有可能实现盈利。还有关于是否应将重点转向降低推理成本或继续 AGI 研究的争论。

**标签**: `#OpenAI`, `#financial analysis`, `#AI industry`, `#business model`, `#startup sustainability`

---

<a id="item-5"></a>
## [美国科学陷入危机：资金、签证、人才流失](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

美国科学陷入混乱，研究资金枯竭，签证限制阻碍外国人才，许多研究人员正在离开美国或放弃科研。 这场危机威胁到美国在科学和创新领域的领导地位，可能对国家的科研事业和经济竞争力造成长期损害。 文章指出科学与政治之间的契约破裂，拨款未获续期，签证限制阻碍了外国研究生的招聘，研究人员中弥漫着明显的紧张情绪。

hackernews · presspot · Jun 17, 09:54 · [社区讨论](https://news.ycombinator.com/item?id=48568058)

**背景**: 美国科学长期以来依赖联邦拨款和国际人才的稳定流入。近期的政策变化和资金削减破坏了这一体系，导致人才流失和研究界士气低落。

**社区讨论**: 评论者分享了因资金削减和签证问题而离开美国或减少工作时间的个人经历。许多人表示情况最近恶化，甚至资深科学家也在准备后备计划。

**标签**: `#science policy`, `#research funding`, `#US politics`, `#brain drain`

---

<a id="item-6"></a>
## [Adam 推出 CADAM：开源 AI CAD 工具，文本生成模型](https://github.com/Adam-CAD/CADAM) ⭐️ 8.0/10

Adam (YC W25) 发布了开源文本转 CAD 平台 CADAM，它通过基于代码的范式（OpenSCAD）从自然语言提示生成参数化 3D 模型。 这标志着向让 AI 成为机械设计主要媒介迈出了重要一步，可能降低快速原型制作的门槛，并使非专业人士也能创建 CAD 模型。 CADAM 通过 WebAssembly 编译的 OpenSCAD 和 Three.js 渲染完全在浏览器中运行，支持多种 LLM（Claude、Gemini、OpenAI），并输出 STL、SCAD 等格式。

hackernews · zachdive · Jun 17, 16:14 · [社区讨论](https://news.ycombinator.com/item?id=48572553)

**背景**: 传统的 CAD 软件（如 Fusion 360 或 SolidWorks）需要大量专业知识和手动建模。文本转 CAD 工具旨在从自然语言生成可编辑的 3D 几何体，类似于 AI 代码生成的工作方式。CADAM 采用代码即 CAD 的方法，生成可通过滑块调整的 OpenSCAD 脚本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/Adam-CAD/CADAM">GitHub - Adam-CAD/CADAM: CADAM is the open source text-to-CAD web application · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/CADAM">CADAM - Wikipedia</a></li>
<li><a href="https://sourceforge.net/projects/cadam.mirror/">CADAM download | SourceForge.net</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区反应不一：一些日常 CAD 用户表示兴奋，而工程师则对实际用例提出担忧，指出对于简单零件，手动建模通常比验证 AI 输出更快、更可靠。

**标签**: `#AI`, `#CAD`, `#open-source`, `#mechanical-design`, `#YC`

---

<a id="item-7"></a>
## [Tesco 因 Broadcom 定价迁移 4 万工作负载离开 VMware](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

英国最大的连锁超市 Tesco 正在将 4 万个服务器工作负载从 VMware 迁移出去，原因是 Broadcom 激进的定价和许可变更导致成本飙升 150%至 1000%。 此次迁移标志着大型企业开始大规模脱离 VMware，可能引发行业内的连锁反应，因为 Broadcom 收购后的策略正在疏远大客户。 Tesco 的新虚拟化软件与其现有的 Veeam 和 Zerto 备份工具不兼容，在迁移过程中带来了数据安全挑战。该公司未透露替代平台，但社区猜测可能是 Proxmox 或 Nutanix。

hackernews · Bender · Jun 17, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48576838)

**背景**: Broadcom 于 2023 年 11 月收购 VMware 后，立即用昂贵的订阅许可取代了永久许可，引入 72 核最低要求，并强制捆绑购买，导致价格上涨 150%至 1000%。这促使许多企业开始探索 Proxmox、Nutanix 或公有云等替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://vmwaremadesimple.com/articles/broadcom-vmware-licensing-changes-2026.html">Broadcom's VMware Licensing Changes in 2026: What Every Admin ...</a></li>
<li><a href="https://cloudinfra.blog/comprehensive-analysis-of-broadcoms-vmware-license-pricing-changes-and-their-impact/">Comprehensive Analysis of Broadcom's VMware License Pricing ...</a></li>
<li><a href="https://www.softwareseni.com/broadcom-vmware-pricing-changes-understanding-the-licensing-crisis-driving-migration/">Broadcom VMware Pricing Changes - Understanding the Licensing ...</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍支持 Tesco 的决定，许多人分享了自身对 Broadcom 的负面体验。有人指出 Broadcom 的激进策略实际上是在为 Proxmox 做宣传。也有人对大规模迁移的高昂成本和复杂性表示担忧。

**标签**: `#VMware`, `#Broadcom`, `#enterprise migration`, `#virtualization`, `#cloud`

---

<a id="item-8"></a>
## [RFC 10008 标准化 HTTP QUERY 方法](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008 于 2026 年 6 月 15 日发布，定义了一种新的 HTTP QUERY 方法，该方法安全、幂等且可携带请求体，填补了 HTTP 协议中长期存在的空白。 这种新方法为使用 POST 进行查询提供了标准化替代方案，支持安全的缓存和重试而无副作用，对 GraphQL API 和复杂搜索操作尤其有益。 QUERY 类似于 POST，但保证安全性和幂等性，意味着请求可以自动重复而无需担心状态变化。请求体包含在缓存键中，可能导致无界的缓存键。

hackernews · schappim · Jun 17, 10:51 · [社区讨论](https://news.ycombinator.com/item?id=48568502)

**背景**: HTTP GET 请求不能有请求体，而 POST 请求既不安全也不幂等，迫使开发人员使用 POST 进行需要请求体的查询，这破坏了缓存并导致重新提交警告。QUERY 方法通过提供带有请求体的安全、幂等方法解决了这个问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008: The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://blainsmith.com/articles/rfc-10008-http-query-method/">RFC 10008: The HTTP QUERY Method - Blain Smith</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，一个有力的示例会更有说服力，并讨论了将请求体包含在缓存键中的奇怪之处。有人想知道 HTML 表单是否会支持 QUERY 以避免重新提交警告，而另一些人提到他们多年来一直在 GET 中发送请求体。

**标签**: `#HTTP`, `#RFC`, `#protocol`, `#web`, `#caching`

---

<a id="item-9"></a>
## [Charity Majors：AI 要求更强的工程纪律](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors 认为，AI 使代码生成变得廉价且可丢弃，因此需要更强的工程纪律，而非更少。她将此转变比作从手工服务器宠物到不可变基础设施的过渡。 这一见解重新定义了 AI 对软件工程的影响，强调虽然代码变得更便宜，但对严谨的系统设计、测试和运维的需求反而增加。它挑战了 AI 会减少对熟练工程师需求的观念。 Majors 指出，代码行从被珍视和精心策划，一夜之间变得可丢弃和可重新生成。她将其与早期从服务器宠物到不可变基础设施的转变相类比，暗示需要类似的纪律加强。

rss · Simon Willison · Jun 17, 17:12

**背景**: Charity Majors 是知名工程师、CTO、Honeycomb 联合创始人，在可观测性和工程文化领域备受尊敬。她的论点基于一个观察：GitHub Copilot 和 Claude Code 等 AI 编程助手大幅降低了代码生成成本，将瓶颈从编写转移到验证和维护系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://charitydotwtf.substack.com/p/ai-demands-more-engineering-discipline">AI demands more engineering discipline. Not less</a></li>
<li><a href="https://perevillega.com/posts/2026-03-16-code-is-cheap-now/">Code Is Cheap Now, And That Changes Everything - Pere Villega</a></li>

</ul>
</details>

**标签**: `#ai-assisted-programming`, `#software-engineering`, `#generative-ai`, `#economics-of-code`

---

<a id="item-10"></a>
## [AI 模型出口管制损害美国网络防御](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

美国政府于 2026 年 6 月 13 日对 Anthropic 的 Claude Fable 5 和 Mythos 5 模型实施出口管制，意外地阻止了要求模型修复含有已知漏洞代码的合法安全研究。 这项政策反而削弱了美国网络防御，因为它阻止防御者使用 AI 来查找、修复和测试安全补丁，而制造漏洞的能力与防御性漏洞修复密不可分。 研究人员使用了含有已知 CVE 的开源代码和故意植入的漏洞，要求 Fable 5“修复此代码”——这一防御性请求触发了出口管制禁令。Kate Moussouris 确认，所谓的“越狱”仅仅是要求模型修复漏洞。

rss · Simon Willison · Jun 16, 05:20

**背景**: AI 模型出口管制旨在防止对手利用先进 AI 进行网络攻击。然而，使模型能够生成漏洞利用代码的相同能力对于漏洞修复和补丁验证等防御性安全任务至关重要。美国工业和安全局（BIS）向 Anthropic 发出“知情”信函，要求与外国人共享模型需获得出口许可证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.aimadetools.com/blog/claude-fable-5-banned-us-export-controls">Claude Fable 5 Banned — US Government Export Controls ...</a></li>
<li><a href="https://cybersecuritynews.com/claude-mythos-5-and-fable-5-export/">U.S. Commerce Dept Imposes Export Controls on Anthropic's ...</a></li>
<li><a href="https://www.gtlaw.com/en/insights/2026/6/ai-company-anthropic-suspends-access-to-claude-fable-5-claude-mythos-5-following-us-export-control-directive">AI Company Anthropic Suspends Access to Claude Fable 5 ...</a></li>

</ul>
</details>

**社区讨论**: 社区讨论强调了该政策的荒谬性，指出非技术决策者将防御性漏洞修复与攻击能力混为一谈。评论者强调，移除修复漏洞的能力将使模型对安全毫无用处，出口管制适得其反。

**标签**: `#AI policy`, `#export controls`, `#cybersecurity`, `#AI safety`, `#open source`

---

<a id="item-11"></a>
## [GitHub Copilot 2026 年 6 月起改为按用量计费](https://t.me/zaihuapd/42003) ⭐️ 8.0/10

GitHub 宣布从 2026 年 6 月 1 日起，所有 GitHub Copilot 套餐将转为按用量计费，用量以 GitHub AI Credits 计算。仍处于传统年度计划中的老用户可继续沿用旧计费模式直到计划到期。 从固定费率转向按用量计费可能会显著增加重度 Copilot 用户的成本，尤其是依赖 GPT-5.5 等昂贵模型的用户。这也使 GitHub Copilot 与典型的云 API 计费模式保持一致，可能影响开发者和组织对 AI 编程助手的预算规划。 在新系统下，每个套餐包含每月 GitHub AI Credits 额度，付费套餐可额外购买用量。在公布的模型乘数表中，GPT-5.5 模型的单次请求计费乘数为 57 倍，但促销定价最初设为 7.5 倍。

telegram · zaihuapd · Jun 17, 03:16

**背景**: GitHub Copilot 是一款 AI 驱动的代码补全工具，可在开发者输入时建议代码片段和函数。此前，Copilot 采用每用户固定月费（例如 Copilot Business 为 19 美元/用户/月），并对高级请求有限制。新的按用量计费引入了 AI Credits，不同模型根据其计算成本以不同速率消耗 Credits。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/">GitHub Copilot is moving to usage-based billing</a></li>
<li><a href="https://docs.github.com/en/copilot/reference/copilot-billing/models-and-pricing">Models and pricing for GitHub Copilot - GitHub Docs</a></li>
<li><a href="https://github.blog/changelog/2026-04-24-gpt-5-5-is-generally-available-for-github-copilot/">GPT-5.5 is generally available for GitHub Copilot</a></li>

</ul>
</details>

**标签**: `#GitHub Copilot`, `#pricing`, `#AI coding assistant`, `#billing`

---

<a id="item-12"></a>
## [中国将科创板 IPO 标准扩展至 AI 与硬科技](https://mp.weixin.qq.com/s/ywLPXkSlqY9S5Vwp8G5saA) ⭐️ 8.0/10

中国证监会主席吴清在 2026 陆家嘴论坛上宣布，科创板第五套上市标准的适用范围将扩大至人工智能、量子科技、生物制造和具身智能等领域。证监会还将推出储架发行等再融资改革，并适时发布规范资本市场人工智能的指导意见。 这一政策转变大幅拓宽了 AI 和硬科技企业的 IPO 准入渠道，可能重塑中国科技行业的资本配置。它标志着政府对战略性新兴产业的强力支持，并可能加速尚未盈利的创新企业上市。 第五套标准此前主要针对生物医药企业，现扩展至量子科技、生物制造和具身智能。证监会还表示将严查借科技之名蹭热点、炒概念等违法违规行为。目前 A 股科技板块市值占比已超三成，市值超千亿的上市公司中科技企业占比达 45%。

telegram · zaihuapd · Jun 17, 08:30

**背景**: 科创板是中国于 2019 年设立的、对标纳斯达克的科技企业板块。其第五套上市标准允许尚未盈利但研发投入和市值达标的企业上市，此前主要被生物医药企业使用。具身智能是指能够与物理世界交互的 AI 系统，例如人形机器人。储架发行是一种发行人一次注册、分次发行的再融资机制。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://macrochina.com.cn/news_speed/hgjj/20250627123825.shtml">macrochina.com.cn/news_speed/hgjj/20250627123825.shtml</a></li>
<li><a href="https://www.caict.ac.cn/kxyj/qwfb/bps/202408/P020240830312499650772.pdf">caict.ac.cn/kxyj/qwfb/bps/202408/P020240830312499650772.pdf</a></li>
<li><a href="https://baike.baidu.com/item/储架发行制度/1648322">储架发行制度_百度百科</a></li>

</ul>
</details>

**标签**: `#AI`, `#IPO`, `#China`, `#regulation`, `#hard tech`

---

<a id="item-13"></a>
## [微软借 OpenAI 模型在华扩张 AI 业务](https://www.bloomberg.com/news/articles/2026-06-17/microsoft-s-china-ai-business-grows-on-openai-model-sales) ⭐️ 8.0/10

微软通过 Azure 向中国科技公司销售 OpenAI 的 AI 模型，在华业务快速扩张，字节跳动是其最大客户，每年在微软 AI 和云服务上的投入预计超 10 亿美元。 这一进展引发了重大的地缘政治和安全担忧，美国立法者和 OpenAI 担心中国公司可能进行技术转移和模型蒸馏，从而削弱美国在 AI 领域的竞争优势。 Azure 在中国的 AI 收入连续两年实现约四倍和三倍增长，微软声称只向成熟企业而非个人开发者销售模型，且模型托管在境外数据中心，客户需通过互联网访问。

telegram · zaihuapd · Jun 18, 01:06

**背景**: 模型蒸馏是一种让较小的“学生”模型从较大的“教师”模型中学习的技术，可能使中国公司无需直接访问就能复制 OpenAI 的能力。微软通过与世纪互联合作在中国运营 Azure 以遵守当地法规，但 OpenAI 模型托管在境外以解决安全问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/china/overview-operations">Microsoft Azure in China</a></li>
<li><a href="https://openai.com/index/update-on-safety-and-security-practices/">An update on our safety & security practices - OpenAI</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#OpenAI`, `#AI regulation`, `#China`, `#cloud computing`

---

<a id="item-14"></a>
## [美国推迟将 DeepSeek 及百余家中国公司列入黑名单](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 7.0/10

据知情人士透露，美国已决定暂缓将中国 AI 初创公司 DeepSeek、内存芯片制造商 CXMT 等 100 多家被认定为国家安全风险的公司列入贸易黑名单。 这一决定标志着美中科技紧张局势可能有所缓和，但也引发了关于执法力度以及对 AI 发展影响的疑问。延迟可能影响 AI 模型和芯片供应链的竞争格局。 该黑名单（即实体清单）限制美国公司向列入清单的实体出售商品和服务，但不禁止从它们那里购买。DeepSeek 的模型采用开放权重，并因出口限制而使用较弱的 AI 芯片进行训练，因此成本效益较高。

hackernews · giuliomagnifico · Jun 17, 03:55 · [社区讨论](https://news.ycombinator.com/item?id=48565498)

**背景**: DeepSeek 是一家成立于 2023 年的中国 AI 公司，其开发的 DeepSeek-R1 模型以极低的成本与 OpenAI 的 GPT-4 相媲美。其成功被称为美国 AI 领域的“斯普特尼克时刻”，威胁到英伟达的市场主导地位。实体清单是美国用于拒绝向被视为国家安全风险的实体出口的贸易限制工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.cnbc.com/2026/06/17/us-deepseek-blacklist-cxmt-national-security-risks-.html">U.S. holds off blacklisting China's DeepSeek, more than 100 ...</a></li>
<li><a href="https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/">Exclusive: US holds off blacklisting China's DeepSeek, more ...</a></li>

</ul>
</details>

**社区讨论**: 评论观点不一：一些用户赞赏 DeepSeek 的性价比和性能，而另一些则批评美国的黑名单政策虚伪或难以执行。关于实体清单是否能有效限制中国 AI 公司存在争议，因为后者对美国商品的依赖有限。

**标签**: `#AI`, `#geopolitics`, `#DeepSeek`, `#regulation`, `#US-China`

---

<a id="item-15"></a>
## [在 EC2 上运行 Firecracker 虚拟机，浏览器启动不到 1 秒](https://browser-use.com/posts/firecracker-browser-infra) ⭐️ 7.0/10

Browser-use.com 描述了一种在 EC2 实例上运行 Firecracker 微虚拟机的方法，可在不到一秒内启动隐身浏览器，反机器人规避率达到 81%。 该方法通过结合快速启动和高反机器人规避能力，显著改进了用于网页抓取和测试的浏览器自动化，但也引发了关于绕过网站保护的伦理问题。 常规 EC2 实例上的嵌套虚拟化自 2026 年 2 月才成为可能，此前需要使用裸金属实例。该系统利用 Firecracker 的最小设备模型来减少攻击面和内存占用。

hackernews · gregpr07 · Jun 16, 15:15 · [社区讨论](https://news.ycombinator.com/item?id=48556561)

**背景**: Firecracker 是 AWS 开发的开源虚拟化技术，可创建启动快速且隔离性强的轻量级微虚拟机。网站的反机器人措施通过指纹识别和行为分析来检测无头浏览器，使得隐身自动化变得困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://firecracker-microvm.github.io/">Firecracker</a></li>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker - microvm / firecracker : Secure and fast microVMs...</a></li>

</ul>
</details>

**社区讨论**: 评论者对这种绕过反机器人措施的技术提出了伦理担忧，而其他人则指出技术限制，例如嵌套虚拟化最近才在常规 EC2 上可用。一些人建议使用 AWS Lambda 或 Lightpanda 浏览器等替代方案来实现更简单的设置。

**标签**: `#Firecracker`, `#EC2`, `#browser automation`, `#anti-bot`, `#virtualization`

---

<a id="item-16"></a>
## [AI 模型在“最后特工生存”游戏基准测试中一决高下](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 7.0/10

OpenRouter 上的一篇博客文章在“最后特工生存”游戏中对 Claude 和 Grok 等 AI 模型进行了基准测试，结果显示 DeepSeek V4 Flash 在成本效率上胜出，而 Grok 虽然性能提升，但引发了关于静默模型路由的担忧。 该基准测试突显了 AI 模型在实时决策场景中成本与性能的权衡，这对于在成本敏感型应用中部署 AI 代理的开发者至关重要。 实验运行了 30 局游戏，总成本为 482 美元，避免了像 Opus 4.7 或 GPT-5.5 这样的前沿模型，否则成本将约为 3000 美元。DeepSeek V4 Flash 是一个混合专家模型，总参数 284B，激活参数 13B，展现了卓越的成本效率。

hackernews · Usu · Jun 17, 21:00 · [社区讨论](https://news.ycombinator.com/item?id=48576824)

**背景**: “最后特工生存”游戏是一种大逃杀模式，AI 代理自主竞争，做出移动、资源收集和战斗等决策。该基准测试考验模型在压力下推理和行动的能力。DeepSeek V4 Flash 是 DeepSeek V4 系列的预览版，专为高效推理设计，支持 100 万 token 的上下文窗口。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek-v4-flash - ollama.com</a></li>

</ul>
</details>

**社区讨论**: 评论者称赞 DeepSeek V4 Flash 的成本效率，一位用户称其为“编码怪兽”。然而，有人担忧 Grok 将模型从 4.1 静默路由到 4.3 并提高价格，这被批评为不良做法。另一条评论指出“每次击杀成本”这个黑暗短语与 AI 公司惊人地相关。

**标签**: `#AI`, `#benchmark`, `#cost efficiency`, `#language models`, `#gaming`

---

<a id="item-17"></a>
## [大众汽车屏蔽 GrapheneOS 用户使用其应用](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 7.0/10

大众汽车将其 API 锁定为仅接受 Play Protect 认证设备，从而有效阻止了注重隐私的基于 Android 的操作系统 GrapheneOS 的用户使用其官方应用。 此举限制了用户的选择和隐私，因为 GrapheneOS 用户被迫要么放弃该操作系统，要么失去对大众应用的使用权，凸显了汽车行业中对设备兼容性的企业控制日益增强。 API 锁定还扼杀了依赖大众 API 的社区驱动项目，例如 Home Assistant 集成，而官方应用被批评包含 60% 的广告和 30% 的功能。

hackernews · microtonal · Jun 17, 15:04 · [社区讨论](https://news.ycombinator.com/item?id=48571526)

**背景**: GrapheneOS 是一个基于 Android 的开源移动操作系统，注重安全和隐私，常被希望避免使用谷歌服务的用户使用。Play Protect 认证是谷歌验证设备是否符合兼容性标准并包含专有谷歌应用的流程。通过要求 Play Protect 认证，大众确保其应用仅在拥有完整谷歌软件栈的设备上运行。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://support.google.com/googleplay/answer/7165974?hl=en">Check & fix Play Protect certification status - Google Play Help</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了沮丧和失望，用户如 mooo99 推迟购车，aka13_404 指出社区集成功能的丧失。一些人认为这是汽车公司限制用户自由的更广泛趋势的一部分。

**标签**: `#privacy`, `#automotive`, `#Android`, `#GrapheneOS`, `#API access`

---

<a id="item-18"></a>
## [MicroUI：用 ANSI C 编写的微型即时模式 GUI 库](https://github.com/rxi/microui) ⭐️ 7.0/10

MicroUI 是一个用 ANSI C 编写的极简、可移植的即时模式 UI 库，旨在轻松集成到能够显示文本和处理鼠标输入的项目中。 其极致的简洁性和可移植性使其非常适合嵌入式系统、游戏开发以及其他资源受限的环境，在这些场景中，完整的 GUI 框架显得过于臃肿。 该库被认为有些被遗弃，存在一个已知的绘制调用迭代器中的指针未对齐访问错误，在 Zig 等环境中可能导致崩溃。

hackernews · peter_d_sherman · Jun 17, 12:04 · [社区讨论](https://news.ycombinator.com/item?id=48569205)

**背景**: 即时模式 GUI（IMGUI）是一种设计模式，UI 元素每帧直接从代码中绘制和处理，而不在帧之间保留状态。这与维护持久化控件树的保留模式 GUI 形成对比。ANSI C 指的是标准化的 C 语言版本（C89/C90），可确保跨编译器和平台的最大可移植性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Immediate_mode_GUI">Immediate mode GUI</a></li>
<li><a href="https://en.wikipedia.org/wiki/ANSI_C">ANSI C</a></li>

</ul>
</details>

**社区讨论**: 社区成员称赞 MicroUI 的简洁性和易集成性，有用户称其为个人玩具项目的首选。但也有人担心其被遗弃的状态和指针未对齐错误，部分用户已 fork 该项目以解决问题。

**标签**: `#C`, `#UI Library`, `#Immediate Mode GUI`, `#Portability`, `#Open Source`

---

<a id="item-19"></a>
## [Photobucket 要求支付 5 美元才能取回你的照片](https://www.lutr.dev/want-your-images-back-sure-that-ll-be-5-dollars) ⭐️ 7.0/10

Photobucket 向用户收取 5 美元的订阅费，才能在其账户删除前下载自己的图片，这实质上是在劫持用户数据。 这种做法引发了关于数据可移植性和企业道德的严重担忧，因为用户被迫付费才能访问自己的内容，可能为云存储服务树立一个危险的先例。 即使只想取回几张旧照片的用户也需要支付这笔费用，而且账户删除通知并未事先警告这一收费。

hackernews · lutr · Jun 17, 13:05 · [社区讨论](https://news.ycombinator.com/item?id=48569954)

**背景**: 数据可移植性是指用户应能轻松地在不同服务之间转移其数据。Photobucket 曾是一个流行的图片托管网站，此前因盈利策略受到批评，例如 2017 年要求每年支付 99 美元才能在第三方网站嵌入图片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Photobucket">Photobucket - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_portability">Data portability</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了愤怒，有人建议发起退款，也有人指出关闭账户可能提供免费下载选项。其他人则争论这是企业贪婪还是失败服务的必要生存之举。

**标签**: `#data portability`, `#cloud storage`, `#consumer rights`, `#tech ethics`

---

<a id="item-20"></a>
## [Datasette 1.0a34 新增行级增删改界面](https://simonwillison.net/2026/Jun/16/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a34 在网页界面中直接新增了插入、编辑和删除行的功能，可在表格页面和行页面上使用。 这一期待已久的功能为 Datasette 界面带来了基本的增删改操作，使非技术用户更易使用，并减少对外部工具或 SQL 查询的依赖。 该功能受 Datasette Agent 启发，后者已支持 SQL 写入操作，凸显了常规界面中的缺失。编辑和删除操作也可在行页面上使用。

rss · Simon Willison · Jun 16, 21:31

**背景**: Datasette 是一个用于探索和发布数据的开源工具，主要与 SQLite 数据库配合使用。此前，修改数据需要 SQL 查询或外部插件（如 datasette-write-ui）。此 alpha 版本原生集成了增删改功能，向 1.0 稳定版迈进。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and analyze data in SQLite</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**标签**: `#datasette`, `#open-source`, `#data management`, `#release`

---

<a id="item-21"></a>
## [Georgi Gerganov 认可 Qwen3.6-27B 用于本地编程](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 7.0/10

llama.cpp 的创建者 Georgi Gerganov 公开认可 Qwen3.6-27B 模型是一款非常强大的本地编程助手，并表示他几乎每天都在自己的 M2 Ultra 和 RTX 5090 系统上使用它。他描述了自己使用 pi agent 框架的轻量级设置，采用精简配置和简短的系统提示词。 来自本地 LLM 基础设施关键人物的认可，验证了 Qwen3.6-27B 作为开发者实用工具的价值，可能加速本地编程助手的采用。这凸显了在消费级硬件上运行强大模型的可行性日益增强，减少了对云端 AI 服务的依赖。 Qwen3.6-27B 是一个稠密的 27B 参数模型，在 SWE-bench Verified 等主要编程基准测试上超越了更大的 Qwen3.5-397B-A17B（77.2% 对比更低）。Gerganov 使用 pi agent 框架的离线模式（pi -nc --offline），并配合来自 llama.cpp 仓库的自定义系统提示词。

rss · Simon Willison · Jun 16, 16:04

**背景**: 本地 LLM 允许开发者在自己的硬件上运行 AI 模型，无需将数据发送到外部服务器，从而增强隐私并降低延迟。Qwen3.6-27B 是阿里巴巴 Qwen 团队近期推出的模型，针对编程任务进行了优化。pi agent 是一个基于终端的极简编程 agent 框架，支持工具使用和文件编辑。由 Gerganov 创建的 llama.cpp 是一个流行的开源库，用于在消费级硬件上高效运行 LLM。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://qwen.ai/blog?id=qwen3.6-27b">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://pi.dev/">Pi Coding Agent</a></li>

</ul>
</details>

**标签**: `#local LLM`, `#coding assistant`, `#Qwen`, `#llama.cpp`, `#AI tools`

---

<a id="item-22"></a>
## [Anthropic 企业 AI 市场份额首超 OpenAI](https://techcrunch.com/2026/06/16/anthropics-latest-feud-with-the-trump-admin-may-actually-help-it-sales-data-suggests/) ⭐️ 7.0/10

根据 Ramp 数据，2026 年 5 月，Anthropic 的企业 AI 订阅份额达到 41%，超过 OpenAI 的 39.5%，尽管特朗普政府以出口管制为由要求 Anthropic 下架其最新的 Mythos 5 和 Fable 5 模型。 这标志着企业 AI 市场的重大转变，OpenAI 长期占据主导地位，同时表明监管冲突可能反而通过提升品牌知名度和企业客户信任来促进销售。 数据来自 Ramp 的 AI Index，追踪超过 7 万家美国企业的支出；Anthropic 被国防部列为供应链风险的月份，其企业采用率最高，而模型下架对 IPO 的潜在影响仍不确定。

telegram · zaihuapd · Jun 17, 09:30

**背景**: Anthropic 是一家 AI 安全公司，开发 Claude 系列模型。2026 年 6 月，它发布了两个高级模型：Claude Mythos 5（一个 10 万亿参数模型）和 Claude Fable 5（一个更安全的通用版本）。然而，特朗普政府以出口管制为由要求下架，担心非美国用户访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ramp.com/data/ai-index">Ramp AI Index</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**标签**: `#AI`, `#Enterprise`, `#Market Share`, `#Regulation`, `#Anthropic`

---

<a id="item-23"></a>
## [微信支付推出 AI 专属卡，每笔消费需本人授权](https://mp.weixin.qq.com/s/WJSr9J0-7LWx2haEZGLmXw) ⭐️ 7.0/10

微信支付于 2026 年 6 月 17 日正式推出 AI 专属卡，用户可通过 AI 智能体进行消费，每笔交易需本人授权。该功能首先接入腾讯企业级智能体 WorkBuddy，通过美团生活助手提供服务。 这标志着 AI 智能体支付迈出重要一步，通过资金隔离和每笔授权解决了安全顾虑。它可能在保持用户控制权的同时加速 AI 驱动商业的普及，影响更广泛的金融科技和 AI 生态。 AI 专属卡与微信支付主账户完全隔离，用户可自行转入资金并设置使用范围。每笔消费必须经过本人最终确认，AI 无法越过授权动用资金。

telegram · zaihuapd · Jun 17, 11:32

**背景**: AI 智能体支付允许智能体在预设规则下代表用户发起并完成交易。微信支付的方案紧随竞争对手支付宝之后，后者在 2026 年 5 月报告了 3 亿笔 AI 支付交易。AI 专属卡提供专用余额和授权机制，防止滥用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260617A0806300">微信支付发布“AI专属卡”，AI可以帮你花钱了_腾讯新闻</a></li>
<li><a href="https://news.qq.com/rain/a/20260617A05V4J00">微信支付全新上线 AI 专属卡功能_腾讯新闻</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2026-06-17/doc-inictaer7031010.shtml">微信支付正式发布AI专属卡！WorkBuddy率先接入：单独余额 不怕乱花钱_...</a></li>

</ul>
</details>

**标签**: `#AI`, `#Fintech`, `#WeChat Pay`, `#Payment`, `#Security`

---

<a id="item-24"></a>
## [运营商词元套餐成本高昂，开发者直呼用不起](https://mp.weixin.qq.com/s/UsHNZNMov1kwFQKAVsQHNw) ⭐️ 7.0/10

记者实测发现，15 元含 600 万词元的套餐，输入一句“你好”就消耗约 5 万 Token，不到一小时即用完。开发者测算月成本约 1000 元，是主流 AI 订阅费用的五六倍。 这表明中国运营商的词元计费模式目前不切实际且缺乏竞争力，可能阻碍开发者对 AI 的采用。它凸显了传统电信计费与 AI 生态系统需求之间的差距。 词元套餐包含运营商自研模型以及 DeepSeek-V4-Flash、GLM-5 等第三方模型。线下营业厅和线上客服对新套餐普遍不熟，落地执行不佳。

telegram · zaihuapd · Jun 17, 12:25

**背景**: 词元计费是大模型的标准计费方式，每个词元代表处理的一个文本单位。运营商正试图通过提供词元套餐进入 AI 市场，类似于销售流量套餐，但面临云厂商和专业 AI 平台的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wallstreetcn.com/articles/3774930">15元买数百万Token...</a></li>
<li><a href="http://m.ce.cn/cy/202606/t20260612_3027162.shtml">词 元 套 餐 便利数字生活_中国经济网</a></li>
<li><a href="https://www.tmtpost.com/8007698.html">AI算力消耗不再管不住， 词 元 服务迎新玩家-钛媒体官方网站</a></li>

</ul>
</details>

**社区讨论**: 在 Telegram 频道中，开发者对高昂成本和糟糕的实施表示不满，有人称这些套餐为“骗局”，并质疑运营商对 AI 需求的理解。情绪普遍负面，很少有人看到当前产品的价值。

**标签**: `#AI pricing`, `#telecom`, `#token economy`, `#China`, `#developer experience`

---

<a id="item-25"></a>
## [OpenAI Codex 现支持自定义第三方模型提供者](https://developers.openai.com/codex/config-advanced) ⭐️ 7.0/10

OpenAI Codex 新增了对自定义第三方模型提供者的支持，用户可以通过配置文件接入 Amazon Bedrock、Azure 以及本地 Ollama 等外部模型。 这一更新极大地提升了开发者的灵活性，使他们能够从更广泛的 AI 模型中选择，并将其无缝集成到编码工作流中，减少了对 OpenAI 自身模型的依赖。 用户需在配置文件中定义提供者名称、接口地址和 API 密钥，并可通过命令行覆盖部分设置，以便在终端环境中快速切换模型。

telegram · zaihuapd · Jun 17, 13:58

**背景**: OpenAI Codex 是一款 AI 辅助编程工具，此前仅支持 OpenAI 的专有模型。此次更新允许开发者使用本地模型（如 Ollama，可本地运行模型以降低延迟和成本）或云服务（如 Amazon Bedrock，提供多种基础模型访问）。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://medium.com/@bluudit/deploy-llms-locally-with-ollama-your-complete-guide-to-local-ai-development-ba60d61b6cea">Deploy LLMs Locally with Ollama: Your Complete Guide to Local AI Development | by Vijay Kumar Maurya | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Bedrock">Amazon Bedrock - Wikipedia</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html">Overview - Amazon Bedrock</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#AI`, `#model-providers`, `#developer-tools`

---