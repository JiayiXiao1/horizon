---
layout: default
title: "Horizon Summary: 2026-06-10 (EN)"
date: 2026-06-10
lang: en
---

> From 33 items, 16 important content pieces were selected

---

1. [Anthropic Releases Claude 3.5 Sonnet with Safety Restrictions](#item-1) ⭐️ 9.0/10
2. [Let's Encrypt Bans Certificates in US-Sanctioned Territories](#item-2) ⭐️ 9.0/10
3. [npm v12 Breaking Changes: Security Fixes and Defaults](#item-3) ⭐️ 8.0/10
4. [Recreating 1990s Software Renderer with Raycasting](#item-4) ⭐️ 8.0/10
5. [FCC Proposes ID Requirement to Eliminate Burner Phones](#item-5) ⭐️ 8.0/10
6. [Apple Withholds Siri from EU After Exemption Denied](#item-6) ⭐️ 8.0/10
7. [Apple's AI Strategy: Privacy as a Competitive Edge](#item-7) ⭐️ 8.0/10
8. [Xiaomi's 1T-Parameter Model Hits 1000 Tokens/s Inference](#item-8) ⭐️ 8.0/10
9. [China Plans $295B National Computing Network with Domestic AI Chips](#item-9) ⭐️ 8.0/10
10. [AI Replaces Employees? That's a Bad CEO](#item-10) ⭐️ 7.0/10
11. [Karpathy: AI Software Demand Surges via Jevons Paradox](#item-11) ⭐️ 7.0/10
12. [Apple WWDC 2026: Siri AI with Vision LLMs and Gemini](#item-12) ⭐️ 7.0/10
13. [Z-Library Launches White-Label Mirrors for Branded Login Sites](#item-13) ⭐️ 7.0/10
14. [Alibaba in Talks to Power Data Centers with Small Nuclear Reactors](#item-14) ⭐️ 7.0/10
15. [Zhuque-2 Rocket Launches Satellites for Direct-to-Cell Tests](#item-15) ⭐️ 7.0/10
16. [CNCERT Warns of Jailbreak and Mining Risks in AI Agent Skills](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Anthropic Releases Claude 3.5 Sonnet with Safety Restrictions](https://www.anthropic.com/news/claude-fable-5-mythos-5) ⭐️ 9.0/10

Anthropic has released Claude 3.5 Sonnet (codenamed 'Fable 5'), a new AI model with improved reasoning, coding, and safety features, including restrictions that prevent the model from being used to accelerate competing AI development. This release marks a significant step in AI safety by implementing model-level restrictions against misuse for developing rival AI systems, while also delivering substantial performance improvements that could benefit developers and enterprises. The model is available via Claude Code, Claude.ai, and the web version, and early testers report it handles difficult problems efficiently, sometimes using half the tokens of previous models for similar results.

hackernews · Philpax · Jun 9, 16:58 · [Discussion](https://news.ycombinator.com/item?id=48463808)

**Background**: Claude is a series of large language models developed by Anthropic, trained using 'constitutional AI' to improve ethical compliance. Claude 3.5 Sonnet is the mid-size model in the Claude 3.5 family, positioned between Haiku and Opus, and was first released in June 2024.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_3.5_Sonnet">Claude 3.5 Sonnet</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (language model) - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/news/claude-3-5-sonnet">Introducing Claude 3.5 Sonnet \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Community members report impressive performance on difficult coding and design tasks, with one user noting it 'crunches through very difficult problems' that had been stalled for months. Another tester observed improved frontend design quality and cost efficiency, though some express concern about the safety restrictions potentially limiting legitimate use.

**Tags**: `#AI`, `#LLM`, `#Anthropic`, `#Claude`, `#Safety`

---

<a id="item-2"></a>
## [Let's Encrypt Bans Certificates in US-Sanctioned Territories](https://letsencrypt.org/documents/LE-SA-v1.7-June-04-2026-diff.pdf) ⭐️ 9.0/10

Let's Encrypt has updated its terms of service to prohibit the issuance of SSL/TLS certificates to users in US-sanctioned territories, effective June 4, 2026. This contradicts Let's Encrypt's mission to create a more secure web for everyone, and it could weaken online security and privacy for users in sanctioned regions like Iran, Cuba, and North Korea. The ban applies to any domain or IP address located in a US-sanctioned territory, and violating the terms could result in revocation of all certificates held by the user, even for non-sanctioned domains.

hackernews · piskov · Jun 8, 22:32 · [Discussion](https://news.ycombinator.com/item?id=48453275)

**Background**: Let's Encrypt is a nonprofit certificate authority that provides free X.509 certificates for TLS encryption, aiming to enable HTTPS for every website. US export control laws restrict the distribution of encryption technology to sanctioned countries, forcing Let's Encrypt to comply despite its global public benefit mission.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Let's_Encrypt">Let ' s Encrypt - Wikipedia</a></li>
<li><a href="https://www.lawfaremedia.org/article/how-geoblocking-limits-digital-access-in-sanctioned-states">How Geoblocking Limits Digital Access in Sanctioned States</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration, noting the irony that Let's Encrypt is restricting security tools in regions that most need them. Some suggested the organization could operate a branch outside the US to avoid such restrictions, while others argued this reveals that digital certificates are fundamentally tools of exclusion.

**Tags**: `#Let's Encrypt`, `#US sanctions`, `#internet censorship`, `#SSL/TLS`, `#digital rights`

---

<a id="item-3"></a>
## [npm v12 Breaking Changes: Security Fixes and Defaults](https://github.blog/changelog/2026-06-09-upcoming-breaking-changes-for-npm-v12/) ⭐️ 8.0/10

npm v12 introduces breaking changes including fixing a decade-old vulnerability (CERT VU#319816) and defaulting the allowScripts configuration to off, following pnpm's lead. This update significantly improves the security of the npm ecosystem by preventing malicious lifecycle scripts from running by default, addressing a long-standing supply chain risk. The allowScripts option, when set to off, disables all package lifecycle scripts unless explicitly allowed via an allow list in package.json. The vulnerability fixed was reported 10 years ago and involved arbitrary code execution via npm scripts.

hackernews · plasma · Jun 9, 21:01 · [Discussion](https://news.ycombinator.com/item?id=48467705)

**Background**: npm lifecycle scripts (e.g., preinstall, postinstall) are commands that run automatically when a package is installed. Malicious actors have exploited these scripts to execute arbitrary code, leading to supply chain attacks. pnpm introduced a similar allowScripts feature 18 months ago.

<details><summary>References</summary>
<ul>
<li><a href="https://www.npmjs.com/package/@lavamoat/allow-scripts">@lavamoat/allow-scripts - npm</a></li>
<li><a href="https://cheatsheetseries.owasp.org/cheatsheets/NPM_Security_Cheat_Sheet.html">NPM Security - OWASP Cheat Sheet Series</a></li>

</ul>
</details>

**Discussion**: The community largely welcomed the security improvements, with users noting the decade-old vulnerability fix and praising npm for following pnpm's lead. Some users questioned the allow list behavior and the design of GitHub's 'vibecoded' badges.

**Tags**: `#npm`, `#JavaScript`, `#security`, `#breaking changes`, `#package management`

---

<a id="item-4"></a>
## [Recreating 1990s Software Renderer with Raycasting](https://staniks.github.io/articles/catlantean-3d-blog-1/) ⭐️ 8.0/10

A detailed article walks through building a retro software renderer from scratch, featuring raycasting, textured floors and ceilings, and gibs, mimicking the style of early 1990s games like Wolfenstein 3D. This deep dive preserves and teaches classic rendering techniques that were foundational to the first-person shooter genre, offering modern developers insight into performance constraints and creative solutions of the era. The renderer uses a raycasting approach with perpendicular walls and constant floor/ceiling height, similar to Wolfenstein 3D, but adds textured floors and ceilings. It also includes a gib system for dismemberment effects.

hackernews · sklopec · Jun 9, 10:46 · [Discussion](https://news.ycombinator.com/item?id=48459294)

**Background**: Raycasting is a fast semi-3D rendering technique used in early games like Wolfenstein 3D, where rays are cast from the player's view to determine wall distances. Unlike true 3D raytracing, raycasting is computationally cheap and was real-time on 1990s hardware. Software rendering means all graphics calculations are done by the CPU without GPU acceleration.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Ray_casting">Ray casting - Wikipedia</a></li>
<li><a href="https://lodev.org/cgtutor/raycasting.html">Raycasting - Lode V</a></li>
<li><a href="https://lodev.org/cgtutor/raycasting2.html">Raycasting II: Floor and Ceiling - Lode V</a></li>

</ul>
</details>

**Discussion**: Commenters noted the renderer's similarity to Wolfenstein 3D's engine, with one pointing out that Doom used a more flexible BSP engine. Another shared a technique for adding lightmaps to textures for dynamic lighting effects like flickering torches.

**Tags**: `#retro graphics`, `#software rendering`, `#raycasting`, `#game development`, `#computer history`

---

<a id="item-5"></a>
## [FCC Proposes ID Requirement to Eliminate Burner Phones](https://www.404media.co/fcc-wants-to-kill-burner-phones-by-forcing-telecoms-to-get-all-customers-ids/) ⭐️ 8.0/10

The FCC has proposed a new rule requiring telecommunications companies to collect identification from all customers, effectively banning anonymous prepaid phones known as burner phones. This proposal could eliminate a key privacy tool for journalists, activists, and ordinary citizens, while raising serious concerns about data security and government surveillance. The rule would require telecoms to verify customer identities at the point of sale, similar to mandatory SIM registration laws already in place in 155 countries. Comments can be submitted to the FCC via their Electronic Comment Filing System.

hackernews · berlianta · Jun 9, 15:21 · [Discussion](https://news.ycombinator.com/item?id=48462308)

**Background**: Burner phones are prepaid mobile devices purchased without identification, often used for short-term communication to protect privacy. They are legal and commonly used by journalists, whistleblowers, and individuals concerned about surveillance. The FCC regulates interstate and international communications in the U.S.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Burner_phones">Burner phones</a></li>

</ul>
</details>

**Discussion**: Commenters expressed strong opposition, citing distrust of telecoms' ability to secure personal data, with one user sharing a personal experience of AT&T data breach. Others noted that many countries already require ID for SIM cards, but argued that the U.S. should not follow suit without strong privacy protections.

**Tags**: `#privacy`, `#telecom regulation`, `#FCC`, `#surveillance`, `#civil liberties`

---

<a id="item-6"></a>
## [Apple Withholds Siri from EU After Exemption Denied](https://www.reuters.com/business/apple-failed-make-its-ai-tool-comply-eu-regulations-eu-commission-says-2026-06-09/) ⭐️ 8.0/10

Apple has decided not to roll out its enhanced Siri AI features in the European Union after EU regulators denied its request for an 18-month exemption from the Digital Markets Act (DMA). This decision highlights the growing tension between big tech innovation and strict EU privacy regulations, potentially putting Apple at a competitive disadvantage in the European market and affecting millions of users who will miss out on advanced AI features. Apple argued that DMA rules hinder its ability to ensure privacy and security for Siri AI, which relies on on-device processing and Private Cloud Compute. The EU countered that Apple failed to demonstrate how its request met the legal criteria for exemption under DMA Article 10.

hackernews · flanged · Jun 9, 16:13 · [Discussion](https://news.ycombinator.com/item?id=48463024)

**Background**: The Digital Markets Act (DMA) is an EU law aimed at making digital markets fairer and more contestable by imposing obligations on large platforms. Apple's Siri AI features, announced for iOS 27 and iPadOS 27, are designed to be private by design, using on-device processing and Private Cloud Compute. Apple requested an 18-month exemption from certain DMA obligations to roll out Siri AI, but the EU rejected it, citing non-compliance.

<details><summary>References</summary>
<ul>
<li><a href="https://telecom.economictimes.indiatimes.com/news/devices/eu-rejects-apples-request-for-siri-ai-exemption-citing-compliance-issues/131622377">Digital Markets Act: EU Rejects Apple's Request for Siri AI Exemption ...</a></li>
<li><a href="https://www.apple.com/newsroom/2026/06/due-to-dma-siri-ai-delayed-in-eu-for-ios-27-and-ipados-27/">Due to DMA, Siri AI delayed in EU for iOS 27 and iPadOS 27 - Apple</a></li>
<li><a href="https://www.bloomberg.com/news/articles/2026-06-08/apple-delays-siri-ai-for-iphone-users-in-eu-says-regulators-refusing-to-engage">Apple Delays Siri AI for iPhone Users in EU , Says Regulators ...</a></li>

</ul>
</details>

**Discussion**: Comments are mixed: some users support Apple's stance, arguing that EU regulations create a backdoor to user data, while others criticize Apple for blaming the EU and prefer a more open platform. Some European users see an opportunity for local alternatives, and a few express willingness to accept a less smart phone rather than see the EU bow to big tech.

**Tags**: `#Apple`, `#EU regulation`, `#privacy`, `#AI`, `#Siri`

---

<a id="item-7"></a>
## [Apple's AI Strategy: Privacy as a Competitive Edge](https://stratechery.com/2026/the-iphones-last-stand/) ⭐️ 8.0/10

Stratechery's analysis argues that Apple's focus on on-device AI processing and privacy, rather than cloud-based AI, may be a strategic advantage despite perceptions of falling behind competitors like Microsoft and Meta. This analysis challenges the narrative that Apple is losing the AI race, suggesting its privacy-centric local AI architecture could become a key differentiator as concerns over data privacy grow. The article highlights Apple's local AI architecture, including on-device processing and private cloud compute, as technically advanced compared to competitors' cloud-dependent approaches.

hackernews · swolpers · Jun 9, 10:08 · [Discussion](https://news.ycombinator.com/item?id=48459001)

**Background**: Apple has historically prioritized user privacy, integrating it into product design. In the AI era, while competitors like Microsoft and Meta push cloud-based AI services, Apple has developed on-device AI capabilities and a private cloud infrastructure to process requests without exposing user data.

**Discussion**: Commenters debated whether Apple's local AI approach is truly superior, with some arguing that cloud-based AI offers more power and flexibility, while others praised Apple's privacy-first design as a long-term advantage.

**Tags**: `#Apple`, `#AI`, `#hardware`, `#privacy`, `#strategy`

---

<a id="item-8"></a>
## [Xiaomi's 1T-Parameter Model Hits 1000 Tokens/s Inference](https://platform.xiaomimimo.com/docs/en-US/model-intro/mimo-v2.5-pro-ultraspeed) ⭐️ 8.0/10

Xiaomi released MiMo-V2.5-Pro-UltraSpeed, a 1-trillion-parameter model achieving 1000 tokens/s inference speed on general GPUs through FP4 mixed-precision quantization and DFlash speculative decoding. This breakthrough enables trillion-parameter models to be deployed in latency-sensitive applications like quantitative trading and real-time risk control, potentially expanding the use of large models in high-frequency decision-making scenarios. The API trial price is about 3 times that of the standard MiMo-V2.5-Pro, while speed is roughly 10 times faster. The trial runs from June 9 to 23, with an application-based approval system, limited to 10 queues per day and 30 minutes per session, prioritizing enterprise users.

telegram · zaihuapd · Jun 9, 03:26

**Background**: FP4 quantization uses 4-bit floating-point numbers to reduce model size and accelerate computation, while speculative decoding uses a smaller draft model to propose multiple tokens that a larger target model verifies in parallel, reducing latency without sacrificing output quality. TileRT is a tile-level runtime engine for ultra-low-latency LLM inference, optimized for specific hardware like B200 GPUs.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>
<li><a href="https://en.wikipedia.org/wiki/Speculative_decoding">Speculative decoding</a></li>
<li><a href="https://github.com/tile-ai/TileRT">GitHub - tile -ai/ TileRT : Tile -Based Runtime for Ultra-Low-Latency LLM...</a></li>

</ul>
</details>

**Tags**: `#AI/ML`, `#model inference`, `#quantization`, `#Xiaomi`, `#large language model`

---

<a id="item-9"></a>
## [China Plans $295B National Computing Network with Domestic AI Chips](https://www.scmp.com/tech/big-tech/article/3353891/china-ramps-building-national-computing-power-network-ai-token-demand-surges) ⭐️ 8.0/10

China plans to invest approximately 2 trillion yuan ($295 billion) over five years (2026–2030) to build a national computing power network, with state-owned telecom operators managing major facilities and prioritizing domestic AI chips from suppliers like Huawei for at least 80% of the infrastructure. This massive investment underscores China's strategic push to reduce reliance on US chip suppliers like Nvidia and AMD, while creating a unified computing resource pool that could accelerate AI adoption across industries and strengthen national AI competitiveness. The plan is part of Beijing's broader 'Six Networks' infrastructure initiative, and telecom operators like China Telecom and China Unicom have already launched 'token packages' that sell computing power in a manner similar to mobile data plans, making high-performance computing more accessible to enterprises and the public.

telegram · zaihuapd · Jun 9, 10:09

**Background**: China's 'Six Networks' initiative encompasses six major infrastructure networks including new power grids, underground pipelines, and computing networks. The computing power network aims to integrate scattered regional computing resources into a unified national system. Token-based pricing, where computing power is measured in tokens (similar to tokens used in AI models), is a novel approach to commoditize computing resources for broader consumption.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260609A07IZQ00">一文详解2万亿AI基础设施计划，历史以来规模最大，80%国产</a></li>
<li><a href="https://www.gov.cn/yaowen/liebiao/202605/content_7069999.htm">我国将抓紧出台“六张网”相关规划和实施方案__中国政府网</a></li>
<li><a href="https://www.guandian.cn/article/20260422/556949.html">中国移动北京公司推出个人 算 力 Token 套 餐 最低5.99元起 - 观点网</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#China tech`, `#computing power`, `#chip independence`, `#national network`

---

<a id="item-10"></a>
## [AI Replaces Employees? That's a Bad CEO](https://www.techdirt.com/2026/06/09/ceos-who-think-ai-replaces-their-employees-are-just-bad-ceos/) ⭐️ 7.0/10

A Techdirt opinion piece argues that CEOs who view AI as a replacement for employees misunderstand AI's limitations and the value of human workers, drawing on decades of shipping and support experience. This perspective challenges the prevailing narrative of AI-driven job displacement, emphasizing that human judgment, support, and shipping expertise remain irreplaceable. It sparks debate on how companies should responsibly integrate AI. The author uses the analogy that shipping a product is far more complex than designing it, and AI cannot handle the nuanced, real-world challenges of delivery and support. The article has 165 comments and a score of 413 points on Techdirt.

hackernews · speckx · Jun 9, 18:45 · [Discussion](https://news.ycombinator.com/item?id=48465675)

**Background**: The article is a response to the growing trend of companies using AI to automate tasks and replace workers. It argues that many CEOs underestimate the human effort required in product shipping and customer support, areas where AI currently falls short.

**Discussion**: Commenters largely agree with the article, with some adding that bad CEOs often lack the skills to do their jobs well. One commenter suggests that CEOs should first replace their own assistants with AI before replacing others, while another quips that AI might actually be good at replacing CEOs themselves.

**Tags**: `#AI`, `#management`, `#employment`, `#technology-critique`

---

<a id="item-11"></a>
## [Karpathy: AI Software Demand Surges via Jevons Paradox](https://simonwillison.net/2026/Jun/9/andrej-karpathy/#atom-everything) ⭐️ 7.0/10

Andrej Karpathy posted on Twitter (via Claude Fable 5) that as AI generates working software on demand, his personal demand for custom applications has grown substantially, citing Jevons paradox. This insight from a leading AI figure suggests that AI-driven software generation will not reduce the need for developers but instead massively increase demand for bespoke applications, reshaping the software industry. Karpathy specifically mentions examples like explainers, visualizers, dashboards, and a hyper-specific wandb clone for a single project, illustrating the breadth of new possibilities.

rss · Simon Willison · Jun 9, 19:03

**Background**: Jevons paradox, first observed in 1865, describes how increased efficiency in resource use can lead to higher overall consumption. In this context, AI makes software generation more efficient, lowering the cost of creating custom applications, which paradoxically increases total demand for software rather than reducing it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Jevons_paradox">Jevons paradox</a></li>
<li><a href="https://github.com/wandb/wandb">GitHub - wandb/wandb: The AI developer platform. Use Weights ... wandb · PyPI wandb (Weights and Biases) - Hugging Face wandb安装与使用 —— 用于跟踪、可视化和协作机器学习实验的工具-CSDN... 新手教程|如何使用 WandB 监控大模型的训练与调试 quickstart - W&B</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software development`, `#Jevons paradox`, `#generative AI`

---

<a id="item-12"></a>
## [Apple WWDC 2026: Siri AI with Vision LLMs and Gemini](https://simonwillison.net/2026/Jun/8/wwdc/#atom-everything) ⭐️ 7.0/10

At WWDC 2026, Apple announced new Siri AI features that leverage vision LLMs to extract information from the user's screen and license a custom Gemini-derived model for complex reasoning tasks, running on Private Cloud Compute infrastructure extended to Google Cloud with NVIDIA GPUs. This marks a more feasible approach to Apple's AI ambitions compared to overhyped 2024 promises, potentially enabling deeper on-device and cloud AI integration without requiring every app to write custom code. The new Core AI library bridges PyTorch and Apple hardware via Core AI PyTorch Extensions, allowing developers to run their own models. The Gemini models on PCC use Google Cloud with NVIDIA GPUs, and Apple publishes all binaries for public inspection.

rss · Simon Willison · Jun 8, 23:58

**Background**: Apple's 2024 Apple Intelligence announcements were criticized for being overly ambitious and underdelivering. Vision LLMs, which can understand visual content from screens, were less mature in 2024 but have since advanced. Private Cloud Compute (PCC) is Apple's secure cloud infrastructure for AI inference, now extended to Google Cloud.

<details><summary>References</summary>
<ul>
<li><a href="https://security.apple.com/blog/expanding-pcc/">Expanding Private Cloud Compute - Apple Security Research</a></li>

</ul>
</details>

**Discussion**: Simon Willison expresses cautious optimism, noting the feasibility improvements but maintaining a 'I'll believe it when I see it' stance due to past overpromises. He highlights the strategic use of vision LLMs and Gemini licensing as pragmatic steps.

**Tags**: `#Apple`, `#Siri`, `#AI`, `#WWDC`, `#Vision LLM`

---

<a id="item-13"></a>
## [Z-Library Launches White-Label Mirrors for Branded Login Sites](https://torrentfreak.com/z-library-lets-people-run-white-label-login-only-pirate-mirrors/) ⭐️ 7.0/10

Z-Library has introduced a white-label mirror feature that allows users to create branded, login-only mirror sites with no Z-Library branding, and operators receive 20% of donations in cryptocurrency. This feature decentralizes access to Z-Library, making it harder for copyright enforcers to identify and block mirrors, and it incentivizes community participation through revenue sharing. Mirror operators receive 20% of donations via cryptocurrency, and Z-Library also provides an offline domain list file for users to store all access points locally in case of a total ban.

telegram · zaihuapd · Jun 9, 05:55

**Background**: Z-Library is a shadow library project that provides free access to millions of books and academic articles, often facing legal challenges and domain seizures. White-label mirrors allow third parties to host branded versions of the site, obscuring its origin and making enforcement more difficult.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Z-Library">Z-Library</a></li>

</ul>
</details>

**Tags**: `#Z-Library`, `#piracy`, `#digital rights`, `#anti-censorship`, `#mirroring`

---

<a id="item-14"></a>
## [Alibaba in Talks to Power Data Centers with Small Nuclear Reactors](https://www.stcn.com/article/detail/3950643.html) ⭐️ 7.0/10

Alibaba has approached a state-owned nuclear power company to discuss building small modular reactors (SMRs) to power its Hangzhou Renhe data center, with negotiations focusing on electricity pricing and supply models. This move signals a major trend where tech giants turn to nuclear energy to meet the surging electricity demand from AI workloads, potentially reshaping data center energy strategies globally. The SMR under consideration is likely based on China National Nuclear Corporation's 'Linglong One' (ACP100), the world's first SMR to pass IAEA safety review, scheduled for commercial operation in 2026.

telegram · zaihuapd · Jun 9, 10:54

**Background**: Small modular reactors (SMRs) are advanced nuclear reactors with a power capacity of up to 300 MW(e) per unit, designed for factory fabrication and modular deployment. They offer stable, carbon-free power suitable for data centers. Tech giants like Meta, Amazon, and Google have also been exploring SMRs for their energy needs.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260609A02R4U00">阿里巴巴接洽核电央企 探讨小型反应堆为数据中心供电</a></li>
<li><a href="https://www.163.com/dy/article/KV0I40EP05118I96.html">阿里洽谈小型核反应堆为数据中心供电|电厂|核电站|阿里巴巴集团|新型...</a></li>
<li><a href="http://www.cb.com.cn/index/show/jj/cv/cv135401422062">阿里巴巴接洽核电央企 探讨小型反应堆为数据中心供电</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#nuclear energy`, `#data centers`, `#Alibaba`, `#energy`

---

<a id="item-15"></a>
## [Zhuque-2 Rocket Launches Satellites for Direct-to-Cell Tests](https://www.news.cn/20260609/4958e6730eba485fae66a56a5b21458a/c.html) ⭐️ 7.0/10

On June 9, 2025, the Zhuque-2 improved Y6 rocket successfully launched the Qianfan DTC01 satellite and China Mobile 02 satellite into orbit, which will conduct tests for direct-to-cell broadband and space-ground network integration. This mission marks a significant step in Chinese commercial spaceflight and satellite internet development, as direct-to-cell technology could enable ubiquitous connectivity without specialized terminals, potentially competing with Starlink's direct-to-cell services. The Zhuque-2 Y6 is a two-stage cryogenic liquid rocket with a diameter of 3.35 meters and a payload capacity of 6 tons to low Earth orbit. The Qianfan DTC01 satellite is operated by Shanghai Yuanxin, while China Mobile 02 will verify direct-to-cell broadband technologies.

telegram · zaihuapd · Jun 9, 14:20

**Background**: The Zhuque-2 is a liquid-fueled rocket developed by Chinese private company LandSpace. Direct-to-cell satellite technology allows standard smartphones to connect directly to satellites, eliminating the need for bulky satellite phones. The Qianfan constellation (also known as G60 Starlink) is a Chinese low-Earth orbit satellite internet project aiming to deploy over 15,000 satellites for global coverage.

<details><summary>References</summary>
<ul>
<li><a href="https://user.guancha.cn/main/content?id=1667424">朱 雀 二 号 改进型遥六运载 火 箭 发射成功_风闻</a></li>
<li><a href="https://wap.eastmoney.com/a/202606093765229138.html">朱 雀 二 号 遥六发射成功 将开展手机直连卫星试验 _ 东方财富网</a></li>
<li><a href="https://www.thecover.cn/news/pkGxb4dKuoeH90qSdq8Jkw==">朱 雀 二 号 遥六发射成功，千帆DTC01星等两颗卫星顺利入轨 - 封面新闻</a></li>

</ul>
</details>

**Tags**: `#spaceflight`, `#satellite`, `#telecommunications`, `#aerospace`

---

<a id="item-16"></a>
## [CNCERT Warns of Jailbreak and Mining Risks in AI Agent Skills](https://www.yicai.com/brief/103222242.html) ⭐️ 7.0/10

China's CNCERT issued an official warning on June 9, 2026, stating that some AI agent skill packs (Skills) are being distributed under the guise of 'large model jailbreak' and 'mining for money', which can bypass model safety restrictions or hijack device resources for illegal cryptomining. This warning highlights a new attack vector in the AI ecosystem, where seemingly useful skill packs can compromise user security and system integrity. It underscores the urgent need for stricter vetting of third-party AI agent extensions, affecting millions of users and developers. The malicious Skills can cause models to generate illegal content, lead to account bans, degrade device performance, and even involve users in money laundering. CNCERT urges users and operators to review skill sources, monitor behavior, and remove suspicious components.

telegram · zaihuapd · Jun 9, 16:58

**Background**: AI agent skill packs (Skills) are modular extensions that enhance the capabilities of large language model (LLM) based agents, such as data analysis or document generation. 'Jailbreak' refers to techniques that trick LLMs into bypassing their safety guardrails, while 'cryptomining' involves using a device's computing power to mine cryptocurrency without consent. CNCERT is China's national cybersecurity emergency response center.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KV0LQF7205198CJN.html">国家互联网应急中心：部分智能体技能包（Skills）存在越狱和挖矿风险...</a></li>
<li><a href="https://www.nbd.com.cn/articles/2026-06-09/4421403.html">国家互联网应急中心提醒：部分智能体技能包（Skills）存在越狱和挖矿...</a></li>
<li><a href="https://finance.eastmoney.com/a/202606093765264792.html">国家互联网应急中心提醒：部分智能体技能包（Skills）存在越狱和挖矿...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#cybersecurity`, `#large language models`, `#cryptomining`, `#jailbreak`

---