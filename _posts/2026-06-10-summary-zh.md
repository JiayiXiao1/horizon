---
layout: default
title: "Horizon Summary: 2026-06-10 (ZH)"
date: 2026-06-10
lang: zh
---

> From 33 items, 16 important content pieces were selected

---

1. [Anthropic 发布 Claude 3.5 Sonnet 并引入安全限制](#item-1) ⭐️ 9.0/10
2. [Let's Encrypt 禁止向美国制裁地区签发证书](#item-2) ⭐️ 9.0/10
3. [npm v12 重大变更：安全修复与默认设置调整](#item-3) ⭐️ 8.0/10
4. [重现 1990 年代的软件渲染器：射线投射](#item-4) ⭐️ 8.0/10
5. [FCC 提议要求身份验证以消灭一次性手机](#item-5) ⭐️ 8.0/10
6. [苹果因豁免请求被拒，不在欧盟推出 Siri](#item-6) ⭐️ 8.0/10
7. [苹果 AI 策略：隐私作为竞争优势](#item-7) ⭐️ 8.0/10
8. [小米 1T 参数模型推理速度达 1000 tokens/s](#item-8) ⭐️ 8.0/10
9. [中国拟投 2 万亿元建设全国算力网络，优先采用国产 AI 芯片](#item-9) ⭐️ 8.0/10
10. [AI 取代员工？那是糟糕的 CEO](#item-10) ⭐️ 7.0/10
11. [Karpathy：AI 软件需求因杰文斯悖论激增](#item-11) ⭐️ 7.0/10
12. [苹果 WWDC 2026：Siri AI 采用视觉大模型和 Gemini](#item-12) ⭐️ 7.0/10
13. [Z-Library 推出白标镜像，用户可自建品牌登录站](#item-13) ⭐️ 7.0/10
14. [阿里巴巴洽谈小型核反应堆为数据中心供电](#item-14) ⭐️ 7.0/10
15. [朱雀二号发射卫星，开展手机直连试验](#item-15) ⭐️ 7.0/10
16. [国家互联网应急中心警告 AI 智能体技能包存在越狱和挖矿风险](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic 发布 Claude 3.5 Sonnet 并引入安全限制](https://www.anthropic.com/news/claude-fable-5-mythos-5) ⭐️ 9.0/10

Anthropic 发布了 Claude 3.5 Sonnet（代号'Fable 5'），这是一款具有更强推理、编码和安全特性的新 AI 模型，其中包括限制该模型被用于加速竞争性 AI 开发的措施。 此次发布通过在模型层面实施限制以防止被滥用于开发竞争性 AI 系统，标志着 AI 安全的重要一步，同时提供了显著的性能提升，可能惠及开发者和企业。 该模型可通过 Claude Code、Claude.ai 和网页版使用，早期测试者报告称它能高效处理难题，有时仅用之前模型一半的 token 就能获得类似结果。

hackernews · Philpax · Jun 9, 16:58 · [社区讨论](https://news.ycombinator.com/item?id=48463808)

**背景**: Claude 是 Anthropic 开发的一系列大语言模型，采用'宪法 AI'技术训练以提升伦理合规性。Claude 3.5 Sonnet 是 Claude 3.5 系列中的中等规模模型，定位介于 Haiku 和 Opus 之间，最初于 2024 年 6 月发布。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_3.5_Sonnet">Claude 3.5 Sonnet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/claude-3-5-sonnet">Introducing Claude 3.5 Sonnet \ Anthropic</a></li>

</ul>
</details>

**社区讨论**: 社区成员报告称该模型在困难的编码和设计任务上表现令人印象深刻，一位用户指出它能'轻松攻克非常困难的问题'，这些问题已停滞数月。另一位测试者观察到前端设计质量提升和成本效率提高，但也有人担心安全限制可能限制合法使用。

**标签**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Safety`

---

<a id="item-2"></a>
## [Let's Encrypt 禁止向美国制裁地区签发证书](https://letsencrypt.org/documents/LE-SA-v1.7-June-04-2026-diff.pdf) ⭐️ 9.0/10

Let's Encrypt 更新了服务条款，自 2026 年 6 月 4 日起禁止向美国制裁地区的用户签发 SSL/TLS 证书。 这与 Let's Encrypt 为所有人创建更安全网络的使命相矛盾，并可能削弱伊朗、古巴、朝鲜等制裁地区用户的在线安全和隐私。 该禁令适用于位于美国制裁地区的任何域名或 IP 地址，违反条款可能导致用户持有的所有证书被吊销，即使是非制裁地区的域名也不例外。

hackernews · piskov · Jun 8, 22:32 · [社区讨论](https://news.ycombinator.com/item?id=48453275)

**背景**: Let's Encrypt 是一个非营利证书颁发机构，免费提供用于 TLS 加密的 X.509 证书，旨在让每个网站都能启用 HTTPS。美国出口管制法限制向受制裁国家分发加密技术，迫使 Let's Encrypt 尽管以全球公共利益为使命，仍必须遵守。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Let's_Encrypt">Let ' s Encrypt - Wikipedia</a></li>
<li><a href="https://www.lawfaremedia.org/article/how-geoblocking-limits-digital-access-in-sanctioned-states">How Geoblocking Limits Digital Access in Sanctioned States</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了沮丧，指出 Let's Encrypt 在最需要安全工具的地区限制安全工具具有讽刺意味。一些人建议该组织可以在美国以外设立分支机构以避免此类限制，而另一些人则认为这揭示了数字证书本质上是排他性工具。

**标签**: `#Let's Encrypt`, `#US sanctions`, `#internet censorship`, `#SSL/TLS`, `#digital rights`

---

<a id="item-3"></a>
## [npm v12 重大变更：安全修复与默认设置调整](https://github.blog/changelog/2026-06-09-upcoming-breaking-changes-for-npm-v12/) ⭐️ 8.0/10

npm v12 引入了重大变更，包括修复一个存在十年的漏洞（CERT VU#319816），并将 allowScripts 配置默认设为关闭，效仿了 pnpm 的做法。 此更新通过默认阻止恶意生命周期脚本运行，解决了长期存在的供应链风险，显著提升了 npm 生态系统的安全性。 当 allowScripts 设置为关闭时，将禁用所有包的生命周期脚本，除非通过 package.json 中的允许列表明确授权。修复的漏洞于 10 年前报告，涉及通过 npm 脚本执行任意代码。

hackernews · plasma · Jun 9, 21:01 · [社区讨论](https://news.ycombinator.com/item?id=48467705)

**背景**: npm 生命周期脚本（如 preinstall、postinstall）是在安装包时自动运行的命令。恶意行为者曾利用这些脚本执行任意代码，导致供应链攻击。pnpm 在 18 个月前引入了类似的 allowScripts 功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.npmjs.com/package/@lavamoat/allow-scripts">@lavamoat/allow-scripts - npm</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/NPM_Security_Cheat_Sheet.html">NPM Security - OWASP Cheat Sheet Series</a></li>

</ul>
</details>

**社区讨论**: 社区普遍欢迎这些安全改进，用户注意到十年漏洞的修复，并称赞 npm 效仿 pnpm 的做法。部分用户对允许列表的行为以及 GitHub 的“vibecoded”徽章设计提出了疑问。

**标签**: `#npm`, `#JavaScript`, `#security`, `#breaking changes`, `#package management`

---

<a id="item-4"></a>
## [重现 1990 年代的软件渲染器：射线投射](https://staniks.github.io/articles/catlantean-3d-blog-1/) ⭐️ 8.0/10

一篇详细文章从头构建了一个复古软件渲染器，包含射线投射、纹理地板和天花板以及血腥碎片，模仿了如《德军总部 3D》等早期 1990 年代游戏的风格。 这篇深度文章保存并教授了经典渲染技术，这些技术是第一人称射击游戏类型的基础，为现代开发者提供了对当时性能限制和创造性解决方案的洞察。 该渲染器采用射线投射方法，具有垂直墙壁和恒定的地板/天花板高度，类似于《德军总部 3D》，但增加了纹理地板和天花板。它还包含一个用于肢解效果的血腥碎片系统。

hackernews · sklopec · Jun 9, 10:46 · [社区讨论](https://news.ycombinator.com/item?id=48459294)

**背景**: 射线投射是一种快速的半 3D 渲染技术，用于《德军总部 3D》等早期游戏，通过从玩家视角投射射线来确定墙壁距离。与真正的 3D 光线追踪不同，射线投射计算成本低，在 1990 年代的硬件上即可实时运行。软件渲染意味着所有图形计算由 CPU 完成，无需 GPU 加速。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ray_casting">Ray casting - Wikipedia</a></li>
<li><a href="https://lodev.org/cgtutor/raycasting.html">Raycasting - Lode V</a></li>
<li><a href="https://lodev.org/cgtutor/raycasting2.html">Raycasting II: Floor and Ceiling - Lode V</a></li>

</ul>
</details>

**社区讨论**: 评论者指出该渲染器与《德军总部 3D》引擎相似，其中一位指出《毁灭战士》使用了更灵活的 BSP 引擎。另一位分享了为纹理添加光照贴图以实现动态光照效果（如闪烁的火炬）的技术。

**标签**: `#retro graphics`, `#software rendering`, `#raycasting`, `#game development`, `#computer history`

---

<a id="item-5"></a>
## [FCC 提议要求身份验证以消灭一次性手机](https://www.404media.co/fcc-wants-to-kill-burner-phones-by-forcing-telecoms-to-get-all-customers-ids/) ⭐️ 8.0/10

美国联邦通信委员会（FCC）提出一项新规，要求电信公司收集所有客户的身份信息，实际上将禁止被称为“一次性手机”的匿名预付费手机。 该提案可能消除记者、活动家和普通公民的一项重要隐私工具，同时引发对数据安全和政府监控的严重担忧。 该规则要求电信公司在销售点验证客户身份，类似于已在 155 个国家实施的强制性 SIM 卡注册法律。公众可通过 FCC 的电子评论提交系统提交意见。

hackernews · berlianta · Jun 9, 15:21 · [社区讨论](https://news.ycombinator.com/item?id=48462308)

**背景**: 一次性手机是无需身份证明即可购买的预付费移动设备，常用于短期通信以保护隐私。它们是合法的，常被记者、举报人和担心监控的个人使用。FCC 负责监管美国州际和国际通信。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Burner_phones">Burner phones</a></li>

</ul>
</details>

**社区讨论**: 评论者表示强烈反对，指出不信任电信公司保护个人数据的能力，一位用户分享了 AT&T 数据泄露的个人经历。其他人指出许多国家已要求 SIM 卡身份验证，但认为美国不应在没有强隐私保护的情况下效仿。

**标签**: `#privacy`, `#telecom regulation`, `#FCC`, `#surveillance`, `#civil liberties`

---

<a id="item-6"></a>
## [苹果因豁免请求被拒，不在欧盟推出 Siri](https://www.reuters.com/business/apple-failed-make-its-ai-tool-comply-eu-regulations-eu-commission-says-2026-06-09/) ⭐️ 8.0/10

苹果决定不在欧盟推出其增强版 Siri AI 功能，此前欧盟监管机构拒绝了其关于《数字市场法案》（DMA）的 18 个月豁免请求。 这一决定凸显了大型科技公司创新与欧盟严格隐私法规之间日益加剧的紧张关系，可能使苹果在欧洲市场处于竞争劣势，并影响数百万用户无法使用先进的 AI 功能。 苹果辩称，DMA 规则阻碍了其确保 Siri AI 隐私和安全的能力，而 Siri AI 依赖于设备端处理和私有云计算。欧盟则反驳称，苹果未能证明其请求符合 DMA 第 10 条规定的豁免法律标准。

hackernews · flanged · Jun 9, 16:13 · [社区讨论](https://news.ycombinator.com/item?id=48463024)

**背景**: 《数字市场法案》（DMA）是欧盟的一项法律，旨在通过对大型平台施加义务，使数字市场更加公平和更具竞争性。苹果为 iOS 27 和 iPadOS 27 宣布的 Siri AI 功能在设计上注重隐私，采用设备端处理和私有云计算。苹果请求从某些 DMA 义务中获得 18 个月的豁免以推出 Siri AI，但欧盟以不合规为由拒绝了该请求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://telecom.economictimes.indiatimes.com/news/devices/eu-rejects-apples-request-for-siri-ai-exemption-citing-compliance-issues/131622377">Digital Markets Act: EU Rejects Apple's Request for Siri AI Exemption ...</a></li>
<li><a href="https://www.apple.com/newsroom/2026/06/due-to-dma-siri-ai-delayed-in-eu-for-ios-27-and-ipados-27/">Due to DMA, Siri AI delayed in EU for iOS 27 and iPadOS 27 - Apple</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-06-08/apple-delays-siri-ai-for-iphone-users-in-eu-says-regulators-refusing-to-engage">Apple Delays Siri AI for iPhone Users in EU , Says Regulators ...</a></li>

</ul>
</details>

**社区讨论**: 评论观点不一：一些用户支持苹果的立场，认为欧盟法规为用户数据打开了后门；另一些用户则批评苹果指责欧盟，并希望平台更加开放。部分欧洲用户看到了本地替代方案的机会，少数人表示宁愿手机变笨也不愿看到欧盟向大型科技公司低头。

**标签**: `#Apple`, `#EU regulation`, `#privacy`, `#AI`, `#Siri`

---

<a id="item-7"></a>
## [苹果 AI 策略：隐私作为竞争优势](https://stratechery.com/2026/the-iphones-last-stand/) ⭐️ 8.0/10

Stratechery 的分析认为，苹果专注于设备端 AI 处理和隐私，而非基于云的 AI，尽管被认为落后于微软和 Meta 等竞争对手，但这可能是一种战略优势。 这一分析挑战了苹果在 AI 竞赛中落后的说法，表明其以隐私为中心的本地 AI 架构可能随着数据隐私问题的加剧而成为关键差异化因素。 文章强调，与竞争对手依赖云的方法相比，苹果的本地 AI 架构（包括设备端处理和私有云计算）在技术上更为先进。

hackernews · swolpers · Jun 9, 10:08 · [社区讨论](https://news.ycombinator.com/item?id=48459001)

**背景**: 苹果历来优先考虑用户隐私，并将其融入产品设计。在 AI 时代，当微软和 Meta 等竞争对手推动基于云的 AI 服务时，苹果开发了设备端 AI 能力和私有云基础设施，以在不暴露用户数据的情况下处理请求。

**社区讨论**: 评论者就苹果的本地 AI 方法是否真正优越展开辩论，一些人认为基于云的 AI 提供更强大的功能和灵活性，而另一些人则称赞苹果的隐私优先设计是长期优势。

**标签**: `#Apple`, `#AI`, `#hardware`, `#privacy`, `#strategy`

---

<a id="item-8"></a>
## [小米 1T 参数模型推理速度达 1000 tokens/s](https://platform.xiaomimimo.com/docs/en-US/model-intro/mimo-v2.5-pro-ultraspeed) ⭐️ 8.0/10

小米发布了 MiMo-V2.5-Pro-UltraSpeed，这是一个 1 万亿参数模型，通过 FP4 混合精度量化和 DFlash 推测解码在通用 GPU 上实现了 1000 tokens/s 的推理速度。 这一突破使得万亿参数模型能够部署在量化交易和实时风控等对延迟敏感的应用中，有望扩展大模型在高频决策场景中的使用。 API 试用价约为标准版 MiMo-V2.5-Pro 的 3 倍，速度提升约 10 倍。试用期为 6 月 9 日至 23 日，采用申请审批制，每日限排队 10 次、单次最多 30 分钟，优先面向企业用户开放。

telegram · zaihuapd · Jun 9, 03:26

**背景**: FP4 量化使用 4 位浮点数来减小模型大小并加速计算，而推测解码则使用较小的草稿模型提出多个 token，由较大的目标模型并行验证，从而在不牺牲输出质量的情况下降低延迟。TileRT 是一个用于超低延迟 LLM 推理的 tile 级运行时引擎，针对 B200 等特定 GPU 进行了优化。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://github.com/tile-ai/TileRT">GitHub - tile -ai/ TileRT : Tile -Based Runtime for Ultra-Low-Latency LLM...</a></li>

</ul>
</details>

**标签**: `#AI/ML`, `#model inference`, `#quantization`, `#Xiaomi`, `#large language model`

---

<a id="item-9"></a>
## [中国拟投 2 万亿元建设全国算力网络，优先采用国产 AI 芯片](https://www.scmp.com/tech/big-tech/article/3353891/china-ramps-building-national-computing-power-network-ai-token-demand-surges) ⭐️ 8.0/10

中国计划在未来五年（2026-2030 年）投入约 2 万亿元人民币（2950 亿美元），建设全国性算力网络，由国有电信企业运营主要设施，并优先采用华为等本土供应商的 AI 芯片，占比至少 80%。 这一巨额投资凸显了中国减少对英伟达、AMD 等美国芯片供应商依赖的战略决心，同时通过整合算力资源，有望加速各行业 AI 应用，提升国家 AI 竞争力。 该计划是北京“六网”基础设施计划的关键一环，中国电信、联通等运营商已推出“算力 Token 套餐”，将算力像移动数据一样打包销售，让企业和公众更易获得高性能计算。

telegram · zaihuapd · Jun 9, 10:09

**背景**: 中国的“六网”基础设施计划涵盖新型电网、城市地下管网等六大网络，其中算力网旨在将分散的区域算力资源整合为全国统一网络。基于 Token 的定价方式（算力以 Token 计量，类似 AI 模型中的词元）是一种将算力商品化的创新模式，便于更广泛的用户购买和使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260609A07IZQ00">一文详解2万亿AI基础设施计划，历史以来规模最大，80%国产</a></li>
<li><a href="https://www.gov.cn/yaowen/liebiao/202605/content_7069999.htm">我国将抓紧出台“六张网”相关规划和实施方案__中国政府网</a></li>
<li><a href="https://www.guandian.cn/article/20260422/556949.html">中国移动北京公司推出个人 算 力 Token 套 餐 最低5.99元起 - 观点网</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#China tech`, `#computing power`, `#chip independence`, `#national network`

---

<a id="item-10"></a>
## [AI 取代员工？那是糟糕的 CEO](https://www.techdirt.com/2026/06/09/ceos-who-think-ai-replaces-their-employees-are-just-bad-ceos/) ⭐️ 7.0/10

Techdirt 的一篇评论文章指出，那些认为 AI 可以取代员工的 CEO 误解了 AI 的局限性以及人类员工的价值，文章基于数十年的产品交付和支持经验。 这一观点挑战了 AI 导致失业的主流叙事，强调人类判断力、支持能力和交付经验仍然不可替代。它引发了关于企业应如何负责任地整合 AI 的讨论。 作者用比喻说明，交付产品远比设计产品复杂得多，而 AI 无法处理交付和支持中细微的现实挑战。该文章在 Techdirt 上有 165 条评论和 413 分。

hackernews · speckx · Jun 9, 18:45 · [社区讨论](https://news.ycombinator.com/item?id=48465675)

**背景**: 这篇文章是对企业利用 AI 自动化任务并取代员工这一趋势的回应。它认为许多 CEO 低估了产品交付和客户支持所需的人力投入，而这些正是 AI 目前力所不及的领域。

**社区讨论**: 评论者大多同意文章观点，有人补充说糟糕的 CEO 往往缺乏做好本职工作的能力。一位评论者建议 CEO 在替换他人之前先用 AI 替换自己的助理，另一位则打趣说 AI 或许很擅长替换 CEO 本身。

**标签**: `#AI`, `#management`, `#employment`, `#technology-critique`

---

<a id="item-11"></a>
## [Karpathy：AI 软件需求因杰文斯悖论激增](https://simonwillison.net/2026/Jun/9/andrej-karpathy/#atom-everything) ⭐️ 7.0/10

Andrej Karpathy 在 Twitter（通过 Claude Fable 5）上发帖称，随着 AI 按需生成可工作的软件，他个人对定制应用的需求大幅增长，并引用了杰文斯悖论。 这位 AI 领军人物提出的见解表明，AI 驱动的软件生成不会减少对开发者的需求，反而会大幅增加对定制应用的需求，从而重塑软件行业。 Karpathy 特别提到了解释器、可视化工具、仪表盘以及为单个项目定制的超特定 wandb 克隆等例子，展示了新可能性的广度。

rss · Simon Willison · Jun 9, 19:03

**背景**: 杰文斯悖论最早于 1865 年被观察到，描述了资源使用效率的提高如何导致总体消费增加。在此背景下，AI 使软件生成更高效，降低了创建定制应用的成本，反而增加了对软件的总体需求，而非减少。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jevons_paradox">Jevons paradox</a></li>
<li><a href="https://github.com/wandb/wandb">GitHub - wandb/wandb: The AI developer platform. Use Weights ... wandb · PyPI wandb (Weights and Biases) - Hugging Face wandb安装与使用 —— 用于跟踪、可视化和协作机器学习实验的工具-CSDN... 新手教程|如何使用 WandB 监控大模型的训练与调试 quickstart - W&B</a></li>

</ul>
</details>

**标签**: `#AI`, `#software development`, `#Jevons paradox`, `#generative AI`

---

<a id="item-12"></a>
## [苹果 WWDC 2026：Siri AI 采用视觉大模型和 Gemini](https://simonwillison.net/2026/Jun/8/wwdc/#atom-everything) ⭐️ 7.0/10

在 WWDC 2026 上，苹果宣布了新的 Siri AI 功能，利用视觉大模型从用户屏幕提取信息，并授权一个定制的 Gemini 衍生模型用于复杂推理任务，该模型运行在扩展到 Google Cloud 并使用 NVIDIA GPU 的 Private Cloud Compute 基础设施上。 与 2024 年过度承诺相比，这标志着苹果 AI 愿景更可行的实现方式，可能实现更深入的设备端和云端 AI 集成，而无需每个应用编写自定义代码。 新的 Core AI 库通过 Core AI PyTorch 扩展桥接 PyTorch 和苹果硬件，允许开发者运行自己的模型。PCC 上的 Gemini 模型使用 Google Cloud 和 NVIDIA GPU，苹果发布所有二进制文件供公众检查。

rss · Simon Willison · Jun 8, 23:58

**背景**: 苹果 2024 年的 Apple Intelligence 公告因过于雄心勃勃且交付不足而受到批评。视觉大模型（能理解屏幕视觉内容）在 2024 年尚不成熟，但此后已取得进展。Private Cloud Compute（PCC）是苹果用于 AI 推理的安全云基础设施，现已扩展到 Google Cloud。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://security.apple.com/blog/expanding-pcc/">Expanding Private Cloud Compute - Apple Security Research</a></li>

</ul>
</details>

**社区讨论**: Simon Willison 表达了谨慎乐观，指出可行性有所改进，但由于过去的过度承诺，他坚持“眼见为实”的态度。他强调使用视觉大模型和 Gemini 授权是务实的步骤。

**标签**: `#Apple`, `#Siri`, `#AI`, `#WWDC`, `#Vision LLM`

---

<a id="item-13"></a>
## [Z-Library 推出白标镜像，用户可自建品牌登录站](https://torrentfreak.com/z-library-lets-people-run-white-label-login-only-pirate-mirrors/) ⭐️ 7.0/10

Z-Library 推出了白标镜像功能，允许用户创建带独立品牌、仅限登录访问的镜像站点，且不显示 Z-Library 标识，运营者可获得 20% 的加密货币捐赠分成。 该功能使 Z-Library 的访问去中心化，增加了版权方识别和封锁镜像的难度，并通过收入分成激励社区参与。 镜像运营者通过加密货币获得 20% 的捐赠分成，Z-Library 还提供离线域名列表文件，让用户本地保存所有访问入口以应对全面封禁。

telegram · zaihuapd · Jun 9, 05:55

**背景**: Z-Library 是一个影子图书馆项目，提供数百万册图书和学术文章的免费访问，经常面临法律挑战和域名查封。白标镜像允许第三方托管带有自己品牌的网站版本，隐藏其来源，使执法更加困难。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Z-Library">Z-Library</a></li>

</ul>
</details>

**标签**: `#Z-Library`, `#piracy`, `#digital rights`, `#anti-censorship`, `#mirroring`

---

<a id="item-14"></a>
## [阿里巴巴洽谈小型核反应堆为数据中心供电](https://www.stcn.com/article/detail/3950643.html) ⭐️ 7.0/10

阿里巴巴已与一家核电央企接触，探讨建设小型模块化反应堆（SMR）为其杭州仁和数据中心供电，谈判核心集中在电价与供电模式上。 此举标志着科技巨头为满足 AI 工作负载激增的电力需求而转向核能的重大趋势，可能重塑全球数据中心的能源策略。 考虑中的 SMR 可能基于中核集团的“玲龙一号”（ACP100），这是全球首个通过国际原子能机构安全审查的小型模块化反应堆，计划于 2026 年投入商业运营。

telegram · zaihuapd · Jun 9, 10:54

**背景**: 小型模块化反应堆（SMR）是先进的核反应堆，每台发电容量可达 300 兆瓦，设计上支持工厂制造和模块化部署。它们能提供稳定、无碳的电力，适合数据中心。Meta、亚马逊、谷歌等科技巨头也在探索 SMR 以满足其能源需求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260609A02R4U00">阿里巴巴接洽核电央企 探讨小型反应堆为数据中心供电</a></li>
<li><a href="https://www.163.com/dy/article/KV0I40EP05118I96.html">阿里洽谈小型核反应堆为数据中心供电|电厂|核电站|阿里巴巴集团|新型...</a></li>
<li><a href="http://www.cb.com.cn/index/show/jj/cv/cv135401422062">阿里巴巴接洽核电央企 探讨小型反应堆为数据中心供电</a></li>

</ul>
</details>

**标签**: `#AI infrastructure`, `#nuclear energy`, `#data centers`, `#Alibaba`, `#energy`

---

<a id="item-15"></a>
## [朱雀二号发射卫星，开展手机直连试验](https://www.news.cn/20260609/4958e6730eba485fae66a56a5b21458a/c.html) ⭐️ 7.0/10

2025 年 6 月 9 日，朱雀二号改进型遥六火箭成功将千帆 DTC01 星和中国移动 02 星送入预定轨道，这两颗卫星将开展手机宽带直连卫星和天地网络融合等技术试验。 此次任务标志着中国商业航天和卫星互联网发展的重要一步，手机直连技术无需专用终端即可实现无处不在的连接，有望与星链的直接对手机服务竞争。 朱雀二号遥六为两级低温液体火箭，直径 3.35 米，近地轨道运载能力 6 吨。千帆 DTC01 星由上海垣信运营，中国移动 02 星将验证手机宽带直连卫星技术。

telegram · zaihuapd · Jun 9, 14:20

**背景**: 朱雀二号是中国民营企业蓝箭航天开发的液体燃料火箭。手机直连卫星技术允许普通智能手机直接连接卫星，无需笨重的卫星电话。千帆星座（又称 G60 星链）是中国低轨卫星互联网项目，计划部署超过 1.5 万颗卫星以实现全球覆盖。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://user.guancha.cn/main/content?id=1667424">朱 雀 二 号 改进型遥六运载 火 箭 发射成功_风闻</a></li>
<li><a href="https://wap.eastmoney.com/a/202606093765229138.html">朱 雀 二 号 遥六发射成功 将开展手机直连卫星试验 _ 东方财富网</a></li>
<li><a href="https://www.thecover.cn/news/pkGxb4dKuoeH90qSdq8Jkw==">朱 雀 二 号 遥六发射成功，千帆DTC01星等两颗卫星顺利入轨 - 封面新闻</a></li>

</ul>
</details>

**标签**: `#spaceflight`, `#satellite`, `#telecommunications`, `#aerospace`

---

<a id="item-16"></a>
## [国家互联网应急中心警告 AI 智能体技能包存在越狱和挖矿风险](https://www.yicai.com/brief/103222242.html) ⭐️ 7.0/10

2026 年 6 月 9 日，国家互联网应急中心（CNCERT）发布官方警告，称部分智能体技能包（Skills）以“大模型越狱”和“挖矿赚钱”为名传播，能够突破模型安全限制或占用设备资源进行非法挖矿。 这一警告揭示了 AI 生态系统中一种新的攻击途径——看似有用的技能包可能危及用户安全和系统完整性。它凸显了对第三方 AI 智能体扩展进行更严格审查的紧迫性，影响数百万用户和开发者。 恶意技能包可能导致模型生成违法信息、账号被封禁、设备性能下降，甚至使用户卷入洗钱活动。CNCERT 敦促用户和运营单位审查技能来源、监控行为，并清除可疑组件。

telegram · zaihuapd · Jun 9, 16:58

**背景**: AI 智能体技能包（Skills）是基于大语言模型（LLM）的智能体的模块化扩展，用于增强数据分析或文档生成等能力。“越狱”指诱使大模型绕过安全限制的技术，“挖矿”指未经同意利用设备算力挖掘加密货币。CNCERT 是中国国家网络安全应急响应中心。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KV0LQF7205198CJN.html">国家互联网应急中心：部分智能体技能包（Skills）存在越狱和挖矿风险...</a></li>
<li><a href="https://www.nbd.com.cn/articles/2026-06-09/4421403.html">国家互联网应急中心提醒：部分智能体技能包（Skills）存在越狱和挖矿...</a></li>
<li><a href="https://finance.eastmoney.com/a/202606093765264792.html">国家互联网应急中心提醒：部分智能体技能包（Skills）存在越狱和挖矿...</a></li>

</ul>
</details>

**标签**: `#AI safety`, `#cybersecurity`, `#large language models`, `#cryptomining`, `#jailbreak`

---