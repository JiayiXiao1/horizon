---
layout: default
title: "Horizon Summary: 2026-06-04 (EN)"
date: 2026-06-04
lang: en
---

> From 35 items, 19 important content pieces were selected

---

1. [Elixir v1.20 Introduces Gradual Typing](#item-1) ⭐️ 9.0/10
2. [Bluetooth Speaker Hacked to Inject Keystrokes via USB](#item-2) ⭐️ 9.0/10
3. [HTTP/2 Bomb DoS Attack Crashes Major Web Servers](#item-3) ⭐️ 9.0/10
4. [Google Releases Gemma 4 12B, an Encoder-Free Multimodal Model](#item-4) ⭐️ 8.0/10
5. [Ted Chiang: AI Is Not Conscious](#item-5) ⭐️ 8.0/10
6. [DaVinci Resolve 21 Adds Photo Management and Motion Graphics](#item-6) ⭐️ 8.0/10
7. [Uber Caps AI Token Spending at $1,500/Month Per Tool](#item-7) ⭐️ 8.0/10
8. [Let's Encrypt Plans Post-Quantum Certificate Transition](#item-8) ⭐️ 8.0/10
9. [Espressif ESP32-S31: RISC-V with SIMD and BitScrambler](#item-9) ⭐️ 8.0/10
10. [Mathematicians Warn About AI's Rapid Progress](#item-10) ⭐️ 8.0/10
11. [Microsoft Unveils MAI-Thinking-1 and MAI-Code-1-Flash](#item-11) ⭐️ 8.0/10
12. [SpaceX Plans $75B IPO at $135/Share, Largest Ever](#item-12) ⭐️ 8.0/10
13. [Google lets websites opt out of AI search results](#item-13) ⭐️ 8.0/10
14. [Developer Shares Anti-NMDA Receptor Encephalitis Diagnosis](#item-14) ⭐️ 7.0/10
15. [Deep Dive into Original PlayStation Architecture](#item-15) ⭐️ 7.0/10
16. [When Every Byte Matters: AoS vs SoA](#item-16) ⭐️ 7.0/10
17. [Massive Proxy Service Blocking by GFW on March 4](#item-17) ⭐️ 7.0/10
18. [Qianwen Opens Platform to Third-Party Agents and Skills](#item-18) ⭐️ 7.0/10
19. [US Teachers Union Calls for AI and Screen Limits in Elementary Schools](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Elixir v1.20 Introduces Gradual Typing](https://elixir-lang.org/blog/2026/06/03/elixir-v1-20-0-released/) ⭐️ 9.0/10

Elixir v1.20, released on June 3, 2026, introduces gradual typing, allowing developers to optionally add type annotations to their code for static type checking while maintaining full dynamic typing compatibility. This marks a paradigm shift for Elixir, addressing a long-standing community demand for static typing and potentially attracting developers who previously avoided the language due to lack of type safety. The gradual type system is implemented as an optional feature; existing untyped code remains fully valid. The initial release focuses on core type checking, with more advanced features planned for future versions.

hackernews · cloud8421 · Jun 3, 19:02 · [Discussion](https://news.ycombinator.com/item?id=48388324)

**Background**: Gradual typing is a type system that allows parts of a program to be dynamically typed and other parts to be statically typed, controlled by the presence or absence of type annotations. Elixir previously relied on Dialyzer for optional static analysis, but v1.20 brings native type checking directly into the compiler.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gradual_typing">Gradual typing - Wikipedia</a></li>
<li><a href="https://jsiek.github.io/home/WhatIsGradualTyping.html">What is Gradual Typing | Jeremy Siek</a></li>
<li><a href="https://www.ituonline.com/tech-definitions/what-is-gradual-typing/">What Is Gradual Typing ? - ITU Online IT Training</a></li>

</ul>
</details>

**Discussion**: The community is largely positive, with many long-time Elixir developers expressing excitement. Some users compare the new system to Dialyzer's success typing approach, while others discuss performance implications of gradual typing and its impact on the untyped vs typed language debate.

**Tags**: `#Elixir`, `#gradual typing`, `#functional programming`, `#programming languages`, `#type systems`

---

<a id="item-2"></a>
## [Bluetooth Speaker Hacked to Inject Keystrokes via USB](https://blog.nns.ee/2026/06/03/katana-badusb/) ⭐️ 9.0/10

A researcher demonstrated a novel attack that wirelessly reflashes the firmware of a Creative Sound Blaster Katana V2X soundbar via Bluetooth, turning it into a USB keyboard to inject keystrokes into the connected PC. This attack bypasses traditional security measures because the soundbar is a trusted USB device, and the reflash requires no authentication or user interaction, making it a stealthy vector for keystroke injection attacks. The soundbar's firmware update process over Bluetooth lacks effective authentication, allowing arbitrary firmware to be written. The researcher added a USB HID keyboard descriptor to the firmware, enabling the soundbar to emulate a keyboard.

hackernews · xx_ns · Jun 3, 10:53 · [Discussion](https://news.ycombinator.com/item?id=48382310)

**Background**: Keystroke injection attacks, like those using USB Rubber Ducky devices, exploit the trust that operating systems place in Human Interface Devices (HID). BadUSB attacks involve reprogramming a USB device's firmware to act as a keyboard. This research extends the concept to peripherals that can be reprogrammed wirelessly.

<details><summary>References</summary>
<ul>
<li><a href="https://www.opswat.com/blog/the-danger-of-a-usb-device-and-keystroke-injection-attack">The Danger of a USB Device and Keystroke Injection Attack</a></li>
<li><a href="https://en.wikipedia.org/wiki/BadUSB_attack">BadUSB attack</a></li>

</ul>
</details>

**Discussion**: Commenters criticized Creative for dismissing the vulnerability as not a cybersecurity risk, and noted the potential for worm propagation in supply chains. Some pointed out that the attack requires physical proximity via Bluetooth, but others argued that the lack of authentication is a serious flaw.

**Tags**: `#security`, `#firmware`, `#bluetooth`, `#badusb`, `#hardware hacking`

---

<a id="item-3"></a>
## [HTTP/2 Bomb DoS Attack Crashes Major Web Servers](https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb) ⭐️ 9.0/10

Researchers disclosed a new remote denial-of-service attack called HTTP/2 Bomb that exploits HPACK compression and slow connection holding to crash popular web servers like NGINX, Apache, IIS, Envoy, and Pingora with minimal bandwidth. This attack can take down major web servers within seconds using a single machine and a 100 Mbps connection, posing a serious threat to internet infrastructure. It highlights the fragility of HTTP/2 implementations and the need for urgent patches. A 100 Mbps home network can render some servers unusable in seconds; Apache httpd and Envoy can hold 32 GB of memory per client in about 20 seconds. NGINX fixed in 1.29.8+, Apache in mod_http2 v2.0.41, while IIS, Envoy, and Pingora have no patches yet.

telegram · zaihuapd · Jun 3, 15:00

**Background**: HTTP/2 uses HPACK compression to reduce header overhead, but it can be abused to amplify small inputs into large memory allocations. Slowloris is a classic attack that keeps many connections open with partial requests to exhaust server resources. The HTTP/2 Bomb combines both techniques: a single byte on the wire triggers a large header allocation, while slow sending keeps the connection alive, causing memory exhaustion.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/codex-discovered-a-hidden-http2-bomb">Codex Discovered a Hidden HTTP / 2 Bomb - Calif</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/new-http-2-bomb-dos-attack-crashes-web-servers-in-under-a-minute/">New ' HTTP / 2 Bomb ' DoS attack crashes web servers in under a minute</a></li>
<li><a href="https://blog.cloudflare.com/hpack-the-silent-killer-feature-of-http-2/">HPACK: the silent killer (feature) of HTTP/2</a></li>

</ul>
</details>

**Tags**: `#security`, `#HTTP/2`, `#DoS`, `#web servers`, `#vulnerability`

---

<a id="item-4"></a>
## [Google Releases Gemma 4 12B, an Encoder-Free Multimodal Model](https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/) ⭐️ 8.0/10

Google DeepMind released Gemma 4 12B on June 3, 2026, an open-weights multimodal model that replaces traditional vision encoders with a lightweight embedding module, enabling direct integration of visual and audio inputs into the language model. This encoder-free architecture reduces latency and memory usage, allowing the model to run on consumer laptops with 16GB of VRAM while approaching the performance of larger 26B models. It democratizes access to advanced multimodal AI for developers and researchers. The model uses a 35M-parameter embedding layer (single matrix multiplication, positional embedding, and normalizations) instead of a dedicated vision encoder like SigLIP. It supports text, image, and audio inputs, and is available in pre-trained and instruction-tuned variants on Hugging Face.

hackernews · rvz · Jun 3, 16:04 · [Discussion](https://news.ycombinator.com/item?id=48385906)

**Background**: Traditional multimodal models use separate encoders (e.g., SigLIP for vision) to convert non-text inputs into representations for the language model, which adds latency and memory overhead. Gemma 4 12B's encoder-free design processes all modalities directly in the language model, simplifying the architecture and improving efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/technology/developers-tools/introducing-gemma-4-12b/">Introducing Gemma 4 12 B</a></li>
<li><a href="https://huggingface.co/google/gemma-4-12B">google/ gemma - 4 - 12 B · Hugging Face</a></li>
<li><a href="https://techstartups.com/2026/06/03/google-deepmind-launches-gemma-4-12b-bringing-frontier-ai-model-to-everyday-laptops/">Google launches Gemma 4 12B, bringing frontier AI model to ...</a></li>

</ul>
</details>

**Discussion**: Community comments show mixed reactions: some users report decent performance on coding benchmarks despite minor syntax errors, while others question the robustness of the 35M embedding layer and note poor image processing quality. There is also debate about Google's strategic motivation for releasing open models.

**Tags**: `#multimodal`, `#encoder-free`, `#Gemma`, `#Google`, `#AI`

---

<a id="item-5"></a>
## [Ted Chiang: AI Is Not Conscious](https://www.theatlantic.com/philosophy/2026/06/no-artificial-intelligence-is-not-conscious/687378/) ⭐️ 8.0/10

Ted Chiang published an essay in The Atlantic arguing that large language models (LLMs) are not conscious, emphasizing the distinction between human-like behavior and subjective experience. This essay reignites the debate on AI consciousness, influencing public discourse and AI ethics, especially as LLMs become more integrated into society. Chiang argues that LLMs are next-token predictors without subjective experience, and that true consciousness would require a body and sense organs.

hackernews · lordleft · Jun 3, 17:51 · [Discussion](https://news.ycombinator.com/item?id=48387270)

**Background**: Large language models (LLMs) like GPT-4 generate text by predicting the next word based on patterns in training data. They can produce human-like responses but lack understanding or consciousness. The question of whether AI can be conscious has been debated since the advent of AI.

**Discussion**: Commenters are divided: some agree that LLMs lack consciousness, while others argue that if an AI behaves as if conscious, it should be treated as such. A few highlight the importance of AI alignment and ethics regardless of consciousness.

**Tags**: `#AI consciousness`, `#philosophy`, `#LLMs`, `#ethics`, `#Ted Chiang`

---

<a id="item-6"></a>
## [DaVinci Resolve 21 Adds Photo Management and Motion Graphics](https://www.blackmagicdesign.com/products/davinciresolve/whatsnew) ⭐️ 8.0/10

Blackmagic Design released DaVinci Resolve 21, introducing a dedicated Photo page for still image editing and management, along with enhanced motion graphics tools and AI-powered features like IntelliSearch and de-aging. This update positions DaVinci Resolve as a direct competitor to Adobe Lightroom and After Effects, potentially disrupting established workflows for photographers and motion designers. The addition of AI tools also improves efficiency for video editors. The Photo page includes advanced color tools from the video side, an effects library with Resolve FX and Fusion FX, and IntelliSearch for content-based image search. The motion graphics enhancements leverage the Fusion page's node-based workflow.

hackernews · pentagrama · Jun 3, 14:18 · [Discussion](https://news.ycombinator.com/item?id=48384482)

**Background**: DaVinci Resolve is a professional video editing, color grading, visual effects, and audio post-production software. It has traditionally focused on video, but version 21 expands into photo management and motion graphics, challenging specialized tools like Lightroom and After Effects.

<details><summary>References</summary>
<ul>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/whatsnew">DaVinci Resolve – What’s New | Blackmagic Design</a></li>
<li><a href="https://documents.blackmagicdesign.com/SupportNotes/DaVinci_Resolve_21_New_Features_Guide.pdf?_v=1776322810000">DaVinci Resolve 21 New Features Guide</a></li>
<li><a href="https://www.blackmagicdesign.com/products/davinciresolve/fusion">DaVinci Resolve – Fusion | Blackmagic Design</a></li>

</ul>
</details>

**Discussion**: Community comments are largely positive, with users praising the photo management and motion graphics additions as significant even without AI features. Some express fatigue with the AI marketing hype, but acknowledge the practical benefits of the new AI tools for editing workflows.

**Tags**: `#video editing`, `#photo management`, `#motion graphics`, `#AI`, `#professional tools`

---

<a id="item-7"></a>
## [Uber Caps AI Token Spending at $1,500/Month Per Tool](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 8.0/10

Uber has capped employee spending on AI coding tools like Claude Code and Cursor at $1,500 per month per tool, after blowing its 2026 AI budget in just four months. The policy applies only to agentic coding software and was instituted in recent months. This marks one of the first major real-world constraints on enterprise AI tool usage, highlighting the unsustainable cost dynamics of token-burning coding agents. It signals that even well-funded companies must rein in AI spending, potentially influencing industry-wide adoption and pricing strategies. The $1,500 cap applies per AI coding tool, meaning an engineer using both Cursor and Claude Code could spend up to $3,000 per month. At a median software engineer compensation of $330,000 per year, the cap represents about 11% of total compensation per engineer.

rss · Simon Willison · Jun 3, 12:01 · [Discussion](https://news.ycombinator.com/item?id=48383056)

**Background**: AI coding agents like Claude Code and Cursor use large language models to autonomously write and edit code, consuming tokens (units of text processed) that incur costs based on model size and usage. Uber's 2026 AI budget was set in 2025 before the explosive popularity of such tools, leading to rapid overspending. Individual subscribers often benefit from subsidized pricing, but enterprises pay full API rates.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>

</ul>
</details>

**Discussion**: Commenters debated whether AI coding tools are a fad or a lasting shift, with some arguing that smaller, cheaper models suffice for most tasks and that large models still produce messy code requiring heavy review. Others noted the rapid adoption and high per-seat spending as evidence of real value. Some questioned whether AI providers will maintain subsidized pricing for individuals given competition from Chinese models like DeepSeek.

**Tags**: `#AI`, `#cost management`, `#coding agents`, `#Uber`, `#LLM economics`

---

<a id="item-8"></a>
## [Let's Encrypt Plans Post-Quantum Certificate Transition](https://letsencrypt.org/2026/06/03/pq-certs) ⭐️ 8.0/10

Let's Encrypt announced plans to transition to post-quantum certificates using Merkle Tree Certificates (MTCs) to protect against future quantum computer attacks. As a major certificate authority, Let's Encrypt's migration will significantly impact the Web PKI ecosystem, pushing the industry toward quantum-safe cryptography and protecting against 'harvest now, decrypt later' threats. MTCs are smaller than current X.509 certificates in common cases, as they combine a single signature, public key, and inclusion proof. The transition also makes transparency a property of issuance itself, simplifying Certificate Transparency.

hackernews · SGran · Jun 3, 15:06 · [Discussion](https://news.ycombinator.com/item?id=48385114)

**Background**: Post-quantum cryptography (PQC) aims to develop algorithms secure against quantum computers, which could break current public-key systems like RSA and ECDSA using Shor's algorithm. Certificate Transparency (CT) is a standard that logs all issued certificates to detect misissuance, but current CT has complexities like inclusion proofs. Let's Encrypt is a free, automated CA that issues a large portion of web certificates.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Post-quantum_cryptography">Post-quantum cryptography</a></li>
<li><a href="https://en.wikipedia.org/wiki/Certificate_Transparency">Certificate Transparency</a></li>

</ul>
</details>

**Discussion**: Commenters raised concerns about current Certificate Transparency being broken and the challenges of validating inclusion proofs. Some noted the practical difficulty of migrating from established algorithms like ed25519, while others praised MTCs for reducing handshake size and simplifying transparency.

**Tags**: `#post-quantum cryptography`, `#Let's Encrypt`, `#TLS/SSL`, `#certificate transparency`, `#infrastructure`

---

<a id="item-9"></a>
## [Espressif ESP32-S31: RISC-V with SIMD and BitScrambler](https://www.espressif.com/en/products/socs/esp32-s31) ⭐️ 8.0/10

Espressif has announced the ESP32-S31, a dual-core 32-bit RISC-V microcontroller running at up to 320 MHz, featuring SIMD instructions and a BitScrambler peripheral for flexible data transformation. The adoption of RISC-V cores with SIMD enables modern toolchains like Rust to be used seamlessly, lowering the barrier for embedded development and expanding the ecosystem for high-performance IoT applications. The ESP32-S31 includes 60 GPIOs, supports Wi-Fi 6 and Gigabit Ethernet, and its BitScrambler peripheral can transform data during DMA transfers, similar to the Raspberry Pi Pico's PIO.

hackernews · volemo · Jun 3, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48385965)

**Background**: The ESP32 family from Espressif has traditionally used Tensilica Xtensa cores. The shift to RISC-V represents a move toward an open-standard ISA, which simplifies toolchain support and enables broader community contributions. SIMD instructions allow parallel processing of data, while the BitScrambler offloads bit-level manipulation from the CPU.

<details><summary>References</summary>
<ul>
<li><a href="https://www.espressif.com/en/products/socs/esp32-s31">ESP32-S31 Dual-Core RISC-V + Multi-Protocol SoC</a></li>
<li><a href="https://docs.espressif.com/projects/esp-idf/en/stable/esp32p4/api-reference/peripherals/bitscrambler.html">BitScrambler Driver - ESP32-P4 - — ESP-IDF Programming Guide...</a></li>
<li><a href="https://hackaday.com/2026/04/08/espressifs-new-esp32-s31-dual-core-risc-v-with-wifi-6-and-gbit-ethernet/">Espressif’s New ESP32-S31: Dual-Core RISC-V With ... - Hackaday</a></li>

</ul>
</details>

**Discussion**: The community is excited about the RISC-V shift, noting that it simplifies Rust development with a simple target triple. Some users express confusion over the naming, as the ESP32 brand now covers many different architectures. The BitScrambler is compared favorably to the Raspberry Pi Pico's PIO.

**Tags**: `#ESP32`, `#RISC-V`, `#embedded systems`, `#Rust`, `#hardware`

---

<a id="item-10"></a>
## [Mathematicians Warn About AI's Rapid Progress](https://www.science.org/content/article/mathematicians-issue-warning-ai-rapidly-gains-ground) ⭐️ 8.0/10

A group of mathematicians has issued a warning about AI's rapid gains in mathematics, highlighting risks to proof verification and attribution. This warning underscores the potential disruption of core mathematical practices, sparking debate on the future role of human reasoning in the field. The mathematicians argue that AI's ability to generate and verify proofs could undermine human oversight and proper attribution, though some see potential for human-machine collaboration.

hackernews · pseudolus · Jun 3, 10:05 · [Discussion](https://news.ycombinator.com/item?id=48382052)

**Background**: Mathematics has traditionally relied on human proof verification and attribution. Recent advances in large language models (LLMs) have enabled AI to assist in generating and checking proofs, raising concerns about the long-term impact on the discipline.

**Discussion**: Community comments express mixed views: some highlight AI's 'long tail of stupidity' and draw parallels to earlier disruptions in art and chess, while others worry about a future where human mathematicians become irrelevant.

**Tags**: `#AI`, `#mathematics`, `#research`, `#LLMs`, `#disruption`

---

<a id="item-11"></a>
## [Microsoft Unveils MAI-Thinking-1 and MAI-Code-1-Flash](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

Microsoft announced two new LLMs: MAI-Thinking-1, a 1-trillion-parameter reasoning model with 35 billion active parameters, and MAI-Code-1-Flash, a 137-billion-parameter code model with 5 billion active parameters, which is rolling out to GitHub Copilot users in VS Code. These models demonstrate Microsoft's push for efficient, high-performance AI using Mixture-of-Experts (MoE) architecture, with MAI-Thinking-1 claiming to be preferred over Sonnet 4.6 in blind evaluations. The deployment of MAI-Code-1-Flash in GitHub Copilot could significantly impact developer productivity and code generation costs. Both models are built on MoE architecture, enabling large total parameters with low active parameters for efficiency. Microsoft claims they were trained on clean, commercially licensed data without distillation from third-party models, though the technical paper reveals the training data includes a proprietary web crawl and Common Crawl, similar to other major LLMs.

rss · Simon Willison · Jun 2, 22:21

**Background**: Mixture-of-Experts (MoE) is a machine learning technique where multiple specialized sub-networks (experts) are activated per input, allowing models to scale parameters without proportional compute cost. MAI-Thinking-1 is a reasoning model designed for complex problem-solving, while MAI-Code-1-Flash is optimized for code generation tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI - Thinking - 1 | Microsoft AI</a></li>
<li><a href="https://microsoft.ai/news/introducingmai-code-1-flash/">Introducing MAI-Code-1-Flash | Microsoft AI</a></li>
<li><a href="https://github.blog/changelog/2026-06-02-mai-code-1-flash-is-now-available-for-github-copilot/">MAI-Code-1-Flash is now available for GitHub Copilot</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Microsoft`, `#AI`, `#code generation`, `#reasoning`

---

<a id="item-12"></a>
## [SpaceX Plans $75B IPO at $135/Share, Largest Ever](https://www.reuters.com/business/media-telecom/spacex-plans-raise-75-billion-ipo-135-per-share-source-says-2026-06-03/) ⭐️ 8.0/10

SpaceX plans to raise $75 billion in an IPO at a fixed price of $135 per share, issuing 555.6 million shares, with trading expected on Nasdaq under ticker SPCX starting June 12, 2026. This would be the largest IPO in history, potentially triggering a wave of mega-IPOs from AI companies like OpenAI and Anthropic, and providing SpaceX with capital to expand AI computing and Starlink. The fixed-price IPO is rare, as pricing is locked before the roadshow; details may still change. SpaceX reported $18.7 billion in revenue last year but a net loss of $4.9 billion, with only Starlink profitable.

telegram · zaihuapd · Jun 3, 09:01

**Background**: An IPO (Initial Public Offering) is when a private company sells shares to the public for the first time. A fixed-price IPO sets the share price in advance, unlike a book-building process. Starlink is a satellite internet constellation operated by SpaceX, providing broadband to remote areas. The roadshow is a marketing event where company executives present to potential investors to generate interest.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starlink">Starlink - Wikipedia</a></li>
<li><a href="https://www.zhihu.com/question/19602940">IPO 之前的「路演」具体是怎样的过程？ - 知乎</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#IPO`, `#finance`, `#AI`, `#Starlink`

---

<a id="item-13"></a>
## [Google lets websites opt out of AI search results](https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/) ⭐️ 8.0/10

Google is adding a new toggle in Search Console that lets website owners opt out of appearing in AI Overviews and AI Mode, without affecting their regular search rankings or Discover traffic. This gives publishers more control over how their content is used by generative AI in search, addressing concerns about traffic declines and lack of attribution. It sets a precedent for how search engines balance AI features with publisher rights. The opt-out is currently being tested with UK websites and will roll out globally later. Google also introduced generative AI search statistics in Search Console, showing impressions, page performance, and geographic data.

telegram · zaihuapd · Jun 3, 12:00

**Background**: AI Overviews are AI-generated summaries that appear at the top of some Google search results, providing quick answers without requiring users to click through to websites. Many publishers have reported significant traffic drops since their introduction, leading to calls for more control. The new opt-out follows a ruling by UK regulators and growing pressure from the web publishing industry.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5google.com/2026/06/02/google-ai-mode-overviews-opt-out/">Google will let sites opt-out of AI Mode and Overviews in Search</a></li>
<li><a href="https://www.androidheadlines.com/2026/06/google-ai-search-opt-out-publisher-control.html">Google Launches Opt Out for AI Search Overviews and AI Mode</a></li>
<li><a href="https://mashable.com/tech/google-will-allow-websites-to-opt-out-of-ai-overviews">Google will allow websites to opt out of AI overviews</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI`, `#SEO`, `#Search Console`, `#Web Publishing`

---

<a id="item-14"></a>
## [Developer Shares Anti-NMDA Receptor Encephalitis Diagnosis](https://burntsushi.net/encephalitis/) ⭐️ 7.0/10

Software developer Andrew Gallant (burntsushi) publicly shared his diagnosis of anti-NMDA receptor encephalitis, a rare autoimmune brain disease, detailing his terrifying symptoms and the challenges of getting correctly diagnosed. This personal account highlights the frequent misdiagnosis of rare autoimmune encephalitis as psychiatric conditions, underscoring the need for greater awareness and better diagnostic tools. It also emphasizes the critical role of biomedical research in discovering treatable causes of severe neurological symptoms. Anti-NMDA receptor encephalitis was first described in 2007 and is caused by antibodies attacking NMDA receptors in the brain. About 80% of cases are female, and roughly half are associated with tumors, most commonly ovarian teratomas.

hackernews · Tomte · Jun 3, 14:10 · [Discussion](https://news.ycombinator.com/item?id=48384355)

**Background**: Anti-NMDA receptor encephalitis is a rare autoimmune disorder where the body's immune system produces antibodies that attack NMDA receptors in the brain, leading to inflammation. Early symptoms often mimic psychiatric conditions like schizophrenia, leading to frequent misdiagnosis. Treatment involves immunosuppression and tumor removal if present, and early intervention significantly improves outcomes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anti-NMDA_receptor_encephalitis">Anti-NMDA receptor encephalitis</a></li>
<li><a href="https://www.ncbi.nlm.nih.gov/books/NBK578203/">Autoimmune Encephalitis - StatPearls - NCBI Bookshelf</a></li>
<li><a href="https://www.med.upenn.edu/autoimmuneneurology/nmdar-encephalitis.html">Anti-NMDAR Encephalitis | Center for Autoimmune Neurology ...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed deep sympathy and shared similar experiences with misdiagnosis of autoimmune conditions. A neurologist noted that the disease is very rare and expected to be misdiagnosed as psychiatric, but praised the excellent neurologic center that treated the author. Others highlighted the importance of continued biomedical research to discover reversible treatments for such disorders.

**Tags**: `#autoimmune disease`, `#medical misdiagnosis`, `#neuroscience`, `#personal story`

---

<a id="item-15"></a>
## [Deep Dive into Original PlayStation Architecture](https://www.copetti.org/writings/consoles/playstation/) ⭐️ 7.0/10

Rodrigo Copetti published a detailed architectural analysis of the original PlayStation, covering its MIPS R3000A CPU, GTE, GPU, and SPU audio system. This analysis provides invaluable insight for retro computing enthusiasts and emulator developers, helping them understand the hardware quirks that defined PlayStation games. The article explains the GTE's role in 3D geometry and lighting, the GPU's tile-based rendering, and the SPU's 24-channel ADPCM audio with 512 KB dedicated RAM.

hackernews · gregsadetsky · Jun 3, 10:24 · [Discussion](https://news.ycombinator.com/item?id=48382142)

**Background**: The original PlayStation, released in 1994, used a MIPS R3000A CPU at 33.8688 MHz and a custom GPU for 3D graphics. Its architecture was unique for its time, with a separate Geometry Transformation Engine (GTE) for vector math and a Sound Processing Unit (SPU) for audio.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PlayStation_technical_specifications">PlayStation technical specifications - Wikipedia</a></li>
<li><a href="https://www.copetti.org/writings/consoles/playstation/">PlayStation Architecture | A Practical Analysis</a></li>
<li><a href="https://psx-spx.consoledev.net/soundprocessingunitspu/">Sound Processing Unit (SPU) - PlayStation Specifications ...</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article's depth and website design, while noting it was a repost from 2019. One developer shared a memory mapping trick used in the Metal Gear Solid PC port, and another asked for PS1 web emulator recommendations.

**Tags**: `#PlayStation`, `#console architecture`, `#retro computing`, `#hardware`

---

<a id="item-16"></a>
## [When Every Byte Matters: AoS vs SoA](https://fzakaria.com/2026/06/01/every-byte-matters) ⭐️ 7.0/10

An article argues that the mantra 'every byte matters' is often misleading, using the array-of-structs (AoS) vs struct-of-arrays (SoA) memory layout choice as a case study to show when byte-level optimization is worthwhile. This discussion helps developers understand when to invest effort in memory optimization, preventing wasted time on micro-optimizations that don't improve performance, while highlighting scenarios where layout changes can yield significant gains. The article points out that reading a single byte is trivial, but reading 1 million bytes (e.g., iterating over 1 million monsters) makes optimization critical. It also notes that JVM object headers (currently 12 bytes, soon 8 bytes) add overhead, and Project Valhalla aims to eliminate headers in some cases.

hackernews · ingve · Jun 3, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48382382)

**Background**: Array-of-structs (AoS) stores each object's fields contiguously, while struct-of-arrays (SoA) stores each field in a separate array. SoA can improve cache locality and SIMD vectorization when iterating over a single field of many objects. The JVM adds per-object overhead (header + padding), making memory layout decisions more impactful in Java than in languages with manual memory control.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AoS_and_SoA">AoS and SoA - Wikipedia</a></li>
<li><a href="https://www.reddit.com/r/bigquery/comments/1fbzy55/array_of_structs_vs_struct_of_arrays/">r/bigquery on Reddit: ARRAY of STRUCTS vs STRUCT of ARRAYS</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree that 'every byte matters' is context-dependent. Some highlight that JVM overhead makes optimization harder but note upcoming improvements like reduced object headers and Project Valhalla. Others share historical perspectives from constrained environments where every bit mattered.

**Tags**: `#memory optimization`, `#data structures`, `#JVM`, `#performance`, `#systems programming`

---

<a id="item-17"></a>
## [Massive Proxy Service Blocking by GFW on March 4](https://t.me/zaihuapd/41740) ⭐️ 7.0/10

On March 4, the Great Firewall of China (GFW) began blocking IP ranges of popular proxy service providers, severely impacting Vless and AnyTLS protocols, while non-TLS encryption appears less affected. This widespread blocking significantly disrupts internet freedom for users relying on proxy services to access blocked content, and highlights the GFW's evolving capability to target newer encryption protocols like Vless and AnyTLS. The blocking specifically targeted Vless protocol deeply, and the newer AnyTLS protocol also appears heavily blocked, though no statistical data is provided. Non-TLS encryption types seem less impacted, but the full extent remains unclear.

telegram · zaihuapd · Jun 3, 11:15

**Background**: The Great Firewall of China (GFW) is a system of censorship and surveillance that blocks access to foreign websites and slows cross-border traffic. Vless is a stateless lightweight transport protocol used in Xray for proxy services, while AnyTLS is a newer protocol designed to mitigate TLS-in-TLS fingerprinting. The GFW has historically blocked protocols like Shadowsocks and VMess, and this event shows its adaptation to newer encryption methods.

<details><summary>References</summary>
<ul>
<li><a href="https://xtls.github.io/en/development/protocols/vless.html">VLESS Protocol | Project X</a></li>
<li><a href="https://github.com/anytls/anytls-go/blob/main/docs/protocol.md">anytls-go/docs/protocol.md at main - GitHub</a></li>
<li><a href="https://en.wikipedia.org/wiki/Great_Firewall">Great Firewall - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#GFW`, `#proxy`, `#encryption`, `#censorship`, `#Vless`

---

<a id="item-18"></a>
## [Qianwen Opens Platform to Third-Party Agents and Skills](https://www.stcn.com/article/detail/3941333.html) ⭐️ 7.0/10

Qianwen APP announced it will fully open its platform to third-party agents and skills, allowing any enterprise to operate its own branded agent on Qianwen. Early enterprise testers include Luckin Coffee, KFC, Mixue Bingcheng, and China Eastern Airlines. This move positions Qianwen as a potential AI super-app by enabling a rich ecosystem of specialized agents and skills, similar to WeChat's mini-program model. It could accelerate enterprise adoption of AI agents for customer service, ordering, and other tasks. The platform supports both Skill (reusable tool templates) and branded agents that enterprises can customize. The first batch of enterprises is currently testing agent services and will go live gradually.

telegram · zaihuapd · Jun 3, 12:15

**Background**: Qianwen is Alibaba's large language model and AI assistant platform. An Agent is an AI system that can autonomously perform tasks, while a Skill is a reusable tool template that equips an agent with specific capabilities. Opening the platform to third parties allows enterprises to create their own branded AI agents within Qianwen, similar to how WeChat hosts mini-programs.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260603A07TGS00">向第三方Agent全面开放，千问正在打造AI时代真正入口</a></li>
<li><a href="https://www.ithome.com/0/959/289.htm">阿里千问向第三方 Agent、Skill 全面开放，肯德基、瑞幸、蜜雪冰城、...</a></li>
<li><a href="https://help.aliyun.com/zh/model-studio/web-search-agent-guide">千问联网检索Agent-大模型服务平台百炼 (Model Studio)-阿里云帮助中...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#platform`, `#agents`, `#enterprise`

---

<a id="item-19"></a>
## [US Teachers Union Calls for AI and Screen Limits in Elementary Schools](https://www.aft.org/press-release/devices-down-eyes-hands-weingarten-calls-screen-bans-ai-limits-active-learning-major) ⭐️ 7.0/10

The American Federation of Teachers (AFT) President Randi Weingarten proposed banning screens in kindergarten through second grade and halting student-facing AI tools in elementary schools, along with prohibiting social chatbots for children under 16. As a major U.S. teachers union representing 1.6 million members, the AFT's stance could influence education policy and technology adoption in schools, potentially reshaping how AI and digital tools are integrated into early childhood education. The plan, called 'Devices Down, Hands On,' also calls for a 'tech tax' on technology companies to fund public education and the creation of an independent research institute free from industry funding to study digital technology's long-term effects on children.

telegram · zaihuapd · Jun 3, 13:30

**Background**: The American Federation of Teachers (AFT) is the second-largest teachers union in the U.S., founded in 1916 and affiliated with the AFL-CIO. Concerns have grown over children's use of AI chatbots for friendship and therapy, with studies showing risks such as inadequate responses to mental health crises.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/American_Federation_of_Teachers">American Federation of Teachers</a></li>

</ul>
</details>

**Tags**: `#education`, `#AI policy`, `#screen time`, `#children`, `#teachers union`

---