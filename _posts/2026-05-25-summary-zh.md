---
layout: default
title: "Horizon Summary: 2026-05-25 (ZH)"
date: 2026-05-25
lang: zh
---

> From 35 items, 15 important content pieces were selected

---

1. [微软开源已知最早的 DOS 源代码](#item-1) ⭐️ 9.0/10
2. [APKPure 上的 Telegram 官方版被植入间谍后门](#item-2) ⭐️ 9.0/10
3. [内存成本已占 AI 芯片近三分之二](#item-3) ⭐️ 8.0/10
4. [约束衰减：LLM 智能体在后端编码约束下失败](#item-4) ⭐️ 8.0/10
5. [AMD 取消 Vivado 免费版 Linux 支持](#item-5) ⭐️ 8.0/10
6. [Armin Ronacher 批评 AI 生成的错误报告](#item-6) ⭐️ 8.0/10
7. [微软内部推广 Claude Code，面向非技术人员](#item-7) ⭐️ 8.0/10
8. [微软披露 OpenAI 单季度亏损 115 亿美元](#item-8) ⭐️ 8.0/10
9. [海盗船采用长鑫存储芯片，DDR5 价格或下调](#item-9) ⭐️ 8.0/10
10. [我国日均词元调用量两年增超千倍](#item-10) ⭐️ 8.0/10
11. [神舟二十三号乘组公布：首位港籍航天员，5 月 24 日发射](#item-11) ⭐️ 8.0/10
12. [DeepSeek Reasonix：原生编码代理，高缓存低成本](#item-12) ⭐️ 7.0/10
13. [骗子滥用微软内部账户发送垃圾邮件](#item-13) ⭐️ 7.0/10
14. [Usborne 80 年代计算机书籍引发怀旧热潮](#item-14) ⭐️ 7.0/10
15. [中国证监会拟对富途罚款 18.5 亿元，老虎证券罚没 4.11 亿元](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [微软开源已知最早的 DOS 源代码](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 9.0/10

微软开源了已知最早的 DOS 源代码，这些代码是通过 OCR 技术从纸质打印件中恢复的。代码由 Yufeng Gao 和 Rich Cini 领导的 DOS 反汇编小组转录。 此次发布让人们得以罕见地一窥个人计算的起源以及微软操作系统的早期开发历程。它也凸显了数字保存的重要性以及从物理介质中恢复历史软件所面临的挑战。 源代码是从 DOS 原作者 Tim Paterson 提供的纸质打印件中恢复的。现代 OCR 软件难以处理数十年历史打印件的质量，使得转录过程非常艰辛。

hackernews · DamnInteresting · May 24, 01:21 · [社区讨论](https://news.ycombinator.com/item?id=48253386)

**背景**: DOS（磁盘操作系统）是早期 IBM PC 及其兼容机的基础操作系统。微软从西雅图计算机产品公司收购了 DOS，并授权给 IBM，这成为 MS-DOS 的基础。该源代码此前未以数字形式保存，仅存于纸质打印件中。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Optical_character_recognition">Optical character recognition - Wikipedia</a></li>
<li><a href="https://www.codegenes.net/blog/need-good-ocr-for-printed-source-code-listing-any-ideas/">Best OCR for Printed Source Code Listings: Top Tools to Avoid Manual Typing & Fix Errors — codegenes.net</a></li>

</ul>
</details>

**社区讨论**: 评论者对微软的发布表示感谢，一些人指出同时开源的 BASIC 源代码也具有历史意义。其他人惊叹于几千行汇编代码就能创办一家成功的软件公司，并推测未来是否会发布早期 Windows 的源代码。

**标签**: `#open source`, `#DOS`, `#history`, `#Microsoft`, `#preservation`

---

<a id="item-2"></a>
## [APKPure 上的 Telegram 官方版被植入间谍后门](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

通过 APKPure 分发的 Telegram 官方应用（版本 12.6.5）被重新打包，植入了名为 DataCollector 的间谍框架，可窃取聊天记录、通讯录、照片、文档、GPS 定位和 SIM 卡信息。 此次供应链攻击危及一款广泛使用的通讯应用，可能暴露数百万从 APKPure 下载 Telegram 用户的敏感数据，并凸显了第三方应用商店的风险。 恶意代码位于 classes3.dex（超过 3000 行），使用 AES-GCM 加密将数据外泄至 C2 服务器 38.190.225.166；该间谍软件可访问全部聊天记录、通讯录、照片、文档、GPS 和 SIM 卡信息。

telegram · zaihuapd · May 24, 11:38

**背景**: APKPure 是一个流行的第三方 Android 应用商店。供应链攻击是指在分发过程中篡改合法应用。Telegram 是一款拥有数亿用户的加密通讯应用。AES-GCM 是一种提供机密性和认证的强加密模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://securityaffairs.com/116635/cyber-crime/apkpure-client-malware.html">Hackers compromised APKPure client to distribute infected Apps</a></li>
<li><a href="https://www.secureblink.com/cyber-security-news/supply-chain-attack-infiltrates-android-apps-with-malicious-spin-ok-sdk">Supply Chain Attack Infiltrates Android Apps with Malicious SpinOK SDK</a></li>

</ul>
</details>

**社区讨论**: 社区讨论（通过 Telegram 群组）确认了该事件并表示担忧；建议用户验证应用签名并避免使用第三方商店。

**标签**: `#security`, `#malware`, `#telegram`, `#supply chain attack`, `#spyware`

---

<a id="item-3"></a>
## [内存成本已占 AI 芯片近三分之二](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

根据 Epoch AI 的数据，内存现在占 AI 芯片组件成本的近三分之二（63%），而前几年约为 13-14%，这主要是由 AI 数据中心对 HBM 的激增需求推动的。 这种成本结构表明，一旦 DRAM 供应赶上需求，AI 硬件成本可能大幅下降（硬件可能降低 3 倍，总成本降低 2 倍），且无需任何技术创新。这也解释了 NVIDIA H100/H200 等 AI GPU 的高昂价格。 AI 芯片的总组件支出从 2024 年的约 220 亿美元增长到 2025 年的 520 亿美元，仅 HBM 支出就占很大一部分。该分析聚焦于 AI 加速器的物料清单，不包括封装或研发等其他成本。

hackernews · intelkishan · May 24, 16:31 · [社区讨论](https://news.ycombinator.com/item?id=48258684)

**背景**: AI 芯片（如 GPU 和定制加速器）严重依赖高带宽内存（HBM）来向计算核心提供数据。AI 热潮导致了 DRAM 短缺，将供应从消费市场转移出去，并推高了 PC 和游戏内存的价格。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://epoch.ai/data-insights/ai-chip-component-cost-shares">AI Chip Component Costs: Memory at 63% | Epoch AI | Epoch AI</a></li>
<li><a href="https://spectrum.ieee.org/dram-shortage">AI Boom Fuels DRAM Shortage and Price Surge - IEEE Spectrum</a></li>
<li><a href="https://intuitionlabs.ai/articles/ram-shortage-2025-ai-demand">RAM Shortage 2025: How AI Demand is Raising DRAM Prices</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，仅通过等待 DRAM 供应正常化，无需创新即可实现 3 倍的硬件成本降低。一些人感叹消费者面临的高内存价格（例如，96GB DDR5 现在售价 1200 美元，而几年前为 250 美元），并对 DRAM 容量每年仅增长 20-25%、不足以满足 AI 需求表示沮丧。

**标签**: `#AI hardware`, `#memory costs`, `#DRAM`, `#GPU pricing`, `#semiconductor industry`

---

<a id="item-4"></a>
## [约束衰减：LLM 智能体在后端编码约束下失败](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

一项新研究系统评估了 LLM 编码智能体在多文件后端生成任务中的表现，揭示了“约束衰减”现象——当智能体必须遵循特定架构规则、ORM 约定和框架约束时，性能急剧下降。 这一发现挑战了 LLM 智能体在生产级后端开发中的可靠性，因为遵守结构约束至关重要，并表明当前智能体仅适用于快速原型设计，而不适用于构建健壮、可维护的系统。 该研究使用了跨越八个 Web 框架的 80 个绿地生成任务和 20 个功能实现任务，通过端到端行为测试和静态验证器进行双重评估。随着约束累积，断言通过率下降约 30 个百分点。

hackernews · wek · May 24, 12:55 · [社区讨论](https://news.ycombinator.com/item?id=48256912)

**背景**: LLM 编码智能体是基于自然语言提示生成代码的 AI 系统。后端代码生成不仅需要功能正确性，还需要遵循架构模式、API 契约和框架特定约定。先前的基准测试通常关注无约束或单文件任务，忽略了真实项目中多个约束的复合效应。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay: The Fragility of LLM Agents in Backend Code Generation</a></li>
<li><a href="https://www.alphaxiv.org/overview/2605.06445v1">Constraint Decay : The Fragility of LLM Agents in Backend... | alphaXiv</a></li>
<li><a href="https://agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - AgentPatterns.ai</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认同这些发现，一些人分享了个人经验，注意到在添加约束时出现类似的性能下降。一位评论者指出，由于成本原因，该研究未充分测试前沿模型，这可能会影响具体的性能数据。另一位建议，逐步而非一次性加入约束可能有助于缓解该问题。

**标签**: `#LLM`, `#code generation`, `#AI reliability`, `#software engineering`, `#research`

---

<a id="item-5"></a>
## [AMD 取消 Vivado 免费版 Linux 支持](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD 的 Vivado 2026.1 将从免费（Basic）版本中移除 Linux 支持，而 Windows 支持保持不变。这一变化引发了 FPGA 开发者社区的强烈反对。 Linux 是 FPGA 开发的主要操作系统，取消免费版的 Linux 支持会疏远学生、爱好者和开源开发者，可能削弱 AMD 赖以发展的生态系统。竞争对手如 Lattice 为所有基础芯片提供免费工具，使 AMD 处于劣势。 免费的 Vivado Standard Edition 此前同时支持 Linux 和 Windows；此变更仅适用于 Basic 版本，不涉及付费的 Enterprise 版本。社区评论显示用户对许可麻烦感到沮丧，并认为 AMD 优先考虑盈利而非用户需求。

hackernews · zdw · May 24, 04:14 · [社区讨论](https://news.ycombinator.com/item?id=48254309)

**背景**: Vivado 是 AMD 的 FPGA 设计套件，用于综合和分析 HDL 设计。免费版允许爱好者和学生免费使用 AMD FPGA。Linux 因其灵活性和工具链兼容性成为 FPGA 开发的主流平台。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado/vivado-buy.html">AMD Vivado ™ Design Suite: Standard & Enterprise Edition</a></li>
<li><a href="https://techtrendtrove.com/science-technology/why-is-vivado-2026-1-dropping-linux-support-for-free-tier/">Why is Vivado 2026.1 dropping Linux support for free tier ?</a></li>

</ul>
</details>

**社区讨论**: 社区情绪普遍负面。用户认为取消 Linux 支持损害了生态系统，并将用户推向 Lattice 等竞争对手。一些长期 AMD 用户表示失望，指出 AMD 收购后公司更注重盈利而非工程。

**标签**: `#FPGA`, `#AMD`, `#Vivado`, `#Linux`, `#Ecosystem`

---

<a id="item-6"></a>
## [Armin Ronacher 批评 AI 生成的错误报告](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Flask 和 Jinja2 的创建者 Armin Ronacher 批评 AI 生成的错误报告不准确却充满自信，并倡导采用简单三步格式的结构化、人类观察的问题报告。 这很重要，因为 AI 生成的错误报告降低了开源问题跟踪器的质量，用误导性信息浪费维护者的时间。Ronacher 呼吁简洁、人类观察的报告，可能提高软件维护的效率。 Ronacher 特别提到像 "clanker" 这样的 AI 工具会改写问题，产生虚假的最小复现和错误的原因猜测。他提出了三步报告格式：运行的命令、预期行为、实际行为，加上确切的错误或日志。

rss · Simon Willison · May 24, 18:46

**背景**: 开源项目依赖高质量的错误报告来高效地识别和修复问题。AI 语言模型越来越多地被用于生成或润色问题报告，但它们常常引入幻觉和听起来自信的不准确信息。“最小可复现示例”（MRE）是调试中的最佳实践，但 AI 生成的示例可能是虚假的最小化，省略了关键上下文。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clanker">Clanker - Wikipedia</a></li>
<li><a href="https://practicaldev-herokuapp-com.global.ssl.fastly.net/moozzyk/why-should-you-care-about-minimal-reproducible-examples-and-how-to-create-one-1obb">Why Should You Care About Minimal Reproducible Examples...</a></li>

</ul>
</details>

**标签**: `#open-source`, `#bug reports`, `#AI`, `#software maintenance`, `#Python`

---

<a id="item-7"></a>
## [微软内部推广 Claude Code，面向非技术人员](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

微软正在其核心工程团队中广泛部署 Anthropic 的 Claude Code，包括 CoreAI 团队以及负责 Windows、Microsoft 365 和 Outlook 的体验与设备部门。工程师现在需要同时使用 Claude Code 和 GitHub Copilot 并提供对比反馈，同时鼓励非技术员工使用 Claude Code 进行原型设计。 此举标志着企业 AI 辅助开发的重大转变——作为 OpenAI 的主要投资者和 GitHub Copilot 的推广者，微软现在开始采用 Anthropic 的竞争性工具。这可能加速代理式编码工具在专业开发者之外的普及，降低非技术人员参与软件创建的门槛。 Claude Code 是一种代理式编码工具，能够读取代码库、编辑文件、运行命令，并通过终端、IDE、桌面应用和浏览器与开发工具集成。微软的内部要求规定工程师需提供 Claude Code 与 GitHub Copilot 的对比反馈，表明对两种工具的战略性评估。

telegram · zaihuapd · May 23, 06:05

**背景**: Claude Code 是 Anthropic 开发的 AI 编程助手，基于 Claude 系列大语言模型，采用宪法 AI 训练以提高伦理合规性。GitHub Copilot 由 GitHub 和 OpenAI 开发，是一款广泛使用的代码补全工具，集成于主流 IDE 中。微软作为 OpenAI 的主要投资者，历来推广 Copilot，但现在开始测试 Anthropic 的替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**标签**: `#AI-assisted development`, `#Microsoft`, `#Claude Code`, `#GitHub Copilot`, `#enterprise AI`

---

<a id="item-8"></a>
## [微软披露 OpenAI 单季度亏损 115 亿美元](https://t.me/zaihuapd/41537) ⭐️ 8.0/10

微软最新财报显示，其对 OpenAI 的权益法投资导致单季度净利润减少 31 亿美元，这意味着 OpenAI 在该季度净亏损约 115 亿美元。 这一巨额亏损凸显了开发前沿 AI 的巨大成本，引发了对 AI 商业模式长期可持续性以及微软等主要投资者财务风险的质疑。 根据微软持有 OpenAI 约 27%的股权计算，该季度净亏损约 115 亿美元；若按税前损失和实际持股比例 32.5%计算，亏损可能超过 120 亿美元。这一亏损规模是 OpenAI 2025 年上半年 43 亿美元营收的近三倍。

telegram · zaihuapd · May 23, 07:40

**背景**: OpenAI 以营利性公益公司形式运营，并设有非营利基金会，其财务状况通过微软的权益法会计部分披露。权益法要求微软报告其在 OpenAI 利润或亏损中的份额。OpenAI 的亏损主要源于在计算基础设施和人才上的巨额支出，用于训练 GPT-4 等大型语言模型。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI">OpenAI - Wikipedia</a></li>
<li><a href="https://shekhar14.medium.com/openais-h1-2025-4-3b-in-income-13-5b-in-loss-de0a63ce6eb4">OpenAI ’s H1 2025: $4.3B in income, $13.5B in loss | Medium</a></li>
<li><a href="https://fortune.com/2025/11/12/openai-cash-burn-rate-annual-losses-2028-profitable-2030-financial-documents/">OpenAI says it plans to report stunning annual losses ... | Fortune</a></li>

</ul>
</details>

**标签**: `#OpenAI`, `#Microsoft`, `#AI Economics`, `#Financial Disclosure`

---

<a id="item-9"></a>
## [海盗船采用长鑫存储芯片，DDR5 价格或下调](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

美商海盗船（Corsair）已开始在其 DDR5 内存模组中使用中国长鑫存储（CXMT）的 DRAM 芯片，标称速率 6000 MT/s 的产品已上市。 这一转变使 DRAM 供应链不再依赖三大巨头（三星、SK 海力士、美光），由于 AI 对 HBM 的需求挤压消费级内存供应，此举有望降低 DDR5 价格。 采用长鑫芯片的 DDR5 内存条为 16GB 容量、6000 MT/s 速率，型号为 CMK5X16G3E60C36A2-CN，性能与国际主流产品一致。

telegram · zaihuapd · May 23, 11:17

**背景**: DRAM（动态随机存取存储器）是电脑和服务器中使用的一种内存。全球 DRAM 市场由三星、SK 海力士和美光主导。近期，这些公司已将产能转向 AI 所需的高带宽内存（HBM），导致消费级 DDR5 供应短缺。长鑫存储（CXMT）是一家成立于 2016 年的中国 DRAM 制造商，正试图填补这一空缺。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1563308.htm">国产 存 储 加速“出海” 海盗船DDR5内 存 首现 长 鑫 DRAM ... - cnBeta.COM</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>

</ul>
</details>

**标签**: `#DRAM`, `#memory`, `#supply chain`, `#Corsair`, `#CXMT`

---

<a id="item-10"></a>
## [我国日均词元调用量两年增超千倍](https://t.me/zaihuapd/41542) ⭐️ 8.0/10

国家数据局披露，我国日均词元（Token）调用量在 2025 年 3 月突破 140 万亿，而 2024 年初仅为 1000 亿，两年增长超千倍。 这一爆发式增长标志着中国人工智能商业化的快速推进，以及围绕词元的价值体系正在形成数据市场，将对 AI 企业、数据提供方和整个数字经济产生深远影响。 词元是大模型处理信息的最小单元，具有可计量、可定价、可交易的特征。国家数据局是中国国家发展和改革委员会管理的机构，负责数据治理。

telegram · zaihuapd · May 23, 14:36

**背景**: 词元是 AI 语言模型中的基本单元，代表文本片段（如单词或子词）。国家数据局于 2023 年成立，负责协调数据治理并推动中国数据要素市场发展。词元调用量的激增既反映了 AI 应用的普及，也体现了政府对数据市场化的推动。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>
<li><a href="https://en.wikipedia.org/wiki/National_Data_Administration">National Data Administration - Wikipedia</a></li>

</ul>
</details>

**标签**: `#AI`, `#China`, `#Token Economy`, `#Data Market`, `#Government Data`

---

<a id="item-11"></a>
## [神舟二十三号乘组公布：首位港籍航天员，5 月 24 日发射](https://t.me/zaihuapd/41554) ⭐️ 8.0/10

中国公布了神舟二十三号乘组，由指令长朱杨柱、航天驾驶员张志远和载荷专家黎家盈组成，计划于 5 月 24 日 23 时 08 分发射。黎家盈是首位港籍航天员，也是首位来自香港的女性载荷专家。 此次任务创造了多项历史：首个由第三批和第四批航天员组成的乘组、首位港籍航天员以及首位来自香港的女性载荷专家。这凸显了中国航天事业的扩展以及将香港纳入国家航天事业的承诺。 指令长朱杨柱曾执行神舟十六号任务，成为首位担任指令长的航天飞行工程师。乘组中有一名航天员将执行一年期飞行任务。乘组于 5 月 23 日在酒泉卫星发射中心与中外媒体见面。

telegram · zaihuapd · May 24, 15:13

**背景**: 中国航天员分为三类：航天驾驶员、航天飞行工程师和载荷专家。载荷专家负责科学实验，通常是科学家或工程师。第四批航天员于 2024 年选拔，首次包括来自香港和澳门的候选人。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://wap.eastmoney.com/a/202605243747407098.html">神舟二十三号 航 天 员乘组5月24日出征太空 在轨期间将新开展100...</a></li>
<li><a href="https://news.qq.com/rain/a/20260523A0A4PZ00">首位来自香港的 航 天 员 ，为何是她？_ 腾讯新闻</a></li>
<li><a href="https://www.ithome.com/0/954/539.htm">发射任务准备进展顺利，神舟二十三乘组 航 天 员身心状态良好 - IT之家</a></li>

</ul>
</details>

**标签**: `#space exploration`, `#China space program`, `#astronaut selection`, `#Shenzhou-23`, `#Hong Kong`

---

<a id="item-12"></a>
## [DeepSeek Reasonix：原生编码代理，高缓存低成本](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek Reasonix 是一个基于终端的 AI 编码代理，专门为 DeepSeek 的 API 设计，利用前缀缓存大幅降低 token 成本。它于 2026 年 5 月在 GitHub 上发布，并在 Hacker News 上引发了讨论。 该工具通过专用编码代理让开发者能够利用 DeepSeek 的高效缓存，从而降低 AI 辅助编程的门槛。它凸显了通过缓存优化 AI API 使用以降低成本的趋势。 Reasonix 采用缓存优先循环和闪存优先成本控制，并为代理查询构建嵌入索引。它支持本地 Ollama 或 DeepSeek 托管的嵌入，并具有自动检查点功能。

hackernews · Alifatisk · May 24, 13:02 · [社区讨论](https://news.ycombinator.com/item?id=48256953)

**背景**: DeepSeek 的 API 提供自动前缀缓存，重复的提示前缀会被缓存到磁盘，缓存命中的 token 可享受折扣（通常约 50% 优惠）。这降低了具有重复上下文的长时间会话的成本。Reasonix 通过保持稳定的前缀来最大化缓存命中率。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://api-docs.deepseek.com/guides/kv_cache">Context Caching | DeepSeek API Docs</a></li>

</ul>
</details>

**社区讨论**: Hacker News 的评论者反应不一：一些人赞赏缓存优势，而另一些人则批评网站的 UX（例如动画打字导致布局偏移），并质疑专用代理的必要性。一位用户指出，现有工具如 Codex 已经受益于 DeepSeek 的缓存，无需特殊代理。

**标签**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#cost efficiency`, `#developer tools`

---

<a id="item-13"></a>
## [骗子滥用微软内部账户发送垃圾邮件](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 7.0/10

数月来，骗子一直在滥用一个通常用于发送合法账户警报的微软内部电子邮件账户，发送垃圾邮件和钓鱼链接。具体的滥用方式尚不清楚。 此事件凸显了微软电子邮件基础设施和域名管理中的重大安全漏洞，削弱了用户对微软官方通信的信任。同时，它也展示了域名混淆如何被用于钓鱼攻击，影响数百万用户。 被滥用的账户是用于发送合法警报的微软内部地址，但骗子找到了通过它发送垃圾邮件的方法。由于缺乏微软拥有的域名的完整列表，用户难以区分合法邮件和钓鱼尝试。

hackernews · spike021 · May 24, 00:51 · [社区讨论](https://news.ycombinator.com/item?id=48253186)

**背景**: 钓鱼攻击通常利用域名混淆，攻击者使用与合法域名相似的域名。微软拥有许多域名，例如 microsoftonline.com，这可能会让用户感到困惑。该公司因其安全实践（包括 Microsoft Authenticator 和登录历史可见性问题）而受到批评。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/">Scammers are abusing an internal Microsoft account ... | TechCrunch</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lodGJPWkVSR0hSdDdvSDhVSVJDZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - Microsoft email scam emails - Overview</a></li>

</ul>
</details>

**社区讨论**: 评论者对微软的域名泛滥和安全实践表示不满，指出即使是内部员工也可能不知道所有拥有的域名。一些人分享了利用类似域名混淆的钓鱼尝试的个人经历，而另一些人建议使用像 internal.microsoft.com 这样的子域名来减少混淆。

**标签**: `#security`, `#phishing`, `#Microsoft`, `#spam`, `#domain confusion`

---

<a id="item-14"></a>
## [Usborne 80 年代计算机书籍引发怀旧热潮](https://usborne.com/us/books/computer-and-coding-books) ⭐️ 7.0/10

一批 20 世纪 80 年代的 Usborne 计算机书籍（包括《练习 BASIC》和《机器码入门》等）在网上重新出现，引发了社区怀旧讨论，人们回忆这些书籍如何激励了早期的编程生涯。 这些书籍在向一代人介绍编程方面发挥了关键作用，在互联网时代之前常常是唯一可获取的资源；它们的重新发现凸显了精心编写的教育材料在软件工程历史中的持久价值。 这些书籍涵盖 BASIC、机器码和机器人等主题，从 20 世纪 80 年代末到 21 世纪初被读者使用，通常是从图书馆借阅或传承而来。社区成员回忆将程序移植到 QBasic 以及按照说明搭建机器人的经历。

hackernews · ngram · May 24, 15:43 · [社区讨论](https://news.ycombinator.com/item?id=48258194)

**背景**: 在 20 世纪 80 年代，ZX Spectrum、Commodore 64 和 Amstrad CPC 等家用电脑很常见，但学习资源稀缺。Usborne 出版了一系列色彩丰富、通俗易懂的书籍，通过动手项目教授编程概念，通常使用 BASIC 语言。这些书籍成为许多未来软件工程师的入门途径，尤其是在英国。

**社区讨论**: 社区评论 overwhelmingly 积极且怀旧，用户分享个人故事，讲述这些书籍如何开启他们的编程之旅。许多人感谢书中清晰的解释和动手项目，也有人指出在没有互联网的情况下搭建机器人的挑战。讨论反映了对这些基础性文本的共同赞赏。

**标签**: `#retro computing`, `#programming education`, `#BASIC`, `#nostalgia`, `#history`

---

<a id="item-15"></a>
## [中国证监会拟对富途罚款 18.5 亿元，老虎证券罚没 4.11 亿元](https://t.me/zaihuapd/41539) ⭐️ 7.0/10

中国证监会及深圳证监局拟对富途控股罚款约 18.5 亿元，对老虎证券子公司罚没约 4.112 亿元，原因是其未经许可在中国内地开展跨境证券、公募基金销售及期货业务。 这是中国金融科技公司面临的最大监管处罚之一，标志着对跨境证券业务的严厉打击，可能重塑行业合规格局。 富途创始人兼首席执行官李华被个人罚款 125 万元，老虎证券首席执行官巫天华被警告并处以相同个人罚款。这些罚款为初步决定，尚待最终确认。

telegram · zaihuapd · May 23, 10:58

**背景**: 富途控股和老虎证券是总部位于香港的主要在线券商，提供美股、港股及其他全球市场交易服务。中国监管机构一直在收紧跨境证券服务规则，以防止资本外流并确保符合国内牌照要求。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260523/herald/e7eb58bb6994d891f986fd9d06c85b1d.html">中国 证 监会拟对富途 罚 款 18.5亿， 老 虎 证 券 罚 没4.112亿 - 21经济网</a></li>
<li><a href="https://www.guancha.cn/GuanJinRong/2026_05_22_818074.shtml">证 监会拟 罚 款 金额公布：富途被 罚 18.5亿， 老 虎 被 罚 4.112亿</a></li>
<li><a href="https://news.sina.com.cn/c/2026-05-22/doc-inhyuwef7514481.shtml">news.sina.com.cn/c/2026-05-22/doc-inhyuwef7514481.shtml</a></li>

</ul>
</details>

**标签**: `#regulatory`, `#fintech`, `#China`, `#securities`, `#cross-border`

---