---
layout: default
title: "Horizon Summary: 2026-06-05 (ZH)"
date: 2026-06-05
lang: zh
---

> From 30 items, 17 important content pieces were selected

---

1. [Cloudflare 收购 VoidZero，将 Vite 集成到 Workers 平台](#item-1) ⭐️ 9.0/10
2. [Anthropic 开源 AI 漏洞发现框架](#item-2) ⭐️ 8.0/10
3. [Meta 在智能眼镜上推出人脸识别功能](#item-3) ⭐️ 8.0/10
4. [高斯点溅射：一种新的 3D 渲染技术](#item-4) ⭐️ 8.0/10
5. [AI 爱好者与怀疑者：与时间和熵赛跑](#item-5) ⭐️ 8.0/10
6. [老虎国际 6 月 12 日起暂停中国境内账户新开仓](#item-6) ⭐️ 8.0/10
7. [DeepSeek 登顶美国企业软件热门榜，企业因成本转向中国 AI](#item-7) ⭐️ 8.0/10
8. [苹果新版 Siri 将采用谷歌和英伟达芯片处理云端 AI](#item-8) ⭐️ 8.0/10
9. [AI 智能体流量首次超过人类流量](#item-9) ⭐️ 8.0/10
10. [谷歌在员工嘲讽后删除“人在回路中”声明](#item-10) ⭐️ 7.0/10
11. [Uber 将 AI 编码工具使用上限设为每工具每月 1500 美元](#item-11) ⭐️ 7.0/10
12. [奥特曼：OpenAI 最高用户每月消耗约 1000 亿 token](#item-12) ⭐️ 7.0/10
13. [微信与手机厂商合作推出 A2A 助手能力](#item-13) ⭐️ 7.0/10
14. [荔枝龙眼杂交新品种“怀石”首次挂果](#item-14) ⭐️ 7.0/10
15. [美国两党 GUARD 法案瞄准中国机器人进口](#item-15) ⭐️ 7.0/10
16. [ChatGPT 记忆升级：自动学习偏好，保持更新](#item-16) ⭐️ 7.0/10
17. [美国科技业 5 月裁员创近两年新高，AI 成首要原因](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Cloudflare 收购 VoidZero，将 Vite 集成到 Workers 平台](https://www.cloudflare.com/press/press-releases/2026/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web/) ⭐️ 9.0/10

Cloudflare 于 2026 年 6 月 4 日宣布收购 VoidZero，该公司是 Vite、Vitest、Rolldown 和 Oxc 等工具的背后团队。这些工具将深度集成到 Cloudflare Workers 平台，实现从本地代码到全球网络的一键部署。 此次收购将广泛使用的前端工具链（Vite 周下载量超过 1.3 亿次）直接整合到主流云平台中，简化了从开发到部署的流程。这也标志着 Cloudflare 为抓住 AI 原生网页趋势的战略举措，因为 AI 编程代理越来越依赖 Vite。 VoidZero 团队将整体加入 Cloudflare，继续推进开源路线图。Cloudflare 承诺投入 100 万美元设立独立的 Vite 生态基金，支持社区贡献者，并承诺 Vite、Rolldown、Oxc、Vitest 等工具继续保持 MIT 开源许可与厂商中立。

telegram · zaihuapd · Jun 5, 00:39

**背景**: Vite 是新一代 JavaScript 构建工具，提供快速的开发服务器启动和热模块替换。它属于更广泛的工具链的一部分，包括 Vitest（测试）、Rolldown（打包器）和 Oxc（基于 Rust 的解析器/代码检查器）。Cloudflare Workers 是一个无服务器边缘计算平台，允许开发者全球运行代码。此次收购旨在将这些工具结合起来，提供从本地开发到边缘部署的无缝开发体验。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance ...</a></li>

</ul>
</details>

**社区讨论**: 社区情绪复杂：一些人对此收购感到不安，担心开源项目可能失去独立性，或者 Cloudflare 的用户体验问题会影响这些工具。另一些人则认为这是自然的商业举措，指出 Vite 在 AI 代理中的流行使其成为战略资产。少数评论者还将其与早期的 Astro 收购相提并论。

**标签**: `#Cloudflare`, `#Vite`, `#acquisition`, `#frontend`, `#open-source`

---

<a id="item-2"></a>
## [Anthropic 开源 AI 漏洞发现框架](https://github.com/anthropics/defending-code-reference-harness) ⭐️ 8.0/10

Anthropic 发布了一个用于 AI 驱动漏洞发现的开源框架，旨在帮助安全研究人员构建自定义工具以实现自动化代码分析。该框架基于其 Claude 模型，旨在降低在安全研究中使用 AI 的门槛。 此次发布使先进的 AI 漏洞发现工具得以普及，此前这些工具仅限大型组织使用，可能显著加速开源软件中安全漏洞的识别。这也表明 Anthropic 对开源安全工具的承诺，可能影响行业实践。 该框架以 'defending-code-reference-harness' 名称托管在 GitHub 上，并包含构建自定义工具的指南。根据仓库说明，使用 Opus 运行该框架的成本约为数百美元，使用 Mythos 则为数千美元，每个智能体每分钟消耗约 1 万个未缓存输入 token 和 2 千个输出 token。

hackernews · binyu · Jun 4, 20:11 · [社区讨论](https://news.ycombinator.com/item?id=48403980)

**背景**: Anthropic 一直使用其 Claude 模型（特别是 Mythos 预览版）来发现开源软件中的漏洞。2026 年 2 月，他们开始使用 Mythos 进行漏洞发现，截至 2026 年 5 月，已在 1000 多个项目中识别出超过 23,000 个问题，其中 6,200 多个为高危或严重漏洞。该框架是他们与安全社区共享工具的广泛努力的一部分。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anthropic.com/coordinated-vulnerability-disclosure">Coordinated vulnerability disclosure for Claude-discovered vulnerabilities \ Anthropic</a></li>
<li><a href="https://red.anthropic.com/2026/cvd/">Anthropic's coordinated vulnerability disclosure dashboard</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/05/26/anthropic-project-glasswing-update/">Anthropic: Claude Mythos identified 10,000+ software flaws - Help Net Security</a></li>

</ul>
</details>

**社区讨论**: 社区讨论反应不一：一些用户将该框架比作研究人员可以自行调整的“车间夹具”，而另一些用户则质疑其运行成本，估计为数百到数千美元。此外，还有人对仓库名称 'Anthropics' 与 'Anthropic' 的差异感到困惑，并提到可能存在影响 GitHub 链接的标记问题。

**标签**: `#AI`, `#security`, `#open-source`, `#vulnerability discovery`, `#Anthropic`

---

<a id="item-3"></a>
## [Meta 在智能眼镜上推出人脸识别功能](https://www.buchodi.com/meta-glasses-facial-recognition/) ⭐️ 8.0/10

Meta 已在其 Ray-Ban 智能眼镜中集成了人脸识别功能，据称名为“Name Tag”，使设备能够识别人物并显示其姓名。该功能目前正在测试中，并引发了重大的隐私和法律争议。 此举重新引发了关于公共场所普遍监控和生物特征数据收集的担忧，尤其是在智能眼镜日益普及的背景下。它还凸显了为面容失认症患者带来的无障碍便利与潜在隐私侵犯之间的紧张关系。 据报道，该功能使用离线照片数据库来识别朋友和熟人，但具体实现细节尚不清楚。法律风险包括可能违反伊利诺伊州的《生物特征信息隐私法》（BIPA），该法对生物特征数据的收集进行了规范。

hackernews · buchodi · Jun 4, 19:36 · [社区讨论](https://news.ycombinator.com/item?id=48403588)

**背景**: 人脸识别技术通过图像或视频识别或验证个人身份。Meta 的 Ray-Ban 智能眼镜是一种配备摄像头和 AI 功能的可穿戴设备，此前曾因未经同意录制他人等隐私问题受到批评。面容失认症（prosopagnosia）是一种影响面部识别的神经系统疾病，如果该技术能在保护隐私的前提下实施，可能对此类患者有益。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prosopagnosia">Prosopagnosia</a></li>
<li><a href="https://www.linkedin.com/posts/ho-mun-fei_meta-ai-privacy-activity-7433846422187237376-Ldb4">Meta 's Name Tag: Facial Recognition in Smart Glasses ... | LinkedIn</a></li>
<li><a href="https://www.bbc.com/news/articles/cj37z8357e5o">Smart glasses are 'an invasion of privacy ' - Meta 's are selling b...</a></li>

</ul>
</details>

**社区讨论**: 评论表达了不同的反应：一些人看到了对面容失认症患者的无障碍好处，而另一些人则强烈反对其隐私影响。用户还提到了 BIPA 下的法律风险以及 Meta 员工曾查看眼镜私密录音的过往事件。

**标签**: `#facial recognition`, `#privacy`, `#smart glasses`, `#Meta`, `#ethics`

---

<a id="item-4"></a>
## [高斯点溅射：一种新的 3D 渲染技术](https://momentsingraphics.de/Siggraph2026.html) ⭐️ 8.0/10

高斯点溅射引入了一种新颖的 3D 渲染方法，使用高斯溅射代替传统多边形，基于最近的 3D 高斯溅射技术实现实时辐射场渲染。 该技术能够从稀疏图像输入实现实时逼真渲染，可能通过提供一种新的复杂场景表示和渲染方式，改变 AAA 游戏开发和其他实时图形应用。 该方法优化了各向异性 3D 高斯，并使用快速的可见性感知渲染算法，实现了实时性能。社区评论将其与 1990 年代的旧点溅射技术以及网格溅射进行比较，指出高斯可能难以处理尖锐特征。

hackernews · ibobev · Jun 4, 10:48 · [社区讨论](https://news.ycombinator.com/item?id=48396792)

**背景**: 高斯溅射是一种体积渲染技术，最初于 1990 年代早期引入，用于直接渲染体积数据。2023 年的 3D 高斯溅射技术使其复兴，能够从少量图像样本中学习并实时渲染逼真场景。传统的 AAA 游戏渲染依赖于多边形网格以及 LOD 和遮挡剔除等技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/">3D Gaussian Splatting for Real-Time Radiance Field Rendering</a></li>
<li><a href="https://huggingface.co/blog/gaussian-splatting">Introduction to 3D Gaussian Splatting</a></li>

</ul>
</details>

**社区讨论**: 社区参与度很高，用户对 AAA 游戏采用表示兴趣，并询问点溅射的教程。一些人将其与 1994 年的游戏 Ecstatica 进行比较，并质疑其处理尖锐特征的能力不如网格溅射。

**标签**: `#computer graphics`, `#rendering`, `#3D splatting`, `#gaussian splatting`, `#real-time rendering`

---

<a id="item-5"></a>
## [AI 爱好者与怀疑者：与时间和熵赛跑](https://simonwillison.net/2026/Jun/4/ai-enthusiasts-ai-skeptics/#atom-everything) ⭐️ 8.0/10

Charity Majors 发表了一篇分析文章，指出 AI 爱好者急于采用 AI 以快速提升能力，而 AI 怀疑者则专注于维护代码质量、可靠性和机构信任，两者之间存在冲突压力。 这篇评论捕捉了软件工程中一个真实而微妙的辩论，影响着团队动态、产品质量和长期业务生存能力。它强调了需要组织设计来弥合这两种观点之间的差距。 Majors 认为两组人都没有错：爱好者看到了 AI 带来的真正能力飞跃，而怀疑者则警告可靠性下降和机构知识流失。她建议设计反馈循环来连接这两组人。

rss · Simon Willison · Jun 4, 23:55

**背景**: 这篇文章讨论了快速采用 AI 与维护软件工程最佳实践之间的紧张关系。AI 爱好者推动更快的迭代和利用 AI 工具，而怀疑者则强调代码审查、测试和文档，以防止技术债务和系统故障。

**标签**: `#AI`, `#software engineering`, `#code quality`, `#technology adoption`

---

<a id="item-6"></a>
## [老虎国际 6 月 12 日起暂停中国境内账户新开仓](https://t.me/zaihuapd/41762) ⭐️ 8.0/10

老虎国际宣布，自 2026 年 6 月 12 日起，暂停中国境内账户所有证券品种的新开仓和加仓交易，仅支持卖出和平仓操作。境内资金转入同步暂停，转出服务保持正常。 此举标志着中国对非法跨境证券服务的整治进入执行阶段，影响大量使用境外券商的内地投资者。它凸显了监管层遏制资本外流、确保境内证券法规合规的决心。 暂停适用于所有中国境内存量账户，但不影响境外服务或现有资产安全。投资者仍可持有、查询和卖出持仓，并正常转出资金。

telegram · zaihuapd · Jun 4, 07:51

**背景**: 2026 年 5 月，中国证监会等八部门联合发布通知，整治非法跨境证券、期货和基金活动，设置两年集中整治期。老虎国际、富途等境外券商被要求逐步停止向内地客户提供服务。此举是更广泛执法行动的一部分，旨在确保跨境证券服务仅由持牌机构提供。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.yicai.com/news/103212592.html">老虎国际：6月12日起，暂停存量投资者账户在中国境内所有品种的新开仓...</a></li>
<li><a href="https://www.csrc.gov.cn/csrc/c100028/c7634328/content.shtml">中国证监会有关部门负责人就《综合整治非法跨境证券期货基金经营活动...</a></li>
<li><a href="https://news.qq.com/rain/a/20260522A094J000">监管全面升级！跨境券商境内展业被全面取缔，协助展业者将被同步整顿_...</a></li>

</ul>
</details>

**标签**: `#fintech`, `#regulation`, `#cross-border securities`, `#China`

---

<a id="item-7"></a>
## [DeepSeek 登顶美国企业软件热门榜，企业因成本转向中国 AI](https://www.scmp.com/tech/tech-trends/article/3355927/more-us-firms-turn-chinas-deepseek-over-pricey-silicon-valley-ai) ⭐️ 8.0/10

DeepSeek 在 2026 年 6 月 Ramp 的“热门软件供应商”榜单中登顶，更多美国公司直接付费使用其 AI 服务，将数据发送至中国服务器处理。该公司还将 V4 Pro 模型的 75%降价永久化，并在首轮融资中估值接近 600 亿美元。 这标志着 AI 行业的重大转变，注重成本的美国企业越来越多地采用中国 AI 模型，而非更昂贵的硅谷替代品。DeepSeek 的崛起可能迫使美国 AI 提供商降价，并加速开源模型的采用。 DeepSeek 的 V4 Pro 是一个混合专家模型，总参数量达 1.6 万亿，激活参数量为 490 亿，支持 100 万 token 的上下文窗口。其永久定价为每百万输入 token 0.435 美元、每百万输出 token 0.87 美元，远低于许多竞争对手。

telegram · zaihuapd · Jun 4, 10:26

**背景**: DeepSeek 是一家中国 AI 公司，开发大型语言模型，以其高性价比的开源模型受到关注。Ramp 是一家美国企业支出管理平台，追踪其 5 万多家客户的软件供应商采用情况。这一趋势反映了企业 AI 采用中日益增长的价格敏感性，像 DeepSeek 这样的开源模型正在挑战美国科技巨头的专有产品。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://apidog.com/blog/deepseek-v4-pro-permanent-price-cut/">DeepSeek V4-Pro 75% Price Cut Is Now Permanent: What It Means ...</a></li>

</ul>
</details>

**标签**: `#AI`, `#DeepSeek`, `#enterprise software`, `#cost optimization`, `#China tech`

---

<a id="item-8"></a>
## [苹果新版 Siri 将采用谷歌和英伟达芯片处理云端 AI](https://www.macrumors.com/2026/06/04/apple-siri-rely-on-google-nvidia-chips/) ⭐️ 8.0/10

苹果计划于 2026 年 9 月推出的新版 Siri，将把云端 AI 查询交给谷歌数据中心处理，该数据中心采用英伟达 Blackwell B200 芯片，并通过英伟达硬件加密保护用户数据。这标志着苹果打破了自研核心硬件的传统。 这一战略转变表明苹果承认自研芯片不足以处理大规模云端 AI，可能重塑其与竞争对手谷歌和英伟达的关系。同时也凸显了云端 AI 处理在消费设备中日益增长的重要性。 据报道，此举是因为苹果自研服务器运行谷歌 Gemini 模型速度过慢。苹果将在下周的 WWDC 上重点强调设备端 AI 能力，新版 Siri 有望重新推出多次延迟的个性化功能。

telegram · zaihuapd · Jun 4, 11:37

**背景**: 苹果智能（Apple Intelligence）自 2024 年发布以来反响平平，苹果一直致力于将谷歌庞大的 Gemini 模型蒸馏到设备端运行。然而，在 iPhone 上完整运行 Gemini 仍具挑战，因此需要云端支持。英伟达 Blackwell B200 GPU 可提供高达 20 petaflops 的 FP4 算力，适合处理大型 AI 任务。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://arstechnica.com/ai/2026/05/apple-reportedly-trying-to-distill-googles-multi-trillion-parameter-gemini-ai-to-run-on-iphone/">Apple working to cram massive Gemini model into iPhone to power new Siri - Ars Technica</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Siri`, `#AI`, `#Nvidia`, `#Google`

---

<a id="item-9"></a>
## [AI 智能体流量首次超过人类流量](https://www.tomshardware.com/tech-industry/artificial-intelligence/bots-have-now-passed-human-traffic-online-cloudflare-boss-laments-says-agentic-traffic-wasnt-expected-to-eclipse-real-people-until-next-year) ⭐️ 8.0/10

Cloudflare 报告称，AI 智能体流量首次超过人类流量，占网页请求的 57.5%，比 CEO Matthew Prince 此前预测的 2027 年提前到来。 这一里程碑标志着互联网使用方式的根本转变，对网络基础设施、机器人检测和网络安全产生影响，因为 AI 智能体越来越多地执行比价、内容检索等任务。 Cloudflare 指出，虽然 AI 智能体产生更多页面请求，但人类在总使用时长上仍占主导，因为流媒体和社交应用每分钟产生的请求较少。该公司的 AI Crawl Control 工具可帮助网站管理机器人流量。

telegram · zaihuapd · Jun 4, 16:49

**背景**: AI 智能体是执行多步骤任务（如浏览、比价或回答客服问题）的自动化程序，模拟人类行为。Cloudflare 作为主要的内容分发网络，对全球网络流量具有广泛可见性，并使用其 AI Crawl Control 来检测和管理此类智能体。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cnet.com/tech/services-and-software/its-official-agentic-bots-surf-the-web-more-than-real-people-do/">AI Agents Now Generate More Web Traffic Than Humans</a></li>
<li><a href="https://www.cloudflare.com/ai-crawl-control/">AI Crawl Control | Cloudflare</a></li>
<li><a href="https://matomo.org/blog/2026/03/humans-agents-understanding-ai-web-traffic/">From humans to AI agents: understanding the new web traffic</a></li>

</ul>
</details>

**标签**: `#AI`, `#web traffic`, `#bots`, `#Cloudflare`, `#internet trends`

---

<a id="item-10"></a>
## [谷歌在员工嘲讽后删除“人在回路中”声明](https://simonwillison.net/2026/Jun/4/a-slightly-different-version/#atom-everything) ⭐️ 7.0/10

谷歌在员工内部分享嘲讽公司 AI 质量的梗图后，从其声明中删除了“保持人在回路中至关重要”的表述。 这一事件表明谷歌在 AI 中保持人类监督的承诺可能发生转变，引发了业界对透明度和伦理责任的担忧。 原始声明由 404 Media 发布，报道刊出后，谷歌发言人要求修改版本，不再包含人在回路中的承诺。

rss · Simon Willison · Jun 4, 16:38

**背景**: “人在回路中”方法是指在 AI 系统中引入人类监督，以确保准确性和伦理决策，尤其在医疗等高风险领域被视为最佳实践。谷歌删除这一承诺，暗示可能转向更自动化的 AI 部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48400311">Google employees internally share memes about how its AI sucks</a></li>

</ul>
</details>

**社区讨论**: Hacker News 评论者指出，这些梗图反映了内部对谷歌 AI 质量的不满，一些人认为取消人类监督是 AI 伦理方面令人担忧的趋势。

**标签**: `#ai-ethics`, `#google`, `#ai`, `#journalism`

---

<a id="item-11"></a>
## [Uber 将 AI 编码工具使用上限设为每工具每月 1500 美元](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 7.0/10

Uber 在短短四个月内用完了 2026 年全年 AI 预算后，对所有员工实施了每款 AI 编码工具每月 1500 美元的使用上限。该政策适用于 Cursor 和 Anthropic 的 Claude Code 等代理式编码工具。 这是大型公司对 AI 编码工具实施严格成本控制的首批具体案例之一，凸显了开发者生产力提升与快速增长的 token 成本之间的矛盾。这表明企业采用 AI 可能需要谨慎的预算规划和使用治理。 1500 美元的上限适用于每款工具，这意味着同时使用 Cursor 和 Claude Code 的工程师每月最多可花费 3000 美元。Uber 软件工程师的薪酬中位数为 33 万美元，AI 使用上限约占该数字的 11%。

rss · Simon Willison · Jun 3, 12:01

**背景**: 像 Claude Code 和 Cursor 这样的 AI 编码工具是“代理式”的——它们能理解整个代码库、编辑文件并自主运行命令。这些工具消耗 token（AI 计算单位），由 Anthropic 和 OpenAI 等提供商定价。此类工具的快速采用已导致许多公司出现意外的成本超支。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.zerohedge.com/ai/uber-introduces-1500-monthly-cap-ai-coding-tools-after-budget-blowout">Uber Introduces $1,500 Monthly Cap On AI Coding Tools ... | ZeroHedge</a></li>

</ul>
</details>

**标签**: `#AI`, `#cost management`, `#enterprise`, `#coding agents`, `#Uber`

---

<a id="item-12"></a>
## [奥特曼：OpenAI 最高用户每月消耗约 1000 亿 token](https://www.businessinsider.com/sam-altman-openai-top-token-spender-ai-costs-issue-2026-6) ⭐️ 7.0/10

Sam Altman 透露，OpenAI 内部最高用户每月消耗约 1000 亿个 token，而 6 年半前仅为 10 万个，且外部用户消耗更多。他还指出，AI 成本压力在 2026 年已成为重大问题。 这一数据凸显了 AI token 使用的爆炸性增长，既表明 AI 采用率上升，也表明 OpenAI 等提供商面临日益增长的成本压力。这强调了整个行业需要更高效的模型和成本管理策略。 Altman 提到，6 年半前每月 10 万个 token 可能已是全球领先水平，而现在大约只是全球人均水平。OpenAI 内部有鼓励高 token 使用的文化，但正积极寻找以更低成本提供更多价值的方法。

telegram · zaihuapd · Jun 4, 02:31

**背景**: Token 是 AI 模型处理文本的基本单位，可以是单词、子词或字符。更高的 token 消耗意味着更广泛地使用 AI 模型进行推理、生成和分析等任务。随着 AI 采用率增长，token 使用量激增，给提供商带来了巨大的基础设施和运营成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>
<li><a href="https://help.openai.com/en/articles/6614209-how-do-i-check-my-token-usage">How do I check my token usage? - OpenAI Help Center</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#AI costs`, `#token usage`, `#Sam Altman`, `#industry trends`

---

<a id="item-13"></a>
## [微信与手机厂商合作推出 A2A 助手能力](https://36kr.com/newsflashes/3838138218662404) ⭐️ 7.0/10

微信正与华为、荣耀、小米、OPPO、vivo 等手机厂商合作推出 A2A（Agent-to-Agent）助手能力，用户可通过手机语音助理发起微信音视频通话或发送消息。荣耀部分机型已支持该功能，通过 YOYO 智能体即可语音操作。 这标志着主流移动平台与头部即时通讯应用之间 AI 智能体互操作性的重要进展，可能为生态内的智能体间通信树立先例。该功能有望提升用户便利性，并推动语音控制交互的普及。 该 A2A 能力基于 Google 于 2025 年 4 月推出的开放 Agent2Agent 协议，该协议使不同框架构建的 AI 智能体能够相互通信。目前仅荣耀部分机型在更新 YOYO 智能体和微信后支持该功能，其他厂商预计将陆续跟进。

telegram · zaihuapd · Jun 4, 04:53

**背景**: Agent-to-Agent（A2A）是一种开放通信协议，允许来自不同平台的 AI 智能体协作完成任务。与专注于连接智能体与工具的 MCP 协议不同，A2A 实现智能体间的直接交互。微信与手机厂商语音助手的集成是该协议在真实消费场景中的典型应用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/a2aproject/A2A">GitHub - a2aproject/A2A: Agent2Agent (A2A) is an open protocol enabling ...</a></li>
<li><a href="https://www.ibm.com/think/topics/agent2agent-protocol">What is A2A protocol (Agent2Agent)? - IBM</a></li>
<li><a href="https://min.news/en/tech/6076456ce940abc960efc06e75ca8a57.html">Magic OS 9 YOYO Intelligent Body The more AI understands you, the...</a></li>

</ul>
</details>

**标签**: `#AI agents`, `#WeChat`, `#mobile assistants`, `#interoperability`, `#voice commands`

---

<a id="item-14"></a>
## [荔枝龙眼杂交新品种“怀石”首次挂果](https://news.ycwb.com/ikimvkmtkh/content_54155752.htm) ⭐️ 7.0/10

广东省农业科学院的科研人员成功培育出全球首个荔枝龙眼杂交新品种“怀石”，该品种于 2025 年 6 月首次挂果。该杂交种以荔枝为母本、龙眼为父本，突破了属间生殖隔离。 这一突破证明了荔枝与龙眼属间杂交的可行性，为水果育种开辟了新途径。该杂交种具有早熟和口感优良的特性，有望为种植者和消费者带来经济效益。 亲本为晚熟荔枝“怀枝”和龙眼“石硖”，但杂交种呈现早熟性状，果肉爽脆清甜、香气浓郁。目前处于品种比较试验阶段，预计五至六年后推向市场。

telegram · zaihuapd · Jun 4, 12:31

**背景**: 荔枝和龙眼是无患子科的近缘水果，但属于不同属，由于生殖隔离，自然杂交极为罕见。属间杂交需要克服遗传不相容和杂种不育等障碍。位于广州的国家荔枝种质资源圃保存了 700 多份荔枝种质资源，为这项研究提供了遗传资源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.ycwb.com/ikimvkmtkh/content_54155752.htm">今年首次挂果！荔枝龙眼杂交新品种“怀石”来了</a></li>
<li><a href="https://news.qq.com/rain/a/20260603A05W9400">全球首个！荔枝×龙眼杂交新品种“怀石”来了：是荔枝，却有龙眼味</a></li>
<li><a href="https://www.sohu.com/a/1032111060_99990677">令人振奋的消息：全球首个荔枝龙眼杂交品种“怀石”来了</a></li>

</ul>
</details>

**标签**: `#agriculture`, `#biotechnology`, `#hybrid`, `#fruit breeding`, `#China`

---

<a id="item-15"></a>
## [美国两党 GUARD 法案瞄准中国机器人进口](http://chinaselectcommittee.house.gov/media/press-releases/moolenaar-obernolte-mcclellan-introduce-legislation-to-ban-dangerous-chinese-robots) ⭐️ 7.0/10

美国议员提出 GUARD 法案，要求对来自中国等敌对国家的仿人机器人和四足机器人进行国家安全审查，并可能限制其进口。 该法案可能对宇树科技等中国机器人公司产生重大影响，该公司正准备 IPO，并可能重塑全球机器人贸易格局。 该法案要求国家安全机构在一年内完成审查；若未完成，FCC 将自动将这些机器人列入“覆盖名单”限制市场准入。批评者指出，与美国机器人公司如 Agility Robotics 存在潜在利益冲突。

telegram · zaihuapd · Jun 4, 13:16

**背景**: GUARD 法案（保护美国免受对抗性机器人主导法案）针对来自中国、俄罗斯等敌对国家的仿人机器人和四足机器人。该法案源于美国对中国技术主导地位和国家安全风险的日益担忧，尽管尚无公开证据支持后门或远程劫持的说法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techmarketbriefs.com/pre-ipo/unitree/">Unitree Stock & IPO 2026: Valuation, Risks & Bull Case | TMB</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agility_Robotics">Agility Robotics - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2025/09/09/chinas-unitree-plans-7-billion-ipo-valuation-as-humanoid-robot-race-heats-up.html">China’s Unitree heats up humanoid robot race as IPO ... - CNBC</a></li>

</ul>
</details>

**标签**: `#geopolitics`, `#robotics`, `#trade policy`, `#China`, `#regulation`

---

<a id="item-16"></a>
## [ChatGPT 记忆升级：自动学习偏好，保持更新](https://openai.com/index/chatgpt-memory-dreaming/) ⭐️ 7.0/10

OpenAI 已向美国 Plus 和 Pro 用户推出全新的 ChatGPT 记忆系统，该系统能从对话中自动学习用户偏好并随时间更新。 此次升级解决了此前手动、静态记忆的关键限制，使 ChatGPT 无需明确指令即可更加个性化和感知上下文，显著提升了用户体验。 该系统采用名为“dreaming”的技术，通过引用聊天历史在后台自动整理记忆，并能动态更新——例如旅行结束后不再推荐当地餐厅。

telegram · zaihuapd · Jun 4, 16:22

**背景**: ChatGPT 之前的记忆系统需要用户明确告诉模型记住某些内容，且这些记忆在手动更改前保持静态。新的“dreaming”架构允许模型自动引用过去的对话，补充了笔记式记忆系统。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/chatgpt-memory-dreaming/">Dreaming: Better memory for a more helpful ChatGPT - OpenAI</a></li>
<li><a href="https://www.makeuseof.com/chatgpt-now-remembers-your-preferences-automatically-and-it-actually-works/">ChatGPT now remembers your preferences automatically - MUO</a></li>
<li><a href="https://www.engadget.com/2187811/chatgpt-s-memory-is-getting-better-especially-if-you-re-on-the-free-tier/">ChatGPT's Memory Is Getting Better, Especially If You're On ...</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#ChatGPT`, `#memory`, `#AI`, `#product update`

---

<a id="item-17"></a>
## [美国科技业 5 月裁员创近两年新高，AI 成首要原因](https://www.tomshardware.com/tech-industry/artificial-intelligence/tech-sector-cut-us-jobs-by-38242-in-may) ⭐️ 7.0/10

美国科技业 5 月宣布裁员 38,242 人，创近两年单月新高，AI 连续第三个月成为企业解释裁员时最常提到的理由。 这凸显了行业重大转变：企业正将预算从传统岗位重新分配到 AI 基础设施，可能重塑科技就业市场，并引发对 AI 影响就业的担忧。 尽管裁员，失业金申请并未明显上升，科技巨头今年资本支出合计约 7,250 亿美元，其中约四分之三投向 AI 基础设施。

telegram · zaihuapd · Jun 5, 01:00

**背景**: 2026 年，随着 AI 投资激增，科技裁员持续上升。一些专家认为，企业可能在进行“AI 洗白”，将 AI 作为其他因素（如需求放缓或成本上升）的方便借口。与此同时，主要云和 AI 提供商正承诺投入数千亿美元用于 AI 基础设施，几乎是此前支出水平的两倍。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://futurumgroup.com/insights/ai-capex-2026-the-690b-infrastructure-sprint/">AI Capex 2026: The $690B Infrastructure Sprint - Futurum</a></li>
<li><a href="https://www.theguardian.com/technology/2026/apr/06/tech-layoffs-ai-work">Tech companies are cutting jobs and betting on AI . The... | The Guardian</a></li>

</ul>
</details>

**标签**: `#tech layoffs`, `#AI impact`, `#job market`, `#capital expenditure`

---