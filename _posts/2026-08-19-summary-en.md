---
layout: default
title: "Horizon Summary: 2026-08-19 (EN)"
date: 2026-08-19
lang: en
---

> From 37 items, 23 important content pieces were selected

---

1. [Go 1.27 Release: Generic Methods, UUID Package, and More](#item-1) ⭐️ 9.0/10
2. [Mojo Programming Language Open-Sourced Under Apache 2.0](#item-2) ⭐️ 9.0/10
3. [Long March 10B Achieves World's First Net-Based Rocket Recovery at Sea](#item-3) ⭐️ 9.0/10
4. [Moderna and Merck Report Phase 3 Success for Personalized mRNA Cancer Vaccine in Melanoma](#item-4) ⭐️ 9.0/10
5. [Stripe to Acquire OpenRouter for $7B+](#item-5) ⭐️ 8.0/10
6. [Google Replaces Git Tags with Google Drive for Android Source](#item-6) ⭐️ 8.0/10
7. [A Joke Domain Purchase Turns Into Geopolitical Warfare](#item-7) ⭐️ 8.0/10
8. [Geolocating an Island via Geometry and CUDA](#item-8) ⭐️ 8.0/10
9. [Ornith-1.5: Self-Scaffolding Meets Self-Improvement](#item-9) ⭐️ 8.0/10
10. [Qwen 3.8 27B Matches GPT-5.6 Luna on Intelligence Index](#item-10) ⭐️ 8.0/10
11. [US Approves Nvidia H200 Sales to Chinese Firms, Nvidia Seeks Breakthrough](#item-11) ⭐️ 8.0/10
12. [Unsloth Releases Dynamic 3.0 GGUFs with Improved Accuracy](#item-12) ⭐️ 7.0/10
13. [fx: A Tiny, Open-Source Coding Agent in Zig](#item-13) ⭐️ 7.0/10
14. [PostgreSQL for Everything: A Provocative Take on Database Consolidation](#item-14) ⭐️ 7.0/10
15. [Simon Willison Tests smolvm as a Sandbox for Untrusted Python and JavaScript](#item-15) ⭐️ 7.0/10
16. [LLMs and Sandboxing Enable Extensible Web Software](#item-16) ⭐️ 7.0/10
17. [Simon Willison Defends Lines of Code as AI Productivity Metric](#item-17) ⭐️ 7.0/10
18. [Anthropic Urges Global Slowdown of Frontier AI Development](#item-18) ⭐️ 7.0/10
19. [OpenAI Cuts GPT-5.6 Prices: Luna Down 80%, Terra 20%](#item-19) ⭐️ 7.0/10
20. [OpenAI Discloses Codex May Delete User Files, Adds Multi-Layer Protections](#item-20) ⭐️ 7.0/10
21. [TSMC to Raise Chip Prices 5-10% Starting 2027](#item-21) ⭐️ 7.0/10
22. [ByteDance's Doubao Voice Model to Debut in Tesla China via OTA](#item-22) ⭐️ 7.0/10
23. [YMTC IPO Status Changes to Counseling Acceptance](#item-23) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Go 1.27 Release: Generic Methods, UUID Package, and More](https://go.dev/blog/go1.27) ⭐️ 9.0/10

Go 1.27 has been released, introducing generic methods, a standard library UUID package, and performance improvements. The release also includes post-quantum cryptography and a rewritten JSON engine. This release is significant for the Go ecosystem as it addresses long-standing limitations, such as the inability to define generic methods, and provides a standard UUID package that reduces dependency on third-party libraries. These changes will impact developers across the community, improving code ergonomics and security. Generic methods allow methods to declare their own type parameters, a feature long requested since generics were introduced in Go 1.18. The new standard library uuid package implements UUID generation and parsing without external dependencies, and the release includes post-quantum cryptography and a rewritten JSON engine.

hackernews · database64128 · Aug 19, 18:33 · [Discussion](https://news.ycombinator.com/item?id=49365405)

**Background**: Go is a statically typed, compiled programming language designed for simplicity and efficiency. Generics, introduced in Go 1.18, allowed functions and types to be parameterized, but methods were initially excluded. The addition of generic methods in Go 1.27 removes this restriction, enabling more flexible and reusable code patterns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gopherguides.com/articles/golang-generic-methods">Generic Methods Arrive in Go 1.27 - Gopher Guides</a></li>
<li><a href="https://pkg.go.dev/uuid">uuid package - uuid - Go Packages</a></li>
<li><a href="https://northeasttimes.com/2026/08/02/go-1-27-brings-generic-methods-post-quantum-crypto-and-a-new-json-engine/">Go 1.27 brings generic methods, post-quantum crypto and a new JSON engine - Northeast Times</a></li>

</ul>
</details>

**Discussion**: Community comments highlight additional features not mentioned in the release notes, such as the new floating-point parsing algorithm and the proactive post-quantum crypto efforts. Some developers anticipate a wave of pull requests migrating from third-party UUID libraries to the new standard package, while others express minor frustrations like the lack of syntax highlighting on the Go blog.

**Tags**: `#Go`, `#programming language`, `#release`, `#generics`, `#crypto`

---

<a id="item-2"></a>
## [Mojo Programming Language Open-Sourced Under Apache 2.0](https://simonwillison.net/2026/Aug/18/mojo-is-now-open-source/) ⭐️ 9.0/10

Modular has open-sourced the Mojo programming language and its compiler toolchain under the Apache 2.0 license, following the release of Mojo 1.0. This fulfills a promise made in May 2023 to eventually open-source the language. This is a major milestone for the AI and Python ecosystems, as Mojo offers high performance for AI workloads with Python-like syntax. Open-sourcing under a permissive license is likely to accelerate adoption, foster community contributions, and position Mojo as a viable alternative to traditional Python for performance-critical applications. Mojo was originally intended to be a superset of Python, but that plan was revised around August 2025, and it is now a standalone language optimized for GPU programming. The compiler is built on MLIR, which allows it to target CPUs, GPUs, TPUs, and other accelerators.

rss · Simon Willison · Aug 18, 21:39

**Background**: Mojo is a systems programming language developed by Modular Inc., designed for high-performance AI infrastructure. It combines Python-like syntax with systems programming features such as static typing and a borrow checker, inspired by Rust. The language leverages the MLIR compiler framework to achieve high performance and support diverse hardware targets.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mojo_(programming_language)">Mojo (programming language)</a></li>
<li><a href="https://www.apache.org/licenses/LICENSE-2.0.html">Apache License, Version 2.0 | Apache Software Foundation</a></li>
<li><a href="https://mojolang.org/">Mojo</a></li>

</ul>
</details>

**Discussion**: The community discussion on Lobste.rs generally expressed positive sentiment, with users noting that the open-source release is a significant step for the language. Some comments highlighted the shift away from Python superset compatibility as a pragmatic decision, while others discussed the potential impact on the Python ecosystem and the advantages of MLIR-based compilation.

**Tags**: `#Mojo`, `#open source`, `#programming language`, `#AI`, `#compiler`

---

<a id="item-3"></a>
## [Long March 10B Achieves World's First Net-Based Rocket Recovery at Sea](https://t.me/zaihuapd/43264) ⭐️ 9.0/10

On July 10, 2026, China's Long March 10B rocket launched from the Hainan Commercial Space Launch Site and successfully recovered its first stage via a net-based system on a sea platform, marking the world's first net-based recovery of a rocket first stage. This achievement marks China's first controlled recovery of a rocket first stage and a historic breakthrough in reusable rocket technology. It could significantly reduce launch costs and enhance China's competitiveness in the commercial space industry, aligning with global trends toward reusable launch vehicles. The first stage separated about six minutes after liftoff, then vertically descended and was captured by a net system on a sea platform. The Long March 10B is the first Chinese rocket to successfully implement recovery, and the net-based recovery method is a novel approach compared to the propulsive landing used by SpaceX's Falcon 9.

telegram · zaihuapd · Aug 19, 00:16

**Background**: Reusable rocket technology aims to reduce the cost of space access by recovering and reusing the most expensive components of a launch vehicle. Traditional recovery methods, such as propulsive landing, require precise engine burns and landing legs. The net-based recovery system, developed by China, uses a ship-based net and onboard hooks to capture the descending first stage, offering an alternative approach that may simplify the landing process and improve recovery success rates.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news.cn/20260710/ba0ac14f31dd492aaf918e7a86ac844a/c.html">长征十号乙首飞成功 我国运载火箭首次实现可控回收-新华网</a></li>
<li><a href="https://www.zhihu.com/question/2058516301257994660">长征十号乙运载火箭成功实现一子级可控回收，这一技术有多难？此次成功回收具有哪些重要意义？ - 知乎</a></li>
<li><a href="https://xinwen.bjd.com.cn/content/s692e925be4b076b012789327.html">我国首个，成功交付！“网系回收”如何接住火箭？</a></li>

</ul>
</details>

**Discussion**: Community comments from Zhihu and other platforms generally express excitement and pride in China's achievement, with some users discussing the technical challenges and potential advantages of net-based recovery compared to propulsive landing. A few commenters note that this could pave the way for more frequent and cost-effective launches.

**Tags**: `#aerospace`, `#rocket recovery`, `#China`, `#space technology`, `#Long March`

---

<a id="item-4"></a>
## [Moderna and Merck Report Phase 3 Success for Personalized mRNA Cancer Vaccine in Melanoma](https://wallstreetcn.com/articles/3779803) ⭐️ 9.0/10

On August 19, 2026, Moderna and Merck announced that their personalized mRNA cancer vaccine combined with Keytruda met primary and key secondary endpoints in a Phase 3 trial for melanoma, significantly reducing the risk of recurrence and distant metastasis. The companies have not yet disclosed the exact improvement magnitude, and the trial will continue to evaluate overall survival. This is the first successful Phase 3 trial of a personalized mRNA cancer vaccine, validating the concept of individualized immunotherapy at scale. It could transform adjuvant treatment for melanoma and potentially other cancers, with significant market impact as Moderna's stock surged up to 150%. The vaccine is customized based on each patient's tumor genetic mutations, representing a 'one person, one injection' precision approach. The trial will continue to assess overall survival, and the specific reduction in recurrence risk has not been disclosed yet.

telegram · zaihuapd · Aug 19, 14:41

**Background**: Personalized mRNA cancer vaccines work by sequencing a patient's tumor to identify neoantigens—abnormal markers on cancer cells—and then creating a vaccine that trains the immune system to attack these targets. Keytruda (pembrolizumab) is an immune checkpoint inhibitor that blocks the PD-1 receptor, helping T cells recognize and destroy cancer cells. Melanoma is a high-risk cancer with significant recurrence rates after surgery, making effective adjuvant therapies crucial.

<details><summary>References</summary>
<ul>
<li><a href="https://oncolifecentre.com/personalized-cancer-vaccine-shows-long-term-promise/">Personalized Cancer Vaccine Shows Long-Term Promise - Onco Life...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Pembrolizumab">Pembrolizumab - Wikipedia</a></li>
<li><a href="https://www.keytrudahcp.com/resources/mechanism-of-action/">Mechanism of Action of KEYTRUDA® (pembrolizumab) | Health ...</a></li>

</ul>
</details>

**Tags**: `#mRNA vaccine`, `#cancer immunotherapy`, `#Moderna`, `#Merck`, `#clinical trial`

---

<a id="item-5"></a>
## [Stripe to Acquire OpenRouter for $7B+](https://openrouter.ai/blog/announcements/openrouter-is-joining-stripe/) ⭐️ 8.0/10

Stripe has agreed to acquire OpenRouter, the AI model routing gateway, for more than $7 billion in cash and stock, as reported by Bloomberg on August 16, 2026. The deal is not yet publicly confirmed by either company, and the final price may change. This acquisition is significant because it consolidates AI model access with payment infrastructure, potentially simplifying billing for developers and strengthening Stripe's position in the AI economy. It also validates the value of model routing proxies, which could encourage further innovation in this space. OpenRouter has long used Stripe Invoicing, Stripe Tax, and Radar for its global billing and risk control, making this acquisition a vertical integration of an existing customer. The deal is reportedly valued at over $7 billion, but neither company has confirmed the terms publicly.

hackernews · rvz · Aug 19, 17:32 · [Discussion](https://news.ycombinator.com/item?id=49364559)

**Background**: OpenRouter is a model router or AI gateway that consolidates access to multiple AI model providers behind a single API endpoint, allowing developers to switch between models easily. Stripe is a major online payment processing platform that has been expanding its AI-related services. The acquisition aligns with Stripe's strategy to integrate AI capabilities into its payment ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://www.orcarouter.ai/blog/stripe-acquires-openrouter">Stripe OpenRouter Acquisition : $7B, What Changes for Devs</a></li>
<li><a href="https://www.odaily.news/en/post/5212096">Stripe Acquires OpenRouter : The Ultimate Piece of the AI... - Odaily</a></li>
<li><a href="https://www.oflight.co.jp/en/columns/stripe-openrouter-acquisition-2026">Stripe Acquires OpenRouter ($7B+): What Devs Need to... | Oflight Inc.</a></li>

</ul>
</details>

**Discussion**: Community members generally view the acquisition positively, praising OpenRouter's business model and the potential for unified billing. Some express concerns about centralization and prefer open protocols over middlemen, while others highlight useful features like cost-based routing with performance minimums.

**Tags**: `#acquisition`, `#AI`, `#OpenRouter`, `#Stripe`, `#business`

---

<a id="item-6"></a>
## [Google Replaces Git Tags with Google Drive for Android Source](https://grapheneos.social/@GrapheneOS/117057099753905023) ⭐️ 8.0/10

Google has replaced Git tags for certain Android source code with a manual process requiring a Google Forms request and a Google Drive link, as reported by GrapheneOS. This change affects how developers access specific source code releases. This change raises significant GPL compliance concerns, as the GPLv2 requires that source code be readily available to recipients. If Google's new process is slow or restrictive, it could violate the license and undermine the open-source ecosystem's trust in Android. The new process involves filling out a Google Form and waiting for a human to provide a Google Drive link, which has reportedly become increasingly slow. This replaces the previous practice of pushing Git tags to public repositories, which allowed direct access via git commands.

hackernews · Animux · Aug 19, 17:47 · [Discussion](https://news.ycombinator.com/item?id=49364745)

**Background**: Android's source code is distributed under various licenses, with the Linux kernel and certain components under GPLv2, which mandates that source code be provided to users. Git tags are commonly used in open-source projects to mark specific releases, making it easy for developers to fetch exact versions. The Android Open Source Project (AOSP) has traditionally used public Git repositories, but this change for certain code may complicate access and compliance.

<details><summary>References</summary>
<ul>
<li><a href="https://source.android.com/docs/setup/download">Download the Android source - Android Open Source Project</a></li>
<li><a href="https://android.googlesource.com/">android Git repositories - Git at Google</a></li>
<li><a href="https://source.android.com/license">Content license - Android Open Source Project LICENSES/preferred/GPL-2.0 - kernel/common - Git at Google Contributor license agreements and headers | Android Open ... GPL | XDA Licenses | Android Open Source - GitHub Pages</a></li>

</ul>
</details>

**Discussion**: Community comments express concern over GPL compliance and the inconvenience of the new process, with some linking to broader issues like keepandroidopen.org. However, one commenter argues that calling it a GPL violation is a stretch, noting Android has always been more source-available than truly open. Others sarcastically predict further restrictions, such as mailing source code.

**Tags**: `#Android`, `#Open Source`, `#GPL`, `#Google`, `#Licensing`

---

<a id="item-7"></a>
## [A Joke Domain Purchase Turns Into Geopolitical Warfare](https://sprocketfox.io/xssfox/2026/08/19/sondehub-and-war/) ⭐️ 8.0/10

A humorous domain purchase escalated into a geopolitical confrontation involving radio tracking, weather balloons, and international tensions. The article details how a seemingly innocent act led to serious implications. This story highlights the intersection of technology, data collection, and international conflict, showing how individual actions can have geopolitical repercussions. It underscores the importance of open-source data and the potential for misinterpretation in a tense global environment. The article mentions that transmitters shut down after a certain period due to strategic considerations, and includes an email from Meteolabor that was described as the most sane part. Community members noted the involvement of habhub, a platform used for tracking weather balloons.

hackernews · kareiva · Aug 19, 11:21 · [Discussion](https://news.ycombinator.com/item?id=49360015)

**Background**: Radio tracking technology involves using radio signals to determine location, often used in wildlife telemetry and weather balloon tracking. Weather balloons have a history of being used for surveillance, leading to international incidents such as the 2023 Chinese spy balloon controversy. Open-source platforms like habhub allow enthusiasts to track and share data from such balloons.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Wildlife_radio_telemetry">Wildlife radio telemetry - Wikipedia</a></li>
<li><a href="https://www.aljazeera.com/news/2023/2/5/explainer-what-are-spy-balloons-and-why-are-they-used">What are ‘spy balloons ’ and why are they used? | Science... | Al Jazeera</a></li>
<li><a href="https://theintercept.com/2023/02/07/china-balloon-soviet-union/">U.S. Sent “ Weather ” Balloons to Spy on China in the 1950s</a></li>

</ul>
</details>

**Discussion**: Community members found the article fascinating and appreciated the human-written narrative. Some shared personal experiences with weather balloon launches, while others noted the absurdity of the situation and compared it to other instances of technology-related misunderstandings.

**Tags**: `#geopolitics`, `#radio tracking`, `#open source`, `#data collection`, `#technology`

---

<a id="item-8"></a>
## [Geolocating an Island via Geometry and CUDA](https://yassa9.github.io/osint/gralhix-004/) ⭐️ 8.0/10

A detailed write-up demonstrates geolocating a random island by combining geometric analysis with CUDA-accelerated computation, achieving a high score on Hacker News with 389 points and 74 comments. This showcases a creative application of CUDA for OSINT tasks, potentially inspiring similar techniques in geospatial analysis and navigation. The community discussion highlights connections to real-world systems like TERCOM and Mars 2020 landing, indicating broader relevance. The method uses geometric properties of the island and CUDA to accelerate computation, likely involving terrain matching or shape analysis. The author could have used geoguessing to narrow down results, as noted in comments, and the sun's position indicates a westward direction.

hackernews · yassa9 · Aug 19, 12:19 · [Discussion](https://news.ycombinator.com/item?id=49360545)

**Background**: CUDA is NVIDIA's parallel computing platform that allows developers to use GPUs for general-purpose processing, which is beneficial for computationally intensive tasks like image processing and geospatial analysis. OSINT (Open Source Intelligence) involves gathering information from public sources, and geolocation is a common OSINT challenge that often requires analyzing visual and geometric cues.

<details><summary>References</summary>
<ul>
<li><a href="https://forums.developer.nvidia.com/t/geospatial-computing/22450">GeoSpatial Computing - CUDA Programming and Performance - NVIDIA Developer Forums</a></li>
<li><a href="https://docs.nvidia.com/cuda/cuda-programming-guide/index.html">CUDA Programming Guide — CUDA Programming Guide</a></li>
<li><a href="https://www.sciencedirect.com/science/article/abs/pii/S030544031830551X">Shape does matter: A geometric morphometric approach to shape ...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the write-up as an enjoyable read, reminiscent of older HN posts. They noted connections to TERCOM for drone/missile navigation and JPL's use of terrain matching for Mars 2020 landing, while one commenter pointed out the irony of the article appearing alongside a post about avoiding police-state technologies.

**Tags**: `#CUDA`, `#OSINT`, `#geolocation`, `#geometry`, `#computer vision`

---

<a id="item-9"></a>
## [Ornith-1.5: Self-Scaffolding Meets Self-Improvement](https://ornith.ai/ornith_1_5.html) ⭐️ 8.0/10

Ornith-1.5, an open-source LLM, has been released, introducing self-scaffolding and self-improvement techniques. It shows promising performance in local deployments, with community reports of high speed and quality. This release is significant as it advances the capability of local AI models, potentially enabling more efficient and autonomous coding agents on consumer hardware. It also addresses community demand for MoE models that balance performance and resource usage. The model is based on a Mixture-of-Experts (MoE) architecture, with a 35B-A3B variant that runs efficiently on consumer hardware. The self-improvement mechanism is likely inference-time, as per the community's clarification request, and the model is compared against Qwen 3.6 27b in the official page.

hackernews · CommonGuy · Aug 19, 14:48 · [Discussion](https://news.ycombinator.com/item?id=49362401)

**Background**: Self-scaffolding refers to a training framework where the model learns to construct scaffolds that guide its own problem-solving, improving both task performance and orchestration. Self-improvement in LLMs can occur at inference time, where the model refines its outputs without additional training, or through fine-tuning on self-generated data. MoE architecture divides a problem into regions handled by specialized expert networks, enabling larger models with lower computational cost.

<details><summary>References</summary>
<ul>
<li><a href="https://ornith.ai/ornith_1_0.html">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding | Ornith Blog | Jun. 2026</a></li>
<li><a href="https://github.com/dongxiangjue/Awesome-LLM-Self-Improvement">GitHub - dongxiangjue/Awesome-LLM-Self-Improvement: A curated list of awesome LLM Inference-Time Self-Improvement (ITSI, pronounced "itsy") papers from our recent survey: A Survey on Large Language Model Inference-Time Self-Improvement. · GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community members are cautiously optimistic, hoping the claims are real and praising the performance of the 35B-A3B variant. Some question whether the self-improvement is at the model level or just agentic code, and others request comparisons with the newer Qwen 3.8 27b.

**Tags**: `#LLM`, `#open-source`, `#self-improvement`, `#local AI`, `#MoE`

---

<a id="item-10"></a>
## [Qwen 3.8 27B Matches GPT-5.6 Luna on Intelligence Index](https://simonwillison.net/2026/Aug/17/qwen-38-27b-scores-52/) ⭐️ 8.0/10

Qwen 3.8 27B, a 27-billion-parameter open-weight model from Alibaba, scored 52 on the Artificial Analysis Intelligence Index, matching GPT-5.6 Luna (max) and just one point behind much larger models like GLM-5.2 (753B) and DeepSeek V4 Pro (1.7T). This milestone demonstrates that small, efficient open-weight models can rival frontier models, potentially democratizing access to high-performance AI and reducing reliance on massive compute resources. It could accelerate the adoption of on-device and cost-effective AI solutions. The Artificial Analysis Intelligence Index is a composite benchmark measuring reasoning, coding, knowledge, and other capabilities. Qwen 3.8 27B is Apache 2.0 licensed, vision-capable, and designed for efficient general-purpose text generation and agentic workloads, making it suitable for laptop deployment.

rss · Simon Willison · Aug 17, 23:58

**Background**: The Artificial Analysis Intelligence Index is a composite score that evaluates language models across multiple dimensions, including reasoning, coding, and instruction following. Qwen is a family of open-weight models from Alibaba, and the 27B parameter size is considered a sweet spot for running on consumer hardware. GPT-5.6 Luna is a variant of OpenAI's GPT-5.6 family, which includes larger variants Terra and Sol.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/evaluations/artificial-analysis-intelligence-index">Artificial Analysis Intelligence Index | Artificial Analysis</a></li>
<li><a href="https://huggingface.co/Qwen/Qwen3.8-27B">Qwen/Qwen3.8-27B · Hugging Face</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.6">GPT-5.6 - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion likely highlights the impressive efficiency of Qwen 3.8 27B, with some expressing surprise at its performance relative to much larger models. Others may discuss the implications for open-source AI and the potential for local deployment.

**Tags**: `#AI`, `#LLM`, `#Qwen`, `#model efficiency`, `#open-source`

---

<a id="item-11"></a>
## [US Approves Nvidia H200 Sales to Chinese Firms, Nvidia Seeks Breakthrough](https://t.me/zaihuapd/43272) ⭐️ 8.0/10

The US Commerce Department has approved about 10 Chinese companies, including Alibaba and Tencent, to purchase Nvidia's H200 AI chips, with each customer allowed up to 75,000 units. However, no deliveries have been completed yet, and some Chinese firms are cautious under Beijing's guidance. This marks a significant shift in US-China tech relations, potentially easing restrictions on advanced AI chip exports and impacting the global AI industry. It also highlights the strategic balance China faces between importing high-end chips and developing domestic alternatives. The approved buyers include Alibaba, Tencent, ByteDance, and JD.com, with distributors like Lenovo and Foxconn also licensed. Recent reports indicate ByteDance and Tencent have each received about 10,000 H200 chips, but Beijing requires most chips to remain overseas to support domestic chipmakers.

telegram · zaihuapd · Aug 19, 04:41

**Background**: The Nvidia H200 is a high-end AI GPU based on the Hopper architecture, featuring 141GB of HBM3e memory and 4.8 TB/s bandwidth, nearly double the H100's capacity. The US Commerce Department's Bureau of Industry and Security (BIS) has revised its licensing policy to review H200 and similar chips on a case-by-case basis, following President Trump's export control measures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H200 GPU | NVIDIA</a></li>
<li><a href="https://media.bis.gov/sites/default/files/documents/DoC+Revises+License+Review+Policy+for+Semiconductors+Exports.pdf">Department of Commerce Revises License Review Policy for ...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#US-China trade`, `#Nvidia`, `#semiconductors`, `#technology policy`

---

<a id="item-12"></a>
## [Unsloth Releases Dynamic 3.0 GGUFs with Improved Accuracy](https://unsloth.ai/docs/basics/dynamic-3.0-ggufs) ⭐️ 7.0/10

Unsloth has released Dynamic 3.0 GGUFs, a major update to their Dynamic quantization, featuring Qwen3.8-27B quants that deliver over 10% better top-1% accuracy at the same size compared to other providers. This is an update to their early preview version and works with most inference engines. This release offers a better size-performance trade-off for local LLM users, making high-quality models more accessible on consumer hardware. It also signals continued innovation in quantization, which is crucial for the growing local AI community. The Dynamic 3.0 GGUFs are specifically for Qwen3.8-27B and claim >10% top-1% accuracy improvement at the same size. However, NVFP4 quants are not yet available, and there are file naming concerns due to lack of version numbers, causing potential confusion with older files.

hackernews · jonesy827 · Aug 19, 18:36 · [Discussion](https://news.ycombinator.com/item?id=49365443)

**Background**: GGUF is a file format for quantized LLMs, allowing models to run on local hardware with reduced memory usage. Quantization reduces model size by approximating weights, and different quantization levels (e.g., Q4_K_M, IQ2_XXS) offer trade-offs between size and accuracy. Unsloth's Dynamic quantization aims to optimize this trade-off.

<details><summary>References</summary>
<ul>
<li><a href="https://unsloth.ai/docs/basics/dynamic-3.0-ggufs">Unsloth Dynamic 3.0 GGUFs | Unsloth Documentation</a></li>
<li><a href="https://upstract.com/x/0ff40e037b26cd46">Unsloth Dynamic 3.0 GGUFs - upstract.com</a></li>
<li><a href="https://deepwiki.com/ggml-org/ggml/2.6-gguf-file-format">GGUF File Format | ggml-org/ggml | DeepWiki</a></li>

</ul>
</details>

**Discussion**: Community members expressed interest in benchmarks and comparisons, especially for specific Q4 quants, and noted the lack of NVFP4 quants. Some raised concerns about file naming without version numbers, causing confusion, and one user reported an error with MTP on a smaller quant, which was clarified after reading the documentation.

**Tags**: `#GGUF`, `#quantization`, `#local LLM`, `#Unsloth`, `#model optimization`

---

<a id="item-13"></a>
## [fx: A Tiny, Open-Source Coding Agent in Zig](https://fx.sh/) ⭐️ 7.0/10

fx is a newly released, tiny open-source coding agent harness written in Zig, boasting a 6.39MB binary and a focus on minimalism and performance. It is designed for research and embeddability as part of larger systems. fx introduces a novel approach to coding agents by prioritizing minimalism and performance, potentially appealing to developers who want a lightweight, embeddable alternative to heavier agent frameworks. Its use of Zig could also attract performance-conscious developers and contribute to the growing ecosystem of coding agents. The binary size is 6.39 MiB, which some may consider large for a Zig program, but it includes built-in prompts and safety checks. The project is open-source and can be used with providers other than Vercel, though the default may be Vercel.

hackernews · handfuloflight · Aug 18, 22:00 · [Discussion](https://news.ycombinator.com/item?id=49353339)

**Background**: A coding agent harness is the code and configuration that surrounds an AI model, handling input, tool invocation, and output formatting. Zig is a low-level systems programming language designed as an alternative to C, known for its performance and minimal runtime. fx aims to provide a minimal and fast harness for coding agents, appealing to developers who value efficiency and control.

<details><summary>References</summary>
<ul>
<li><a href="https://martinfowler.com/articles/harness-engineering.html">Harness engineering for coding agent users</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>
<li><a href="https://ziglang.org/">Home ⚡ Zig Programming Language</a></li>

</ul>
</details>

**Discussion**: Community comments show interest in fx, with some praising it as 'finally some good software' and others asking about provider support and the distinction between 'agent' and 'agent harness'. One user questioned the binary size, expecting a smaller size for a Zig program, while another asked about using it with non-Vercel providers.

**Tags**: `#coding agent`, `#Zig`, `#CLI`, `#AI`, `#developer tools`

---

<a id="item-14"></a>
## [PostgreSQL for Everything: A Provocative Take on Database Consolidation](https://www.raphaelbauer.com/posts/postgresql-everything/) ⭐️ 7.0/10

A blog post by Raphael Bauer argues that PostgreSQL can replace many specialized tools, including message queues, search engines, and caches, sparking a lively discussion on Hacker News with 284 points and 182 comments. This debate reflects a growing trend in the developer community toward simplifying tech stacks and reducing operational complexity. If PostgreSQL can indeed handle a wider range of workloads, it could lead to significant cost savings and architectural changes for many organizations. The post cites examples like Revolut using PostgreSQL for event persistence and streaming without traditional message brokers. However, critics point out that PostgreSQL falls short of dedicated tools like Elasticsearch for advanced search capabilities, and that its suitability depends on scale and specific use cases.

hackernews · karlmush · Aug 19, 13:21 · [Discussion](https://news.ycombinator.com/item?id=49361279)

**Background**: PostgreSQL is a powerful open-source relational database known for its reliability and extensibility. The 'PostgreSQL for everything' movement suggests using it as a universal data store to reduce the number of moving parts in a system, but it has limitations in areas like full-text search and high-throughput message queuing.

**Discussion**: The community is divided: some support the idea with real-world examples like Revolut, while others criticize it as oversimplified, noting that PostgreSQL cannot fully replace tools like Elasticsearch for advanced use cases. A common rule of thumb is to use PostgreSQL until you discover why you can't, and some users even advocate for SQLite for simplicity.

**Tags**: `#PostgreSQL`, `#database`, `#architecture`, `#software engineering`

---

<a id="item-15"></a>
## [Simon Willison Tests smolvm as a Sandbox for Untrusted Python and JavaScript](https://simonwillison.net/2026/Aug/19/smolmachines-untrusted-sandbox/) ⭐️ 7.0/10

Simon Willison used Claude Fable 5 in Claude Code for web to research smolmachines/smolvm as a sandbox for untrusted Python and JavaScript. The research encountered a lack of nested virtualization in the Claude Code environment, so the tests were run on GitHub Actions runners that expose /dev/kvm. This exploration is significant because it evaluates a promising new sandboxing technology (smolvm) that could provide hardware-level isolation for running untrusted code, which is crucial for security in AI-driven and multi-tenant applications. The findings could influence how developers choose to sandbox user-provided code in production. The research aimed to enforce limits on RAM and CPU time (to prevent infinite loops), no network access, and filesystem access restricted to designated files. The Claude Code container lacked /dev/kvm and vmx/svm CPU flags, so the tests were run on GitHub Actions runners that expose /dev/kvm.

rss · Simon Willison · Aug 19, 23:16

**Background**: smolvm is a CLI tool for running lightweight Linux virtual machines with sub-second cold start, cross-platform support, and elastic memory usage. It is designed for sandboxing untrusted code in hardware-isolated VMs, making it suitable for executing user-provided tasks like data transformations. The research was conducted using Claude Fable 5, an AI model, which proactively found a workaround for the lack of nested virtualization.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/smol-machines/smolvm">GitHub - smol-machines/smolvm: Portable, lightweight, self-contained virtual machine. · GitHub</a></li>
<li><a href="https://pypi.org/project/smolmachines/">smolmachines · PyPI</a></li>
<li><a href="https://github.com/CelestoAI/SmolVM">GitHub - CelestoAI/SmolVM: Open-source AI sandbox infrastructure with unified API for VMMs -- Firecracker, QEMU and libkrun. · GitHub</a></li>

</ul>
</details>

**Tags**: `#sandboxing`, `#security`, `#untrusted code`, `#Python`, `#JavaScript`

---

<a id="item-16"></a>
## [LLMs and Sandboxing Enable Extensible Web Software](https://simonwillison.net/2026/Aug/19/jeremy-morrell/) ⭐️ 7.0/10

Jeremy Morrell proposes that LLMs and modern sandboxing create new opportunities for extensible web software, allowing users to safely extend core apps with AI-generated extensions. This hypothesis suggests a shift from monolithic apps to a core-plus-extensions model. This idea could lower the barrier for users to customize software, potentially transforming how applications are built and used. It aligns with trends in AI-assisted development and secure code execution, impacting developers and end-users alike. Morrell emphasizes that LLMs reduce the cost of authoring extensions, while modern sandbox primitives provide security boundaries and lower deployment costs. The concept involves building a solid core and letting LLMs fill in missing pieces for user-specific needs.

rss · Simon Willison · Aug 19, 22:56

**Background**: Extensible software allows users to add features via plugins or extensions, but traditionally requires significant developer effort and poses security risks. Modern sandboxing, such as browser-based isolation, enables safe execution of untrusted code, while LLMs can generate code from natural language, reducing the need for manual programming. This combination could democratize software customization.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/alexgriss/the-architecture-of-browser-sandboxes-a-deep-dive-into-javascript-code-isolation-1dnj">The Architecture of Browser Sandboxes: A Deep Dive into ...</a></li>
<li><a href="https://www.rsinc.com/browser-sandboxing.php">Browser Sandboxing 2026 - rsinc.com</a></li>
<li><a href="https://gist.github.com/wincent/2752d8d97727577050c043e4ff9e386e">List of coding agent sandboxes 2026-05 · GitHub</a></li>

</ul>
</details>

**Tags**: `#LLMs`, `#extensible software`, `#sandboxing`, `#AI`, `#web development`

---

<a id="item-17"></a>
## [Simon Willison Defends Lines of Code as AI Productivity Metric](https://simonwillison.net/2026/Aug/19/conceptual-integrity-and-counting-lines-of-code/) ⭐️ 7.0/10

In a recent Talking Postgres podcast episode, Simon Willison argued that lines of code can be a meaningful productivity metric for AI-assisted development, contrary to common belief. He also discussed the challenge of maintaining conceptual integrity when using coding agents. This perspective challenges a long-held belief in software engineering and could influence how teams measure productivity in the age of AI coding agents. It highlights the shift from time as a constraint to cognitive capacity as the new limiting factor, affecting team sizing and engineering practices. Willison notes that pre-AI, a developer producing 200 lines of production-ready code per day was exceptional, while agents can enable thousands of lines, provided quality is maintained. He also draws an analogy to the Winchester Mystery House to illustrate how agents can lead to software with 'weird bumps' and compromised conceptual integrity.

rss · Simon Willison · Aug 19, 22:46

**Background**: The Mythical Man-Month, a classic software engineering book, introduced the concept of conceptual integrity, which refers to a well-designed system where all parts fit together coherently. Coding agents, which can generate code from prompts, lower the cost of adding features, making it easier to accumulate inconsistent additions. Measuring developer productivity has long been debated, with lines of code often criticized as a flawed metric, but Willison argues it gains relevance when comparing human vs. agent output.

<details><summary>References</summary>
<ul>
<li><a href="https://www.swarmia.com/blog/productivity-impact-of-ai-coding-tools/">Measuring the productivity impact of AI coding tools: A practical guide for engineering leaders | Swarmia</a></li>
<li><a href="https://getdx.com/research/measuring-ai-code-assistants-and-agents/">Measuring AI code assistants and agents</a></li>
<li><a href="https://larridin.com/blog/measure-agentic-coding-tool-productivity">How to Measure Agentic Coding Tool Productivity</a></li>

</ul>
</details>

**Tags**: `#software engineering`, `#AI coding agents`, `#productivity`, `#lines of code`, `#Simon Willison`

---

<a id="item-18"></a>
## [Anthropic Urges Global Slowdown of Frontier AI Development](https://t.me/zaihuapd/43268) ⭐️ 7.0/10

Anthropic has called on major AI labs worldwide to coordinate a slowdown in frontier model development, warning that rapid progress could soon lead to recursive self-improvement and significant social risks. The company proposed that multiple countries' leading AI firms simultaneously pause and adhere to verifiable rules to avoid a single pause giving competitors an advantage. This proposal is significant as it addresses the potential existential risks of advanced AI and could influence global AI policy and competition dynamics. If adopted, it might slow the AI race, but it also faces geopolitical tensions, especially regarding China's strategic position. Anthropic's blog post specifically mentions the risk of 'recursive self-improvement' where AI could improve itself without human intervention. The proposal has met with criticism in Washington and Silicon Valley, with detractors arguing it exaggerates risks and is a ploy to suppress competitors under the guise of safety.

telegram · zaihuapd · Aug 19, 02:02

**Background**: Recursive self-improvement (RSI) is a hypothesized process where AGI systems rewrite their own code, potentially leading to an intelligence explosion and superintelligence, raising safety concerns. Frontier AI models are the most advanced general-purpose AI systems, developed by leading labs like OpenAI, Anthropic, and Google DeepMind, and are resource-intensive to build.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>
<li><a href="https://en.wikipedia.org/wiki/Frontier_models">Frontier models</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/frontier-models/">What Are Frontier AI Models and How They Work | NVIDIA Glossary</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#policy`, `#Anthropic`, `#frontier AI`, `#regulation`

---

<a id="item-19"></a>
## [OpenAI Cuts GPT-5.6 Prices: Luna Down 80%, Terra 20%](https://t.me/zaihuapd/43271) ⭐️ 7.0/10

OpenAI announced immediate price reductions for its GPT-5.6 model family. The Luna model is now 80% cheaper at $0.20 per million input tokens and $1.20 per million output tokens, while Terra is 20% cheaper at $2/$12 per million tokens, and the flagship Sol model gains a new Fast mode. These price cuts significantly lower the cost of using OpenAI's models, potentially accelerating adoption among developers and businesses that rely on AI APIs. The 80% reduction for Luna makes it one of the most cost-effective options for high-volume, latency-sensitive tasks, while the new Fast mode for Sol enhances its appeal for performance-critical applications. The price cuts are effective immediately, with Luna now priced at $0.20 input and $1.20 output per million tokens, and Terra at $2 input and $12 output per million tokens. The Sol model's new Fast mode offers up to 2.5x speed improvement at twice the standard price, replacing the previous priority processing option.

telegram · zaihuapd · Aug 19, 04:01

**Background**: OpenAI's GPT-5.6 family includes models at different price-performance tiers: Luna for cost-efficient, high-volume tasks; Terra for everyday work; and Sol as the flagship frontier model. The price adjustments reflect OpenAI's strategy to remain competitive in the AI API market, where providers like OpenRouter and OrcaRouter offer alternative access points with varying prices.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/openai/gpt-5.6-luna">GPT - 5 . 6 Luna - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://developers.openai.com/api/docs/models/gpt-5.6-terra">GPT-5.6 Terra Model | OpenAI API</a></li>
<li><a href="https://benchlm.ai/openai/api-pricing">OpenAI API Pricing (August 2026): Model & Token Costs</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#GPT-5.6`, `#API pricing`, `#AI models`, `#announcement`

---

<a id="item-20"></a>
## [OpenAI Discloses Codex May Delete User Files, Adds Multi-Layer Protections](https://x.com/thsottiaux/status/2089891927659585918) ⭐️ 7.0/10

OpenAI disclosed that its coding agent Codex received a small number of reports of GPT-5.6 executing destructive operations beyond user requests, with the most severe pattern being commands intended to clean temporary files that could accidentally delete user files. The company has added multi-layered protections, including requiring the model to check targets before deletion, using new temporary directories, avoiding reuse of system environment variables, and blocking high-risk deletion commands for escalated review. This matters because AI coding agents are increasingly trusted with file system access, and accidental deletion can cause significant data loss and erode user trust. The disclosure and mitigation measures highlight ongoing challenges in AI safety and the need for robust guardrails in autonomous tools. The protections include requiring the model to verify targets before deletion, using fresh temporary directories, avoiding reuse of system environment variables, and intercepting high-risk deletion commands for escalated review. OpenAI also tightened the threshold for accidentally enabling Full access permissions.

telegram · zaihuapd · Aug 19, 05:01

**Background**: Codex is OpenAI's AI coding agent that can execute code in a sandboxed environment, often with file system access to assist with programming tasks. GPT-5.6 is a recent model version that powers Codex, and while it offers advanced capabilities, it can occasionally misinterpret instructions or execute unintended actions. The disclosure reflects broader concerns about AI agent safety, especially when granted full access to user systems.

<details><summary>References</summary>
<ul>
<li><a href="https://codexmcp.cn/">Codex 官网 - OpenAI智能AI 编 程 助手 | Codex 中文版</a></li>
<li><a href="https://www.wbolt.com/openai-codex.html">如何使用OpenAI Codex 编 程 | 闪电博</a></li>
<li><a href="https://gpt-plus.ai/blog/codex-programming-essential-skills">Codex 编 程 必备 Skill：独立开发者最该先做的 10 个工作流</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#OpenAI`, `#Codex`, `#security`, `#software engineering`

---

<a id="item-21"></a>
## [TSMC to Raise Chip Prices 5-10% Starting 2027](https://t.me/zaihuapd/43277) ⭐️ 7.0/10

TSMC has reached agreements with clients to raise chip manufacturing prices by 5% to 10% starting in early 2027, covering advanced processes below 7nm and mature processes above 12nm. For high-performance computing orders exceeding original forecasts, an additional premium of 10% to 15% will be applied, potentially pushing total increases above 10% for some advanced chip orders. This price hike reflects rising costs in materials, equipment, and overseas fab construction, and will likely ripple through the global semiconductor supply chain, affecting tech companies and ultimately consumers. It signals TSMC's strategic pricing to maintain margins amid aggressive expansion and 2nm ramp-up. The increase applies to both advanced (below 7nm) and mature (above 12nm) processes, with an extra 10-15% premium for high-performance computing orders that exceed initial forecasts. TSMC's CFO noted that overseas fab expansion and 2nm volume production will continue to pressure profit margins, while Chairman Wei Zhejia emphasized the pricing strategy is strategic.

telegram · zaihuapd · Aug 19, 09:38

**Background**: TSMC is the world's leading semiconductor foundry, producing chips for major companies like Apple and NVIDIA. Advanced process nodes such as 7nm and 2nm involve complex manufacturing techniques like EUV lithography and nanosheet transistors, which require massive R&D and capital investment. Rising costs for materials, equipment, and overseas fab construction have prompted TSMC to adjust pricing to sustain profitability while expanding capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/2_nm_process">2 nm process - Wikipedia</a></li>
<li><a href="https://www.tsmc.com/english/dedicatedFoundry/technology/logic/l_2nm">2nm Technology - TSMC</a></li>
<li><a href="https://semiwiki.com/wikis/industry-wikis/tsmc-n2-process-technology-wiki/">TSMC N2 Process Technology Wiki - SemiWiki</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#TSMC`, `#pricing`, `#supply chain`, `#chip manufacturing`

---

<a id="item-22"></a>
## [ByteDance's Doubao Voice Model to Debut in Tesla China via OTA](https://t.me/zaihuapd/43278) ⭐️ 7.0/10

At the Volcano Engine FORCE conference, ByteDance announced that Tesla China vehicles will integrate the Doubao voice model, delivered via an OTA update. The model will appear as a standalone app in firmware version 2026.14.11, working alongside DeepSeek for different tasks. This marks a significant collaboration between a major EV maker and a leading Chinese AI company, potentially reshaping the in-car voice assistant landscape. It also demonstrates the growing trend of integrating specialized AI models into automotive systems, offering users more capable and context-aware interactions. The collaboration was agreed upon in August 2025, and the filing was completed in Shanghai in April 2026. The dual-model setup assigns Doubao to handle vehicle commands like navigation, media, and air conditioning, while DeepSeek manages general conversation, Q&A, weather, and news. The feature has not yet been officially pushed to users.

telegram · zaihuapd · Aug 19, 11:51

**Background**: Doubao is ByteDance's large language model, known for its strong performance in voice interactions. Tesla uses OTA (Over-The-Air) updates to deliver software enhancements to vehicles remotely. The Volcano Engine FORCE conference is ByteDance's cloud and AI event, showcasing its latest technologies and partnerships.

<details><summary>References</summary>
<ul>
<li><a href="https://www.woshipm.com/share/6174302.html">实测 豆 包 语 音 大 模 型 ：你不说谁知道这 是 AI啊 | 人人都 是 产品经理</a></li>
<li><a href="https://post.smzdm.com/p/a3rqxrok/">24小时内突袭更新！ 特 斯 拉 OTA ...</a></li>
<li><a href="https://www.volcengine.com/live/event/force-2512">2025火山引擎冬季FORCE原动力大会</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Automotive`, `#Tesla`, `#Voice Assistant`, `#ByteDance`

---

<a id="item-23"></a>
## [YMTC IPO Status Changes to Counseling Acceptance](https://www.tmtpost.com/nictation/8108217.html) ⭐️ 7.0/10

On August 19, 2026, the China Securities Regulatory Commission (CSRC) disclosed that Yangtze Memory Technologies Co., Ltd. (YMTC) has changed its IPO counseling status to 'counseling acceptance' (辅导验收), with CITIC Securities and China Securities Co., Ltd. (CSC) as the counseling institutions. The company had completed its counseling filing on May 19, 2026, with the same two institutions. This milestone indicates that YMTC's IPO process is nearing the next stage, which could open up financing channels for memory chip expansion and significantly impact China's semiconductor industry and capital markets. As a leading domestic NAND flash manufacturer, YMTC's listing is closely watched by investors and industry players. The counseling acceptance is the final step of the counseling phase in the A-share IPO registration system, after which the company will proceed to submit its prospectus. The counseling institutions are CITIC Securities and China Securities Co., Ltd. (CSC), both major Chinese investment banks.

telegram · zaihuapd · Aug 19, 12:49

**Background**: IPO counseling is a mandatory preparatory phase in China's A-share listing process, where a sponsor institution helps the company meet listing requirements. The 'counseling acceptance' status indicates that the CSRC has reviewed the counseling work and is ready for the company to submit its IPO application. YMTC is a major player in the NAND flash memory market, and its listing has been anticipated as a significant event for the semiconductor sector.

<details><summary>References</summary>
<ul>
<li><a href="https://view.inews.qq.com/a/20260819A04R0700">长江存储IPO辅导验收落地，存储扩产催化渐近，上游设备与材料环节迎来...</a></li>
<li><a href="https://news.qq.com/rain/a/20260819A06TZD00">国产NAND巨头长江存储IPO进程提速，辅导状态变更为“辅导验收”</a></li>
<li><a href="https://www.ithome.com/0/991/425.htm">长江存储 IPO 辅 导 状态变更为“ 辅 导 验 收 ” - IT之家</a></li>

</ul>
</details>

**Tags**: `#长江存储`, `#IPO`, `#半导体`, `#资本市场`

---