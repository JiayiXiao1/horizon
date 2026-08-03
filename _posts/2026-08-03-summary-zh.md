---
layout: default
title: "Horizon Summary: 2026-08-03 (ZH)"
date: 2026-08-03
lang: zh
---

> From 35 items, 17 important content pieces were selected

---

1. [OpenAI Astra 模型在十项长期数学难题上取得突破](#item-1) ⭐️ 9.0/10
2. [Kakehashi：在 Linux ARM 上运行 macOS 二进制文件](#item-2) ⭐️ 8.0/10
3. [eBay 骚扰活动导致 5600 万美元赔偿及监禁判决](#item-3) ⭐️ 8.0/10
4. [AI 巨头反对开放权重模型限制](#item-4) ⭐️ 8.0/10
5. [中国在联合国峰会上向全球南方推广开放权重 AI 模型](#item-5) ⭐️ 8.0/10
6. [微软确认今年推出 Copilot「超级应用」](#item-6) ⭐️ 8.0/10
7. [Karpathy 点赞 sqliteai/waste：从 NVMe 流式加载 Kimi K3](#item-7) ⭐️ 7.0/10
8. [Karpathy 的 AI 鹈鹕引发关于物理世界基准的讨论](#item-8) ⭐️ 7.0/10
9. [F*：一种通用的面向证明的编程语言](#item-9) ⭐️ 7.0/10
10. [EA 以 550 亿美元被沙特财团收购，交易下周完成](#item-10) ⭐️ 7.0/10
11. [长鑫存储发布 DDR5 和 LPDDR5X，DDR5 速率达 8000Mbps](#item-11) ⭐️ 7.0/10
12. [AI 芯片数量每 9 个月翻番，预计 2028 年达 2 亿颗](#item-12) ⭐️ 7.0/10
13. [苹果限制漏洞报告以遏制 AI 生成的垃圾信息](#item-13) ⭐️ 7.0/10
14. [中国 AI 框架以 90%准确率检测比特币洗钱](#item-14) ⭐️ 7.0/10
15. [中国发布公共预警短信强制性国家标准](#item-15) ⭐️ 7.0/10
16. [深海热液喷口附近 92%动物体内检出微塑料](#item-16) ⭐️ 7.0/10
17. [美国多州拟取消数据中心税收优惠，AI 基础设施成本上升](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI Astra 模型在十项长期数学难题上取得突破](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI 宣布其下一代模型 Astra 的内部版本在十个长期未解决的数学与理论计算机科学问题上取得新成果，涵盖高维球体堆积、非索菲克群以及 Connes 刚性猜想反例等。这些证明已在 Lean 中形式化验证，每个问题的 token 成本不到 2000 美元。 这标志着 AI 辅助数学研究的一个重要里程碑，表明 AI 能够为解决数十年未获进展的问题做出贡献。这可能加速数学和理论计算机科学领域的发现速度，并引发关于成果归属以及 AI 在研究中的角色的重要讨论。 这些问题包括高维球体堆积、非索菲克群的存在性、Connes 刚性猜想反例、算术电路下界、量子并行重复、最近向量问题的难度以及多色 Ramsey 数等。OpenAI 已在 GitHub 仓库中发布了 Lean 4 形式化证明和描述解决方案的论文，但未公开所使用的提示词。

telegram · zaihuapd · Aug 1, 07:59

**背景**: 球体堆积是数学中的经典问题，研究如何在给定维度中排列球体以最大化其占据的空间比例。目前仅在 1、2、3、8 和 24 维中已知最优解，其他维度的问题仍未解决。Lean 形式化验证是一种使用计算机检查的证明助手来证明数学陈述的方法，确保其正确性。这些成果是 AI 用于数学研究的更广泛趋势的一部分，正如陶哲轩提出的“大数学”概念所强调的那样。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/克卜勒猜想">克卜勒猜想 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1571316.htm">OpenAI下一代模型Astra：10... - cnBeta.COM</a></li>
<li><a href="https://news.marsbit.co/20260802090912297284.html">突发！ OpenAI下一代AI攻克10项菲尔兹奖级难题 | Mars Finance</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论既包含惊叹也包含怀疑。一些评论者对 AI 在数学中的潜力表示兴奋，而另一些人则质疑这些成果的重要性以及提示词缺乏透明度的问题。还有讨论将这一事件比作数学界的“深蓝时刻”，与著名的国际象棋人机大战相类比。

**标签**: `#AI`, `#mathematics`, `#OpenAI`, `#formal verification`, `#research`

---

<a id="item-2"></a>
## [Kakehashi：在 Linux ARM 上运行 macOS 二进制文件](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi，一个实验性的用户态翻译层，现已成功在 Linux ARM 上运行 macOS CLI 二进制文件，并提供了 7-Zip、curl 和 Xcode Tools Git 的工作原型。该项目在 Linux aarch64 上加载 Darwin Mach-O 二进制文件，并翻译 BSD 系统调用，无需 JIT。 该项目解决了跨操作系统二进制兼容性方面的重大技术挑战，有望使 macOS 应用程序在 Linux ARM 硬件上原生运行。它可能通过提供对 macOS 专属工具和应用程序的访问来扩展 Linux 生态系统，类似于 Wine/Proton 对 Windows 应用程序所做的那样。 当前实现以 CLI 为主，没有 JIT，性能仍低于原生执行——例如，7-Zip 的运行速度大约慢 5.2 倍。该项目映射了一个独立的 libSystem 并翻译 BSD 系统调用，可以通过 cargo install kakehashi 安装。

hackernews · vlad_kalinkin · Aug 2, 16:26 · [社区讨论](https://news.ycombinator.com/item?id=49145937)

**背景**: macOS 二进制文件使用 Mach-O 格式，Linux 原生不支持该格式。Darling 项目是一个更全面的解决方案，旨在 Linux 上运行 macOS 应用程序，并且有一个开放的 ARM64 支持 PR。Kakehashi 采取了不同的、仅用户态的方法，专注于 CLI 二进制文件，避免内核级修改。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie-project/ kakehashi : Userspace macOS translation layer for Linux ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区对该项目的潜力充满热情，一些人将其与 Wine/Proton 相提并论，并建议与 Darling 项目合作。其他人则持谨慎乐观态度，指出该项目仍处于早期阶段，并对其未来方向表示好奇，例如支持音频插件的 AU 二进制文件。

**标签**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#userspace`

---

<a id="item-3"></a>
## [eBay 骚扰活动导致 5600 万美元赔偿及监禁判决](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

eBay 已同意向大卫和伊娜·斯坦纳夫妇支付 5600 万美元，这对夫妇曾是 eBay 安全团队策划的骚扰活动的目标。包括吉姆·鲍在内的多名前安全高管被判处监禁，其中鲍被判 57 个月。 此案凸显了严重的企业问责问题，显示一家大型科技公司的安全团队如何滥用权力针对批评者。它引发了对企业安全部门监督和道德行为的质疑，可能促使其他公司审查其做法。 骚扰活动包括发送令人不安的包裹、监视和威胁。eBay 安全团队的七名成员（包括前警察队长）参与其中，判决从已服刑期到 57 个月监禁不等。

hackernews · JumpCrisscross · Aug 2, 19:19 · [社区讨论](https://news.ycombinator.com/item?id=49147435)

**背景**: eBay 是一个全球电子商务平台，用户可以在上面买卖商品。斯坦纳夫妇发布了一份批评 eBay 的通讯，据称引发了骚扰。此案凸显了企业安全团队在针对被认为对公司声誉构成威胁的对象时，可能超越法律和道德界限。

**社区讨论**: 评论者表示怀疑骚扰仅限于一对夫妇，认为其他批评者可能也受到针对。一些人质疑涉案前警察的行为，另一些人则指出 eBay 的高额卖家费用是另一个问题。

**标签**: `#eBay`, `#harassment`, `#corporate accountability`, `#legal`, `#security`

---

<a id="item-4"></a>
## [AI 巨头反对开放权重模型限制](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

2026 年 7 月下旬，微软、英伟达、亚马逊、OpenAI 等 230 多家公司签署公开信，倡导开放权重 AI 模型，以应对美国政府可能的限制。Anthropic 拒绝签署并发布了自己的立场，另有 1324 名 AI 员工签署公开信呼吁放缓前沿 AI 发展。 这一协调的行业行动可能影响美国 AI 监管，平衡创新与安全担忧。争论凸显了支持开放模型的公司与担心滥用和国家安全问题之间的分歧日益扩大。 微软主导的公开信明确支持蒸馏技术，即模型利用其他模型的输出进行训练，这被一些人视为助长抄袭。Anthropic 在 CEO Dario Amodei 的领导下回应，警告威权政府可能构建强大 AI，并呼吁打击工业规模的蒸馏操作，同时否认主张禁止开放权重模型。

rss · Simon Willison · Aug 2, 04:16

**背景**: 开放权重模型是指公开其训练参数的 AI 模型，允许开发者运行、修改和审计，而封闭模型只能通过 API 访问。这一争论是更广泛的 AI 安全、竞争和国家安全政策讨论的一部分，特别是在中美竞争的背景下。

**标签**: `#AI policy`, `#open-weight models`, `#regulation`, `#industry`, `#Simon Willison`

---

<a id="item-5"></a>
## [中国在联合国峰会上向全球南方推广开放权重 AI 模型](https://www.semafor.com/article/07/28/2026/token-diplomacy-how-china-is-shaping-the-worlds-ai-future) ⭐️ 8.0/10

7 月底在日内瓦联合国“智能向善”峰会上，中国代表团向巴基斯坦、俄罗斯、赞比亚等全球南方国家推介中国开放权重 AI 模型。阿里云架构师王坚表示，中国 AI 可以像能源一样成为其他国家发展的“基石”。 此举将中国定位为美国闭源 AI 模型的替代选择，可能塑造全球 AI 基础设施和标准。这可能增强中国在发展中国家中的地缘政治影响力，并造成对中国技术的依赖，挑战美国在 AI 领域的主导地位。 美国国务院对此表示担忧，警告此类举措可能导致对中国基础设施和标准的依赖。值得注意的是，美方前沿实验室及特朗普政府官员明显缺席峰会，凸显了地缘政治分歧。

telegram · zaihuapd · Aug 1, 10:06

**背景**: 开放权重模型公开训练好的参数，任何人都可以下载、使用或微调，无需重新训练，但不一定公开完整训练代码和数据。这与 OpenAI 等闭源模型形成对比，后者保持权重专有。中国的“词元外交”策略旨在以更低成本输出 AI 基础设施，包括培训和支持，以赢得全球南方的影响力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.wbolt.com/open-weight-models.html">开放源码和开放权重模型之间有何区别？</a></li>
<li><a href="https://www.sina.cn/news/detail/5208191114938882.html">什么是开源模型？什么是开放权重模型？虽然两者的概念经常被混淆，但它们之间是有很大区别的。开放权重模型指的是把模型训练好的参数公开出来，大家直接下载就能用，上手很方便。但它并不公开底层代码和完整的训练细节，所以你能用、能微调到一定程度，但想彻底看懂或大改架构就比较难。例如 Meta 的 _新浪新闻</a></li>
<li><a href="https://m.cls.cn/detail/1989989">OpenAI这次要open了，奥尔特曼所说的“开放权重模型”是什么？</a></li>

</ul>
</details>

**标签**: `#AI geopolitics`, `#open-source AI`, `#China`, `#global south`, `#AI governance`

---

<a id="item-6"></a>
## [微软确认今年推出 Copilot「超级应用」](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

微软 CEO 纳德拉在财报电话会议上确认，公司将于今年推出一款 AI「超级应用」，将 Copilot 的聊天、编程和智能体能力整合到一起，覆盖消费者和商用场景。本季度将把这些体验（包括代码功能）合并进一个超级应用。 这一整合使微软能够直接与 OpenAI 的 ChatGPT Work 等集成式 AI 平台竞争，可能重塑开发者和企业访问 AI 工具的方式。这标志着向统一 AI 工作空间发展的趋势，可能影响软件工程工作流和企业生产力。 据《财富》此前报道，该超级应用将整合 Copilot 聊天、GitHub Copilot、Copilot Cowork 和 Autopilot 系统。微软上季度营收增至 900 亿美元，主要由 AI 与云业务推动。OpenAI 近期推出了整合 ChatGPT 与 Codex 的 ChatGPT Work 应用，显示出竞争态势。

telegram · zaihuapd · Aug 1, 13:18

**背景**: Copilot 是微软集成在其产品中的 AI 助手，从聊天工具演进到「Cowork」和「Autopilots」以实现自动化。「超级应用」将多种功能整合到一个平台，类似于微信。GitHub Copilot 是编程助手，而 Copilot Cowork 是 Microsoft 365 中的 AI 自动化层，Autopilot 则指代自动化任务的智能体 AI 系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/microsoft-launches-copilot-cowork-built-anthropic-cross-m365-bora-g2xzc?tl=en">Microsoft launches Copilot Cowork , built with Anthropic...</a></li>
<li><a href="https://theplanettools.ai/blog/microsoft-copilot-cowork-ga-runs-on-anthropic-claude-not-mai-2026">Copilot Cowork Runs on Claude, Not MAI — Why... | ThePlanetTools.ai</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**标签**: `#Microsoft`, `#Copilot`, `#AI`, `#Super App`, `#Product Announcement`

---

<a id="item-7"></a>
## [Karpathy 点赞 sqliteai/waste：从 NVMe 流式加载 Kimi K3](https://github.com/sqliteai/waste) ⭐️ 7.0/10

Andrej Karpathy 点赞了 GitHub 仓库 sqliteai/waste，该项目通过直接从 NVMe 存储流式加载激活的权重，使得在消费级硬件上运行完整的 2.78 万亿参数 Kimi K3 模型成为可能。该项目解决了模型（发布时 1.42 TB，转换后 982 GB）无法装入主流系统 RAM 的限制。 Karpathy 的认可表明人们对这种技术有浓厚兴趣，该技术可能使最先进的大型语言模型的访问民主化，让研究人员和爱好者无需昂贵硬件即可运行大规模模型。这可能加速本地 AI 推理的创新，并影响未来的模型部署策略。 该项目使用 C 语言编写，采用 Apache License 2.0 许可证。它仅从 NVMe 流式加载激活的权重，从而降低内存需求，并专门为 Kimi K3 模型设计。

github · karpathy · Aug 2, 17:19

**背景**: 像 Kimi K3 这样的大型语言模型拥有数十亿或数万亿参数，推理时需要大量内存。传统方法将整个模型加载到 RAM 或 GPU 内存中，这在消费级硬件上往往不可行。从存储（如 NVMe SSD）流式加载权重，通过仅获取每一步所需的部分来运行模型，用存储带宽换取内存容量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/sqliteai/waste">GitHub - sqliteai / waste : Run the full 2.78-trillion-parameter Kimi...</a></li>
<li><a href="https://trendshift.io/repositories/96638">sqliteai / waste — GitHub trending stats & insights | Trendshift</a></li>

</ul>
</details>

**标签**: `#SQLite`, `#AI`, `#data management`, `#open source`, `#Karpathy`

---

<a id="item-8"></a>
## [Karpathy 的 AI 鹈鹕引发关于物理世界基准的讨论](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy 在 Twitter 上分享了一个 AI 生成的 3D 鹈鹕动画，迅速引发了社区关于将此类输出作为 AI 理解物理世界基准的讨论。该推文获得了大量关注，有 421 个点赞和 333 条评论。 这一讨论凸显了 AI 评估从静态图像生成向动态 3D 动画的转变，后者更能揭示模型对物理规律和空间推理的掌握程度。它强调了衡量物理世界理解的基准日益重要，这是迈向更强大 AI 系统的关键一步。 社区成员指出，鹈鹕动画很可能是使用 three.js（一个 JavaScript 3D 图形库）生成的，一些人怀疑 Anthropic 模型经过专门训练，擅长生成 three.js 代码。动画未公开提示词成为争议点，因为这影响了可复现性。

hackernews · delichon · Aug 2, 04:05 · [社区讨论](https://news.ycombinator.com/item?id=49140998)

**背景**: 物理 AI 指的是能够感知、理解并在现实世界中行动的 AI 系统，它将模型与传感器和执行器相结合。传统基准通常侧重于文本或静态图像，而 3D 动画要求模型推理空间关系、物体交互和物理合理性，从而提供对理解能力的更全面测试。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://artificialanalysis.ai/microevals/threejs-3d-modeling-and-animation-benchmark-1755135878779">Three.js 3 D Modeling and Animation Benchmark | Artificial Analysis</a></li>
<li><a href="https://venturebeat.com/technology/three-ways-ai-is-learning-to-understand-the-physical-world">Three ways AI is learning to understand the physical world | VentureBeat</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧：一些人称赞该动画是物理世界理解的新基准，而另一些人则批评其缺乏可复现性，并质疑 three.js 生成是否真正表明物理理解。一些评论者分享了他们使用 AI 生成 3D 动画的个人经验，指出需要自定义调整以及当前模型在创建完全功能场景方面的局限性。

**标签**: `#AI`, `#3D animation`, `#benchmarks`, `#Karpathy`, `#machine learning`

---

<a id="item-9"></a>
## [F*：一种通用的面向证明的编程语言](https://fstar-lang.org/) ⭐️ 7.0/10

F* 是一种通用的、面向证明的编程语言，它集成了形式化验证，允许开发者编写程序的同时附上机器检查的属性证明。该语言已在学术界和工业界得到应用，近期工作包括用于并发分离逻辑的 Steel 语言。 F* 之所以重要，是因为它支持高可信软件开发，尤其是在正确性至关重要的关键系统中。其面向证明的方法可以减少错误和安全漏洞，并且它在迁移 C 代码库中的实际应用显示了其现实世界的适用性。 F* 发音为“F star”，旨在编写带有机器检查证明的程序。主页缺少直接的代码示例，这引起了社区的批评，但教程可在 fstar-lang.org/tutorial 获取。

hackernews · ducktective · Aug 2, 12:31 · [社区讨论](https://news.ycombinator.com/item?id=49143925)

**背景**: 形式化验证是一种使用数学方法证明系统正确性的技术，例如密码协议和软件。传统语言依赖测试和调试，而像 F* 这样的面向证明的语言将数学证明技术集成到开发过程中，允许对程序属性进行机器检查的证明。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fstar-lang.org/">F *: A Proof - Oriented Programming Language</a></li>
<li><a href="https://www.linkedin.com/pulse/f-general-purpose-proof-oriented-programming-language-kusho-4bipc">F * : A general-purpose proof - oriented programming language</a></li>
<li><a href="https://www.linuxlinks.com/f-general-purpose-proof-oriented-programming-language/">F * - general-purpose, proof - oriented programming language</a></li>

</ul>
</details>

**社区讨论**: 社区讨论既有赞扬也有批评：一些用户欣赏 F* 在迁移 C 代码库方面的实用性，而另一些用户则抱怨主页缺少代码示例。还有人好奇其工业用途，以及关于响应式样式表中副作用的幽默评论。

**标签**: `#formal verification`, `#programming language`, `#proof-oriented`, `#functional programming`, `#F*`

---

<a id="item-10"></a>
## [EA 以 550 亿美元被沙特财团收购，交易下周完成](https://www.gamersky.com/news/202607/2180618.shtml) ⭐️ 7.0/10

艺电（EA）宣布，由沙特公共投资基金（PIF）牵头，联合银湖资本和 Affinity Partners 组成的财团对其的收购已获得所有监管批准。这笔 550 亿美元的交易预计将于 2026 年 8 月 4 日正式完成，届时 EA 将成为一家私营公司。 此次收购是游戏史上第二大收购案，凸显了沙特在全球游戏行业的激进布局。这将显著扩大 PIF 的游戏版图，并可能重塑行业格局，因为 EA 的财务数据将不再公开，降低了投资者和竞争对手的透明度。 收购财团包括 PIF、银湖资本和 Affinity Partners。该交易对 EA 的估值为 550 亿美元，仅次于 2023 年微软以 754 亿美元收购动视暴雪，成为游戏史上第二大收购案。PIF 此前已全资收购了 Scopely 和 Niantic，并持有其他游戏公司的股份。

telegram · zaihuapd · Aug 1, 09:10

**背景**: 沙特公共投资基金（PIF）一直积极投资游戏行业，作为其“2030 愿景”经济多元化计划的一部分。该基金已持有任天堂、Take-Two 等主要发行商的股份，并全资收购了移动游戏开发商 Scopely 和 Niantic。银湖资本是一家专注于科技领域的知名私募股权公司，而 Affinity Partners 是由贾里德·库什纳创立的投资公司。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://english.indianews.in/tech-auto/from-riyadh-to-silicon-valley-how-ea-became-the-jewel-of-saudi-arabias-gaming-vision-840036/">From Riyadh to Silicon Valley: How EA became the jewel of Saudi ...</a></li>
<li><a href="https://www.nairaland.com/8533217/why-saudi-investing-heavily-gaming">Why Saudi Is Investing Heavily In Gaming : The $38B Gaming Drive...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Silver_Lake_(investment_firm)">Silver Lake (investment firm) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Affinity_Partners">Affinity Partners - Wikipedia</a></li>

</ul>
</details>

**标签**: `#EA`, `#acquisition`, `#gaming`, `#Saudi PIF`, `#industry news`

---

<a id="item-11"></a>
## [长鑫存储发布 DDR5 和 LPDDR5X，DDR5 速率达 8000Mbps](https://t.me/zaihuapd/42925) ⭐️ 7.0/10

在 IC China 上，长鑫存储首次全面展示了其最新的 DDR5 和 LPDDR5X 产品线。DDR5 系列最高速率达 8000Mbps，LPDDR5X 最高速率达 10667Mbps。 这标志着中国半导体产业的重要里程碑，长鑫存储的 DDR5 速率已进入国际顶级梯队，可能重塑全球存储市场格局。相比主流 6400Mbps 产品 25%的速率提升，可能给竞争对手带来压力，并为数据中心和移动设备提供更多选择。 DDR5 系列还推出了 24Gb 大容量颗粒，以满足数据中心扩容需求；LPDDR5X 提供 16Gb 颗粒，涵盖 12GB 至 32GB 等多种封装方案。这些产品已实现量产，据报道长鑫存储正在批量生产速率达 8000Mbps 的 24Gb DDR5 模块和速率达 10667Mbps 的 16Gb LPDDR5X 模块。

telegram · zaihuapd · Aug 1, 15:30

**背景**: DDR5 是最新一代 DRAM 内存，相比 DDR4 提供更高的速率和带宽。LPDDR5X 是面向移动设备的低功耗版本。长鑫存储是中国首家实现 DRAM 大规模量产的 IDM 企业，在全球供应链动态和技术限制背景下，其进展备受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://larcomse.com/news/shownews.php?id=84">长鑫存储官宣发布 LPDDR 5 X ！ 速 率 登顶 10667 Mbps ...</a></li>
<li><a href="https://www.csdn.net/article/2025-12-05/155597521">全球存储格局或将重塑！ 长鑫 LPDDR 5 X 以 10667 Mbps ...</a></li>
<li><a href="https://www.chiphell.com/thread-2846391-1-1.html">长 鑫 存 储 产能快速飙升 预计年末达每月35...</a></li>

</ul>
</details>

**标签**: `#半导体`, `#DDR5`, `#存储`, `#长鑫存储`, `#LPDDR5X`

---

<a id="item-12"></a>
## [AI 芯片数量每 9 个月翻番，预计 2028 年达 2 亿颗](https://www.nytimes.com/interactive/2026/07/29/technology/ai-chips-data-center-boom.html) ⭐️ 7.0/10

据 Epoch AI 估算，目前全球 AI 芯片数量约为 2000 万颗，并且每 9 个月翻一番，预计到 2028 年底将达到约 2 亿颗。IDC 预测，到 2029 年全球 AI 基础设施投资将突破 1 万亿美元，而去年为 3180 亿美元。 AI 芯片部署的爆炸式增长标志着基础设施投资规模空前，其驱动力是规模定律——算力越大，AI 能力越强。这对能源消耗、环境影响以及 AI 的经济可持续性具有重大影响，同时也加剧了地缘政治竞争，美国控制着全球约 80%的 AI 算力。 美国控制着全球约 80%的 AI 算力，仅 Google 一家的 AI 芯片数量据信是中国所有公司的四倍。中国正通过自研半导体和 AI 基础设施加速追赶，但大规模建设引发电价上涨与环境争议，经济学家警告当前支出可能超过盈利。

telegram · zaihuapd · Aug 2, 01:01

**背景**: AI 中的规模定律是指一种经验观察，即增加模型规模、训练数据和计算量会带来 AI 性能的可预测提升。这促使科技巨头大力投资数据中心和专用 AI 芯片（如 GPU 和 TPU），以训练和运行日益强大的模型。AI 基础设施的快速增长让人联想到历史上的基建狂热，这些狂热有时以泡沫破裂告终。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://grokipedia.com/page/Epoch_AI">Epoch AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/alejandro-antunez_idc-explosive-growth-in-ai-infrastructure-activity-7249459714709692416-KJVo">IDC : Explosive Growth in AI Infrastructure Investment | Official...</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#infrastructure`, `#scaling laws`, `#data centers`, `#investment`

---

<a id="item-13"></a>
## [苹果限制漏洞报告以遏制 AI 生成的垃圾信息](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

苹果已限制研究人员可同时提交的漏洞报告数量，并设置 30 天冷却期，以应对 AI 生成的低质量安全报告激增。意大利初创公司 Bynario 使用 ChatGPT 在三周内发现了 50 多个 macOS 漏洞，包括一个提权漏洞链，但因新限额而无法报告。 这凸显了 AI 对网络安全的双重影响：AI 既能加速漏洞发现，也会用低质量报告淹没厂商，迫使政策调整，可能无意中阻碍合法研究人员。该事件强调了需要平衡的披露政策，既能过滤噪音，又不阻碍真正的发现。 Bynario 首席执行官 Alfredo Pesoli 估计，未报告的漏洞在黑市价值 10 万至 20 万美元。苹果已联系 Bynario 审核其提交，其最新安全更新修复的漏洞数量约为平时的五倍，并致谢 Anthropic 和 OpenAI 的工具。

telegram · zaihuapd · Aug 2, 05:50

**背景**: 苹果的漏洞赏金计划鼓励研究人员报告漏洞以获取奖励，但 AI 生成的报告涌入使审核人员不堪重负。类似问题也影响了其他项目，例如 Linux 内核维护者 Linus Torvalds 曾抱怨 AI 生成的错误报告垃圾信息。像 ChatGPT 这样的 AI 工具现在可以协助发现真实漏洞，但也会产生许多误报。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://the-decoder.com/a-real-macos-flaw-worth-200k-went-unreported-because-apples-bug-bounty-inbox-was-full-of-ai-slop/">A real macOS flaw worth $200K went unreported because Apple's bug...</a></li>
<li><a href="https://bugflation.com/systems/bynario-ai/">BynarIO AI - Bugflation</a></li>
<li><a href="https://www.artofsm.art/t/linus-torvalds-blasts-ai-security-bug-reports/18906">Linus Torvalds Blasts AI Security Bug Reports - security - Art of Smart</a></li>

</ul>
</details>

**社区讨论**: 鉴于限制报告的争议，讨论可能会很活跃。一些人可能认为苹果的政策是管理 AI 垃圾信息的必要之举，而另一些人可能批评它阻碍了合法研究人员，并可能使漏洞得不到修补。

**标签**: `#cybersecurity`, `#AI`, `#vulnerability disclosure`, `#Apple`, `#macOS`

---

<a id="item-14"></a>
## [中国 AI 框架以 90%准确率检测比特币洗钱](https://www.scmp.com/news/china/science/article/3362493/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-90-accuracy) ⭐️ 7.0/10

中国人民公安大学的研究人员开发了一种结合记忆模块和大语言模型的 AI 框架，能够以近 90%的准确率检测非法比特币交易。该研究成果发表在 5 月刊的同行评审期刊《情报杂志》上。 这一发展为执法部门和金融监管机构提供了打击加密货币相关洗钱活动的有力工具，而此类活动在全球范围内日益受到关注。它展示了 AI 在增强金融犯罪检测方面的实际应用，并可能影响未来的监管方法。 该框架据称在识别非法交易方面实现了近 90%的总体准确率。据中国最高人民检察院数据，2025 年全国检方共起诉 3,259 名涉及虚拟货币和地下银行洗钱案的嫌疑人。

telegram · zaihuapd · Aug 2, 08:22

**背景**: 比特币和其他加密货币具有假名性，使其成为洗钱和其他非法活动的诱人工具。传统检测方法往往难以应对区块链交易的规模和匿名性。这一新的 AI 框架利用先进的机器学习技术分析交易模式并识别可疑活动，为监管机构提供了一种更高效且可解释的方法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3362493/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-90-accuracy?pgtype=live">Chinese police AI algorithm tracks bitcoin money laundering with 90 ...</a></li>
<li><a href="https://dallasgazettenews.com/2026/08/01/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-with-90-accuracy/">Chinese police AI algorithm tracks bitcoin money laundering with 90 ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#cryptocurrency`, `#money laundering`, `#law enforcement`, `#research`

---

<a id="item-15"></a>
## [中国发布公共预警短信强制性国家标准](https://t.me/zaihuapd/42937) ⭐️ 7.0/10

国家市场监督管理总局批准发布了强制性国家标准 GB 32634-2025《公共预警短消息业务技术要求》，该标准将于 2026 年 5 月 1 日起实施，全部代替推荐性国家标准 GB/T 32634-2016，由推荐性升级为强制性。 此次升级使电信运营商和设备制造商必须遵守该标准，确保全国公共预警短信更加可靠和标准化。它加强了国家自然灾害警报能力，特别是地震等灾害的预警推送，通过更有效的应急通信可能挽救生命。 该标准由工业和信息化部归口，主要起草单位包括中国信通院、中国电信、中国移动和中国联通。标准涵盖公共预警短消息业务的总体要求、业务流程及终端规范，支持地震等自然灾害的国家级警报推送。

telegram · zaihuapd · Aug 2, 10:16

**背景**: 在中国，国家标准分为强制性（GB）和推荐性（GB/T）两类。强制性标准具有法律强制力，必须执行；推荐性标准自愿采用。公共预警短消息业务是一种利用小区广播或点对点消息向移动用户发送紧急警报的服务，新的强制性标准旨在确保跨网络和设备的一致、可靠实施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bzpt.com/gb/425984.html">GB 32634 - 2025 公 共 预 警 短 消 息 业 务 技 术 要 求 .pdf_标准平台</a></li>
<li><a href="https://www.antpedia.com/standard/1764613859.html">GB 32634 - 2025 公 共 预 警 短 消 息 业 务 技 术 要 求 标准</a></li>
<li><a href="http://deweixiansz.com/list_27/1174.html">deweixiansz.com/list_27/1174.html</a></li>

</ul>
</details>

**标签**: `#public warning`, `#SMS`, `#standard`, `#China`, `#telecommunications`

---

<a id="item-16"></a>
## [深海热液喷口附近 92%动物体内检出微塑料](https://www.yahoo.com/news/science/articles/most-isolated-environments-microplastics-finding-020000452.html) ⭐️ 7.0/10

由韩国生物科学与生物技术研究院领衔、发表于《Water Research》的一项研究，在西南太平洋和印度洋约 2000 米深的深海热液喷口附近采集的 12 只动物中，有 11 只（92%）体内检出微塑料，平均每只含 3.42 片，主要成分为聚苯乙烯。 这一发现表明，微塑料污染已渗透至最偏远、最原始的深海生态系统，凸显了塑料污染的全球性影响。由于深海清理几乎无法实施，该研究强调了从源头减少塑料排放的紧迫性，并为深海监测与保护政策提供了关键数据。 该研究检查了四种动物，包括滤食性贻贝和食草性蜗牛。微塑料在贻贝体内分布均匀，但在蜗牛体内集中于消化器官，且印度洋样本中的浓度高于太平洋样本。

telegram · zaihuapd · Aug 2, 11:00

**背景**: 深海热液喷口是 1977 年才被发现的极端环境，支持着依赖化能合成而非阳光的独特生态系统。微塑料是尺寸小于 5 毫米的微小塑料颗粒，可被海洋生物摄入并进入食物链。此前研究表明，滤食性动物（如鲸类和贝类）可能摄入大量微塑料，对海洋生物和人类健康构成风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.sciencenet.cn/htmlpaper/2025/5/2025512155355670132746.shtm">99.999%的 深 海 海 底仍未被人类探索—论文—科学网</a></li>
<li><a href="https://news.sciencenet.cn/htmlnews/2022/11/488718.shtm">国际最新研究：美海岸 滤 食 性 鲸每天 摄 入 最多1000...</a></li>

</ul>
</details>

**标签**: `#microplastics`, `#deep-sea`, `#environmental science`, `#pollution`, `#marine biology`

---

<a id="item-17"></a>
## [美国多州拟取消数据中心税收优惠，AI 基础设施成本上升](https://theinformation.com/articles/exclusive-data-center-costs-set-rise-u-s-states-move-repeal-tax-breaks) ⭐️ 7.0/10

美国多个州正考虑取消或收紧针对数据中心的税收优惠，这可能会提高 AI 基础设施的建设成本。据 The Information 报道，这一政策转变正值数据中心的电力需求和财政压力不断增加之际。 这一政策转变可能显著提高美国数据中心建设成本，影响 AI 基础设施部署的经济性。它可能影响企业选择建设数据中心的地点，并可能减缓 AI 扩张的步伐，对云服务提供商和 AI 初创公司都会产生影响。 报道指出，此前各州通过免除服务器和电力成本来吸引数据中心投资，但现在一些州正在重新考虑这些激励措施。摘要中未明确具体州份和时间表，但这一趋势表明，在 AI 驱动的需求上升之际，各州正在更广泛地重新评估税收激励政策。

telegram · zaihuapd · Aug 3, 00:42

**背景**: 数据中心是容纳计算机系统及相关组件（如电信和存储）的设施，对于云计算和 AI 训练至关重要，这些应用需要大量的计算能力和电力。为了吸引这些设施，美国许多州曾提供设备和公用事业税收豁免，但 AI 的快速发展导致能源需求和基础设施成本飙升，促使一些州重新考虑这些激励措施。根据 Data Center Watch 项目的数据，去年 3 月至 6 月期间，约有 20 个数据中心项目被阻止或推迟，涉及投资总额近 980 亿美元，反映出当地反对声浪日益高涨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.cnbeta.com.tw/view/1557568.htm">威斯康星小城全民公投叫停 数 据 中 心 税 收 优 惠 - cnBeta.COM 移动版</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#data centers`, `#tax policy`, `#cloud computing`, `#regulation`

---