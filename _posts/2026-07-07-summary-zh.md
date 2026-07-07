---
layout: default
title: "Horizon Summary: 2026-07-07 (ZH)"
date: 2026-07-07
lang: zh
---

> From 27 items, 13 important content pieces were selected

---

1. [OpenWrt One：开源硬件路由器发布](#item-1) ⭐️ 8.0/10
2. [Anthropic 发现大语言模型中的“全局工作空间”神经元](#item-2) ⭐️ 8.0/10
3. [腾讯发布 Hy3：295B MoE 模型，Apache 2.0 许可](#item-3) ⭐️ 8.0/10
4. [中国拟削减 SCI 发表激励以保安全](#item-4) ⭐️ 8.0/10
5. [FBI 通过微软 GDID 设备标识符追踪黑客](#item-5) ⭐️ 8.0/10
6. [B 站向开源项目 BiliRoaming 发律师函](#item-6) ⭐️ 8.0/10
7. [微软重塑 Xbox 以追求盈利](#item-7) ⭐️ 7.0/10
8. [硬科技专业毕业生薪资反超软件](#item-8) ⭐️ 7.0/10
9. [美国富人花数万美元让孩子接受 AI 教育](#item-9) ⭐️ 7.0/10
10. [微软近四成利润记在爱尔兰，当地员工仅占 3%](#item-10) ⭐️ 7.0/10
11. [SpaceX 猎鹰 9 号碎片在高空造成金属污染](#item-11) ⭐️ 7.0/10
12. [中国计划构建天地一体化小行星防御系统](#item-12) ⭐️ 7.0/10
13. [Claude Cowork 沙箱逃逸漏洞披露](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenWrt One：开源硬件路由器发布](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt 与软件自由保护协会联合推出了 OpenWrt One，这是首个完全上游支持的开源硬件路由器设计，于 2024 年底发布。 该项目使用户能够延长路由器寿命并获得超出制造商支持的高级功能，推动了网络领域的维修权和开源硬件发展。 OpenWrt One 基于 Banana Pi 板，并通过软件自由保护协会组织。它旨在为 OpenWrt 提供一个完全开放且受支持的硬件平台。

hackernews · peter_d_sherman · Jul 6, 18:23 · [社区讨论](https://news.ycombinator.com/item?id=48808482)

**背景**: OpenWrt 是一个基于 Linux 的开源嵌入式操作系统，主要用于网络路由。历史上，它作为第三方固件安装在不同路由器上，但 OpenWrt One 是首个专门为其设计的官方硬件。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt - Wikipedia</a></li>
<li><a href="https://lwn.net/Articles/957255/">The OpenWrt One project [LWN.net]</a></li>
<li><a href="https://www.theregister.com/2024/12/02/openwrt_one_foss_wifi_router/">Open source router firmware OpenWrt ships its own hardware</a></li>

</ul>
</details>

**社区讨论**: 社区评论总体积极，用户称赞 OpenWrt 延长了路由器寿命并增加了功能。一些人提到安装复杂性和对更快 LAN 端口的需求，而其他人则分享了使用该设备的个人经验。

**标签**: `#OpenWrt`, `#open hardware`, `#router`, `#networking`, `#open source`

---

<a id="item-2"></a>
## [Anthropic 发现大语言模型中的“全局工作空间”神经元](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic 的研究在语言模型中发现了一组“全局工作空间”神经元，它们能够跨不同任务整合信息，这与认知科学中的全局工作空间理论相呼应。 这项工作通过揭示语言模型如何实现连贯且上下文感知的行为，推进了机制可解释性研究，有望带来更安全、更可控的 AI 系统。 这些“全局工作空间”神经元是通过一种方法识别的，该方法测量层激活的微小变化对最终输出的影响程度，形成一个代表跨上下文共享推理的“J 空间”。

hackernews · in-silico · Jul 6, 17:44 · [社区讨论](https://news.ycombinator.com/item?id=48808002)

**背景**: 全局工作空间理论（GWT）是 20 世纪 80 年代提出的一种认知架构，它假设存在一个中央工作空间，来自专门模块的信息在此广播到大脑的其他部分，从而实现意识感知。Anthropic 的研究将这一概念应用于大语言模型，表明人工神经网络中也存在类似的整合机制。这是 Anthropic 更广泛的可解释性工作的一部分，旨在理解并确保像 Claude 这样的已部署模型的安全性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_workspace_theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/research/mapping-mind-language-model">Mapping the Mind of a Large Language Model \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍对这项可解释性工作表示赞赏，但质疑其与人类意识的类比，指出所识别的“J 空间”可能仅仅反映了一个抽象推理子空间，而非真正的意识。一些用户回忆起相关的实验，例如复制数学求解层以提高性能，表明这一领域将产生更多见解。

**标签**: `#interpretability`, `#language models`, `#AI research`, `#neural networks`, `#cognitive science`

---

<a id="item-3"></a>
## [腾讯发布 Hy3：295B MoE 模型，Apache 2.0 许可](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

腾讯发布了 Hy3，这是一个 2950 亿参数的混合专家（MoE）语言模型，拥有 210 亿激活参数和 38 亿 MTP 层参数，采用 Apache 2.0 许可证。该模型支持 256K 上下文长度，已在 Hugging Face 和 OpenRouter 上提供。 Hy3 的性能优于同类模型，并可媲美参数规模大 2-5 倍的旗舰开源模型，成为开源 AI 生态系统的重要补充。其 Apache 2.0 许可证鼓励广泛采用和进一步开发。 全精度模型在 Hugging Face 上为 598GB，而 FP8 量化版本为 300GB。该模型在 OpenRouter 上免费提供至 2026 年 7 月 21 日。

rss · Simon Willison · Jul 6, 23:57

**背景**: 混合专家（MoE）是一种机器学习技术，它将问题划分为由专门专家网络处理的区域，每次输入仅激活部分参数以提高效率。MTP（多令牌预测）是一种同时预测多个未来令牌以提升推理速度的技术。FP8 量化通过使用 8 位浮点数来减小模型大小并加速推理。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://verl.readthedocs.io/en/latest/advance/mtp.html">Guide to Using MTP in SFT/RL Training and Inference</a></li>

</ul>
</details>

**标签**: `#AI`, `#open-source`, `#LLM`, `#Mixture-of-Experts`, `#Tencent`

---

<a id="item-4"></a>
## [中国拟削减 SCI 发表激励以保安全](https://www.ft.com/content/64a811f1-b132-4211-8a8c-2252cf964039?syn-25a6b1a6=1) ⭐️ 8.0/10

中国政策制定者正讨论削减科研人员向 SCI 等国际期刊投稿的激励，并可能降低 SCI 论文在学术晋升和终身教职评定中的权重。国家自然科学基金委已要求受资助项目至少 20%的代表性论文发表于中文期刊。 这一政策转变可能显著改变全球科学出版格局，因为中国是国际期刊的主要贡献者。同时，它也引发了关于学术自由以及国家安全与开放科学之间平衡的担忧。 中国国安部上月指控一名研究人员在向国际期刊投稿中泄露核心装备结构与关键实验数据。一名材料学学者表示，因安全审查标准模糊且趋严，他已停止向外国期刊投稿。

telegram · zaihuapd · Jul 6, 01:03

**背景**: SCI（科学引文索引）是广泛使用的科学期刊索引数据库，在 SCI 期刊上发表论文一直是中国学术评价的关键指标。政府一直在推动国内期刊发展，以减少对外国平台的依赖并防止技术泄露。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.edu.cn/rd/gai_kuang/zhuan_jia_ping_shu/202004/t20200408_1720343.shtml">破除“SCI至上”，要从质量与分类评价入手-高校科技-中国教育和科研计算机网CERNET</a></li>
<li><a href="https://epaper.gmw.cn/gmrb/html/2025-06/26/nw.D110000gmrb_20250626_2-16.htm">打造自主可控的学术出版平台-光明日报-光明网</a></li>
<li><a href="https://www.nppa.gov.cn/xxfb/zcfg/gfxwj/202106/t20210623_4514.html">中共中央宣传部 教育部 科技部印发 《关于推动学术期刊繁荣发展的意见》的通知</a></li>

</ul>
</details>

**社区讨论**: 有群友猜测该政策可能是为了打击学术造假。讨论反映了不同观点，有人支持安全考量，也有人担心可能对研究质量和国际合作产生负面影响。

**标签**: `#science policy`, `#national security`, `#academic publishing`, `#China`, `#technology transfer`

---

<a id="item-5"></a>
## [FBI 通过微软 GDID 设备标识符追踪黑客](https://www.itnews.com.au/news/microsoft-device-telemetry-key-to-unmasking-alleged-scattered-spider-hacker-627148) ⭐️ 8.0/10

美国联邦调查局利用微软的全球设备标识符（GDID）逮捕了 19 岁黑客 Peter Stokes，该标识符是持久的设备级标识符，即使使用 VPN 也不会改变。 此案表明，执法部门可利用微软的 GDID 跨 VPN 追踪用户，这引发了全球 Windows 用户的重大隐私担忧。 GDID 在 Windows 安装时生成，并在更新后保持不变；用户若不重装系统则无法轻易更改。FBI 将 GDID 与代理日志以及 Snapchat、苹果和 Facebook 的账户数据进行交叉比对。

telegram · zaihuapd · Jul 6, 04:15

**背景**: GDID 代表全球设备标识符，是每个 Windows 安装所绑定的唯一字符串，微软用于设备遥测。与 IP 地址或浏览器指纹不同，GDID 不易伪造或更改，因此成为一种强大的追踪工具。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/windows-11-identifier-used-to-track-scattered-spider-perp-after-microsoft-shared-info-with-fbi-19-year-old-us-estonian-hacker-arrested-over-alleged-ties-to-infamous-extortion-group">Windows 11 identifier code used to track Scattered Spider perp after Microsoft shared info with FBI — 19-year-old US-Estonian hacker arrested over alleged ties to infamous extortion group | Tom's Hardware</a></li>
<li><a href="https://securityonline.info/microsoft-gdid-tracking/">Microsoft GDID Tracking: How Windows Caught a Hacker</a></li>
<li><a href="https://www.pcmag.com/news/a-hackers-arrest-reveals-microsoft-can-track-users-via-a-windows-device">A Hacker's Arrest Reveals Microsoft Can Track Users Via a Windows Device ID | PCMag</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#Microsoft`, `#device tracking`, `#law enforcement`

---

<a id="item-6"></a>
## [B 站向开源项目 BiliRoaming 发律师函](https://github.com/yujincheng08/BiliRoaming) ⭐️ 8.0/10

B 站委托律师事务所向开源项目 BiliRoaming 发出侵权告知函，要求其停止逆向工程并删除绕过区域限制和付费保护机制的代码。 此次法律行动凸显了版权执法与开源逆向工程之间的紧张关系，可能为平台如何处理修改客户端行为的第三方工具树立先例。 函件特别指出播放鉴权 Hook、将付费番剧改写为可观看、绕过安全传输锁定以及改写 CDN 回源盗用平台分发资源等行为。

telegram · zaihuapd · Jul 6, 08:21

**背景**: BiliRoaming 是一个 Android Xposed 模块，用于解除 B 站番剧内容的区域限制并提供其他小功能。Xposed 是一个框架，允许在不修改 APK 文件的情况下改变 Android 应用的行为。CDN 回源是指当 CDN 节点未缓存内容时，从源站获取资源的过程。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chiphell.com/thread-2842265-1-1.html">付费番剧解限制工具“哔哩漫游”收到 B 站 律师函，GitHub...</a></li>
<li><a href="https://modules.lsposed.org/module/me.iacn.biliroaming/">哔哩漫游/ BiliRoaming · Xposed Module Repository</a></li>
<li><a href="https://sourceforge.net/projects/biliroaming.mirror/">BiliRoaming download | SourceForge.net</a></li>

</ul>
</details>

**标签**: `#open-source`, `#reverse engineering`, `#legal`, `#Bilibili`, `#DMCA`

---

<a id="item-7"></a>
## [微软重塑 Xbox 以追求盈利](https://news.xbox.com/en-us/2026/07/06/resetting-xbox/) ⭐️ 7.0/10

微软在 2026 年 7 月的一篇博文中宣布对 Xbox 部门进行重大重组，旨在提高利润率并恢复增长。 此举标志着 Xbox 从追求市场份额转向可持续盈利的战略转变，反映了行业对成本控制的趋势，并可能重塑微软的游戏生态系统。 重组包括裁员和关闭工作室，CEO Asha 承认过去的企业管理不善，并允许部分工作室恢复独立运营。

hackernews · dijksterhuis · Jul 6, 14:18 · [社区讨论](https://news.ycombinator.com/item?id=48804993)

**背景**: Xbox 每季度营收约 50 亿美元，但利润率微薄且不增长，仅约 1.5-1.6 亿美元。游戏行业成本不断上升，并转向 Game Pass 等服务模式，而任天堂等竞争对手则专注于低成本、高销量的游戏。

**社区讨论**: 社区评论批评声强烈，用户称重组是“一团糟”，并指责前领导层战略失误。一些人对被裁员工表示同情，并赞赏新 CEO 的坦诚，而另一些人则怀疑微软因其工程导向的文化而永远无法在游戏领域成功。

**标签**: `#Xbox`, `#Microsoft`, `#gaming industry`, `#business strategy`, `#restructuring`

---

<a id="item-8"></a>
## [硬科技专业毕业生薪资反超软件](https://news.sina.com.cn/c/2026-07-05/doc-inifuaqy8947308.shtml) ⭐️ 7.0/10

麦可思研究院发布的《2026 年中国本科生就业报告》显示，2025 届毕业生中，微电子科学与工程和电子科学与技术薪资位居前两名，而计算机科学与技术、软件工程跌出前十。 这一变化表明中国产业升级重心正从互联网转向硬科技和智能制造，将影响学生的专业选择和高校资源分配。 2025 届本科生毕业半年后平均月收入为 6435 元，微电子科学与工程为 7814 元，电子科学与技术为 7752 元。该报告反映了硬件相关领域经济价值上升的广泛趋势。

telegram · zaihuapd · Jul 6, 06:34

**背景**: 多年来，由于互联网行业蓬勃发展，计算机科学与技术和软件工程一直占据高薪专业前列。但随着中国优先发展半导体自主可控和先进制造，对硬件人才的需求激增，推高了微电子和电子科学领域的薪资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.peopleapp.com/rmharticle/30049394366">哪些 专 业 就 业 好、收入高？_ 教育在线</a></li>
<li><a href="https://www.gk100.com/read_1212041133466.htm">电子科学与技术专业就业方向及前景!附2025大学排名及分数线-高考100</a></li>

</ul>
</details>

**标签**: `#education`, `#industry trends`, `#salary report`, `#hard tech`

---

<a id="item-9"></a>
## [美国富人花数万美元让孩子接受 AI 教育](https://www.theverge.com/ai-artificial-intelligence/961505/wealthy-ai-schools-alpha-forge-prep) ⭐️ 7.0/10

美国富裕家庭正将孩子送入 Forge Prep 和 Alpha School 等以 AI 授课的私立学校，每年学费高达 7.5 万美元，但批评者认为孩子被当作未经验证技术的测试对象。 这一趋势引发了对教育领域未受监管的 AI 应用、潜在不平等以及缺乏透明度的伦理担忧，因为学校不公布成果数据来证明 AI 优于传统方法。 Alpha School 联合创始人表示，女性权利、奴隶制历史等有争议的社会议题被排除在课程之外，部分校区覆盖 K-12 全学段。Forge Prep 首年收到 600 份申请，但仅提供 34 个名额。

telegram · zaihuapd · Jul 6, 07:19

**背景**: 教育中的 AI 是指利用人工智能实现个性化学习，通常用软件取代传统教师。Forge Prep 和 Alpha School 是严重依赖 AI 进行教学的私立机构，以人类“引导员”代替教师。批评者担心缺乏证据以及可能对儿童造成伤害。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://forgeprep.org/ai-head-of-school/">AI Head of School - Forge Prep</a></li>
<li><a href="https://alpha.school/learn-more/">Learn More About Alpha School | AI -Powered 2-Hour Learning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Alpha_School">Alpha School - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI in education`, `#ethics`, `#EdTech`, `#inequality`, `#privacy`

---

<a id="item-10"></a>
## [微软近四成利润记在爱尔兰，当地员工仅占 3%](https://www.techspot.com/news/113001-microsoft-new-eu-disclosure-shows-exactly-how-tech.html) ⭐️ 7.0/10

微软的欧盟披露文件显示，在截至 2025 年 6 月的财年中，公司近 40%的全球税前利润记在爱尔兰，而当地员工仅占全球约 3%。 这一披露凸显了大型科技公司激进的利润转移策略，削弱了高税率国家的税基，并引发了关于全球税制改革和企业透明度的辩论。 在德国、法国和意大利，利润率仅为个位数，其中德国报告的利润占比不到 0.5%；卢森堡的 34 名员工创造了 2.83 亿美元的税前收入，利润率高达 142%。

telegram · zaihuapd · Jul 6, 09:19

**背景**: 利润转移是指跨国公司将其利润从高税率管辖区转移到低税率管辖区（如爱尔兰，企业税率 12.5%）以减少税负。欧盟 2021 年的透明度指令要求大型公司按国别披露收入和纳税情况，从而暴露此类行为。OECD 的 BEPS 项目旨在通过协调规则打击税基侵蚀和利润转移。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://time.com/6326583/tax-shelters-multinational-corporations/">How Corporations Shift Profits to Avoid Taxes - TIME</a></li>
<li><a href="https://www.oecd.org/en/topics/base-erosion-and-profit-shifting-beps.html">Base erosion and profit shifting (BEPS) | OECD</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ireland_as_a_tax_haven">Ireland as a tax haven - Wikipedia</a></li>

</ul>
</details>

**标签**: `#tax avoidance`, `#Microsoft`, `#corporate transparency`, `#EU regulation`, `#profit shifting`

---

<a id="item-11"></a>
## [SpaceX 猎鹰 9 号碎片在高空造成金属污染](https://t.me/zaihuapd/42387) ⭐️ 7.0/10

一项发表在《自然》子刊上的新研究直接探测到 SpaceX 猎鹰 9 号火箭再入大气层产生的锂羽流，在 96 公里高度锂浓度飙升了 10 倍。 这是首次直接证据表明火箭再入碎片将可测量的金属污染引入高层大气，可能威胁臭氧层，并引发对日益增长航天工业的环境担忧。 锂羽流是在猎鹰 9 号上面级在欧洲上空失控再入约 20 小时后，利用高精度激光雷达探测到的。锂浓度比正常背景水平高出约 10 倍。

telegram · zaihuapd · Jul 6, 11:17

**背景**: 火箭级再入地球大气层时会燃烧，释放出锂、铝和铜等金属。这些金属可能在高层大气中积累，并可能催化消耗臭氧层的反应。激光雷达（LiDAR）是一种利用激光脉冲测量高空大气成分的遥感技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sciencenews.org/article/rocket-reentry-metal-pollution-detected">Metal pollution from a rocket reentry detected for the first time</a></li>
<li><a href="https://theconversation.com/spacex-rocket-left-behind-a-plume-of-chemical-pollution-as-it-burnt-up-in-the-atmosphere-276266">SpaceX rocket left behind a plume of chemical pollution as it ...</a></li>
<li><a href="https://gizmodo.com/study-confirms-reentering-spacex-rockets-are-peppering-the-upper-atmosphere-with-metal-pollution-2000723932">Study Confirms: Reentering SpaceX Rockets Are Peppering the Upper ...</a></li>

</ul>
</details>

**标签**: `#space pollution`, `#SpaceX`, `#atmospheric science`, `#rocket reentry`, `#environmental impact`

---

<a id="item-12"></a>
## [中国计划构建天地一体化小行星防御系统](http://paper.people.com.cn/rmrb/pc/content/202607/06/content_30166956.html) ⭐️ 7.0/10

中国正在正式论证构建小行星防御系统，该系统将整合地面大口径望远镜和天基星座实现昼夜连续监测，并正在开发动能撞击和引力牵引等偏转技术。 这一宣布标志着全球行星防御迈出重要一步，中国加入美国和欧洲的行列，开发主动防御能力。它解决了探测中型近地天体（140 米级）的关键缺口，目前仅发现了约 45%。 该系统将结合动能撞击等瞬时处置技术和引力牵引、离子束推离、激光烧蚀等持续作用技术。中国已初步突破撞击风险预警模型，正在开发业务化预警系统。

telegram · zaihuapd · Jul 6, 13:36

**背景**: 近地天体（NEO）是指轨道接近地球的小行星和彗星。虽然直径 1 公里以上的大型小行星大部分已被编录，但 140 米级的中型小行星更难探测，可能造成区域性灾难。行星防御包括探测、跟踪和偏转潜在危险天体。美国有 NASA 的 DART 任务（2022 年成功演示动能撞击），欧洲有后续的 Hera 任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.youth.cn/gn/202606/t20260630_16739416.htm">news.youth.cn/gn/202606/t20260630_16739416.htm</a></li>
<li><a href="https://www.chinanews.com/gn/2026/07-06/10653371.shtml">天外来客 防 范有策 我国正在论证 小 行 星 防 御 系统-中新网</a></li>

</ul>
</details>

**标签**: `#asteroid defense`, `#space technology`, `#planetary defense`, `#China space program`, `#near-Earth objects`

---

<a id="item-13"></a>
## [Claude Cowork 沙箱逃逸漏洞披露](https://cyberpress.org/claude-cowork-flaw/) ⭐️ 7.0/10

一名安全研究人员在 Anthropic 的 Claude Desktop for Windows 中发现了一条沙箱逃逸链，利用 Claude Cowork 功能中的 DLL sideloading 和未过滤参数，在 Ubuntu VM 中获取 root 权限并窃取 /etc/shadow 文件。Anthropic 将该报告归类为“不构成安全问题”，因为利用前提是主机上已执行恶意代码。 该漏洞凸显了 AI 编码工具中沙箱隔离的风险，成功逃逸可能使攻击者访问敏感主机数据。披露事件也引发了对 Anthropic 安全响应的质疑，因为他们驳回了一条记录详尽的利用链。 攻击链利用 claude.exe 的 DLL sideloading 以及 spawn 接口中两个未过滤参数（isResume 和 allowedDomains），结合 nsenter 跳出 bubblewrap 沙箱。该漏洞于 2026 年 3 月报告，在 Cyber Press 上评分为 7.0/10。

telegram · zaihuapd · Jul 6, 14:53

**背景**: DLL sideloading 是一种攻击技术，攻击者将恶意 DLL 放置在合法应用程序加载的目录中，利用 Windows 的搜索顺序执行代码。Bubblewrap 是一种轻量级沙箱工具，被 Flatpak 和其他容器系统用于隔离应用程序。nsenter 是一个 Linux 命令，允许进入另一个进程的命名空间，常被用于逃逸容器。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techzone.bitdefender.com/en/tech-explainers/what-is-dll-sideloading.html">What is DLL Sideloading – Bitdefender TechZone</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged ...</a></li>
<li><a href="https://man7.org/linux/man-pages/man1/nsenter.1.html">nsenter(1) - Linux manual page</a></li>

</ul>
</details>

**标签**: `#security`, `#vulnerability`, `#sandbox escape`, `#Anthropic`, `#Claude`

---