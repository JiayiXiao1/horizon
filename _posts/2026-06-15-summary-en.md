---
layout: default
title: "Horizon Summary: 2026-06-15 (EN)"
date: 2026-06-15
lang: en
---

> From 34 items, 17 important content pieces were selected

---

1. [Pyodide 314.0 Enables Direct WASM Wheel Publishing to PyPI](#item-1) ⭐️ 9.0/10
2. [Rio's Homegrown LLM Exposed as Weighted Merge](#item-2) ⭐️ 8.0/10
3. [Jane Street on Formal Methods and AI Code](#item-3) ⭐️ 8.0/10
4. [The Birth and Death of JavaScript (2014) Talk](#item-4) ⭐️ 8.0/10
5. [AI Hasn't Replaced Software Engineers, Data Shows](#item-5) ⭐️ 8.0/10
6. [Over 75 US data center projects worth $130B blocked in Q1 2026](#item-6) ⭐️ 8.0/10
7. [Huawei Open-Sources Pangu 2.0 Model, Targets Global Leadership](#item-7) ⭐️ 8.0/10
8. [US Government Orders Anthropic to Block Two AI Models](#item-8) ⭐️ 8.0/10
9. [First Global Map of Underground Fungal Networks Revealed](#item-9) ⭐️ 8.0/10
10. [Adobe's Overly Strict EPUB Validation Causes False Errors on Kobo](#item-10) ⭐️ 7.0/10
11. [Local ML Indexes 669 GB of GoPro Videos on M1 Max](#item-11) ⭐️ 7.0/10
12. [How to Earn a Billion Dollars](#item-12) ⭐️ 7.0/10
13. [Not Everyone Is Using AI Extensively, Data Shows](#item-13) ⭐️ 7.0/10
14. [Mapping SQLite Result Columns to Source Tables](#item-14) ⭐️ 7.0/10
15. [OpenRouter Fusion Router: Claude-level intelligence at half cost](#item-15) ⭐️ 7.0/10
16. [Krugman: Musk is a 'Human Ponzi Scheme', SpaceX IPO Forces Ordinary Investors](#item-16) ⭐️ 7.0/10
17. [Australia's teen social media ban fails after 4 months](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Pyodide 314.0 Enables Direct WASM Wheel Publishing to PyPI](https://simonwillison.net/2026/Jun/13/publishing-wasm-wheels/#atom-everything) ⭐️ 9.0/10

Pyodide 314.0 allows Python package maintainers to publish WebAssembly (WASM) wheels directly to PyPI, using the new pyemscripten platform tag defined in PEP 783. Previously, Pyodide maintainers had to manually build and host over 300 packages. This removes a major bottleneck for Python in the browser, enabling the broader Python ecosystem to distribute packages for Pyodide without manual intervention. It significantly reduces the maintenance burden on Pyodide maintainers and accelerates the availability of new packages. The feature is supported by a PR to PyPI's warehouse repository that landed on April 21st. Simon Willison demonstrated the workflow by publishing a luau-wasm package, which can be installed in Pyodide via micropip install.

rss · Simon Willison · Jun 13, 23:55

**Background**: Pyodide is a Python distribution for the browser and Node.js based on WebAssembly. PEP 783 defines the pyemscripten platform tag for binary Python packages compiled to WebAssembly. Previously, distributing such packages required manual hosting and maintenance by Pyodide maintainers.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 314.0.0</a></li>
<li><a href="https://peps.python.org/pep-0783/">PEP 783 – Emscripten Packaging - Python Enhancement Proposals</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the article) shows high engagement and positive sentiment, with many users expressing excitement about the removal of this long-standing limitation. Some commenters noted the potential for more complex Python packages to run in the browser.

**Tags**: `#Pyodide`, `#WebAssembly`, `#Python`, `#PyPI`, `#package distribution`

---

<a id="item-2"></a>
## [Rio's Homegrown LLM Exposed as Weighted Merge](https://github.com/nex-agi/Nex-N2/issues/4) ⭐️ 8.0/10

An investigation revealed that Rio de Janeiro's claimed homegrown LLM, Rio-3.5-Open-397B, is actually a weighted merge of approximately 60% Nex-N2 Pro and 40% Qwen3.5-397B-A17B, with no additional training. This raises serious questions about transparency and attribution in AI development, especially for public sector projects claiming homegrown innovation. It also highlights the growing practice of model merging, which can blur the lines between original work and derivative models. Every weight tensor in the Rio model was found to be, to thousands of standard deviations, the same 0.6/0.4 blend of Nex and Qwen across all 60 layers. The model was presented as a fine-tune of Qwen3.5 but no distillation or training was applied to the released version.

hackernews · unrvl22 · Jun 14, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48528371)

**Background**: Model merging is a technique that combines the weights of two or more pre-trained models into a single model without additional training, often using methods like linear interpolation or SLERP. It can improve performance on multiple tasks but raises attribution concerns when the merged model is presented as original work. The municipality of Rio de Janeiro released the model via its IT company IplanRIO.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2212.09849">[2212.09849] Dataless Knowledge Fusion by Merging Weights of Language Models</a></li>
<li><a href="https://developer.nvidia.com/blog/an-introduction-to-model-merging-for-llms/">An Introduction to Model Merging for LLMs | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether the lack of disclosure was intentional or a misunderstanding, with some noting that the claimed improvements likely came from on-policy distillation that was not included in the uploaded model. Others expressed frustration over the lack of proper attribution, while a few found it remarkable that a simple linear combination of weights could enhance performance without degradation.

**Tags**: `#LLM`, `#open-source`, `#AI ethics`, `#model merging`, `#transparency`

---

<a id="item-3"></a>
## [Jane Street on Formal Methods and AI Code](https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1) ⭐️ 8.0/10

Jane Street published a blog post discussing the growing importance of formal methods in programming, especially with the rise of AI-generated code. The post highlights how formal verification can help manage the verification bottleneck and improve code quality. This discussion is significant because it addresses a critical challenge in modern software engineering: ensuring the correctness of AI-generated code. Formal methods could shift the role of human developers from writing code to verifying it, potentially transforming the software development lifecycle. The blog post is part of a series on formal methods at Jane Street, a firm known for using OCaml. It notes that types are already valuable when programming with AI agents, and more powerful proof techniques could offer even greater benefits.

hackernews · eatonphil · Jun 14, 12:35 · [Discussion](https://news.ycombinator.com/item?id=48526633)

**Background**: Formal methods are mathematically based techniques for specifying, developing, and verifying software and hardware systems. They use logic, type theory, and automated theorem proving to ensure correctness. Jane Street, a quantitative trading firm, has long been a proponent of OCaml and formal verification in production.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.janestreet.com/formal-methods-at-jane-street-index/?from_theconsensus=1">Jane Street Blog - Formal methods and the future of programming</a></li>
<li><a href="https://en.wikipedia.org/wiki/Formal_methods">Formal methods - Wikipedia</a></li>
<li><a href="https://users.ece.cmu.edu/~koopman/des_s99/formal_methods/">Formal Methods - Electrical and Computer Engineering</a></li>

</ul>
</details>

**Discussion**: Community comments reflect a mix of experience and skepticism. One commenter recalls early proof automation tools like the Boyer-Moore prover, while another notes that formal specs can feel like writing tests in a different way. A third commenter highlights the potential for formal methods to help non-native English speakers verify AI-generated code.

**Tags**: `#formal methods`, `#programming`, `#verification`, `#AI`, `#software engineering`

---

<a id="item-4"></a>
## [The Birth and Death of JavaScript (2014) Talk](https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript) ⭐️ 8.0/10

Gary Bernhardt's 2014 PyCon talk humorously predicts JavaScript's evolution into a compilation target and its eventual replacement by WebAssembly and TypeScript, which has largely come true. The talk's prescient insights have proven accurate, influencing how developers think about JavaScript's role and the future of web development. The talk traces JavaScript's history from 1995 to 2035, mixing comedy with serious analysis, and correctly foresaw asm.js (later WebAssembly) and the rise of compile-to-JS languages.

hackernews · subset · Jun 14, 12:38 · [Discussion](https://news.ycombinator.com/item?id=48526661)

**Background**: JavaScript was created in 1995 as a simple scripting language for browsers, but over time it became the dominant language for web development. However, its limitations led to the creation of compile-to-JS languages like TypeScript and alternative runtimes like WebAssembly, which allow other languages to run in the browser.

<details><summary>References</summary>
<ul>
<li><a href="https://www.destroyallsoftware.com/talks/the-birth-and-death-of-javascript">The Birth & Death of JavaScript</a></li>
<li><a href="https://en.wikipedia.org/wiki/WebAssembly">WebAssembly - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/WebAssembly/Guides/Rust_to_Wasm">Compiling from Rust to WebAssembly - WebAssembly | MDN</a></li>

</ul>
</details>

**Discussion**: Commenters praised the talk's accuracy, noting that JavaScript indeed became a compilation target and that WebAssembly fulfilled the prediction. Some also referenced Bernhardt's earlier 'Wat' talk as a classic.

**Tags**: `#JavaScript`, `#WebAssembly`, `#Programming Languages`, `#Tech Talk`, `#Prediction`

---

<a id="item-5"></a>
## [AI Hasn't Replaced Software Engineers, Data Shows](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that data does not support the narrative that AI will cause mass layoffs in software engineering, citing New York's WARN Act filings where zero out of 160+ companies checked the AI disclosure box in the first year. This evidence-based counterargument challenges the prevailing narrative of AI-driven job displacement, especially in a profession considered uniquely vulnerable to automation, and suggests that other sectors may be even more insulated. The authors identify three real bottlenecks in software engineering that resist automation: deciding and specifying what to build, verifying and being accountable for deliverables, and deep human understanding of the codebase, business, and environment.

rss · Simon Willison · Jun 14, 23:54

**Background**: The WARN Act requires companies to provide 60-day advance notice of mass layoffs. In March 2025, New York became the first U.S. state to add an AI disclosure checkbox to WARN filings, asking whether technological innovation or automation contributed to layoffs. Despite widespread fears, no company has checked that box in the first year.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>
<li><a href="https://opentools.ai/news/new-yorks-ai-layoff-disclosure-law-0-compliance-shocking-revelations">New York's AI Layoff Disclosure Law: 0 Compliance, Shocking Revelations! | AI News</a></li>
<li><a href="https://www.softwareseni.com/why-ai-layoff-disclosure-laws-are-not-working-and-what-would-actually-fix-them/">Why AI Layoff Disclosure Laws Are Not Working and What Would Actually Fix Them - SoftwareSeni</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#employment`, `#job displacement`, `#evidence-based`

---

<a id="item-6"></a>
## [Over 75 US data center projects worth $130B blocked in Q1 2026](https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs) ⭐️ 8.0/10

In the first quarter of 2026, more than 75 data center construction projects worth approximately $130 billion were blocked or delayed across the United States, matching the total for all of 2025. Grassroots opposition groups surged from 396 to 833 in three months, spanning 49 states. This wave of opposition signals a major shift in public and political sentiment toward data center expansion, driven by fears of soaring energy costs, water consumption, and environmental impact. It could slow the buildout of AI infrastructure and force the industry to adopt more sustainable practices. The blocked projects represent about $130 billion in value, and the number of active grassroots opposition groups reached 833 across 49 states. State legislatures have introduced numerous regulatory bills, and some federal lawmakers have proposed moratoriums on data center construction.

telegram · zaihuapd · Jun 14, 03:03

**Background**: Data centers consume massive amounts of electricity and water, and their rapid expansion has raised concerns about grid strain, rate hikes, and environmental degradation. In the U.S., data center electricity demand is projected to grow significantly, prompting bipartisan opposition at local and state levels. Proponents argue that concerns are overblown and that data centers bring economic benefits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/more-than-75-data-center-build-outs-worth-usd130-billion-have-been-successfully-blocked-in-the-first-four-months-of-2026-bipartisan-opposition-mounts-nationwide-over-fears-of-soaring-power-and-water-costs">More than 75 data center build-outs worth $130 billion have been successfully blocked in the first three months of 2026 — bipartisan opposition mounts nationwide over fears of soaring power and water costs | Tom's Hardware</a></li>
<li><a href="https://arstechnica.com/tech-policy/2026/06/130-billion-in-data-center-projects-blocked-by-protests-so-far-this-year/">$130 billion in data center projects blocked by protests so far this year - Ars Technica</a></li>
<li><a href="https://www.carbon-direct.com/insights/data-centers-and-their-energy-use-trends-in-state-capitals">Data centers and their energy use: Trends in state capitals | Carbon Direct</a></li>

</ul>
</details>

**Tags**: `#data centers`, `#energy policy`, `#AI infrastructure`, `#regulation`, `#environment`

---

<a id="item-7"></a>
## [Huawei Open-Sources Pangu 2.0 Model, Targets Global Leadership](https://t.me/zaihuapd/41948) ⭐️ 8.0/10

At Huawei Developer Conference 2026, Huawei announced the open-source release of the openPangu 2.0 model, including a 505B-parameter Pro version and a 92B-parameter Flash version, supporting a 512K context window. The company plans to open-source seven major components, including pre-training code, starting June 30. This release marks a major step in Huawei's AI strategy, challenging global leaders like GPT-4 and Llama with a fully open-source, domestically-produced large model. It strengthens China's AI ecosystem by providing a high-performance alternative to NVIDIA-based solutions, leveraging Huawei's Ascend chips and HarmonyOS. The 505B Pro model is one of the largest open-source LLMs globally, while the 92B Flash version offers a more efficient option. The 512K context window enables processing of extremely long documents, such as entire books or lengthy codebases. The model is optimized for Huawei's Ascend AI chips and HarmonyOS.

telegram · zaihuapd · Jun 14, 08:05

**Background**: Large language models (LLMs) like GPT-4 have transformed AI, but most leading models are developed by US companies and require expensive NVIDIA GPUs. Huawei's Ascend chips are a domestic alternative, and openPangu 2.0 is designed to run efficiently on this hardware. The 512K context window is significantly larger than typical models (e.g., GPT-4's 128K), allowing the model to handle more information at once.

<details><summary>References</summary>
<ul>
<li><a href="https://thamizhelango.medium.com/mindspore-zhipu-ai-huawei-ascend-how-china-built-a-frontier-ai-model-without-a-single-nvidia-68403d92cedb">MindSpore, Zhipu AI & Huawei Ascend : How China Built... | Medium</a></li>
<li><a href="https://www.bitrue.com/blog/huawei-ascend-ai-chip-specs-2025">Huawei Ascend AI Chips : Specifications, Models, and Performance in...</a></li>
<li><a href="https://www.reddit.com/r/LocalLLaMA/comments/1eplndh/what_is_the_current_largest_context_window_for_an/">What is the current largest context window for an open LLM? : r/LocalLLaMA - Reddit</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#large language model`, `#Huawei`, `#Pangu`

---

<a id="item-8"></a>
## [US Government Orders Anthropic to Block Two AI Models](https://t.me/zaihuapd/41949) ⭐️ 8.0/10

The US government, citing national security, issued an export control directive to Anthropic, ordering the company to restrict access to its Fable 5 and Mythos 5 AI models for all customers, including foreign employees. Anthropic has complied by shutting down access to these models while other Claude models remain unaffected. This marks a significant escalation in government intervention over advanced AI models, setting a precedent for export controls on AI capabilities. It impacts businesses and researchers relying on these models and highlights growing tensions between AI innovation and national security. The directive specifically targets Fable 5 and Mythos 5, with the Commerce Department citing concerns over security risks if the models are jailbroken. Anthropic stated it is working to restore access as soon as possible, but all customers, including foreign employees, are currently blocked.

telegram · zaihuapd · Jun 14, 09:06

**Background**: Anthropic's Mythos-class models, including Mythos 5, are designed for advanced cybersecurity tasks such as finding software vulnerabilities. Fable 5 is a safer, publicly released version of the Mythos class. The US government has been increasingly using export controls to limit access to advanced AI technologies, especially to prevent adversaries from gaining capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://www.euronews.com/my-europe/2026/06/14/us-export-controls-on-anthropic-should-not-be-discriminatory-eu-commission-warns">US export controls on Anthropic 'should not be... | Euronews</a></li>
<li><a href="https://www.americanactionforum.org/insight/ai-export-controls-balancing-national-security-and-ai-innovation/">AI Export Controls : Balancing National Security and AI Innovation...</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export control`, `#national security`, `#Anthropic`, `#AI safety`

---

<a id="item-9"></a>
## [First Global Map of Underground Fungal Networks Revealed](https://insideclimatenews.org/news/11062026/earths-massive-underground-fungal-networks/) ⭐️ 8.0/10

Scientists from the Society for the Protection of Underground Networks (SPUN) have created the first global map of arbuscular mycorrhizal fungal networks, estimating their total length at 110 quintillion kilometers and their mass at about five times the weight of all humans on Earth. This map reveals the immense scale and carbon storage capacity of underground fungal networks, which sequester about 1 billion tons of carbon annually, highlighting their critical role in climate change mitigation and ecosystem health. The map shows that fungal density in farmland is only half that of wild ecosystems, and wild grasslands, which hold about 40% of the world's arbuscular mycorrhizal fungal biomass, are being converted to farmland four times faster than forests.

telegram · zaihuapd · Jun 14, 14:58

**Background**: Arbuscular mycorrhizal fungi form symbiotic relationships with about 80% of land plants, extending plant root systems and helping them absorb water and nutrients. These fungi also store carbon in their extensive underground networks, making them important for climate regulation.

<details><summary>References</summary>
<ul>
<li><a href="https://news.sciencenet.cn/htmlnews/2023/4/498730.shtm">地上地下搭起“通讯 网 ” 植物间交流无处不在—新闻—科学 网</a></li>
<li><a href="https://madechango.com/study-guide/view/2108">Threads of underground fungal networks are long enough to reach...</a></li>

</ul>
</details>

**Tags**: `#ecology`, `#climate change`, `#mycology`, `#carbon sequestration`, `#research`

---

<a id="item-10"></a>
## [Adobe's Overly Strict EPUB Validation Causes False Errors on Kobo](https://andreklein.net/your-epub-is-fine-kobo-disagrees-blame-adobe/) ⭐️ 7.0/10

A technical deep-dive reveals that Adobe's EPUB validation tool (based on RMSDK) is overly strict, flagging valid EPUB files as erroneous, which causes display issues on Kobo devices. This issue affects Kobo users who rely on Adobe's validation, leading to frustration and wasted time. It also highlights broader concerns about Adobe's software quality and QA practices. The article explains that Adobe's RMSDK (Reader Mobile SDK) enforces stricter rules than the EPUB standard requires, causing false positives. Workarounds include using kepubify or alternative devices like the PineNote.

hackernews · sohkamyung · Jun 14, 22:54 · [Discussion](https://news.ycombinator.com/item?id=48533848)

**Background**: EPUB is a widely used open standard for ebooks. Adobe's RMSDK is a proprietary rendering engine used by many ereaders, including Kobo. Validation tools like EPUBCheck check compliance with the standard, but Adobe's implementation adds extra checks that can reject valid files.

<details><summary>References</summary>
<ul>
<li><a href="https://www.epubconversion.com/epub-validator/">Free ePub validator | ePub checker | validate ePub format ebooks</a></li>
<li><a href="https://hmdpublishing.com/education/tools/epub-validator">Free EPUB Validator & Fixer Online — Check EPUB 2.0 & 3.0 Files</a></li>

</ul>
</details>

**Discussion**: Commenters note that Adobe has a history of poor QA, citing Flash as an example. Some suggest using kepubify to convert EPUBs to Kobo's native format, while others recommend the PineNote device for more open software.

**Tags**: `#ePub`, `#Adobe`, `#Kobo`, `#ebooks`, `#software quality`

---

<a id="item-11"></a>
## [Local ML Indexes 669 GB of GoPro Videos on M1 Max](https://news.ycombinator.com/item?id=48528029) ⭐️ 7.0/10

A developer indexed 628 GoPro videos (669 GB, 15+ hours of footage) on an M1 Max MacBook using open-source ML models, enabling search and automatic compilation of highlights into a DaVinci Resolve timeline. This demonstrates that powerful local AI video indexing is now feasible on consumer hardware, offering privacy and offline capabilities that cloud services cannot match, and opens up new workflows for content creators and archivists. The pipeline processes 1 frame per second, analyzing 57,537 frames total, with a total compute time of 67 hours and 40 minutes. It uses open-source ML models for scene detection and semantic search, and outputs selected clips directly to DaVinci Resolve.

hackernews · iliashad · Jun 14, 15:13

**Background**: Video indexing traditionally requires manual tagging or expensive cloud AI services. Local ML models, such as those used in this project, run entirely on the user's machine, preserving privacy and avoiding recurring costs. The M1 Max's unified memory and Neural Engine accelerate these workloads significantly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Machine_learning">Machine learning - Wikipedia</a></li>
<li><a href="https://www.creativeainews.com/blog/framedex-local-video-indexing-gemma-4-claude-code-2026/">Framedex: Local Video Indexing with Gemma 4 and Claude</a></li>
<li><a href="https://github.com/bryanrandell/DaVinci-Resolve-Timeline-Utility">GitHub - bryanrandell/ DaVinci - Resolve - Timeline -Utility: Switch quickly...</a></li>

</ul>
</details>

**Discussion**: Commenters noted similar projects (e.g., Framedex) and pointed out that DaVinci Resolve 21 already includes built-in AI indexing (IntelliSearch), though only in the Studio version. Some questioned the practicality of processing 67 hours locally versus using cloud acceleration, while others expressed enthusiasm for local AI video tools.

**Tags**: `#machine learning`, `#video indexing`, `#local AI`, `#GoPro`, `#M1 Max`

---

<a id="item-12"></a>
## [How to Earn a Billion Dollars](https://paulgraham.com/earn.html) ⭐️ 7.0/10

Paul Graham published an essay arguing that earning a billion dollars requires creating value at scale, typically through technology startups that solve real problems. This essay sparks debate on the ethics and mechanics of extreme wealth creation, influencing how entrepreneurs and the public perceive billion-dollar fortunes. The essay received 452 points and 1372 comments on Hacker News, with mixed discussion quality including insightful counterpoints about wealth extraction and moral semantics.

hackernews · kingstoned · Jun 14, 11:50 · [Discussion](https://news.ycombinator.com/item?id=48526360)

**Background**: Paul Graham is a well-known venture capitalist and essayist, co-founder of Y Combinator. His essays often explore startup dynamics and wealth creation. The term 'earn' in this context is debated, as critics argue that billion-dollar fortunes often involve extraction rather than pure value creation.

**Discussion**: Comments show a split: some defend Graham's value-creation thesis, while others argue that billion-dollar fortunes inherently involve exploitation or semantic manipulation of 'earn'. A few users humorously calculate extreme growth scenarios to illustrate the concept.

**Tags**: `#wealth creation`, `#startups`, `#entrepreneurship`, `#economics`, `#Paul Graham`

---

<a id="item-13"></a>
## [Not Everyone Is Using AI Extensively, Data Shows](https://gabrielweinberg.com/p/people-are-consuming-ai-like-they) ⭐️ 7.0/10

An article argues that despite AI's capabilities, many people are not using it extensively, citing data showing over 50% of respondents use AI less than once per week. This challenges the prevailing AI hype narrative and reveals a gap between perceived and actual adoption, which has implications for product design, workplace policies, and investment strategies. The article uses data from surveys and personal anecdotes to show that AI usage is not universal, and that many people still rely on traditional methods or use AI infrequently.

hackernews · yegg · Jun 14, 14:44 · [Discussion](https://news.ycombinator.com/item?id=48527700)

**Background**: Since the release of ChatGPT in late 2022, there has been widespread speculation that AI is rapidly transforming work and daily life. However, actual adoption data often lags behind the hype, and many users remain skeptical or uncertain about how to integrate AI effectively.

**Discussion**: Commenters share mixed experiences: some find AI helpful with supervision, others feel pressure to use it or fear being left out. A key insight is that AI adoption may grow more through embedded features in existing software than through standalone chat interfaces.

**Tags**: `#AI adoption`, `#technology trends`, `#workplace`, `#LLMs`, `#skepticism`

---

<a id="item-14"></a>
## [Mapping SQLite Result Columns to Source Tables](https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/#atom-everything) ⭐️ 7.0/10

Simon Willison explored methods to programmatically map SQL query result columns back to their source table.column, using Claude Code (Opus 4.8) to find solutions via APSW, ctypes, and EXPLAIN analysis. This technique could enable Datasette to enrich arbitrary SQL query results with column provenance information, improving data understanding and debugging for users. The solutions include using the APSW library, accessing SQLite's sqlite3_column_table_name() C function via ctypes, and parsing EXPLAIN output to infer column origins.

rss · Simon Willison · Jun 13, 23:05

**Background**: Datasette is a tool for exploring and publishing SQLite databases. Column provenance refers to identifying which table and column each result column originates from, which is not natively exposed by SQLite's Python interface.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/13/sqlite-column-provenance/">Research: Mapping SQLite result columns back to their source `table.column`</a></li>
<li><a href="https://docs.datasette.io/en/stable/sql_queries.html">Running SQL queries - Datasette documentation</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#Datasette`, `#SQL`, `#AI-assisted development`, `#column provenance`

---

<a id="item-15"></a>
## [OpenRouter Fusion Router: Claude-level intelligence at half cost](https://x.com/i/status/2065856853989270011) ⭐️ 7.0/10

OpenRouter has introduced the Fusion Router (openrouter/fusion), a multi-model negotiation system that achieves intelligence comparable to Claude Fable at roughly half the cost by running parallel model calls and consensus analysis. This innovation could significantly reduce the cost of high-quality AI inference, making advanced intelligence more accessible to developers and enterprises, and potentially reshaping LLM routing strategies across the industry. The Fusion Router works by having a primary model decide when to invoke a panel of models in parallel, then a judge model compares their responses to produce structured analysis (consensus, contradictions, etc.). The cost is about 4-5 times that of a single completion, and internal calls do not trigger recursion.

telegram · zaihuapd · Jun 14, 01:21

**Background**: OpenRouter is a platform that provides unified access to various large language models (LLMs). The Fusion Router extends this by enabling multi-model deliberation, where multiple models collaborate to produce more reliable answers. This approach is similar to ensemble methods in machine learning, but applied to LLM inference.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/docs/guides/routing/routers/fusion-router">Fusion Router | Multi-model AI... | OpenRouter | Documentation</a></li>
<li><a href="https://openrouter.ai/docs/guides/features/plugins/fusion">Fusion | Multi-model AI Analysis with... | OpenRouter | Documentation</a></li>
<li><a href="https://writingmate.ai/models/openrouter/fusion">OpenRouter : Fusion - AI Model Details | Writingmate</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#OpenRouter`, `#model routing`, `#AI inference`, `#multi-model`

---

<a id="item-16"></a>
## [Krugman: Musk is a 'Human Ponzi Scheme', SpaceX IPO Forces Ordinary Investors](https://paulkrugman.substack.com/p/elon-musk-human-ponzi-scheme) ⭐️ 7.0/10

Nobel laureate Paul Krugman published an opinion piece arguing that Elon Musk's unfulfilled promises constitute a 'human Ponzi scheme', and that SpaceX's upcoming IPO at a $1.77 trillion valuation, combined with index rule changes, will force ordinary investors to buy in through index funds. This critique from a prominent economist highlights concerns about market distortions caused by passive investing and the valuation of high-profile private companies. It could influence public debate on index fund mechanics and the accountability of visionary entrepreneurs. SpaceX reportedly had only $18.7 billion in revenue last year and remains unprofitable, yet its IPO valuation is $1.77 trillion. Index providers like Nasdaq 100 and FTSE Russell have recently modified rules to allow rapid inclusion of SpaceX, meaning index-tracking funds must buy its shares.

telegram · zaihuapd · Jun 14, 04:52

**Background**: A Ponzi scheme is a fraudulent investment model that pays returns to earlier investors using capital from newer investors, rather than from legitimate profits. Index funds passively track market indices, and when a stock is added to a major index, all funds tracking that index must buy it, regardless of price. This mechanism can inflate valuations and force ordinary investors to hold overvalued stocks.

<details><summary>References</summary>
<ul>
<li><a href="https://tech.ifeng.com/c/8tx0ZbKkemQ">tech.ifeng.com/c/8tx0ZbKkemQ</a></li>
<li><a href="https://money.udn.com/money/story/5599/9556737">被 動 基 金 搶進 SpaceX ... | 經濟日報</a></li>
<li><a href="https://xueqiu.com/6943090400/381595097?scene=1036&share_uid=6943090400">xueqiu.com/6943090400/381595097?scene=1036&share_uid...</a></li>

</ul>
</details>

**Tags**: `#Elon Musk`, `#SpaceX`, `#Ponzi scheme`, `#index funds`, `#tech criticism`

---

<a id="item-17"></a>
## [Australia's teen social media ban fails after 4 months](https://t.me/zaihuapd/41955) ⭐️ 7.0/10

A survey by the Molly Rose Foundation found that 61% of Australians aged 12-15 still have active social media accounts four months after a ban on under-16s took effect, with TikTok, YouTube, and Instagram retaining over 52% of their underage users. This reveals significant enforcement gaps in Australia's social media regulation, highlighting the difficulty of age-based restrictions and the need for stronger platform accountability, which has implications for similar policies worldwide. About 60% of surveyed teens reported that platforms took no action to deactivate or restrict their accounts, and many used VPNs to circumvent the ban, undermining the law's effectiveness.

telegram · zaihuapd · Jun 15, 01:02

**Background**: Australia passed a law in 2024 banning social media access for children under 16, aiming to protect minors from online harms. The Molly Rose Foundation, established after the death of 14-year-old Molly Russell linked to social media, advocates for safer online environments. VPNs allow users to bypass geographic restrictions by masking their IP addresses.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Molly_Rose_Foundation">Molly Rose Foundation</a></li>
<li><a href="https://www.alwaysvpn.com/guides/where-vpns-illegal-banned">Where Are VPNs Illegal or Banned ? | AlwaysVPN</a></li>

</ul>
</details>

**Tags**: `#social media regulation`, `#Australia`, `#teen online safety`, `#platform governance`, `#VPN`

---