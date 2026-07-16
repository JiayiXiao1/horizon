---
layout: default
title: "Horizon Summary: 2026-07-16 (ZH)"
date: 2026-07-16
lang: zh
---

> From 35 items, 20 important content pieces were selected

---

1. [Stripe 与 Advent 联合出价超 530 亿美元收购 PayPal](#item-1) ⭐️ 9.0/10
2. [Thinking Machines 发布开放权重多模态模型 Inkling](#item-2) ⭐️ 8.0/10
3. [xAI 开源 Grok 构建系统](#item-3) ⭐️ 8.0/10
4. [Gemma 4 26B 在 13 年前的 Xeon CPU 上以 5 tokens/秒运行](#item-4) ⭐️ 8.0/10
5. [Telegram 数据中心：编号、位置与 FSB 关联](#item-5) ⭐️ 8.0/10
6. [睡眠规律性比时长更能预测死亡风险](#item-6) ⭐️ 8.0/10
7. [Claude web_fetch 工具绕过漏洞导致数据通过提示注入泄露](#item-7) ⭐️ 8.0/10
8. [Lobste.rs 从 MariaDB 迁移到 SQLite](#item-8) ⭐️ 8.0/10
9. [Armin Ronacher：摩擦构建共享理解，AI 代理可能绕过它](#item-9) ⭐️ 8.0/10
10. [DeepSeek 首轮融资 74 亿美元，采用特殊架构维持创始人控制](#item-10) ⭐️ 8.0/10
11. [马斯克：X 将无条件开源全部代码](#item-11) ⭐️ 8.0/10
12. [开发者利用沙盒逃逸让 Filza 读取 iOS 27 备忘录数据库](#item-12) ⭐️ 8.0/10
13. [Telegram 推出机器人后端无服务器平台](#item-13) ⭐️ 8.0/10
14. [软件开发中的心理健康与沟通](#item-14) ⭐️ 7.0/10
15. [Dependabot 默认对版本更新实施三天冷却期](#item-15) ⭐️ 7.0/10
16. [在 GitHub Actions 中缓存友好地使用 uvx](#item-16) ⭐️ 7.0/10
17. [包括 Apple 智能在内的 7 款手机端侧 AI 模型获中国备案](#item-17) ⭐️ 7.0/10
18. [中国零售业边界模糊：山姆、零食店、拼多多争夺同一钱包](#item-18) ⭐️ 7.0/10
19. [法官质疑 Epic 与谷歌反垄断和解背后 800 万美元合作](#item-19) ⭐️ 7.0/10
20. [ASML 计划提高 EUV 和 DUV 光刻设备价格](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Stripe 与 Advent 联合出价超 530 亿美元收购 PayPal](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

据消息人士透露，Stripe 与私募股权公司 Advent International 联合出价超过 530 亿美元收购 PayPal。 此次收购将整合两大支付平台，引发重大反垄断担忧，可能减少在线支付领域的竞争，从而影响数百万企业和消费者。 该交易将把 Stripe 基于 API 的现代支付基础设施与 PayPal 面向消费者的品牌（如 Venmo 和 Braintree）整合在一起，形成一个在非面对面交易中拥有巨大市场力量的实体。

hackernews · rvz · Jul 15, 03:32 · [社区讨论](https://news.ycombinator.com/item?id=48915953)

**背景**: Stripe 是一家估值约 1590 亿美元的私有金融科技公司，2025 年为 500 万家企业处理了超过 1.9 万亿美元的支付。Advent International 是一家专注于收购的全球私募股权公司。PayPal 成立于 1998 年，是一家上市公司，旗下拥有 Venmo、Braintree 和 Xoom，近年来面临来自 Stripe 日益激烈的竞争。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stripe,_Inc.">Stripe, Inc. - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论表达了对竞争减少、费用上涨以及 Stripe 对某些行业（如大麻和成人内容）限制政策的强烈担忧。一些用户担心这会影响他们转账的能力以及账户被冻结的风险，而另一些人则质疑该交易能否通过反垄断审查。

**标签**: `#acquisition`, `#payments`, `#antitrust`, `#fintech`, `#Stripe`

---

<a id="item-2"></a>
## [Thinking Machines 发布开放权重多模态模型 Inkling](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines 发布了 Inkling，一个支持音频的开放权重多模态模型，专为定制化和高效本地推理而设计。 Inkling 是支持音频的最大开放权重模型，使企业能够以更低成本本地微调和部署自有模型，可能挑战闭源替代方案。 Inkling 可在 Tinker 平台上进行微调，社区成员已创建 GGUF 和 NVFP4 量化版本用于本地推理。该模型并非整体最强，但结合了多模态能力、高效推理和定制化选项。

hackernews · vimarsh6739 · Jul 15, 18:12 · [社区讨论](https://news.ycombinator.com/item?id=48924912)

**背景**: 开放权重模型公开发布训练后的参数，允许任何人下载并本地运行。多模态模型可处理文本、音频和图像等多种数据类型。本地推理在边缘设备上运行模型，无需依赖云端，具有隐私和成本优势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_model">Multimodal model</a></li>

</ul>
</details>

**社区讨论**: 评论者对 Inkling 的音频支持和本地部署潜力感到兴奋，有人将其与 DeepSeek 比较，并认为 Thinking Machines 可能成为关键参与者。社区还分享了量化工具和微调资源的技术链接。

**标签**: `#open-weights`, `#multimodal`, `#AI`, `#machine learning`, `#audio`

---

<a id="item-3"></a>
## [xAI 开源 Grok 构建系统](https://github.com/xai-org/grok-build) ⭐️ 8.0/10

xAI 已在 GitHub 的 xai-org/grok-build 仓库中开源了 Grok 构建系统，这是一个基于 Rust 的 CLI/TUI 工具，用于其 AI 代理运行时。 此举允许社区检查、修改和分叉代码，有望在隐私丑闻（该工具被发现将整个目录上传到 xAI 的云）后提高透明度和信任度。 代码库包含一个使用 Unicode 框绘图的独立终端 Mermaid 图表渲染器，并且该仓库会定期从 xAI 的内部单体仓库同步。

hackernews · skp1995 · Jul 15, 20:24 · [社区讨论](https://news.ycombinator.com/item?id=48926590)

**背景**: Grok 是 xAI 开发的 AI 聊天机器人，提供语音聊天、图像/视频生成和高级推理功能。作为 Grok 生态系统一部分的 CLI 工具，因未经同意上传用户数据而遭到强烈反对，促使 xAI 开源构建系统作为危机管控措施。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">GitHub - xai -org/ grok - build : SpaceXAI's coding agent harness and...</a></li>
<li><a href="https://x.ai/open-source">Grok Build CLI is open source. Browse the code on GitHub. | SpaceXAI</a></li>

</ul>
</details>

**社区讨论**: 社区反应不一：一些人称赞开源并注意到有趣的技术细节（如 Mermaid 渲染器），而另一些人则批评此举是对隐私丑闻的策略性公关回应。已经出现了分叉，例如一个注重隐私的分叉，移除了遥测并阻止自动更新。

**标签**: `#open source`, `#AI`, `#Grok`, `#privacy`, `#xAI`

---

<a id="item-4"></a>
## [Gemma 4 26B 在 13 年前的 Xeon CPU 上以 5 tokens/秒运行](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

一篇技术博客展示了如何通过量化和 CPU 优化，在没有 GPU 的 13 年前双路 Xeon 服务器上，以每秒 5 个 token 的速度运行 Google 的 Gemma 4 26B A4B 模型。 这表明现代大语言模型可以在极其老旧的硬件上运行，降低了本地 AI 推理的门槛，并引发了关于与云 API 相比成本效益的讨论。 Gemma 4 26B A4B 模型采用混合专家架构，总参数量 26B，激活参数量 4B，专为高效推理设计。该设置可能使用了 4 位量化和 CPU 特定优化，在双路 Xeon E5-2690 v2（Ivy Bridge）系统上实现了 5 tokens/秒。

hackernews · neomindryan · Jul 15, 15:34 · [社区讨论](https://news.ycombinator.com/item?id=48922434)

**背景**: 大语言模型通常需要强大的 GPU 才能快速推理。然而，量化（降低数值精度）和 CPU 优化推理库等技术使得这些模型能在老旧硬件上运行。Gemma 4 是谷歌最新的开放模型系列，其中 26B A4B 变体在规模和速度之间取得了平衡。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 4 model overview - Google AI for Developers</a></li>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://www.intel.com/content/www/us/en/developer/articles/technical/boost-performance-llms-pytorch-xeon-processors-pt2.html">Boost Performance for LLMs Using PyTorch: Part 2 - Intel</a></li>

</ul>
</details>

**社区讨论**: 评论者就成本效率展开辩论：一些人指出运行这种老旧硬件的电费可能超过云 API 价格，而另一些人则强调本地推理在隐私和离线使用方面的价值。有用户预测到 2027 年中，200B 参数的 MoE 模型将能在消费级硬件上运行，并引用自己在 MacBook Air 上运行 35B 模型的经验。

**标签**: `#LLM`, `#inference optimization`, `#local AI`, `#hardware`, `#cost analysis`

---

<a id="item-5"></a>
## [Telegram 数据中心：编号、位置与 FSB 关联](https://dev.moe/en/3025) ⭐️ 8.0/10

一项深入分析揭示了 Telegram 的数据中心编号方案（DC1-5）、其位置（迈阿密、阿姆斯特丹、新加坡）以及运营怪癖，例如 DC3 的神秘缺失和 DC5 对中国用户的频繁宕机。 这很重要，因为 Telegram 的基础设施选择影响用户隐私和可靠性；与 FSB 的潜在重叠引发了对元数据监控和该应用隐私保证的严重担忧。 Telegram 声称有五个数据中心（DC1-5），其中 DC1 和 DC3 位于迈阿密，DC2 和 DC4 位于阿姆斯特丹，DC5 位于新加坡；DC3 在公开文档中明显缺失，而 DC5 经常宕机，影响中国用户。

hackernews · theanonymousone · Jul 15, 13:22 · [社区讨论](https://news.ycombinator.com/item?id=48920475)

**背景**: Telegram 是一款基于云的即时通讯应用，由帕维尔·杜罗夫和尼古拉·杜罗夫于 2013 年创立，以其对安全性和隐私的关注而闻名。其服务器分布在全球各地，在代码和文档中数据中心以编号（DC1-5）标识。OCCRP 和 Istories 最近的调查将 Telegram 的基础设施与一家与 FSB 有关联的俄罗斯承包商联系起来，暗示存在元数据监控风险。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://dev.moe/en/3025">Mysteries of Telegram DC - Coxxs</a></li>
<li><a href="https://istories.media/en/stories/2025/06/10/telegram-fsb/">Telegram, the FSB, and the Man in the Middle - istories.media</a></li>
<li><a href="https://en.wikipedia.org/wiki/Telegram_(software)">Telegram (software) - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区评论强调了与 FSB 基础设施的重叠，并附有 Istories 调查的链接。用户指出 DC2 为俄罗斯和乌克兰用户服务且经常宕机，而 DC3 的缺失引发了对特殊账户数据的猜测。一些人质疑自定义数据中心处理的技术债务。

**标签**: `#Telegram`, `#data centers`, `#infrastructure`, `#security`, `#privacy`

---

<a id="item-6"></a>
## [睡眠规律性比时长更能预测死亡风险](https://academic.oup.com/sleep/article/47/1/zsad253/7280269) ⭐️ 8.0/10

2023 年发表在《睡眠》期刊上的一项研究发现，睡眠规律性（即入睡和醒来时间的一致性）比睡眠时长更能预测全因死亡风险。 这将关注点从睡眠时长转向睡眠时间的规律性，为改善寿命提供了一个可调整的目标。它挑战了公共卫生指南中仅强调睡眠时长的常见做法。 该研究分析了英国生物银行超过 6 万名参与者的数据，使用基于加速度计的睡眠规律性指数（SRI）评分。与睡眠不规律者相比，睡眠规律者的死亡风险降低 20-48%，且独立于睡眠时长。

hackernews · bilsbie · Jul 15, 11:46 · [社区讨论](https://news.ycombinator.com/item?id=48919363)

**背景**: 睡眠规律性衡量的是每日睡眠-觉醒时间的一致性，通常用睡眠规律性指数（SRI）来量化。以往研究主要关注睡眠时长作为关键健康指标，但这项研究强调了昼夜节律对齐的重要性。研究结果表明，保持一致的睡眠时间表可能比固定睡眠时长更为关键。

**社区讨论**: 评论者讨论了潜在的混杂变量，如职业和轮班工作，一些人指出研究调整了轮班工作但未针对具体职业进行调整。其他人分享了通过补充镁改善睡眠的个人经验，而少数人批评该研究为观察性研究，易受混杂因素影响。

**标签**: `#sleep`, `#health`, `#longevity`, `#research`, `#epidemiology`

---

<a id="item-7"></a>
## [Claude web_fetch 工具绕过漏洞导致数据通过提示注入泄露](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

研究员 Ayush Paul 发现 Anthropic 的 Claude web_fetch 工具存在一个绕过漏洞，攻击者可通过从恶意站点获取的嵌套链接链来窃取用户记忆（姓名、位置、雇主）。Anthropic 已通过禁止 web_fetch 跟随获取内容中的链接来修复该漏洞。 该攻击表明，即使是精心设计的 AI 安全措施也可能被绕过，凸显了保护能访问私有数据和外部工具的 LLM 代理所面临的持续挑战。它强调了在生产级 AI 系统中针对间接提示注入和数据泄露建立强大防御的必要性。 该攻击利用了一个漏洞：web_fetch 被允许访问先前获取页面中嵌入的 URL，从而使得一个蜜罐站点能够通过引导代理跟随一系列生成的链接来窃取数据。恶意站点仅对 User-Agent 中包含 'Claude-User' 的客户端提供攻击内容以逃避检测。Anthropic 未支付漏洞赏金，声称他们已在内部发现了该问题。

rss · Simon Willison · Jul 15, 14:21

**背景**: 提示注入是一种安全漏洞，恶意输入会导致 LLM 产生意外行为。在“致命三重奏”场景中，能够访问私有数据并拥有获取网页内容工具的 LLM 可能被诱骗通过其访问的 URL 泄露数据。Claude 的 web_fetch 工具原本设计为仅导航到用户提供的 URL 或其 web_search 工具返回的结果，但嵌套链接漏洞使得间接提示注入能够绕过这一限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://cdn.openai.com/pdf/dd8e7875-e606-42b4-80a1-f824e4e11cf4/prevent-url-data-exfil.pdf">Preventing URL -Based Data Exfiltration in Language-Model Agents</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者对漏洞的严重性表示担忧，并批评 Anthropic 在研究员负责任披露后未支付漏洞赏金。一些人争论修复是否完全解决了根本原因，而另一些人则称赞技术文章清晰明了。

**标签**: `#AI safety`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#security`

---

<a id="item-8"></a>
## [Lobste.rs 从 MariaDB 迁移到 SQLite](https://simonwillison.net/2026/Jul/14/lobsters-sqlite/#atom-everything) ⭐️ 8.0/10

社区新闻网站 Lobste.rs 已完成从 MariaDB 到 SQLite 的迁移，现在完全运行在单个 VPS 上，性能提升且成本降低。 这一真实案例表明，SQLite 可以作为中等规模 Web 应用的主要数据库，挑战了“始终需要客户端-服务器数据库”的假设。 迁移后主 SQLite 数据库大小为 3.8GB，另有独立的缓存、队列和 rack_attack 数据库。CPU 和内存使用率下降，网站响应更快，停用 MariaDB 服务器后 VPS 成本减半。

rss · Simon Willison · Jul 14, 19:44

**背景**: SQLite 是一种无服务器、嵌入式关系数据库引擎，将数据存储在单个文件中，无需单独的数据库服务器。它常用于移动应用和小型网站，但较少作为多用户 Web 应用的主要数据库。Lobste.rs 是一个基于 Rails 的计算机讨论社区网站，类似于 Hacker News。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/lobsters/lobsters">GitHub - lobsters / lobsters : Computing-focused community centered...</a></li>
<li><a href="https://www.sqlitetutorial.net/">SQLite Tutorial - An Easy Way to Master SQLite Fast</a></li>

</ul>
</details>

**社区讨论**: Lobste.rs 社区讨论氛围积极，网站管理员报告 SQLite 表现优异。评论者分享了迁移过程的技术细节，并对该架构表示兴趣。

**标签**: `#SQLite`, `#database migration`, `#Rails`, `#performance`, `#web architecture`

---

<a id="item-9"></a>
## [Armin Ronacher：摩擦构建共享理解，AI 代理可能绕过它](https://simonwillison.net/2026/Jul/14/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher 认为，软件项目中的共享理解是通过摩擦（如代码审查和跨团队协调）来维持的，而 AI 编码代理可能绕过这种摩擦，从而侵蚀维持系统一致性的协作知识。 随着 AI 代理自主编写和修改代码的能力增强，团队可能会失去同步贡献者之间理解的关键人际过程，导致知识碎片化和系统维护难度增加。 Ronacher 的文章《塔楼不断上升》指出，项目中的共享语言包括关于概念、边界、不变量和所有权的未书面知识，这些知识是通过向他人解释变更等摩擦建立起来的。

rss · Simon Willison · Jul 14, 18:04

**背景**: 软件团队中的共享理解是关于系统如何工作以及为何如此设计的集体知识，通常是隐性的，分布在文档、代码和对话中。摩擦——例如协调变更所需的努力——迫使开发人员沟通并调整他们的心智模型，这对于长期可维护性至关重要。能够在不产生这种摩擦的情况下进行更改的 AI 代理可能会产生孤立工作的代码，但会破坏团队的一致性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://lucumr.pocoo.org/2026/7/13/the-tower-keeps-rising/">Vibecoding and the possible collapse of a shared language.</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-agents-engineering-teams-powerful-tools-yet-andras-ludanyi-9x6ie">AI Agents in Engineering Teams: Powerful Tools, But Not Yet...</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>

</ul>
</details>

**标签**: `#software engineering`, `#AI agents`, `#collaboration`, `#shared understanding`, `#code review`

---

<a id="item-10"></a>
## [DeepSeek 首轮融资 74 亿美元，采用特殊架构维持创始人控制](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek 在首轮融资中筹得逾 500 亿元人民币（约 74 亿美元），估值超过 500 亿美元。本轮采用非常规架构，投资者需将资金注入由 CEO 梁文锋管理的有限合伙企业，并接受五年锁定期且不享有表决权。 这笔巨额融资凸显了 DeepSeek 作为主要 AI 参与者的迅速崛起，挑战了 OpenAI 等全球领导者。独特的治理结构使创始人梁文锋在吸引腾讯和宁德时代等战略投资者的同时保持控制权，为 AI 初创企业融资树立了先例。 创始人梁文锋在本轮融资中个人投资 200 亿元。腾讯考虑投资 100 亿元，宁德时代计划投资 50 亿元，可能成为最大的外部投资者。DeepSeek 对此暂未置评。

telegram · zaihuapd · Jul 15, 12:56

**背景**: DeepSeek 是一家中国 AI 公司，由梁文锋于 2023 年 7 月创立，梁文锋同时管理对冲基金幻方量化。该公司在 2025 年 1 月凭借 R1 模型获得全球关注，该模型以极低的成本达到了 GPT-4 的性能。公司采用在中国常见的有限合伙架构，创始人作为普通合伙人（GP）保留控制权，而投资者作为有限合伙人（LP）权利有限。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_AI_Research">DeepSeek AI Research</a></li>
<li><a href="https://zh.wikipedia.org/wiki/深度求索">深度求索 - 维基百科，自由的百科全书</a></li>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=4930dbb9aae194241204">有限合伙企业如何实现控制权 - ailegal.baidu.com</a></li>

</ul>
</details>

**标签**: `#AI`, `#funding`, `#DeepSeek`, `#startup`, `#governance`

---

<a id="item-11"></a>
## [马斯克：X 将无条件开源全部代码](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 8.0/10

埃隆·马斯克宣布，在完成安全漏洞审查后，X 将无条件开源其全部代码库，并邀请第三方审查者验证正在运行的系统与开源代码一致。 此举可能显著提升 X 平台的透明度和信任度，为社交媒体公司在代码开放和独立验证方面树立新标准。 开源将在安全漏洞审查后进行，第三方审查者将检查实时系统与开源代码是否一致。马斯克强调，完全透明带来的信任是唯一值得相信的东西。

telegram · zaihuapd · Jul 15, 13:32

**背景**: X（前身为 Twitter）自成立以来一直是一个专有平台。开源整个代码库将允许任何人检查、审计和贡献代码，可能提升安全性和问责性。这一声明是马斯克在平台上推动透明度和言论自由的更广泛努力的一部分。

**标签**: `#open source`, `#social media`, `#transparency`, `#Elon Musk`, `#X`

---

<a id="item-12"></a>
## [开发者利用沙盒逃逸让 Filza 读取 iOS 27 备忘录数据库](https://x.com/0xjohnny/status/2077216973256274272) ⭐️ 8.0/10

开发者 johnny 修改了 iOS 文件管理工具 Filza，利用 iOS 27 beta 3 上的沙盒逃逸漏洞，使修改后的工具能够在 iPhone 17 Pro Max 上访问备忘录数据库。 这展示了最新 iOS beta 上的重大安全绕过，突显了持续的沙盒弱点，可能被恶意应用利用或用于越狱开发。 该漏洞针对应用沙盒容器限制，修改后的 Filza 可以浏览其自身容器之外的外部数据。所使用的具体漏洞尚未公开。

telegram · zaihuapd · Jul 15, 14:35

**背景**: Filza 是一款流行的 iOS 文件管理器，通常只能在应用的沙盒内运行。沙盒逃逸漏洞允许应用突破其受限环境，访问其他应用的数据或系统文件。iOS 27 是苹果移动操作系统的最新主要版本，目前处于测试阶段。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.tigisoftware.com/default/?page_id=78">Filza – TIGI Software</a></li>
<li><a href="https://medium.com/ssd-secure-disclosure/ios-vulnerabilities-3-sandbox-escape-cves-5233c92ad875">iOS Vulnerabilities — 3 Sandbox Escape CVE’s you should know | by Imriah | SSD Secure Disclosure | Medium</a></li>

</ul>
</details>

**标签**: `#iOS security`, `#sandbox escape`, `#jailbreak`, `#vulnerability`, `#Filza`

---

<a id="item-13"></a>
## [Telegram 推出机器人后端无服务器平台](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram 正式推出无服务器平台，开发者可以使用纯 JavaScript 模块编写机器人和 Mini App 的后端代码，并通过一条 CLI 命令直接部署在 Telegram 的基础设施上。 这消除了开发者管理服务器、容器或扩展的需求，大幅降低了运维成本，并降低了构建 Telegram 机器人和 Mini App 的门槛。 该平台在紧邻 Bot API 的隔离 V8 沙箱中运行代码，并内置了 SQLite 数据库。部署通过命令 'npx tgcloud push' 完成。

telegram · zaihuapd · Jul 15, 16:00

**背景**: 无服务器计算允许开发者编写和部署代码，而无需配置或管理服务器，由云提供商处理扩展和基础设施。Telegram 的平台专门针对其机器人生态系统设计，此前开发者需要自行托管服务器来处理 webhook 更新或轮询。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/07/15/telegram-serverless-bots-without-a-server/">Telegram Serverless: serverless bot backends - elsolitario.org</a></li>
<li><a href="https://daily.dev/posts/telegram-serverless-uej7tlh7t">Telegram Serverless - daily.dev</a></li>

</ul>
</details>

**标签**: `#serverless`, `#Telegram`, `#bots`, `#JavaScript`, `#cloud computing`

---

<a id="item-14"></a>
## [软件开发中的心理健康与沟通](https://ramones.dev/posts/mental-health/) ⭐️ 7.0/10

一篇个人博客文章强调了心理健康和沟通对软件开发者的重要性，引发了关于神经多样性和自我管理的社区讨论。 这个话题与软件工程师高度相关，因为心理健康挑战和沟通问题在科技行业很常见，讨论为自我管理提供了实用见解。 该帖子获得了 285 个点赞和 245 条评论，表明在社区中引起了强烈共鸣。评论者分享了个人经历和管理神经多样性及改善沟通的策略。

hackernews · ramon156 · Jul 15, 11:27 · [社区讨论](https://news.ycombinator.com/item?id=48919198)

**背景**: 科技行业的心理健康是一个日益被讨论的话题，许多开发者面临倦怠、冒名顶替综合症和沟通障碍。神经多样性（如 ADHD 或自闭症）可能影响工作模式，需要量身定制的应对策略。

**社区讨论**: 评论者普遍认为心理健康至关重要，神经多样性个体需要个性化的管理策略，而不是试图“摆脱它”。一些人强调工作应与个人性格和优势相匹配。

**标签**: `#mental health`, `#software engineering`, `#neurodivergence`, `#communication`, `#self-management`

---

<a id="item-15"></a>
## [Dependabot 默认对版本更新实施三天冷却期](https://simonwillison.net/2026/Jul/14/github-changeling/#atom-everything) ⭐️ 7.0/10

GitHub 的 Dependabot 现在默认在打开版本更新拉取请求前等待三天，无需额外配置。 这减少了不必要的更新噪音，并通过延迟采用可能有恶意软件包来缓解供应链攻击。 冷却期仅适用于版本更新，不适用于安全更新；该功能此前于 2025 年 7 月作为可选功能引入。

rss · Simon Willison · Jul 14, 22:43

**背景**: 依赖冷却期有意延迟新软件包版本的安装，以便有时间识别和移除恶意发布。这种做法在类似 axios 供应链攻击事件后得到了推广。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/">Dependabot version updates introduce default package cooldown</a></li>
<li><a href="https://docs.github.com/en/code-security/reference/supply-chain-security/dependabot-options-reference">Dependabot options reference - GitHub Docs</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/dependency-cooldowns/">The case for dependency cooldowns in a post-axios world | Datadog Security Labs</a></li>

</ul>
</details>

**标签**: `#dependabot`, `#github`, `#dependency-management`, `#security`, `#packaging`

---

<a id="item-16"></a>
## [在 GitHub Actions 中缓存友好地使用 uvx](https://simonwillison.net/2026/Jul/14/uvx-github-actions-cache/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了一种在 GitHub Actions 中使用 uvx 的方法：设置 UV_EXCLUDE_NEWER 为固定日期，并将该日期加入缓存键，从而缓存工具，仅在手动更新日期时才升级。 该模式避免了每次工作流运行时重复从 PyPI 下载，显著加快了使用 uvx 运行 linter 或 formatter 等工具的 Python 项目的 CI 速度。 环境变量 UV_EXCLUDE_NEWER 设置为类似 "2026-07-12" 的日期，缓存键包含该日期；要升级工具，用户只需更新日期。文章还链接了一个 issue，要求 astral-sh/setup-uv 默认缓存 wheel。

rss · Simon Willison · Jul 14, 00:56

**背景**: uvx 是 Astral 推出的工具，可在临时隔离环境中运行 Python CLI 工具。默认情况下，每次调用都可能从 PyPI 下载工具及其依赖，这在 CI 中很慢。GitHub Actions 缓存可以存储这些下载，但缓存键需要精心设计以避免工具过时。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/concepts/tools/">Tools | uv</a></li>
<li><a href="https://docs.astral.sh/uv/reference/environment/">Environment variables | uv - Astral Docs</a></li>

</ul>
</details>

**社区讨论**: 文章链接了 astral-sh/setup-uv 仓库中的一个现有 issue，要求将默认行为改为缓存而非从 PyPI 清除 wheel，表明社区对更好的缓存默认值感兴趣。

**标签**: `#GitHub Actions`, `#Python`, `#CI/CD`, `#uv`, `#caching`

---

<a id="item-17"></a>
## [包括 Apple 智能在内的 7 款手机端侧 AI 模型获中国备案](https://mp.weixin.qq.com/s/5MTWh4pWVAlL71RQbU-Udg) ⭐️ 7.0/10

2026 年 7 月 15 日，中国网信办宣布，包括 Apple 智能、华为小艺、OPPO AndesGPT、vivo 蓝心智能大模型、小米澎湃 AI、三星 Galaxy AI 和中兴模型在内的七款手机端侧语言模型已完成政府备案，可在智能手机上部署。 这标志着将先进 AI 集成到中国主流智能手机的重大监管里程碑，确保了符合当地法律，并为广泛面向消费者铺平了道路。这也表明苹果等全球科技巨头正在调整其 AI 产品以满足中国严格的内容和数据治理要求。 备案涵盖专门用于设备端推理的模型，应用场景仅限于手机。值得注意的是，阿里巴巴的千问将作为 Apple 智能在中国区的底层 AI 能力，为 iOS、iPadOS、macOS 和 visionOS 设备提供文本与图像理解、内容生成和多轮对话服务。

telegram · zaihuapd · Jul 15, 08:06

**背景**: 中国 2023 年《生成式人工智能服务管理暂行办法》要求向公众提供生成式 AI 的公司向网信部门备案。备案流程包括提交模型细节、安全评估和数据管理实践。这七款模型的获批表明它们已通过监管审查，现在可以在消费设备上部署。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2026-07/15/c_1785861480767004.htm">关于发布7款提供手机端侧生成式人工智能服务已备案信息的公告关于发布...</a></li>
<li><a href="https://www.sohu.com/a/1050785859_546984">国行Apple智能过审！阿里千问接入iPhone，7款手机端侧大模型备案出炉...</a></li>
<li><a href="https://news.qq.com/rain/a/20260715A08MGP00">苹果AI入华有戏了？工信部发布7款手机端侧大模型备案信息：Apple智能...</a></li>

</ul>
</details>

**标签**: `#AI`, `#mobile`, `#regulation`, `#China`, `#LLM`

---

<a id="item-18"></a>
## [中国零售业边界模糊：山姆、零食店、拼多多争夺同一钱包](https://mp.weixin.qq.com/s/dAHAVxglD-F1RovjcvqCRw) ⭐️ 7.0/10

基于 257 份访谈和 5224 份问卷的调研显示，中国零售业已进入融合时代，山姆会员店、零食折扣店、即时零售和拼多多正在争夺同一笔家庭开支。研究发现，48%的受访者计划控制消费，信任已超越价格成为首要竞争因素。 这一转变标志着中国零售业垂直分类时代的终结，迫使零售商在信任和便利性上竞争，而不仅仅是价格。这对商业战略具有深远影响，企业必须适应消费者优先考虑可靠性和距离而非折扣的新格局。 山姆会员店今年在华收入有望达 1800 至 2000 亿元；零食店头部品牌门店近 4 万家；拼多多旗下多多买菜年销售额约 3000 亿元，年内有望冲击 4000 亿元。调研还发现，对于食品等入口商品，过低价格反而引发安全疑虑，信任成为第一竞争力。

telegram · zaihuapd · Jul 15, 09:01

**背景**: 中国零售业传统上分为超市、便利店、电商平台等不同类别。但近期趋势显示，这些边界正在消融，消费者跨渠道追求便利和信任。即时零售（分钟级配送）和零食折扣店（低价散装零食）快速增长，而拼多多等平台利用社交电商和团购模式抢占家庭开支。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chinairn.com/scfx/20260715/153343594.shtml">2026年零食折扣店行业深度分析：市场规模、竞争格局、渠道红利与头部品牌梳理_中研普华_中研网</a></li>
<li><a href="https://m.ikanchai.com/article/125970">一文读懂 即 时 零 售 ：本地供给、 即 时 需求、 即 时 配送成核心三要素</a></li>
<li><a href="https://www.36kr.com/p/2937876087152007">多多买菜战略大拆解 - 36氪</a></li>

</ul>
</details>

**标签**: `#retail`, `#China`, `#consumer behavior`, `#e-commerce`, `#business strategy`

---

<a id="item-19"></a>
## [法官质疑 Epic 与谷歌反垄断和解背后 800 万美元合作](https://t.me/zaihuapd/42588) ⭐️ 7.0/10

美国地区法官 James Donato 在听证会上披露，Epic Games 与谷歌已达成新的商业合作，涵盖联合产品开发、营销及合作伙伴关系，Epic 将在 6 年内向谷歌支付约 8 亿美元。 这一合作可能削弱 Epic 推动 Android 生态改革的立场，法官质疑该协议是否损害了 Epic 的反垄断立场。此案对应用商店竞争和 Android 开发者费用具有重大影响。 该合作涉及 Unreal Engine、《堡垒之夜》及 Android 相关业务。Epic CEO Tim Sweeney 表示，协议未包含放弃 Epic 反垄断索赔的承诺。

telegram · zaihuapd · Jul 15, 11:15

**背景**: Epic Games 于 2020 年起诉谷歌，指控其 Google Play 商店存在反竞争行为。2024 年，陪审团认定谷歌垄断。双方于 2025-2026 年达成和解，谷歌同意降低 Epic 的 Play 商店佣金并允许替代应用商店。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/03/04/google-settles-with-epic-games-drops-its-play-store-commissions-to-20/">Google settles with Epic Games, drops its Play Store ...</a></li>
<li><a href="https://www.adwaitx.com/google-epic-800m-android-unreal-deal/">Google & Epic Strike $800M Deal: Secret Android Partnership</a></li>

</ul>
</details>

**标签**: `#antitrust`, `#Epic Games`, `#Google`, `#Android`, `#legal`

---

<a id="item-20"></a>
## [ASML 计划提高 EUV 和 DUV 光刻设备价格](https://news.bloomberglaw.com/artificial-intelligence/asml-plans-price-increases-on-chipmaking-equipment-information) ⭐️ 7.0/10

ASML 宣布计划提高其芯片制造设备的价格，包括对中国部分客户将 DUV 系统价格上调 10%，这些客户已接受该涨幅；而与台积电就 EUV 设备涨价的谈判则遭到抵制。 作为先进光刻设备的主导供应商，ASML 的定价权直接影响全球半导体供应链和芯片成本，尤其是先进制程节点。台积电与中国企业的不同反应凸显了地缘政治紧张局势和市场动态。 ASML 首席财务官 Roger Dassen 表示，当前环境赋予公司更好的定价权，先进 EUV 光刻机的产能几乎已预订至 2027 年底。涨价涉及 EUV 和 DUV 系统，其中对中国部分客户 DUV 涨价 10%。

telegram · zaihuapd · Jul 15, 16:49

**背景**: ASML 是全球唯一的极紫外（EUV）光刻系统供应商，这些系统对于制造 5nm 和 3nm 等最先进制程的半导体芯片至关重要。深紫外（DUV）光刻则用于非关键层和较老制程。由于其垄断地位和芯片制造设备的战略重要性，ASML 的定价决策备受关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASML">ASML</a></li>
<li><a href="https://en.wikipedia.org/wiki/Photolithography">Photolithography - Wikipedia</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#ASML`, `#lithography`, `#chipmaking`, `#geopolitics`

---