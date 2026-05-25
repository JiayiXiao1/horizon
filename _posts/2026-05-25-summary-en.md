---
layout: default
title: "Horizon Summary: 2026-05-25 (EN)"
date: 2026-05-25
lang: en
---

> From 35 items, 15 important content pieces were selected

---

1. [Microsoft open-sources earliest known DOS source code](#item-1) ⭐️ 9.0/10
2. [Telegram Official App on APKPure Backdoored with Spyware](#item-2) ⭐️ 9.0/10
3. [Memory now accounts for nearly two-thirds of AI chip costs](#item-3) ⭐️ 8.0/10
4. [Constraint Decay: LLM Agents Fail Under Backend Coding Constraints](#item-4) ⭐️ 8.0/10
5. [AMD drops Linux support for Vivado free tier](#item-5) ⭐️ 8.0/10
6. [Armin Ronacher Slams AI-Generated Bug Reports](#item-6) ⭐️ 8.0/10
7. [Microsoft pushes Claude Code internally, targets non-technical staff](#item-7) ⭐️ 8.0/10
8. [Microsoft reveals OpenAI's $11.5B quarterly loss](#item-8) ⭐️ 8.0/10
9. [Corsair Adopts CXMT DRAM, DDR5 Prices May Drop](#item-9) ⭐️ 8.0/10
10. [China's Daily Token Calls Surge Over 1000x in Two Years](#item-10) ⭐️ 8.0/10
11. [Shenzhou-23 Crew Announced: First Hong Kong Astronaut, Launch May 24](#item-11) ⭐️ 8.0/10
12. [DeepSeek Reasonix: Native Coding Agent with High Caching](#item-12) ⭐️ 7.0/10
13. [Scammers abuse internal Microsoft account to send spam](#item-13) ⭐️ 7.0/10
14. [Usborne 1980s Computer Books Spark Nostalgia](#item-14) ⭐️ 7.0/10
15. [China Fines Futu $2.5B, Tiger Brokers $560M for Cross-Border Violations](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Microsoft open-sources earliest known DOS source code](https://arstechnica.com/gadgets/2026/04/microsoft-open-sources-the-earliest-dos-source-code-discovered-to-date/) ⭐️ 9.0/10

Microsoft has open-sourced the earliest known version of DOS source code, recovered from paper printouts using OCR technology. The code was transcribed by the DOS Disassembly Group led by Yufeng Gao and Rich Cini. This release provides a rare glimpse into the origins of personal computing and the early development of Microsoft's operating system. It also highlights the importance of digital preservation and the challenges of recovering historical software from physical media. The source code was recovered from paper printouts provided by Tim Paterson, the original author of DOS. Modern OCR software struggled with the quality of the decades-old printouts, making the transcription process painstaking.

hackernews · DamnInteresting · May 24, 01:21 · [Discussion](https://news.ycombinator.com/item?id=48253386)

**Background**: DOS (Disk Operating System) was the foundational operating system for early IBM PCs and compatibles. Microsoft acquired DOS from Seattle Computer Products and licensed it to IBM, which became the basis for MS-DOS. The source code had not been stored digitally and was only available on paper printouts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Optical_character_recognition">Optical character recognition - Wikipedia</a></li>
<li><a href="https://www.codegenes.net/blog/need-good-ocr-for-printed-source-code-listing-any-ideas/">Best OCR for Printed Source Code Listings: Top Tools to Avoid Manual Typing & Fix Errors — codegenes.net</a></li>

</ul>
</details>

**Discussion**: Commenters expressed gratitude to Microsoft for the release, with some noting the historical significance of the accompanying BASIC source code. Others marveled at how a few thousand lines of assembly code launched a successful software company, and speculated about future releases of early Windows source code.

**Tags**: `#open source`, `#DOS`, `#history`, `#Microsoft`, `#preservation`

---

<a id="item-2"></a>
## [Telegram Official App on APKPure Backdoored with Spyware](https://x.com/EricParker/status/2058411298195661221) ⭐️ 9.0/10

The official Telegram app (version 12.6.5) distributed via APKPure was repackaged with a spyware framework called DataCollector, which can steal chat history, contacts, photos, documents, GPS location, and SIM card information. This supply chain attack compromises a widely-used messaging app, potentially exposing sensitive data of millions of users who downloaded Telegram from APKPure, and highlights the risks of third-party app stores. The malicious code resides in classes3.dex (over 3000 lines) and uses AES-GCM encryption to exfiltrate data to C2 server 38.190.225.166; the spyware can access all chat history, contacts, photos, documents, GPS, and SIM info.

telegram · zaihuapd · May 24, 11:38

**Background**: APKPure is a popular third-party Android app store. Supply chain attacks occur when a legitimate app is tampered with during distribution. Telegram is an encrypted messaging app with hundreds of millions of users. AES-GCM is a strong encryption mode that provides both confidentiality and authentication.

<details><summary>References</summary>
<ul>
<li><a href="https://securityaffairs.com/116635/cyber-crime/apkpure-client-malware.html">Hackers compromised APKPure client to distribute infected Apps</a></li>
<li><a href="https://www.secureblink.com/cyber-security-news/supply-chain-attack-infiltrates-android-apps-with-malicious-spin-ok-sdk">Supply Chain Attack Infiltrates Android Apps with Malicious SpinOK SDK</a></li>

</ul>
</details>

**Discussion**: The community discussion (via Telegram group) confirms the incident and expresses concern; users are advised to verify app signatures and avoid third-party stores.

**Tags**: `#security`, `#malware`, `#telegram`, `#supply chain attack`, `#spyware`

---

<a id="item-3"></a>
## [Memory now accounts for nearly two-thirds of AI chip costs](https://epoch.ai/data-insights/ai-chip-component-cost-shares) ⭐️ 8.0/10

According to Epoch AI, memory now accounts for nearly two-thirds (63%) of AI chip component costs, up from roughly 13-14% in previous years, driven by surging demand for HBM in AI data centers. This cost structure suggests that AI hardware costs could drop significantly (potentially 3x for hardware, 2x total) once DRAM supply catches up with demand, without requiring any technical innovation. It also explains the high prices of AI GPUs like NVIDIA's H100/H200. Total component spend on AI chips grew from about $22 billion in 2024 to $52 billion in 2025, with HBM spending alone accounting for a large portion. The analysis focuses on the bill of materials for AI accelerators, not including other costs like packaging or R&D.

hackernews · intelkishan · May 24, 16:31 · [Discussion](https://news.ycombinator.com/item?id=48258684)

**Background**: AI chips like GPUs and custom accelerators rely heavily on high-bandwidth memory (HBM) to feed data to compute cores. The AI boom has caused a DRAM shortage, diverting supply from consumer markets and driving up prices for PC and gaming memory as well.

<details><summary>References</summary>
<ul>
<li><a href="https://epoch.ai/data-insights/ai-chip-component-cost-shares">AI Chip Component Costs: Memory at 63% | Epoch AI | Epoch AI</a></li>
<li><a href="https://spectrum.ieee.org/dram-shortage">AI Boom Fuels DRAM Shortage and Price Surge - IEEE Spectrum</a></li>
<li><a href="https://intuitionlabs.ai/articles/ram-shortage-2025-ai-demand">RAM Shortage 2025: How AI Demand is Raising DRAM Prices</a></li>

</ul>
</details>

**Discussion**: Commenters noted that a 3x hardware cost reduction is possible just by waiting for DRAM supply to normalize, without innovation. Some lamented the high RAM prices for consumers (e.g., 96GB DDR5 now costs $1200 vs $250 a few years ago), and expressed frustration that DRAM capacity grows only 20-25% per year, insufficient to meet AI demand.

**Tags**: `#AI hardware`, `#memory costs`, `#DRAM`, `#GPU pricing`, `#semiconductor industry`

---

<a id="item-4"></a>
## [Constraint Decay: LLM Agents Fail Under Backend Coding Constraints](https://arxiv.org/abs/2605.06445) ⭐️ 8.0/10

A new study systematically evaluates LLM coding agents on multi-file backend generation and reveals 'constraint decay'—a sharp performance drop when agents must follow specific architectural rules, ORM conventions, and framework constraints. This finding challenges the reliability of LLM agents for production backend development, where adherence to structural constraints is critical, and suggests that current agents are only suitable for rapid prototyping, not for building robust, maintainable systems. The study uses 80 greenfield generation tasks and 20 feature-implementation tasks across eight web frameworks, with a dual evaluation using end-to-end behavioral tests and static verifiers. The assertion pass rate drops by about 30 percentage points as constraints accumulate.

hackernews · wek · May 24, 12:55 · [Discussion](https://news.ycombinator.com/item?id=48256912)

**Background**: LLM coding agents are AI systems that generate code based on natural language prompts. Backend code generation requires not only functional correctness but also adherence to architectural patterns, API contracts, and framework-specific conventions. Prior benchmarks often focused on unconstrained or single-file tasks, overlooking the compounding effect of multiple constraints in real-world projects.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2605.06445">[2605.06445] Constraint Decay: The Fragility of LLM Agents in Backend Code Generation</a></li>
<li><a href="https://www.alphaxiv.org/overview/2605.06445v1">Constraint Decay : The Fragility of LLM Agents in Backend... | alphaXiv</a></li>
<li><a href="https://agentpatterns.ai/verification/constraint-decay-backend-agents/">Constraint Decay in Backend Code Generation - AgentPatterns.ai</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree with the findings, with some sharing personal experiences of noticing similar degradation when adding constraints. One commenter noted that the study did not fully test frontier models due to cost, which may affect the specific performance numbers. Another suggested that including constraints incrementally rather than upfront might mitigate the issue.

**Tags**: `#LLM`, `#code generation`, `#AI reliability`, `#software engineering`, `#research`

---

<a id="item-5"></a>
## [AMD drops Linux support for Vivado free tier](https://adaptivesupport.amd.com/s/question/0D5Pd00001YQLdMKAX/why-is-vivado-20261-dropping-linux-support-for-free-tier-?language=en_US) ⭐️ 8.0/10

AMD's Vivado 2026.1 will remove Linux support from its free (Basic) tier, while Windows support remains. This change has sparked backlash from the FPGA developer community. Linux is the primary OS for FPGA development, and removing free-tier Linux support alienates students, hobbyists, and open-source developers, potentially shrinking the ecosystem that AMD relies on for growth. Competitors like Lattice offer free tools for all basic chips, putting AMD at a disadvantage. The free Vivado Standard Edition previously supported both Linux and Windows; the change applies only to the Basic tier, not the paid Enterprise edition. Community comments indicate frustration with licensing hassles and a perception that AMD is prioritizing monetization over user needs.

hackernews · zdw · May 24, 04:14 · [Discussion](https://news.ycombinator.com/item?id=48254309)

**Background**: Vivado is AMD's FPGA design suite, used for synthesizing and analyzing HDL designs. The free tier allows hobbyists and students to work with AMD FPGAs at no cost. Linux is the dominant platform for FPGA development due to its flexibility and toolchain compatibility.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vivado">Vivado - Wikipedia</a></li>
<li><a href="https://www.amd.com/en/products/software/adaptive-socs-and-fpgas/vivado/vivado-buy.html">AMD Vivado ™ Design Suite: Standard & Enterprise Edition</a></li>
<li><a href="https://techtrendtrove.com/science-technology/why-is-vivado-2026-1-dropping-linux-support-for-free-tier/">Why is Vivado 2026.1 dropping Linux support for free tier ?</a></li>

</ul>
</details>

**Discussion**: Community sentiment is overwhelmingly negative. Users argue that removing Linux support harms the ecosystem and drives users to competitors like Lattice. Some long-time AMD users express disappointment, noting that the acquisition by AMD has led to a focus on monetization over engineering.

**Tags**: `#FPGA`, `#AMD`, `#Vivado`, `#Linux`, `#Ecosystem`

---

<a id="item-6"></a>
## [Armin Ronacher Slams AI-Generated Bug Reports](https://simonwillison.net/2026/May/24/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher, creator of Flask and Jinja2, criticized AI-generated bug reports for being inaccurate yet confident, and advocated for structured, human-observed issue reports following a simple three-step format. This matters because AI-generated bug reports degrade the quality of open-source issue trackers, wasting maintainers' time with misleading information. Ronacher's call for concise, human-observed reports could improve efficiency in software maintenance. Ronacher specifically mentioned that AI tools like "clanker" reword issues, producing fake-minimal repros and incorrect root cause guesses. He proposed a three-step report format: command run, expected behavior, actual behavior, plus exact error or log.

rss · Simon Willison · May 24, 18:46

**Background**: Open-source projects rely on high-quality bug reports to identify and fix issues efficiently. AI language models are increasingly used to generate or polish issue reports, but they often introduce hallucinations and confident-sounding inaccuracies. "Minimal reproducible examples" (MREs) are a best practice in debugging, but AI-generated ones can be fake-minimal, omitting crucial context.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Clanker">Clanker - Wikipedia</a></li>
<li><a href="https://practicaldev-herokuapp-com.global.ssl.fastly.net/moozzyk/why-should-you-care-about-minimal-reproducible-examples-and-how-to-create-one-1obb">Why Should You Care About Minimal Reproducible Examples...</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#bug reports`, `#AI`, `#software maintenance`, `#Python`

---

<a id="item-7"></a>
## [Microsoft pushes Claude Code internally, targets non-technical staff](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

Microsoft is widely deploying Anthropic's Claude Code across its major engineering teams, including CoreAI and the Experiences & Devices division responsible for Windows, Microsoft 365, and Outlook. Engineers are now required to use both Claude Code and GitHub Copilot and provide comparative feedback, while non-technical employees are encouraged to use Claude Code for prototyping. This move signals a major shift in enterprise AI-assisted development, as Microsoft—a key investor in OpenAI and promoter of GitHub Copilot—is now embracing a competing tool from Anthropic. It could accelerate the adoption of agentic coding tools beyond professional developers, lowering the barrier for non-technical staff to participate in software creation. Claude Code is an agentic coding tool that reads codebases, edits files, runs commands, and integrates with development tools via terminal, IDE, desktop app, and browser. Microsoft's internal mandate requires engineers to provide comparative feedback on Claude Code versus GitHub Copilot, indicating a strategic evaluation of both tools.

telegram · zaihuapd · May 23, 06:05

**Background**: Claude Code is an AI coding assistant developed by Anthropic, based on the Claude series of large language models trained using constitutional AI for improved ethical compliance. GitHub Copilot, developed by GitHub and OpenAI, is a widely used code completion tool that integrates with popular IDEs. Microsoft, a major investor in OpenAI, has historically promoted Copilot but is now testing Anthropic's alternative.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/overview">Overview - Claude Code Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#Microsoft`, `#Claude Code`, `#GitHub Copilot`, `#enterprise AI`

---

<a id="item-8"></a>
## [Microsoft reveals OpenAI's $11.5B quarterly loss](https://t.me/zaihuapd/41537) ⭐️ 8.0/10

Microsoft's latest earnings report disclosed that its equity method investment in OpenAI resulted in a $3.1 billion reduction in net profit for the quarter, implying OpenAI suffered a net loss of approximately $11.5 billion in a single quarter. This massive loss highlights the enormous costs of developing cutting-edge AI, raising questions about the long-term sustainability of AI business models and the financial risks for major investors like Microsoft. Based on Microsoft's approximately 27% stake in OpenAI, the quarterly net loss is estimated at $11.5 billion; using a pre-tax loss and actual stake of 32.5%, the loss could exceed $12 billion. This loss is nearly three times OpenAI's $4.3 billion revenue in the first half of 2025.

telegram · zaihuapd · May 23, 07:40

**Background**: OpenAI operates as a for-profit public benefit corporation with a nonprofit foundation, and its financials are partially disclosed through Microsoft's equity method accounting. The equity method requires Microsoft to report its share of OpenAI's profits or losses. OpenAI's losses are driven by massive spending on computing infrastructure and talent for training large language models like GPT-4.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI">OpenAI - Wikipedia</a></li>
<li><a href="https://shekhar14.medium.com/openais-h1-2025-4-3b-in-income-13-5b-in-loss-de0a63ce6eb4">OpenAI ’s H1 2025: $4.3B in income, $13.5B in loss | Medium</a></li>
<li><a href="https://fortune.com/2025/11/12/openai-cash-burn-rate-annual-losses-2028-profitable-2030-financial-documents/">OpenAI says it plans to report stunning annual losses ... | Fortune</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Microsoft`, `#AI Economics`, `#Financial Disclosure`

---

<a id="item-9"></a>
## [Corsair Adopts CXMT DRAM, DDR5 Prices May Drop](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

Corsair has started using DRAM chips from Chinese manufacturer ChangXin Memory Technologies (CXMT) in its DDR5 memory modules, with 6000 MT/s kits already available on the market. This shift diversifies the DRAM supply chain away from the three dominant players (Samsung, SK Hynix, Micron), potentially lowering DDR5 prices as AI demand for HBM tightens supply of consumer memory. The CXMT-based DDR5 modules are 16GB sticks rated at 6000 MT/s with model number CMK5X16G3E60C36A2-CN, matching mainstream performance specifications.

telegram · zaihuapd · May 23, 11:17

**Background**: DRAM (Dynamic Random Access Memory) is a type of memory used in computers and servers. The global DRAM market is dominated by Samsung, SK Hynix, and Micron. Recently, these companies have shifted production capacity to High Bandwidth Memory (HBM) for AI applications, causing shortages in consumer DDR5 supply. CXMT is a Chinese DRAM manufacturer founded in 2016, aiming to fill the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1563308.htm">国产 存 储 加速“出海” 海盗船DDR5内 存 首现 长 鑫 DRAM ... - cnBeta.COM</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#memory`, `#supply chain`, `#Corsair`, `#CXMT`

---

<a id="item-10"></a>
## [China's Daily Token Calls Surge Over 1000x in Two Years](https://t.me/zaihuapd/41542) ⭐️ 8.0/10

China's National Data Administration reported that daily token calls exceeded 140 trillion in March 2025, up from 100 billion in early 2024, a more than 1000-fold increase in two years. This explosive growth signals rapid commercialization of AI in China and the formation of a data market around token-based value systems, impacting AI companies, data providers, and the broader digital economy. Tokens are the smallest units of information processed by large language models, and their usage is now being metered, priced, and traded. The National Data Administration is a bureau under China's National Development and Reform Commission overseeing data governance.

telegram · zaihuapd · May 23, 14:36

**Background**: Tokens are fundamental units in AI language models, representing pieces of text (e.g., words or subwords). The National Data Administration was established in 2023 to coordinate data governance and promote the data element market in China. The surge in token calls reflects both increased AI adoption and the government's push for data marketization.

<details><summary>References</summary>
<ul>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>
<li><a href="https://en.wikipedia.org/wiki/National_Data_Administration">National Data Administration - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI`, `#China`, `#Token Economy`, `#Data Market`, `#Government Data`

---

<a id="item-11"></a>
## [Shenzhou-23 Crew Announced: First Hong Kong Astronaut, Launch May 24](https://t.me/zaihuapd/41554) ⭐️ 8.0/10

China announced the Shenzhou-23 crew, consisting of Commander Zhu Yangzhu, Pilot Zhang Zhiyuan, and Payload Specialist Li Jiaying, with launch scheduled for May 24 at 23:08 Beijing time. Li Jiaying is the first Hong Kong astronaut and the first female payload specialist from Hong Kong. This mission marks several historic firsts: the first crew composed of third- and fourth-generation astronauts, the first Hong Kong astronaut, and the first female payload specialist from Hong Kong. It underscores China's expanding space program and its commitment to including Hong Kong in national space efforts. Commander Zhu Yangzhu, a former Shenzhou-16 crew member, becomes the first aerospace flight engineer to serve as commander. One crew member will perform a one-year mission. The crew met the media on May 23 at Jiuquan Satellite Launch Center.

telegram · zaihuapd · May 24, 15:13

**Background**: China's astronaut corps is divided into three types: spacecraft pilots, spaceflight engineers, and payload specialists. Payload specialists are responsible for scientific experiments and are typically scientists or engineers. The fourth batch of astronauts, selected in 2024, includes candidates from Hong Kong and Macau for the first time.

<details><summary>References</summary>
<ul>
<li><a href="https://wap.eastmoney.com/a/202605243747407098.html">神舟二十三号 航 天 员乘组5月24日出征太空 在轨期间将新开展100...</a></li>
<li><a href="https://news.qq.com/rain/a/20260523A0A4PZ00">首位来自香港的 航 天 员 ，为何是她？_ 腾讯新闻</a></li>
<li><a href="https://www.ithome.com/0/954/539.htm">发射任务准备进展顺利，神舟二十三乘组 航 天 员身心状态良好 - IT之家</a></li>

</ul>
</details>

**Tags**: `#space exploration`, `#China space program`, `#astronaut selection`, `#Shenzhou-23`, `#Hong Kong`

---

<a id="item-12"></a>
## [DeepSeek Reasonix: Native Coding Agent with High Caching](https://esengine.github.io/DeepSeek-Reasonix/) ⭐️ 7.0/10

DeepSeek Reasonix is a terminal-based AI coding agent designed specifically for DeepSeek's API, leveraging prefix caching to reduce token costs significantly. It was released on GitHub and discussed on Hacker News in May 2026. This tool makes DeepSeek's cost-efficient caching accessible to developers in a dedicated coding agent, potentially lowering the barrier for AI-assisted coding. It highlights the growing trend of optimizing AI API usage through caching to reduce expenses. Reasonix uses a cache-first loop and flash-first cost control, and it builds an embedding index for agent queries. It supports local Ollama or DeepSeek-hosted embeddings and auto-checkpoints.

hackernews · Alifatisk · May 24, 13:02 · [Discussion](https://news.ycombinator.com/item?id=48256953)

**Background**: DeepSeek's API offers automatic prefix caching, where repeated prompt prefixes are cached on disk, giving discounts on cache-hit tokens (typically ~50% off). This reduces costs for long sessions with repetitive context. Reasonix is engineered to maximize cache hits by maintaining stable prefixes.

<details><summary>References</summary>
<ul>
<li><a href="https://esengine.github.io/DeepSeek-Reasonix/">Reasonix — DeepSeek -native AI coding agent</a></li>
<li><a href="https://api-docs.deepseek.com/quick_start/agent_integrations/reasonix">Integrate with Reasonix | DeepSeek API Docs</a></li>
<li><a href="https://api-docs.deepseek.com/guides/kv_cache">Context Caching | DeepSeek API Docs</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters had mixed reactions: some appreciated the caching benefits, while others criticized the website's UX (e.g., animated typing causing layout shifts) and questioned the need for a dedicated agent. One user noted that existing tools like Codex already benefit from DeepSeek's cache without special agents.

**Tags**: `#AI coding agent`, `#DeepSeek`, `#caching`, `#cost efficiency`, `#developer tools`

---

<a id="item-13"></a>
## [Scammers abuse internal Microsoft account to send spam](https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/) ⭐️ 7.0/10

Scammers have been exploiting an internal Microsoft email account, typically used for legitimate account alerts, to send spam and phishing links for months. The exact method of abuse remains unclear. This incident highlights significant security weaknesses in Microsoft's email infrastructure and domain management, undermining trust in official Microsoft communications. It also demonstrates how domain confusion can be exploited for phishing attacks, affecting millions of users. The abused account is an internal Microsoft address used for sending legitimate alerts, but scammers have found a way to send spam through it. The lack of a comprehensive list of Microsoft-owned domains makes it difficult for users to distinguish legitimate emails from phishing attempts.

hackernews · spike021 · May 24, 00:51 · [Discussion](https://news.ycombinator.com/item?id=48253186)

**Background**: Phishing attacks often rely on domain confusion, where attackers use domains that look similar to legitimate ones. Microsoft owns many domains, such as microsoftonline.com, which can be confusing for users. The company has faced criticism for its security practices, including issues with Microsoft Authenticator and login history visibility.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/05/21/scammers-are-abusing-an-internal-microsoft-account-to-send-spam/">Scammers are abusing an internal Microsoft account ... | TechCrunch</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lodGJPWkVSR0hSdDdvSDhVSVJDZ0FQAQ?hl=en-US&gl=US&ceid=US:en">Google News - Microsoft email scam emails - Overview</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with Microsoft's domain sprawl and security practices, noting that even internal employees may not know all owned domains. Some shared personal experiences with phishing attempts exploiting similar domain confusion, while others suggested using subdomains like internal.microsoft.com to reduce confusion.

**Tags**: `#security`, `#phishing`, `#Microsoft`, `#spam`, `#domain confusion`

---

<a id="item-14"></a>
## [Usborne 1980s Computer Books Spark Nostalgia](https://usborne.com/us/books/computer-and-coding-books) ⭐️ 7.0/10

A collection of 1980s Usborne computer books, including titles like 'Practice Your BASIC' and 'Machine Code for Beginners,' has resurfaced online, prompting a wave of nostalgic community discussion about their role in inspiring early programming careers. These books played a pivotal role in introducing a generation to programming, often serving as the only accessible resource before the internet era, and their rediscovery highlights the enduring value of well-crafted educational materials in software engineering history. The books cover topics like BASIC, machine code, and robotics, and were used by readers from the late 1980s into the early 2000s, often borrowed from libraries or handed down. Community members recall porting programs to QBasic and building robots from the instructions.

hackernews · ngram · May 24, 15:43 · [Discussion](https://news.ycombinator.com/item?id=48258194)

**Background**: In the 1980s, home computers like the ZX Spectrum, Commodore 64, and Amstrad CPC were common, but learning resources were scarce. Usborne published a series of colorful, accessible books that taught programming concepts through hands-on projects, often in BASIC. These books became a gateway for many future software engineers, especially in the UK.

**Discussion**: The community comments are overwhelmingly positive and nostalgic, with users sharing personal stories of how these books launched their coding journeys. Many express gratitude for the clear explanations and hands-on projects, while some note the challenges of building robots without the internet. The discussion reflects a shared appreciation for these foundational texts.

**Tags**: `#retro computing`, `#programming education`, `#BASIC`, `#nostalgia`, `#history`

---

<a id="item-15"></a>
## [China Fines Futu $2.5B, Tiger Brokers $560M for Cross-Border Violations](https://t.me/zaihuapd/41539) ⭐️ 7.0/10

Chinese regulators proposed fines of approximately 18.5 billion yuan against Futu Holdings and 4.112 billion yuan against Tiger Brokers' subsidiaries for conducting unauthorized cross-border securities, public fund sales, and futures businesses in mainland China. This marks one of the largest regulatory penalties against Chinese fintech firms, signaling a crackdown on cross-border securities activities and potentially reshaping the industry's compliance landscape. Futu's founder and CEO Li Hua faces a personal fine of 1.25 million yuan, while Tiger Brokers' CEO Wu Tianhua received a warning and a similar personal fine. The penalties are preliminary and subject to final determination.

telegram · zaihuapd · May 23, 10:58

**Background**: Futu Holdings and Tiger Brokers are major online brokerages based in Hong Kong, offering trading in US, Hong Kong, and other global markets. Chinese regulators have been tightening rules on cross-border securities services to prevent capital outflows and ensure compliance with domestic licensing requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260523/herald/e7eb58bb6994d891f986fd9d06c85b1d.html">中国 证 监会拟对富途 罚 款 18.5亿， 老 虎 证 券 罚 没4.112亿 - 21经济网</a></li>
<li><a href="https://www.guancha.cn/GuanJinRong/2026_05_22_818074.shtml">证 监会拟 罚 款 金额公布：富途被 罚 18.5亿， 老 虎 被 罚 4.112亿</a></li>
<li><a href="https://news.sina.com.cn/c/2026-05-22/doc-inhyuwef7514481.shtml">news.sina.com.cn/c/2026-05-22/doc-inhyuwef7514481.shtml</a></li>

</ul>
</details>

**Tags**: `#regulatory`, `#fintech`, `#China`, `#securities`, `#cross-border`

---