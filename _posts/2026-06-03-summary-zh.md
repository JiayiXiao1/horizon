---
layout: default
title: "Horizon Summary: 2026-06-03 (ZH)"
date: 2026-06-03
lang: zh
---

> From 36 items, 15 important content pieces were selected

---

1. [黑客利用 Meta AI 机器人劫持 Instagram 账户](#item-1) ⭐️ 9.0/10
2. [Anthropic 将 Project Glasswing 扩展至 15 个国家](#item-2) ⭐️ 8.0/10
3. [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 大语言模型](#item-3) ⭐️ 8.0/10
4. [腾讯秘密为微信打造 AI 智能体，连接小程序](#item-4) ⭐️ 8.0/10
5. [老虎国际暂停中国境内账户新开仓](#item-5) ⭐️ 8.0/10
6. [特朗普签署人工智能行政令，要求企业自愿提交模型审查](#item-6) ⭐️ 8.0/10
7. [iOS 27 或为折叠屏 iPhone 引入分屏功能](#item-7) ⭐️ 8.0/10
8. [CT 扫描揭示比亚迪汽车零部件工程细节](#item-8) ⭐️ 7.0/10
9. [用户因侵入式 AI 功能离开 Gmail](#item-9) ⭐️ 7.0/10
10. [西雅图监控步行之旅揭露隐藏摄像头](#item-10) ⭐️ 7.0/10
11. [为什么你应该爱上 systemd 定时器](#item-11) ⭐️ 7.0/10
12. [Wise 因可疑交易在比利时接受调查](#item-12) ⭐️ 7.0/10
13. [Clash Verge Rev 的 CVD 协议引发隐私与兼容性争议](#item-13) ⭐️ 7.0/10
14. [农村老人困在“古稀陷阱”：谁来支付体面老去的账单？](#item-14) ⭐️ 7.0/10
15. [OpenAI 推出 Sites：Codex 将想法变为交互应用](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [黑客利用 Meta AI 机器人劫持 Instagram 账户](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 9.0/10

黑客通过简单要求 Meta 的 AI 支持聊天机器人将新邮箱地址关联到高知名度 Instagram 账户，成功劫持了包括奥巴马白宫账户在内的多个账号。 此事件揭示了将 AI 聊天机器人与敏感账户恢复系统集成时的严重安全漏洞，可能影响数百万用户并削弱对 AI 驱动客户支持的信任。 该攻击是一种提示注入，机器人被欺骗绕过了双重身份验证等标准验证步骤。Meta 尚未发布修复方案或官方声明。

rss · Simon Willison · Jun 1, 21:14

**背景**: 提示注入是一种攻击者通过精心构造输入来覆盖 AI 聊天机器人预期行为的技术。在此案例中，Meta 的 AI 支持机器人被赋予了执行账户恢复操作的能力，黑客通过简单要求其关联新邮箱来利用这一能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/01/meta-ai-hack-obama-sephora-instagram">Hackers trick Meta AI support bot to infiltrate Obama White House Instagram account | Meta | The Guardian</a></li>
<li><a href="https://techcrunch.com/2026/06/01/hackers-hijacked-instagram-accounts-by-tricking-meta-ai-support-chatbot-into-granting-access/">Hackers hijacked Instagram accounts by tricking Meta AI support chatbot ...</a></li>
<li><a href="https://cybersecuritynews.com/metas-ai-support-bot-instagram/">Hackers Use Meta's AI Bot to Reset Passwords and Hijack Instagram Accounts</a></li>

</ul>
</details>

**社区讨论**: 社区表达了震惊和批评，许多人指出这是一个明显的设计缺陷。一些网络安全专家表示，这种攻击几乎算不上提示注入，因为机器人本就被设计为执行被诱骗执行的操作。

**标签**: `#security`, `#AI`, `#Meta`, `#prompt injection`, `#account takeover`

---

<a id="item-2"></a>
## [Anthropic 将 Project Glasswing 扩展至 15 个国家](https://www.anthropic.com/news/expanding-project-glasswing) ⭐️ 8.0/10

Anthropic 宣布将其使用 Claude Mythos AI 模型的安全扫描计划 Project Glasswing 扩展至 15 个国家的关键基础设施。 此次扩展将先进 AI 用于关键系统的漏洞检测，可能提升全球网络安全，但也引发了关于访问权限和可靠性的担忧。 Claude Mythos 是一个旨在发现软件漏洞的大型语言模型，但由于安全顾虑尚未公开发布。社区反馈指出存在误报和计算能力有限的问题。

hackernews · surprisetalk · Jun 2, 13:15 · [社区讨论](https://news.ycombinator.com/item?id=48369863)

**背景**: Project Glasswing 是 Anthropic 于 2026 年 4 月发起的网络安全计划，旨在利用 AI 保护关键软件基础设施。Claude Mythos 是一个被内部描述为能力“阶跃变化”的先进模型，但其受限预览引发了褒贬不一的反应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Glasswing">Project Glasswing</a></li>
<li><a href="https://www.anthropic.com/research/glasswing-initial-update">Project Glasswing: An initial update \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了怀疑：一些用户报告该工具产生大量误报和噪音，而另一些人质疑 Anthropic 的动机，认为计算能力不足被伪装成安全问题。此外，一些安全专业人士指出，即使是大型组织也难以获得访问权限。

**标签**: `#AI`, `#security`, `#Anthropic`, `#critical infrastructure`, `#Claude`

---

<a id="item-3"></a>
## [微软发布 MAI-Thinking-1 和 MAI-Code-1-Flash 大语言模型](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

微软宣布了两款新的文本大语言模型：MAI-Thinking-1，一个 1 万亿参数、35 亿活跃参数的推理模型；以及 MAI-Code-1-Flash，一个 1370 亿参数、50 亿活跃参数的代码模型，专为 GitHub Copilot 构建。 这些模型展示了微软利用混合专家架构推动高效、专业化 AI 的努力，声称在性能上与 Claude Opus 4.6 等更大模型竞争。代码模型集成到 GitHub Copilot 中可能显著影响开发者工作流程。 MAI-Thinking-1 是一个稀疏 MoE 模型，总参数 1 万亿，但仅 35 亿活跃，使用企业级数据训练，未从第三方模型蒸馏。MAI-Code-1-Flash 正在向 VS Code 中的 GitHub Copilot 个人用户推出，由微软端到端构建，使用干净且适当许可的数据。

rss · Simon Willison · Jun 2, 22:21

**背景**: 混合专家（MoE）模型每个 token 仅激活部分参数，从而在较低推理成本下实现更大的总容量。微软的 MAI 模型是面向推理和代码生成等特定任务的专用高效大语言模型这一更广泛趋势的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI-Thinking-1 - Microsoft AI</a></li>
<li><a href="https://microsoft.ai/news/introducingmai-code-1-flash/">Introducing MAI-Code-1-Flash | Microsoft AI</a></li>
<li><a href="https://github.blog/changelog/2026-06-02-mai-code-1-flash-is-now-available-for-github-copilot/">MAI-Code-1-Flash is now available for GitHub Copilot - GitHub Changelog</a></li>

</ul>
</details>

**标签**: `#LLM`, `#Microsoft`, `#AI models`, `#reasoning`, `#code generation`

---

<a id="item-4"></a>
## [腾讯秘密为微信打造 AI 智能体，连接小程序](https://t.me/zaihuapd/41705) ⭐️ 8.0/10

据外媒援引四位知情人士称，腾讯正秘密为微信打造一款 AI 智能体，旨在连接数百万个小程序，让智能体代用户完成预约出租车、订购杂货等任务。 如果成功，该 AI 智能体可利用微信 14 亿月活跃用户，成为 AI 驱动服务的领先平台，加剧与阿里巴巴和字节跳动在中国 AI 市场的竞争。 该智能体旨在与微信内运行的数百万个小程序协作，可能自动化大量日常任务。腾讯尚未回应置评请求。

telegram · zaihuapd · Jun 2, 05:03

**背景**: 微信是腾讯开发的超级应用，集成了即时通讯、社交媒体、移动支付和数千个第三方小程序。小程序是轻量级应用，无需单独安装即可在微信内运行，涵盖从电商到交通等服务。AI 智能体是能自主代用户执行任务的软件程序，将其与消息平台集成是科技行业的一个增长趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WeChat_Mini_Program">WeChat Mini Program</a></li>
<li><a href="https://walkthechat.com/wechat-mini-programs-simple-introduction/">What are WeChat Mini-Programs? A Simple Introduction - WalktheChat</a></li>

</ul>
</details>

**标签**: `#AI Agent`, `#WeChat`, `#Tencent`, `#Mini Programs`, `#China Tech`

---

<a id="item-5"></a>
## [老虎国际暂停中国境内账户新开仓](https://mp.weixin.qq.com/s/LgwHvOhuFw338kvWPgPyvw) ⭐️ 8.0/10

老虎国际宣布，自 2026 年 6 月 12 日起，为落实监管要求，暂停中国境内账户所有品种的新开仓和加仓操作，仅保留卖出、平仓功能。 这标志着中国打击非法跨境证券活动的重要一步，影响大量使用境外券商的内地投资者，预示着监管趋严，可能重塑跨境交易格局。 暂停适用于所有证券品种，包括股票，同时暂停境内资金转入，转出服务正常。现有资产及境外服务不受影响。

telegram · zaihuapd · Jun 2, 12:56

**背景**: 中国证监会等八部门近期联合印发《综合整治非法跨境证券期货基金经营活动实施方案》，针对老虎证券、富途证券等境外券商，要求用两年时间清理存量非法业务，禁止其招揽境内客户或开立新账户。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.stcn.com/article/detail/3922656.html">中国证监会等八部门联合印发《综合整治非法跨境证券期货基金经营活动实施方案》</a></li>
<li><a href="https://www.news.cn/fortune/20260522/d155e2db294442bfb63d0bddb97cc9cc/c.html">财经深一度丨强监管聚合力 8部门重拳整治非法跨境证券期货基金经营活动-新华网</a></li>
<li><a href="https://www.yicai.com/news/103198159.html">八部门联手综合整治非法跨境展业，境外券商无牌经营“灰色时代”终结</a></li>

</ul>
</details>

**标签**: `#regulatory`, `#fintech`, `#cross-border trading`, `#China`, `#securities`

---

<a id="item-6"></a>
## [特朗普签署人工智能行政令，要求企业自愿提交模型审查](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

美国总统特朗普于 2026 年 6 月 2 日签署了一项行政命令，建立了一个自愿性框架，要求 AI 开发者在公开发布先进模型前 30 天提交给政府进行网络安全审查，并成立了一个 AI 网络安全清算所。 该行政令标志着美国向自愿性、对行业友好的 AI 监管转变，在国家安全关切与维持美国 AI 领先地位之间取得平衡。它可能为未来的 AI 治理树立先例，并影响全球监管趋势。 最终命令将早期草案中的 90 天审查期缩短为 30 天，并明确禁止强制性的政府许可或预检机制。AI 网络安全清算所将协调政府和关键基础设施领域的漏洞发现与修复。

telegram · zaihuapd · Jun 2, 16:44

**背景**: 该行政令是美国持续监管 AI 努力的一部分，此前有拜登政府的 AI 行政令等尝试。自愿性框架旨在应对先进 AI 模型带来的网络安全风险，同时不扼杀创新，此前行业对强制性要求表示反对。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives | Federal News Network</a></li>
<li><a href="https://www.cybersecuritydive.com/news/trump-ai-security-executive-order/821755/">Trump signs EO seeking early government access to powerful AI models | Cybersecurity Dive</a></li>
<li><a href="https://www.csoonline.com/article/4180205/trump-revives-parts-of-canceled-ai-order-with-cybersecurity-focused-directive.html">Trump revives parts of canceled AI order with cybersecurity-focused directive | CSO Online</a></li>

</ul>
</details>

**社区讨论**: 社区评论对该行政令的实质内容表示怀疑，有人称其为最终禁止开源模型的'关门'步骤。其他人则质疑自愿审查的实际实施，并指出从 90 天减少到 30 天是行业的胜利。

**标签**: `#AI regulation`, `#executive order`, `#cybersecurity`, `#US policy`, `#AI safety`

---

<a id="item-7"></a>
## [iOS 27 或为折叠屏 iPhone 引入分屏功能](https://www.macrumors.com/2026/06/02/ios-27-split-screen-app-adaptation-feature/) ⭐️ 8.0/10

据 MacRumors 报道，苹果正在 iOS 27 中开发一项系统级横屏适配功能，可自动将竖屏应用调整为宽屏布局，从而在传闻中拥有 7.8 英寸内屏的折叠屏 iPhone 上实现分屏多任务。该功能预计将在 WWDC 2026 上公布。 这将解决 iOS 在大屏幕上长期存在的短板，可能加速折叠屏 iPhone 的普及，并使 iOS 生态与 iPadOS 的多任务能力对齐。同时，它还能减轻开发者负担，无需手动重新设计应用。 该功能是系统级的，可自动生效，无需开发者干预，类似于 iPadOS 处理应用缩放的方式。传闻中的折叠屏 iPhone 据称配备 5.5 英寸外屏和 7.8 英寸内屏，折叠厚度 9.5 毫米，展开仅 4.5 毫米。

telegram · zaihuapd · Jun 3, 02:02

**背景**: iOS 历来缺乏强大的分屏多任务功能，而 Android 折叠屏手机已提供该功能多年。苹果的 iPadOS 已支持分屏和侧拉，但 iPhone 应用通常为竖屏设计。系统级适配将弥合这一差距，无需开发者单独创建布局。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://post.smzdm.com/p/aggzp65w/">等了 6 年！ 苹果 折 叠 屏 iPhone ...</a></li>

</ul>
</details>

**标签**: `#iOS`, `#foldable`, `#split-screen`, `#WWDC`, `#Apple`

---

<a id="item-8"></a>
## [CT 扫描揭示比亚迪汽车零部件工程细节](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield 发布了比亚迪汽车零部件的高分辨率 CT 扫描图像，包括钥匙、驱动单元和电池包，以前所未有的方式展示了其内部工程结构。 这挑战了外界对中国汽车质量的负面看法，展示了坚固且设计精良的零部件，并凸显了比亚迪的垂直整合能力和制造规模。 扫描图像显示了比亚迪钥匙中的机械备用钥匙、集成电机和逆变器的驱动单元，以及刀片电池包。比亚迪约 75%的零部件自产，比例与特斯拉相当但规模更大。

hackernews · viasfo · Jun 2, 20:30 · [社区讨论](https://news.ycombinator.com/item?id=48375824)

**背景**: 比亚迪是一家中国汽车制造商和电池生产商，从锂矿开采到整车组装实现垂直整合。CT 扫描利用 X 射线生成横截面图像，可无损检测内部结构。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BYD_Auto">BYD Auto - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论总体积极，一位高级技师称赞比亚迪 Shark 车型的坚固做工。有用户纠正了关于钥匙机械结构的细节，另一用户指出比亚迪产量超过特斯拉。

**标签**: `#BYD`, `#EV`, `#engineering`, `#teardown`, `#automotive`

---

<a id="item-9"></a>
## [用户因侵入式 AI 功能离开 Gmail](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 7.0/10

一位用户公开宣布离开 Gmail，原因是谷歌强行整合 AI 功能（如智能回复和邮件撰写），并转而使用 Fastmail。 这反映了用户对优先考虑便利性而非用户自主权的 AI 功能日益增长的反感，并凸显了免费服务与 Fastmail 等付费替代方案之间的权衡。 该用户称赞 Fastmail 速度快、操作即时，并具备应用密码和隐藏邮箱等功能，但指出其日历缺少地址自动补全。

hackernews · speckx · Jun 2, 19:27 · [社区讨论](https://news.ycombinator.com/item?id=48375016)

**背景**: Gmail 一直在集成由 Gemini 驱动的 AI 功能，如智能撰写和建议回复，部分用户认为这些功能具有侵入性且不必要。Fastmail 是一款付费电子邮件托管服务，以速度和隐私著称，提供简洁的界面，没有 AI 驱动的建议。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fastmail">Fastmail - Wikipedia</a></li>
<li><a href="https://www.fastmail.com/">Email and calendar made better | Fastmail</a></li>
<li><a href="https://www.expressvpn.com/blog/gmail-ai-privacy-risks/">Your guide to understanding Google Gmail AI security</a></li>

</ul>
</details>

**社区讨论**: 评论者就 AI 在邮件中的价值展开辩论，一些人认为智能回复对简单回复有用，但批评冗长的 LLM 生成草稿。其他人指出，许多“Gmail 杀手”只是付费服务，而 Fastmail 和 HEY 提供了不同的心智模型。

**标签**: `#email`, `#AI`, `#privacy`, `#user experience`, `#Gmail`

---

<a id="item-10"></a>
## [西雅图监控步行之旅揭露隐藏摄像头](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 7.0/10

coveillance.org 上记录的一次西雅图步行之旅，绘制了该市广泛的监控基础设施，包括摄像头、车牌读取器和 Amazon Go 追踪技术，并强调了它们对隐私和社会规范的影响。 这次旅行提高了人们对公共场所监控常态化的关键认识，引发了关于隐私、公民自由以及技术以微妙方式强制社会遵从的公众辩论。 这次旅行涵盖了各种监控技术，如自动车牌读取器、交通监控设备和商店追踪系统，重点在于摄像头如何编码“观看方式”以强制社会规范。

hackernews · eustoria · Jun 2, 13:24 · [社区讨论](https://news.ycombinator.com/item?id=48369980)

**背景**: 自 9/11 以来，西雅图等城市的监控基础设施显著扩展，摄像头和传感器变得无处不在。这些系统通常以公共安全为理由，但引发了隐私和公民自由侵蚀的担忧。这次步行之旅作为实地指南，旨在让公众看到这些隐藏的技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://all-waterparks.com/general/a-walking-tour-of-surveillance-infrastructure-in-seattle/">A walking tour of surveillance infrastructure in Seattle - All Waterparks</a></li>
<li><a href="https://flipso.com/p/9wdryxgwl">A walking tour of surveillance infrastructure in Seattle · Flipso | Flipso</a></li>
<li><a href="https://www.kaggle.com/datasets/city-of-seattle/seattle-surveillance-technologies">Seattle Surveillance Technologies | Kaggle</a></li>

</ul>
</details>

**社区讨论**: 评论表达了不同观点：一些人认为监控是“新常态”并质疑其有效性（例如，检察官需要视频证据），而另一些人则批评这次旅行使用的学术语言难以理解。少数评论者哀叹自由的丧失以及政府与企业的勾结。

**标签**: `#surveillance`, `#privacy`, `#Seattle`, `#civil liberties`, `#technology`

---

<a id="item-11"></a>
## [为什么你应该爱上 systemd 定时器](https://blog.tjll.net/you-dont-love-systemd-timers-enough/) ⭐️ 7.0/10

一篇博客文章主张 systemd 定时器优于 cron 用于 Linux 任务调度，强调了可预测路径、对系统启动时间的弹性以及更好的 systemd 生态系统集成等优势。 这很重要，因为 systemd 定时器解决了 cron 的关键限制，例如系统停机期间错过任务，并提供与现代 Linux 系统更紧密的集成，使其成为系统管理员更稳健的选择。 与 cron 的单个 crontab 条目相比，systemd 定时器需要两个文件（一个 .timer 单元和一个 .service 单元），有些人认为这是一个缺点。然而，它们支持单调定时器、随机延迟和持久定时器等功能，可在启动后运行错过的任务。

hackernews · yacin · Jun 2, 09:34 · [社区讨论](https://news.ycombinator.com/item?id=48367904)

**背景**: Cron 是传统的 Linux 任务调度器，在固定时间运行任务，但如果系统关闭则会跳过任务。systemd 定时器是 systemd 初始化系统的一部分，提供更灵活的调度、通过 journalctl 记录日志以及依赖管理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://xtom-dev.pages.dev/blog/systemd-vs-cron-linux-task-scheduling/">Systemd Timers vs . Cron : Which One Should You Use? | xTom</a></li>
<li><a href="https://medium.com/@tolulinux/linux-scheduled-cron-vs-systemd-timer-738dedcc6a71">Linux Scheduled: Cron vs Systemd timers | by Tolulope... | Medium</a></li>
<li><a href="https://unix.stackexchange.com/questions/278564/cron-vs-systemd-timers">Cron vs systemd timers - Unix & Linux Stack Exchange</a></li>

</ul>
</details>

**社区讨论**: 评论意见不一：一些人称赞定时器的弹性和 journalctl 集成，而另一些人则批评需要两个文件过于繁琐。一位用户分享了备份自动化的实际用例，另一位用户幽默地描述了使用定时器每周打印一张狗狗图片。

**标签**: `#systemd`, `#cron`, `#Linux`, `#scheduling`, `#system administration`

---

<a id="item-12"></a>
## [Wise 因可疑交易在比利时接受调查](https://www.thebureauinvestigates.com/stories/2026-06-01/money-transfer-giant-wise-investigated-for-half-a-billion-in-suspicious-transactions) ⭐️ 7.0/10

比利时检方正在调查 Wise 涉嫌未遵守反洗钱法规，涉及欧洲范围内约 5 亿欧元的可疑交易。 此次调查可能削弱对 Wise 乃至整个金融科技行业的信任，凸显跨境执行反洗钱合规的挑战。 调查涉及来自 30 多个欧洲国家的数百项司法请求，Wise 的美国子公司此前曾因类似违规被罚款 420 万美元。

telegram · zaihuapd · Jun 2, 03:59

**背景**: 反洗钱法规要求金融机构核实客户身份并报告可疑活动。Wise 是一家总部位于英国的汇款金融科技公司，已在多个司法管辖区因合规问题受到监管审查。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.bankingdive.com/news/wise-aml-investigation-europe/821721/">Fintech Wise probed over AML concerns | Banking Dive</a></li>
<li><a href="https://fintechnews.sg/132383/payments/wise-money-laundering/">Wise Faces Belgium Probe Over Money Laundering Control...</a></li>

</ul>
</details>

**标签**: `#fintech`, `#regulatory`, `#anti-money laundering`, `#compliance`, `#investigation`

---

<a id="item-13"></a>
## [Clash Verge Rev 的 CVD 协议引发隐私与兼容性争议](https://github.com/clash-verge-rev/clash-verge-rev/commit/2cb9c13ab6f0b0fec5ccc622c669843c935942ed) ⭐️ 7.0/10

Clash Verge Rev 在 dev 分支引入了一项名为 CVD（Clash Verge 设备绑定协议）的新订阅安全机制，通过生成设备密钥并按设备加密下发订阅，以防止订阅 URL 被滥用。 该协议解决了订阅 URL 泄露和批量滥用的实际问题，但同时也引入了隐私风险，因为生成了持久的设备标识符，并可能降低与第三方客户端和跨设备同步的兼容性。 CVD 协议仍处于早期开发阶段，大部分由 AI 生成，尚未实际部署；其可行性需要社区进一步讨论和分析。

telegram · zaihuapd · Jun 2, 11:07

**背景**: Clash Verge Rev 是一款基于 Tauri 框架的流行开源代理客户端，支持 Windows、macOS 和 Linux。传统的订阅 URL 一旦泄露，可被无限复制并被多台设备使用，导致滥用。CVD 旨在通过要求客户端上报公钥，将订阅绑定到特定设备，从而允许服务器限制设备数量并撤销访问权限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/clash-verge-rev/clash-verge-rev">GitHub - clash - verge - rev / clash - verge - rev : A modern GUI client based...</a></li>
<li><a href="https://talkin.icu/blog/cvd-device-binding-privacy-risks">CVD Device Binding : Privacy Risks Explained</a></li>
<li><a href="https://clash-verge.org/">Clash Verge - Modern Cross-Platform Proxy Client | Open Source...</a></li>

</ul>
</details>

**社区讨论**: 社区意见分歧：一些人赞赏这种防止订阅滥用的安全改进，而另一些人则担心设备指纹识别的隐私影响以及强制采用可能破坏现有工作流程。

**标签**: `#proxy`, `#security`, `#privacy`, `#open-source`, `#protocol`

---

<a id="item-14"></a>
## [农村老人困在“古稀陷阱”：谁来支付体面老去的账单？](https://www.caixin.com/2026-06-01/102449600.html) ⭐️ 7.0/10

财新分析揭示，中国农村老年人面临“古稀陷阱”，每月约 250 元的养老金不足以维持生活，迫使他们在老年继续劳动。 这凸显了中国社会保障的系统性缺口，影响约 2.6 亿低收入人口（90%在农村），并引发代际公平担忧，年轻劳动者质疑现收现付制度的可持续性。 农村养老金仅为城镇职工养老金的 1/15，低于农村最低生活保障标准 594 元。“古稀陷阱”指 70 岁后劳动能力下降，但养老金未能充分替代，收入急剧下降。

telegram · zaihuapd · Jun 2, 15:47

**背景**: 中国的双轨制养老金体系为城镇职工提供优厚待遇，而农村居民依赖基础计划。传统上，土地和家庭支持充当安全网，但城市化和土地碎片化削弱了这些。“古稀陷阱”概念由学术文献提出，描述农村老年人在 70 岁左右面临的收入崩溃。

<details><summary>参考链接</summary>
<ul>
<li><a href="http://njnydxxbskb.paperonce.org/oa/pdfdow.aspx?Sid=20220405">标题</a></li>
<li><a href="https://www.workercn.cn/papers/grrb/2024/07/12/6/grrb202407126.pdf">workercn.cn/papers/grrb/2024/07/12/6/grrb202407126.pdf</a></li>

</ul>
</details>

**标签**: `#rural aging`, `#social security`, `#China`, `#pension gap`, `#economic inequality`

---

<a id="item-15"></a>
## [OpenAI 推出 Sites：Codex 将想法变为交互应用](https://x.com/OpenAI/status/2061845949170045346) ⭐️ 7.0/10

OpenAI 推出了 Sites 功能，该功能允许用户将工作内容、想法和计划转化为可通过 URL 访问的交互式网站或应用。该功能首先面向 Business 和 Enterprise 用户开放，后续将扩大覆盖范围。 Sites 降低了创建交互式 Web 应用的门槛，使非开发人员无需编码专业知识即可将想法转化为功能应用。这可能会加速组织内的原型设计和协作，扩大 AI 辅助开发的覆盖范围。 Sites 将本地源项目链接到由 Codex 管理的托管服务，并将链接信息存储在 .openai/hosting.json 文件中。该功能目前仅限于 Business 和 Enterprise 层级，尚未公布更广泛开放的定价或日期。

telegram · zaihuapd · Jun 2, 17:29

**背景**: OpenAI Codex 是一个将自然语言转化为代码的 AI 系统，为 GitHub Copilot 等工具提供支持。Sites 扩展了 Codex 的能力，允许将生成的代码直接部署为交互式 Web 应用，从而弥合了创意生成与功能软件之间的鸿沟。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developers.openai.com/codex/sites">Sites – Codex | OpenAI Developers</a></li>
<li><a href="https://grokipedia.com/page/OpenAI_Codex">OpenAI Codex</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Codex`, `#AI-assisted development`, `#interactive applications`, `#product launch`

---