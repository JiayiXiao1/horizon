---
layout: default
title: "Horizon Summary: 2026-07-01 (EN)"
date: 2026-07-01
lang: en
---

> From 37 items, 16 important content pieces were selected

---

1. [vLLM v0.24.0 Adds MiniMax-M3 and DeepSeek-V4 Optimizations](#item-1) ⭐️ 9.0/10
2. [US Lifts Export Controls on Anthropic's Claude Fable 5 and Mythos 5](#item-2) ⭐️ 9.0/10
3. [Anthropic Releases Claude Sonnet 5 with Strong Agentic Abilities](#item-3) ⭐️ 9.0/10
4. [Claude Code Steganographically Marks Requests](#item-4) ⭐️ 8.0/10
5. [Anthropic Launches Claude Science for Scientific Data Analysis](#item-5) ⭐️ 8.0/10
6. [Kubernetes Ported to the Browser via WebAssembly](#item-6) ⭐️ 8.0/10
7. [shot-scraper video: AI agents record demo videos](#item-7) ⭐️ 8.0/10
8. [Ornith-1.0: Open-Source Self-Scaffolding LLMs for Agentic Coding](#item-8) ⭐️ 8.0/10
9. [Huawei Open-Sources Pangu 2.0 with 505B and 92B Variants](#item-9) ⭐️ 8.0/10
10. [Anthropic Releases Claude Sonnet 4.6 with Major Upgrades](#item-10) ⭐️ 8.0/10
11. [Tesla Supervised FSD Launches in China](#item-11) ⭐️ 8.0/10
12. [Google DeepMind Releases Nano Banana 2 Lite](#item-12) ⭐️ 7.0/10
13. [Anthropic Regains US Approval to Deploy Mythos 5 to Critical Infrastructure](#item-13) ⭐️ 7.0/10
14. [Memory Chip Price Hike Triggers Smartphone Production Cuts](#item-14) ⭐️ 7.0/10
15. [UK Proposes Easing Apple and Google App Store Payment Rules](#item-15) ⭐️ 7.0/10
16. [Claude Desktop Linux Beta Launches for Ubuntu and Debian](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.24.0 Adds MiniMax-M3 and DeepSeek-V4 Optimizations](https://github.com/vllm-project/vllm/releases/tag/v0.24.0) ⭐️ 9.0/10

vLLM v0.24.0, released with 571 commits from 256 contributors, adds support for the MiniMax-M3 multimodal model and delivers major optimizations for DeepSeek-V4, including a FlashInfer sparse index cache and prefill chunk-planning improvements. This release significantly expands vLLM's model support and inference performance, benefiting users of cutting-edge open-weight models like MiniMax-M3 and DeepSeek-V4. The optimizations reduce latency and improve throughput, making large-scale LLM serving more efficient. Key technical highlights include the integration of DeepEP v2 for expert parallelism, a new streaming parser engine for tool-call/reasoning, and the addition of DiffusionGemma for diffusion LLMs. The Rust frontend now supports API-key authentication and CORS, and the device selection mechanism has changed to use a 'device_ids' argument instead of setting CUDA_VISIBLE_DEVICES.

github · khluu · Jun 29, 19:41

**Background**: vLLM is a high-performance open-source library for LLM inference and serving, widely used for its efficient memory management and fast decoding. MiniMax-M3 is a multimodal vision-language model with a 1M-token context window, while DeepSeek-V4 is a powerful open-weight model featuring architectural innovations like Manifold-Constrained Hyper-Connections. FlashInfer is a kernel library that provides efficient attention implementations for LLM serving.

<details><summary>References</summary>
<ul>
<li><a href="https://build.nvidia.com/minimaxai/minimax-m3/modelcard">minimax-m3 Model by Minimaxai | NVIDIA NIM</a></li>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Pro">deepseek-ai/DeepSeek-V4-Pro · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#DeepSeek-V4`, `#MiniMax-M3`, `#open source`

---

<a id="item-2"></a>
## [US Lifts Export Controls on Anthropic's Claude Fable 5 and Mythos 5](https://twitter.com/AnthropicAI/status/2072106151890809341) ⭐️ 9.0/10

The US Department of Commerce has lifted export controls on Anthropic's Claude Fable 5 and Mythos 5, allowing these advanced AI models to be exported internationally. The decision follows Anthropic's agreement to proactively detect and address security risks associated with the models. This policy change marks a significant shift in AI regulation, potentially impacting US-China competition and the global AI market. It also raises concerns about business reliance on frontier models and the effectiveness of export controls. Claude Fable 5 is a Mythos-class model made safe for general use, while Mythos 5 is a cybersecurity-focused model currently limited to vetted partners. The models became available on June 9, 2026, on multiple platforms including AWS, Google Cloud, and Microsoft Foundry.

hackernews · Pragmata · Jun 30, 23:55 · [Discussion](https://news.ycombinator.com/item?id=48740771)

**Background**: Export controls on advanced AI models were imposed to prevent sensitive technology from falling into the hands of adversaries, particularly China. Anthropic's Claude models are among the most capable AI systems, and their release has been subject to safety and misuse concerns. The lifting of controls suggests a reassessment of the balance between security and commercial interests.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude Platform Docs</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Fable_5">Claude Fable 5</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism and concern: some argue that the damage is already done and that businesses cannot rely on US frontier models, while others note that Chinese models have proven competitive without massive capital expenditure. There is also criticism that the administration's actions are performative and that security measures were already in place.

**Tags**: `#AI regulation`, `#export controls`, `#Anthropic`, `#US-China competition`, `#frontier models`

---

<a id="item-3"></a>
## [Anthropic Releases Claude Sonnet 5 with Strong Agentic Abilities](https://t.me/zaihuapd/42280) ⭐️ 9.0/10

Anthropic released Claude Sonnet 5 on June 30, 2026, claiming it is the most agentic Sonnet model yet, capable of planning, using tools like browsers and terminals, and running autonomously. It is available immediately across all plans, with Free and Pro users getting it as the default model. Claude Sonnet 5 brings near-Opus-level agentic performance at a lower price point, making advanced AI agent capabilities more accessible to developers and businesses. This release signals a trend toward more autonomous, tool-using AI models that can handle complex tasks independently. Claude Sonnet 5 outperforms Sonnet 4.6 in reasoning, tool use, coding, and knowledge work, and approaches Opus 4.8 performance. Pricing is set at $2 per million input tokens and $10 per million output tokens until August 31, 2026, making it cheaper than Opus 4.8 ($5/$25).

telegram · zaihuapd · Jul 1, 01:12

**Background**: Anthropic's Claude model family includes Haiku (fastest), Sonnet (balanced), and Opus (most capable). Sonnet models are designed for a balance of speed and capability, while Opus targets maximum performance. Agentic AI refers to models that can autonomously plan and execute multi-step tasks using external tools, rather than just generating text responses.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-5">Introducing Claude Sonnet 5 \ Anthropic</a></li>
<li><a href="https://www.mejba.me/blog/claude-sonnet-5-agentic-coding">Claude Sonnet 5 Changes Everything About Agentic Coding</a></li>
<li><a href="https://www.digitalapplied.com/blog/claude-sonnet-5-agentic-coding-near-opus-price-2026">Claude Sonnet 5 : Near-Opus Agentic Coding at Sonnet Price</a></li>

</ul>
</details>

**Discussion**: Community comments express mixed reactions: some users question the value proposition, noting that Opus performs better per cost at higher effort levels, while others appreciate the speed and agentic focus. A user's benchmark shows Sonnet 5 scores well on speed but has weak spots in trivia and combined tool-calling tasks.

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#agent`

---

<a id="item-4"></a>
## [Claude Code Steganographically Marks Requests](https://thereallo.dev/blog/claude-code-prompt-steganography) ⭐️ 8.0/10

Anthropic's Claude Code tool embeds hidden identifiers in outgoing requests using steganography, likely to detect unauthorized use by Chinese firms for model distillation. This practice raises serious concerns about transparency and trust in AI developer tools, as users may be unaware that their requests contain hidden markers that could be used for tracking or enforcement. The steganographic technique was discovered through reverse engineering; the hidden data is embedded in a way that is not visible to users but can be extracted by Anthropic's servers.

hackernews · kirushik · Jun 30, 15:44 · [Discussion](https://news.ycombinator.com/item?id=48734373)

**Background**: Steganography is the practice of concealing a message within another message or physical object. In AI contexts, it can be used to hide data in model inputs or outputs. Claude Code is an agentic coding tool released by Anthropic in 2025 that allows developers to delegate coding tasks via natural language in the terminal.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_(language_model)">Claude (AI) - Wikipedia</a></li>
<li><a href="https://github.com/anthropics/claude-code">GitHub - anthropics/claude-code: Claude Code is an agentic coding tool that lives in your terminal, understands your codebase, and helps you code faster by executing routine tasks, explaining complex code, and handling git workflows - all through natural language commands. · GitHub</a></li>

</ul>
</details>

**Discussion**: Community comments are mixed: some criticize the lack of transparency, while others downplay the severity, arguing the intent is clearly to prevent model distillation by Chinese firms. A few users express distrust toward Anthropic and suggest using open-source alternatives like Codex CLI.

**Tags**: `#steganography`, `#AI ethics`, `#Anthropic`, `#developer tools`, `#privacy`

---

<a id="item-5"></a>
## [Anthropic Launches Claude Science for Scientific Data Analysis](https://claude.com/product/claude-science) ⭐️ 8.0/10

Anthropic has launched Claude Science, a local server-based AI workbench that integrates with databases and high-performance computing (HPC) clusters for scientific data analysis. This tool enables researchers to run AI-powered data analysis locally within secure environments, bridging the gap between advanced AI capabilities and sensitive scientific data that cannot be moved to the cloud. Claude Science runs a local server with a web-based UI, allowing it to connect to institutional clusters and databases while keeping data on-premises. It supports tools like pandas for data manipulation and produces auditable artifacts.

hackernews · lebovic · Jun 30, 17:07 · [Discussion](https://news.ycombinator.com/item?id=48735770)

**Background**: Scientific research often involves sensitive or proprietary data that cannot be processed on cloud AI services due to security or compliance reasons. Traditional data analysis workflows require researchers to manually code and manage computational resources. Claude Science aims to provide an AI assistant that works directly within the researcher's local or institutional computing environment.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-science-ai-workbench">Claude Science, an AI workbench for scientists, is now available</a></li>
<li><a href="https://grokipedia.com/page/Claude_for_Life_Sciences">Claude for Life Sciences</a></li>
<li><a href="https://aithinkerlab.com/run-claude-ai-locally/">Can You Run Claude Locally in 2026? Real Answer + Workarounds</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the tool's architecture (local server + web UI) as a key differentiator for secure environments, with one commenter noting its integration with HPC clusters. Some users found it useful for specific tasks like designing biopesticides, while others questioned its value over existing tools like Claude Code with org-mode.

**Tags**: `#AI`, `#data science`, `#Anthropic`, `#scientific computing`, `#HPC`

---

<a id="item-6"></a>
## [Kubernetes Ported to the Browser via WebAssembly](https://ngrok.com/blog/i-ported-kubernetes-to-the-browser) ⭐️ 8.0/10

ngrok released a demo called 'Wébernetes' that runs a full Kubernetes cluster entirely in the browser using WebAssembly, accessible at webernetes-demo.ngrok.app. This enables interactive Kubernetes learning and testing without any local setup, lowering the barrier for newcomers and providing a safe environment for experimentation. The project is open-source on GitHub under ngrok/webernetes, and the demo runs a single-node cluster using k3s compiled to WebAssembly.

hackernews · peterdemin · Jun 30, 20:48 · [Discussion](https://news.ycombinator.com/item?id=48738985)

**Background**: Kubernetes is a container orchestration platform that typically requires a cluster of machines to run. WebAssembly (Wasm) is a binary instruction format that runs in browsers at near-native speed. Porting Kubernetes to Wasm allows it to run in environments without traditional OS support.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cncf.io/blog/2024/03/12/webassembly-on-kubernetes-from-containers-to-wasm-part-01/">WebAssembly on Kubernetes: from containers to Wasm (part 01) | CNCF</a></li>
<li><a href="https://ngrok.com/blog/ngrok-k8s">Introducing the ngrok Kubernetes Operator | ngrok blog</a></li>
<li><a href="https://github.com/ngrok/ngrok-operator">GitHub - ngrok/ngrok-operator: The official ngrok Kubernetes Operator · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project for its educational value, noting it could replace platforms like Katacoda for conceptual learning. One commenter highlighted the workflow of testing AI-generated code against real Kubernetes behavior as a key insight.

**Tags**: `#Kubernetes`, `#WebAssembly`, `#Browser`, `#Education`, `#DevOps`

---

<a id="item-7"></a>
## [shot-scraper video: AI agents record demo videos](https://simonwillison.net/2026/Jun/30/shot-scraper-video/#atom-everything) ⭐️ 8.0/10

Simon Willison released shot-scraper 1.10 with a new 'shot-scraper video' command that uses Playwright to record WebM videos of web application routines defined in a YAML storyboard file. This tool enables AI coding agents to automatically produce verifiable video demos of their work, addressing a critical need for trust and validation in agent-generated code. The storyboard file specifies server setup, viewport, cursor visibility, wait conditions, JavaScript overrides (e.g., clipboard mocking), and a sequence of scenes with actions like pause, click, and type.

rss · Simon Willison · Jun 30, 16:54

**Background**: shot-scraper is a command-line tool for taking screenshots of web pages using Playwright. The new video command extends this to recording, allowing developers and AI agents to create reproducible demos of web interactions.

<details><summary>References</summary>
<ul>
<li><a href="https://shot-scraper.datasette.io/en/stable/video.html">Recording videos - shot - scraper</a></li>
<li><a href="https://simonwillison.net/2026/Jun/30/shot-scraper-video/">Have your agent record video demos of its work with shot - scraper ...</a></li>
<li><a href="https://www.remio.ai/post/shot-scraper-video-lets-ai-agents-record-demo-videos">Shot - scraper Video Lets AI Agents Record Demo Videos</a></li>

</ul>
</details>

**Tags**: `#developer-tools`, `#automation`, `#testing`, `#playwright`, `#ai-agents`

---

<a id="item-8"></a>
## [Ornith-1.0: Open-Source Self-Scaffolding LLMs for Agentic Coding](https://simonwillison.net/2026/Jun/29/ornith/#atom-everything) ⭐️ 8.0/10

DeepReinforce released Ornith-1.0, a new open-weight LLM family under MIT license, with sizes from 9B to 397B parameters, achieving state-of-the-art coding benchmark performance among open-source models of comparable size. Ornith-1.0's self-scaffolding capability allows it to autonomously plan, write, test, and debug code, advancing agentic coding and reducing human intervention. Its open-source nature under MIT license promotes widespread adoption and further research. The model family includes 9B Dense, 31B Dense, 35B MoE, and 397B MoE variants, built on Gemma 4 and Qwen 3.5 (both Apache 2.0). It supports up to 262k context length and is compatible with vLLM for deployment.

rss · Simon Willison · Jun 29, 16:17

**Background**: Agentic coding refers to AI agents that autonomously plan, write, test, and modify code with minimal human input. Traditional coding assistants require step-by-step guidance, while agentic models like Ornith-1.0 can independently handle complex tasks. Ornith-1.0 learns its own agent scaffolds through reinforcement learning post-training, a novel approach called self-scaffolding.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jun/29/ornith/">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding</a></li>
<li><a href="https://deep-reinforce.com/ornith_1_0.html">Ornith-1.0: Self-Scaffolding LLMs for Agentic Coding | DeepReinforce Blog | Jun. 2026</a></li>
<li><a href="https://www.marktechpost.com/2026/06/25/deepreinforce-releases-ornith-1-0-an-open-source-coding-model-family-that-learns-its-own-rl-scaffolds/">DeepReinforce Releases Ornith-1.0: An Open-Source Coding Model Family That Learns Its Own RL Scaffolds - MarkTechPost</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#open-source`, `#coding`, `#agentic`, `#AI`

---

<a id="item-9"></a>
## [Huawei Open-Sources Pangu 2.0 with 505B and 92B Variants](https://t.me/zaihuapd/42259) ⭐️ 8.0/10

At HDC 2026, Huawei announced the open-source release of the openPangu 2.0 model, including a Pro version with 505 billion total parameters and a Flash version with 92 billion total parameters, supporting a 512K context length. The company plans to gradually release seven components starting June 30. This release marks a major milestone in the open-source AI ecosystem, as Huawei aims to transition Pangu from China's leading model to a world-leading one. The large-scale open-source model, optimized for Ascend chips and HarmonyOS, could accelerate AI adoption and competition globally. The Pro version has 505B total parameters with an undisclosed number of activated parameters, while the Flash version has 92B total and 6B activated parameters. The model is designed to be more affinity with Ascend computing power and adapted to HarmonyOS.

telegram · zaihuapd · Jun 30, 06:01

**Background**: Huawei first released the Pangu large model in 2021, before the global AI boom triggered by ChatGPT. The openPangu 2.0 is built on Huawei's Ascend AI chips and aims to provide an open-source alternative to proprietary models like GPT-4. The model's 512K context window allows processing of very long documents or conversations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kucoin.com/news/flash/huawei-launches-openpangu-2-0-with-50-5b-parameters-and-512k-context">Huawei Launches OpenPangu 2 . 0 with 50.5 Billion... | KuCoin</a></li>
<li><a href="https://news.aibase.com/news/29268">Huawei openPangu 2 . 0 Launches Two Versions: Accelerating the...</a></li>
<li><a href="https://www.aimadetools.com/blog/best-chinese-open-source-ai-models-june-2026/">Best Chinese Open -Source AI Models June 2026: Pangu , DeepSeek...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Open Source`, `#Large Language Model`, `#Huawei`, `#Deep Learning`

---

<a id="item-10"></a>
## [Anthropic Releases Claude Sonnet 4.6 with Major Upgrades](https://t.me/zaihuapd/42277) ⭐️ 8.0/10

Anthropic has released Claude Sonnet 4.6, a full upgrade across coding, computer use, long-context reasoning, and agent planning. The model is now the default for Free and Pro users, with a 1M token context window. This release significantly improves AI's ability to perform complex coding tasks and interact with computer interfaces, making it more useful for developers and knowledge workers. The 1M token context window enables handling of very long documents and complex agent workflows. Claude Sonnet 4.6 shows notable gains on the OSWorld benchmark for computer use tasks, where the model sees a screenshot and decides actions like clicking and typing. The model is available via API and major cloud platforms, with pricing unchanged from the previous version.

telegram · zaihuapd · Jun 30, 17:58

**Background**: Anthropic's Claude models are large language models designed for safe and capable AI assistance. Computer use is a feature that allows the model to directly interact with graphical user interfaces by interpreting screenshots and performing actions, enabling automation of tasks that typically require human mouse and keyboard input. The OSWorld benchmark evaluates AI agents on real-world computer tasks across multiple applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-sonnet-4-6">Introducing Claude Sonnet 4.6</a></li>
<li><a href="https://cobusgreyling.substack.com/p/claude-sonnet-46-and-computer-use">Claude Sonnet 4.6 & Computer Use</a></li>
<li><a href="https://os-world.github.io/">OSWorld : Benchmarking Multimodal Agents for Open-Ended Tasks in...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#Anthropic`, `#Claude`, `#LLM`, `#model release`

---

<a id="item-11"></a>
## [Tesla Supervised FSD Launches in China](https://t.me/zaihuapd/42281) ⭐️ 8.0/10

Tesla announced on social media platform X that its supervised Full Self-Driving (FSD) system is now available in China, marking the official entry of its advanced driver-assistance technology into the Chinese market. This expansion is significant because China is the world's largest automotive market and a key battleground for autonomous driving technology, potentially boosting Tesla's revenue and competitive position against local rivals like BYD and XPeng. The supervised FSD in China is reportedly limited compared to the US version, as Tesla can only use local data for training and faces regulatory restrictions, and it is expected to be priced similarly to the $99/month subscription in the US.

telegram · zaihuapd · Jul 1, 01:22

**Background**: Tesla's FSD is a suite of advanced driver-assistance features that require active driver supervision. The system has been under development for years and is gradually being rolled out in select markets. China has strict regulations on autonomous driving data and requires foreign companies to store and process data locally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tesla.com/fsd">Full Self-Driving ( Supervised ) | Tesla</a></li>
<li><a href="https://www.teslarati.com/tesla-china-expects-fsd-approval-end-of-2024-musk/">Tesla China FSD approval expected by end of 2024: Musk</a></li>
<li><a href="https://www.notebookcheck.net/Tesla-brings-half-baked-FSD-to-full-price-customers-in-China-as-it-can-only-use-local-data-for-training.967429.0.html">Tesla brings half-baked FSD to full-price customers in China as it can...</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#FSD`, `#autonomous driving`, `#China`, `#EV`

---

<a id="item-12"></a>
## [Google DeepMind Releases Nano Banana 2 Lite](https://deepmind.google/models/gemini-image/flash-lite/) ⭐️ 7.0/10

Google DeepMind has released Nano Banana 2 Lite, a distilled version of its Nano Banana 2 image generation model, offering faster inference and improved text rendering, but access is restricted to Google One subscribers. This release makes high-quality image generation more accessible to consumers through faster speeds, but the Google One account requirement may limit adoption, especially for Workspace users. Nano Banana 2 Lite generates images in under 5 seconds, compared to ~30 seconds for the base model, but does not support programmatic aspect ratio control and is not as capable with highly nuanced prompts.

hackernews · minimaxir · Jun 30, 16:48 · [Discussion](https://news.ycombinator.com/item?id=48735444)

**Background**: Model distillation is a technique where a smaller, faster 'student' model is trained to mimic a larger 'teacher' model, reducing computational cost while retaining much of the quality. Google DeepMind's Nano Banana series focuses on efficient image generation for consumer applications.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bentoml.com/blog/a-guide-to-open-source-image-generation-models">The Best Open-Source Image Generation Models in 2026</a></li>
<li><a href="https://blog.segmind.com/distilledstable-diffusion-models/">A Comprehensive Guide to Distilled Stable Diffusion Models</a></li>

</ul>
</details>

**Discussion**: Community comments highlight mixed reactions: some users praise the speed and text rendering improvements, while others criticize the Google One account restriction and express frustration with real estate agents using AI-generated images deceptively. One user also notes the omission of ChatGPT from comparison charts.

**Tags**: `#AI`, `#image generation`, `#Google DeepMind`, `#model release`

---

<a id="item-13"></a>
## [Anthropic Regains US Approval to Deploy Mythos 5 to Critical Infrastructure](https://t.me/zaihuapd/42260) ⭐️ 7.0/10

On June 27, 2026, the U.S. government notified Anthropic that its strongest cybersecurity model, Mythos 5, can be redeployed to organizations operating and defending critical infrastructure, after being suspended since June 12. This approval signals a shift in government policy toward allowing advanced AI models for critical infrastructure defense, potentially setting a precedent for future AI deployment in high-stakes security contexts. Anthropic is rapidly restoring access for these organizations while continuing negotiations with the government to expand Mythos 5's scope and to also approve the Fable 5 model. Mythos 5 is a cybersecurity-focused model designed to find software vulnerabilities.

telegram · zaihuapd · Jun 30, 07:04

**Background**: Claude Mythos is a large language model developed by Anthropic to find vulnerabilities in software. Due to safety and misuse concerns, Anthropic had not publicly released the model. The government suspension and subsequent approval reflect ongoing debates about balancing AI capabilities with security risks.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#Anthropic`, `#government policy`, `#critical infrastructure`

---

<a id="item-14"></a>
## [Memory Chip Price Hike Triggers Smartphone Production Cuts](https://t.me/zaihuapd/42265) ⭐️ 7.0/10

Rising memory chip prices have led major smartphone makers including Xiaomi, OPPO, vivo, and Transsion to cut their 2026 production targets by 15-20%, with a focus on mid-to-low-end and overseas models. This could trigger a smartphone industry downturn, with TrendForce predicting a 7% decline in 2026 production and potential price increases for consumers, affecting the entire supply chain. Xiaomi and OPPO cut orders by over 20%, vivo by nearly 15%, and Transsion also lowered targets. The cuts primarily target cost-sensitive segments, suggesting manufacturers are absorbing some cost pressure.

telegram · zaihuapd · Jun 30, 08:44

**Background**: Memory chips, including DRAM and NAND flash, are essential components in smartphones. Their prices have been rising due to supply constraints and increased demand from AI and data centers, squeezing phone makers' margins.

**Tags**: `#storage chips`, `#smartphone industry`, `#supply chain`, `#price hike`, `#TrendForce`

---

<a id="item-15"></a>
## [UK Proposes Easing Apple and Google App Store Payment Rules](https://www.reuters.com/world/uk-regulator-proposes-easing-apple-google-app-store-payment-rules-2026-06-30/) ⭐️ 7.0/10

On June 30, 2026, the UK Competition and Markets Authority (CMA) proposed allowing app developers to direct users to alternative payment options outside Apple and Google's app stores, with fees for such direction capped to be fair and reasonable. This proposal could significantly reduce the 15-30% commissions that Apple and Google charge developers, potentially lowering costs for consumers and fostering competition in the mobile ecosystem. The CMA also considers requiring Apple to open its NFC technology for contactless payments, enabling third-party payment services in iOS apps. The proposal is part of a consultation under the UK's new digital markets regime, with a final decision expected later in 2026.

telegram · zaihuapd · Jun 30, 12:12

**Background**: The CMA is the UK's principal competition regulator, responsible for promoting competitive markets. In 2025, Apple and Google were designated as having 'strategic market status' in mobile ecosystems under the UK's new digital markets regime, which gives the CMA powers to impose conduct requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Competition_and_Markets_Authority">Competition and Markets Authority - Wikipedia</a></li>
<li><a href="https://www.gov.uk/government/organisations/competition-and-markets-authority">Competition and Markets Authority - GOV. UK</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lfZ2FEZ0R4RUJ3YkI0ZFZFWXd5Z0FQAQ?hl=en-GB&gl=GB&ceid=GB:en">Google News - CMA on Google's market status - Overview</a></li>

</ul>
</details>

**Tags**: `#antitrust`, `#app store`, `#regulation`, `#Apple`, `#Google`

---

<a id="item-16"></a>
## [Claude Desktop Linux Beta Launches for Ubuntu and Debian](https://x.com/ClaudeDevs/status/2071988881717871065) ⭐️ 7.0/10

Anthropic released a Linux beta of Claude Desktop on June 30, providing native desktop support for Ubuntu and Debian systems. Paid users can now access Claude Code, Claude Cowork, and chat features directly on the desktop. This expansion brings the full desktop experience to Linux users, a key demographic of developers and power users who previously relied on browser or terminal access. It strengthens Claude's position as a versatile AI platform across operating systems. The beta supports only Ubuntu and Debian distributions initially, and is available to all paid plans. Features include Claude Code for AI-assisted coding, Claude Cowork for non-technical tasks, and the standard chat interface.

telegram · zaihuapd · Jun 30, 17:12

**Background**: Claude is a series of large language models developed by Anthropic, trained using constitutional AI for ethical compliance. Previously, Linux users could only interact with Claude through a web browser or terminal; this desktop client provides a native, integrated experience.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Cowork">Claude Cowork</a></li>
<li><a href="https://grokipedia.com/page/Claude_Cowork">Claude Cowork</a></li>

</ul>
</details>

**Tags**: `#Claude`, `#Linux`, `#Desktop`, `#AI`, `#Ubuntu`

---