---
layout: default
title: "Horizon Summary: 2026-07-06 (EN)"
date: 2026-07-06
lang: en
---

> From 38 items, 18 important content pieces were selected

---

1. [Digital vs. Physical Games: The Real Issue Is Ownership](#item-1) ⭐️ 8.0/10
2. [sqlite-utils 4.0rc2: AI-Written by Claude Fable for $149](#item-2) ⭐️ 8.0/10
3. [Newer Claude Models Show Tool-Calling Regression](#item-3) ⭐️ 8.0/10
4. [iOS 27 Adds Trust Insights On-Device Anti-Fraud Feature](#item-4) ⭐️ 8.0/10
5. [F-Droid Calls Google ADV Malware on 4 Billion Devices](#item-5) ⭐️ 8.0/10
6. [Hong Kong Handles Over Half of China's Chip Imports](#item-6) ⭐️ 8.0/10
7. [Fudan Exam: Students Design Questions to Stump AI](#item-7) ⭐️ 8.0/10
8. [SpaceX Shows Investors Prototype Smartphone](#item-8) ⭐️ 8.0/10
9. [China Plans to Cut SCI Publication Incentives to Prevent Tech Leaks](#item-9) ⭐️ 8.0/10
10. [Karpathy's nanochat: Build ChatGPT for $100](#item-10) ⭐️ 7.0/10
11. [Starring the Computer: Movie & TV Computer Catalog](#item-11) ⭐️ 7.0/10
12. [Free Online Compiler Textbook Released](#item-12) ⭐️ 7.0/10
13. [World Map in 445 Bytes Using Deflate and Fetch](#item-13) ⭐️ 7.0/10
14. [South Korea Plans 800 Trillion Won Semiconductor Cluster, Aims to Double DRAM Output](#item-14) ⭐️ 7.0/10
15. [Linux tops 2026 CVE charts; maintainer says it's good news](#item-15) ⭐️ 7.0/10
16. [Samsung Plans ~20% DRAM Price Hike in Q3](#item-16) ⭐️ 7.0/10
17. [OpenAI Never Visited Stargate UK Site, Guardian Finds](#item-17) ⭐️ 7.0/10
18. [Chinese Startup Tests CO2 Cold Launch Rocket Technology](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Digital vs. Physical Games: The Real Issue Is Ownership](https://popcar.bearblog.dev/its-about-ownership/) ⭐️ 8.0/10

A blog post argues that the core issue in the digital vs. physical games debate is ownership, not format, and calls for regulations to ensure buyers have transfer and usage rights. This discussion highlights a growing consumer rights concern as digital game sales dominate, and could influence future regulation on digital ownership and DRM practices. The post emphasizes that digital games are often licensed, not sold, and that DRM can revoke access. It suggests regulations should mandate transferability and permanent access.

hackernews · popcar2 · Jul 5, 14:56 · [Discussion](https://news.ycombinator.com/item?id=48794750)

**Background**: Digital rights management (DRM) restricts how users can access and transfer purchased digital content. Many digital game platforms, like Steam, use DRM that ties games to accounts, limiting resale and long-term access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Always-on_DRM">Always-on DRM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Digital_rights_management">Digital rights management - Wikipedia</a></li>
<li><a href="https://d3.harvard.edu/rethinking-digital-ownership-rights-governance-and-the-path-forward/">Rethinking Digital Ownership: Rights, Governance, and the Path Forward | Harvard Business School AI Institute</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree on the need for ownership rights, with some proposing banning the word 'buy' for licensed games. Others note that cracks and piracy currently provide the only real ownership for PC games.

**Tags**: `#digital ownership`, `#gaming`, `#regulation`, `#DRM`, `#consumer rights`

---

<a id="item-2"></a>
## [sqlite-utils 4.0rc2: AI-Written by Claude Fable for $149](https://simonwillison.net/2026/Jul/5/sqlite-utils-fable/#atom-everything) ⭐️ 8.0/10

Simon Willison released sqlite-utils 4.0rc2, with most of the code written by Anthropic's Claude Fable AI model at a cost of approximately $149.25. The AI identified critical bugs, including a data-loss issue in delete_where(), that were fixed before the stable release. This demonstrates a practical, cost-effective use of AI in software development, where an LLM not only wrote code but also performed thorough code review, catching severe bugs. It highlights the potential for AI to assist in maintaining high-quality open-source projects with limited human resources. The development involved 37 prompts, 34 commits, and +1,321/-190 code changes across 30 files. Claude Fable's review identified 5 release-blocker issues, including a transaction bug in delete_where() that could cause silent data loss.

rss · Simon Willison · Jul 5, 01:00

**Background**: sqlite-utils is a Python CLI tool and library for manipulating SQLite databases, created by Simon Willison. Semantic versioning (SemVer) uses a three-part version number (Major.Minor.Patch) to indicate compatibility; breaking changes require a major version bump. Claude Fable is Anthropic's advanced AI model designed for complex coding tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/simonw/sqlite-utils">GitHub - simonw/sqlite-utils: Python CLI utility and library ...</a></li>
<li><a href="https://sqlite-utils.datasette.io/">sqlite-utils</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable">Claude Fable</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#sqlite-utils`, `#Claude Fable`, `#software engineering`, `#open source`

---

<a id="item-3"></a>
## [Newer Claude Models Show Tool-Calling Regression](https://simonwillison.net/2026/Jul/4/better-models-worse-tools/#atom-everything) ⭐️ 8.0/10

Armin Ronacher reports that newer Claude models (Opus 4.8, Sonnet 5) sometimes invent extra fields in tool call schemas, causing Pi's edit tool to reject valid edits, while older models do not exhibit this issue. This counterintuitive regression threatens the reliability of LLM-based coding agents that depend on precise tool call schemas, potentially forcing third-party tools to adapt to model-specific quirks. The invented fields include names like 'type', 'id', 'kind', 'unique', 'matchCase', and nested properties; the edit content itself is usually correct, but the malformed arguments cause rejection. The issue appears in about 20% of edits in some sessions.

rss · Simon Willison · Jul 4, 22:53

**Background**: LLM tool calling allows models to invoke external functions by generating structured JSON matching a predefined schema. Anthropic's Claude models have a built-in text editor tool used by Claude Code, and newer models may have been reinforcement-trained to prefer that tool's schema, causing interference with custom tools like Pi's.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/earendil-works/pi/issues/6278">New Claude models work poorly with the current Pi's edit tool, failing about 20% edits in some sessions · Issue #6278 · earendil-works/pi</a></li>
<li><a href="https://techplanet.today/post/better-models-worse-tools-understanding-the-tool-calling-regression-in-newer-claude-models">Better Models, Worse Tools: Understanding the Tool-Calling Regression in Newer Claude Models | TechPlanet</a></li>
<li><a href="https://simonwillison.net/2026/Jul/4/better-models-worse-tools/">Better Models: Worse Tools</a></li>

</ul>
</details>

**Discussion**: The GitHub issue #6278 on Pi's repository confirms the problem, with users reporting that newer Claude models fail about 20% of edits. Some suggest implementing multiple edit tools to match the model's preferred schema.

**Tags**: `#LLM`, `#tool calling`, `#Anthropic`, `#Claude`, `#reliability`

---

<a id="item-4"></a>
## [iOS 27 Adds Trust Insights On-Device Anti-Fraud Feature](https://www.cultofmac.com/news/ios-27-trust-insights-feature) ⭐️ 8.0/10

Apple announced Trust Insights, a new on-device anti-fraud feature in iOS 27, which analyzes user behavior patterns, timing, context, and sensor data to detect scams in real time. When high or medium risk is identified, apps can display warnings, introduce payment delays, or require extra authentication. This feature represents a privacy-preserving approach to real-time scam detection, as all analysis happens on-device and raw data is immediately deleted. It could significantly reduce financial losses from social engineering scams, especially those involving phone calls directing victims to transfer money. Trust Insights does not read messages, emails, or photo content; it only sends a single output value to the server. Users can disable the feature, but a cooldown period prevents scammers from turning it off during a call.

telegram · zaihuapd · Jul 4, 14:30

**Background**: Traditional anti-fraud systems often rely on server-side analysis of messages or transactions, which can raise privacy concerns. Trust Insights shifts detection to the device, using behavioral signals such as unusual typing speed or screen interactions during a call to identify potential manipulation. This approach aligns with Apple's emphasis on privacy and on-device intelligence.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cultofmac.com/news/ios-27-trust-insights-feature">Trust Insights will help your iPhone identify (and stop) scammers| Cult ...</a></li>
<li><a href="https://techmymoney.com/2026/07/04/ios-27-trust-insights-will-warn-iphone-owners-mid-scam-before-money-moves/">iOS 27 Trust Insights: iPhone Scam Warnings Explained</a></li>
<li><a href="https://applemagazine.com/ios-27-trust-insights/">iOS 27 Trust Insights Helps Apps Detect Scam Coaching</a></li>

</ul>
</details>

**Tags**: `#iOS`, `#anti-fraud`, `#privacy`, `#Apple`, `#mobile security`

---

<a id="item-5"></a>
## [F-Droid Calls Google ADV Malware on 4 Billion Devices](https://f-droid.org/2026/07/01/adv-malware.html) ⭐️ 8.0/10

F-Droid has officially labeled Google's Android Developer Verification (ADV) as malware, warning that it is pre-installed on approximately 4 billion Android devices and will begin blocking unapproved apps in select countries starting September 2026. This development threatens the open nature of the Android ecosystem by giving Google unprecedented control over app installation, potentially restricting user freedom and harming alternative app stores like F-Droid. ADV runs as a system process with root privileges via Play Protect, cannot be removed, and will first activate in Brazil, Indonesia, Singapore, and Thailand on September 30, 2026, with global rollout planned for 2027 and beyond.

telegram · zaihuapd · Jul 5, 00:41

**Background**: Android Developer Verification (ADV) is a Google requirement that apps be registered to an identity-verified developer before they can be installed on certified Android devices. F-Droid is a free and open-source app store that hosts only FOSS apps, and it opposes ADV as a threat to user freedom. Over 70 organizations including EFF, FSF, and ACLU have signed an open letter condemning the program.

<details><summary>References</summary>
<ul>
<li><a href="https://www.lineageos.org/Developer-Verification/">Developer Verification – LineageOS</a></li>
<li><a href="https://cybernews.com/security/f-droid-google-android-verifier-malware/">F-Droid calls Google Android verifier malware | Cybernews</a></li>
<li><a href="https://en.wikipedia.org/wiki/F-Droid">F-Droid</a></li>

</ul>
</details>

**Tags**: `#Android`, `#Malware`, `#Digital Rights`, `#Google`, `#F-Droid`

---

<a id="item-6"></a>
## [Hong Kong Handles Over Half of China's Chip Imports](https://thenextweb.com/news/hong-kong-china-ai-chip-trade-hub) ⭐️ 8.0/10

In the first five months of 2026, Hong Kong processed over half of China's chip imports, with re-exports valued at approximately $124 billion, accounting for 52% of China's total chip procurement. This milestone underscores Hong Kong's emergence as a critical AI trade hub amid geopolitical tensions, reshaping global semiconductor supply chains and highlighting its strategic role in China's technology imports. AI-related electronics now account for 57% to 70% of Hong Kong's exports, prompting the Hong Kong Trade Development Council to raise its 2026 export growth forecast to over 20%.

telegram · zaihuapd · Jul 5, 02:45

**Background**: Hong Kong's free-port status—with no tariffs, no capital controls, and a developed air cargo network—makes it ideal for high-value, low-weight, time-sensitive semiconductor trade. Re-export trade involves goods passing through a third country or region before reaching their final destination, often to circumvent trade barriers.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hk/自由港">自由港 - 維基百科，自由的百科全書</a></li>
<li><a href="https://zh.wikipedia.org/wiki/转口贸易">转口贸易 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.yzaobao.com/news/hkMacao/202607/0475607.html">全球AI热潮推动亚洲增长 香港崛起为中国晶片贸易关键中转站</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#AI trade`, `#Hong Kong`, `#China`, `#geopolitics`

---

<a id="item-7"></a>
## [Fudan Exam: Students Design Questions to Stump AI](https://mp.weixin.qq.com/s/d53O-6mVFZqMa_Sti1yEPw) ⭐️ 8.0/10

Fudan University's 'Data Mining' course replaced traditional exams with a human-vs-AI challenge where 51 students each created 10 calculation problems to test three AI models, scoring higher when the AI answered incorrectly. This innovative assessment reflects a paradigm shift in education, moving from testing algorithmic knowledge to evaluating students' ability to judge and critique AI outputs, which is crucial for AI literacy in the workforce. 50 out of 51 students managed to stump at least one model, but only 4 achieved a zero score on any model's entire test; the strongest model, Claude, was never completely defeated, and the class average was 85.7 out of 100.

telegram · zaihuapd · Jul 5, 08:40

**Background**: Traditional exams in data mining often focus on memorizing algorithms and formulas, but generative AI models like Claude can now solve many such problems. This course, taught by Professor Xiao Yanghua, instead trains students to command AI and evaluate its results, emphasizing judgment and creativity over rote learning.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude ( AI ) - Wikipedia</a></li>
<li><a href="https://docs.anthropic.com/en/docs/intro-to-claude">Intro to Claude - Anthropic</a></li>
<li><a href="https://digitalpromise.org/2026/01/26/evaluating-ai-in-education-an-analysis-of-state-guidance/">Evaluating AI in Education: An Analysis of State Guidance</a></li>

</ul>
</details>

**Tags**: `#AI in Education`, `#AI Evaluation`, `#Educational Innovation`, `#AI Literacy`, `#Pedagogy`

---

<a id="item-8"></a>
## [SpaceX Shows Investors Prototype Smartphone](https://www.wsj.com/tech/spacexs-telecom-dreams-d461e568) ⭐️ 8.0/10

SpaceX has shown investors a prototype smartphone that is thinner than an iPhone and runs its own operating system, aiming to integrate Starlink satellite connectivity for mobile services. This move signals SpaceX's potential entry into the mobile device market, leveraging its Starlink network to disrupt traditional telecom and satellite industries. The prototype reportedly runs a proprietary operating system and is slimmer than current iPhones. SpaceX president Gwynne Shotwell has also discussed building ground networks or partnering with cellular carriers for mobile services.

telegram · zaihuapd · Jul 5, 14:10

**Background**: SpaceX's Starlink satellite constellation provides broadband internet globally. The company already offers Direct to Cell service with T-Mobile for basic connectivity. A custom smartphone could tightly integrate satellite access, bypassing traditional carriers.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibtimes.co.uk/spacex-secret-ai-phone-prototype-1806844">SpaceX AI Phone Rumours Explained: Report Claims... | IBTimes UK</a></li>
<li><a href="https://www.forbes.com/sites/zacharyfolk/2026/07/01/musk-denies-report-spacex-is-developing-handheld-ai-device/">Musk Calls Reporting on SpaceX Prototype AI Device ‘Utterly False’</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Starlink`, `#mobile devices`, `#telecommunications`, `#satellite internet`

---

<a id="item-9"></a>
## [China Plans to Cut SCI Publication Incentives to Prevent Tech Leaks](https://www.ft.com/content/64a811f1-b132-4211-8a8c-2252cf964039?syn-25a6b1a6=1) ⭐️ 8.0/10

Chinese policymakers are discussing reducing incentives for researchers to publish in SCI journals, including lowering the weight of SCI papers in academic promotion and tenure decisions, due to national security concerns over technology leakage. This policy shift could significantly impact global academic publishing, as China is a major contributor to SCI journals, and may accelerate the development of domestic journals while raising concerns about research integrity and international collaboration. The National Natural Science Foundation of China now requires at least 20% of representative papers from funded projects to be published in Chinese-language journals, and a materials scientist has stopped submitting to foreign journals due to vague and tightening security reviews.

telegram · zaihuapd · Jul 6, 01:03

**Background**: SCI (Science Citation Index) is a prestigious citation database used to evaluate journal quality and researcher performance. China has long incentivized SCI publications to boost research output, but concerns about technology leakage and academic fraud have prompted a policy reevaluation. The government is also promoting domestic journals through initiatives like the 'China Science and Technology Journal Excellence Action Plan.'

<details><summary>References</summary>
<ul>
<li><a href="https://www.nppa.gov.cn/xxfb/zcfg/gfxwj/202106/t20210623_4514.html">中共中央宣传部 教育部 科技部印发 《关于推动学术期刊繁荣发展的意见...</a></li>
<li><a href="https://www.moe.gov.cn/jyb_xwfb/s5147/202106/t20210628_540716.html">中宣部、教育部、科技部印发《关于推动学术期刊繁荣发展的意见》 - 中...</a></li>

</ul>
</details>

**Discussion**: One commenter suggested the policy aims to combat academic fraud, reflecting a common sentiment that the current incentive system encourages misconduct.

**Tags**: `#academic publishing`, `#national security`, `#science policy`, `#China`, `#research integrity`

---

<a id="item-10"></a>
## [Karpathy's nanochat: Build ChatGPT for $100](https://github.com/karpathy/nanochat) ⭐️ 7.0/10

Andrej Karpathy created a branch in his nanochat repository to build a ChatGPT-like model for just $100, aiming to outperform GPT-2 (1.6B parameters) on an 8XH100 GPU node. This project demonstrates that a competitive LLM can be built at a fraction of typical costs, potentially democratizing AI development and enabling more researchers and hobbyists to experiment with large language models. The project is open-source, written in roughly 8,000 lines of PyTorch, and focuses on minimizing wall-clock time to surpass GPT-2 performance. The primary metric is 'time to GPT-2' on an 8XH100 node.

github · karpathy · Jul 4, 03:44

**Background**: Large language models like ChatGPT typically require millions of dollars in compute and data costs. Karpathy's nanochat aims to strip down the stack to essentials, showing that a capable model can be trained on a tight budget using efficient techniques and modest hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/karpathy/nanochat">GitHub - karpathy / nanochat : The best ChatGPT that $100 can buy.</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/10/andrej-karpathys-nanochat/">Build ChatGPT Clone with Andrej Karpathy 's nanochat</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ChatGPT`, `#open-source`, `#LLM`, `#cost-efficient`

---

<a id="item-11"></a>
## [Starring the Computer: Movie & TV Computer Catalog](https://www.starringthecomputer.com/computers.html) ⭐️ 7.0/10

A comprehensive online catalog, Starring the Computer, documents computers appearing in movies and TV shows with screenshots and context, covering decades of media. This resource serves as a valuable reference for retro computing enthusiasts, film historians, and prop designers, highlighting the cultural and technological significance of computers in media. The site includes entries from classic films like 2001: A Space Odyssey to modern TV shows, with consistent quality in screenshots and descriptions. Community comments provide technical corrections and additional resources.

hackernews · gitowiec · Jul 5, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48796093)

**Background**: Computers have been featured in films and TV for decades, often as props that reflect contemporary technology. This catalog systematically captures those appearances, offering a unique lens on both computing history and pop culture.

**Discussion**: Community comments include a correction about IBM AN-FSQ-7 panels from the 1950s SAGE system being modems, not computers, and a note that a user misidentified 6502 assembly in Westworld (1973) before realizing the 6502 didn't exist then. Another comment points to the similar Internet Movie Car Database (IMCDB).

**Tags**: `#computers`, `#movies`, `#pop culture`, `#curation`, `#retro computing`

---

<a id="item-12"></a>
## [Free Online Compiler Textbook Released](https://dthain.github.io/books/compiler/) ⭐️ 7.0/10

A free online textbook titled 'Introduction to Compilers and Language Design' has been published, based on a university course by Dr. Thain. This textbook provides a practical, accessible resource for learning compiler construction, which is a core topic in computer science education. The book includes a sample project that guides students to build a working C-style compiler step by step, similar to the course project.

hackernews · AlexeyBrin · Jul 5, 11:54 · [Discussion](https://news.ycombinator.com/item?id=48793454)

**Background**: Compilers translate high-level programming languages into machine code. Understanding compiler design is essential for language developers and advanced programmers.

**Discussion**: Former students highly recommend the book, praising Dr. Thain's teaching and the hands-on project. Some commenters also suggested related resources like C4 and C4x86.

**Tags**: `#compilers`, `#language design`, `#education`, `#programming languages`

---

<a id="item-13"></a>
## [World Map in 445 Bytes Using Deflate and Fetch](https://simonwillison.net/2026/Jul/4/building-a-world-map-with-only-500-bytes/#atom-everything) ⭐️ 7.0/10

Iwo Kadziela created a 445-byte ASCII world map by compressing the map data with deflate and using a JavaScript snippet that fetches a data URI and decompresses it via the DecompressionStream API. This demonstrates a clever combination of web APIs (fetch with data URIs, DecompressionStream) and compression to achieve extreme data efficiency, inspiring new approaches for embedding rich content in minimal bytes. The compressed data is stored as a base64-encoded data URI, fetched with fetch(), then piped through DecompressionStream('deflate-raw') to decompress, and finally rendered as a <pre> element with a small font size.

rss · Simon Willison · Jul 4, 23:09

**Background**: Deflate is a lossless compression algorithm widely used in formats like PNG and ZIP. The DecompressionStream API, part of the Compression Streams standard, allows streaming decompression in browsers. Data URIs embed data directly in URLs, and fetch() can retrieve them as if they were HTTP resources.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/DecompressionStream">DecompressionStream - Web APIs | MDN</a></li>
<li><a href="https://stackoverflow.com/questions/66573468/why-can-i-fetch-data-uris">javascript - Why can I fetch data URIs ? - Stack Overflow</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (item 48747762) was highly positive, with many praising the clever use of compression and web APIs. Some commenters discussed alternative compression methods and the elegance of the approach.

**Tags**: `#compression`, `#web APIs`, `#ASCII art`, `#JavaScript`, `#data URI`

---

<a id="item-14"></a>
## [South Korea Plans 800 Trillion Won Semiconductor Cluster, Aims to Double DRAM Output](https://t.me/zaihuapd/42357) ⭐️ 7.0/10

South Korea's Ministry of Trade, Industry and Energy announced a national semiconductor cluster plan, investing 800 trillion won (about 3.52 trillion yuan) to build four memory fabs in the southwestern region, aiming to double DRAM production within five years. This massive investment underscores South Korea's determination to maintain its leadership in the global memory market, especially as AI-driven demand for high-bandwidth memory (HBM) is crowding out commodity DRAM supply, potentially reshaping the semiconductor landscape. The plan includes building a second semiconductor production base in the southwestern region, with the government also allocating 30 trillion won over 15 years for related infrastructure. The global memory market is expected to grow more than fourfold in five years.

telegram · zaihuapd · Jul 4, 15:15

**Background**: DRAM (Dynamic Random-Access Memory) is a type of volatile memory widely used as main memory in computers and graphics cards. South Korea's Samsung Electronics and SK Hynix are two of the three major DRAM suppliers globally, alongside Micron Technology. The cluster plan aims to consolidate their competitive edge amid rising demand from AI and data centers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random-access memory - Wikipedia</a></li>
<li><a href="https://baike.baidu.com/item/半导体与集成电路产业集群/67318946">半导体与集成电路产业集群_百度百科</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#DRAM`, `#South Korea`, `#manufacturing`, `#investment`

---

<a id="item-15"></a>
## [Linux tops 2026 CVE charts; maintainer says it's good news](https://linuxiac.com/linux-tops-2026-cve-charts/) ⭐️ 7.0/10

In the first half of 2026, Linux led all vendors with 2,308 CVEs, ahead of Google (1,752), Microsoft (843), and Apple (284). Kernel maintainer Greg Kroah-Hartman argues this reflects more complete and transparent vulnerability reporting, not worse security. This highlights a systemic difference in vulnerability disclosure between open-source and proprietary software, where commercial vendors often report only high-severity CVEs while open-source projects report all known issues. It challenges the common perception that high CVE counts indicate poor security. Greg Kroah-Hartman noted that commercial vendors like Apple and Microsoft often only report CVEs classified as 'high severity,' whereas open-source projects cannot predict downstream usage and must report all issues. He called on other vendors to 'step up' and report CVEs comprehensively rather than selectively.

telegram · zaihuapd · Jul 4, 16:00

**Background**: CVE (Common Vulnerabilities and Exposures) is a publicly accessible catalog of cybersecurity vulnerabilities, managed by the CVE Program. Each CVE ID is assigned by a CNA (CVE Numbering Authority) after a vulnerability is reported and validated. The Linux kernel runs on billions of devices worldwide, making comprehensive CVE reporting critical for downstream users to assess risk.

<details><summary>References</summary>
<ul>
<li><a href="https://nvd.nist.gov/general/cve-process">NVD - CVEs and the NVD Process</a></li>
<li><a href="https://www.cve.org/">CVE : Common Vulnerabilities and Exposures</a></li>
<li><a href="https://en.wikipedia.org/wiki/Greg_Kroah-Hartman">Greg Kroah - Hartman - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Linux`, `#CVE`, `#security`, `#open source`, `#vulnerability reporting`

---

<a id="item-16"></a>
## [Samsung Plans ~20% DRAM Price Hike in Q3](https://t.me/zaihuapd/42362) ⭐️ 7.0/10

Samsung Electronics plans to raise DRAM prices by approximately 20% in the third quarter and has verbally notified some customers. The company has not yet issued an official comment on the pricing. This price increase reflects tightening supply and sustained strong demand from AI servers and advanced devices, directly impacting hardware costs for data centers and AI/ML systems. Industry analysts expect similar price hikes across the memory market. TrendForce forecasts Q3 DRAM contract prices to rise 13%–18% quarter-over-quarter, and NAND flash contract prices to rise 10%–15%. Sigmaintell Consulting expects LPDDR5X 8 GB chip contract prices to increase by about 20%.

telegram · zaihuapd · Jul 5, 04:03

**Background**: DRAM (Dynamic Random-Access Memory) is a type of volatile memory widely used as main memory in computers and servers. NAND flash is a non-volatile storage technology used in SSDs and memory cards. LPDDR5X is a low-power DRAM variant commonly used in mobile devices and AI applications. The memory market is dominated by three major suppliers: Samsung, SK Hynix, and Micron.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DRAM">DRAM</a></li>
<li><a href="https://en.wikipedia.org/wiki/NAND_flash">NAND flash</a></li>
<li><a href="https://en.wikipedia.org/wiki/LPDDR">LPDDR</a></li>

</ul>
</details>

**Tags**: `#DRAM`, `#Samsung`, `#memory pricing`, `#AI infrastructure`, `#supply chain`

---

<a id="item-17"></a>
## [OpenAI Never Visited Stargate UK Site, Guardian Finds](https://www.theguardian.com/technology/2026/jul/04/openai-apparent-failure-visit-key-site-questions-stargate-uk-project) ⭐️ 7.0/10

A Guardian investigation revealed that OpenAI never visited the key UK site for its Stargate project, Cobalt Park in North Tyneside, and local authorities held no meetings with OpenAI or partner Nscale. The project was paused in April 2026, with insiders calling it a government PR stunt. This casts doubt on the credibility of OpenAI's $30 billion investment pledge and raises questions about the transparency of major AI infrastructure announcements. It could undermine trust in tech companies' commitments and affect UK tech policy and international investment relations. The Stargate UK project was announced during a Trump visit to the UK as a flagship UK-US AI collaboration. It was paused due to regulatory environment and high energy costs, and a local Conservative MP said the project 'looks extremely unlikely' to proceed.

telegram · zaihuapd · Jul 5, 05:09

**Background**: Stargate is a massive AI infrastructure initiative by OpenAI, initially envisioned to involve up to $1 trillion in data centers globally. The UK project was a key part of this plan, but the Guardian's findings suggest it may have been announced without proper due diligence, potentially as a political gesture.

<details><summary>References</summary>
<ul>
<li><a href="https://thenextweb.com/news/openai-apparently-never-visited-the-site-of-its-flagship-uk-ai-project">OpenAI never visited its Stargate UK site, Guardian finds</a></li>
<li><a href="https://www.evolmagazine.com/en/news/ai/openai-stargate-plan-trillion-global-data-centers.html">OpenAI Stargate Plan: $1 Trillion in AI Data Centers</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cobalt_Park">Cobalt Park - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Stargate`, `#AI infrastructure`, `#investigative journalism`, `#UK tech policy`

---

<a id="item-18"></a>
## [Chinese Startup Tests CO2 Cold Launch Rocket Technology](https://www.techradar.com/pro/chinese-tests-rocket-using-the-same-gas-used-by-coca-cola-to-make-space-flights-cheaper-safer-cleaner-and-cooler) ⭐️ 7.0/10

Chinese startup Zhiyu Aerospace Technology, in collaboration with Z-Trak Space, is testing a cold launch system that uses supercritical carbon dioxide to eject a rocket before igniting its engine. If successful, this technology could significantly reduce launch infrastructure costs and enable higher launch frequencies by avoiding the extreme heat damage from traditional launches, potentially transforming small liquid-fuel rocket launches. Supercritical CO₂ is a fluid state achieved at high temperature and pressure, which expands instantaneously to generate high-pressure gas for ejection. The system is designed for small launch vehicles and is still experimental.

telegram · zaihuapd · Jul 5, 13:29

**Background**: Cold launch technology, pioneered by the Soviets, ejects a missile or rocket from its launcher using gas before the main engine ignites, reducing thermal and mechanical stress on launch infrastructure. Supercritical carbon dioxide is a non-toxic, inexpensive substance commonly used in carbonated beverages.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3359056/can-chinas-co2-rocket-launch-cold-same-gas-carbonates-coca-cola">Can China’s ‘CO2 rocket’ launch cold on the same gas that carbonates Coca-Cola? | South China Morning Post</a></li>
<li><a href="https://www.chinatechnews.com/2026/07/01/124743-can-chinas-co2-rocket-launch-cold-on-the-same-gas-that-carbonates-coca-cola">Can China’s ‘CO2 rocket’ launch cold on the same gas that ...</a></li>
<li><a href="https://www.techradar.com/pro/chinese-tests-rocket-using-the-same-gas-used-by-coca-cola-to-make-space-flights-cheaper-safer-cleaner-and-cooler">This Chinese startup thinks fizzy drink gas could make rocket launches dramatically cheaper and cleaner | TechRadar</a></li>

</ul>
</details>

**Discussion**: The Telegram comment accompanying the news is lighthearted, noting the title was meant to be fun, but no substantive technical discussion was provided.

**Tags**: `#rocket technology`, `#aerospace`, `#cold launch`, `#carbon dioxide`, `#China`

---