---
layout: default
title: "Horizon Summary: 2026-06-20 (ZH)"
date: 2026-06-20
lang: zh
---

> From 31 items, 18 important content pieces were selected

---

1. [历经十年，Project Valhalla 终在 JDK 28 落地](#item-1) ⭐️ 9.0/10
2. [ATProto 没有实例：一个澄清](#item-2) ⭐️ 8.0/10
3. [挪威禁止小学生使用人工智能](#item-3) ⭐️ 8.0/10
4. [中国拟出台分布式数字身份互通互认规定](#item-4) ⭐️ 8.0/10
5. [智谱创始人称模型或于明年一季度达 Mythos 级别](#item-5) ⭐️ 8.0/10
6. [美国施压 ASML，称 EUV 光刻机或流入中国](#item-6) ⭐️ 8.0/10
7. [多款婴儿纸尿裤检出生殖毒性物质甲酰胺](#item-7) ⭐️ 8.0/10
8. [中欧就电动汽车进口争端达成解决方案，欧盟发布价格指导](#item-8) ⭐️ 8.0/10
9. [苹果同意在巴西开放第三方应用商店](#item-9) ⭐️ 8.0/10
10. [SpaceX 上市前向中国投资者出售股份](#item-10) ⭐️ 8.0/10
11. [北航退学博士指控两名教授论文造假](#item-11) ⭐️ 8.0/10
12. [现代汽车从软银完全收购波士顿动力](#item-12) ⭐️ 7.0/10
13. [Google Workspace 可屏蔽 Firefox，但由管理员决定](#item-13) ⭐️ 7.0/10
14. [EFF 主张法院记录应免费](#item-14) ⭐️ 7.0/10
15. [Datasette Apps：在 Datasette 内托管沙盒 HTML 应用](#item-15) ⭐️ 7.0/10
16. [Google 推出侧载未验证应用需等待 24 小时的新流程](#item-16) ⭐️ 7.0/10
17. [印度为防作弊封锁 Telegram，VPN 注册量激增 150%](#item-17) ⭐️ 7.0/10
18. [英国总检察长要求部门停用 X](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [历经十年，Project Valhalla 终在 JDK 28 落地](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 9.0/10

Project Valhalla 的值类型终于随 JDK 28 到来，它允许对象内联存储，无需堆头或指针，从根本上改变了 Java 处理内存和性能的方式。 这是 Java 的一次重大范式转变，使开发者能够编写更高效的代码，改善内存局部性并减少垃圾回收压力，让 Java 的性能更接近 C 或 Rust 等语言。 值类型使用与对象引用相同的 'L' 描述符，但在数组和字段中内联存储，并可能带有一个空值标志。不过，堆扁平化仅适用于表示大小不超过 64 位的对象。

hackernews · philonoist · Jun 19, 06:35 · [社区讨论](https://news.ycombinator.com/item?id=48595511)

**背景**: Project Valhalla 是一个长期的 OpenJDK 项目，旨在通过值对象增强 Java 对象模型，将面向对象的抽象与基本类型的性能结合起来。传统上，所有 Java 对象都是引用类型，需要堆分配和指针间接访问，这增加了开销。值类型通过直接在内存布局中存储数据来消除这种开销。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openjdk.org/projects/valhalla/">Project Valhalla - OpenJDK</a></li>
<li><a href="https://www.jvm-weekly.com/p/project-valhalla-explained-how-a">Project Valhalla, Explained: How a Decade of... - JVM Weekly vol. 180</a></li>
<li><a href="https://dev.to/adaumircosta/understanding-value-types-project-valhalla-faf">Understanding Value Types (Project Valhalla) - DEV Community</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反应不一：有人赞赏这项艰苦工作，但批评其复杂性和错失的空安全机会；也有人为 Java 的演进辩护，指出许多批评者对 JVM 的看法已经过时。此外，关于大对象堆扁平化的技术限制也存在争议。

**标签**: `#Java`, `#JVM`, `#Project Valhalla`, `#value types`, `#performance`

---

<a id="item-2"></a>
## [ATProto 没有实例：一个澄清](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 8.0/10

Dan Abramov 发表了一篇博客文章，解释 ATProto（Bluesky 背后的协议）没有像 Mastodon 那样的“实例”，而是将功能分离为个人数据服务器（PDS）、中继（Relay）和应用视图（AppView）以实现可扩展性。 这一澄清解决了去中心化社交媒体社区中的一个常见误解，突出了 ATProto 与基于 ActivityPub 的系统（如 Mastodon）在架构上的差异。它帮助开发者和用户理解中心化与去中心化设计之间的权衡。 在 ATProto 中，PDS 托管用户数据，中继将多个 PDS 的数据聚合为数据流，AppView 则消费该数据流以构建特定应用的视图（例如 Bluesky 的社交信息流）。这种分离使得每个组件可以独立扩展。

hackernews · danabramov · Jun 19, 15:10 · [社区讨论](https://news.ycombinator.com/item?id=48599515)

**背景**: Mastodon 和其他使用 ActivityPub 的平台被组织成“实例”——每个实例托管用户账户、内容和审核。用户加入一个实例，实例之间相互通信。相比之下，ATProto 将数据存储（PDS）、数据聚合（中继）和数据展示（AppView）解耦，旨在实现更大的灵活性和可扩展性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://atproto.wiki/en/wiki/reference/core-architecture/appview">AppViews | AT Protocol Community Wiki</a></li>
<li><a href="https://getskyscraper.com/blog/atprotocol-federation-architecture-guide">ATProtocol Federation Architecture: PDS, Relay, AppView & How ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论者就与 RSS 和 Google Reader 的类比进行了辩论，一些人认为 RSS 对中心化服务的依赖程度低于 ATProto 的中继。其他人指出，虽然协议是去中心化的，但 Bluesky 公司仍然运行着大部分基础设施，导致实际上的中心化。

**标签**: `#ATProto`, `#Bluesky`, `#decentralization`, `#protocol design`, `#ActivityPub`

---

<a id="item-3"></a>
## [挪威禁止小学生使用人工智能](https://www.reuters.com/technology/norway-imposes-near-ban-ai-elementary-school-2026-06-19/) ⭐️ 8.0/10

挪威政府宣布，从 2026-2027 学年起，基本禁止 6 至 13 岁学生使用人工智能，14 至 16 岁学生可在教师监督下谨慎使用。 这是首批明确限制生成式 AI 在基础教育中使用的国家政策之一，为各国政府如何在技术应用与基础学习技能之间取得平衡树立了先例。 该禁令适用于所有 AI 工具，包括 ChatGPT 等生成式 AI，小学生完全禁止使用；高年级学生可在教师指导下谨慎使用。政策旨在保护儿童读写和批判性思维能力的发展。

hackernews · ilreb · Jun 19, 16:03 · [社区讨论](https://news.ycombinator.com/item?id=48600093)

**背景**: ChatGPT 等生成式 AI 工具能生成类似人类的文本、图像和代码，引发了对学术诚信和基础技能削弱的担忧。许多教育工作者担心过度依赖 AI 可能阻碍学生独立学习核心科目的能力。

**社区讨论**: 评论者普遍支持该禁令，将其类比为在学生学会算术前不提供计算器。一些人指出了 AI 在教育中制造“回音室”的更大问题，即教师和学生都依赖 AI 完成作业和评分。

**标签**: `#AI policy`, `#education`, `#Norway`, `#generative AI`, `#regulation`

---

<a id="item-4"></a>
## [中国拟出台分布式数字身份互通互认规定](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

2026 年 6 月 18 日，国家网信办发布《促进分布式数字身份互通互认应用规定（征求意见稿）》向社会公开征求意见，截止日期为 7 月 18 日。该规定明确分布式数字身份基于区块链技术，通过标识符、密钥、可验证凭证和可验证声明实现用户自主管理身份信息。 该征求意见稿标志着中国在基于区块链的身份系统方面的重要政策方向，有望实现金融、交通、海关、税务和数字人民币等领域的跨平台身份互通互认。若正式实施，将加速分布式身份在公共和私营部门的采用，影响个人和机构管理数字身份的方式。 规定提出建立分布式数字身份公共服务体系，依托国家区块链网络建设“身份链”。境内外个人、机构和工业设备均可自愿申请注册，相关机构需履行数据安全和个人信息保护义务。

telegram · zaihuapd · Jun 19, 01:39

**背景**: 分布式数字身份（DID）是一种基于区块链的身份模型，允许用户拥有和控制自己的身份数据，无需依赖中心化机构。它通常包括去中心化标识符（DID）、公私钥对、可验证凭证（如数字证书）和可验证声明（关于实体的陈述）。该概念符合 W3C 标准，被视为 Web3 和元宇宙应用的关键基础。中国一直在探索基于区块链的身份解决方案，如 eID 数字身份链，以提升安全性和互操作性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/article/2488015">基于区块链的数字身份认证：重塑身份安全的新范式-腾讯云开发者社区-腾讯云</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/425859804">区块链数字身份：数字经济时代基础设施 ——火链科技研究院产业应用系列报告之五 - 知乎</a></li>

</ul>
</details>

**标签**: `#decentralized identity`, `#blockchain`, `#regulation`, `#China`, `#digital identity`

---

<a id="item-5"></a>
## [智谱创始人称模型或于明年一季度达 Mythos 级别](https://x.com/jietang/status/2067580270078030088) ⭐️ 8.0/10

智谱 AI 创始人唐杰表示，其模型可能在明年第一季度达到“Mythos 级别”，回应了用户关于中国 AI 模型落后美国约 7 个月的评估。埃隆·马斯克也在同一讨论下评论“Probably Q1”。 这一讨论凸显了中美 AI 能力差距正在缩小，对全球 AI 领导地位和竞争格局具有重要影响。达到高级 AI 水平的时间线直接影响行业投资和政策决策。 该用户估计智谱 GLM-5.2 模型大致相当于 Claude Opus 4.7-4.8 水平，并预测中国模型将在 2026 年 11 月至 12 月达到 Anthropic 的 Mythos（Fable）级别。唐杰回应“won't take that long”，暗示进展更快。

telegram · zaihuapd · Jun 19, 02:24

**背景**: Mythos 级别是 Anthropic 用来描述其最先进 AI 模型的术语，如 Claude Fable 5，代表了超越前代的新能力层级。GLM-5.2 是智谱最新的开源模型，拥有 7440 亿参数和 100 万 token 上下文窗口，在某些基准测试中仅次于 Claude Opus 4.8。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ia.acs.org.au/article/2026/anthropic-releases--mythos-level--chatbot-to-public.html">Anthropic releases ‘ Mythos - level ’ chatbot to public | Information Age</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/zhipus-glm-5-2-is-the-new-top-open-model">Data Points: Zhipu’s GLM-5.2 is the new top open model</a></li>
<li><a href="https://benchlm.ai/compare/claude-opus-4-7-adaptive-vs-claude-opus-4-8">Claude Opus 4.7 (Adaptive) vs Claude Opus 4.8: AI Benchmark ...</a></li>

</ul>
</details>

**社区讨论**: 讨论反映了对中美 AI 差距的积极辩论，马斯克的“Probably Q1”被解读为 2027 年第一季度，而唐杰的回应暗示更早的时间线。社区对于中国模型能否比预期更快缩小差距存在分歧。

**标签**: `#AI`, `#LLM`, `#China AI`, `#Zhipu`, `#model comparison`

---

<a id="item-6"></a>
## [美国施压 ASML，称 EUV 光刻机或流入中国](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 8.0/10

美国商务部长卢特尼克向 ASML 高管表示，一台顶级 EUV 光刻机可能已非法流入中国，违反美国主导的出口管制。ASML 坚决否认，称从未向中国出口过完整的 EUV 系统。 此事件加剧了美中科技紧张局势，可能导致更严格的半导体设备出口管制。同时，它也影响了美欧关系，因为 ASML 是荷兰公司，并可能影响美国国会正在推动的对华芯片制造限制法案。 ASML 声称全球运行的 314 台 EUV 光刻机均不在中国。美方官员声称掌握 ASML 向中国出口 EUV 相关运输设备的证据，但未出示。

telegram · zaihuapd · Jun 19, 03:09

**背景**: EUV（极紫外）光刻是最先进的芯片制造技术，用于生产 7 纳米以下的芯片。ASML 是全球唯一的 EUV 光刻机供应商，这些设备受到严格的出口管制，以防止中国获得先进的半导体制造能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/极紫外光刻">极紫外光刻 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.eet-china.com/mp/a299998.html">【科普】芯片制造工艺：光刻 (下)--euv极紫外光刻-电子工程专辑</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1948833673634887034">极紫外光刻机(EUV)中国"卡脖子"深度解析：核心技术壁垒与突围路径</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#export controls`, `#EUV lithography`, `#US-China tech war`, `#ASML`

---

<a id="item-7"></a>
## [多款婴儿纸尿裤检出生殖毒性物质甲酰胺](https://t.me/zaihuapd/42051) ⭐️ 8.0/10

《经济参考报》委托专业机构检测发现，好奇、碧芭宝贝、Babycare 等品牌婴幼儿纸尿裤中检出生殖毒性物质甲酰胺，部分婴幼儿血液和尿液中也检出该物质。 这暴露了中国纸尿裤国家标准中未对甲酰胺设限的监管空白，该物质可通过皮肤吸收并在体内蓄积，对婴幼儿造成长期健康风险。 甲酰胺被列为生殖毒性物质，在中国化妆品目录中已禁用，但纸尿裤国标未设限。一名记者穿戴一款纸尿裤一夜后，血液中甲酰胺浓度飙升近一倍。

telegram · zaihuapd · Jun 19, 06:05

**背景**: 甲酰胺是一种用于某些工业过程的化学物质，可能从纸尿裤材料中释放。动物研究表明，它具有生殖和发育毒性，可导致胎儿畸形和生育力下降。欧盟将其列为 1B 类生殖毒性物质。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.sohu.com/a/1038359743_539932">“好奇”、“碧芭宝贝”、“Babycare”多款知名婴儿纸尿裤检测出甲酰胺生殖...</a></li>
<li><a href="https://k.sina.cn/article_7880068208_1d5b04c7006801ef46.html">为何国标对纸尿裤甲酰胺含量没有规定？|Baby|检测|标准|毒性|监管_新...</a></li>
<li><a href="https://www.sohu.com/a/1038369618_100117963">曝多款婴儿纸尿裤含有毒物质，Babycare等紧急回应_检测_国家标准_相关</a></li>

</ul>
</details>

**标签**: `#public health`, `#consumer safety`, `#regulatory gap`, `#toxicology`, `#infant products`

---

<a id="item-8"></a>
## [中欧就电动汽车进口争端达成解决方案，欧盟发布价格指导](https://t.me/zaihuapd/42056) ⭐️ 8.0/10

2025 年 1 月 12 日，中国和欧盟宣布就欧盟进口中国制造电动汽车的争端达成解决方案，欧盟发布指导文件，包括最低进口价格（MIP）机制，以替代此前高达 35.3%的关税。 该协议缓和了中欧之间重大的贸易冲突，可能稳定欧洲电动汽车市场，并为中国汽车制造商在欧洲的出口和投资提供可预测的框架。 最低进口价格机制为中国电动汽车进口设定了价格底线，欧盟在设定具体价格时将考虑中国汽车制造商在欧洲的投资计划。该协议取代了 2024 年实施的反补贴关税。

telegram · zaihuapd · Jun 19, 08:57

**背景**: 2024 年，欧盟以不公平补贴为由，对中国电动汽车征收高达 35.3%的反补贴关税，导致贸易紧张。新的最低进口价格机制允许中国汽车制造商通过承诺最低出口价格来避免这些关税，旨在抵消补贴优势，同时鼓励在欧洲本地投资。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260113A01LYD00">中欧电动汽车关税达成"价格承诺"框架，2026年销量会如何？</a></li>
<li><a href="https://www.sohu.com/a/883920608_121124378">取代欧盟对华汽车关税的"最低进口价格机制"妙在哪？</a></li>
<li><a href="https://wallstreetcn.com/articles/3763155">中欧电动汽车关税达成"价格承诺"框架，2026年销量会如何？</a></li>

</ul>
</details>

**标签**: `#trade policy`, `#electric vehicles`, `#China-EU relations`, `#automotive industry`

---

<a id="item-9"></a>
## [苹果同意在巴西开放第三方应用商店](https://t.me/zaihuapd/42059) ⭐️ 8.0/10

苹果与巴西反垄断监管机构达成和解，同意允许巴西的 iPhone 用户在 App Store 之外购买应用和服务，并支持第三方应用商店。该协议终止了持续三年的针对苹果反竞争行为的调查。 这标志着开放应用分发在监管层面取得重大胜利，可能影响其他司法管辖区的反垄断行动。巴西的开发者将在支付处理和分发方面获得更多自由，而苹果仍保留部分费用收取权。 苹果需在 105 天内落实相关改变，协议有效期为三年。开发者可展示外部支付方式和替代购买链接，苹果的支付系统将与 App Store 解耦，但苹果仍可对相关交易收取费用。

telegram · zaihuapd · Jun 19, 11:15

**背景**: 苹果的 App Store 因其强制使用苹果内购系统及 30%佣金而面临全球反垄断审查。此前苹果已在欧盟和日本做出类似让步，反映出监管压力迫使苹果开放其生态系统的趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://m.163.com/dy/article/KHIARRBT0514R9OJ.html">m.163.com/dy/article/KHIARRBT0514R9OJ.html</a></li>
<li><a href="https://finance.sina.com.cn/tech/discovery/2025-12-24/doc-inhcwtcp4520356.shtml">苹果与巴西反垄断机构和解 将开放第三方应用商店|巴西|反垄断|第三方应用_新浪科技_新浪网</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2025-12-24/doc-inhcwxmf5844889.shtml">苹果巴西反垄断调查终结：同意开放外部支付与第三方应用商店|反垄断|苹果|巴西_新浪科技_新浪网</a></li>

</ul>
</details>

**标签**: `#Apple`, `#antitrust`, `#App Store`, `#Brazil`, `#regulation`

---

<a id="item-10"></a>
## [SpaceX 上市前向中国投资者出售股份](https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china) ⭐️ 8.0/10

ProPublica 获得的法院解密文件显示，SpaceX 在 2018 年至 2021 年间向至少十几名地址位于中国大陆、香港或俄罗斯的投资者出售股份，尽管后来在 IPO 中禁止了此类投资者。 这引发了严重的国家安全和监管合规担忧，因为 SpaceX 是美国军方的主要国防承包商，来自受限国家的外资持股可能违反出口管制法律。 中间商 Tomales Bay Capital 促成了这些交易，并向投资者承诺提供季度更新、参观设施和接触首席财务官的机会。其中一名投资者与中国军工承包商有联系。

telegram · zaihuapd · Jun 19, 12:00

**背景**: SpaceX 是一家私营航天公司，为美国国家安全任务提供发射服务。其 2026 年的 IPO 因监管风险排除了中国和香港投资者。该公司估值从 2019 年的 333 亿美元飙升至 2.7 万亿美元。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china">Before SpaceX IPO, Investors in China Secretly Acquired Stakes — ProPublica</a></li>
<li><a href="https://www.warren.senate.gov/newsroom/press-releases/warren-kim-warn-that-undisclosed-investments-in-spacex-by-chinese-interests-may-threaten-national-security-raise-questions-about-compliance-with-national-security-law">Warren, Kim Warn That Undisclosed Investments in SpaceX by Chinese Interests May Threaten National Security, Raise Questions about Compliance with National Security Law | U.S. Senator Elizabeth Warren of Massachusetts</a></li>

</ul>
</details>

**标签**: `#SpaceX`, `#national security`, `#foreign investment`, `#regulatory compliance`, `#investigative journalism`

---

<a id="item-11"></a>
## [北航退学博士指控两名教授论文造假](https://www.zaobao.com.sg/news/china/story20260619-9231002) ⭐️ 8.0/10

北航退学博士生耿江涛公开指控常凌乾和王军两名教授在《自然》等期刊论文中数据造假，大量网民涌入北航官网查询，导致网站一度瘫痪。 这一事件凸显了中国顶尖高校科研诚信问题的日益关注，以及个人举报者引发机构审查的力量，可能导致论文撤稿和政策调整。 耿江涛运营科普账号“耿同学讲故事”，此前已举报其他四所高校的五名学者，均被处理。被指控的教授包括北航医工学院副院长常凌乾和航空科学与工程学院教授王军。

telegram · zaihuapd · Jun 19, 16:02

**背景**: 耿江涛曾是北航博士生，2025 年退学后成为科普博主。自 2026 年 4 月起，他通过数据分析公开质疑已发表研究的真实性。最新指控针对两名北航教授，其中常凌乾在《自然》上关于柔性可植入电子贴片的论文被指实验数据“完美到诡异”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ygy.buaa.edu.cn/info/1087/4350.htm">常凌乾-北航医学科学与工程学院</a></li>
<li><a href="https://news.buaa.edu.cn/info/1005/65745.htm">《Nature》报道北航常凌乾教授团队与合作者破解给药难题：一种柔性可...</a></li>
<li><a href="https://www.sinchew.com.my/news/20260601/international/7552269">耿同学停学术打假 社媒遭限流 学者：平台或担心愈演愈烈</a></li>

</ul>
</details>

**标签**: `#academic integrity`, `#research misconduct`, `#China`, `#university`, `#data fabrication`

---

<a id="item-12"></a>
## [现代汽车从软银完全收购波士顿动力](https://startupfortune.com/hyundai-takes-full-control-of-boston-dynamics-as-softbank-exits-for-325-million/) ⭐️ 7.0/10

现代汽车集团行使看跌期权，以 3.25 亿美元收购软银持有的波士顿动力剩余 9%股份，从而完全控制这家机器人公司。 此次收购使现代汽车能够将 Atlas 等先进人形机器人商业化，应对韩国劳动力短缺问题，并与特斯拉在通用机器人领域竞争。 该交易对波士顿动力的估值约为 36 亿美元；现代汽车此前在 2020 年 12 月以 8.8 亿美元收购了 80%股份，当时公司估值为 11 亿美元。

hackernews · ck2 · Jun 19, 16:28 · [社区讨论](https://news.ycombinator.com/item?id=48600312)

**背景**: 波士顿动力以 Spot、Atlas 和 Handle 等高机动性机器人闻名。现代汽车计划将 Atlas 整合到其工厂中，并开发用于物流和未来工作的 AI 驱动机器人，这与它在 CES 2026 上公布的物理 AI 战略一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boston_Dynamics">Boston Dynamics - Wikipedia</a></li>
<li><a href="https://bostondynamics.com/">The World's Leading Robotics Company | Boston Dynamics</a></li>
<li><a href="https://www.theaibulletin.com/post/hyundai-s-ai-robotics-strategy-debuts-atlas-at-ces-2026">Hyundai 's AI Robotics Strategy Debuts Atlas at CES 2026</a></li>

</ul>
</details>

**社区讨论**: 评论者就人形机器人相对于专用机器的实用性展开辩论，有人质疑人形在制造中的效率。另一些人将此次收购与韩国劳动年龄人口下降联系起来，认为这是应对劳动力短缺的战略举措。

**标签**: `#robotics`, `#acquisition`, `#Hyundai`, `#Boston Dynamics`, `#humanoid robots`

---

<a id="item-13"></a>
## [Google Workspace 可屏蔽 Firefox，但由管理员决定](https://tales.fromprod.com/2026/169/google-workspace-threatening-to-block-firefox.html) ⭐️ 7.0/10

一篇博客文章揭露，Google Workspace 的 Context-Aware Access 产品可以屏蔽 Firefox 浏览器访问，但这是企业管理员配置，并非 Google 的全局政策。 这澄清了常见的误解——Google 并非针对 Firefox，而是突显了企业 IT 政策在浏览器限制中的作用，并引发了关于浏览器检测和 User-Agent 操纵的更广泛讨论。 Context-Aware Access 仅适用于 Google Workspace Enterprise 版本，而非博客作者使用的 Business Plus。该功能允许管理员根据设备属性（如浏览器类型）设置策略。

hackernews · birdculture · Jun 19, 16:30 · [社区讨论](https://news.ycombinator.com/item?id=48600345)

**背景**: Google Workspace 的 Context-Aware Access 允许管理员根据用户身份、设备安全状态、位置和 IP 地址创建细粒度的访问控制策略。这是一项面向企业环境的安全功能，而非面向消费者的限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://knowledge.workspace.google.com/admin/security/protect-your-business-with-context-aware-access">Protect your business with Context-Aware Access - Google</a></li>
<li><a href="https://knowledge.workspace.google.com/admin/security/create-context-aware-access-levels">Create Context-Aware access levels | Security & data ... - Google</a></li>
<li><a href="https://workspaceupdates.googleblog.com/2025/08/context-aware-access-openid-connect-apps.html">Google Workspace Updates: Context-Aware Access policies can ...</a></li>

</ul>
</details>

**社区讨论**: 社区迅速纠正了最初认为 Google 屏蔽 Firefox 的印象，指出这是管理员可配置的功能。博客作者确认自己是管理员，使用的是 Business Plus 版本（不含 Context-Aware Access），因此屏蔽可能由其他设置导致。一些评论者表达了对浏览器检测的广泛担忧，并希望消除 User-Agent 字符串。

**标签**: `#Google Workspace`, `#Firefox`, `#browser detection`, `#enterprise IT`, `#privacy`

---

<a id="item-14"></a>
## [EFF 主张法院记录应免费](https://www.eff.org/deeplinks/2026/06/court-records-should-be-free) ⭐️ 7.0/10

电子前哨基金会（EFF）发表文章，主张公众应免费获取法院记录，批评联邦法院记录系统 PACER 收取高额费用。 这很重要，因为 PACER 费用为获取法律信息设置了经济障碍，削弱了透明度和司法平等。这场辩论凸显了法院系统资金需求与公众知情权之间的紧张关系。 PACER 每页收费 0.10 美元，每份文件最高 3.00 美元，但频繁使用者可能产生高额费用。EFF 提到了 CourtListener 和 RECAP 等项目，这些项目通过众包方式提供免费访问 PACER 文档的途径。

hackernews · hn_acker · Jun 19, 17:34 · [社区讨论](https://news.ycombinator.com/item?id=48600946)

**背景**: PACER（公共访问法院电子记录）是联邦司法系统用于电子访问法院文档的系统。虽然该系统主要通过用户费用维持运营，但批评者认为这些费用限制了公众获取本应免费提供的法律材料。CourtListener 是 Free Law Project 的一个项目，提供免费的法律意见搜索引擎，并通过 RECAP 浏览器扩展程序存档用户共享的 PACER 文档。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/06/court-records-should-be-free">Court Records Should Be Free | Electronic Frontier Foundation</a></li>
<li><a href="https://pacer.uscourts.gov/pacer-pricing-how-fees-work">PACER Pricing: How fees work | PACER: Federal Court Records</a></li>
<li><a href="https://free.law/projects/courtlistener/">CourtListener Research and Awareness Website | Free Law Project | Making the legal ecosystem more equitable and competitive.</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了实际问题：有人提到州法院费用可能比 PACER 更高，例如爱达荷州每页收费 10 美元。另一位称赞 CourtListener 和 RECAP 填补了重要空白，并希望当免费访问实现时它们能变得过时。还有评论者认为，经济成本是政府限制公民权利获取的众多方式之一。

**标签**: `#legal tech`, `#open government`, `#PACER`, `#public records`, `#access to justice`

---

<a id="item-15"></a>
## [Datasette Apps：在 Datasette 内托管沙盒 HTML 应用](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

datasette-apps 插件允许用户在 Datasette 内托管自定义 HTML+JavaScript 应用，这些应用在沙盒化的 iframe 中运行，具有只读 SQL 访问权限和可选的配置写入查询。 该插件将 Datasette 从数据探索工具转变为完整的应用平台，使开发者无需单独托管即可构建交互式数据驱动应用。 应用通过 iframe sandbox 属性和 CSP 标头进行沙盒化，阻止外部 HTTP 请求，防止数据泄露。写入查询需要通过存储查询进行显式配置。

rss · Simon Willison · Jun 18, 23:58

**背景**: Datasette 是一个用于探索和发布数据的开源工具，提供 JSON API 用于自定义前端。此前，开发者需要单独托管 HTML/JS 应用；该插件将它们直接集成到 Datasette 实例中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette Apps</a></li>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-apps/">Datasette Apps: Host custom HTML applications inside Datasette</a></li>

</ul>
</details>

**标签**: `#datasette`, `#plugin`, `#sql`, `#web-applications`, `#sandbox`

---

<a id="item-16"></a>
## [Google 推出侧载未验证应用需等待 24 小时的新流程](https://t.me/zaihuapd/42054) ⭐️ 7.0/10

Google 公布了 Android 安装未验证开发者应用的“高级流程”，要求用户等待 24 小时并完成多步验证后才能安装。 这一更新大幅提高了侧载的门槛，旨在为数百万 Android 用户降低欺诈和恶意软件风险，同时影响在 Google Play 之外分发应用的开发者。 用户需先开启开发者模式、确认并非在他人诱导下操作、重启手机并重新验证身份，经过 24 小时冷静期后，再用指纹、面容识别或设备 PIN 确认才能继续安装；完成后可将权限设为 7 天或长期有效。

telegram · zaihuapd · Jun 19, 07:59

**背景**: 侧载是指从官方应用商店以外的来源安装应用，这可能会使用户接触到未经验证的软件。Google 一直在加强安全措施，包括 2025 年 8 月宣布的开发者验证要求，以打击恶意应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sideloading">Sideloading - Wikipedia</a></li>
<li><a href="https://developer.android.com/developer-verification">Android developer verification | Android Developers</a></li>
<li><a href="https://developer.android.com/studio/debug/dev-options">Configure on-device developer options | Android Studio ...</a></li>

</ul>
</details>

**标签**: `#Android`, `#security`, `#sideloading`, `#Google`, `#mobile`

---

<a id="item-17"></a>
## [印度为防作弊封锁 Telegram，VPN 注册量激增 150%](https://t.me/zaihuapd/42058) ⭐️ 7.0/10

印度政府为防止 NEET-UG 医学入学考试作弊，于 2024 年 6 月 16 日至 22 日临时封锁 Telegram，导致 Proton VPN 报告来自印度的注册量飙升 150%。 此事件凸显了政府审查与数字权利之间的紧张关系，以及使用 BGP 劫持进行封锁的意外后果，影响了印度以外的用户。 据报道，印度电信运营商通过 BGP 劫持强制执行封锁，意外导致阿联酋等其他国家用户也无法访问 Telegram。Telegram CEO 批评了这一举措。

telegram · zaihuapd · Jun 19, 10:30

**背景**: BGP 劫持是通过破坏路由表恶意重定向互联网流量的行为。NEET-UG 是印度的国家医学入学考试。Proton VPN 是一家瑞士 VPN 服务商，在封锁期间来自印度的每小时注册量增加了 150%。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BGP_hijacking">BGP hijacking - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proton_VPN">Proton VPN</a></li>
<li><a href="https://neet.nta.nic.in/">NATIONAL ELIGIBILITY CUM ENTRANCE TEST | NEET | India</a></li>

</ul>
</details>

**标签**: `#censorship`, `#VPN`, `#BGP hijacking`, `#India`, `#Telegram`

---

<a id="item-18"></a>
## [英国总检察长要求部门停用 X](https://www.theguardian.com/technology/2026/jun/18/uk-attorney-general-tells-staff-stop-using-x-disinformation-concerns) ⭐️ 7.0/10

英国总检察长理查德·赫默已要求其办公室停止在 X（原推特）上发帖，使其成为首个因虚假信息和仇恨言论担忧而弃用该平台的英国政府机构。 此举标志着英国政府社交媒体监管政策的潜在转变，这是首个因虚假信息担忧而离开 X 的政府机构，可能影响其他部门，并为公共部门与该平台的互动开创先例。 该决定是在 2026 年 6 月初南安普敦和贝尔法斯特发生暴力事件后做出的，赫默越发担心 X 被用来散播种族仇恨和分裂社区。英国政府已宣布禁止 16 岁以下青少年使用社交媒体，并计划修订《在线安全法》，要求平台在危机期间更快删除煽动性内容。

telegram · zaihuapd · Jun 19, 15:30

**背景**: 英格兰和威尔士总检察长是英国政府的首席法律顾问。《2023 年在线安全法》规定了在线平台的注意义务，要求其处理非法和有害内容，违者最高可被处以 1800 万英镑或年营业额 10%的罚款。自埃隆·马斯克收购以来，X 因成为虚假信息温床而受到广泛批评，包括欧盟的调查和多家主流媒体退出该平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Attorney_General_for_England_and_Wales">Attorney General for England and Wales - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Online_Safety_Act_2023">Online Safety Act 2023</a></li>
<li><a href="https://tech.co/news/x-worst-platform-disinformation">Here's Why X is The Worst Platform for Disinformation - Tech.co</a></li>

</ul>
</details>

**标签**: `#social media`, `#disinformation`, `#UK government`, `#X`, `#regulation`

---