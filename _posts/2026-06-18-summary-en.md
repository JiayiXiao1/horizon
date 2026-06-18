---
layout: default
title: "Horizon Summary: 2026-06-18 (EN)"
date: 2026-06-18
lang: en
---

> From 44 items, 25 important content pieces were selected

---

1. [GLM-5.2: New Leading Open-Weight LLM Released](#item-1) ⭐️ 9.0/10
2. [Critical Path Traversal in Nezha Monitor (CVSS 9.1)](#item-2) ⭐️ 9.0/10
3. [Epic Games Unveils Lore: Open-Source VCS for Game Dev](#item-3) ⭐️ 8.0/10
4. [Leaked Docs Reveal OpenAI Losing Billions Annually](#item-4) ⭐️ 8.0/10
5. [U.S. Science in Crisis: Funding, Visas, Brain Drain](#item-5) ⭐️ 8.0/10
6. [Adam Launches CADAM: Open-Source AI CAD from Text](#item-6) ⭐️ 8.0/10
7. [Tesco moves 40k workloads off VMware over Broadcom pricing](#item-7) ⭐️ 8.0/10
8. [RFC 10008 Standardizes HTTP QUERY Method](#item-8) ⭐️ 8.0/10
9. [Charity Majors: AI Demands More Engineering Discipline](#item-9) ⭐️ 8.0/10
10. [Export Controls on AI Models Harm US Cyber Defense](#item-10) ⭐️ 8.0/10
11. [GitHub Copilot switches to usage-based billing from June 2026](#item-11) ⭐️ 8.0/10
12. [China Expands STAR Market IPO Criteria to AI and Hard Tech](#item-12) ⭐️ 8.0/10
13. [Microsoft Expands China AI Business via OpenAI Models](#item-13) ⭐️ 8.0/10
14. [US delays blacklisting DeepSeek and over 100 Chinese firms](#item-14) ⭐️ 7.0/10
15. [Firecracker VMs on EC2 Launch Browsers in <1s](#item-15) ⭐️ 7.0/10
16. [AI Models Battle in 'Last Agent Standing' Game Benchmark](#item-16) ⭐️ 7.0/10
17. [Volkswagen blocks GrapheneOS users from app](#item-17) ⭐️ 7.0/10
18. [MicroUI: Tiny Immediate-Mode GUI Library in ANSI C](#item-18) ⭐️ 7.0/10
19. [Photobucket Demands $5 to Retrieve Your Own Photos](#item-19) ⭐️ 7.0/10
20. [Datasette 1.0a34 Adds CRUD UI for Rows](#item-20) ⭐️ 7.0/10
21. [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](#item-21) ⭐️ 7.0/10
22. [Anthropic surpasses OpenAI in enterprise AI market share](#item-22) ⭐️ 7.0/10
23. [WeChat Pay Launches AI-Exclusive Card with Per-Transaction Authorization](#item-23) ⭐️ 7.0/10
24. [Chinese Telecom Token Plans Shock Developers with High Costs](#item-24) ⭐️ 7.0/10
25. [OpenAI Codex Now Supports Custom Third-Party Model Providers](#item-25) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GLM-5.2: New Leading Open-Weight LLM Released](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B-parameter Mixture-of-Experts open-weights LLM with 40B active parameters and a 1M token context window, under the MIT license on June 16, 2026. GLM-5.2 is the first open-weights model to top the Artificial Analysis Intelligence Index, outperforming MiniMax-M3 and DeepSeek V4 Pro, and ranks 2nd on Code Arena WebDev, challenging proprietary models at a fraction of the cost. The model uses 43k output tokens per task on the Intelligence Index, more than competitors, and is available via OpenRouter at $1.40/M input and $4.40/M output tokens. It is text-only; Z.ai's vision model GLM-5V-Turbo remains closed-source.

rss · Simon Willison · Jun 17, 23:58

**Background**: Mixture-of-Experts (MoE) is an architecture that activates only a subset of parameters per token, enabling large models to be efficient. GLM-5.2's 1M context window allows processing of very long documents, such as entire codebases or books. Open-weights models are released with publicly available model parameters, allowing researchers and developers to run them locally or fine-tune them.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.z.ai/guides/llm/glm-5.2">GLM - 5 . 2 - Overview - Z.AI DEVELOPER DOCUMENT</a></li>
<li><a href="https://www.datacamp.com/blog/glm-5-2">GLM - 5 . 2 : Features, Setup, and Model Switching Guide | DataCamp</a></li>
<li><a href="https://lushbinary.com/blog/glm-5-2-developer-guide-1m-context-coding-plan/">GLM 5 . 2 Developer Guide: 1M Context & MoE | Lushbinary</a></li>

</ul>
</details>

**Discussion**: Community members praised GLM-5.2's performance and low cost, with some noting it rivals proprietary models like Opus 4.7 at a fraction of the price. However, concerns were raised about reasoning efficiency, as one user reported a simple math evaluator task took 15 minutes and 45k tokens. Others highlighted the model's token-hungry nature compared to peers.

**Tags**: `#LLM`, `#open-weights`, `#GLM-5.2`, `#AI`, `#benchmark`

---

<a id="item-2"></a>
## [Critical Path Traversal in Nezha Monitor (CVSS 9.1)](https://t.me/zaihuapd/42001) ⭐️ 9.0/10

A critical unauthenticated path traversal vulnerability (CVE-2026-53519, CVSS 9.1) has been disclosed in Nezha monitoring tool versions below 2.0.13, allowing attackers to read configuration files and obtain JWT secrets. This vulnerability affects a widely-used open-source monitoring tool, enabling unauthenticated attackers to compromise the entire monitoring infrastructure by stealing JWT secrets, which can lead to full system takeover. The vulnerability is exploited by sending a crafted GET request like /dashboard../data/config.yaml, which bypasses authentication due to a prefix confusion bug. Users must upgrade to version 2.0.13 or later immediately.

telegram · zaihuapd · Jun 17, 01:25

**Background**: Nezha is a popular open-source, lightweight monitoring and alerting system for servers. Path traversal vulnerabilities allow attackers to access files outside the intended directory. JWT secrets are used to sign authentication tokens; if leaked, attackers can forge tokens and gain unauthorized access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tjsky.net/news/1664">哪吒探针爆致命 漏 洞 （ CVE - 2026 - 53519 ）大批 MJJ... | 秋风于渭水</a></li>
<li><a href="https://nezha.io/">哪 吒 监 控 Nezha Monitoring</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#open-source`, `#monitoring`, `#path-traversal`

---

<a id="item-3"></a>
## [Epic Games Unveils Lore: Open-Source VCS for Game Dev](https://lore.org/) ⭐️ 8.0/10

Epic Games has announced Lore, an open-source version control system designed for scalability, targeting game development as a competitor to Perforce. Lore addresses a major pain point in game development—handling large binary files and file locking—which Git struggles with, potentially offering a free, open-source alternative to the proprietary Perforce. Lore is optimized for projects combining code with large binary assets, such as textures, 3D models, and audio files, and includes features like exclusive file locking for artists.

hackernews · regnerba · Jun 17, 14:30 · [Discussion](https://news.ycombinator.com/item?id=48571081)

**Background**: Version control systems (VCS) track changes to files over time. Git is popular for code but inefficient for large binary files; Perforce is the industry standard in game development but is proprietary and complex. Lore aims to combine the openness of Git with the scalability of Perforce.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/EpicGames/lore">Lore is a next-generation, open source revision control system</a></li>
<li><a href="https://www.phoronix.com/news/Epic-Games-Lore-VCS">Epic Games Announces Lore Open-Source Version Control System</a></li>
<li><a href="https://dev.epicgames.com/documentation/unreal-engine/lore-version-control-in-unreal-engine?lang=en-US">Lore Version Control in Unreal Engine - Epic Dev</a></li>

</ul>
</details>

**Discussion**: The Hacker News community largely sees Lore as a promising challenger to Perforce, especially for Unreal Engine development. Some commenters note Git's UI unfriendliness and Perforce's complexity, while others question whether Lore can match Perforce's maturity and ecosystem.

**Tags**: `#version control`, `#game development`, `#open source`, `#scalability`, `#Perforce`

---

<a id="item-4"></a>
## [Leaked Docs Reveal OpenAI Losing Billions Annually](https://arstechnica.com/ai/2026/06/leaked-financial-docs-show-openai-is-losing-billions-of-dollars-a-year/) ⭐️ 8.0/10

Leaked financial documents show OpenAI is losing billions of dollars per year due to extremely high overhead and massive R&D spending, despite rapid revenue growth. This revelation raises serious questions about the sustainability of OpenAI's business model and the broader AI industry's path to profitability, affecting investors, competitors, and customers. The documents indicate SG&A costs are 55% of revenue, which is very high, and R&D costs are astronomical, suggesting that even with revenue growth, profitability remains distant.

hackernews · greenchair · Jun 17, 21:31 · [Discussion](https://news.ycombinator.com/item?id=48577208)

**Background**: OpenAI is a leading AI research and deployment company known for ChatGPT and GPT-4. As a startup, it has prioritized rapid growth and cutting-edge research over short-term profitability, but these leaks highlight the financial strain of that strategy.

**Discussion**: Community comments are divided: some argue the losses are unsustainable due to high overhead and R&D costs, while others point to rapid revenue growth and a potential path to profitability if costs are managed. There is also debate about whether the focus should shift to reducing inference costs or continuing AGI research.

**Tags**: `#OpenAI`, `#financial analysis`, `#AI industry`, `#business model`, `#startup sustainability`

---

<a id="item-5"></a>
## [U.S. Science in Crisis: Funding, Visas, Brain Drain](https://www.scientificamerican.com/article/americas-compact-between-science-and-politics-is-broken/) ⭐️ 8.0/10

U.S. science is in chaos as research funding dries up, visa restrictions block foreign talent, and many researchers are leaving the country or abandoning science altogether. This crisis threatens U.S. leadership in science and innovation, potentially causing long-term damage to the nation's research enterprise and economic competitiveness. The article highlights a broken compact between science and politics, with grant funding not renewed, visa restrictions preventing hiring of foreign graduate students, and a palpable sense of tension among researchers.

hackernews · presspot · Jun 17, 09:54 · [Discussion](https://news.ycombinator.com/item?id=48568058)

**Background**: U.S. science has long relied on federal grants and a steady influx of international talent. Recent policy changes and funding cuts have disrupted this system, leading to a brain drain and demoralization in the research community.

**Discussion**: Commenters share personal stories of leaving the U.S. or reducing work hours due to funding cuts and visa issues. Many express that the situation has worsened recently, with even established scientists preparing backup plans.

**Tags**: `#science policy`, `#research funding`, `#US politics`, `#brain drain`

---

<a id="item-6"></a>
## [Adam Launches CADAM: Open-Source AI CAD from Text](https://github.com/Adam-CAD/CADAM) ⭐️ 8.0/10

Adam (YC W25) has launched CADAM, an open-source text-to-CAD platform that generates parametric 3D models from natural language prompts using a code-based paradigm (OpenSCAD). This marks a significant step toward making AI the primary medium for mechanical design, potentially lowering the barrier for rapid prototyping and enabling non-experts to create CAD models. CADAM runs entirely in the browser via WebAssembly-compiled OpenSCAD and Three.js rendering, supports multiple LLMs (Claude, Gemini, OpenAI), and outputs STL, SCAD, and other formats.

hackernews · zachdive · Jun 17, 16:14 · [Discussion](https://news.ycombinator.com/item?id=48572553)

**Background**: Traditional CAD software like Fusion 360 or SolidWorks requires significant expertise and manual modeling. Text-to-CAD tools aim to generate editable 3D geometry from natural language, similar to how AI code generation works. CADAM uses a code-as-CAD approach, producing OpenSCAD scripts that can be tweaked via sliders.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/Adam-CAD/CADAM">GitHub - Adam-CAD/CADAM: CADAM is the open source text-to-CAD web application · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/CADAM">CADAM - Wikipedia</a></li>
<li><a href="https://sourceforge.net/projects/cadam.mirror/">CADAM download | SourceForge.net</a></li>

</ul>
</details>

**Discussion**: The Hacker News community showed mixed reactions: some daily CAD users expressed excitement, while engineers raised concerns about practical use cases, noting that for simple parts, manual modeling is often faster and more reliable than verifying AI output.

**Tags**: `#AI`, `#CAD`, `#open-source`, `#mechanical-design`, `#YC`

---

<a id="item-7"></a>
## [Tesco moves 40k workloads off VMware over Broadcom pricing](https://arstechnica.com/information-technology/2026/06/tesco-moving-40000-server-workloads-off-vmware-amid-broadcoms-abusive-conduct/) ⭐️ 8.0/10

Tesco, the UK's largest supermarket chain, is migrating 40,000 server workloads away from VMware due to Broadcom's aggressive pricing and licensing changes, which have caused costs to skyrocket by 150-1000%. This migration signals a major enterprise shift away from VMware, potentially triggering a wave of similar moves across industries as Broadcom's post-acquisition strategy alienates large customers. Tesco's new virtualization software is incompatible with its existing Veeam and Zerto backup tools, creating data security challenges during the migration. The company has not disclosed the alternative platform, but community speculation points to Proxmox or Nutanix.

hackernews · Bender · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576838)

**Background**: Broadcom acquired VMware in November 2023 and immediately replaced perpetual licenses with expensive subscriptions, introduced a 72-core minimum, and enforced bundled purchases, causing price increases of 150-1000%. This has driven many enterprises to explore alternatives like Proxmox, Nutanix, or public cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://vmwaremadesimple.com/articles/broadcom-vmware-licensing-changes-2026.html">Broadcom's VMware Licensing Changes in 2026: What Every Admin ...</a></li>
<li><a href="https://cloudinfra.blog/comprehensive-analysis-of-broadcoms-vmware-license-pricing-changes-and-their-impact/">Comprehensive Analysis of Broadcom's VMware License Pricing ...</a></li>
<li><a href="https://www.softwareseni.com/broadcom-vmware-pricing-changes-understanding-the-licensing-crisis-driving-migration/">Broadcom VMware Pricing Changes - Understanding the Licensing ...</a></li>

</ul>
</details>

**Discussion**: Commenters widely support Tesco's move, with many sharing their own negative experiences with Broadcom. Some note that Broadcom's aggressive tactics are effectively marketing for Proxmox. Others express concern about the high cost and complexity of large-scale migrations.

**Tags**: `#VMware`, `#Broadcom`, `#enterprise migration`, `#virtualization`, `#cloud`

---

<a id="item-8"></a>
## [RFC 10008 Standardizes HTTP QUERY Method](https://www.rfc-editor.org/info/rfc10008/) ⭐️ 8.0/10

RFC 10008, published on June 15, 2026, defines a new HTTP QUERY method that is safe, idempotent, and can carry a request body, filling a long-standing gap in the HTTP protocol. This new method provides a standardized alternative to using POST for queries, enabling safe caching and retries without side effects, which is particularly beneficial for GraphQL APIs and complex search operations. QUERY is similar to POST but guarantees safety and idempotency, meaning the request can be automatically repeated without concern for state changes. The request body is included in the cache key, which may lead to unbounded cache keys.

hackernews · schappim · Jun 17, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48568502)

**Background**: HTTP GET requests cannot have a body, and POST requests are neither safe nor idempotent, forcing developers to use POST for queries that require a body, which breaks caching and causes re-submission warnings. The QUERY method solves this by providing a safe, idempotent method with a body.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rfc-editor.org/info/rfc10008/">RFC 10008: The HTTP QUERY Method | RFC Editor</a></li>
<li><a href="https://httpwg.org/http-extensions/draft-ietf-httpbis-safe-method-w-body.html">The HTTP QUERY Method</a></li>
<li><a href="https://blainsmith.com/articles/rfc-10008-http-query-method/">RFC 10008: The HTTP QUERY Method - Blain Smith</a></li>

</ul>
</details>

**Discussion**: Commenters noted that a strong motivating example would have helped, and discussed the oddity of including the request body in the cache key. Some wondered if HTML forms will support QUERY to avoid re-submission warnings, while others mentioned they have been sending bodies with GET for years.

**Tags**: `#HTTP`, `#RFC`, `#protocol`, `#web`, `#caching`

---

<a id="item-9"></a>
## [Charity Majors: AI Demands More Engineering Discipline](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors argues that AI has made code generation cheap and disposable, requiring more engineering discipline, not less. She compares this shift to the transition from handcrafted server pets to immutable infrastructure. This insight reframes the impact of AI on software engineering, emphasizing that while code becomes cheaper, the need for rigorous system design, testing, and operations increases. It challenges the notion that AI reduces the need for skilled engineers. Majors notes that lines of code went from being treasured and carefully curated to disposable and regenerable overnight. She draws a parallel to the earlier shift from server pets to immutable infrastructure, suggesting a similar need for increased discipline.

rss · Simon Willison · Jun 17, 17:12

**Background**: Charity Majors is a well-known engineer and CTO, co-founder of Honeycomb, and a respected voice in observability and engineering culture. Her argument builds on the observation that AI coding assistants like GitHub Copilot and Claude Code have dramatically lowered the cost of generating code, shifting the bottleneck from writing to verifying and maintaining systems.

<details><summary>References</summary>
<ul>
<li><a href="https://charitydotwtf.substack.com/p/ai-demands-more-engineering-discipline">AI demands more engineering discipline. Not less</a></li>
<li><a href="https://perevillega.com/posts/2026-03-16-code-is-cheap-now/">Code Is Cheap Now, And That Changes Everything - Pere Villega</a></li>

</ul>
</details>

**Tags**: `#ai-assisted-programming`, `#software-engineering`, `#generative-ai`, `#economics-of-code`

---

<a id="item-10"></a>
## [Export Controls on AI Models Harm US Cyber Defense](https://simonwillison.net/2026/Jun/16/fable-5-export-controls/#atom-everything) ⭐️ 8.0/10

The US government's export controls on Anthropic's Claude Fable 5 and Mythos 5 models, imposed on June 13, 2026, inadvertently block legitimate security research that asks models to fix code with known vulnerabilities. This policy paradoxically weakens US cyber defense by preventing defenders from using AI to find, fix, and test security patches, while the capability to craft exploits is inseparable from defensive bug-fixing. Researchers used open-source code with known CVEs and deliberately planted vulnerabilities, asking Fable 5 to 'fix this code'—a defensive request that triggered the export control ban. Kate Moussouris confirmed that the 'jailbreak' was simply asking the model to fix bugs.

rss · Simon Willison · Jun 16, 05:20

**Background**: Export controls on AI models aim to prevent adversaries from using advanced AI for cyber attacks. However, the same capabilities that allow models to generate exploit code are essential for defensive security tasks like vulnerability remediation and patch verification. The Bureau of Industry and Security (BIS) issued a 'Is Informed' letter to Anthropic, requiring export licenses for sharing models with foreign nationals.

<details><summary>References</summary>
<ul>
<li><a href="https://www.aimadetools.com/blog/claude-fable-5-banned-us-export-controls">Claude Fable 5 Banned — US Government Export Controls ...</a></li>
<li><a href="https://cybersecuritynews.com/claude-mythos-5-and-fable-5-export/">U.S. Commerce Dept Imposes Export Controls on Anthropic's ...</a></li>
<li><a href="https://www.gtlaw.com/en/insights/2026/6/ai-company-anthropic-suspends-access-to-claude-fable-5-claude-mythos-5-following-us-export-control-directive">AI Company Anthropic Suspends Access to Claude Fable 5 ...</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights the absurdity of the policy, noting that non-technical decision-makers conflate defensive bug-fixing with offensive capability. Commenters emphasize that removing the ability to fix bugs would make models useless for security, and that the export controls are counterproductive.

**Tags**: `#AI policy`, `#export controls`, `#cybersecurity`, `#AI safety`, `#open source`

---

<a id="item-11"></a>
## [GitHub Copilot switches to usage-based billing from June 2026](https://t.me/zaihuapd/42003) ⭐️ 8.0/10

GitHub announced that from June 1, 2026, all GitHub Copilot plans will transition to usage-based billing, where usage is measured in GitHub AI Credits. Legacy users on annual plans can keep their old billing until their plan expires. This shift from flat-rate to usage-based pricing could significantly increase costs for heavy Copilot users, especially those relying on expensive models like GPT-5.5. It also aligns GitHub Copilot with typical cloud API billing models, potentially affecting how developers and organizations budget for AI coding assistance. Under the new system, each plan includes a monthly allowance of GitHub AI Credits, with paid plans able to purchase additional usage. The GPT-5.5 model has a 57x multiplier per request in the announced multiplier table, though promotional pricing initially set it at 7.5x.

telegram · zaihuapd · Jun 17, 03:16

**Background**: GitHub Copilot is an AI-powered code completion tool that suggests code snippets and functions as developers type. Previously, Copilot used a flat monthly fee per user (e.g., Copilot Business at $19/user/month) with a limit on premium requests. The new usage-based billing introduces AI Credits, where different models consume credits at different rates based on their computational cost.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/news-insights/company-news/github-copilot-is-moving-to-usage-based-billing/">GitHub Copilot is moving to usage-based billing</a></li>
<li><a href="https://docs.github.com/en/copilot/reference/copilot-billing/models-and-pricing">Models and pricing for GitHub Copilot - GitHub Docs</a></li>
<li><a href="https://github.blog/changelog/2026-04-24-gpt-5-5-is-generally-available-for-github-copilot/">GPT-5.5 is generally available for GitHub Copilot</a></li>

</ul>
</details>

**Tags**: `#GitHub Copilot`, `#pricing`, `#AI coding assistant`, `#billing`

---

<a id="item-12"></a>
## [China Expands STAR Market IPO Criteria to AI and Hard Tech](https://mp.weixin.qq.com/s/ywLPXkSlqY9S5Vwp8G5saA) ⭐️ 8.0/10

China Securities Regulatory Commission (CSRC) Chairman Wu Qing announced at the 2026 Lujiazui Forum that the STAR Market's fifth set of listing criteria will be expanded to include AI, quantum technology, biomanufacturing, and embodied AI companies. The regulator also plans to introduce shelf offering reforms and issue guidelines on AI in capital markets. This policy shift significantly broadens IPO access for AI and hard tech firms, potentially reshaping capital allocation in China's technology sector. It signals strong government support for strategic emerging industries and may accelerate the listing of innovative but pre-revenue companies. The fifth set of criteria previously focused on biotech firms; now it covers quantum, biomanufacturing, and embodied AI. CSRC also vowed to crack down on fraudulent tech claims and market manipulation. Currently, tech firms account for over 30% of A-share market cap and 45% of companies with market cap over 100 billion yuan.

telegram · zaihuapd · Jun 17, 08:30

**Background**: The STAR Market (科创板) is China's Nasdaq-style board for tech companies, launched in 2019. Its fifth set of listing criteria allows pre-revenue companies to go public if they meet certain R&D and market value thresholds. Previously, this standard was primarily used by biotech firms. Embodied AI refers to AI systems that interact with the physical world, such as humanoid robots. Shelf offering (储架发行) is a mechanism where issuers register securities once and issue them in multiple tranches over time.

<details><summary>References</summary>
<ul>
<li><a href="http://macrochina.com.cn/news_speed/hgjj/20250627123825.shtml">macrochina.com.cn/news_speed/hgjj/20250627123825.shtml</a></li>
<li><a href="https://www.caict.ac.cn/kxyj/qwfb/bps/202408/P020240830312499650772.pdf">caict.ac.cn/kxyj/qwfb/bps/202408/P020240830312499650772.pdf</a></li>
<li><a href="https://baike.baidu.com/item/储架发行制度/1648322">储架发行制度_百度百科</a></li>

</ul>
</details>

**Tags**: `#AI`, `#IPO`, `#China`, `#regulation`, `#hard tech`

---

<a id="item-13"></a>
## [Microsoft Expands China AI Business via OpenAI Models](https://www.bloomberg.com/news/articles/2026-06-17/microsoft-s-china-ai-business-grows-on-openai-model-sales) ⭐️ 8.0/10

Microsoft is rapidly expanding its AI business in China by selling OpenAI models through Azure, with ByteDance as its largest customer spending over $1 billion annually on Microsoft AI and cloud services. This development raises significant geopolitical and security concerns, as US lawmakers and OpenAI worry about potential technology transfer and model distillation by Chinese firms, which could erode US competitive advantage in AI. Azure's AI revenue in China has grown rapidly, doubling or tripling annually for two consecutive years, and Microsoft claims it only sells to established enterprises, not individual developers, with models hosted in overseas data centers accessed via the internet.

telegram · zaihuapd · Jun 18, 01:06

**Background**: Model distillation is a technique where a smaller 'student' model learns from a larger 'teacher' model, potentially allowing Chinese companies to replicate OpenAI's capabilities without direct access. Microsoft operates Azure in China through a partnership with 21Vianet to comply with local regulations, but the OpenAI models are hosted outside China to address security concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/azure/china/overview-operations">Microsoft Azure in China</a></li>
<li><a href="https://openai.com/index/update-on-safety-and-security-practices/">An update on our safety & security practices - OpenAI</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#OpenAI`, `#AI regulation`, `#China`, `#cloud computing`

---

<a id="item-14"></a>
## [US delays blacklisting DeepSeek and over 100 Chinese firms](https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/) ⭐️ 7.0/10

The US has decided to hold off on adding Chinese AI startup DeepSeek, memory chipmaker CXMT, and more than 100 other companies flagged as national security risks to a trade blacklist, according to sources familiar with the matter. This decision signals a potential easing of US-China tech tensions, but also raises questions about enforcement and the impact on AI development. The delay could affect the competitive landscape for AI models and chip supply chains. The blacklist, known as the Entity List, restricts US companies from selling goods and services to listed entities, but does not forbid buying from them. DeepSeek's models are open-weight and trained using weaker AI chips due to export restrictions, making them cost-effective.

hackernews · giuliomagnifico · Jun 17, 03:55 · [Discussion](https://news.ycombinator.com/item?id=48565498)

**Background**: DeepSeek is a Chinese AI company founded in 2023 that developed the DeepSeek-R1 model, which rivals OpenAI's GPT-4 at a fraction of the cost. Its success has been described as a 'Sputnik moment' for US AI, threatening Nvidia's market dominance. The Entity List is a US trade restriction tool used to deny exports to entities deemed a national security risk.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(Company)">DeepSeek (Company)</a></li>
<li><a href="https://www.cnbc.com/2026/06/17/us-deepseek-blacklist-cxmt-national-security-risks-.html">U.S. holds off blacklisting China's DeepSeek, more than 100 ...</a></li>
<li><a href="https://www.reuters.com/world/china/us-holds-off-blacklisting-chinas-deepseek-more-than-100-firms-deemed-security-2026-06-17/">Exclusive: US holds off blacklisting China's DeepSeek, more ...</a></li>

</ul>
</details>

**Discussion**: Comments express mixed views: some users appreciate DeepSeek's affordability and performance, while others criticize US blacklisting as hypocritical or unenforceable. There is debate over whether the Entity List effectively restricts Chinese AI companies given their limited reliance on US goods.

**Tags**: `#AI`, `#geopolitics`, `#DeepSeek`, `#regulation`, `#US-China`

---

<a id="item-15"></a>
## [Firecracker VMs on EC2 Launch Browsers in <1s](https://browser-use.com/posts/firecracker-browser-infra) ⭐️ 7.0/10

Browser-use.com describes a method to run Firecracker microVMs on EC2 instances, enabling stealthy browser startups in under one second with an 81% anti-bot evasion rate. This approach significantly improves browser automation for web scraping and testing by combining fast startup with high anti-bot evasion, though it raises ethical concerns about bypassing website protections. Nested virtualization on regular EC2 instances was only possible since February 2026, previously requiring metal instances. The system uses Firecracker's minimal device model to reduce attack surface and memory footprint.

hackernews · gregpr07 · Jun 16, 15:15 · [Discussion](https://news.ycombinator.com/item?id=48556561)

**Background**: Firecracker is an open-source virtualization technology by AWS that creates lightweight microVMs with fast boot times and strong isolation. Anti-bot measures on websites detect headless browsers through fingerprinting and behavioral analysis, making stealthy automation challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://firecracker-microvm.github.io/">Firecracker</a></li>
<li><a href="https://github.com/firecracker-microvm/firecracker">GitHub - firecracker - microvm / firecracker : Secure and fast microVMs...</a></li>

</ul>
</details>

**Discussion**: Commenters raised ethical concerns about using such technology to bypass anti-bot measures, while others noted technical limitations like nested virtualization only recently becoming available on regular EC2. Some suggested alternatives like AWS Lambda or Lightpanda browser for simpler setups.

**Tags**: `#Firecracker`, `#EC2`, `#browser automation`, `#anti-bot`, `#virtualization`

---

<a id="item-16"></a>
## [AI Models Battle in 'Last Agent Standing' Game Benchmark](https://openrouter.ai/blog/insights/royale-last-agent-standing/) ⭐️ 7.0/10

A blog post on OpenRouter benchmarks AI models like Claude and Grok in a 'last agent standing' game, revealing that DeepSeek V4 Flash wins on cost efficiency while Grok shows performance improvements but raises concerns about silent model rerouting. This benchmark highlights the trade-offs between cost and performance for AI models in real-time decision-making scenarios, which is crucial for developers deploying AI agents in cost-sensitive applications. The experiment ran 30 games costing $482 total, avoiding frontier-tier models like Opus 4.7 or GPT-5.5 which would have cost around $3,000. DeepSeek V4 Flash, a Mixture-of-Experts model with 284B total parameters and 13B activated, demonstrated exceptional cost efficiency.

hackernews · Usu · Jun 17, 21:00 · [Discussion](https://news.ycombinator.com/item?id=48576824)

**Background**: The 'last agent standing' game is a battle royale where AI agents compete autonomously, making decisions on movement, resource gathering, and combat. This benchmark tests models' ability to reason and act under pressure. DeepSeek V4 Flash is a preview of the DeepSeek V4 series, designed for efficient reasoning with a 1M-token context window.

<details><summary>References</summary>
<ul>
<li><a href="https://api-docs.deepseek.com/news/news260424">DeepSeek V4 Preview Release | DeepSeek API Docs</a></li>
<li><a href="https://ollama.com/library/deepseek-v4-flash">deepseek-v4-flash - ollama.com</a></li>

</ul>
</details>

**Discussion**: Commenters praised DeepSeek V4 Flash's cost efficiency, with one user noting it's a 'monster at coding.' However, concerns were raised about Grok silently rerouting models from 4.1 to 4.3 and increasing prices, which was criticized as bad practice. Another comment highlighted the dark phrase 'cost per kill' as disturbingly relevant to AI companies.

**Tags**: `#AI`, `#benchmark`, `#cost efficiency`, `#language models`, `#gaming`

---

<a id="item-17"></a>
## [Volkswagen blocks GrapheneOS users from app](https://discuss.grapheneos.org/d/35949-volkswagen-app?page=3) ⭐️ 7.0/10

Volkswagen has locked its API to only accept Play Protect certified devices, effectively blocking users of GrapheneOS, a privacy-focused Android-based OS, from using its official app. This move restricts user choice and privacy, as GrapheneOS users are forced to either abandon the OS or lose access to Volkswagen's app, highlighting growing corporate control over device compatibility in the automotive industry. The API lock also kills community-driven projects that relied on Volkswagen's API, such as Home Assistant integrations, and the official app is criticized for containing 60% advertisements and 30% features.

hackernews · microtonal · Jun 17, 15:04 · [Discussion](https://news.ycombinator.com/item?id=48571526)

**Background**: GrapheneOS is an open-source mobile OS based on Android that prioritizes security and privacy, often used by users who want to avoid Google services. Play Protect certification is Google's process to verify that devices meet compatibility standards and include proprietary Google apps. By requiring Play Protect certification, Volkswagen ensures its app only runs on devices with Google's full software stack.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GrapheneOS">GrapheneOS</a></li>
<li><a href="https://support.google.com/googleplay/answer/7165974?hl=en">Check & fix Play Protect certification status - Google Play Help</a></li>
<li><a href="https://grapheneos.org/">GrapheneOS: the private and secure mobile OS</a></li>

</ul>
</details>

**Discussion**: Community comments express frustration and disappointment, with users like mooo99 delaying car purchases and aka13_404 noting the loss of community integrations. Some see this as part of a broader trend of automotive companies restricting user freedom.

**Tags**: `#privacy`, `#automotive`, `#Android`, `#GrapheneOS`, `#API access`

---

<a id="item-18"></a>
## [MicroUI: Tiny Immediate-Mode GUI Library in ANSI C](https://github.com/rxi/microui) ⭐️ 7.0/10

MicroUI is a minimal, portable immediate-mode UI library written in ANSI C, designed for easy integration into projects that can display text and handle mouse input. Its extreme minimalism and portability make it ideal for embedded systems, game development, and other resource-constrained environments where a full GUI framework is overkill. The library is noted for being somewhat abandoned, with a known misaligned pointer access bug in the draw call iterator that can cause panics in environments like Zig.

hackernews · peter_d_sherman · Jun 17, 12:04 · [Discussion](https://news.ycombinator.com/item?id=48569205)

**Background**: Immediate-mode GUI (IMGUI) is a design pattern where UI elements are drawn and processed each frame directly from code, without retaining state between frames. This contrasts with retained-mode GUIs that maintain a persistent widget tree. ANSI C refers to the standardized version of C (C89/C90) that ensures maximum portability across compilers and platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Immediate_mode_GUI">Immediate mode GUI</a></li>
<li><a href="https://en.wikipedia.org/wiki/ANSI_C">ANSI C</a></li>

</ul>
</details>

**Discussion**: Community members praise MicroUI for its minimalism and ease of integration, with one user calling it their go-to for toy projects. However, concerns about its abandoned status and the pointer alignment bug are noted, with some users forking the project to address issues.

**Tags**: `#C`, `#UI Library`, `#Immediate Mode GUI`, `#Portability`, `#Open Source`

---

<a id="item-19"></a>
## [Photobucket Demands $5 to Retrieve Your Own Photos](https://www.lutr.dev/want-your-images-back-sure-that-ll-be-5-dollars) ⭐️ 7.0/10

Photobucket is charging users a $5 subscription fee to download their own images before account deletion, effectively holding data hostage. This practice raises serious concerns about data portability and corporate ethics, as users are forced to pay to access their own content, potentially setting a dangerous precedent for cloud storage services. The fee is required even for users who only want to retrieve a few old images, and the account deletion notice gives no prior warning of this charge.

hackernews · lutr · Jun 17, 13:05 · [Discussion](https://news.ycombinator.com/item?id=48569954)

**Background**: Data portability is the concept that users should be able to easily transfer their data between services. Photobucket, once a popular image hosting site, has faced criticism before for monetization tactics, such as requiring a $99 annual subscription for third-party image embedding in 2017.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Photobucket">Photobucket - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Data_portability">Data portability</a></li>

</ul>
</details>

**Discussion**: Commenters expressed outrage, with some suggesting chargebacks or noting that closing the account may offer a free download option. Others debated whether this is corporate greed or a necessary survival move for a failing service.

**Tags**: `#data portability`, `#cloud storage`, `#consumer rights`, `#tech ethics`

---

<a id="item-20"></a>
## [Datasette 1.0a34 Adds CRUD UI for Rows](https://simonwillison.net/2026/Jun/16/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a34 introduces insert, edit, and delete row functionality directly in the web interface, available on table pages and row pages. This long-overdue feature brings basic CRUD operations to the Datasette UI, making it more accessible for non-technical users and reducing reliance on external tools or SQL queries. The feature was inspired by Datasette Agent, an AI assistant that already supported SQL write operations, highlighting the gap in the regular UI. Edit and delete actions are also available on the row page.

rss · Simon Willison · Jun 16, 21:31

**Background**: Datasette is an open-source tool for exploring and publishing data, primarily working with SQLite databases. Previously, modifying data required SQL queries or external plugins like datasette-write-ui. This alpha release integrates CRUD natively, moving toward the 1.0 stable release.

<details><summary>References</summary>
<ul>
<li><a href="https://agent.datasette.io/">Datasette Agent: an AI assistant for Datasette to help explore and analyze data in SQLite</a></li>
<li><a href="https://datasette.io/">Datasette: An open source multi-tool for exploring and publishing data</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#open-source`, `#data management`, `#release`

---

<a id="item-21"></a>
## [Georgi Gerganov Endorses Qwen3.6-27B for Local Coding](https://simonwillison.net/2026/Jun/16/georgi-gerganov/#atom-everything) ⭐️ 7.0/10

Georgi Gerganov, creator of llama.cpp, publicly endorsed the Qwen3.6-27B model as a highly capable local coding assistant, stating he uses it almost daily on his M2 Ultra and RTX 5090 systems. He described his lightweight setup using the pi agent harness with a stripped-down configuration and a short system prompt. This endorsement from a key figure in local LLM infrastructure validates Qwen3.6-27B as a practical tool for developers, potentially accelerating adoption of local coding agents. It highlights the growing viability of running capable models on consumer hardware, reducing reliance on cloud-based AI services. Qwen3.6-27B is a dense 27B parameter model that outperforms the much larger Qwen3.5-397B-A17B on major coding benchmarks like SWE-bench Verified (77.2% vs. lower). Gerganov uses it with the pi agent harness in offline mode (pi -nc --offline) and a custom system prompt from the llama.cpp repository.

rss · Simon Willison · Jun 16, 16:04

**Background**: Local LLMs allow developers to run AI models on their own hardware without sending data to external servers, enhancing privacy and reducing latency. Qwen3.6-27B is a recent model from Alibaba's Qwen team, optimized for coding tasks. The pi agent is a minimal terminal-based coding agent harness that supports tool use and file editing. llama.cpp, created by Gerganov, is a popular open-source library for running LLMs efficiently on consumer hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/Qwen/Qwen3.6-27B">Qwen/Qwen3.6-27B · Hugging Face</a></li>
<li><a href="https://qwen.ai/blog?id=qwen3.6-27b">Qwen3.6-27B: Flagship-Level Coding in a 27B Dense Model</a></li>
<li><a href="https://pi.dev/">Pi Coding Agent</a></li>

</ul>
</details>

**Tags**: `#local LLM`, `#coding assistant`, `#Qwen`, `#llama.cpp`, `#AI tools`

---

<a id="item-22"></a>
## [Anthropic surpasses OpenAI in enterprise AI market share](https://techcrunch.com/2026/06/16/anthropics-latest-feud-with-the-trump-admin-may-actually-help-it-sales-data-suggests/) ⭐️ 7.0/10

In May 2026, Anthropic's enterprise AI subscription share reached 41%, surpassing OpenAI's 39.5%, according to Ramp data, despite the Trump administration forcing Anthropic to remove its latest Mythos 5 and Fable 5 models over export control concerns. This marks a significant shift in the enterprise AI market, where OpenAI has long been dominant, and suggests that regulatory conflicts may paradoxically boost sales by increasing brand visibility and trust among enterprise customers. The data comes from Ramp's AI Index, which tracks spending by over 70,000 U.S. businesses; the month Anthropic was flagged as a supply chain risk by the Department of Defense saw its highest enterprise adoption, and the impact of the model removal on IPO prospects remains uncertain.

telegram · zaihuapd · Jun 17, 09:30

**Background**: Anthropic is an AI safety company that develops the Claude family of models. In June 2026, it released two advanced models: Claude Mythos 5, a 10-trillion-parameter model, and Claude Fable 5, a safer version for general use. However, the Trump administration ordered their removal due to export control concerns, citing risks of non-US access.

<details><summary>References</summary>
<ul>
<li><a href="https://ramp.com/data/ai-index">Ramp AI Index</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Enterprise`, `#Market Share`, `#Regulation`, `#Anthropic`

---

<a id="item-23"></a>
## [WeChat Pay Launches AI-Exclusive Card with Per-Transaction Authorization](https://mp.weixin.qq.com/s/WJSr9J0-7LWx2haEZGLmXw) ⭐️ 7.0/10

WeChat Pay officially launched the AI-exclusive card on June 17, 2026, enabling users to make purchases through AI agents with user authorization required for each transaction. The feature is first integrated with Tencent's enterprise agent WorkBuddy via Meituan's life assistant service. This marks a significant step in AI agent payments, addressing security concerns by isolating funds and requiring per-transaction approval. It could accelerate the adoption of AI-driven commerce while maintaining user control, influencing the broader fintech and AI ecosystem. The AI-exclusive card is fully isolated from the main WeChat Pay account; users can top up funds and set usage limits. Each transaction requires the user's final confirmation, and the AI cannot access funds without authorization.

telegram · zaihuapd · Jun 17, 11:32

**Background**: AI agent payments allow intelligent agents to initiate and complete transactions on behalf of users under preset rules. WeChat Pay's solution follows similar moves by competitors like Alipay, which reported 300 million AI payment transactions in May 2026. The AI-exclusive card provides a dedicated balance and authorization mechanism to prevent misuse.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260617A0806300">微信支付发布“AI专属卡”，AI可以帮你花钱了_腾讯新闻</a></li>
<li><a href="https://news.qq.com/rain/a/20260617A05V4J00">微信支付全新上线 AI 专属卡功能_腾讯新闻</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2026-06-17/doc-inictaer7031010.shtml">微信支付正式发布AI专属卡！WorkBuddy率先接入：单独余额 不怕乱花钱_...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Fintech`, `#WeChat Pay`, `#Payment`, `#Security`

---

<a id="item-24"></a>
## [Chinese Telecom Token Plans Shock Developers with High Costs](https://mp.weixin.qq.com/s/UsHNZNMov1kwFQKAVsQHNw) ⭐️ 7.0/10

A recent test by reporters found that a 15 yuan token plan containing 6 million tokens was exhausted in under an hour, with a simple query like 'hello' consuming about 50,000 tokens. Developers estimate monthly costs around 1,000 yuan, five to six times more than mainstream AI subscriptions. This reveals that Chinese telecom operators' token-based pricing is currently impractical and uncompetitive, potentially hindering AI adoption among developers. It highlights the gap between traditional telecom billing and the needs of the AI ecosystem. The token plans include both operators' self-developed models and third-party models like DeepSeek-V4-Flash and GLM-5. Customer service staff at physical stores and online are generally unfamiliar with the new plans, indicating poor rollout execution.

telegram · zaihuapd · Jun 17, 12:25

**Background**: Token-based pricing is a standard billing method for large language models, where each token represents a unit of text processed. Telecom operators are attempting to enter the AI market by offering token plans, similar to how they sell data plans, but face competition from cloud providers and specialized AI platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://wallstreetcn.com/articles/3774930">15元买数百万Token...</a></li>
<li><a href="http://m.ce.cn/cy/202606/t20260612_3027162.shtml">词 元 套 餐 便利数字生活_中国经济网</a></li>
<li><a href="https://www.tmtpost.com/8007698.html">AI算力消耗不再管不住， 词 元 服务迎新玩家-钛媒体官方网站</a></li>

</ul>
</details>

**Discussion**: In the Telegram channel, developers expressed frustration over the high costs and poor implementation, with some calling the plans a 'scam' and questioning the operators' understanding of AI needs. The sentiment is largely negative, with few seeing value in the current offerings.

**Tags**: `#AI pricing`, `#telecom`, `#token economy`, `#China`, `#developer experience`

---

<a id="item-25"></a>
## [OpenAI Codex Now Supports Custom Third-Party Model Providers](https://developers.openai.com/codex/config-advanced) ⭐️ 7.0/10

OpenAI Codex has introduced support for custom third-party model providers, allowing users to configure external models such as Amazon Bedrock, Azure, and local Ollama via a configuration file. This update significantly increases flexibility for developers, enabling them to choose from a wider range of AI models and integrate them seamlessly into their coding workflows, reducing dependency on OpenAI's own models. Users define the provider name, endpoint URL, and API key in a configuration file, and can override settings via command line for quick model switching in terminal environments.

telegram · zaihuapd · Jun 17, 13:58

**Background**: OpenAI Codex is an AI-powered tool that assists with code generation and completion. Previously, it only worked with OpenAI's proprietary models. This change allows developers to leverage local models like Ollama, which runs models locally for lower latency and cost, or cloud services like Amazon Bedrock, which provides access to various foundation models.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/@bluudit/deploy-llms-locally-with-ollama-your-complete-guide-to-local-ai-development-ba60d61b6cea">Deploy LLMs Locally with Ollama: Your Complete Guide to Local AI Development | by Vijay Kumar Maurya | Medium</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amazon_Bedrock">Amazon Bedrock - Wikipedia</a></li>
<li><a href="https://docs.aws.amazon.com/bedrock/latest/userguide/what-is-bedrock.html">Overview - Amazon Bedrock</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI`, `#model-providers`, `#developer-tools`

---