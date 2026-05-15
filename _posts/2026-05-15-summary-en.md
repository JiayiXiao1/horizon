---
layout: default
title: "Horizon Summary: 2026-05-15 (EN)"
date: 2026-05-15
lang: en
---

> From 36 items, 17 important content pieces were selected

---

1. [First Public macOS Kernel Exploit on Apple M5](#item-1) ⭐️ 9.0/10
2. [Bun Rewritten from Zig to Rust, Merged](#item-2) ⭐️ 9.0/10
3. [18-Year-Old NGINX RCE Flaw (CVE-2026-42945) Threatens Billions of Servers](#item-3) ⭐️ 9.0/10
4. [DeepSeek Session Isolation Bug Leaks User Conversations](#item-4) ⭐️ 9.0/10
5. [vLLM v0.21.0: KV Offload, Blackwell Backend, Breaking Changes](#item-5) ⭐️ 8.0/10
6. [Removing Modem and GPS from 2024 RAV4 Hybrid](#item-6) ⭐️ 8.0/10
7. [RTX 5090 eGPU on M4 MacBook Air: Gaming & LLM Gains](#item-7) ⭐️ 8.0/10
8. [arXiv Bans Authors for 1 Year Over AI Hallucinated References](#item-8) ⭐️ 8.0/10
9. [Anthropic partners with SpaceX for massive GPU compute](#item-9) ⭐️ 8.0/10
10. [US Clears H200 Sales to China, Nvidia Seeks Breakthrough](#item-10) ⭐️ 8.0/10
11. [JD.com Launches AI Hardware Store with Sanctioned NVIDIA GPUs](#item-11) ⭐️ 8.0/10
12. [Codex Now Available in ChatGPT Mobile App for Free](#item-12) ⭐️ 7.0/10
13. [MIT President Addresses Funding and Talent Pipeline Crisis](#item-13) ⭐️ 7.0/10
14. [CSP Allow-list Experiment: Dynamic Domain Whitelisting](#item-14) ⭐️ 7.0/10
15. [Obesity rates plateau in rich nations, rise in poorer ones](#item-15) ⭐️ 7.0/10
16. [ChatGPT Android Teardown Reveals Codex Remote Desktop Feature](#item-16) ⭐️ 7.0/10
17. [China in Talks for Up to 500 Boeing 737 MAX Jets](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [First Public macOS Kernel Exploit on Apple M5](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

A security research team published the first public kernel memory corruption exploit targeting Apple's M5 chip, accompanied by a 55-page technical report. This exploit demonstrates that even Apple's latest M5 chip with advanced mitigations like MTE can be compromised, highlighting ongoing security challenges and potentially influencing bug bounty valuations. The exploit was achieved within a week against the best protections, and the report details how the bug survived through Memory Tagging Extension (MTE). The exploit's value on Apple's bug bounty platform is estimated at $100,000, but could reach $1.5 million if packaged appropriately.

hackernews · quadrige · May 14, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48139219)

**Background**: Apple M5 is the latest ARM-based SoC from Apple, built on third-generation 3nm technology, featuring a 10-core GPU with Neural Accelerators. Kernel memory corruption exploits target the operating system's core to gain elevated privileges, and MTE is a hardware mitigation designed to detect memory safety errors.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://www.apple.com/newsroom/2025/10/apple-unleashes-m5-the-next-big-leap-in-ai-performance-for-apple-silicon/">Apple unleashes M5, the next big leap in AI performance for Apple silicon - Apple</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed reactions: some praised the technical achievement and looked forward to the report, while others questioned how the bug bypassed MTE. There was also debate about the exploit's bug bounty value, with estimates ranging from $100,000 to $1.5 million. A sarcastic comment suggested Apple might be fabricating vulnerabilities to hype Mythos, and one user regretted buying the M5 specifically for MIE.

**Tags**: `#macOS`, `#kernel exploit`, `#Apple M5`, `#security`, `#memory corruption`

---

<a id="item-2"></a>
## [Bun Rewritten from Zig to Rust, Merged](https://github.com/oven-sh/bun/pull/30412) ⭐️ 9.0/10

Bun's core has been rewritten from Zig to Rust, resulting in over 1 million lines of Rust code, and the pull request has been merged into the main branch. This rewrite marks a major architectural shift for Bun, a widely-used JavaScript runtime, potentially improving memory safety and performance while reducing bugs like use-after-free and double-free errors. The rewrite took about one week of active coding, but was preceded by extensive preparation including detailed mapping of Zig idioms to Rust equivalents. The codebase now contains over 1 million lines of Rust, with approximately 10,428 unsafe blocks across 736 files.

hackernews · Chaoses · May 14, 08:15 · [Discussion](https://news.ycombinator.com/item?id=48132488)

**Background**: Bun is a fast all-in-one JavaScript runtime that includes a bundler, transpiler, task runner, and npm client. It was originally written in Zig, a systems programming language focused on robustness and optimality. Rust is another systems language known for memory safety without garbage collection. This rewrite moves Bun from Zig to Rust, leveraging Rust's ownership model to prevent common memory bugs.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://en.wikipedia.org/wiki/Zig_(programming_language)">Zig (programming language)</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the impressive preparation and mapping between Zig and Rust idioms, with some noting the codebase size approaching that of the Rust compiler. Concerns were raised about the high number of unsafe blocks, but the Bun maintainer explained that Rust eliminates many memory bugs that were common in the Zig version.

**Tags**: `#Bun`, `#Rust`, `#JavaScript Runtime`, `#Software Rewrite`, `#Systems Programming`

---

<a id="item-3"></a>
## [18-Year-Old NGINX RCE Flaw (CVE-2026-42945) Threatens Billions of Servers](https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability) ⭐️ 9.0/10

A critical heap buffer overflow vulnerability (CVE-2026-42945, CVSS 9.2) in NGINX's rewrite module, present since 2008, was disclosed on May 13, 2026, affecting all versions from 0.6.27 to 1.30.0 and multiple enterprise products. Patches are available in NGINX 1.31.0 and 1.30.1. This vulnerability allows unauthenticated remote code execution on NGINX workers, potentially compromising billions of servers used in cloud-native environments, Kubernetes ingress, and API gateways. The 18-year-old root cause highlights the difficulty of detecting subtle memory safety bugs in legacy C code. The bug arises from an inconsistency in NGINX's two-pass script engine: the `is_args` flag remains set after a rewrite containing '?', causing the first pass to allocate insufficient buffer space, while the second pass writes escaped characters (e.g., '+' expands to 3 bytes). Exploitation requires a specific configuration with `rewrite` and `set` directives using unnamed capture groups.

telegram · zaihuapd · May 14, 02:41

**Background**: NGINX is a widely used open-source web server and reverse proxy, often deployed as a Kubernetes ingress controller or API gateway. The rewrite module processes URL rewrites using a two-pass engine: first to calculate buffer size, then to copy data. A heap buffer overflow occurs when the size calculation underestimates the actual data written, potentially allowing an attacker to overwrite adjacent memory and execute arbitrary code.

<details><summary>References</summary>
<ul>
<li><a href="https://depthfirst.com/research/nginx-rift-achieving-nginx-rce-via-an-18-year-old-vulnerability">NGINX Rift: Achieving NGINX Remote Code Execution via... | depthfirst</a></li>
<li><a href="https://thehackernews.com/2026/05/18-year-old-nginx-rewrite-module-flaw.html">18-Year-Old NGINX Rewrite Module Flaw Enables Unauthenticated RCE</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/18-year-old-nginx-vulnerability-allows-dos-potential-rce/">18-year-old NGINX vulnerability allows DoS, potential RCE</a></li>

</ul>
</details>

**Discussion**: Community comments note that the published proof-of-concept disables ASLR, but the researchers claim a reliable bypass exists. Some users suggest using named capture groups as a mitigation, while others debate the practicality of exploitation in real-world deployments with ASLR enabled.

**Tags**: `#security`, `#nginx`, `#vulnerability`, `#rce`, `#cve`

---

<a id="item-4"></a>
## [DeepSeek Session Isolation Bug Leaks User Conversations](https://github.com/deepseek-ai/DeepSeek-R1/issues/840) ⭐️ 9.0/10

A session isolation vulnerability in DeepSeek's dialogue system allows attackers to retrieve other users' conversation fragments by sending an unclosed <think string in an empty chat. This vulnerability exposes sensitive user data such as code, keys, and private information, affecting both Web and API users of DeepSeek, a widely-used AI chatbot. The attack works by sending an unclosed <think string in a brand new empty conversation, causing the model to return fragments from other users' histories. The vulnerability was responsibly disclosed by reporter cancat2024 on May 11, 2026.

telegram · zaihuapd · May 14, 13:15

**Background**: DeepSeek is a generative AI chatbot developed by the Chinese company DeepSeek, released in January 2025. Session isolation is a security mechanism that ensures each user's data is kept separate; a failure in this isolation can lead to cross-user data leakage.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/DeepSeek_(chatbot)">DeepSeek (chatbot) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Community comments note that third-party deployments also exhibit this behavior, suggesting it may be a hallucination issue rather than a pure isolation flaw.

**Tags**: `#security`, `#vulnerability`, `#AI`, `#DeepSeek`, `#data leak`

---

<a id="item-5"></a>
## [vLLM v0.21.0: KV Offload, Blackwell Backend, Breaking Changes](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 introduces KV cache offloading with a hybrid memory allocator, a new TOKENSPEED_MLA attention backend for NVIDIA Blackwell GPUs, and speculative decoding that respects thinking budgets. It also deprecates transformers v4 and raises the C++ build requirement to C++20. These features significantly improve memory efficiency and inference speed for large language models, especially on Blackwell hardware. The breaking changes may require users to update their build environments and model loading code. The KV offloading with HMA supports sliding window groups and distributed offloading via MooncakeStoreConnector. The TOKENSPEED_MLA backend is optimized for DeepSeek-R1 and Kimi-K25 models on Blackwell GPUs. Speculative decoding now correctly caps reasoning tokens when a thinking budget is set.

github · khluu · May 14, 23:15

**Background**: vLLM is a high-throughput LLM inference engine that manages KV cache to reduce memory usage. KV offloading moves cache data to CPU memory when GPU memory is full. Speculative decoding uses a smaller draft model to generate tokens faster, but previously ignored thinking budgets for reasoning models.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/hybrid_kv_cache_manager/">Hybrid KV Cache Manager - vLLM</a></li>
<li><a href="https://vllm-project.github.io/2026/01/08/kv-offloading-connector.html">Inside vLLM’s New KV Offloading Connector: Smarter Memory ...</a></li>
<li><a href="https://github.com/vllm-project/vllm/issues/39573">[Bug]: Thinking token budget not enforced with MTP ... - GitHub</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#breaking changes`, `#speculative decoding`

---

<a id="item-6"></a>
## [Removing Modem and GPS from 2024 RAV4 Hybrid](https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/) ⭐️ 8.0/10

A detailed guide was published on physically removing the Data Communication Module (DCM) and built-in GPS from a 2024 RAV4 Hybrid to stop telemetry data collection. This empowers car owners to take direct control over their vehicle's data privacy, bypassing corporate opt-out policies, and highlights the growing tension between connected car features and user privacy. After modem removal, Bluetooth pairing still allows the car to use the phone's internet to send telemetry; wired USB CarPlay is recommended instead, though CarPlay itself also collects vehicle data.

hackernews · arkadiyt · May 14, 17:08 · [Discussion](https://news.ycombinator.com/item?id=48138136)

**Background**: Modern vehicles like the RAV4 are equipped with telematics units that continuously transmit driving data to manufacturers. Toyota's Safety Connect and similar services collect location, speed, and other metrics, often shared with third parties like insurers if the owner is opted in.

<details><summary>References</summary>
<ul>
<li><a href="https://arkadiyt.com/2026/05/13/removing-the-modem-and-gps-from-my-rav4/">Removing the Modem and GPS from my 2024 RAV4 Hybrid</a></li>
<li><a href="https://www.cryptogon.com/?p=75142">cryptogon.com » “Removing the Modem and GPS from my 2024 RAV4 ...</a></li>
<li><a href="https://conzit.com/post/taking-control-disabling-data-tracking-in-2024-rav4-hybrid">Taking Control: Disabling Data Tracking in 2024 RAV4 Hybrid</a></li>

</ul>
</details>

**Discussion**: Commenters noted alternative methods like fuse removal on the Ford Maverick, and debated whether Toyota shares data with insurers only when the owner is opted in. Some expressed frustration with Toyota's denial of GPS issues affecting CarPlay navigation.

**Tags**: `#privacy`, `#automotive`, `#telematics`, `#hardware hacking`, `#data ownership`

---

<a id="item-7"></a>
## [RTX 5090 eGPU on M4 MacBook Air: Gaming & LLM Gains](https://scottjg.com/posts/2026-05-05-egpu-mac-gaming/) ⭐️ 8.0/10

A developer successfully connected an NVIDIA RTX 5090 eGPU to an M4 MacBook Air via Thunderbolt, enabling playable gaming and significantly faster LLM inference. The setup overcomes Apple's official lack of eGPU support on Apple Silicon through a custom Linux VM with GPU passthrough. This breakthrough demonstrates that eGPUs can work on Apple Silicon, potentially expanding Mac gaming and AI capabilities. It also highlights a practical path for Mac users to access high-end NVIDIA GPUs for LLM inference, addressing the prompt processing bottleneck of Apple's unified memory. The setup uses a Linux VM with GPU passthrough, limiting GPU memory to a 1.5 GB window due to macOS restrictions. Game benchmarks show playable frame rates, and LLM prompt processing speed improves dramatically compared to native Apple Silicon.

hackernews · allenleee · May 14, 15:47 · [Discussion](https://news.ycombinator.com/item?id=48137145)

**Background**: Apple Silicon Macs integrate CPU and GPU on a single chip with unified memory, which is great for many tasks but blocks external GPU support. eGPUs were officially supported only on Intel-based Macs, and only with AMD GPUs. NVIDIA GPUs have never been officially supported on macOS. This project uses a custom Linux VM to bypass these limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://support.apple.com/en-us/102363">Use an external graphics processor with your Mac - Apple Support</a></li>
<li><a href="https://www.aimadetools.com/blog/llm-inference-apple-silicon/">LLM Inference on Apple Silicon — M4 Performance Guide (2026)</a></li>
<li><a href="https://egpu.io/setup-guide-external-graphics-card-mac/">The Beginner’s External Graphics Card Setup Guide for Mac | eGPU.io</a></li>

</ul>
</details>

**Discussion**: The community is impressed by the technical achievement, with many noting the LLM inference improvements as the most practical benefit. Some commenters express frustration with Apple's lack of official eGPU support, while others suggest alternative approaches like using Vulkan translation layers for gaming.

**Tags**: `#eGPU`, `#Mac gaming`, `#LLM inference`, `#Apple Silicon`, `#RTX 5090`

---

<a id="item-8"></a>
## [arXiv Bans Authors for 1 Year Over AI Hallucinated References](https://twitter.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv has introduced a new policy that bans authors for one year if they submit papers containing AI-hallucinated references, followed by a requirement that future submissions must first be accepted at a reputable peer-reviewed venue. This policy directly addresses the growing problem of AI-generated inaccuracies in academic publishing, reinforcing integrity and trust in scholarly communication. The ban lasts one year, after which authors must have their papers accepted at a reputable peer-reviewed venue before posting on arXiv. The policy is reportedly being enforced as of this week.

hackernews · gjuggler · May 14, 20:39 · [Discussion](https://news.ycombinator.com/item?id=48140922)

**Background**: AI hallucination refers to when large language models generate plausible-sounding but false information, including citations to non-existent papers. This has become a significant issue in academic publishing, with studies finding hallucinated citations in papers accepted at top venues like NeurIPS.

<details><summary>References</summary>
<ul>
<li><a href="https://byteiota.com/arxiv-bans-authors-1-year-for-ai-hallucinated-citations/">arXiv Bans Authors 1 Year for AI-Hallucinated Citations</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC13051339/">Hallucinated citations produced by generative artificial ...</a></li>
<li><a href="https://spylab.ai/blog/hallucinations/">Trends in LLM-Generated Citations on arXiv - SPY Lab</a></li>

</ul>
</details>

**Discussion**: Community comments are largely supportive, with one user calling the policy 'incredibly good for science' and another stating that if authors don't check LLM output carefully, it's not worth reading. Some caution that careful vetting is needed before adverse actions, while others note that LLM enthusiasts are angry about the policy.

**Tags**: `#arXiv`, `#academic integrity`, `#AI-generated content`, `#hallucinations`, `#policy`

---

<a id="item-9"></a>
## [Anthropic partners with SpaceX for massive GPU compute](https://t.me/zaihuapd/41371) ⭐️ 8.0/10

Anthropic announced a partnership with SpaceX to access the full compute capacity of xAI's Colossus 1 data center, gaining over 300 MW of power and more than 220,000 NVIDIA GPUs within a month. Consequently, Claude Code rate limits have been doubled for Pro and Max tiers, and Claude Opus API rate limits have been significantly increased. This deal dramatically expands Anthropic's compute capacity, enabling faster model training and inference for Claude, which directly benefits developers and enterprises relying on Claude Code and Claude API. It also signals a major infrastructure scaling trend in the AI industry, where access to massive GPU clusters becomes a key competitive advantage. The Colossus 1 data center, built by xAI in Memphis, Tennessee, is currently the world's largest AI supercomputer. The partnership gives Anthropic exclusive access to its entire 300 MW capacity and over 220,000 NVIDIA GPUs, with immediate effect on Claude's service limits.

telegram · zaihuapd · May 14, 00:57

**Background**: Anthropic develops the Claude series of large language models, including Claude Code (an agentic coding tool) and Claude Opus (the most capable model). Colossus 1 is a supercomputer built by xAI, owned by SpaceX and Elon Musk, primarily used to train the Grok chatbot. This partnership provides Anthropic with massive computational resources to scale its AI services.

<details><summary>References</summary>
<ul>
<li><a href="https://www.datacenterdynamics.com/en/news/anthropic-to-use-all-of-spacex-xais-colossus-1-data-center-compute/">Anthropic to use all of SpaceX-xAI's Colossus 1 data center ...</a></li>
<li><a href="https://greyjournal.net/news/anthropic-spacex-colossus-deal/">Anthropic Rents All of SpaceX’s Colossus 1 Data Center</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#SpaceX`, `#AI Infrastructure`, `#Claude`, `#GPU`

---

<a id="item-10"></a>
## [US Clears H200 Sales to China, Nvidia Seeks Breakthrough](https://www.reuters.com/business/retail-consumer/us-clears-h200-chip-sales-10-china-firms-nvidia-ceo-looks-breakthrough-2026-05-14/) ⭐️ 8.0/10

The US Commerce Department has approved the sale of Nvidia's H200 chips to about 10 Chinese firms, including Alibaba and Tencent, with individual customers allowed to purchase up to 75,000 units. This approval signals a potential shift in US export controls on advanced AI chips to China, impacting the global AI hardware supply chain and the balance between US chip exports and China's domestic AI chip development. Despite the approvals, no deliveries have been completed yet, as Chinese firms are exercising caution under guidance from Beijing. Nvidia CEO Jensen Huang's visit to China is seen as a key effort to facilitate the transactions.

telegram · zaihuapd · May 14, 08:57

**Background**: The H200 is Nvidia's latest GPU based on the Hopper architecture, featuring 141 GB of HBM3e memory and 4.8 TB/s bandwidth, nearly double the capacity of the H100. The US has previously imposed strict export controls to limit China's access to advanced AI chips, aiming to curb its AI and defense advancements.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.runpod.io/articles/guides/nvidia-h200-gpu">Nvidia H200 GPU: Specs, VRAM, Price, and AI Performance</a></li>
<li><a href="https://www.linkedin.com/pulse/us-tightens-export-controls-ai-chips-china-dusan-simic-urqvf">US Tightens Export Controls on AI Chips to China</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#AI hardware`, `#US-China trade`, `#NVIDIA`, `#export controls`

---

<a id="item-11"></a>
## [JD.com Launches AI Hardware Store with Sanctioned NVIDIA GPUs](https://u.jd.com/HaDkFMa) ⭐️ 8.0/10

JD.com has launched an 'AI Hardware JD Self-Operated Store' featuring NVIDIA GeForce RTX 5090 32G Turbo Edition, RTX PRO 6000 Blackwell Workstation Edition, and H100 GPUs, which were previously subject to export restrictions to China. This move significantly improves access to high-end AI hardware in China, potentially boosting local AI development and circumventing previous export controls. It signals a shift in hardware availability that could affect global AI supply chains. The RTX 5090 Turbo Edition is a global unified specification without any performance cuts, while the RTX PRO 6000 features 96GB GDDR7 ECC memory and targets professional rendering and data centers. The H100 was previously halted from export to China due to sanctions.

telegram · zaihuapd · May 14, 15:15

**Background**: The U.S. government has imposed export restrictions on advanced AI chips to China, including NVIDIA's H100 and A100 GPUs, to limit China's AI capabilities. JD.com is a major Chinese e-commerce platform, and its self-operated store ensures product authenticity and reliable supply.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nvidia.com/en-us/geforce/graphics-cards/50-series/">GeForce RTX 50 Series Graphics Cards | NVIDIA</a></li>
<li><a href="https://www.nvidia.com/en-us/products/workstations/professional-desktop-gpus/rtx-pro-6000/">NVIDIA RTX PRO 6000 Blackwell Workstation Edition</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h100/">H 100 GPU | NVIDIA</a></li>

</ul>
</details>

**Tags**: `#AI hardware`, `#NVIDIA`, `#export restrictions`, `#China`, `#GPU`

---

<a id="item-12"></a>
## [Codex Now Available in ChatGPT Mobile App for Free](https://openai.com/index/work-with-codex-from-anywhere/) ⭐️ 7.0/10

OpenAI has made Codex, its AI coding agent, accessible through the ChatGPT mobile app for free, allowing users to write and debug code on the go. This expansion brings powerful AI-assisted coding to mobile devices, potentially increasing developer productivity and making coding assistance more accessible to a broader audience. Codex is included in the free plan of ChatGPT, but user interactions may be used for training. The mobile experience may be limited by screen size and lack of keyboard, leading to mixed results compared to desktop usage.

hackernews · mikeevans · May 14, 20:06 · [Discussion](https://news.ycombinator.com/item?id=48140529)

**Background**: Codex is a suite of AI-driven coding agents from OpenAI that automates software engineering tasks. It can be used via CLI, desktop app, or now the ChatGPT mobile app, with features like remote control and local execution.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/openai/codex/releases">Releases · openai / codex</a></li>
<li><a href="https://github.com/openai/codex">GitHub - openai / codex : Lightweight coding agent that runs in your...</a></li>

</ul>
</details>

**Discussion**: Community members expressed surprise that Codex is free, with some noting it's included in the free plan. Users reported mixed results on mobile due to screen and input constraints, and some desired better integration with local files and Linux support.

**Tags**: `#AI`, `#code generation`, `#mobile app`, `#OpenAI`, `#developer tools`

---

<a id="item-13"></a>
## [MIT President Addresses Funding and Talent Pipeline Crisis](https://president.mit.edu/writing-speeches/video-transcript-message-president-kornbluth-about-funding-and-talent-pipeline) ⭐️ 7.0/10

MIT President Sally Kornbluth released a video message addressing the challenges of research funding and the talent pipeline, highlighting widespread disillusionment with academia. This message signals a systemic crisis in academia, where declining funding and poor career prospects are driving PhD graduates away from research careers, potentially undermining U.S. scientific leadership. The median science PhD takes six years with grueling work and low pay, and most recent graduates are considering leaving academia despite initial career aspirations.

hackernews · dmayo · May 14, 14:51 · [Discussion](https://news.ycombinator.com/item?id=48136262)

**Background**: The U.S. research enterprise relies heavily on federal grants and a steady pipeline of talented PhDs. However, stagnating funding, rising costs, and a tight job market have led to growing dissatisfaction among early-career researchers, threatening the long-term health of academic research.

**Discussion**: Commenters expressed diverse views: some highlighted the broken academic model and generational reset, while others noted that PhDs moving to industry is not necessarily a waste. A few pointed to China's rising prominence in education as a competitive challenge.

**Tags**: `#academia`, `#research funding`, `#talent pipeline`, `#higher education`

---

<a id="item-14"></a>
## [CSP Allow-list Experiment: Dynamic Domain Whitelisting](https://simonwillison.net/2026/May/13/csp-allow/#atom-everything) ⭐️ 7.0/10

Simon Willison published an experiment that dynamically adds domains to a Content Security Policy (CSP) allow-list by intercepting fetch errors in a sandboxed iframe and prompting the user for approval. This approach offers a user-friendly way to manage CSP restrictions without breaking functionality, potentially improving web security practices by reducing the need for overly permissive policies. The experiment uses a custom fetch() inside a sandboxed iframe to catch CSP violations, then communicates the blocked origin to the parent window, which displays a dialog asking the user to add the domain to the allow-list and refresh the page.

rss · Simon Willison · May 13, 04:50

**Background**: Content Security Policy (CSP) is a browser security mechanism that restricts which resources a page can load, helping prevent cross-site scripting (XSS) attacks. Traditionally, CSP policies are static and require manual updates when new origins are needed, which can lead to overly permissive policies or broken functionality.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/May/13/csp-allow/">Tool: CSP Allow-list Experiment - simonwillison.net</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/CSP">Content Security Policy (CSP) - HTTP | MDN - MDN Web Docs</a></li>

</ul>
</details>

**Tags**: `#CSP`, `#web security`, `#sandbox`, `#iframe`, `#experiment`

---

<a id="item-15"></a>
## [Obesity rates plateau in rich nations, rise in poorer ones](https://www.nature.com/articles/s41586-026-10383-0) ⭐️ 7.0/10

A large-scale study covering 200 countries and 232 million people found that obesity rates among children and adolescents in high-income countries have slowed since the 1990s and mostly stabilized after 2000, with some countries like Italy, Portugal, and France even seeing slight declines. In contrast, obesity rates in low- and middle-income countries continue to rise steadily or accelerate. This research highlights a global shift in obesity trends, suggesting that socioeconomic and policy factors in wealthy nations may have curbed the epidemic, while poorer countries now face a growing burden. The findings underscore the need for targeted interventions in low- and middle-income countries to prevent further health and economic impacts. The study analyzed data from 1980 to 2024, covering 200 countries and 232 million individuals. In some high-income countries, adult obesity rates also plateaued after an initial rise, while in low- and middle-income countries, prevalence has in some cases surpassed that of wealthy nations.

telegram · zaihuapd · May 14, 09:45

**Background**: Obesity is a major risk factor for chronic diseases such as diabetes, heart disease, and certain cancers. The study suggests that factors like food availability, affordability, and usage, influenced by social, economic, and technological changes, may have helped high-income countries curb obesity, but similar progress has not been seen in lower-income regions.

**Tags**: `#public health`, `#obesity`, `#global health`, `#epidemiology`

---

<a id="item-16"></a>
## [ChatGPT Android Teardown Reveals Codex Remote Desktop Feature](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

An APK teardown of ChatGPT Android version 1.2026.125 reveals strings indicating OpenAI is developing a remote desktop control feature for Codex, allowing users to find and reconnect to remote sessions from their phone. This feature would significantly expand Codex's utility, enabling developers to manage coding tasks remotely from mobile devices, potentially increasing productivity and making AI-assisted development more accessible. The feature is still under development with no preview available, and it requires the desktop client to be logged into the same account as the mobile device. The official release date has not been announced.

telegram · zaihuapd · May 14, 21:48

**Background**: OpenAI Codex is an AI agent designed to automate software engineering tasks, such as building features and refactoring code. An APK teardown involves decompiling an Android app's installation file to inspect its code and resources, often revealing upcoming features not yet publicly available.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_Codex">OpenAI Codex - Wikipedia</a></li>
<li><a href="https://openai.com/codex/">Codex | AI Coding Partner from OpenAI | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#Android`, `#remote desktop`, `#AI`

---

<a id="item-17"></a>
## [China in Talks for Up to 500 Boeing 737 MAX Jets](https://t.me/zaihuapd/41389) ⭐️ 7.0/10

China and Boeing are negotiating a potential order of up to 500 Boeing 737 MAX aircraft, which would be China's first major Boeing order in nearly a decade, with an announcement expected around Trump's visit to China. This deal would mark a significant thaw in US-China trade tensions and provide a major boost to Boeing's 737 MAX program, which has faced safety and production challenges. The negotiations also include around 100 Boeing 787 and 777X wide-body jets, but those are likely to be announced separately. The deal is not yet finalized, and the announcement format and binding commitments remain under discussion.

telegram · zaihuapd · May 15, 01:09

**Background**: The Boeing 737 MAX is a narrow-body aircraft series that was grounded globally from March 2019 to November 2020 after two fatal crashes linked to its MCAS system. China was the first country to ground the MAX and has been slow to resume deliveries and orders amid trade tensions with the US.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Boeing`, `#China`, `#aviation`, `#trade`, `#737 MAX`

---