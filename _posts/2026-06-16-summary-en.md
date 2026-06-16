---
layout: default
title: "Horizon Summary: 2026-06-16 (EN)"
date: 2026-06-16
lang: en
---

> From 37 items, 17 important content pieces were selected

---

1. [Backdoor in LinkedIn Job Offer Targets Developers via npm](#item-1) ⭐️ 9.0/10
2. [Critical Path Traversal in Nezha Monitoring (CVSS 9.1)](#item-2) ⭐️ 9.0/10
3. [vLLM v0.23.0 Optimizes DeepSeek-V4 and Expands Model Runner V2](#item-3) ⭐️ 8.0/10
4. [Banned Book Library Hidden in a Smart Light Bulb](#item-4) ⭐️ 8.0/10
5. [Iroh 1.0: Peer-to-Peer Networking Library Released](#item-5) ⭐️ 8.0/10
6. [Hetzner Cloud Server Prices Surge Up to 3x](#item-6) ⭐️ 8.0/10
7. [Fox to Acquire Roku for $22 Billion](#item-7) ⭐️ 8.0/10
8. [Salesforce to Acquire Fin for $3.6B](#item-8) ⭐️ 8.0/10
9. [Why AI Hasn't Replaced Software Engineers, and Won't](#item-9) ⭐️ 8.0/10
10. [US orders Anthropic to disable two AI models over security](#item-10) ⭐️ 8.0/10
11. [Rio 3.5 Model Exposed as Shell of Chinese Open-Source Models](#item-11) ⭐️ 8.0/10
12. [Local LLMs Replace Cloud Coding Assistants](#item-12) ⭐️ 7.0/10
13. [Commander Keen Engine White Paper Released](#item-13) ⭐️ 7.0/10
14. [Copper drug restores memory, clears Alzheimer's proteins in mice](#item-14) ⭐️ 7.0/10
15. [Personality Clashes Led to Anthropic Models Going Offline](#item-15) ⭐️ 7.0/10
16. [ByteDance in Talks to Buy AI Chips from Iluvatar Corex, Baidu](#item-16) ⭐️ 7.0/10
17. [Lawsuit Accuses Anthropic of Misleading AI Plan Limits](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Backdoor in LinkedIn Job Offer Targets Developers via npm](https://roman.pt/posts/linkedin-backdoor/) ⭐️ 9.0/10

A developer discovered a backdoor hidden in a GitHub repository sent by a fake recruiter on LinkedIn, which exploits npm's automatic script execution to run malicious code when dependencies are installed. This novel social engineering attack targets developers during job interviews, a trusted process, and could lead to widespread supply chain compromises if successful, as multiple victims have already been reported. The backdoor is buried in commented-out test code and executes via npm's 'prepare' script, which runs automatically after 'npm install'. The payload communicates with a remote server to receive commands.

hackernews · lwhsiao · Jun 15, 20:00 · [Discussion](https://news.ycombinator.com/item?id=48546294)

**Background**: npm is a package manager for Node.js that allows packages to define scripts (e.g., 'prepare') that run automatically during installation. This feature, while convenient, can be abused to execute arbitrary code. Social engineering attacks on developers have increased, with fake job offers being a common vector.

<details><summary>References</summary>
<ul>
<li><a href="https://dev.to/trknhr/lessons-from-the-spring-2026-oss-incidents-hardening-npm-pnpm-and-github-actions-against-1jnp">Lessons from the Spring 2026 OSS Incidents: Hardening npm , pnpm...</a></li>
<li><a href="https://docs.bswen.com/blog/2026-03-31-axios-supply-chain-attack/">What Happened in the Axios npm Supply Chain Attack? | BSWEN</a></li>

</ul>
</details>

**Discussion**: Commenters express concern that this attack is uncomfortably close to normal interview tasks, with some reporting they have encountered similar attempts multiple times. There is frustration that GitHub and LinkedIn have not taken down the malicious content despite reports.

**Tags**: `#supply chain attack`, `#social engineering`, `#npm`, `#cybersecurity`, `#LinkedIn`

---

<a id="item-2"></a>
## [Critical Path Traversal in Nezha Monitoring (CVSS 9.1)](https://github.com/nezhahq/nezha/security/advisories/GHSA-5c25-7vpj-9mqh) ⭐️ 9.0/10

A critical path traversal vulnerability (CVE-2026-53519, CVSS 9.1) has been disclosed in Nezha Monitoring versions below 2.0.13, allowing unauthenticated attackers to read arbitrary files such as config.yaml and extract JWT secrets. Nezha Monitoring is widely used for server monitoring; this vulnerability could lead to full compromise of the dashboard and connected agents, as JWT secrets can be used to forge authentication tokens. The vulnerability resides in the dashboard's NoRoute handler, where any URL starting with /dashboard is treated as an admin-frontend asset request, enabling path traversal via sequences like /dashboard../data/config.yaml. No authentication is required for exploitation.

telegram · zaihuapd · Jun 15, 09:25

**Background**: Nezha Monitoring is an open-source, lightweight server monitoring and O&M tool that consists of a dashboard (server) and agents installed on monitored hosts. JWT (JSON Web Token) is commonly used for authentication; if the secret is leaked, attackers can forge valid tokens to gain unauthorized access.

<details><summary>References</summary>
<ul>
<li><a href="https://www.thehackerwire.com/nezha-monitoring-unauthenticated-file-read-cve-2026-53519/">Nezha Monitoring Unauthenticated File Read (CVE-2026-53519) – TheHackerWire</a></li>
<li><a href="https://cve.threatint.eu/CVE/CVE-2026-53519">CVE-2026-53519 | THREATINT</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#nezha`, `#path traversal`, `#open source`

---

<a id="item-3"></a>
## [vLLM v0.23.0 Optimizes DeepSeek-V4 and Expands Model Runner V2](https://github.com/vllm-project/vllm/releases/tag/v0.23.0) ⭐️ 8.0/10

vLLM v0.23.0 introduces major optimizations for DeepSeek-V4, including decoupled sparse MLA metadata, a TRTLLM-gen attention kernel, and EPLB support for Mega-MoE, while expanding Model Runner V2 (MRv2) by default to Llama and Mistral dense models. These improvements significantly boost inference performance and efficiency for two of the most important model families—DeepSeek-V4 and Llama/Mistral—making vLLM an even more attractive open-source inference engine for production deployments. The release includes 408 commits from 200 contributors, adds support for new models like Step-3.7-Flash and Gemma 4 Unified, and introduces a Rust frontend with streaming generate and dynamic LoRA endpoints.

github · khluu · Jun 15, 05:27

**Background**: vLLM is a high-performance open-source library for LLM inference and serving, widely used in the AI community. Model Runner V2 (MRv2) is a ground-up reimplementation of vLLM's execution core, designed to be more modular and efficient. DeepSeek-V4 is a large language model with sparse Mixture-of-Experts (MoE) architecture, and its MLA (Multi-head Latent Attention) mechanism is key to its efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://vllm-website-5zwgmvte0-inferact-inc.vercel.app/blog/mrv2">Model Runner V 2 : A Modular and Faster Core for vLLM | vLLM Blog</a></li>
<li><a href="https://docs.vllm.ai/en/latest/api/vllm/models/deepseek_v4/sparse_mla/">sparse_mla - vLLM Documentation</a></li>
<li><a href="https://nvidia.github.io/TensorRT-LLM/features/attention.html">Multi-Head, Multi-Query, and Group-Query Attention — TensorRT LLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#DeepSeek`, `#open source`, `#AI infrastructure`

---

<a id="item-4"></a>
## [Banned Book Library Hidden in a Smart Light Bulb](https://www.richardosgood.com/posts/banned-book-library/) ⭐️ 8.0/10

A developer embedded a library of banned books into a Wi-Fi smart light bulb using open-source firmware Tasmota, allowing anyone nearby to access the books via the bulb's Wi-Fi network. This project creatively combines IoT hacking with free speech advocacy, demonstrating how everyday devices can be repurposed to circumvent censorship and preserve access to information. The bulb runs a web server that serves EPUB files of banned books when connected to its Wi-Fi network; the storage is limited to about 2 MB, so only a small selection of books can be stored.

hackernews · sohkamyung · Jun 15, 22:37 · [Discussion](https://news.ycombinator.com/item?id=48547985)

**Background**: Tasmota is an open-source firmware that replaces the stock firmware on many ESP8266-based smart devices, giving users full control over the device. The project was inspired by PirateBox and LibraryBox, which turn Wi-Fi access points into offline file-sharing hubs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.richardosgood.com/posts/banned-book-library/">Banned Book Library | Rick's Blog</a></li>
<li><a href="https://github.com/ct-Open-Source/tuya-convert/issues/830">Merkury MI-BW904-999W, Merkury Innovations A21 Smart Light Bulb ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/List_of_books_banned_by_governments">List of books banned by governments - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project's creativity and political statement, with some drawing parallels to PirateBox and mesh networking. One user noted concerns about the 'banned books' list being influenced by media narratives, but overall sentiment was positive.

**Tags**: `#censorship`, `#IoT`, `#free speech`, `#hacking`, `#privacy`

---

<a id="item-5"></a>
## [Iroh 1.0: Peer-to-Peer Networking Library Released](https://www.iroh.computer/blog/v1) ⭐️ 8.0/10

Iroh 1.0 has been released as a peer-to-peer networking library that enables easy, secure connections between app instances without requiring user accounts, and now supports custom transports. This simplifies distributed app development by providing a 'Tailscale at the application layer' approach, reducing the need for centralized infrastructure and user account management. Iroh uses QUIC multipath under the hood and supports IPv4, IPv6, and relay transports out of the box, with the new custom transport API allowing integration of protocols like WebRTC, BLE, or Tor.

hackernews · chadfowler · Jun 15, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48542480)

**Background**: Iroh is a Rust-based peer-to-peer library built on QUIC with relays and holepunching. Peers connect using NodeIds, which are verified during the handshake to provide end-to-end encryption and authentication. This is similar to how Tailscale works but at the application layer, meaning developers can embed Iroh directly into their apps without requiring users to have separate accounts or VPN software.

<details><summary>References</summary>
<ul>
<li><a href="https://www.iroh.computer/docs/overview">A high-level description of what iroh is</a></li>
<li><a href="https://www.iroh.computer/blog/tor-custom-transport">Use iroh with Tor for anonymous connections - Iroh</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights Iroh as 'Tailscale at the application layer', with developers asking about custom transport support (WebRTC, BLE, LoRa) and noting the need for clearer documentation on dial keys and relay usage. Some users questioned the problem Iroh solves, while others praised the move toward decentralized networking.

**Tags**: `#networking`, `#peer-to-peer`, `#rust`, `#library`, `#release`

---

<a id="item-6"></a>
## [Hetzner Cloud Server Prices Surge Up to 3x](https://docs.hetzner.com/general/infrastructure-and-availability/price-adjustment/#cloud-servers) ⭐️ 8.0/10

Hetzner announced major price adjustments for its cloud servers, with some instances seeing up to a 3x increase, effective for new servers immediately and for existing servers from February 1, 2025. This significant price hike from a major European cloud provider reflects the broader impact of AI-driven demand on hardware costs, potentially forcing developers and businesses to reconsider their cloud spending or seek alternatives. The price increases range from 30-43% for most cloud products, but some instances like the CX22 saw a jump from €3.49 to €10.49 per month, a 200% increase. Traffic overage prices remain unchanged.

hackernews · tuhtah · Jun 15, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48540844)

**Background**: Hetzner is a popular German hosting provider known for affordable dedicated servers and cloud services. The price surge is attributed to rising hardware costs driven by AI demand, which has increased competition for RAM and SSDs, as well as global supply chain constraints.

<details><summary>References</summary>
<ul>
<li><a href="https://lowendtalk.com/discussion/200033/hetzner-black-friday-price-increase-surprise">Hetzner Black Friday Price Increase Surprise — LowEndTalk</a></li>
<li><a href="https://microage.ca/winnipeg/whats-driving-the-surge-in-hardware-prices/">What’s Driving the Surge in Hardware Prices – MB – Manitoba</a></li>

</ul>
</details>

**Discussion**: Community reactions are largely negative, with users expressing shock at the 3x increase and questioning the justification. Some commenters note that hardware costs have indeed risen, while others suggest alternatives like GTHost or compare with hyperscalers.

**Tags**: `#cloud computing`, `#pricing`, `#Hetzner`, `#hardware costs`, `#AI infrastructure`

---

<a id="item-7"></a>
## [Fox to Acquire Roku for $22 Billion](https://www.wsj.com/business/deals/fox-roku-deal-f6e564f9) ⭐️ 8.0/10

Fox Corporation has agreed to acquire Roku for approximately $22 billion, marking one of the largest streaming industry acquisitions in recent years. This deal could reshape the TV hardware landscape by giving a major content provider direct control over a platform used by 30-50% of U.S. households, raising concerns about content neutrality and antitrust issues. To win antitrust approval, Fox has promised to keep the Roku platform open to competitors like Netflix, Disney+, and Max. Fox shares fell 15% on the announcement.

hackernews · thm · Jun 15, 12:50 · [Discussion](https://news.ycombinator.com/item?id=48540499)

**Background**: Roku is a leading streaming hardware and software platform, known for its service-agnostic architecture that allows users to access various streaming apps without favoring any particular content provider. Fox, a major media conglomerate, owns Fox News, Fox Sports, and the Fox broadcast network. The acquisition represents Fox's first major deal since Lachlan Murdoch consolidated control.

<details><summary>References</summary>
<ul>
<li><a href="https://easternherald.com/2026/06/15/fox-corporation-roku-22-billion-acquisition-antitrust-open-platform/">Fox Buys Roku for $22 Billion — and Its Biggest Problem Is Its Own...</a></li>
<li><a href="https://www.usatoday.com/story/money/business/2026/06/15/fox-roku-22b-streaming-deal/90557322007/">Fox to acquire Roku for $22B in streaming push</a></li>

</ul>
</details>

**Discussion**: Community sentiment is largely pessimistic, with users expressing concerns about Fox gaining control over Roku's hardware and the potential loss of platform neutrality. Some users have already started migrating to alternatives like Nvidia Shield to avoid ads and content bias.

**Tags**: `#acquisition`, `#streaming`, `#media`, `#antitrust`, `#Roku`

---

<a id="item-8"></a>
## [Salesforce to Acquire Fin for $3.6B](https://www.salesforce.com/news/press-releases/2026/06/15/salesforce-signs-definitive-agreement-to-acquire-fin/?bc=HL) ⭐️ 8.0/10

Salesforce has signed a definitive agreement to acquire Fin, an AI customer support startup formerly known as Intercom, for $3.6 billion. This acquisition intensifies competition in the AI agent space, particularly against Sierra (valued at $15.8B) founded by Salesforce's ex-Co-CEO Bret Taylor, and signals Salesforce's commitment to embedding AI agents into its CRM ecosystem. Fin charges per resolution rather than per token and learns from past conversations; it already handles 76% of Intercom's customer support requests. The deal comes shortly after Fin's rebrand from Intercom a month ago.

hackernews · colesantiago · Jun 15, 12:08 · [Discussion](https://news.ycombinator.com/item?id=48540126)

**Background**: Fin is an AI-powered customer support agent that automates responses and escalations. Salesforce has been developing its own AI agent platform called Agentforce, which allows building and deploying custom AI agents within the Salesforce ecosystem. The acquisition helps Salesforce compete with standalone AI support startups like Sierra and Decagon.

<details><summary>References</summary>
<ul>
<li><a href="https://fin.ai/">Fin . The highest performing Customer Agent</a></li>
<li><a href="https://www.salesforce.com/agentforce/">Agentforce: The AI Agent Platform | Salesforce</a></li>
<li><a href="https://www.linkedin.com/pulse/1-12m-year-startup-inside-jayanthan-swamy-hj2xc">$1 to $12M in a year: a startup inside a Startup</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some praise AI support agents when well-executed (e.g., Starlink), while others worry about hallucinated excuses. Commenters note the competitive landscape with Sierra and Decagon, and some question the long-term viability of helpdesk SaaS for non-enterprise customers.

**Tags**: `#acquisition`, `#AI`, `#customer support`, `#Salesforce`, `#startup`

---

<a id="item-9"></a>
## [Why AI Hasn't Replaced Software Engineers, and Won't](https://simonwillison.net/2026/Jun/14/why-ai-hasnt-replaced-software-engineers/#atom-everything) ⭐️ 8.0/10

Arvind Narayanan and Sayash Kapoor published an essay arguing that AI has not and will not replace software engineers, citing data from New York's WARN Act filings showing no AI-related layoffs in the first year of disclosure. This evidence-based counterargument challenges the prevailing narrative that AI will cause mass unemployment in software engineering, a profession considered uniquely vulnerable to AI disruption. It reassures engineers and informs public debate on AI's labor impact. The authors identify three real bottlenecks in software engineering that AI cannot automate: deciding what to build, verifying and being accountable for deliverables, and deep human understanding of the codebase, business, and environment. They note that AI speeds up coding but not these core activities.

rss · Simon Willison · Jun 14, 23:54

**Background**: The Worker Adjustment and Retraining Notification (WARN) Act requires employers to provide advance notice of mass layoffs. In March 2025, New York added an AI disclosure checkbox to its WARN filings, making it the first U.S. state to do so. Over 160 companies filed notices in the first year, but none checked the AI box. Arvind Narayanan and Sayash Kapoor are Princeton AI scholars and authors of the book 'AI Snake Oil', which critically examines AI hype.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hunton.com/hunton-employment-labor-perspectives/new-york-warn-act-no-ai-related-layoffs-reported-in-first-year-of-adding-ai-related-disclosure-to-the-system">New York WARN Act: No AI-Related Layoffs Reported in First Year of Adding AI-Related Disclosure to the System</a></li>
<li><a href="https://en.wikipedia.org/wiki/Arvind_Narayanan">Arvind Narayanan - Wikipedia</a></li>
<li><a href="https://engineering.princeton.edu/news/2025/01/13/ai-snake-oil-conversation-princeton-ai-experts-arvind-narayanan-and-sayash-kapoor">‘AI Snake Oil’: A conversation with Princeton AI experts Arvind Narayanan and Sayash Kapoor - Princeton Engineering</a></li>

</ul>
</details>

**Tags**: `#AI`, `#software engineering`, `#job displacement`, `#labor economics`

---

<a id="item-10"></a>
## [US orders Anthropic to disable two AI models over security](https://t.me/zaihuapd/41960) ⭐️ 8.0/10

The US Commerce Department issued an export control directive to Anthropic, ordering the company to suspend access to its Fable 5 and Mythos 5 AI models for any foreign national, both inside and outside the US. In response, Anthropic disabled access to these models for all customers, including its own foreign employees. This marks a significant escalation in government intervention over AI model access, setting a precedent for national security-based export controls on advanced AI. It could reshape how AI companies deploy models globally and may lead to stricter regulations across the industry. The directive was reportedly driven by concerns that the models could be jailbroken, posing security risks. Anthropic stated that other Claude models remain unaffected, and the company is working to restore access as soon as possible.

telegram · zaihuapd · Jun 15, 08:55

**Background**: Fable 5 and Mythos 5 are Anthropic's most advanced AI models, with Mythos 5 being the top-tier model. The US government has increasingly used export controls to limit the spread of sensitive technologies, especially AI, to foreign entities. This action follows similar measures targeting other AI companies.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/13/anthropic-disable-advanced-ai-models-us-government-order">Anthropic to disable its most advanced AI models after US order...</a></li>
<li><a href="https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/">Anthropic disables Fable and Mythos AI models following... | Fortune</a></li>
<li><a href="https://www.aljazeera.com/news/2026/6/13/us-orders-anthropic-to-disable-ai-models-for-all-foreign-nationals">US orders Anthropic to disable AI models for all foreign... | Al Jazeera</a></li>

</ul>
</details>

**Tags**: `#AI regulation`, `#export controls`, `#national security`, `#Anthropic`, `#AI safety`

---

<a id="item-11"></a>
## [Rio 3.5 Model Exposed as Shell of Chinese Open-Source Models](https://mp.weixin.qq.com/s/0oYevRBT8PPxG5hudOXxug) ⭐️ 8.0/10

The open-source Rio 3.5 model, previously celebrated as state-of-the-art, was revealed to be a 'shell' model combining Nex and Qwen, leading to its takedown and an apology from the Rio team. This incident exposes a significant case of model plagiarism in the open-source AI community, undermining trust and highlighting the need for better verification of claimed innovations. Nex team found that without system prompts, Rio 3.5 identified itself as Nex 79% of the time, and weight analysis showed collinearity over 0.98 with a mix ratio of about 0.57 Nex to 0.43 Qwen.

telegram · zaihuapd · Jun 15, 12:39

**Background**: Rio 3.5 is a 397-billion-parameter Mixture-of-Experts model claimed to be developed by the city of Rio de Janeiro. Nex-N2-Pro is an open-source model released by Chinese AI lab Nex-AGI in early June 2026, built on Alibaba's Qwen3.5 base. The controversy follows similar past incidents, such as Cursor's Composer 2 being revealed as Kimi and Stanford's Llama3-V copying MiniCPM-Llama3-V 2.5.

<details><summary>References</summary>
<ul>
<li><a href="https://iset-news.online/article/rio-de-janeiro-built-an-ai-model-that-beat-deepseek-but-was-based-on-someone-elses-work-nPTNdp">Rio de Janeiro Built an AI Model That Beat... — ISET-NEWS</a></li>
<li><a href="https://dev.to/jamilxt/rio-de-janeiros-homegrown-ai-was-someone-elses-model-with-a-new-name-jcb">Rio de Janeiro's 'Homegrown' AI Was Someone Else's Model Wit...</a></li>
<li><a href="https://huggingface.co/nex-agi/Nex-N2-Pro">nex -agi/ Nex -N2-Pro · Hugging Face</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#plagiarism`, `#model controversy`, `#LLM`

---

<a id="item-12"></a>
## [Local LLMs Replace Cloud Coding Assistants](https://news.ycombinator.com/item?id=48542100) ⭐️ 7.0/10

Hacker News users report fully replacing cloud-based coding assistants like Claude and GPT with local models such as Qwen3.6 and Gemma, achieving speeds up to 150 tokens per second on consumer hardware. This shift demonstrates that local models are now viable for daily coding, offering privacy and cost savings without sacrificing performance for many tasks, potentially reducing reliance on expensive cloud subscriptions. Users report using setups like llama.cpp with Qwen3.6-35B-A3B-MTP on dual RTX 3090s or Mac Studio with 128GB RAM, with quality comparable to frontier models from 8-12 months ago.

hackernews · cloudking · Jun 15, 14:46

**Background**: Local LLMs run on the user's own hardware, avoiding cloud costs and data privacy concerns. Tools like Ollama, llama.cpp, and Continue extension for VSCode make it easier to set up local coding assistants. Tokens per second (tok/s) measures inference speed; 150 tok/s is considered fast for local models.

<details><summary>References</summary>
<ul>
<li><a href="https://medium.com/data-science-collective/how-to-build-your-own-llm-coding-assistant-with-qwen2-5-coder-b26aaadf071d">How to Build Your Own LLM Coding Assistant With... | Medium</a></li>
<li><a href="https://vasilkoff.com/blog/vscodium-and-ollama">VSCodium + Ollama: Local LLM Coding Setup Guide</a></li>
<li><a href="https://www.packetswitch.co.uk/using-the-continue-vscode-extension-and-local-llms-for-improved-coding/">How to Use Continue and Local LLMs for Better Coding in VSCode?</a></li>

</ul>
</details>

**Discussion**: Commenters generally agree that local models are good enough for most daily coding tasks, though not as smart as top cloud models. Some highlight the importance of privacy and cost savings, while others note the need for powerful hardware like dual RTX 3090s.

**Tags**: `#local LLM`, `#coding assistant`, `#privacy`, `#open source`

---

<a id="item-13"></a>
## [Commander Keen Engine White Paper Released](https://forgottenbytes.net/commander_keen.html) ⭐️ 7.0/10

A detailed white paper analyzing the game engine of Commander Keen has been published, highlighting its technical innovations in smooth scrolling on early PC hardware. This deep-dive provides valuable insight into the pioneering techniques used by id Software, which laid the groundwork for later industry-defining games like Wolfenstein 3D and Doom. The white paper covers the adaptive tile refresh (ATR) technique, which used EGA's CRTC to read four bytes in parallel, enabling smooth scrolling on the limited hardware of the era.

hackernews · mfiguiere · Jun 15, 17:52 · [Discussion](https://news.ycombinator.com/item?id=48544781)

**Background**: Commander Keen is a series of side-scrolling platform games developed by id Software in the early 1990s. At that time, PC graphics hardware (EGA) lacked hardware sprite support, making smooth scrolling a significant challenge. The adaptive tile refresh technique was a clever software solution that built a virtual screen in VRAM and scrolled it smoothly.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Commander_Keen">Commander Keen - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Enhanced_Graphics_Adapter">Enhanced Graphics Adapter - Wikipedia</a></li>
<li><a href="https://ohtldr.com/summary/commander-keens-adaptive-tile-refresh/">Commander Keen ’s adaptive tile refresh – Oh TL;DR</a></li>

</ul>
</details>

**Discussion**: Commenters praised the white paper, with some recommending the book 'Masters of Doom' for historical context and others noting the need to compare PC hardware with consoles like the SNES to understand the achievement. One user also pointed to similar analyses like Cosmodoc.

**Tags**: `#game engine`, `#retro computing`, `#id Software`, `#technical deep-dive`

---

<a id="item-14"></a>
## [Copper drug restores memory, clears Alzheimer's proteins in mice](https://www.monash.edu/news/articles/copper-drug-restores-memory-and-clears-toxic-alzheimers-proteins) ⭐️ 7.0/10

Researchers at Monash University have shown that a copper transport drug can restore memory and clear toxic amyloid-beta proteins in mouse models of Alzheimer's disease. The drug has already undergone safety evaluations for other diseases, potentially enabling rapid human trials. This represents a potential breakthrough in Alzheimer's treatment, as current therapies targeting amyloid-beta have largely failed in clinical trials. If successful in humans, it could offer a new therapeutic avenue for millions of patients worldwide. The drug works by restoring copper homeostasis in the brain, which is thought to facilitate the clearance of amyloid-beta plaques. However, the study is still at the preclinical stage, and skepticism remains regarding the amyloid hypothesis of Alzheimer's disease.

hackernews · bookofjoe · Jun 15, 14:48 · [Discussion](https://news.ycombinator.com/item?id=48542132)

**Background**: Alzheimer's disease is characterized by the accumulation of amyloid-beta plaques in the brain, a hallmark that has driven drug development for decades. However, many amyloid-targeting drugs have failed to show clinical benefit, leading to debate about whether amyloid is a cause or a consequence of the disease. Copper dysregulation has also been implicated in Alzheimer's pathology, making copper transport a novel therapeutic target.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48542132">Copper transport drug restores memory and clears... | Hacker News</a></li>
<li><a href="https://vue-hackernews-ssr-5cavbdjcta-ew.a.run.app/item/48542132">Vue HN 2.0 | Copper transport drug restores memory and clears toxic...</a></li>
<li><a href="https://colab.ws/articles/10.1007/s00249-007-0235-2">Copper transport and Alzheimer ’ s disease | CoLab</a></li>

</ul>
</details>

**Discussion**: Community comments express cautious optimism but also skepticism. Some users note that amyloid-targeting therapies have a poor track record, while others argue that amyloid plaques are real and may still be relevant. One commenter highlights that the drug has only been tested in mice, and human trials are needed.

**Tags**: `#Alzheimer's`, `#copper transport`, `#amyloid-beta`, `#drug discovery`, `#neuroscience`

---

<a id="item-15"></a>
## [Personality Clashes Led to Anthropic Models Going Offline](https://simonwillison.net/2026/Jun/15/axios-clashes-anthropics/#atom-everything) ⭐️ 7.0/10

Axios reported that personality clashes and behind-the-scenes tensions between Anthropic and the US government led to an export control directive, forcing Anthropic to disable its advanced AI models Fable and Mythos for all users. This incident highlights how interpersonal dynamics and governance issues can directly impact AI deployment and national security policy, potentially affecting Anthropic's IPO prospects and the broader AI industry's relationship with regulators. The article cites sources familiar with the administration and Anthropic, noting that a 'potential narrow, non-universal jailbreak' triggered the government response, and that perfect jailbreak resistance may be impossible.

rss · Simon Willison · Jun 15, 14:57

**Background**: Anthropic is an AI safety company that developed advanced models like Fable and Mythos. In June 2026, the US government issued an export control directive ordering Anthropic to suspend access to these models for foreign nationals, citing national security concerns. The company complied by disabling the models for all users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/13/anthropic-disable-advanced-ai-models-us-government-order">Anthropic to disable its most advanced AI models after US order...</a></li>
<li><a href="https://fortune.com/2026/06/13/anthropic-disables-fable-mythos-export-controls-national-security-threat/">Anthropic disables Fable and Mythos AI models following... | Fortune</a></li>

</ul>
</details>

**Discussion**: The community discussion on Simon Willison's blog expresses skepticism about the government's reasoning and notes the political experience of Anthropic's red team lead. Commenters also question whether Anthropic has addressed universal jailbreak attacks from 2023.

**Tags**: `#Anthropic`, `#AI governance`, `#export controls`, `#policy`, `#AI safety`

---

<a id="item-16"></a>
## [ByteDance in Talks to Buy AI Chips from Iluvatar Corex, Baidu](https://www.reuters.com/world/china/bytedance-talks-with-chinas-iluvatar-corex-purchase-ai-chips-sources-say-2026-06-15/) ⭐️ 7.0/10

ByteDance is in talks to purchase at least 50,000 AI chips from Chinese startup Iluvatar Corex for inference tasks, and is also considering Baidu's Kunlun chips. If the deal goes through, Iluvatar Corex would become ByteDance's third-largest domestic GPU supplier after Huawei and Cambricon. This move signals ByteDance's strategic push to reduce reliance on Nvidia amid US export restrictions, and highlights the growing maturity of China's domestic AI chip ecosystem. The news caused Iluvatar Corex's stock price to jump 12%. The chips are intended for AI inference workloads, not training. ByteDance is also evaluating Baidu's Kunlun chips as an additional option. Iluvatar Corex develops GPGPUs for AI, and Baidu's Kunlun M100 and M300 are set to launch in 2026 and 2027.

telegram · zaihuapd · Jun 15, 06:53

**Background**: ByteDance, the parent company of TikTok, is one of the world's largest consumers of AI chips, primarily using Nvidia GPUs. However, US export controls have restricted Nvidia's advanced chip sales to China, prompting Chinese tech firms to seek domestic alternatives. Iluvatar Corex is a Shanghai-based AI chip startup, while Baidu's Kunlun chip is a self-developed AI accelerator. Huawei and Cambricon are already major domestic GPU suppliers to ByteDance.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Iluvatar_CoreX">Iluvatar CoreX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Kunlunxin">Kunlunxin - Wikipedia</a></li>
<li><a href="https://www.chinadaily.com.cn/a/202511/14/WS69166bfba310d6866eb29629.html">Baidu unveils new Kunlun chips - Chinadaily.com.cn</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#ByteDance`, `#China tech`, `#semiconductors`, `#geopolitics`

---

<a id="item-17"></a>
## [Lawsuit Accuses Anthropic of Misleading AI Plan Limits](https://www.wsj.com/tech/ai/anthropic-sued-over-limits-on-its-200-a-month-ai-plans-e2a109e4) ⭐️ 7.0/10

A Washington D.C. consumer, Karl Kahn, filed a class-action lawsuit against Anthropic, alleging that its $100/month Max 5x and $200/month Max 20x subscription plans do not deliver the advertised usage limits. This is one of the first major legal challenges to AI subscription transparency, potentially forcing companies to clearly disclose usage caps and refund customers if limits are misleading. The lawsuit cites an email from Anthropic in July 2025 as evidence, and seeks refunds for all users who purchased these plans since April 2024. Anthropic's help center states that Max plans provide 5x or 20x more usage per session than Pro, but users report unclear and lower actual limits.

telegram · zaihuapd · Jun 15, 14:17

**Background**: Anthropic offers Claude Pro ($20/month) and higher-tier Max plans ($100 and $200/month) that promise 5x or 20x more usage. However, users have complained that the actual usage limits are vague and often lower than advertised, leading to confusion and frustration. This lawsuit highlights growing consumer concerns over AI subscription pricing and transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://support.claude.com/en/articles/11049741-what-is-the-max-plan">What is the Max plan? | Claude Help Center</a></li>
<li><a href="https://support.anthropic.com/en/articles/11145838-using-claude-code-with-your-pro-or-max-plan">Using Claude Code with your Pro or Max Plan | Anthropic Help Center</a></li>
<li><a href="https://blog.laozhang.ai/en/posts/claude-daily-limit">Claude Daily Limit in 2026: What Free, Pro, and Max Actually Reset</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#lawsuit`, `#AI subscription`, `#consumer protection`, `#transparency`

---