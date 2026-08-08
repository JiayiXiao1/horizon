---
layout: default
title: "Horizon Summary: 2026-08-08 (EN)"
date: 2026-08-08
lang: en
---

> From 33 items, 23 important content pieces were selected

---

1. [Rewriting Postgres in Rust Achieves 300x Analytics Speedup](#item-1) ⭐️ 9.0/10
2. [DeepSeek V4 Flash 0731 Delivers Major Performance and Cost Gains](#item-2) ⭐️ 8.0/10
3. [Assembly Hall of Shame: Documenting the Slowest x86 Instructions](#item-3) ⭐️ 8.0/10
4. [Tech Worker Sadness: A Crisis of Faith in the Industry](#item-4) ⭐️ 8.0/10
5. [Oracle Bans AI-Generated Code in OpenJDK Contributions](#item-5) ⭐️ 8.0/10
6. [2027 Memory Capacity Reportedly Sold Out Due to HBM Demand](#item-6) ⭐️ 8.0/10
7. [Cloudflare Unveils Kitesurf, an Agent-First Browser on V8 Isolates](#item-7) ⭐️ 8.0/10
8. [Website Owner's Year-Long Battle Against Bots Highlights Cost and Open Web Concerns](#item-8) ⭐️ 8.0/10
9. [New Mexico Court Orders Meta to Pay $567M for Teen Mental Health Harms](#item-9) ⭐️ 8.0/10
10. [Wyzer: A New Language for Distributed Safety via Choreographic Programming](#item-10) ⭐️ 8.0/10
11. [AMD acquires Taalas to etch AI models into silicon for faster inference](#item-11) ⭐️ 8.0/10
12. [Datasette 1.0a38 Fixes SQL Injection in Mixed Public/Private Tables](#item-12) ⭐️ 8.0/10
13. [Meta Launches Muse Code and Muse Spark 1.2 with Long-Sequence Agentic Tool Calling](#item-13) ⭐️ 8.0/10
14. [US Probes China's Offshore Access to Nvidia Chips](#item-14) ⭐️ 8.0/10
15. [SK Hynix Confirms 375-Layer V10 NAND with Wafer Bonding](#item-15) ⭐️ 8.0/10
16. [Critical OAuth Account Takeover in sub2api (CVSS 8.8)](#item-16) ⭐️ 8.0/10
17. [Rumor: OpenAI to Launch New Model Astra Next Week](#item-17) ⭐️ 8.0/10
18. [App Store Rejects App for Nonexistent Tarot Feature](#item-18) ⭐️ 7.0/10
19. [GPT-5.6 Sol Ultra Outshines Claude Fable 5 in Raccoon Heist Game Test](#item-19) ⭐️ 7.0/10
20. [Tokenpocalypse: Companies Scramble to Cut AI Token Costs](#item-20) ⭐️ 7.0/10
21. [Claude Fable 5 Relaunch Faces Quality Complaints and Safety Misjudgments](#item-21) ⭐️ 7.0/10
22. [Nasdaq Seeks 23-Hour Trading, Following NYSE's 22-Hour Approval](#item-22) ⭐️ 7.0/10
23. [Amazon Cracks Down on Internal CPU Waste as Agentic AI Drives Demand](#item-23) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Rewriting Postgres in Rust Achieves 300x Analytics Speedup](https://malisper.me/how-we-made-postgres-hundreds-of-times-faster-the-query-engine/) ⭐️ 9.0/10

The pgrust project, an experimental rewrite of PostgreSQL in Rust, has achieved up to 300x speedup for analytical queries through batching, operator fusion, and SIMD. The project also emphasizes correctness via formal verification and differential testing, proving over 1000 user-facing functions match Postgres logic. This demonstrates a viable path to dramatically improve Postgres analytics performance, potentially benefiting the vast ecosystem that relies on Postgres. It also sparks debate about trust and the role of community-driven rewrites in critical infrastructure. The new executor is vectorized, push-based, and JIT-compiled, with a thread-based concurrency model. The project compiles to WebAssembly and runs in the browser, and the author has focused on formal verification and differential fuzz testing to ensure correctness.

hackernews · poly2it · Aug 7, 11:00 · [Discussion](https://news.ycombinator.com/item?id=49208535)

**Background**: Traditional query engines often materialize intermediate results between operators, which is inefficient. Operator fusion combines multiple operations into a single pass, and SIMD (Single Instruction, Multiple Data) allows processing multiple data points in one instruction, both improving performance. pgrust is an experimental rewrite of PostgreSQL in Rust, aiming to leverage modern language features for better performance and safety.

<details><summary>References</summary>
<ul>
<li><a href="https://pgrust.com/">pgrust — postgres, rewritten in rust</a></li>
<li><a href="https://github.com/malisper/pgrust">GitHub - malisper/ pgrust : Postgres rewritten in Rust , now faster than...</a></li>
<li><a href="https://arxiv.org/pdf/1610.09166">Push vs. Pull-Based Loop Fusion in Query Engines</a></li>

</ul>
</details>

**Discussion**: The author engaged in the discussion, addressing trust concerns by highlighting formal verification and differential testing. Some commenters expressed skepticism about adoption due to trust in the Postgres team, while others praised the potential for adaptive planning and hoped it would prove viability. There were also technical questions about I/O scheduling and thread management.

**Tags**: `#Postgres`, `#query-engine`, `#performance`, `#Rust`, `#SIMD`

---

<a id="item-2"></a>
## [DeepSeek V4 Flash 0731 Delivers Major Performance and Cost Gains](https://arcprize.org/results/deepseek-v4-flash-0731) ⭐️ 8.0/10

DeepSeek released the V4 Flash 0731 update on July 31, 2025, a sparse mixture-of-experts model with 13B active parameters out of 284B total. It outperforms the earlier V4 Pro (Preview) on benchmarks while offering significantly lower pricing and faster speeds. This update makes high-performance AI more accessible and affordable, potentially shifting developer preferences away from more expensive proprietary models. Its combination of speed, capability, and low cost could accelerate adoption in cost-sensitive applications and local deployments. The model supports a 1M token context window and a maximum output of 65,536 tokens. Pricing is $0.14 per 1M input tokens and $0.28 per 1M output tokens (or $0.09/$0.18 on OpenRouter), with fastest output speeds observed at 189 tokens/s on Fireworks.

hackernews · tosh · Aug 7, 17:56 · [Discussion](https://news.ycombinator.com/item?id=49214008)

**Background**: DeepSeek is a Chinese AI lab known for releasing competitive open-weight models at low cost. The V4 Flash series is designed for efficiency, using a sparse mixture-of-experts architecture to activate only a fraction of parameters per token, balancing performance and cost.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/models/deepseek-v4-flash">DeepSeek V4 Flash 0731 (max) - Intelligence, Performance & Price Analysis</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash-0731">deepseek-ai/DeepSeek-V4-Flash-0731 · Hugging Face</a></li>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-flash-0731">DeepSeek V4 Flash 0731 - API Pricing & Benchmarks | OpenRouter</a></li>

</ul>
</details>

**Discussion**: Users report excellent real-world performance, with one noting it's 'good enough for almost everything' and costs are negligible, spending under $5/day even with multiple sessions. Another user highlights the speed as a killer feature, achieving ~8k tok/s prefill and ~250 tok/s on a single stream locally. Some express concern about an upcoming price increase and note that V4 Pro is still in post-processing.

**Tags**: `#AI`, `#DeepSeek`, `#LLM`, `#performance`, `#release`

---

<a id="item-3"></a>
## [Assembly Hall of Shame: Documenting the Slowest x86 Instructions](https://github.com/xoreaxeaxeax/asm-hall-of-shame) ⭐️ 8.0/10

A GitHub repository titled 'Assembly Hall of Shame' has been created to document the slowest x86 instructions, featuring a leaderboard of intentionally slow operations and creative assembly tricks. The project has gained significant attention, scoring 8.0/10 with 225 points and 45 comments. This repository highlights obscure and often overlooked aspects of x86 architecture, providing valuable insights for low-level systems programmers and security researchers. The community discussion reveals potential security implications, such as using slow instructions to trigger System Management Mode (SMM) traps, which could be exploited in firmware attacks. The repository includes a leaderboard of the slowest instructions, with rules stating that trapped, emulated, or virtualized instructions may only time the trap, not the handler. One notable entry is a 12ms write to an ACPI IO port, which may actually be trapping to SMM. The author also has related projects, such as a compiler that emits only 'mov' instructions and another that deliberately obfuscates control flow to draw symbols in debuggers.

hackernews · piotrgrabowski · Aug 7, 18:01 · [Discussion](https://news.ycombinator.com/item?id=49214098)

**Background**: x86 is a complex instruction set architecture (ISA) that includes many legacy and rarely used instructions. Some instructions are inherently slow due to microcode emulation or interactions with system management mode (SMM), a special operating mode for firmware. The repository explores these slow instructions, often for educational or security research purposes, and has sparked discussions about their potential misuse.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/List_of_x86_instructions">List of x 86 instructions - Wikipedia</a></li>
<li><a href="https://learn.microsoft.com/en-us/windows-hardware/drivers/debugger/x86-instructions">x 86 Instructions - Windows drivers | Microsoft Learn</a></li>
<li><a href="https://dev.to/shankararyal/deep-dive-assembly-language-security-vulnerabilities-and-mitigations-in-modern-systems-1d0j">Deep Dive: Assembly Language Security Vulnerabilities and Mitigations in Modern Systems - DEV Community</a></li>

</ul>
</details>

**Discussion**: Community comments highlight related projects, such as using slow instructions to break SMI (System Management Interrupt) and the author's other works like a compiler that emits only 'mov' instructions. There is also a humorous suggestion that 'nop' should be #1 because it is infinitely slow for what it does, and a reference to Core War, a programming game.

**Tags**: `#assembly`, `#x86`, `#low-level programming`, `#security research`, `#performance`

---

<a id="item-4"></a>
## [Tech Worker Sadness: A Crisis of Faith in the Industry](https://www.noemamag.com/why-is-everyone-in-tech-so-sad/) ⭐️ 8.0/10

An article on Noema Magazine explores the widespread sadness and loss of faith among tech workers, sparking a large community discussion on Hacker News with 356 points and 492 comments. The piece examines the toxic online culture and career disillusionment affecting the industry. This discussion highlights a growing crisis in tech culture, where burnout and disillusionment are becoming widespread, potentially impacting retention and innovation. It resonates with broader concerns about mental health and sustainability in high-pressure industries. The article's title poses a question about an entire class of workers losing faith, drawing parallels to historical trades like printers. Community comments reference the toxicity of the modern web and personal experiences of declining enthusiasm after decades in tech.

hackernews · RickJWagner · Aug 7, 12:42 · [Discussion](https://news.ycombinator.com/item?id=49209539)

**Background**: The tech industry has long been associated with optimism and rapid advancement, but recent years have seen rising reports of burnout, layoffs, and a toxic online culture. This article taps into a broader conversation about the sustainability of tech careers and the mental health of workers.

**Discussion**: Comments reflect a mix of historical analogies (e.g., printers) and personal anecdotes of disillusionment, with some noting the web's toxicity and others finding the article's tone off-putting. Overall sentiment is one of shared concern and resonance with the topic.

**Tags**: `#tech culture`, `#burnout`, `#career`, `#mental health`, `#industry trends`

---

<a id="item-5"></a>
## [Oracle Bans AI-Generated Code in OpenJDK Contributions](https://app.dealroom.co/news/feed/oracle-bans-ai-generated-code-from-openjdk-despite-ellison-s-claim-oracle-isn-t-writing-its-own-code) ⭐️ 8.0/10

Oracle has implemented an interim policy banning AI-generated code contributions to OpenJDK, effective April 9, 2026, until a final policy is drafted by their legal team. This policy sets a precedent for how major open-source projects handle AI-generated contributions, potentially influencing other projects and raising legal and review burden concerns. It also highlights the tension between Oracle's AI investments and its cautious approach to code provenance. The interim policy explicitly prohibits content generated in part or in full by large language models, diffusion models, or similar deep-learning systems. The final policy is being written by Oracle's lawyers, and the decision is partly motivated by past copyright issues in Java and the need to protect against legal risks.

hackernews · delduca · Aug 7, 17:36 · [Discussion](https://news.ycombinator.com/item?id=49213754)

**Background**: OpenJDK is the open-source implementation of the Java Platform, Standard Edition, and is developed by a community including Oracle and other contributors. AI-generated code has raised legal questions about copyright and licensing, as seen in cases like Doe v. GitHub, where AI tools may reproduce licensed code without proper attribution. Oracle's policy aims to mitigate these risks by requiring human authorship and provenance clarity.

<details><summary>References</summary>
<ul>
<li><a href="https://openjdk.org/legal/ai">OpenJDK Interim Policy on Generative AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/OpenJDK">OpenJDK - Wikipedia</a></li>
<li><a href="https://www.mbhb.com/intelligence/snippets/navigating-the-legal-landscape-of-ai-generated-code-ownership-and-liability-challenges/">Navigating the Legal Landscape of AI-Generated Code: Ownership and Liability Challenges - MBHB</a></li>

</ul>
</details>

**Discussion**: Commenters generally view the policy as sensible given legal concerns, though some note irony in Oracle's AI investments. Others point to the review burden on human reviewers and the potential for the final policy to be overly restrictive. A few express surprise that Oracle develops OpenJDK, mistaking it for a purely community-driven project.

**Tags**: `#OpenJDK`, `#AI policy`, `#open source`, `#legal`, `#software development`

---

<a id="item-6"></a>
## [2027 Memory Capacity Reportedly Sold Out Due to HBM Demand](https://www.ign.com/articles/ramageddon-continues-another-year-as-2027-memory-capacity-is-reportedly-sold-out) ⭐️ 8.0/10

A report indicates that memory capacity for 2027 has been fully sold out, primarily due to the surging demand for High Bandwidth Memory (HBM) in AI applications. This has constrained the supply of non-HBM DRAM, raising concerns about memory availability for other products. This development is significant because it highlights the growing impact of AI hardware on the global memory supply chain. The shortage could affect a wide range of consumer and enterprise products, from smartphones and laptops to servers, potentially leading to price increases and delayed availability. HBM production consumes approximately three times the wafer supply compared to standard DDR5 for the same number of bits, according to industry analysis. This trade-off means that as HBM capacity expands, less wafer capacity is available for conventional DRAM, exacerbating the supply crunch.

hackernews · inigyou · Aug 7, 07:58 · [Discussion](https://news.ycombinator.com/item?id=49207236)

**Background**: High Bandwidth Memory (HBM) is a 3D-stacked DRAM technology designed for high-performance computing, particularly AI and graphics processing. It offers significantly higher bandwidth and lower power consumption compared to traditional DRAM, making it essential for AI accelerators like NVIDIA GPUs. The rapid growth of AI infrastructure has driven unprecedented demand for HBM, straining the overall DRAM supply chain.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.trendforce.com/presscenter/news/20260804-13166.html">DRAM Supply to Remain Tight in 2027 , Prompting NVIDIA to Lower...</a></li>
<li><a href="https://www.dqindia.com/semiconductors/diverging-memory-market-outlook-in-2027-as-dram-supply-remains-tight-while-nand-flash-supply-conditions-ease-12218465">Diverging memory market outlook in 2027 as DRAM supply remains...</a></li>

</ul>
</details>

**Discussion**: Community comments reflect a mix of concern and technical insight. One user highlighted the wafer trade-off between HBM and DDR5, explaining why HBM production constrains non-HBM supply. Others expressed worries about the impact on consumer electronics and inflation, while some suggested alternative solutions like a USB-like standard for RAM sticks.

**Tags**: `#memory`, `#HBM`, `#supply chain`, `#AI hardware`, `#semiconductors`

---

<a id="item-7"></a>
## [Cloudflare Unveils Kitesurf, an Agent-First Browser on V8 Isolates](https://blog.cloudflare.com/kitesurf/) ⭐️ 8.0/10

Cloudflare announced Kitesurf, an agent-first browser that runs in V8 isolates, built on the open-source Blitz engine. It aims to enable browser automation and AI agents on Cloudflare's edge network. This marks a significant step in bringing browser automation and AI agents to the edge, potentially transforming web scraping, testing, and content generation. It also raises important questions about Cloudflare's dual role as both a CDN with anti-bot measures and a provider of agent-friendly infrastructure. Kitesurf is built on Blitz, a modular open-source browser engine written in Rust, and runs in V8 isolates, the same engine powering Chrome and Node.js. Cloudflare intends to open source and upstream their patches to Blitz, according to community comments.

hackernews · m3h · Aug 7, 10:42 · [Discussion](https://news.ycombinator.com/item?id=49208393)

**Background**: V8 isolates are lightweight sandboxed environments that allow multiple instances of JavaScript code to run concurrently, making them ideal for edge computing. Blitz is a new independent web engine implemented in Rust, designed to be modular and flexible for various use cases. Agent-first browsers are designed to enable AI agents to perform tasks in the browser, such as web scraping and automation.

<details><summary>References</summary>
<ul>
<li><a href="https://nlnet.nl/project/Blitz/">NLnet; Blitz - a modular web renderer</a></li>
<li><a href="https://dev.to/tomlienard/v8-isolates-are-taking-over-the-world-3h4m">V 8 Isolates are taking over the world - DEV Community</a></li>

</ul>
</details>

**Discussion**: Community comments raise concerns about Cloudflare's conflict of interest, as it both provides anti-bot protection and agent-friendly infrastructure. Some question whether Kitesurf instances will bypass Cloudflare's own anti-bot mechanisms, while others ask for practical examples of agent use cases. There is also a lighthearted comment about kitesurfing being outdated.

**Tags**: `#browser`, `#cloudflare`, `#AI agents`, `#web scraping`, `#browser automation`

---

<a id="item-8"></a>
## [Website Owner's Year-Long Battle Against Bots Highlights Cost and Open Web Concerns](https://patronview.com/news/99-percent-of-my-website-traffic-is-bots/) ⭐️ 8.0/10

A website owner shared a detailed account of a year-long struggle against bots that consumed 99% of traffic, causing a 500% cost spike in one month. The post discusses the use of Cloudflare and the trade-offs of relying on third-party bot mitigation services. This story underscores the growing burden of bot traffic on website owners, both financially and operationally. It raises important questions about the sustainability of the open web and the implications of outsourcing access control to large companies like Cloudflare. The site's normal monthly bill is around $90, but spiked by about 500% during a bad month, partly due to D1 database costs. The author acknowledges being a scraper themselves, adding nuance to the discussion. Community members suggest alternatives like Anubis, a proof-of-work based bot detection tool, and consider moving to static sites to reduce costs.

hackernews · petercooper · Aug 7, 14:51 · [Discussion](https://news.ycombinator.com/item?id=49211386)

**Background**: Web scraping bots are automated programs that visit websites to extract data, often consuming significant bandwidth and server resources. Bot mitigation services like Cloudflare use various techniques, including machine learning and behavioral analysis, to distinguish between human users and bots, assigning a bot score to each request. However, these services can be costly and may inadvertently block legitimate users, raising concerns about centralizing control over web access.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/bots/get-started/bot-management/">Bot Management · Cloudflare bot solutions docs</a></li>
<li><a href="https://www.cloudflare.com/learning/bots/what-is-bot-management/">What is bot management? | Learning Center</a></li>
<li><a href="https://www.scrapehero.com/detect-and-block-bots/">How Websites Use Bot Mitigation Tools [Detection Explained]</a></li>

</ul>
</details>

**Discussion**: Community comments express concern about outsourcing web access decisions to large companies like Cloudflare, fearing it undermines the open web. Users recommend alternative solutions like Anubis, which uses proof-of-work to detect real browsers, and suggest cost-saving measures such as moving to static sites. Some share personal experiences with bot traffic, like Claude-searchbot fetching 205,000 pages without sending any referral, highlighting the lack of compensation for scraped content.

**Tags**: `#web scraping`, `#bot mitigation`, `#Cloudflare`, `#website costs`, `#open web`

---

<a id="item-9"></a>
## [New Mexico Court Orders Meta to Pay $567M for Teen Mental Health Harms](https://www.theguardian.com/technology/2026/aug/06/new-mexico-court-meta) ⭐️ 8.0/10

A New Mexico state court ordered Meta Platforms to pay $567 million into an abatement fund and make significant changes to its platforms for underage users, following a ruling that its social media platforms harmed teens' mental health. This judgment adds to a previous $375 million civil penalty, bringing the total to $942 million. This is the largest judgment yet in U.S. litigation over social media's impact on children, setting a precedent that could influence other states and countries to take similar action. It signals that tech companies may face substantial financial and operational consequences for platform design choices affecting minors. The court found Meta violated New Mexico's public nuisance law (NMSA 1978 § 30-8-1), which prohibits knowingly maintaining anything injurious to public health, safety, morals, or welfare. The $567 million abatement fund is intended to address the damage, and Meta must implement changes for underage accounts, though specific changes were not detailed in the summary.

hackernews · boplicity · Aug 7, 00:06 · [Discussion](https://news.ycombinator.com/item?id=49204352)

**Background**: Public nuisance law traditionally applies to activities that harm the public at large, such as pollution or obstruction of public rights. In recent years, states have used this legal theory to hold tech companies accountable for social harms, arguing that addictive platform designs constitute a public nuisance. Meta, the parent company of Facebook and Instagram, has faced multiple lawsuits from states and school districts over teen mental health, with this ruling being a notable outcome.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kob.com/new-mexico/nm-court-orders-meta-to-pay-567m-make-changes-for-underage-users/">NM court orders Meta to pay $567M, make changes for underage users</a></li>
<li><a href="https://www.reuters.com/legal/government/how-could-new-mexicos-567-million-ruling-change-meta-2026-08-07/">Explainer: How could New Mexico's $567 million ruling change Meta?</a></li>
<li><a href="https://www.malwarebytes.com/blog/uncategorized/2026/08/meta-ordered-to-pay-942-million-over-harm-to-children">Meta ordered to pay $942 million over harm to children</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that while the fine may seem small relative to Meta's global revenue, it is significant for a small jurisdiction like New Mexico, with one user calculating the per-capita impact. Others discuss the legal basis under public nuisance law and compare it to other jurisdictions, while some express skepticism that such penalties are merely a 'cost of doing business' and question whether they will drive meaningful change.

**Tags**: `#Meta`, `#legal`, `#mental health`, `#children`, `#regulation`

---

<a id="item-10"></a>
## [Wyzer: A New Language for Distributed Safety via Choreographic Programming](https://github.com/Wyzer-Lang/wyzer) ⭐️ 8.0/10

Wyzer is a new statically typed, compiled, resource-oriented programming language that integrates choreographic programming and the Perceus memory model to address distributed deadlocks and protocol mismatches, which Rust does not guarantee. The project is nearing its 0.1.0 release after five months of research and a few weeks of development. This project is significant because it attempts to bring academic concepts like choreographic programming into a practical, high-level language, potentially offering stronger safety guarantees for distributed systems than existing languages like Rust. If successful, it could influence future language design and improve reliability in distributed computing. Wyzer uses linear/affine types and Perceus reference counting instead of borrow checkers and lifetimes, which the author claims is computationally simpler for an LSP to understand. The language aims to generalize choreographic programming, ensuring that every send has a corresponding receive, thus preventing deadlocks within the choreography scope.

hackernews · v0id_isgood · Aug 7, 12:28 · [Discussion](https://news.ycombinator.com/item?id=49209385)

**Background**: Choreographic programming is a paradigm for distributed systems where programs are written as global descriptions of interactions among participants, and a compiler can project these into local implementations, ensuring deadlock-freedom by construction. Perceus is a reference counting technique that enables efficient memory management without a garbage collector, as used in the Koka language. Rust provides memory safety through its borrow checker but does not address distributed deadlocks or protocol mismatches, which motivated the creation of Wyzer.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Choreographic_programming">Choreographic programming</a></li>
<li><a href="https://www.microsoft.com/en-us/research/wp-content/uploads/2020/11/perceus-tr-v1.pdf">Perceus : Garbage Free Reference Counting with ReuseMicrosoft...</a></li>

</ul>
</details>

**Discussion**: The HN community is generally positive about the ambition and novelty of the project, with commenters like jerf praising it for not being another 'state of the art in 2015' language. However, they also suggest improvements: jerf recommends recalibrating documentation to highlight the genuinely new ideas, hyperhello asks for more examples and notes the syntax is generic but conservative, and vlovich123 questions how distributed deadlock freedom is guaranteed, asking for concrete examples. renox raises concerns about the lack of distinction between internal and external function calls, particularly regarding latency and timeouts.

**Tags**: `#programming language`, `#distributed systems`, `#memory safety`, `#choreographic programming`, `#Rust`

---

<a id="item-11"></a>
## [AMD acquires Taalas to etch AI models into silicon for faster inference](https://www.theregister.com/systems/2026/08/06/amd-acquires-ai-chip-startup-taalas-to-boost-inference-performance-by-etching-models-into-silicon/5284344) ⭐️ 8.0/10

AMD announced a definitive agreement to acquire Toronto-based AI chip startup Taalas on August 6, 2026. Taalas specializes in etching specific AI models directly onto silicon, achieving inference speeds like 17,000 tokens per second for Llama 3.1 8B. This acquisition could significantly boost AMD's AI inference performance and efficiency, challenging Nvidia's dominance in the AI hardware market. It also signals a trend toward model-specific silicon, which may lead to faster and more energy-efficient on-device AI. Taalas, founded in 2023, has raised $219 million and employs a 24-person team. AMD plans to integrate Taalas' technology with its Instinct GPUs to deliver system-level solutions for the growing AI inference market.

hackernews · itvision · Aug 6, 20:23 · [Discussion](https://news.ycombinator.com/item?id=49201970)

**Background**: Traditional AI chips, like GPUs, are general-purpose and execute models via software instructions. Taalas takes a different approach by physically etching a specific AI model's architecture into the silicon, eliminating the need for software execution and dramatically improving speed and efficiency. This is similar to how dedicated hardware for video decoding became standard in consumer devices.

<details><summary>References</summary>
<ul>
<li><a href="https://ir.amd.com/news-events/press-releases/detail/1296/amd-acquires-taalas-to-advance-compute-solutions-for-rapidly-growing-ai-inference-market">AMD Acquires Taalas to Advance Compute Solutions for Rapidly Growing AI ...</a></li>
<li><a href="https://qz.com/amd-acquires-taalas-ai-inference-chip-startup-080726">AMD acquires Taalas AI inference chip startup</a></li>
<li><a href="https://www.cnbc.com/2026/08/06/amd-buys-taalas-startup-that-hardwires-ai-models-into-its-silicon.html">AMD buys Taalas, startup that hardwires AI models into its silicon - CNBC</a></li>

</ul>
</details>

**Discussion**: Community comments express surprise that OpenAI or Anthropic didn't make a similar move, noting that Chinese open-weight models are commoditizing their value. Some see this as enabling 'good enough' LLMs to run on-device at battery-level power, while others highlight potential inflection points in UX and faster iteration cycles.

**Tags**: `#AMD`, `#AI hardware`, `#inference`, `#acquisition`, `#silicon`

---

<a id="item-12"></a>
## [Datasette 1.0a38 Fixes SQL Injection in Mixed Public/Private Tables](https://simonwillison.net/2026/Aug/6/datasette/#atom-everything) ⭐️ 8.0/10

Datasette 1.0a38, released on August 6, 2026, fixes a SQL injection vulnerability that allowed users with access to public tables to execute raw SQL queries and read private tables in the same database. The fix is also backported to Datasette 0.65.3. This security fix is critical for Datasette instances that serve a mix of public and private tables, as it prevents unauthorized read access to private data. It highlights the importance of prompt patching and responsible disclosure in open-source data publishing tools. The vulnerability affected instances using the Datasette permissions system to restrict access to private tables. Administrators are advised to disable the execute-sql permission on databases with mixed access to mitigate the issue until the patch is applied.

rss · Simon Willison · Aug 6, 18:24

**Background**: Datasette is an open-source tool for publishing and exploring data, often used to share datasets online. It includes a permissions system to control access to databases and tables, and allows users to execute read-only SQL queries. SQL injection is a common web vulnerability where attackers can manipulate queries to access unauthorized data.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/authentication.html">Authentication and permissions - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/Aug/6/datasette/">Release: datasette 1.0a38 | Simon Willison’s Weblog</a></li>
<li><a href="https://portswigger.net/web-security/sql-injection">What is SQL Injection ? Tutorial & Examples | Web Security Academy</a></li>

</ul>
</details>

**Discussion**: No community comments were provided for this news item.

**Tags**: `#security`, `#datasette`, `#sql-injection`, `#open-source`, `#release`

---

<a id="item-13"></a>
## [Meta Launches Muse Code and Muse Spark 1.2 with Long-Sequence Agentic Tool Calling](https://simonwillison.net/2026/Aug/5/muse-code-and-muse-spark-12/#atom-everything) ⭐️ 8.0/10

Meta has introduced Muse Code, a new AI coding agent, alongside Muse Spark 1.2, an updated coding-focused model. The release emphasizes long-sequence agentic tool calling, with improvements in code generation, debugging, and codebase understanding. This release underscores the growing importance of long-sequence agentic tool calling in AI models, a key capability for complex software engineering tasks. It also introduces a novel pricing model that offers a significant discount for users who allow Meta to use their data, potentially reshaping how AI coding tools are priced and adopted. Muse Spark 1.2 is offered under two model IDs: 'muse-spark-1.2' at $1.25/million input and $4.25/million output, and 'muse-spark-1.2-contributor' at $0.10/$0.20, which requires agreeing to let Meta use your data. The model was co-trained with Muse Code to optimize harness compatibility, and it was trained on long-horizon coding tasks including whole-repository generation and auto-research.

rss · Simon Willison · Aug 5, 23:58

**Background**: Agentic tool calling refers to the ability of an AI model to autonomously select and execute external functions or tools to accomplish tasks, bridging the gap between reasoning and action. Long-sequence agentic tool calling extends this to complex, multi-step workflows, which is crucial for coding agents that need to navigate large codebases and perform end-to-end development tasks. Meta's Muse Spark is a family of coding-focused models, and Muse Code is a new agent built on top of it.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/05/meta-launches-muse-code-ai-coding-agent-for-macos-and-linux/">Meta launches Muse Code AI coding agent for macOS and... - 9to5Mac</a></li>
<li><a href="https://techcrunch.com/2026/08/05/meta-launches-muse-code-an-ai-agent-for-large-code-bases/">Meta launches Muse Code , an AI agent for large code ... | TechCrunch</a></li>
<li><a href="https://www.forbes.com/sites/jonmarkman/2026/08/06/meta-launches-muse-code-a-new-ai-coding-agent-powered-by-spark-12/">Meta Launches Muse Code , A New AI Coding Agent Powered By...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely highlights the significance of long-sequence agentic tool calling and the innovative pricing model. Some may debate the trade-offs of the contributor pricing, while others might focus on the model's performance improvements and the implications for the AI coding agent market.

**Tags**: `#AI`, `#coding agent`, `#Meta`, `#Muse`, `#model release`

---

<a id="item-14"></a>
## [US Probes China's Offshore Access to Nvidia Chips](https://www.bloomberg.com/news/articles/2026-08-07/us-reviews-china-s-offshore-access-to-nvidia-chips-after-ai-breakthroughs) ⭐️ 8.0/10

The US Commerce Department's Bureau of Industry and Security (BIS) has launched a systematic review of how Chinese AI firms access Nvidia chips overseas, including via remote computing. This follows allegations that Chinese AI company Moonshot AI illegally obtained Nvidia chips and accessed them remotely through Thailand. This investigation could lead to new US export controls on cloud computing and remote access to advanced AI chips, potentially reshaping the global AI supply chain. It affects Chinese AI companies, US chipmakers like Nvidia, and cloud service providers, and may escalate US-China tech tensions. BIS is compiling two lists: one of black-market locations suspected of smuggling restricted chips into China, and another of countries where Chinese firms remotely rent chips. The legality of restricting remote access is questionable, but the US House has passed a bipartisan bill to grant that authority, which Nvidia and others may oppose.

telegram · zaihuapd · Aug 7, 11:18

**Background**: The US has imposed export controls on advanced AI chips to limit China's technological and military capabilities. However, these controls do not cover cloud computing, allowing customers to rent chips via services like AWS, Azure, or Google Cloud. The investigation also involves Megaspeed, a Singapore-based company under US investigation for allegedly smuggling Nvidia chips to China, with Alibaba linked through a Cayman entity.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bis.gov/">Homepage | Bureau of Industry and Security</a></li>
<li><a href="https://www.voachinese.com/a/law-makers-introduced-bipartisan-bill-to-close-loophole-in-advanced-ai-chip-export-controls-20260629/8166013.html">voachinese.com/a/law-makers-introduced-bipartisan-bill-to-close...</a></li>
<li><a href="https://hk.on.cc/hk/bkn/cnt/finance/20251223/bkn-20251223115205132-1223_00842_001_cn.html">英 伟 达 东南亚最大合作伙伴 Megaspeed 陷晶 片 走私问题遭美 调 查</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Nvidia`, `#export controls`, `#geopolitics`, `#semiconductors`

---

<a id="item-15"></a>
## [SK Hynix Confirms 375-Layer V10 NAND with Wafer Bonding](https://www.gelonghui.com/live/2599953) ⭐️ 8.0/10

SK Hynix has confirmed that its next-generation V10 NAND flash memory will feature 375-layer stacking, succeeding the 321-layer V9 '4D NAND'. This marks the company's first NAND product to adopt wafer bonding technology, delivering 2.5 times the performance per watt of its predecessor. This milestone is significant for AI infrastructure, as it addresses the growing demand for high-performance, energy-efficient storage. The adoption of wafer bonding technology could set a new industry trend, intensifying competition with rivals like Samsung in the advanced NAND market. The V10 NAND is optimized for AI environments that require both energy efficiency and performance. Mass production of enterprise SSDs based on this technology is scheduled for early 2027, according to industry reports.

telegram · zaihuapd · Aug 7, 12:19

**Background**: NAND flash memory is a type of non-volatile storage used in devices like smartphones and data centers. Wafer bonding is a technique where memory cells and peripheral logic are fabricated separately on different wafers and then bonded vertically, enabling higher layer counts and improved performance. SK Hynix's V10 follows the industry trend toward ultra-high stacking, as seen with Samsung's 400+ layer V10 BV-NAND.

<details><summary>References</summary>
<ul>
<li><a href="https://www.trendforce.com/news/2026/08/05/news-samsung-unveils-industry-first-400-layer-v10-bv-nand-memory-density-up-58-vs-v9/">[News] Samsung Unveils Industry-First 400+ Layer V10 BV- NAND ...</a></li>
<li><a href="https://www.ajupress.com/view/20260805101311102">Samsung, SK hynix wage next battle for AI memory... | Aju Press</a></li>
<li><a href="https://www.techzine.eu/news/infrastructure/143432/samsung-unveils-v10-bv-nand-with-wafer-bonding-and-400-layers/">Samsung unveils V10 BV- NAND with wafer bonding and 400 layers</a></li>

</ul>
</details>

**Tags**: `#NAND flash`, `#SK Hynix`, `#semiconductor`, `#AI infrastructure`, `#memory technology`

---

<a id="item-16"></a>
## [Critical OAuth Account Takeover in sub2api (CVSS 8.8)](https://github.com/Wei-Shaw/sub2api/issues/5350) ⭐️ 8.0/10

sub2api v0.1.171 and earlier contain a critical OAuth account takeover vulnerability (CVSS 8.8) that allows an attacker to bind their OAuth identity to a victim's account using only the victim's email, without password, verification code, or user interaction. This vulnerability enables full account takeover, granting attackers control over API keys, billing balance, and subscription quotas. It poses a severe risk to all sub2api users and highlights a critical flaw in OAuth implementation that could affect other projects using similar pending-session flows. The flaw lies in the pending session flow's existingUser branch, which fails to verify password or verification code, allowing an attacker to set the target user ID to the victim and complete OAuth binding. The vulnerability affects all OAuth providers that route through the pending-session flow, including linux.do, OIDC, WeChat, and DingTalk.

telegram · zaihuapd · Aug 7, 14:59

**Background**: OAuth is a widely used authorization framework that allows users to log in to third-party applications without sharing passwords. In sub2api, the pending-session flow is designed to handle users who are already registered, but the existingUser branch lacks proper authentication checks, enabling the account takeover. This vulnerability is similar to other OAuth account takeover issues that have been reported in various platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://linux.do/t/topic/2721334">sub2api 曝 OAuth ... - LINUX DO</a></li>

</ul>
</details>

**Tags**: `#security`, `#OAuth`, `#vulnerability`, `#account takeover`, `#sub2api`

---

<a id="item-17"></a>
## [Rumor: OpenAI to Launch New Model Astra Next Week](https://t.me/zaihuapd/43046) ⭐️ 8.0/10

According to a rumor from a Telegram channel, OpenAI is preparing to release a new large model named Astra, targeting next week. The model is described as a fresh pretraining and the largest OpenAI has trained since GPT-4.5, with its latest internal test checkpoint codenamed 'mewfour' set as the release candidate. If true, this would mark a significant milestone in AI development, as Astra could be OpenAI's most powerful model yet, potentially advancing capabilities in reasoning, math, and other domains. The release could intensify competition among AI labs and impact industries relying on cutting-edge AI. The rumor originates from an unverified Telegram post, and OpenAI has not officially confirmed the release. The internal codename 'mewfour' has been mentioned in recent AI news discussions, and web search results suggest OpenAI confirmed the Astra name in a math report dated August 1, 2026, describing it as its 'next major model family.'

telegram · zaihuapd · Aug 7, 16:44

**Background**: OpenAI is a leading AI research organization known for developing large language models like GPT-4 and GPT-4.5. Large models are trained on vast datasets to perform tasks such as text generation, reasoning, and problem-solving. The rumored Astra model could represent a new generation of AI, potentially with enhanced capabilities in complex domains like mathematics, as hinted by reports of it solving open math problems.

<details><summary>References</summary>
<ul>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lwMWZQZEVSSDNFeXNYVkZ6YlNDZ0FQAQ?hl=en-IN&gl=IN&ceid=IN:en">Google News - OpenAI Astra model solves ten unsolved math...</a></li>
<li><a href="https://mykreatool.com/en/news/openai-astra-ii-agenty-reshenie-zadach">OpenAI Astra Model Solves 10 Open Math Problems — MyKreaTool</a></li>
<li><a href="https://glm5.app/blog/what-is-openai-astra">What Is OpenAI Astra ? The $2,000 Math Breakthrough... - GLM 5</a></li>
<li><a href="https://www.youtube.com/watch?v=JJvSODvTCes">Grok 4.6 HUGE LEAKS, OpenAI ' mewfour ', GLM... - YouTube</a></li>
<li><a href="https://www.blocktempo.com/openai-astra-model-mewfour-leak-launch-next-week/">OpenAI 傳下週推出最強模型「Astra」！ 內部代號 mewfour ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI model`, `#rumor`, `#GPT-4.5`, `#Astra`

---

<a id="item-18"></a>
## [App Store Rejects App for Nonexistent Tarot Feature](https://daringfireball.net/2026/08/app_store_rejection_of_the_week_dark_hours) ⭐️ 7.0/10

Apple's App Review Board upheld a rejection of developer Godier's app 'Dark Hours' based on the incorrect claim that it includes a live tarot reading feature, despite the app having no such functionality. The rejection persisted even after the developer escalated the issue through multiple levels of appeal. This incident highlights the arbitrary and opaque nature of Apple's App Store review process, which can significantly impact developers' ability to distribute their apps. It underscores ongoing concerns about platform governance and the lack of accountability in app store policies, affecting the broader developer ecosystem. The developer, Godier, escalated the rejection to the App Review Board, which responded that the original rejection was valid because they 'understand that the app includes a live tarot reading feature.' The app has no tarot, horoscope, or astrology-related content, making the rejection factually incorrect.

hackernews · _da_ · Aug 7, 18:59 · [Discussion](https://news.ycombinator.com/item?id=49214863)

**Background**: Apple's App Store review process requires all iOS apps to be approved by Apple's App Review team before publication. Developers often report inconsistent and arbitrary rejection decisions, which can be difficult to resolve. This case exemplifies the challenges developers face when navigating Apple's opaque review guidelines.

<details><summary>References</summary>
<ul>
<li><a href="https://daringfireball.net/2026/08/app_store_rejection_of_the_week_dark_hours">Daring Fireball: App Store Rejection of the Week: Dark Hours</a></li>
<li><a href="https://en.wikipedia.org/wiki/IOS_app_approvals">iOS app approvals - Wikipedia</a></li>
<li><a href="https://creativestrategies.com/apple-and-developer-satisfaction-with-app-store/">Apple and Developer Satisfaction With App Store - Creative Strategies</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration with the arbitrary nature of App Store reviews, with one noting the inconsistency compared to apps like Co-Star, which is entirely astrology-based and was an Editor's Choice. Others highlighted the broader problem of gatekeeping by two major companies and pointed to the Keep Android Open movement as a response.

**Tags**: `#App Store`, `#Developer Experience`, `#Platform Governance`, `#Mobile Apps`

---

<a id="item-19"></a>
## [GPT-5.6 Sol Ultra Outshines Claude Fable 5 in Raccoon Heist Game Test](https://simonwillison.net/2026/Aug/7/moonlight-mayhem/#atom-everything) ⭐️ 7.0/10

Simon Willison used the exact same prompt to generate a raccoon heist game with both Claude Fable 5 and GPT-5.6 Sol Ultra (via Codex Desktop), finding that GPT-5.6 Sol Ultra produced a much better game. The resulting game, 'Moonlight & Mayhem', is available online with its GitHub repository. This comparison highlights the rapid advancement in AI coding capabilities, showing that newer models like GPT-5.6 Sol Ultra can generate more complex and polished applications from a single prompt. It provides practical evidence for developers evaluating AI-assisted development tools and models. GPT-5.6 Sol Ultra's version features a museum heist where the player rescues raccoon crewmates to stack up and steal a golden sardine, whereas Claude Fable 5's version was a simpler backyard coin collection. However, the one-shot GPT-5.6 Sol Ultra version had a bug with oversized eyeballs, which was fixed by prompting 'Why do the raccoons have huge black spheres on them?' and then 'Fix it'. The Codex session took 52 minutes and would have cost $23.28 at full API prices.

rss · Simon Willison · Aug 7, 19:18

**Background**: AI coding agents like Claude Code and Codex Desktop can generate complete applications from natural language prompts. GPT-5.6 Sol Ultra is OpenAI's latest coding model, which uses sub-agents to handle complex tasks in parallel, and has set a new state-of-the-art on the Artificial Analysis Coding Agent Index. This test is part of a broader trend of using LLMs for one-shot game development.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/gpt-5-6/">GPT - 5 . 6 : Frontier intelligence that scales with your ambition | OpenAI</a></li>
<li><a href="https://openai.com/index/introducing-the-codex-app/">Introducing the Codex app | OpenAI</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai/ codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**Tags**: `#AI coding`, `#GPT-5.6`, `#Claude`, `#game generation`, `#LLM comparison`

---

<a id="item-20"></a>
## [Tokenpocalypse: Companies Scramble to Cut AI Token Costs](https://simonwillison.net/2026/Aug/7/pdfs-are-terrible/#atom-everything) ⭐️ 7.0/10

A 404 Media article reports that companies are struggling with rising AI token costs, citing Accenture's internal discussions about non-engineers driving token usage and the inefficiency of converting PDFs to markdown. This highlights a significant industry trend where AI token costs are becoming a major concern for enterprises, potentially impacting AI adoption and prompting more efficient practices. The anecdote from Accenture provides practical insight into how non-technical staff and inefficient document processing contribute to rising costs. The article mentions that Accenture's data shows non-engineers are driving token consumption, and converting PDFs to markdown is a major token consumer. The discussion suggests that PDFs are a terrible medium for communicating information, and converting them to markdown can reduce token usage by 33% to 90% depending on the source.

rss · Simon Willison · Aug 7, 16:18

**Background**: AI tokens are the units of text that language models process, and they cost money because every API call charges per token. Converting PDFs to markdown before feeding to AI can significantly reduce token usage by removing formatting noise, as shown by various sources. This is part of a broader trend where companies are seeking to optimize AI costs as they scale usage.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://www.mindstudio.ai/blog/convert-files-markdown-reduce-ai-tokens">How to Convert Files to Markdown to Reduce AI Token Usage by Up...</a></li>
<li><a href="https://www.mdspin.app/guides/convert-pdf-for-chatgpt">How to Convert PDFs for ChatGPT, Claude & Gemini | MDSpin</a></li>

</ul>
</details>

**Tags**: `#AI costs`, `#token consumption`, `#enterprise AI`, `#PDF processing`, `#industry trends`

---

<a id="item-21"></a>
## [Claude Fable 5 Relaunch Faces Quality Complaints and Safety Misjudgments](https://t.me/zaihuapd/43026) ⭐️ 7.0/10

After the US lifted export controls, Anthropic's flagship model Claude Fable 5 has been relaunched, but users report degraded performance and frequent safety misjudgments. During the transition period until July 7, Pro and Max subscribers can only use 50% of their weekly quota for this model, and after that date it will no longer be included in subscriptions, requiring pay-per-use. This matters because it affects a wide range of developers and enterprises relying on Claude Fable 5 for complex tasks, and the subscription changes could increase costs and reduce accessibility. The safety misjudgments, especially around code-related keywords, undermine trust in the model's reliability for technical work. The model automatically downgrades when handling C/C++, Rust low-level code, or when keywords like 'vulnerability' or 'hook' appear, leading to degraded output. Anthropic cites compute constraints as the reason for the quota reduction, promising to reinstate subscription access once capacity improves.

telegram · zaihuapd · Aug 7, 06:05

**Background**: Claude Fable 5 is Anthropic's most capable generally available model, released on June 9, 2026, and is designed for ambitious, long-running, asynchronous work. On June 12, 2026, the Trump administration imposed an export control directive that forced Anthropic to pull its two most advanced models offline, but a federal court later granted a preliminary injunction, leading to the relaunch.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://boesl.org/en/anthropic-export-control-claude-fable-mythos/">Anthropic Export Control on Claude Fable and Mythos 5</a></li>
<li><a href="https://www.trymurph.com/insights/the-anthropic-export-ban-wasn-t-about-security-it-was-about-control">The Anthropic Export Ban Wasn't About Security. It Was About...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#model deployment`, `#safety`

---

<a id="item-22"></a>
## [Nasdaq Seeks 23-Hour Trading, Following NYSE's 22-Hour Approval](https://t.me/zaihuapd/43037) ⭐️ 7.0/10

On December 15, Nasdaq filed an application with the U.S. SEC to extend its trading hours to 23 hours on weekdays, proposing to open trading from 9:00 PM to 4:00 AM Eastern Time. If approved, the extended hours are expected to launch in early Q3 2026. This move signals a major shift toward near-24/7 stock trading, which could reshape market dynamics, trading technology, and investor behavior. It follows NYSE's preliminary approval for 22-hour trading, indicating a broader industry trend toward extended sessions. The proposed hours would add to existing pre-market, regular, and after-hours sessions, bringing total weekday trading to 23 hours. Nasdaq expects to launch the extended hours in early Q3 2026, pending SEC approval, while NYSE has already received preliminary approval for 22-hour trading.

telegram · zaihuapd · Aug 7, 10:03

**Background**: Extended trading hours refer to trading sessions outside the official market open, such as pre-market and after-hours. During the pandemic, platforms like Robinhood began offering 24-hour stock trading via over-the-counter systems, increasing demand for round-the-clock access. Regulatory approval from the SEC is required for exchanges to extend their official trading hours.

<details><summary>References</summary>
<ul>
<li><a href="https://www.poems.com.sg/zh-hans/market-journal/night-owls-and-early-birds/">夜鹰先行，晨鸟先机： 延 长 交 易 时 段 指南 - POEMS</a></li>
<li><a href="https://tg.sizhefu.com/posts/347">纳 斯 达 克 申请将 交 易 时 间 延 长 至 23 小 时 美国 纳 斯 达 克 交 易 所 12 月 15...</a></li>
<li><a href="https://www.weiyangx.com/446175.html">纳 斯 达 克 拟将 交 易 时 间 延 长 至24... | 未央网</a></li>

</ul>
</details>

**Tags**: `#finance`, `#trading`, `#regulation`, `#fintech`, `#stock market`

---

<a id="item-23"></a>
## [Amazon Cracks Down on Internal CPU Waste as Agentic AI Drives Demand](https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity) ⭐️ 7.0/10

Amazon Web Services (AWS) has begun cracking down on internal CPU waste among its engineers, requiring them to reduce inefficient use of EC2 instances to ensure capacity for customers. This has led to longer wait times for internal instance requests, from hours to days. This shift highlights the growing impact of agentic AI workloads, which require more CPU resources relative to GPUs, potentially reshaping cloud infrastructure strategies and costs. It signals that CPU demand is becoming a critical factor in AI infrastructure planning, affecting both cloud providers and enterprises. The GPU-to-CPU ratio in data centers is shifting from 8:1 or 4:1 toward 1:1 due to agentic AI workloads, which involve extensive tool calls and complex GPU orchestration running on CPUs. AMD and Nvidia are both increasing their data center CPU offerings to compete in this market.

telegram · zaihuapd · Aug 7, 16:31

**Background**: Agentic AI refers to AI systems that can autonomously perform tasks by calling tools and orchestrating workflows, unlike traditional chatbot-style AI that primarily relies on GPU-heavy inference. These workloads require more CPU for orchestration, memory management, and data movement, increasing the importance of CPU resources in AI infrastructure. AWS uses various CPU types in its EC2 instances, including AMD, Intel, and its own Graviton chips.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/pc-components/cpus/amazon-cracks-down-on-cpu-waste-among-engineers-as-agentic-ai-crunch-intensifies-cpu-demand-makes-low-utilization-ec2-instances-a-hot-commodity">Amazon cracks down on ' CPU waste ' among... | Tom's Hardware</a></li>
<li><a href="https://www.linkedin.com/posts/akashborate_understanding-how-agentic-ai-is-rewriting-activity-7474321519674826752-RgCw">Agentic AI Breaks CPU -to- GPU Rule | Akash Borate posted... | LinkedIn</a></li>
<li><a href="https://www.computeforecast.com/Opinion/meta-graviton-cpu-ai-infrastructure-shortage-underestimated/">Meta Graviton Deal Reveals the CPU Shortage Nobody Modelled</a></li>

</ul>
</details>

**Tags**: `#AWS`, `#CPU`, `#AI infrastructure`, `#agentic AI`, `#cloud computing`

---