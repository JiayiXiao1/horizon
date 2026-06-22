---
layout: default
title: "Horizon Summary: 2026-06-22 (ZH)"
date: 2026-06-22
lang: zh
---

> From 28 items, 8 important content pieces were selected

---

1. [三维光纤微镊实现十万倍力增强](#item-1) ⭐️ 9.0/10
2. [我过去的工作是否只因欺诈而存在？](#item-2) ⭐️ 8.0/10
3. [宁可重复代码，也不要错误的抽象](#item-3) ⭐️ 8.0/10
4. [Peter Norvig 的经典 Lisp 解释器教程](#item-4) ⭐️ 8.0/10
5. [Polymarket 被曝雇人制作虚假交易视频引流](#item-5) ⭐️ 8.0/10
6. [Apertus：面向主权 AI 的开放基础模型](#item-6) ⭐️ 7.0/10
7. [sqlite-utils 4.0rc1 新增迁移和嵌套事务](#item-7) ⭐️ 7.0/10
8. [Cloudflare 推出面向 AI 代理的临时账户](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [三维光纤微镊实现十万倍力增强](https://www.stdaily.com/web/gdxw/2026-06/19/content_534836.html) ⭐️ 9.0/10

安徽大学与中国科学技术大学团队利用飞秒激光复合制造方法，在商用光纤端部构建出新型三维光纤微镊，成果发表于《自然》。该微镊输出力达到传统光镊的十万倍以上，实现了对微米尺度目标的高精度、低损伤三维操控。 该突破克服了传统光镊作用力弱、无法操控不透明物体以及机械微夹持器在狭小空间内精度受限的瓶颈。通过提供紧凑的光纤集成工具和可编程力控制，为单细胞操作、显微手术和生物医学研究开辟了新途径。 该微镊将光传输、光热转换、材料响应和微结构力学输出高度集成于同一根光纤。通过调节输入光功率即可连续精密控制作用力，并能在百微米级的窄小空间内完成精准取样。

telegram · zaihuapd · Jun 20, 15:19

**背景**: 光镊利用高度聚焦的激光束捕获和操控微观粒子，但其作用力通常在皮牛量级，限制了应用。飞秒激光制造利用超快激光脉冲在材料上创建精确的微纳结构。本工作将两种技术结合，创造出基于光纤的工具，在保持精度的同时大幅放大了作用力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC11277908/">Metal Material Processing Using Femtosecond Lasers: Theories, Principles, and Applications - PMC</a></li>
<li><a href="https://en.wikipedia.org/wiki/Optical_tweezers">Optical tweezers</a></li>
<li><a href="https://spj.science.org/doi/10.34133/2021/9783514">Femtosecond Laser Precision Engineering: From Micron, Submicron, to Nanoscale | Ultrafast Science</a></li>

</ul>
</details>

**标签**: `#optical tweezers`, `#femtosecond laser`, `#micro-manipulation`, `#biomedical engineering`, `#Nature`

---

<a id="item-2"></a>
## [我过去的工作是否只因欺诈而存在？](https://david.newgas.net/did-my-old-job-only-exist-because-of-fraud/) ⭐️ 8.0/10

一篇个人文章和 Hacker News 讨论揭示了科技岗位中（尤其是政府合同领域）的计费操纵和欺诈行为如何夸大职位数量，并质疑其合法性。 此事重要，因为它揭露了系统性欺诈浪费纳税人的钱并扭曲科技就业市场，引发软件工程师和承包商的伦理担忧。 例子包括承包商通过外包公司以虚高费率重新聘用，以及经理在政府项目中欺诈性编辑工时表以耗尽预算。

hackernews · advisedwang · Jun 21, 21:40 · [社区讨论](https://news.ycombinator.com/item?id=48622867)

**背景**: 在政府合同中，公司通常按工时计费，且预算必须在年底前花完。欺诈行为可能包括伪造工时表或虚增人头数以最大化收入，有时会导致法律后果。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=33755400">Engineers' billing nightmares | Hacker News</a></li>
<li><a href="https://blog.theodorewatson.com/avoiding-the-pathway-on-government-contract-fraud-and-federal-procurement-fraud-do-you-have-the-right-defense-lawyer/">Avoiding the Pathway on Government Contract Fraud - Do You Have the Right Defense Lawyer?</a></li>
<li><a href="https://oig.hhs.gov/fraud/contract-fraud/">Contract Fraud | Office of Inspector General | Government Oversight | U.S. Department of Health and Human Services</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了在银行和政府项目中遇到的计费欺诈经历，指出这种做法常见但有风险。一些人强调共谋的伦理困境，另一些人则指出举报可能带来危险。

**标签**: `#fraud`, `#software engineering`, `#workplace ethics`, `#tech industry`, `#government contracting`

---

<a id="item-3"></a>
## [宁可重复代码，也不要错误的抽象](https://sandimetz.com/blog/2016/1/20/the-wrong-abstraction) ⭐️ 8.0/10

Sandi Metz 在 2016 年的文章中指出，过早抽象是有害的，重复代码往往比强行使用错误的抽象更好，主张在模式清晰之前等待再重构。 这篇文章挑战了软件工程的一个核心原则——代码重复总是坏事——并提供了一个细微的视角，影响了许多开发者对抽象和重构的看法。 文章强调，错误的抽象可能比重复代码更有害，开发者只应在出现清晰、重复的模式时才引入抽象，而不是过早进行。

hackernews · rafaepta · Jun 21, 16:08 · [社区讨论](https://news.ycombinator.com/item?id=48620090)

**背景**: 抽象是软件工程中的一个基本概念，将通用代码提取到单个可复用组件中以减少重复。然而，如果抽象基于不完整的理解，可能导致复杂且难以修改的代码。Sandi Metz 是 Ruby 社区中知名的作者和演讲者，她的著作《Practical Object-Oriented Design in Ruby》（POODR）备受推崇。

**社区讨论**: 评论普遍同意文章的前提，有些人强调当重复代码导致耦合时，仍应尊重“单一真相来源”原则。其他人指出函数式编程可以减少对抽象的需求，而代码重复往往源于开发孤岛而非抽象问题。

**标签**: `#software engineering`, `#abstraction`, `#code quality`, `#refactoring`, `#OOP`

---

<a id="item-4"></a>
## [Peter Norvig 的经典 Lisp 解释器教程](https://norvig.com/lispy.html) ⭐️ 8.0/10

Peter Norvig 于 2010 年发布的教程《如何用 Python 编写一个 Lisp 解释器》至今仍是学习语言实现的经典资源，通过用 Python 构建一个 Scheme 解释器来教学。 该教程提供了编写解释器的清晰实践入门，让具备基础 Python 知识的程序员也能上手，并激励了许多人探索编程语言设计。 该教程用大约 100 行 Python 代码实现了 Scheme 的一个子集 Lispy（lis.py），涵盖环境、求值和递归。后续的第二部分增加了宏和续延。

hackernews · tosh · Jun 21, 15:36 · [社区讨论](https://news.ycombinator.com/item?id=48619831)

**背景**: Lisp 是一族编程语言，以其完全括号化的前缀表示法和对符号计算的支持而闻名。解释器直接执行代码而无需编译，因此非常适合学习语言内部机制。Peter Norvig 是著名的计算机科学家，曾任 Google 研究总监。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.norvig.com/lispy.html">(How to Write a ( Lisp ) Interpreter (in Python ))</a></li>
<li><a href="https://en.wikipedia.org/wiki/Lisp_(programming_language)">Lisp (programming language) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Peter_Norvig">Peter Norvig - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调该教程是学习语言实现的最佳起点，并提到了 Ribbit 和 Crafting Interpreters 等相关项目。有人指出其教育目的以及引导出更快的 Lisp 的价值。

**标签**: `#Lisp`, `#Python`, `#interpreter`, `#tutorial`, `#programming languages`

---

<a id="item-5"></a>
## [Polymarket 被曝雇人制作虚假交易视频引流](https://www.wsj.com/business/media/polymarket-social-media-bets-prediction-market-441cdeb5) ⭐️ 8.0/10

《华尔街日报》调查发现，Polymarket 雇佣数十名年轻创作者在模拟网站上制作虚假交易视频，并隐藏付费合作关系。在分析的 1105 个视频中，70% 展示了总计 190 万美元的虚假下注，其中 118 个视频宣称赢得近 90 万美元，但这些交易本会亏损超过 16.6 万美元。 这种欺骗性营销行为违反了美国联邦广告法关于付费代言必须披露利益关系的规定，并损害了预测市场的信任度。Polymarket 自 2022 年起已被禁止在美国提供主要加密交易服务，但仍通过社交媒体向美国用户推送内容。 调查分析了 1105 个视频，其中 70% 包含总计 190 万美元的虚假下注。在 118 个宣称赢得近 90 万美元的视频中，实际交易本会导致超过 16.6 万美元的亏损。Polymarket 回应称致力于市场透明，并计划全面审计现有推广内容。

telegram · zaihuapd · Jun 21, 06:31

**背景**: Polymarket 是一个去中心化预测市场平台，用户可以对选举、体育等事件的结果进行下注。2022 年，美国商品期货交易委员会（CFTC）命令 Polymarket 支付 140 万美元罚款，并禁止其向美国用户提供服务。美国联邦法律要求付费代言必须明确披露，以避免误导消费者。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.reddit.com/r/technology/comments/1ubnbyu/polymarket_accused_of_using_fake_winning_bets_to/">Polymarket Accused of Using Fake Winning Bets to Fuel Viral Growth</a></li>
<li><a href="https://www.ftc.gov/news-events/topics/truth-advertising/advertisement-endorsements">Advertisement Endorsements | Federal Trade Commission</a></li>

</ul>
</details>

**社区讨论**: 在 Reddit 上，用户对 Polymarket 的诚信表示怀疑，有评论指出“大户可以翻转投票并拿走所有人的钱”。讨论凸显了人们对预测市场操纵和公平性的广泛担忧。

**标签**: `#Polymarket`, `#deceptive marketing`, `#prediction markets`, `#regulatory compliance`, `#investigative journalism`

---

<a id="item-6"></a>
## [Apertus：面向主权 AI 的开放基础模型](https://apertvs.ai/) ⭐️ 7.0/10

2025 年 9 月 2 日，瑞士 AI 倡议（EPFL、苏黎世联邦理工学院和瑞士国家超级计算中心）发布了 Apertus，这是一个完全开放的大语言模型，在超过 1800 种语言上训练，并以 Apache 2.0 许可证发布。 Apertus 代表了向主权 AI 迈出的重要一步，使各国能够利用自己的基础设施和数据构建 AI 能力，减少对美国和中国科技巨头的依赖。 Apertus 完全开放，包括训练数据、代码、权重、方法和对齐原则，使其可复现。然而，社区评论指出其指令模型基于去年的 Llama 3.1 微调，且多语言性能被批评为幻觉出不存在的词汇。

hackernews · T-A · Jun 21, 21:29 · [社区讨论](https://news.ycombinator.com/item?id=48622778)

**背景**: 主权 AI 指国家利用自身基础设施、数据和劳动力生产 AI 的能力。Apertus 由瑞士 AI 倡议开发，该倡议是 EPFL、苏黎世联邦理工学院和 CSCS 的合作项目，旨在提供透明且多语言的专有模型替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Apertus_(LLM)">Apertus (LLM) - Wikipedia</a></li>
<li><a href="https://apertvs.ai/">Fully Open Foundation Model for Sovereign AI</a></li>
<li><a href="https://ethz.ch/en/news-and-events/eth-news/news/2025/09/press-release-apertus-a-fully-open-transparent-multilingual-language-model.html">Apertus: a fully open, transparent, multilingual language model</a></li>

</ul>
</details>

**社区讨论**: 社区评论对 Apertus 的竞争力和速度表示怀疑，一位用户指出其以“委员会的速度”推进，可能无法与当前模型竞争。其他人则指出已有完全开放的模型如 OLMo 和 K2 Think V2，并质疑其许可证的长期可行性。

**标签**: `#open-source`, `#AI`, `#foundation model`, `#sovereign AI`, `#LLM`

---

<a id="item-7"></a>
## [sqlite-utils 4.0rc1 新增迁移和嵌套事务](https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/#atom-everything) ⭐️ 7.0/10

sqlite-utils 4.0rc1 引入了内置的数据库迁移功能以及通过 db.atomic() 实现的嵌套事务支持，这是 4.0 版本的第一个候选发布版。 此次更新通过提供轻量级的迁移系统和更安全的事务处理，简化了 Python 开发者的 SQLite 数据库管理，减少了对外部工具的依赖。 迁移被定义为使用 @migrations() 装饰的 Python 函数，可以通过 Python 或 CLI 命令 'sqlite-utils migrate' 应用。该系统不支持反向迁移，鼓励仅向前修复。

rss · Simon Willison · Jun 21, 23:35

**背景**: sqlite-utils 是一个 Python 库和 CLI 工具，在 SQLite 的 sqlite3 模块之上提供高级操作。它被广泛用于导入 JSON 数据和转换表等任务。新的迁移功能移植自成熟的 sqlite-migrate 包，该包已在 LLM 等项目中使用多年。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://sqlite-utils.datasette.io/en/latest/migrations.html">Database migrations - sqlite-utils</a></li>
<li><a href="https://github.com/simonw/sqlite-migrate">GitHub - simonw/sqlite-migrate: A simple database migration system for ...</a></li>
<li><a href="https://simonwillison.net/2026/Jun/21/sqlite-utils-40rc1/">sqlite-utils 4.0rc1 adds migrations and nested transactions</a></li>

</ul>
</details>

**标签**: `#Python`, `#SQLite`, `#database`, `#migrations`, `#open source`

---

<a id="item-8"></a>
## [Cloudflare 推出面向 AI 代理的临时账户](https://simonwillison.net/2026/Jun/21/temporary-cloudflare-accounts/#atom-everything) ⭐️ 7.0/10

Cloudflare 宣布通过 `wrangler deploy --temporary` 命令实现临时、短暂的 Workers 部署，无需 Cloudflare 账户即可运行代码 60 分钟。 该功能移除了身份验证障碍，简化了开发者和 AI 代理的部署流程，无需手动创建账户即可进行快速原型设计和自动化工作流。 临时部署存活时间恰好为 60 分钟，之后会被删除，除非通过提供的 URL 认领。认领 URL 允许人类登录并将项目转为永久。

rss · Simon Willison · Jun 21, 22:01

**背景**: Cloudflare Workers 是一个在边缘运行代码的无服务器计算平台。传统上，部署 Worker 需要创建账户并通过 OAuth 或 API 令牌进行身份验证，这对自动化代理可能构成障碍。`--temporary` 标志通过创建一个仅在部署生命周期内存在的临时预览账户来绕过这一限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.cloudflare.com/workers/platform/claim-deployments/">Claim deployments (temporary accounts) - Cloudflare Docs</a></li>
<li><a href="https://www.explainx.ai/blog/cloudflare-temporary-accounts-ai-agents-wrangler-2026">Cloudflare Temporary Accounts for AI Agents (2026) - explainx.ai</a></li>
<li><a href="https://letsdatascience.com/news/cloudflare-enables-temporary-accounts-for-ai-agents-d518d809">Cloudflare Enables Temporary Accounts for AI Agents</a></li>

</ul>
</details>

**标签**: `#cloudflare`, `#serverless`, `#deployment`, `#developer-experience`

---