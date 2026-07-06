---
layout: default
title: "Horizon Summary: 2026-07-06 (ZH)"
date: 2026-07-06
lang: zh
---

> From 38 items, 18 important content pieces were selected

---

1. [数字游戏 vs 实体游戏：核心问题是所有权](#item-1) ⭐️ 8.0/10
2. [sqlite-utils 4.0rc2：由 Claude Fable 以 149 美元编写](#item-2) ⭐️ 8.0/10
3. [新 Claude 模型工具调用出现倒退](#item-3) ⭐️ 8.0/10
4. [iOS 27 将加入 Trust Insights 设备端反诈功能](#item-4) ⭐️ 8.0/10
5. [F-Droid 称 Google ADV 为恶意软件，已预装 40 亿设备](#item-5) ⭐️ 8.0/10
6. [香港处理中国过半芯片进口](#item-6) ⭐️ 8.0/10
7. [复旦期末考：学生出题难倒 AI](#item-7) ⭐️ 8.0/10
8. [SpaceX 向投资者展示原型手机](#item-8) ⭐️ 8.0/10
9. [中国拟削减 SCI 发表激励以防技术泄密](#item-9) ⭐️ 8.0/10
10. [Karpathy 的 nanochat：用 100 美元构建 ChatGPT](#item-10) ⭐️ 7.0/10
11. [《电脑主演》：影视剧中电脑的详尽目录](#item-11) ⭐️ 7.0/10
12. [免费在线编译器教科书发布](#item-12) ⭐️ 7.0/10
13. [用 445 字节和 Deflate 压缩生成世界地图](#item-13) ⭐️ 7.0/10
14. [韩国拟投 800 万亿韩元建半导体集群，DRAM 产量目标五年翻倍](#item-14) ⭐️ 7.0/10
15. [Linux 登顶 2026 CVE 榜单，维护者称这是好事](#item-15) ⭐️ 7.0/10
16. [三星计划第三季度 DRAM 涨价约 20%](#item-16) ⭐️ 7.0/10
17. [卫报调查：OpenAI 从未到访星际之门英国选址](#item-17) ⭐️ 7.0/10
18. [中国初创公司测试二氧化碳冷发射火箭技术](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [数字游戏 vs 实体游戏：核心问题是所有权](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 8.0/10

一篇博客文章指出，数字游戏与实体游戏争论的核心问题是所有权而非格式，并呼吁制定法规确保买家拥有转让和使用权。 随着数字游戏销售占据主导地位，这一讨论凸显了日益增长的消费者权益问题，并可能影响未来关于数字所有权和 DRM 实践的法规。 文章强调数字游戏通常是许可而非销售，DRM 可以撤销访问权限。它建议法规应强制要求可转让性和永久访问权。

hackernews · popcar2 · Jul 5, 14:56 · [社区讨论](https://news.ycombinator.com/item?id=48794750)

**背景**: 数字版权管理（DRM）限制用户访问和转让已购买的数字内容。许多数字游戏平台（如 Steam）使用 DRM 将游戏绑定到账户，限制了转售和长期访问。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Always-on_DRM">Always-on DRM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://d3.harvard.edu/rethinking-digital-ownership-rights-governance-and-the-path-forward/">Rethinking Digital Ownership: Rights, Governance, and the Path Forward | Harvard Business School AI Institute</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同所有权权利的必要性，有人提议禁止在许可游戏中使用“购买”一词。其他人指出，破解和盗版目前是 PC 游戏真正所有权的唯一来源。

**标签**: `#digital ownership`, `#gaming`, `#regulation`, `#DRM`, `#consumer rights`

---

<a id="item-2"></a>
## [sqlite-utils 4.0rc2：由 Claude Fable 以 149 美元编写](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/#atom-everything) ⭐️ 8.0/10

Simon Willison 发布了 sqlite-utils 4.0rc2，其中大部分代码由 Anthropic 的 Claude Fable AI 模型编写，成本约为 149.25 美元。AI 识别了关键错误，包括 delete_where()中的数据丢失问题，这些问题在稳定版发布前已修复。 这展示了 AI 在软件开发中的实用且经济高效的应用，LLM 不仅编写代码，还进行了彻底的代码审查，发现了严重错误。它突显了 AI 在有限人力资源下协助维护高质量开源项目的潜力。 开发过程涉及 37 次提示、34 次提交和跨 30 个文件的+1,321/-190 行代码变更。Claude Fable 的审查识别了 5 个发布阻塞问题，包括 delete_where()中的一个事务错误，该错误可能导致静默数据丢失。

rss · Simon Willison · Jul 5, 01:00

**背景**: sqlite-utils 是 Simon Willison 创建的用于操作 SQLite 数据库的 Python CLI 工具和库。语义化版本控制（SemVer）使用三位版本号（Major.Minor.Patch）来表示兼容性；破坏性变更需要增加主版本号。Claude Fable 是 Anthropic 为复杂编码任务设计的高级 AI 模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ...</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable">Claude Fable</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#sqlite-utils`, `#Claude Fable`, `#software engineering`, `#open source`

---

<a id="item-3"></a>
## [新 Claude 模型工具调用出现倒退](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 报告称，较新的 Claude 模型（Opus 4.8、Sonnet 5）有时会在工具调用模式中凭空添加额外字段，导致 Pi 的编辑工具拒绝原本正确的编辑，而旧模型则没有此问题。 这种反直觉的倒退威胁到依赖精确工具调用模式的基于 LLM 的编码代理的可靠性，可能迫使第三方工具适应特定模型的怪癖。 凭空添加的字段包括 'type'、'id'、'kind'、'unique'、'matchCase' 等名称以及嵌套属性；编辑内容本身通常正确，但格式错误的参数导致拒绝。在某些会话中，约 20%的编辑会出现此问题。

rss · Simon Willison · Jul 4, 22:53

**背景**: LLM 工具调用允许模型通过生成匹配预定义模式的 JSON 来调用外部函数。Anthropic 的 Claude 模型内置了 Claude Code 使用的文本编辑器工具，较新的模型可能经过强化训练以偏好该工具的模式，从而干扰了像 Pi 这样的自定义工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/earendil-works/pi/issues/6278">New Claude models work poorly with the current Pi's edit tool, failing about 20% edits in some sessions · Issue #6278 · earendil-works/pi</a></li>
<li><a href="https://techplanet.today/post/better-models-worse-tools-understanding-the-tool-calling-regression-in-newer-claude-models">Better Models, Worse Tools: Understanding the Tool-Calling Regression in Newer Claude Models | TechPlanet</a></li>
<li><a href="https://simonwillison.net/2026/Jul/4/better-models-worse-tools/">Better Models: Worse Tools</a></li>

</ul>
</details>

**社区讨论**: Pi 仓库的 GitHub issue #6278 确认了该问题，用户报告称较新的 Claude 模型约 20%的编辑失败。有人建议实现多个编辑工具以匹配模型偏好的模式。

**标签**: `#LLM`, `#tool calling`, `#Anthropic`, `#Claude`, `#reliability`

---

<a id="item-4"></a>
## [iOS 27 将加入 Trust Insights 设备端反诈功能](https://www.cultofmac.com/news/ios-27-trust-insights-feature) ⭐️ 8.0/10

Apple 宣布在 iOS 27 中加入 Trust Insights 功能，这是一个设备端反诈特性，通过分析用户的操作模式、时机、上下文和传感器数据来实时识别诈骗。当检测到中高风险时，应用可以显示警告、引入支付延迟或要求额外验证。 该功能代表了一种保护隐私的实时诈骗检测方法，所有分析均在设备端进行，原始数据会立即删除。它有望显著减少因社会工程诈骗（尤其是通过电话指导受害者转账）造成的财务损失。 Trust Insights 不会读取信息、邮件或照片内容，仅向服务器发送单一输出值。用户可以关闭该功能，但存在冷却期，防止诈骗分子在通话中诱导用户立即关闭。

telegram · zaihuapd · Jul 4, 14:30

**背景**: 传统的反诈系统通常依赖服务器端分析消息或交易，这可能引发隐私担忧。Trust Insights 将检测移至设备端，利用行为信号（如通话期间异常的输入速度或屏幕交互）来识别潜在操控。这种方法符合 Apple 对隐私和设备端智能的重视。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cultofmac.com/news/ios-27-trust-insights-feature">Trust Insights will help your iPhone identify (and stop) scammers| Cult ...</a></li>
<li><a href="https://techmymoney.com/2026/07/04/ios-27-trust-insights-will-warn-iphone-owners-mid-scam-before-money-moves/">iOS 27 Trust Insights: iPhone Scam Warnings Explained</a></li>
<li><a href="https://applemagazine.com/ios-27-trust-insights/">iOS 27 Trust Insights Helps Apps Detect Scam Coaching</a></li>

</ul>
</details>

**标签**: `#iOS`, `#anti-fraud`, `#privacy`, `#Apple`, `#mobile security`

---

<a id="item-5"></a>
## [F-Droid 称 Google ADV 为恶意软件，已预装 40 亿设备](https://f-droid.org/2026/07/01/adv-malware.html) ⭐️ 8.0/10

F-Droid 正式将 Google 的 Android 开发者验证（ADV）定性为恶意软件，警告称该程序已预装在约 40 亿台安卓设备上，并将于 2026 年 9 月起在部分国家开始阻止未经批准的软件运行。 这一进展威胁到安卓生态系统的开放性，赋予 Google 前所未有的应用安装控制权，可能限制用户自由并损害 F-Droid 等替代应用商店。 ADV 通过 Play Protect 以 root 权限作为系统进程运行，无法移除，将于 2026 年 9 月 30 日在巴西、印尼、新加坡和泰国首批激活，全球推广计划在 2027 年及以后。

telegram · zaihuapd · Jul 5, 00:41

**背景**: Android 开发者验证（ADV）是 Google 的一项要求，应用必须注册到经过身份验证的开发者才能在认证的安卓设备上安装。F-Droid 是一个自由开源的应用商店，仅托管 FOSS 应用，它反对 ADV 认为其威胁用户自由。包括 EFF、FSF 和 ACLU 在内的 70 多个组织已签署公开信谴责该计划。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.lineageos.org/Developer-Verification/">Developer Verification – LineageOS</a></li>
<li><a href="https://cybernews.com/security/f-droid-google-android-verifier-malware/">F-Droid calls Google Android verifier malware | Cybernews</a></li>
<li><a href="https://en.wikipedia.org/wiki/F-Droid">F-Droid</a></li>

</ul>
</details>

**标签**: `#Android`, `#Malware`, `#Digital Rights`, `#Google`, `#F-Droid`

---

<a id="item-6"></a>
## [香港处理中国过半芯片进口](https://thenextweb.com/news/hong-kong-china-ai-chip-trade-hub) ⭐️ 8.0/10

2026 年前五个月，香港经手了中国逾半数的芯片进口，转口至内地的芯片价值约 1240 亿美元，占中国同期芯片采购总额的 52%。 这一里程碑凸显了香港在地缘政治紧张局势下作为关键 AI 贸易枢纽的崛起，重塑了全球半导体供应链，并突显了其在中国技术进口中的战略作用。 AI 相关电子产品目前已占香港出口的 57%至 70%，促使香港贸发局将 2026 年出口增长预测上调至逾 20%。

telegram · zaihuapd · Jul 5, 02:45

**背景**: 香港的自由港地位——无关税、无资本管制以及发达的航空货运网络——使其成为高价值、低重量、时效性强的半导体贸易的理想中转地。转口贸易是指货物通过第三国或地区中转后再运往最终目的地的贸易方式，常被用于规避贸易壁垒。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hk/自由港">自由港 - 維基百科，自由的百科全書</a></li>
<li><a href="https://zh.wikipedia.org/wiki/转口贸易">转口贸易 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.yzaobao.com/news/hkMacao/202607/0475607.html">全球AI热潮推动亚洲增长 香港崛起为中国晶片贸易关键中转站</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#AI trade`, `#Hong Kong`, `#China`, `#geopolitics`

---

<a id="item-7"></a>
## [复旦期末考：学生出题难倒 AI](https://mp.weixin.qq.com/s/d53O-6mVFZqMa_Sti1yEPw) ⭐️ 8.0/10

复旦大学“数据挖掘技术”课程用“人考 AI”挑战取代传统考试，51 名学生各出 10 道有唯一答案的计算题来测试三个 AI 模型，AI 答错越多得分越高。 这一创新考核方式反映了教育范式的转变，从测试算法知识转向评估学生评判和批判 AI 输出的能力，这对职场中的 AI 素养至关重要。 51 名学生中有 50 人至少难倒过某个模型一次，但只有 4 人能让任一模型整张试卷得 0 分；最强模型 Claude 从未被完全考倒，全班平均分 85.7 分。

telegram · zaihuapd · Jul 5, 08:40

**背景**: 传统的数据挖掘考试通常侧重于记忆算法和公式，但像 Claude 这样的生成式 AI 模型现在可以解决许多此类问题。这门由肖仰华教授讲授的课程转而训练学生指挥 AI 并评估其结果，强调判断力和创造力而非死记硬背。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://docs.anthropic.com/en/docs/intro-to-claude">Intro to Claude - Anthropic</a></li>
<li><a href="https://digitalpromise.org/2026/01/26/evaluating-ai-in-education-an-analysis-of-state-guidance/">Evaluating AI in Education: An Analysis of State Guidance</a></li>

</ul>
</details>

**标签**: `#AI in Education`, `#AI Evaluation`, `#Educational Innovation`, `#AI Literacy`, `#Pedagogy`

---

<a id="item-8"></a>
## [SpaceX 向投资者展示原型手机](https://www.wsj.com/tech/spacexs-telecom-dreams-d461e568) ⭐️ 8.0/10

SpaceX 向投资者展示了一款比 iPhone 更薄、运行自有操作系统的原型手机，旨在整合 Starlink 卫星连接以提供移动服务。 此举标志着 SpaceX 可能进入移动设备市场，利用其 Starlink 网络颠覆传统电信和卫星行业。 据报道，该原型机运行专有操作系统，且比当前 iPhone 更薄。SpaceX 总裁 Gwynne Shotwell 还讨论了建设地面网络或与蜂窝运营商合作提供移动服务。

telegram · zaihuapd · Jul 5, 14:10

**背景**: SpaceX 的 Starlink 卫星星座提供全球宽带互联网。该公司已与 T-Mobile 合作提供 Direct to Cell 服务，实现基本连接。定制智能手机可以紧密集成卫星接入，绕过传统运营商。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ibtimes.co.uk/spacex-secret-ai-phone-prototype-1806844">SpaceX AI Phone Rumours Explained: Report Claims... | IBTimes UK</a></li>
<li><a href="https://www.forbes.com/sites/zacharyfolk/2026/07/01/musk-denies-report-spacex-is-developing-handheld-ai-device/">Musk Calls Reporting on SpaceX Prototype AI Device ‘Utterly False’</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#Starlink`, `#mobile devices`, `#telecommunications`, `#satellite internet`

---

<a id="item-9"></a>
## [中国拟削减 SCI 发表激励以防技术泄密](https://www.ft.com/content/64a811f1-b132-4211-8a8c-2252cf964039?syn-25a6b1a6=1) ⭐️ 8.0/10

中国政策制定者正讨论削减科研人员向 SCI 期刊投稿的激励，包括降低 SCI 论文在学术晋升和终身教职评定中的权重，原因是担心技术泄密的国家安全问题。 这一政策转变可能对全球学术出版产生重大影响，因为中国是 SCI 期刊的主要贡献者，同时可能加速国内期刊的发展，但也引发了对科研诚信和国际合作的担忧。 国家自然科学基金委现要求受资助项目至少 20%的代表性论文发表于中文期刊，一名材料学学者因安全审查标准模糊且趋严，已停止向外国期刊投稿。

telegram · zaihuapd · Jul 6, 01:03

**背景**: SCI（科学引文索引）是一个用于评估期刊质量和研究者绩效的权威引文数据库。中国长期以来激励 SCI 发表以提升研究产出，但对技术泄密和学术造假的担忧促使政策重新评估。政府还通过“中国科技期刊卓越行动计划”等举措推动国内期刊发展。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nppa.gov.cn/xxfb/zcfg/gfxwj/202106/t20210623_4514.html">中共中央宣传部 教育部 科技部印发 《关于推动学术期刊繁荣发展的意见...</a></li>
<li><a href="https://www.moe.gov.cn/jyb_xwfb/s5147/202106/t20210628_540716.html">中宣部、教育部、科技部印发《关于推动学术期刊繁荣发展的意见》 - 中...</a></li>

</ul>
</details>

**社区讨论**: 有群友评论称此举意在打击学术造假，反映了当前激励体系助长不端行为的普遍看法。

**标签**: `#academic publishing`, `#national security`, `#science policy`, `#China`, `#research integrity`

---

<a id="item-10"></a>
## [Karpathy 的 nanochat：用 100 美元构建 ChatGPT](https://github.com/karpathy/nanochat) ⭐️ 7.0/10

Andrej Karpathy 在其 nanochat 仓库中创建了一个分支，旨在仅用 100 美元构建一个类似 ChatGPT 的模型，目标是在 8XH100 GPU 节点上超越 GPT-2（1.6B 参数）。 该项目表明，以极低的成本即可构建具有竞争力的 LLM，这有望推动 AI 开发的民主化，让更多研究人员和爱好者能够实验大型语言模型。 该项目是开源的，使用约 8000 行 PyTorch 代码编写，专注于最小化超越 GPT-2 性能的挂钟时间。主要指标是在 8XH100 节点上的“达到 GPT-2 的时间”。

github · karpathy · Jul 4, 03:44

**背景**: 像 ChatGPT 这样的大型语言模型通常需要数百万美元的计算和数据成本。Karpathy 的 nanochat 旨在精简堆栈至核心要素，展示通过高效技术和适度硬件，可以在有限预算下训练出有能力的模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/karpathy/nanochat">GitHub - karpathy / nanochat : The best ChatGPT that $100 can buy.</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/10/andrej-karpathys-nanochat/">Build ChatGPT Clone with Andrej Karpathy 's nanochat</a></li>

</ul>
</details>

**标签**: `#AI`, `#ChatGPT`, `#open-source`, `#LLM`, `#cost-efficient`

---

<a id="item-11"></a>
## [《电脑主演》：影视剧中电脑的详尽目录](https://www.starringthecomputer.com/computers.html) ⭐️ 7.0/10

一个名为《电脑主演》的综合性在线目录，通过截图和背景介绍，记录了电影和电视节目中出现的电脑，涵盖数十年的影视作品。 该资源为复古计算爱好者、电影历史学家和道具设计师提供了宝贵参考，突显了电脑在媒体中的文化和技术意义。 该网站收录了从《2001 太空漫游》等经典电影到现代电视剧的条目，截图和描述质量一致。社区评论提供了技术修正和额外资源。

hackernews · gitowiec · Jul 5, 17:33 · [社区讨论](https://news.ycombinator.com/item?id=48796093)

**背景**: 几十年来，电脑一直出现在电影和电视中，通常作为反映当代技术的道具。该目录系统地捕捉了这些出现，为计算历史和流行文化提供了独特视角。

**社区讨论**: 社区评论包括对 1950 年代 SAGE 系统的 IBM AN-FSQ-7 面板的更正——这些是调制解调器而非电脑；还有用户指出在《西部世界》（1973）中误认了 6502 汇编代码，后来意识到 6502 当时尚未问世。另一条评论提到了类似的互联网电影汽车数据库（IMCDB）。

**标签**: `#computers`, `#movies`, `#pop culture`, `#curation`, `#retro computing`

---

<a id="item-12"></a>
## [免费在线编译器教科书发布](https://dthain.github.io/books/compiler/) ⭐️ 7.0/10

一本名为《编译器和语言设计导论》的免费在线教科书已发布，基于 Thain 博士的大学课程。 这本教科书为学习编译器构造提供了实用且易于获取的资源，这是计算机科学教育的核心主题。 该书包含一个示例项目，指导学生逐步构建一个可工作的 C 风格编译器，与课程项目类似。

hackernews · AlexeyBrin · Jul 5, 11:54 · [社区讨论](https://news.ycombinator.com/item?id=48793454)

**背景**: 编译器将高级编程语言翻译成机器代码。理解编译器设计对于语言开发者和高级程序员至关重要。

**社区讨论**: 前学生强烈推荐这本书，称赞 Thain 博士的教学和动手项目。一些评论者还建议了相关资源，如 C4 和 C4x86。

**标签**: `#compilers`, `#language design`, `#education`, `#programming languages`

---

<a id="item-13"></a>
## [用 445 字节和 Deflate 压缩生成世界地图](https://simonwillison.net/2026/Jul/4/building-a-world-map-with-only-500-bytes/#atom-everything) ⭐️ 7.0/10

Iwo Kadziela 通过 deflate 压缩地图数据，并使用 JavaScript 代码片段通过 fetch 获取 data URI 并利用 DecompressionStream API 解压，生成了一个仅 445 字节的 ASCII 世界地图。 这展示了 web API（fetch 与 data URI 结合、DecompressionStream）与压缩技术的巧妙组合，实现了极致的数效率，为在极少量字节中嵌入丰富内容提供了新思路。 压缩数据以 base64 编码的 data URI 形式存储，通过 fetch() 获取，然后经 DecompressionStream('deflate-raw') 解压，最后以 <pre> 元素并设置小字号渲染。

rss · Simon Willison · Jul 4, 23:09

**背景**: Deflate 是一种无损压缩算法，广泛用于 PNG 和 ZIP 等格式。DecompressionStream API 是 Compression Streams 标准的一部分，允许在浏览器中进行流式解压。Data URI 将数据直接嵌入 URL，而 fetch() 可以像获取 HTTP 资源一样获取它们。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/DecompressionStream">DecompressionStream - Web APIs | MDN</a></li>
<li><a href="https://stackoverflow.com/questions/66573468/why-can-i-fetch-data-uris">javascript - Why can I fetch data URIs ? - Stack Overflow</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论（条目 48747762）非常积极，许多人称赞压缩和 web API 的巧妙运用。一些评论者讨论了替代压缩方法以及该方法的优雅之处。

**标签**: `#compression`, `#web APIs`, `#ASCII art`, `#JavaScript`, `#data URI`

---

<a id="item-14"></a>
## [韩国拟投 800 万亿韩元建半导体集群，DRAM 产量目标五年翻倍](https://t.me/zaihuapd/42357) ⭐️ 7.0/10

韩国产业通商资源部公布半导体全国集群计划，投资 800 万亿韩元（约 3.52 万亿元人民币）在西南圈建设 4 座内存晶圆厂，目标在五年内将 DRAM 产量翻倍。 这一巨额投资凸显了韩国保持全球内存市场领先地位的决心，尤其是在 AI 驱动的高带宽内存（HBM）需求正挤压通用 DRAM 供应的背景下，此举可能重塑半导体产业格局。 该计划包括在西南圈打造第二半导体生产基地，政府还将在 15 年内投入 30 万亿韩元用于相关基础设施。全球内存市场预计将在五年内实现四倍以上增长。

telegram · zaihuapd · Jul 4, 15:15

**背景**: DRAM（动态随机存取存储器）是一种易失性存储器，广泛用作计算机和显卡的主内存。韩国的三星电子和 SK 海力士是全球三大 DRAM 供应商之二（另一家为美光科技）。该集群计划旨在巩固其在 AI 和数据中心需求增长背景下的竞争优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random-access memory - Wikipedia</a></li>
<li><a href="https://baike.baidu.com/item/半导体与集成电路产业集群/67318946">半导体与集成电路产业集群_百度百科</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#DRAM`, `#South Korea`, `#manufacturing`, `#investment`

---

<a id="item-15"></a>
## [Linux 登顶 2026 CVE 榜单，维护者称这是好事](https://linuxiac.com/linux-tops-2026-cve-charts/) ⭐️ 7.0/10

这凸显了开源与专有软件在漏洞披露上的系统性差异：商业厂商往往只上报高危 CVE，而开源项目则报告所有已知问题。它挑战了“高 CVE 数量等于安全性差”的常见认知。 Greg Kroah-Hartman 指出，苹果、微软等商业厂商往往只上报被归类为“高危”的 CVE，而开源项目因无法预知下游使用场景，不得不报告所有问题。他呼吁其他厂商“行动起来”，全面上报 CVE，而非选择性提交。

telegram · zaihuapd · Jul 4, 16:00

**背景**: CVE（通用漏洞与暴露）是一个公开的网络安全漏洞目录，由 CVE 项目管理。每个 CVE ID 由 CNA（CVE 编号授权机构）在漏洞报告并验证后分配。Linux 内核运行在全球数十亿台设备上，全面的 CVE 报告对于下游用户评估风险至关重要。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nvd.nist.gov/general/cve-process">NVD - CVEs and the NVD Process</a></li>
<li><a href="https://www.cve.org/">CVE : Common Vulnerabilities and Exposures</a></li>
<li><a href="https://en.wikipedia.org/wiki/Greg_Kroah-Hartman">Greg Kroah - Hartman - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Linux`, `#CVE`, `#security`, `#open source`, `#vulnerability reporting`

---

<a id="item-16"></a>
## [三星计划第三季度 DRAM 涨价约 20%](https://t.me/zaihuapd/42362) ⭐️ 7.0/10

三星电子计划在第三季度将 DRAM 价格上调约 20%，并已口头通知部分客户。该公司尚未就定价发布正式评论。 此次涨价反映了供应紧张以及 AI 服务器和先进设备需求的持续强劲，直接影响数据中心和 AI/ML 系统的硬件成本。行业分析师预计内存市场将出现类似的涨价。 TrendForce 预计第三季度 DRAM 合约价环比上涨 13%至 18%，NAND 闪存合约价环比上涨 10%至 15%；Sigmaintell Consulting 预计 LPDDR5X 8 GB 芯片合约价上涨约 20%。

telegram · zaihuapd · Jul 5, 04:03

**背景**: DRAM（动态随机存取存储器）是一种易失性存储器，广泛用作计算机和服务器的主内存。NAND 闪存是一种非易失性存储技术，用于 SSD 和存储卡。LPDDR5X 是一种低功耗 DRAM 变体，常用于移动设备和 AI 应用。内存市场由三大供应商主导：三星、SK 海力士和美光。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DRAM">DRAM</a></li>
<li><a href="https://en.wikipedia.org/wiki/NAND_flash">NAND flash</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#Samsung`, `#memory pricing`, `#AI infrastructure`, `#supply chain`

---

<a id="item-17"></a>
## [卫报调查：OpenAI 从未到访星际之门英国选址](https://www.theguardian.com/technology/2026/jul/04/openai-apparent-failure-visit-key-site-questions-stargate-uk-project) ⭐️ 7.0/10

《卫报》调查发现，OpenAI 从未实地造访其星际之门项目的英国核心选址——北泰恩赛德的 Cobalt Park 商业园区，当地政府也从未与 OpenAI 或合作方 Nscale 举行过会议。该项目已于 2026 年 4 月暂停，知情人士称其为政府公关噱头。 此事对 OpenAI 300 亿美元投资承诺的可信度构成质疑，并引发对重大 AI 基础设施公告透明度的担忧。这可能削弱对科技公司承诺的信任，并影响英国科技政策及国际投资关系。 星际之门英国项目是在特朗普访英期间作为英美 AI 合作旗舰工程宣布的。该项目因监管环境和能源成本过高而暂停，当地保守党议员表示项目落地“看起来极不可能”。

telegram · zaihuapd · Jul 5, 05:09

**背景**: 星际之门是 OpenAI 的一项大规模 AI 基础设施计划，最初设想在全球范围内投资高达 1 万亿美元建设数据中心。英国项目是该计划的关键部分，但《卫报》的调查表明，该项目可能在未经适当尽职调查的情况下宣布，可能是一种政治姿态。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://thenextweb.com/news/openai-apparently-never-visited-the-site-of-its-flagship-uk-ai-project">OpenAI never visited its Stargate UK site, Guardian finds</a></li>
<li><a href="https://www.evolmagazine.com/en/news/ai/openai-stargate-plan-trillion-global-data-centers.html">OpenAI Stargate Plan: $1 Trillion in AI Data Centers</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cobalt_Park">Cobalt Park - Wikipedia</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Stargate`, `#AI infrastructure`, `#investigative journalism`, `#UK tech policy`

---

<a id="item-18"></a>
## [中国初创公司测试二氧化碳冷发射火箭技术](https://www.techradar.com/pro/chinese-tests-rocket-using-the-same-gas-used-by-coca-cola-to-make-space-flights-cheaper-safer-cleaner-and-cooler) ⭐️ 7.0/10

中国初创公司湖南智宇航天科技与奇阳空间动力科技合作，正在测试一种使用超临界二氧化碳将火箭弹射出去后再点燃发动机的冷发射系统。 如果成功，该技术可通过避免传统发射产生的极端热损伤，大幅降低发射基础设施成本并提高发射频率，可能彻底改变小型液体燃料火箭的发射模式。 超临界 CO₂是在高温高压下达到的流体状态，能瞬间膨胀产生高压气体用于弹射。该系统针对小型运载火箭设计，目前仍处于实验阶段。

telegram · zaihuapd · Jul 5, 13:29

**背景**: 冷发射技术由苏联首创，利用气体将导弹或火箭从发射装置中弹出后再点燃主发动机，从而减少对发射设施的热应力和机械应力。超临界二氧化碳是一种无毒、廉价的物质，常用于碳酸饮料。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3359056/can-chinas-co2-rocket-launch-cold-same-gas-carbonates-coca-cola">Can China’s ‘CO2 rocket’ launch cold on the same gas that carbonates Coca-Cola? | South China Morning Post</a></li>
<li><a href="https://www.chinatechnews.com/2026/07/01/124743-can-chinas-co2-rocket-launch-cold-on-the-same-gas-that-carbonates-coca-cola">Can China’s ‘CO2 rocket’ launch cold on the same gas that ...</a></li>
<li><a href="https://www.techradar.com/pro/chinese-tests-rocket-using-the-same-gas-used-by-coca-cola-to-make-space-flights-cheaper-safer-cleaner-and-cooler">This Chinese startup thinks fizzy drink gas could make rocket launches dramatically cheaper and cleaner | TechRadar</a></li>

</ul>
</details>

**社区讨论**: 随新闻附带的 Telegram 评论语气轻松，指出标题是为了娱乐，但没有提供实质性的技术讨论。

**标签**: `#rocket technology`, `#aerospace`, `#cold launch`, `#carbon dioxide`, `#China`

---