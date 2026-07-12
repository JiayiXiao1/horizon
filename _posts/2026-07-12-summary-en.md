---
layout: default
title: "Horizon Summary: 2026-07-12 (EN)"
date: 2026-07-12
lang: en
---

> From 28 items, 16 important content pieces were selected

---

1. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-1) ⭐️ 9.0/10
2. [Humanoid Robot Performs World's First Live Pig Gallbladder Surgery](#item-2) ⭐️ 9.0/10
3. [OpenAI Releases GPT-5.6 Series with Flagship Sol Model](#item-3) ⭐️ 9.0/10
4. [SGLang v0.5.15 Boosts GLM-5.2 on Blackwell with Spec V2](#item-4) ⭐️ 8.0/10
5. [ClickHouse scales PgBouncer to 4x throughput](#item-5) ⭐️ 8.0/10
6. [SK Hynix CEO Warns of Worst Memory Shortage by 2027](#item-6) ⭐️ 8.0/10
7. [SpaceXAI and Cursor Release Grok 4.5 for Coding, Legal, Finance](#item-7) ⭐️ 8.0/10
8. [Apple Sues OpenAI for Trade Secret Theft](#item-8) ⭐️ 8.0/10
9. [6 U-Boot Bootloader Flaws Allow Code Execution Before OS Boot](#item-9) ⭐️ 8.0/10
10. [Shanghai Aims for High-Quality Brain Control by 2027](#item-10) ⭐️ 8.0/10
11. [Prefer strict tables in SQLite](#item-11) ⭐️ 7.0/10
12. [Stop Telling Me to Ask an LLM](#item-12) ⭐️ 7.0/10
13. [Nilay Patel: AR Glasses Require Invasive Privacy Trade-offs](#item-13) ⭐️ 7.0/10
14. [Zhipu Founder Launches 'Touch High' Plan for AGI](#item-14) ⭐️ 7.0/10
15. [Claude Code Desktop Adds Built-in Browser](#item-15) ⭐️ 7.0/10
16. [Google Opposes European Site Blocking as US Piracy Laws Gain Momentum](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 9.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and achieves Transformers modeling backend performance parity with native vLLM. This release marks a paradigm shift in vLLM's architecture, simplifying the codebase and improving maintainability while delivering performance gains. The Transformers backend parity enables users to run Hugging Face models with native vLLM speed, broadening adoption. The release includes 558 commits from 232 contributors, with new support for EVS, realtime embeddings, prefix caching for Mamba hybrid models, and dynamic speculative decoding. PagedAttention is fully removed as V1/MRv2 backends become the standard.

github · khluu · Jul 11, 20:06

**Background**: vLLM is a high-performance LLM inference and serving engine originally developed at UC Berkeley. PagedAttention was its core innovation for efficient memory management, but the newer Model Runner V2 backend offers better performance and flexibility. The Transformers backend allows vLLM to run models from the Hugging Face ecosystem without custom kernels.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2025-04-11-transformers-backend">Transformers modeling backend integration in vLLM | vLLM Blog</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#model serving`, `#open source`, `#release`

---

<a id="item-2"></a>
## [Humanoid Robot Performs World's First Live Pig Gallbladder Surgery](https://arstechnica.com/ai/2026/07/humanoid-robots-controlled-by-surgeons-did-world-first-operation-on-live-pigs/) ⭐️ 9.0/10

Surgeons remotely controlled a Unitree G1 humanoid robot to perform laparoscopic gallbladder removal on live pigs, marking the first time a general-purpose humanoid robot has been used for live surgery. The results were published in Nature. This breakthrough demonstrates that low-cost humanoid robots (starting at $13,500) could replace expensive specialized surgical systems like da Vinci, potentially expanding access to minimally invasive surgery in rural, battlefield, or space settings. The Unitree G1 robot is 1.5 meters tall, weighs 27 kg, and costs $13,500 base or $67,000 with dexterous hands—far less than the $500,000+ da Vinci system. The study was conducted by researchers at the University of California San Diego.

telegram · zaihuapd · Jul 11, 02:29

**Background**: Laparoscopic gallbladder removal (cholecystectomy) is a minimally invasive procedure to remove the gallbladder using a laparoscope. Traditionally, robotic surgery relies on purpose-built platforms like Intuitive Surgical's da Vinci system, which are expensive and bulky. The Unitree G1 is a general-purpose humanoid robot designed for mobility and manipulation, originally intended for industrial and service tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Unitree_Robotics">Unitree Robotics - Wikipedia</a></li>
<li><a href="https://www.unitree.com/g1/">Humanoid robot G1_Humanoid Robot Functions_Humanoid Robot Price | Unitree Robotics</a></li>
<li><a href="https://humanoid-surgeon.github.io/">In vivo feasibility study of humanoid robots in surgery</a></li>

</ul>
</details>

**Tags**: `#robotics`, `#surgery`, `#humanoid robot`, `#medical technology`, `#teleoperation`

---

<a id="item-3"></a>
## [OpenAI Releases GPT-5.6 Series with Flagship Sol Model](https://t.me/zaihuapd/42497) ⭐️ 9.0/10

OpenAI has officially launched the GPT-5.6 series, introducing three model tiers: Sol (flagship), Terra (balanced), and Luna (cost-efficient). The series brings significant improvements in code generation, knowledge work, design, research, and cybersecurity, along with new features like max/ultra reasoning, multi-agent collaboration, and Programmatic Tool Calling. This release marks a major step in OpenAI's model strategy, offering tiered pricing and capabilities to serve diverse use cases from high-performance tasks to high-volume, low-cost applications. The introduction of multi-agent collaboration and Programmatic Tool Calling could enable more complex, autonomous workflows in AI applications. Pricing per 1M tokens: Sol at $5 input / $30 output, Terra at $2.50 / $15, and Luna at $1 / $6. The default API alias 'gpt-5.6' routes to Sol, while explicit model IDs are gpt-5.6-sol, gpt-5.6-terra, and gpt-5.6-luna. The series also introduces more predictable prompt caching.

telegram · zaihuapd · Jul 11, 13:34

**Background**: OpenAI's GPT series has evolved from GPT-3 to GPT-4 and now GPT-5.6, with each generation improving reasoning, accuracy, and domain-specific capabilities. Multi-agent collaboration allows multiple AI agents to work together on complex tasks, while Programmatic Tool Calling enables agents to write and execute code to invoke tools, reducing token usage and improving efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/previewing-gpt-5-6-sol/">Previewing GPT-5.6 Sol: a next-generation model | OpenAI</a></li>
<li><a href="https://www.vellum.ai/blog/gpt-5-6-benchmarks-explained">GPT-5.6 Sol vs Terra vs Luna: Which Tier Should You Actually Use?</a></li>
<li><a href="https://www.mindstudio.ai/blog/what-is-gpt-5-6-soul-terra-luna-explained">What Is GPT-5.6? OpenAI's Soul, Terra, and Luna Model Tiers Explained | MindStudio</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#AI models`, `#machine learning`, `#natural language processing`

---

<a id="item-4"></a>
## [SGLang v0.5.15 Boosts GLM-5.2 on Blackwell with Spec V2](https://github.com/sgl-project/sglang/releases/tag/v0.5.15) ⭐️ 8.0/10

SGLang v0.5.15 introduces Spec V2 as the default speculative decoding method, achieving 500+ tokens per second per user on 8x B300 for GLM-5.2 NVFP4, and adds IndexShare MTP which reduces draft-step cost by up to 1.9x at long context. This release significantly improves the efficiency of serving large language models on NVIDIA Blackwell hardware, making high-throughput inference more accessible for production deployments. The optimizations, especially Spec V2 and IndexShare MTP, set new performance benchmarks for speculative decoding. Spec V2 achieves +11% end-to-end TPS through CUDA-graphable DSA draft-extend and fused metadata ops. IndexShare MTP reuses the indexer top-k across draft steps, reducing draft-step cost by up to 1.9x at long context. Additionally, TopK V2 fuses top-k selection with page-table transform, supporting runtime k up to 2048.

github · Fridge003 · Jul 10, 22:58

**Background**: SGLang is a high-performance serving framework for large language and multimodal models. Speculative decoding is a technique that uses a draft model to predict multiple tokens per step, accelerating inference. NVFP4 is a 4-bit floating point format introduced by NVIDIA for Blackwell GPUs, designed to improve inference efficiency while maintaining accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://sgl-project-sglang-93.mintlify.app/advanced/speculative-decoding">Speculative Decoding - SGLang</a></li>
<li><a href="https://docs.sglang.io/">Welcome to SGLang - SGLang Documentation</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#LLM serving`, `#performance optimization`, `#speculative decoding`, `#NVIDIA Blackwell`, `#SGLang`

---

<a id="item-5"></a>
## [ClickHouse scales PgBouncer to 4x throughput](https://clickhouse.com/blog/pgbouncer-clickhouse-managed-postgres) ⭐️ 8.0/10

ClickHouse engineers improved PgBouncer throughput by 4x using SO_REUSEPORT and a peering mechanism to handle connection cancellation efficiently. This optimization addresses a critical bottleneck in PostgreSQL connection pooling, enabling higher scalability for large-scale deployments without changing the underlying database. SO_REUSEPORT allows multiple PgBouncer processes to bind to the same port, while peering forwards cancellation requests to the correct process, preventing dropped cancellations.

hackernews · saisrirampur · Jul 11, 15:28 · [Discussion](https://news.ycombinator.com/item?id=48872874)

**Background**: PgBouncer is a lightweight connection pooler for PostgreSQL. Connection cancellation requests can land on the wrong process when multiple poolers are used, causing failures. SO_REUSEPORT is a Linux socket option that enables multiple sockets to listen on the same port, improving load distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://www.pgbouncer.org/config.html">PgBouncer config</a></li>
<li><a href="https://github.com/pgbouncer/pgbouncer/issues/328">pgbouncer unavailable while churning through cancellations · Issue #328 · pgbouncer/pgbouncer</a></li>
<li><a href="https://pgstef.github.io/talks/en/20250912_PGDayLowlands_PgBouncer-at-scale.pdf">PgBouncer at scale</a></li>

</ul>
</details>

**Discussion**: Commenters suggested alternative solutions like Odyssey and pgdog, and asked about the ease of setting up peering in PgBouncer. Some shared their experiences running multiple PgBouncer instances on Kubernetes.

**Tags**: `#PostgreSQL`, `#PgBouncer`, `#connection pooling`, `#scalability`, `#ClickHouse`

---

<a id="item-6"></a>
## [SK Hynix CEO Warns of Worst Memory Shortage by 2027](https://www.reuters.com/world/asia-pacific/sk-hynix-ceo-sees-worst-ever-memory-supply-shortage-2027-says-demand-outstrip-2026-07-10/) ⭐️ 8.0/10

SK Hynix CEO Kwak Noh-jung warned that the global memory industry will face its worst-ever supply shortage by 2027, with demand outstripping supply even after aggressive expansion. The warning came on the day of SK Hynix's Nasdaq debut, where shares closed up 13.3% at $168.85. This warning from a top memory manufacturer signals a prolonged supply crunch that could impact global tech supply chains, affecting everything from AI accelerators to consumer electronics. The shortage may drive up memory prices and force companies to secure long-term supply agreements. SK Hynix is considering overseas wafer fab locations in the US, Japan, and Southeast Asia, prioritizing regions with the best land, power, and labor costs. The company reported a record operating profit of 47 trillion won ($31 billion) in 2025, with Q2 2026 expected to reach 65.5 trillion won.

telegram · zaihuapd · Jul 11, 00:45

**Background**: SK Hynix is one of the world's largest memory chip manufacturers, specializing in DRAM and NAND flash memory. The company is part of the 'Big Three' memory makers alongside Samsung and Micron. Memory chips are critical components in computers, smartphones, and increasingly in AI data centers, where high-bandwidth memory (HBM) is essential for training large AI models.

<details><summary>References</summary>
<ul>
<li><a href="https://www.asiaone.com/asia/sk-hynix-ceo-sees-worst-memory-shortage-2027-demand-outstrip-supply-beyond-2030">SK Hynix CEO sees worst memory shortage in 2027 ... - AsiaOne</a></li>
<li><a href="https://en.wikipedia.org/wiki/SK_Hynix">SK Hynix</a></li>
<li><a href="https://wccftech.com/memory-makers-only-meet-60-percent-dram-demand-through-2027/">Memory Makers Will Only Meet 60% of DRAM Demand Through 2027 ...</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#memory`, `#supply chain`, `#SK Hynix`, `#industry forecast`

---

<a id="item-7"></a>
## [SpaceXAI and Cursor Release Grok 4.5 for Coding, Legal, Finance](https://t.me/zaihuapd/42484) ⭐️ 8.0/10

SpaceXAI and Cursor have jointly released Grok 4.5, the first model since SpaceX's $60 billion acquisition of Cursor, achieving top ranking on the Harvey legal agent benchmark and offering double the token efficiency of comparable models. This release signals a major push into domain-specific AI for high-stakes professional tasks, potentially disrupting legal, financial, and cybersecurity sectors with a model that combines coding prowess with legal and financial expertise. Grok 4.5 runs at 80 tokens per second and costs $2 per million input tokens, with token efficiency claimed to be twice that of leading competitors, and it also features enhanced cybersecurity capabilities.

telegram · zaihuapd · Jul 11, 01:44

**Background**: Cursor is an AI-powered code editor and development environment, valued at $29.3 billion before SpaceX's acquisition. The Harvey Legal Agent Benchmark is an open-source benchmark for evaluating AI agents on legal tasks. Token efficiency refers to how many tokens a model uses to generate a response, directly impacting cost and speed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.harvey.ai/blog/introducing-harveys-legal-agent-benchmark">Introducing Harvey’s Legal Agent Benchmark</a></li>
<li><a href="https://en.wikipedia.org/wiki/Cursor_(code_editor)">Cursor (code editor)</a></li>
<li><a href="https://www.vals.ai/benchmarks/hlab">Harvey's Legal Agent Benchmark</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#SpaceXAI`, `#Cursor`, `#Grok`

---

<a id="item-8"></a>
## [Apple Sues OpenAI for Trade Secret Theft](https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html) ⭐️ 8.0/10

On July 10, 2026, Apple filed a lawsuit in the U.S. District Court for the Northern District of California against OpenAI, two former employees, and io Products, alleging systematic theft of trade secrets related to product design, manufacturing processes, and supply chain to accelerate OpenAI's hardware business. This high-profile legal battle between two tech giants could set a precedent for how trade secrets are protected in the AI and hardware industries, potentially impacting competition and innovation. If proven, the allegations could severely damage OpenAI's hardware ambitions and its partnership with Jony Ive's io Products. Apple alleges that former employee Chang Liu accessed internal networks after leaving and downloaded dozens of hardware files, while OpenAI's hardware head Tang Yew Tan sent supplier information to his personal email before resigning and asked job candidates to bring Apple components to interviews. Apple also claims that over 400 former employees now work at OpenAI.

telegram · zaihuapd · Jul 11, 03:14

**Background**: OpenAI, best known for its AI models like GPT-4, has been expanding into hardware. In May 2025, it acquired io Products, a company founded by former Apple design chief Jony Ive, to lead its hardware development. The first OpenAI device was expected in 2026 but has been delayed to 2027 due to a trademark lawsuit. Apple's lawsuit adds another major obstacle.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbc.com/2026/07/10/apple-openai-lawsuit-trade-secrets.html">Apple sues OpenAI alleging trade secret theft, says scheme was 'at every level'</a></li>
<li><a href="https://www.engadget.com/2212759/apple-calls-openais-hardware-business-rotten-to-its-core-in-trade-secret-theft-lawsuit/">Apple calls OpenAI's hardware business 'rotten to its core' in trade secret theft lawsuit - Engadget</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_(company)">io (company) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-9"></a>
## [6 U-Boot Bootloader Flaws Allow Code Execution Before OS Boot](https://www.bleepingcomputer.com/news/security/new-u-boot-flaws-could-enable-stealthy-firmware-attacks/) ⭐️ 8.0/10

Firmware security firm Binarly disclosed six vulnerabilities in U-Boot's FIT image signature verification, two of which enable arbitrary code execution and four cause denial of service, affecting versions since 2013.07. These flaws allow attackers to execute malicious code before the operating system boots, potentially disabling firmware security features or installing persistent malware, affecting a vast number of embedded devices. The vulnerabilities (BRLY-2026-037 through BRLY-2026-042) reside in the FIT signature verification code and have been present for over 50 stable releases; patches have been accepted upstream but require vendor integration.

telegram · zaihuapd · Jul 11, 08:32

**Background**: U-Boot is a widely used open-source bootloader for embedded devices, responsible for loading the operating system. FIT (Flattened Image Tree) is a standard image format used by U-Boot to package kernel, device tree, and other components. Signature verification ensures only trusted images are booted, forming a critical part of the secure boot chain.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/07/six-new-u-boot-flaws-could-let.html">Six New U - Boot Flaws Could Let Malicious Images Crash Devices or...</a></li>
<li><a href="https://cybersecuritynews.com/u-boot-fit-signature-verification/">Six U - Boot FIT Signature Verification Flaws Enable Code Execution...</a></li>

</ul>
</details>

**Tags**: `#security`, `#U-Boot`, `#bootloader`, `#firmware`, `#vulnerability`

---

<a id="item-10"></a>
## [Shanghai Aims for High-Quality Brain Control by 2027](https://t.me/zaihuapd/42501) ⭐️ 8.0/10

The Shanghai Municipal Science and Technology Commission issued the "Shanghai Brain-Computer Interface Future Industry Cultivation Action Plan (2025-2030)", targeting high-quality brain control by 2027, with semi-invasive BCI products leading clinical application in China and breakthroughs in invasive BCI research. This government action plan signals significant investment and policy support for brain-computer interface technology, which could accelerate the development of medical BCI devices for patients with paralysis or speech loss, positioning Shanghai as a leader in the neurotechnology industry. The plan aims to have at least five invasive or semi-invasive BCI products complete medical device type testing and clinical trials, enabling partial restoration of language and motor functions for patients with aphasia or paralysis.

telegram · zaihuapd · Jul 11, 15:49

**Background**: Brain-computer interfaces (BCIs) are systems that create a direct communication pathway between the brain and external devices. They are categorized into non-invasive (e.g., scalp electrodes), semi-invasive (e.g., electrodes placed under the skull but outside the brain), and invasive (e.g., electrodes implanted directly into brain tissue). Semi-invasive BCIs offer a balance between signal quality and surgical risk, making them promising for clinical applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nhsa.gov.cn/art/2025/3/13/art_52_15967.html">nhsa.gov.cn/art/2025/3/13/art_52_15967.html</a></li>
<li><a href="https://segmentfault.com/a/1190000044921513">segmentfault.com/a/1190000044921513</a></li>
<li><a href="https://www.jfdaily.com/wx/detail.do?id=874565">三家“ 脑 机 接 口 ”头部企业为何出现在上海？｜跟着项目经理看未来产业</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#policy`, `#China`, `#neurotechnology`, `#medical devices`

---

<a id="item-11"></a>
## [Prefer strict tables in SQLite](https://evanhahn.com/prefer-strict-tables-in-sqlite/) ⭐️ 7.0/10

A blog post by Evan Hahn advocates for using STRICT tables in SQLite to enforce type safety, highlighting that strict tables prevent accidental type mismatches and improve data integrity. This matters because SQLite's default flexible typing can lead to subtle bugs, and adopting strict tables brings SQLite closer to the type safety of traditional SQL databases, benefiting developers who rely on SQLite for production applications. Strict tables require every column to have a specified datatype (INT, INTEGER, REAL, TEXT, BLOB, or ANY) and enforce type checking on insertions, but there is no built-in ALTER TABLE command to convert an existing table to strict; migration requires copying data to a new strict table.

hackernews · ingve · Jul 11, 17:33 · [Discussion](https://news.ycombinator.com/item?id=48873940)

**Background**: SQLite traditionally uses flexible typing, where column types are affinities rather than strict constraints, allowing any value to be stored in any column regardless of declared type. This design simplifies prototyping and compatibility with loosely-typed data, but can lead to data corruption if type mismatches go unnoticed. STRICT tables, introduced in SQLite 3.37.0 (November 2021), enforce rigid type rules similar to other SQL databases.

<details><summary>References</summary>
<ul>
<li><a href="https://sqlite.org/stricttables.html">STRICT Tables</a></li>
<li><a href="https://www.sqlitetutorial.net/sqlite-strict-tables/">SQLite Strict Tables</a></li>
<li><a href="https://antonz.org/sqlite-strict-tables/">STRICT tables in SQLite</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed opinions: some developers strongly prefer strict tables and wish they were the default, while others defend flexible typing for its simplicity and compatibility with ad-hoc scripts. Simon Willison created a tool to convert non-strict tables to strict using sqlite-utils, and a link to SQLite's official defense of flexible typing was shared.

**Tags**: `#SQLite`, `#database`, `#type safety`, `#software engineering`

---

<a id="item-12"></a>
## [Stop Telling Me to Ask an LLM](https://blog.yaelwrites.com/stop-telling-me-to-ask-an-llm/) ⭐️ 7.0/10

The article critiques the common reflex in technical discussions to suggest asking an LLM without acknowledging the asker's prior research effort, highlighting a communication breakdown. This matters because it exposes a growing friction in knowledge work communities where LLMs are treated as a universal answer, potentially devaluing human expertise and discouraging deeper inquiry. The author emphasizes they already consulted Claude before asking, and the reflex response ignores that effort, leading to frustration. The piece is not anti-LLM but focuses on communication dynamics.

hackernews · theorchid · Jul 11, 22:28 · [Discussion](https://news.ycombinator.com/item?id=48876441)

**Background**: In technical communities, it's common to suggest using search engines or LLMs before asking questions, a practice known as LMGTFY. However, when the asker has already done that, the suggestion can feel dismissive and unhelpful.

**Discussion**: Commenters largely agree with the author, noting that including prior research upfront can prevent such responses. Some point out that the suggestion may be a polite way to decline answering, while others argue that LLMs can indeed provide better answers in some cases.

**Tags**: `#LLM`, `#communication`, `#tech culture`, `#knowledge work`, `#Hacker News`

---

<a id="item-13"></a>
## [Nilay Patel: AR Glasses Require Invasive Privacy Trade-offs](https://simonwillison.net/2026/Jul/10/nilay-patel/#atom-everything) ⭐️ 7.0/10

Nilay Patel argues that augmented reality glasses inherently require continuous recording and cloud processing, which inevitably invade privacy, and suggests society should consider halting such products. This commentary highlights a fundamental privacy dilemma in AR development, challenging the industry's assumption that AR glasses can be made privacy-friendly. It raises critical societal questions about whether the trade-offs are acceptable. Patel states that no chip small enough to fit in glasses stems can perform real-time processing; data must be sent to the cloud. The alternative is a bulky device like Apple Vision Pro with an external battery pack.

rss · Simon Willison · Jul 10, 17:05

**Background**: Augmented reality (AR) overlays digital information onto the real world. Current AR glasses like Meta's Ray-Ban Stories use cameras and cloud AI for features like object recognition. On-device processing preserves privacy but is limited by power and size constraints, while cloud processing offers more capability but raises privacy concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Augmented_reality">Augmented reality - Wikipedia</a></li>
<li><a href="https://www.rayneo.com/blogs/news/ai-powered-smart-glasses-what-artificial-intelligence-actually-does-for-you">AI-Powered Smart Glasses : What Artificial Intelligence Actually Does...</a></li>
<li><a href="https://www.digitalapplied.com/blog/android-xr-google-ai-glasses-developer-guide">Android XR & AI Glasses : Developer Guide 2026</a></li>

</ul>
</details>

**Tags**: `#augmented reality`, `#privacy`, `#cloud computing`, `#hardware`

---

<a id="item-14"></a>
## [Zhipu Founder Launches 'Touch High' Plan for AGI](https://mp.weixin.qq.com/s/3CQSkf_kBnXiCDgS4L-Cgg) ⭐️ 7.0/10

Zhipu AI founder Tang Jie announced the 'Touch High' (Mo Gao) plan, committing billions of yuan to research on mechanistic interpretability to make black-box models transparent, as part of a broader AGI roadmap. This signals a major Chinese AI lab prioritizing long-term AGI safety over short-term profits, potentially influencing global AI safety research and open-source model transparency. The plan outlines four peaks to conquer: long-horizon tasks, autonomous agent systems, fully self-training, and extreme safety governance. Zhipu's GLM-5.2 model is said to approach frontier capabilities of overseas models.

telegram · zaihuapd · Jul 11, 13:59

**Background**: Mechanistic interpretability aims to reverse-engineer neural networks to understand their internal algorithms, similar to debugging software. Black-box AI models, especially deep neural networks, often make decisions that even their creators cannot fully explain, raising trust and safety concerns. AGI safety research focuses on preventing accidents or misuse of advanced AI systems.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mechanistic_interpretability">Mechanistic interpretability</a></li>
<li><a href="https://www.ibm.com/think/topics/black-box-ai">What Is Black Box AI and How Does It Work? | IBM</a></li>
<li><a href="https://en.wikipedia.org/wiki/AGI_safety">AGI safety</a></li>

</ul>
</details>

**Tags**: `#AGI`, `#AI safety`, `#mechanistic interpretability`, `#智谱`, `#open source`

---

<a id="item-15"></a>
## [Claude Code Desktop Adds Built-in Browser](https://x.com/ClaudeDevs/status/2075635283211772279) ⭐️ 7.0/10

Claude Code Desktop now includes a built-in browser that allows users to open and interact with websites directly within the application, using a sandboxed design with configurable session persistence. This feature streamlines developer workflows by eliminating the need to switch between the IDE and an external browser for documentation, design previews, or local servers, enhancing productivity and focus. The browser is sandboxed for security, and users can configure whether browsing sessions are preserved across restarts. It supports reading, clicking, and interacting with websites, similar to working with a local development server.

telegram · zaihuapd · Jul 11, 14:34

**Background**: Claude Code is an AI-powered coding assistant from Anthropic that integrates with IDEs. The desktop version provides a full-featured environment with Git isolation, parallel sessions, and integrated tools. Adding a built-in browser extends its capabilities for web-based tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/zh-CN/desktop">Desktop application - Claude Code Docs</a></li>
<li><a href="https://claude.com/download">Download Claude | Claude by Anthropic</a></li>

</ul>
</details>

**Tags**: `#Claude Code`, `#IDE`, `#浏览器`, `#开发者工具`, `#AI`

---

<a id="item-16"></a>
## [Google Opposes European Site Blocking as US Piracy Laws Gain Momentum](https://torrentfreak.com/google-opposes-site-blocking-in-europe-as-u-s-piracy-blocking-plans-gain-momentum/) ⭐️ 7.0/10

Google submitted a formal filing to the European Commission opposing expanded site-blocking measures, arguing that blocking DNS resolvers, IP addresses, and VPNs is ineffective and disproportionate. Meanwhile, the U.S. Congress is advancing similar anti-piracy legislation, with Representative Issa planning to introduce a site-blocking bill. This highlights a growing global divide in internet governance: Europe is reconsidering site blocking due to overblocking concerns, while the U.S. moves toward stricter enforcement. Google's stance could influence policy debates and affect how platforms handle copyright enforcement. Google's filing cited specific overblocking incidents, including Italy's anti-piracy system mistakenly blocking Google Drive subdomains and Cloudflare IP addresses that host 42 million domains. Google has not publicly commented on the U.S. plans but advocates for providing better legal alternatives to piracy rather than expanding blocking.

telegram · zaihuapd · Jul 11, 15:10

**Background**: Site blocking is a common anti-piracy tool where ISPs or DNS resolvers are ordered to block access to infringing websites. However, such measures can inadvertently block legitimate services (overblocking), as seen with Cloudflare's shared IP ranges. DNS resolvers translate domain names to IP addresses; blocking them can disrupt access to many sites at once.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cloudflare.com/ips/">IP Ranges | Cloudflare</a></li>

</ul>
</details>

**Tags**: `#internet governance`, `#copyright`, `#site blocking`, `#Google`, `#piracy`

---