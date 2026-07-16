---
layout: default
title: "Horizon Summary: 2026-07-16 (EN)"
date: 2026-07-16
lang: en
---

> From 35 items, 20 important content pieces were selected

---

1. [Stripe and Advent Jointly Offer to Acquire PayPal for Over $53 Billion](#item-1) ⭐️ 9.0/10
2. [Thinking Machines Releases Inkling, an Open-Weights Multimodal Model](#item-2) ⭐️ 8.0/10
3. [xAI Open-Sources Grok Build System](#item-3) ⭐️ 8.0/10
4. [Gemma 4 26B runs at 5 tokens/sec on 13-year-old Xeon CPU](#item-4) ⭐️ 8.0/10
5. [Telegram Data Centers: Numbering, Locations, and FSB Ties](#item-5) ⭐️ 8.0/10
6. [Sleep Regularity Tops Duration in Predicting Mortality Risk](#item-6) ⭐️ 8.0/10
7. [Claude web_fetch tool bypass enables data exfiltration via prompt injection](#item-7) ⭐️ 8.0/10
8. [Lobste.rs Migrates from MariaDB to SQLite](#item-8) ⭐️ 8.0/10
9. [Armin Ronacher: Friction Builds Shared Understanding, AI Risks Bypassing It](#item-9) ⭐️ 8.0/10
10. [DeepSeek Raises $7.4B in First Round with Unique Control Structure](#item-10) ⭐️ 8.0/10
11. [Musk: X to Unconditionally Open-Source Entire Codebase](#item-11) ⭐️ 8.0/10
12. [Developer Sandbox Escape Lets Filza Read iOS 27 Notes DB](#item-12) ⭐️ 8.0/10
13. [Telegram Launches Serverless Platform for Bot Backends](#item-13) ⭐️ 8.0/10
14. [Mental Health and Communication in Software Development](#item-14) ⭐️ 7.0/10
15. [Dependabot Defaults to Three-Day Cooldown for Version Updates](#item-15) ⭐️ 7.0/10
16. [Cache-friendly uvx usage in GitHub Actions](#item-16) ⭐️ 7.0/10
17. [7 Mobile AI Models Including Apple Intelligence Get China Approval](#item-17) ⭐️ 7.0/10
18. [Chinese Retail Blurs: Sam's, Snack Stores, Pinduoduo Vie for Same Wallet](#item-18) ⭐️ 7.0/10
19. [Judge Questions Epic-Google Antitrust Settlement Over $800M Deal](#item-19) ⭐️ 7.0/10
20. [ASML Plans Price Hikes on EUV and DUV Lithography Equipment](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Stripe and Advent Jointly Offer to Acquire PayPal for Over $53 Billion](https://www.reuters.com/business/finance/stripe-advent-offer-buy-paypal-more-than-53-billion-sources-say-2026-07-15/) ⭐️ 9.0/10

Stripe and private equity firm Advent International have made a joint offer to acquire PayPal for more than $53 billion, according to sources. This acquisition would consolidate two dominant payment platforms, raising significant antitrust concerns and potentially reducing competition in online payments, which could impact millions of businesses and consumers. The deal would bring together Stripe's modern API-based payment infrastructure with PayPal's consumer-facing brands like Venmo and Braintree, creating a combined entity with enormous market power in card-not-present transactions.

hackernews · rvz · Jul 15, 03:32 · [Discussion](https://news.ycombinator.com/item?id=48915953)

**Background**: Stripe is a privately held fintech company valued at around $159 billion, processing over $1.9 trillion in payments in 2025 for 5 million businesses. Advent International is a global private equity firm specializing in buyouts. PayPal, founded in 1998, is a publicly traded company that owns Venmo, Braintree, and Xoom, and has faced increasing competition from Stripe in recent years.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Stripe,_Inc.">Stripe, Inc. - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Advent_International">Advent International - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments express strong concerns about reduced competition, higher fees, and Stripe's restrictive policies on certain industries like cannabis and adult content. Some users worry about the impact on their ability to transmit money and the potential for account freezes, while others question whether the deal will pass antitrust scrutiny.

**Tags**: `#acquisition`, `#payments`, `#antitrust`, `#fintech`, `#Stripe`

---

<a id="item-2"></a>
## [Thinking Machines Releases Inkling, an Open-Weights Multimodal Model](https://thinkingmachines.ai/news/introducing-inkling/) ⭐️ 8.0/10

Thinking Machines has released Inkling, an open-weights multimodal model that supports audio, designed for customization and efficient local inference. Inkling is the largest open-weights model to support audio, enabling enterprises to fine-tune and deploy their own models locally at lower cost, potentially challenging closed-source alternatives. Inkling is available on Tinker for fine-tuning, and community members have already created GGUF and NVFP4 quantized versions for local inference. The model is not the strongest overall but combines multimodal capabilities, efficient thinking, and customization options.

hackernews · vimarsh6739 · Jul 15, 18:12 · [Discussion](https://news.ycombinator.com/item?id=48924912)

**Background**: Open-weights models release trained parameters publicly, allowing anyone to download and run them locally. Multimodal models process multiple data types like text, audio, and images. Local inference runs models on edge devices without cloud dependency, offering privacy and cost benefits.

<details><summary>References</summary>
<ul>
<li><a href="https://opensource.org/ai/open-weights">Open Weights: not quite what you’ve been told</a></li>
<li><a href="https://hai.stanford.edu/ai-definitions/what-is-an-open-weight-model">What is an Open-Weight Model? - Stanford HAI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Multimodal_model">Multimodal model</a></li>

</ul>
</details>

**Discussion**: Commenters are excited about Inkling's audio support and local deployment potential, with some comparing it to DeepSeek and suggesting Thinking Machines could become a key player. Technical links to quantization tools and fine-tuning resources were shared.

**Tags**: `#open-weights`, `#multimodal`, `#AI`, `#machine learning`, `#audio`

---

<a id="item-3"></a>
## [xAI Open-Sources Grok Build System](https://github.com/xai-org/grok-build) ⭐️ 8.0/10

xAI has open-sourced the Grok build system, a Rust-based CLI/TUI tool for their AI agent runtime, on GitHub under the xai-org/grok-build repository. This move allows the community to inspect, modify, and fork the code, potentially improving transparency and trust after a privacy scandal where the tool was found uploading entire directories to xAI's cloud. The codebase includes a self-contained terminal renderer for Mermaid diagrams using Unicode box-drawing, and the repository is synced periodically from xAI's internal monorepo.

hackernews · skp1995 · Jul 15, 20:24 · [Discussion](https://news.ycombinator.com/item?id=48926590)

**Background**: Grok is an AI chatbot developed by xAI, offering voice chat, image/video generation, and advanced reasoning. The CLI tool, part of the Grok ecosystem, faced backlash for uploading user data without consent, prompting xAI to open-source the build system as a damage-control measure.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/xai-org/grok-build">GitHub - xai -org/ grok - build : SpaceXAI's coding agent harness and...</a></li>
<li><a href="https://x.ai/open-source">Grok Build CLI is open source. Browse the code on GitHub. | SpaceXAI</a></li>

</ul>
</details>

**Discussion**: The community response is mixed: some praise the open-sourcing and note interesting technical details like the Mermaid renderer, while others criticize the move as a tactical PR response to the privacy scandal. Forks have already emerged, such as a privacy-focused fork that strips telemetry and blocks auto-updates.

**Tags**: `#open source`, `#AI`, `#Grok`, `#privacy`, `#xAI`

---

<a id="item-4"></a>
## [Gemma 4 26B runs at 5 tokens/sec on 13-year-old Xeon CPU](https://www.neomindlabs.com/2026/06/08/running-gemma-4-26b-at-5-tokens-sec-on-a-13-year-old-xeon-with-no-gpu/) ⭐️ 8.0/10

A technical blog post demonstrates running Google's Gemma 4 26B A4B model at 5 tokens per second on a 13-year-old dual Xeon server without a GPU, using quantization and CPU optimizations. This shows that modern large language models can run on extremely old hardware, lowering the barrier for local AI inference and sparking debate about cost-effectiveness versus cloud APIs. The Gemma 4 26B A4B model is a Mixture-of-Experts architecture with 26B total parameters and 4B active parameters, designed for efficient inference. The setup likely uses 4-bit quantization and CPU-specific optimizations to achieve 5 tokens/sec on a dual Xeon E5-2690 v2 (Ivy Bridge) system.

hackernews · neomindryan · Jul 15, 15:34 · [Discussion](https://news.ycombinator.com/item?id=48922434)

**Background**: Large language models typically require powerful GPUs for fast inference. However, techniques like quantization (reducing numerical precision) and CPU-optimized inference libraries enable running these models on older hardware. Gemma 4 is Google's latest open model family, with the 26B A4B variant balancing size and speed.

<details><summary>References</summary>
<ul>
<li><a href="https://ai.google.dev/gemma/docs/core">Gemma 4 model overview - Google AI for Developers</a></li>
<li><a href="https://huggingface.co/google/gemma-4-26B-A4B-it">google/gemma-4-26B-A4B-it · Hugging Face</a></li>
<li><a href="https://www.intel.com/content/www/us/en/developer/articles/technical/boost-performance-llms-pytorch-xeon-processors-pt2.html">Boost Performance for LLMs Using PyTorch: Part 2 - Intel</a></li>

</ul>
</details>

**Discussion**: Commenters debate the cost efficiency: some note that electricity costs for running such old hardware may exceed cloud API prices, while others highlight the value of local inference for privacy and offline use. A user predicts that by mid-2027, 200B MoE models will run on consumer hardware, citing their own experience running a 35B model on a MacBook Air.

**Tags**: `#LLM`, `#inference optimization`, `#local AI`, `#hardware`, `#cost analysis`

---

<a id="item-5"></a>
## [Telegram Data Centers: Numbering, Locations, and FSB Ties](https://dev.moe/en/3025) ⭐️ 8.0/10

An in-depth analysis reveals Telegram's data center numbering scheme (DC1-5), their locations (Miami, Amsterdam, Singapore), and operational quirks like DC3's mysterious absence and DC5's frequent downtime for Chinese users. This matters because Telegram's infrastructure choices affect user privacy and reliability; the potential FSB overlap raises serious concerns about metadata surveillance and the app's privacy guarantees. Telegram claims five data centers (DC1-5), with DC1 and DC3 in Miami, DC2 and DC4 in Amsterdam, and DC5 in Singapore; DC3 is notably absent from public documentation, and DC5 is often down, affecting Chinese users.

hackernews · theanonymousone · Jul 15, 13:22 · [Discussion](https://news.ycombinator.com/item?id=48920475)

**Background**: Telegram is a cloud-based instant messaging app founded by Pavel and Nikolai Durov in 2013, known for its focus on security and privacy. Its servers are distributed worldwide, with data centers identified by numbers (DC1-5) in code and documentation. Recent investigations by OCCRP and Istories have linked Telegram's infrastructure to a Russian contractor with ties to the FSB, suggesting potential metadata surveillance risks.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.moe/en/3025">Mysteries of Telegram DC - Coxxs</a></li>
<li><a href="https://istories.media/en/stories/2025/06/10/telegram-fsb/">Telegram, the FSB, and the Man in the Middle - istories.media</a></li>
<li><a href="https://en.wikipedia.org/wiki/Telegram_(software)">Telegram (software) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the FSB infrastructure overlap, with a link to an Istories investigation. Users note that DC2 serves Russian and Ukrainian users and is often down, while DC3's absence sparks speculation about special account data. Some question the technical debt of custom data center handling.

**Tags**: `#Telegram`, `#data centers`, `#infrastructure`, `#security`, `#privacy`

---

<a id="item-6"></a>
## [Sleep Regularity Tops Duration in Predicting Mortality Risk](https://academic.oup.com/sleep/article/47/1/zsad253/7280269) ⭐️ 8.0/10

A 2023 study published in *Sleep* found that sleep regularity—consistency of sleep and wake times—is a stronger predictor of all-cause mortality than sleep duration. This shifts the focus from how long you sleep to how consistent your sleep schedule is, offering a modifiable target for improving longevity. It challenges the common emphasis on sleep duration alone in public health guidelines. The study analyzed data from over 60,000 participants in the UK Biobank, using accelerometer-based sleep regularity index (SRI) scores. Regular sleepers had a 20-48% lower mortality risk compared to irregular sleepers, independent of sleep duration.

hackernews · bilsbie · Jul 15, 11:46 · [Discussion](https://news.ycombinator.com/item?id=48919363)

**Background**: Sleep regularity measures the day-to-day consistency of sleep-wake timing, often quantified by the sleep regularity index (SRI). Previous research has largely focused on sleep duration as a key health metric, but this study highlights the importance of circadian alignment. The findings suggest that maintaining a consistent sleep schedule may be more critical than getting a fixed number of hours.

**Discussion**: Commenters discussed potential confounding variables like occupation and shift work, with some noting that the study adjusted for shift work but not for specific occupations. Others shared personal experiences with magnesium supplementation for sleep improvement, while a few criticized the study for being observational and prone to confounding.

**Tags**: `#sleep`, `#health`, `#longevity`, `#research`, `#epidemiology`

---

<a id="item-7"></a>
## [Claude web_fetch tool bypass enables data exfiltration via prompt injection](https://simonwillison.net/2026/Jul/15/claude-web-fetch-exfiltration/#atom-everything) ⭐️ 8.0/10

Researcher Ayush Paul discovered a bypass in Anthropic's Claude web_fetch tool that allowed an attacker to exfiltrate user memories (name, location, employer) via a chain of nested links fetched from a malicious site. Anthropic has since closed the loophole by preventing web_fetch from following links embedded in fetched content. This attack demonstrates that even carefully designed AI safety measures can be circumvented, highlighting the ongoing challenge of securing LLM agents with access to private data and external tools. It underscores the need for robust defenses against indirect prompt injection and data exfiltration in production AI systems. The attack exploited a loophole where web_fetch was allowed to visit URLs embedded in previously fetched pages, enabling a honeypot site to trick the agent into exfiltrating data by following a sequence of generated links. The malicious site only served the attack to clients with 'Claude-User' in their user-agent to evade detection. Anthropic did not pay a bug bounty, claiming they had already internally identified the issue.

rss · Simon Willison · Jul 15, 14:21

**Background**: Prompt injection is a security exploit where malicious inputs cause LLMs to behave unexpectedly. In the 'lethal trifecta' scenario, an LLM with access to private data and a tool to fetch web content can be tricked into exfiltrating data via URLs it visits. Claude's web_fetch tool was designed to only navigate to user-provided URLs or results from its web_search tool, but the nested-link loophole allowed indirect prompt injection to bypass this restriction.

<details><summary>References</summary>
<ul>
<li><a href="https://platform.claude.com/docs/en/agents-and-tools/tool-use/web-fetch-tool">Web fetch tool - Claude Platform Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection_attack">Prompt injection attack</a></li>
<li><a href="https://cdn.openai.com/pdf/dd8e7875-e606-42b4-80a1-f824e4e11cf4/prevent-url-data-exfil.pdf">Preventing URL -Based Data Exfiltration in Language-Model Agents</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters expressed concern about the severity of the vulnerability and criticized Anthropic for not paying a bug bounty despite the researcher's responsible disclosure. Some debated whether the fix fully addresses the root cause, while others praised the technical write-up for its clarity.

**Tags**: `#AI safety`, `#prompt injection`, `#data exfiltration`, `#Claude`, `#security`

---

<a id="item-8"></a>
## [Lobste.rs Migrates from MariaDB to SQLite](https://simonwillison.net/2026/Jul/14/lobsters-sqlite/#atom-everything) ⭐️ 8.0/10

Lobste.rs, a community news site, has completed its migration from MariaDB to SQLite, now running entirely on a single VPS with improved performance and reduced costs. This real-world case study demonstrates that SQLite can serve as a viable primary database for a moderately sized web application, challenging the assumption that a client-server database is always necessary. The migration resulted in a 3.8GB primary SQLite database, along with separate cache, queue, and rack_attack databases. CPU and memory usage dropped, and the site feels snappier, with half the VPS cost after decommissioning the MariaDB server.

rss · Simon Willison · Jul 14, 19:44

**Background**: SQLite is a serverless, embedded relational database engine that stores data in a single file, requiring no separate database server. It is commonly used in mobile apps and small websites, but less frequently as the primary database for multi-user web applications. Lobste.rs is a Rails-based community site for computing discussions, similar to Hacker News.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/lobsters/lobsters">GitHub - lobsters / lobsters : Computing-focused community centered...</a></li>
<li><a href="https://www.sqlitetutorial.net/">SQLite Tutorial - An Easy Way to Master SQLite Fast</a></li>

</ul>
</details>

**Discussion**: The Lobsters community discussion is positive, with the site admin reporting that SQLite passed with flying colors. Commenters share technical details about the migration process and express interest in the architecture.

**Tags**: `#SQLite`, `#database migration`, `#Rails`, `#performance`, `#web architecture`

---

<a id="item-9"></a>
## [Armin Ronacher: Friction Builds Shared Understanding, AI Risks Bypassing It](https://simonwillison.net/2026/Jul/14/armin-ronacher/#atom-everything) ⭐️ 8.0/10

Armin Ronacher argues that shared understanding in software projects is maintained by friction—such as code review and cross-team coordination—which AI coding agents risk bypassing, potentially eroding the collaborative knowledge that keeps systems coherent. As AI agents become more capable of autonomously writing and modifying code, teams may lose the essential human processes that synchronize understanding across contributors, leading to fragmented knowledge and harder-to-maintain systems. Ronacher's essay, 'The Tower Keeps Rising,' highlights that shared language in a project includes unwritten knowledge about concepts, boundaries, invariants, and ownership, which is built through friction like explaining changes to others.

rss · Simon Willison · Jul 14, 18:04

**Background**: Shared understanding in software teams is the collective knowledge of how a system works and why it is designed that way, often tacit and distributed across documentation, code, and conversations. Friction—such as the effort required to coordinate changes—forces developers to communicate and align their mental models, which is crucial for long-term maintainability. AI agents that can make changes without this friction may produce code that works in isolation but undermines team coherence.

<details><summary>References</summary>
<ul>
<li><a href="https://lucumr.pocoo.org/2026/7/13/the-tower-keeps-rising/">Vibecoding and the possible collapse of a shared language.</a></li>
<li><a href="https://www.linkedin.com/pulse/ai-agents-engineering-teams-powerful-tools-yet-andras-ludanyi-9x6ie">AI Agents in Engineering Teams: Powerful Tools, But Not Yet...</a></li>
<li><a href="https://www.ibm.com/think/topics/ai-agents">What Are AI Agents ? | IBM</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#AI agents`, `#collaboration`, `#shared understanding`, `#code review`

---

<a id="item-10"></a>
## [DeepSeek Raises $7.4B in First Round with Unique Control Structure](https://t.me/zaihuapd/42589) ⭐️ 8.0/10

DeepSeek has raised over 50 billion RMB (approximately $7.4 billion) in its first funding round, valuing the company at over $50 billion. The round uses an unconventional structure where investors must invest in a limited partnership managed by CEO Liang Wenfeng, with a five-year lock-up and no voting rights. This massive funding round underscores DeepSeek's rapid rise as a major AI player, challenging global leaders like OpenAI. The unique governance structure allows founder Liang Wenfeng to maintain control while attracting strategic investors like Tencent and CATL, setting a precedent for AI startup financing. Founder Liang Wenfeng personally invested 20 billion RMB in this round. Tencent is considering investing 10 billion RMB, and CATL plans to invest 5 billion RMB, potentially becoming the largest external investors. DeepSeek has not commented on the report.

telegram · zaihuapd · Jul 15, 12:56

**Background**: DeepSeek is a Chinese AI company founded in July 2023 by Liang Wenfeng, who also runs the hedge fund High-Flyer. It gained global attention in January 2025 with its R1 model, which matched GPT-4 performance at a fraction of the cost. The company uses a limited partnership structure, common in China, where the founder as GP retains control while investors as LP have limited rights.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_AI_Research">DeepSeek AI Research</a></li>
<li><a href="https://zh.wikipedia.org/wiki/深度求索">深度求索 - 维基百科，自由的百科全书</a></li>
<li><a href="https://ailegal.baidu.com/legalarticle/qadetail?id=4930dbb9aae194241204">有限合伙企业如何实现控制权 - ailegal.baidu.com</a></li>

</ul>
</details>

**Tags**: `#AI`, `#funding`, `#DeepSeek`, `#startup`, `#governance`

---

<a id="item-11"></a>
## [Musk: X to Unconditionally Open-Source Entire Codebase](https://x.com/elonmusk/status/2077361679034118271) ⭐️ 8.0/10

Elon Musk announced that after completing a security vulnerability review, X will unconditionally open-source its entire codebase and invite third-party reviewers to verify that the running system matches the open-source code. This move could significantly increase transparency and trust in X's platform, setting a new standard for social media companies regarding code openness and independent verification. The open-sourcing will occur after a security vulnerability review, and third-party reviewers will check that the live system matches the open-source code. Musk emphasized that trust from full transparency is the only thing worth believing.

telegram · zaihuapd · Jul 15, 13:32

**Background**: X (formerly Twitter) has been a proprietary platform since its inception. Open-sourcing the entire codebase would allow anyone to inspect, audit, and contribute to the code, potentially improving security and accountability. This announcement follows Musk's broader push for transparency and free speech on the platform.

**Tags**: `#open source`, `#social media`, `#transparency`, `#Elon Musk`, `#X`

---

<a id="item-12"></a>
## [Developer Sandbox Escape Lets Filza Read iOS 27 Notes DB](https://x.com/0xjohnny/status/2077216973256274272) ⭐️ 8.0/10

Developer johnny modified the iOS file manager Filza to exploit a sandbox escape vulnerability on iOS 27 beta 3, allowing the modified tool to access the Notes database on an iPhone 17 Pro Max. This demonstrates a significant security bypass on the latest iOS beta, highlighting ongoing sandbox weaknesses that could be exploited by malicious apps or used for jailbreak development. The exploit targets the app sandbox container restrictions, and the modified Filza can browse external data beyond its own container. The specific vulnerability used has not been disclosed.

telegram · zaihuapd · Jul 15, 14:35

**Background**: Filza is a popular file manager for iOS that normally operates within an app's sandbox. A sandbox escape vulnerability allows an app to break out of its restricted environment and access other apps' data or system files. iOS 27 is the latest major version of Apple's mobile operating system, currently in beta.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tigisoftware.com/default/?page_id=78">Filza – TIGI Software</a></li>
<li><a href="https://medium.com/ssd-secure-disclosure/ios-vulnerabilities-3-sandbox-escape-cves-5233c92ad875">iOS Vulnerabilities — 3 Sandbox Escape CVE’s you should know | by Imriah | SSD Secure Disclosure | Medium</a></li>

</ul>
</details>

**Tags**: `#iOS security`, `#sandbox escape`, `#jailbreak`, `#vulnerability`, `#Filza`

---

<a id="item-13"></a>
## [Telegram Launches Serverless Platform for Bot Backends](https://core.telegram.org/bots/serverless) ⭐️ 8.0/10

Telegram has officially launched a serverless platform that allows developers to run bot and Mini App backend code directly on Telegram's infrastructure using plain JavaScript modules, deployable with a single CLI command. This eliminates the need for developers to manage servers, containers, or scaling, significantly reducing operational overhead and lowering the barrier to entry for building Telegram bots and Mini Apps. The platform runs code in an isolated V8 sandbox located close to the Bot API, and includes a built-in SQLite database. Deployment is done via the command 'npx tgcloud push'.

telegram · zaihuapd · Jul 15, 16:00

**Background**: Serverless computing allows developers to write and deploy code without provisioning or managing servers, as the cloud provider handles scaling and infrastructure. Telegram's platform is specifically tailored for its bot ecosystem, which previously required developers to host their own servers to handle webhook updates or polling.

<details><summary>References</summary>
<ul>
<li><a href="https://elsolitario.org/en/2026/07/15/telegram-serverless-bots-without-a-server/">Telegram Serverless: serverless bot backends - elsolitario.org</a></li>
<li><a href="https://daily.dev/posts/telegram-serverless-uej7tlh7t">Telegram Serverless - daily.dev</a></li>

</ul>
</details>

**Tags**: `#serverless`, `#Telegram`, `#bots`, `#JavaScript`, `#cloud computing`

---

<a id="item-14"></a>
## [Mental Health and Communication in Software Development](https://ramones.dev/posts/mental-health/) ⭐️ 7.0/10

A personal blog post emphasizes the importance of mental health and communication for software developers, sparking a community discussion on neurodivergence and self-management. This topic is highly relevant to software engineers, as mental health challenges and communication issues are common in the tech industry, and the discussion provides practical insights for self-management. The post has high engagement with 285 points and 245 comments, indicating strong resonance within the community. Commenters share personal experiences and strategies for managing neurodivergence and improving communication.

hackernews · ramon156 · Jul 15, 11:27 · [Discussion](https://news.ycombinator.com/item?id=48919198)

**Background**: Mental health in tech is an increasingly discussed topic, with many developers facing burnout, imposter syndrome, and communication breakdowns. Neurodivergence, such as ADHD or autism, can affect work patterns and require tailored coping strategies.

**Discussion**: Commenters generally agree that mental health is crucial and that neurodivergent individuals need personalized management strategies rather than trying to 'snap out of it.' Some emphasize aligning work with one's personality and strengths.

**Tags**: `#mental health`, `#software engineering`, `#neurodivergence`, `#communication`, `#self-management`

---

<a id="item-15"></a>
## [Dependabot Defaults to Three-Day Cooldown for Version Updates](https://simonwillison.net/2026/Jul/14/github-changeling/#atom-everything) ⭐️ 7.0/10

GitHub's Dependabot now defaults to a three-day cooldown before opening version update pull requests, requiring no configuration. This reduces unnecessary update noise and mitigates supply-chain attacks by delaying adoption of potentially malicious packages. The cooldown applies only to version updates, not security updates, and was previously an opt-in feature introduced in July 2025.

rss · Simon Willison · Jul 14, 22:43

**Background**: Dependency cooldowns intentionally delay installation of new package versions to give time for malicious releases to be identified and removed. This practice gained traction after incidents like the axios supply-chain attack.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-07-14-dependabot-version-updates-introduce-default-package-cooldown/">Dependabot version updates introduce default package cooldown</a></li>
<li><a href="https://docs.github.com/en/code-security/reference/supply-chain-security/dependabot-options-reference">Dependabot options reference - GitHub Docs</a></li>
<li><a href="https://securitylabs.datadoghq.com/articles/dependency-cooldowns/">The case for dependency cooldowns in a post-axios world | Datadog Security Labs</a></li>

</ul>
</details>

**Tags**: `#dependabot`, `#github`, `#dependency-management`, `#security`, `#packaging`

---

<a id="item-16"></a>
## [Cache-friendly uvx usage in GitHub Actions](https://simonwillison.net/2026/Jul/14/uvx-github-actions-cache/#atom-everything) ⭐️ 7.0/10

Simon Willison published a recipe for using uvx in GitHub Actions that sets UV_EXCLUDE_NEWER to a fixed date and includes that date in the cache key, so tools are cached and only updated when the date is manually bumped. This pattern avoids repeated downloads from PyPI on every workflow run, significantly speeding up CI for Python projects that use uvx to run tools like linters or formatters. The environment variable UV_EXCLUDE_NEWER is set to a date like "2026-07-12", and the cache key includes that date; to upgrade tools, users simply update the date. The post also links to an issue requesting that astral-sh/setup-uv cache wheels by default.

rss · Simon Willison · Jul 14, 00:56

**Background**: uvx is a tool from Astral that runs Python CLI tools in ephemeral isolated environments. By default, each invocation may download the tool and its dependencies from PyPI, which is slow in CI. GitHub Actions caching can store these downloads, but the cache key must be carefully designed to avoid stale tools.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.astral.sh/uv/concepts/tools/">Tools | uv</a></li>
<li><a href="https://docs.astral.sh/uv/reference/environment/">Environment variables | uv - Astral Docs</a></li>

</ul>
</details>

**Discussion**: The post links to an existing issue on the astral-sh/setup-uv repository requesting that the default behavior switch to caching rather than purging wheels from PyPI, indicating community interest in better caching defaults.

**Tags**: `#GitHub Actions`, `#Python`, `#CI/CD`, `#uv`, `#caching`

---

<a id="item-17"></a>
## [7 Mobile AI Models Including Apple Intelligence Get China Approval](https://mp.weixin.qq.com/s/5MTWh4pWVAlL71RQbU-Udg) ⭐️ 7.0/10

On July 15, 2026, China's Cyberspace Administration announced that seven mobile-side AI language models, including Apple Intelligence, Huawei Xiaoyi, OPPO AndesGPT, vivo BlueHeart, Xiaomi Hyper AI, Samsung Galaxy AI, and ZTE's model, have completed the government filing (备案) for deployment on smartphones. This marks a major regulatory milestone for integrating advanced AI into mainstream smartphones in China, ensuring compliance with local laws and paving the way for widespread consumer availability. It also signals that global tech giants like Apple are adapting their AI offerings to meet China's strict content and data governance requirements. The filing covers models specifically designed for on-device inference, with application scenarios limited to mobile phones. Notably, Alibaba's Qwen will serve as the underlying AI capability for Apple Intelligence in China, providing text and image understanding, content generation, and multi-turn dialogue for iOS, iPadOS, macOS, and visionOS devices.

telegram · zaihuapd · Jul 15, 08:06

**Background**: China's 2023 Interim Measures for the Management of Generative AI Services require companies offering generative AI to the public to file with the cyberspace authorities. This filing process involves submitting model details, safety assessments, and data handling practices. The approval of these seven models indicates they have passed regulatory review and can now be deployed on consumer devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2026-07/15/c_1785861480767004.htm">关于发布7款提供手机端侧生成式人工智能服务已备案信息的公告关于发布...</a></li>
<li><a href="https://www.sohu.com/a/1050785859_546984">国行Apple智能过审！阿里千问接入iPhone，7款手机端侧大模型备案出炉...</a></li>
<li><a href="https://news.qq.com/rain/a/20260715A08MGP00">苹果AI入华有戏了？工信部发布7款手机端侧大模型备案信息：Apple智能...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mobile`, `#regulation`, `#China`, `#LLM`

---

<a id="item-18"></a>
## [Chinese Retail Blurs: Sam's, Snack Stores, Pinduoduo Vie for Same Wallet](https://mp.weixin.qq.com/s/dAHAVxglD-F1RovjcvqCRw) ⭐️ 7.0/10

A survey based on 257 interviews and 5,224 questionnaires reveals that China's retail industry has entered an era of convergence, where Sam's Club, snack discount stores, instant retail, and Pinduoduo are competing for the same household spending. The research indicates that 48% of respondents plan to control consumption, and trust has become the primary competitive factor, surpassing price. This shift signals the end of vertical retail categories in China, forcing retailers to compete on trust and convenience rather than just price. It has profound implications for business strategy, as companies must adapt to a landscape where consumers prioritize reliability and proximity over discounts. Sam's Club is projected to achieve annual revenue of 180-200 billion yuan in China; leading snack store chains have nearly 40,000 outlets; and Pinduoduo's Duoduo Maicai has annual sales of about 300 billion yuan, potentially reaching 400 billion yuan this year. The survey also found that for food products, excessively low prices trigger safety concerns, making trust the top competitive advantage.

telegram · zaihuapd · Jul 15, 09:01

**Background**: Chinese retail has traditionally been segmented into distinct categories such as hypermarkets, convenience stores, and e-commerce platforms. However, recent trends show these boundaries dissolving as consumers seek convenience and trust across channels. Instant retail, which delivers goods within minutes, and snack discount stores, which offer low-priced bulk snacks, have grown rapidly, while platforms like Pinduoduo leverage social commerce and group buying to capture household spending.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chinairn.com/scfx/20260715/153343594.shtml">2026年零食折扣店行业深度分析：市场规模、竞争格局、渠道红利与头部品牌梳理_中研普华_中研网</a></li>
<li><a href="https://m.ikanchai.com/article/125970">一文读懂 即 时 零 售 ：本地供给、 即 时 需求、 即 时 配送成核心三要素</a></li>
<li><a href="https://www.36kr.com/p/2937876087152007">多多买菜战略大拆解 - 36氪</a></li>

</ul>
</details>

**Tags**: `#retail`, `#China`, `#consumer behavior`, `#e-commerce`, `#business strategy`

---

<a id="item-19"></a>
## [Judge Questions Epic-Google Antitrust Settlement Over $800M Deal](https://t.me/zaihuapd/42588) ⭐️ 7.0/10

U.S. District Judge James Donato disclosed during a hearing that Epic Games and Google have entered a new commercial partnership involving joint product development, marketing, and partnerships, with Epic paying Google approximately $800 million over six years. This partnership could undermine Epic's push for Android ecosystem reform, as the judge questioned whether the deal compromises Epic's antitrust stance. The case has significant implications for app store competition and developer fees on Android. The partnership involves Unreal Engine, Fortnite, and Android-related businesses. Epic CEO Tim Sweeney stated that the agreement does not include a commitment to drop Epic's antitrust claims.

telegram · zaihuapd · Jul 15, 11:15

**Background**: Epic Games sued Google in 2020, alleging anticompetitive practices in the Google Play Store. In 2024, a jury found Google liable for monopolization. The parties reached a settlement in 2025-2026, with Google agreeing to reduce Play Store commissions for Epic and allow alternative app stores.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Epic_Games_v._Google">Epic Games v. Google - Wikipedia</a></li>
<li><a href="https://techcrunch.com/2026/03/04/google-settles-with-epic-games-drops-its-play-store-commissions-to-20/">Google settles with Epic Games, drops its Play Store ...</a></li>
<li><a href="https://www.adwaitx.com/google-epic-800m-android-unreal-deal/">Google & Epic Strike $800M Deal: Secret Android Partnership</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#Epic Games`, `#Google`, `#Android`, `#legal`

---

<a id="item-20"></a>
## [ASML Plans Price Hikes on EUV and DUV Lithography Equipment](https://news.bloomberglaw.com/artificial-intelligence/asml-plans-price-increases-on-chipmaking-equipment-information) ⭐️ 7.0/10

ASML announced plans to raise prices on its chipmaking equipment, including a 10% increase on DUV systems for some Chinese customers who have already accepted the hike, while negotiations with TSMC over EUV price increases face resistance. As the dominant supplier of advanced lithography equipment, ASML's pricing power directly impacts the global semiconductor supply chain and chip costs, especially for leading-edge nodes. The divergent responses from TSMC and Chinese firms highlight geopolitical tensions and market dynamics. ASML's CFO Roger Dassen stated that the current environment gives the company better pricing power, and advanced EUV lithography machine capacity is nearly fully booked through the end of 2027. The price increases apply to both EUV and DUV systems, with DUV up 10% for certain Chinese customers.

telegram · zaihuapd · Jul 15, 16:49

**Background**: ASML is the world's only supplier of extreme ultraviolet (EUV) lithography systems, which are essential for manufacturing the most advanced semiconductor chips at nodes like 5nm and 3nm. Deep ultraviolet (DUV) lithography is used for less critical layers and older nodes. The company's pricing decisions are closely watched due to its monopoly position and the strategic importance of chipmaking equipment.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/EUV_lithography">EUV lithography</a></li>
<li><a href="https://en.wikipedia.org/wiki/ASML">ASML</a></li>
<li><a href="https://en.wikipedia.org/wiki/Photolithography">Photolithography - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#ASML`, `#lithography`, `#chipmaking`, `#geopolitics`

---