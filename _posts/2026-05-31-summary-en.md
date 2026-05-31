---
layout: default
title: "Horizon Summary: 2026-05-31 (EN)"
date: 2026-05-31
lang: en
---

> From 36 items, 18 important content pieces were selected

---

1. [vLLM v0.22.0: DeepSeek V4 Hardening, MRv2, Rust Frontend](#item-1) ⭐️ 8.0/10
2. [Microsoft to Downgrade Perpetual Office Licenses to View-Only](#item-2) ⭐️ 8.0/10
3. [Domain Expertise Is the Real Competitive Advantage](#item-3) ⭐️ 8.0/10
4. [Accenture acquires Ookla for $1.2B to boost network AI](#item-4) ⭐️ 8.0/10
5. [Zig ELF Linker Advances Toward C Replacement](#item-5) ⭐️ 8.0/10
6. [OpenRouter Raises $113M Series B](#item-6) ⭐️ 8.0/10
7. [Anthropic Details Sandboxing Techniques for Claude Across Products](#item-7) ⭐️ 8.0/10
8. [Running Python ASGI Apps in Browser via Pyodide + Service Worker](#item-8) ⭐️ 8.0/10
9. [Blue Origin's New Glenn Rocket Explodes During Static Fire Test](#item-9) ⭐️ 8.0/10
10. [SpaceX Wins $4.16B U.S. Space Force Satellite Contract](#item-10) ⭐️ 8.0/10
11. [Huawei's 'Tao's Law' Proposes Time Scaling to Replace Geometric Scaling](#item-11) ⭐️ 8.0/10
12. [Voxel Space Algorithm Explained](#item-12) ⭐️ 7.0/10
13. [Openrsync: OpenBSD's Secure Rsync Implementation](#item-13) ⭐️ 7.0/10
14. [Pope Leo's First Encyclical Criticizes Technological Messianism](#item-14) ⭐️ 7.0/10
15. [Chad Whitacre Retires from Tech, Cites AI as Last Straw](#item-15) ⭐️ 7.0/10
16. [Datasette 1.0a31 Adds Write Queries and Stored Queries](#item-16) ⭐️ 7.0/10
17. [Delivery Rider Oversupply: 20M Riders for 4M Needed](#item-17) ⭐️ 7.0/10
18. [Codex Now Supports Cross-Device Remote Control](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [vLLM v0.22.0: DeepSeek V4 Hardening, MRv2, Rust Frontend](https://github.com/vllm-project/vllm/releases/tag/v0.22.0) ⭐️ 8.0/10

vLLM v0.22.0 introduces major hardening for DeepSeek V4, advances Model Runner V2 toward default, and adds an experimental Rust frontend. The release includes 459 commits from 230 contributors. This release significantly improves support for cutting-edge models like DeepSeek V4 and Qwen3, and the Model Runner V2 promises a cleaner, more efficient inference core. The experimental Rust frontend could pave the way for better performance and safety in production deployments. DeepSeek V4 gains NVFP4 fused MoE support, CUDA graph full/piecewise modes, and MTP speculative decoding. Model Runner V2 now automatically selects for Qwen3 dense models and falls back to MRv1 when a KV connector is present.

github · khluu · May 29, 10:28

**Background**: vLLM is a high-throughput, memory-efficient inference engine for large language models. Model Runner V2 is a ground-up reimplementation of the core execution path, designed to be more modular and efficient. NVFP4 is a 4-bit floating-point format from NVIDIA that reduces memory usage while maintaining accuracy.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/v0.10.2/api/vllm/model_executor/layers/quantization/utils/nvfp4_moe_support.html">nvfp4_moe_support - vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/mrv2">Model Runner V2: A Modular and Faster Core for vLLM | vLLM Blog</a></li>

</ul>
</details>

**Tags**: `#LLM inference`, `#vLLM`, `#DeepSeek`, `#open source`, `#performance`

---

<a id="item-2"></a>
## [Microsoft to Downgrade Perpetual Office Licenses to View-Only](https://consumerrights.wiki/w/Microsoft_Office_2019_and_2021_for_Mac_view-only_conversion_(2026)) ⭐️ 8.0/10

Microsoft announced that starting July 13, 2026, perpetually-licensed Office 2019 and 2021 for Mac will switch to view-only mode due to a required security certificate update that older versions cannot support. This move effectively revokes core functionality of previously purchased perpetual licenses, undermining the traditional promise of indefinite offline use and pushing users toward Microsoft 365 subscriptions. The view-only mode allows users to open and read files but prevents editing, printing, or creating new documents. The change applies to Word, Excel, PowerPoint, Outlook, and OneNote on Mac.

hackernews · antipurist · May 30, 23:26 · [Discussion](https://news.ycombinator.com/item?id=48341578)

**Background**: Perpetual licenses allow users to use software indefinitely after a one-time purchase, unlike subscriptions which require ongoing payments. Microsoft has been increasingly shifting from perpetual licenses to subscription-based Microsoft 365, and this move is seen as a further step in that direction.

<details><summary>References</summary>
<ul>
<li><a href="https://cpl.thalesgroup.com/software-monetization/perpetual-vs-subscription-licenses">Perpetual License vs. Subscription Model: Long-Term Effects on Revenue</a></li>
<li><a href="https://talk.tidbits.com/t/office-2019-switching-to-view-only-mode-what-to-do/33495">Office 2019 switching to view-only mode—what to do?</a></li>
<li><a href="https://learn.microsoft.com/en-us/answers/questions/5637995/i-bought-office-but-excel-and-word-shows-view-only">I bought office but excel and word shows view only</a></li>

</ul>
</details>

**Discussion**: Community comments express strong backlash, with users calling the change illegal and noting that pirated versions may better honor the original contract. Some speculate the accelerated timeline is driven by AI labs using offline Office in agents, prompting Microsoft to push subscription licensing.

**Tags**: `#Microsoft`, `#licensing`, `#software`, `#Office`, `#consumer rights`

---

<a id="item-3"></a>
## [Domain Expertise Is the Real Competitive Advantage](https://www.brethorsting.com/blog/2026/05/domain-expertise-has-always-been-the-real-moat/) ⭐️ 8.0/10

A blog post argues that domain expertise, not AI proficiency, is the true moat in software development, challenging the hype around AI-assisted coding. This perspective reframes the debate on AI's role in software engineering, suggesting that deep domain knowledge will remain irreplaceable even as AI tools improve. The post references 'vibe coding'—a practice where developers accept AI-generated code without thorough review—and argues that domain experts who lack software engineering skills still need traditional engineers to build robust systems.

hackernews · aaronbrethorst · May 30, 20:40 · [Discussion](https://news.ycombinator.com/item?id=48340411)

**Background**: Vibe coding, coined by Andrej Karpathy in 2025, is an AI-assisted development approach where users describe projects in prompts and accept generated code without deep review. It has sparked debate about whether AI reduces the need for traditional software engineering skills.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Vibe_coding">Vibe coding</a></li>
<li><a href="https://grokipedia.com/page/Vibe_coding">Vibe coding</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about shifting goalposts on what makes a good developer, with some noting that domain experts still need software engineers to fix issues like poor database design. Others argue that software itself is a domain, and generalists remain valuable.

**Tags**: `#AI`, `#software engineering`, `#domain expertise`, `#vibe coding`

---

<a id="item-4"></a>
## [Accenture acquires Ookla for $1.2B to boost network AI](https://newsroom.accenture.com/news/2026/accenture-to-acquire-ookla-to-strengthen-network-intelligence-and-experience-with-data-and-ai-for-enterprises) ⭐️ 8.0/10

Accenture has agreed to acquire Ookla, the owner of Speedtest, Downdetector, Ekahau, and RootMetrics, for $1.2 billion to strengthen its network intelligence and data-driven AI services for enterprises. This acquisition gives Accenture access to Ookla's massive dataset of over 250 million consumer-initiated tests per month, enabling it to offer telecoms and enterprises deeper insights for optimizing 5G and Wi-Fi networks. It also signals the growing value of network data as a key asset for AI-driven consulting and services. Ookla's data platform includes controlled drive, walk, and embedded testing options in addition to consumer-initiated tests. Accenture was already a competitor in this space through its earlier acquisition of Umlaut, a network testing firm.

hackernews · Garbage · May 30, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48337987)

**Background**: Ookla is best known for Speedtest.net, a popular tool for measuring internet connection performance, and Downdetector, which tracks real-time service outages. The company's primary revenue comes from selling aggregated network performance data to telecom operators, who pay six-figure annual fees for insights to improve their infrastructure. Accenture is a global IT services and consulting firm that has been investing heavily in AI, including a $3 billion commitment to generative AI.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ookla.com/speedtest-intelligence">Speedtest Intelligence ® Global Performance Metrics | Ookla</a></li>
<li><a href="https://en.wikipedia.org/wiki/Downdetector">Downdetector - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the deal is primarily a data acquisition, as Ookla's real value lies in selling network intelligence to telcos, not in the consumer-facing Speedtest or Downdetector. Some expressed concern about Downdetector's independence now that it is owned by a consulting firm that works with the same companies it monitors.

**Tags**: `#acquisition`, `#network intelligence`, `#data monetization`, `#telecom`, `#AI`

---

<a id="item-5"></a>
## [Zig ELF Linker Advances Toward C Replacement](https://ziglang.org/devlog/2026/#2026-05-30) ⭐️ 8.0/10

Zig's latest devlog reports that the new ELF linker can now build the self-hosted Zig compiler with LLVM and LLD libraries enabled, marking a significant milestone in linker development. This improvement brings Zig closer to becoming a full C replacement with fast iteration speeds, potentially enabling developers to achieve C-like performance with development cycles as quick as those in JavaScript or Python. The linker is capable of incremental linking, which speeds up development builds, but it may be mutually exclusive with link-time optimization (LTO) typically used in release builds.

hackernews · kristoff_it · May 30, 17:29 · [Discussion](https://news.ycombinator.com/item?id=48338673)

**Background**: An ELF linker combines compiled object files into an executable or shared library. Zig is developing its own linker to replace the traditional GNU ld or LLVM's lld, aiming for faster compilation and better integration with its build system.

<details><summary>References</summary>
<ul>
<li><a href="https://ziglang.org/devlog/2026/?2026-05-30">Devlog Zig Programming Language</a></li>
<li><a href="https://hn.nuxt.dev/item/48338673">Nuxt HN | Zig ELF Linker Improvements Devlog</a></li>
<li><a href="https://ziggit.dev/t/devlog-elf-linker-improvements/15808">Devlog ELF Linker Improvements - Media - Ziggit</a></li>

</ul>
</details>

**Discussion**: Community members are enthusiastic, with one user noting that Zig's linker progress makes it a viable C replacement for fast iteration. Another user expressed gladness for choosing Zig as a transpilation target over Rust, citing its superior build system design.

**Tags**: `#Zig`, `#linker`, `#systems programming`, `#compiler`, `#programming languages`

---

<a id="item-6"></a>
## [OpenRouter Raises $113M Series B](https://openrouter.ai/announcements/series-b) ⭐️ 8.0/10

OpenRouter announced a $113 million Series B funding round, solidifying its role as a critical proxy layer for accessing multiple LLM providers with low friction and billing controls. This funding validates OpenRouter's position in the AI infrastructure stack, enabling developers to easily experiment with and switch between models without managing multiple API integrations, which is increasingly important as the LLM landscape diversifies. OpenRouter charges a 5% surcharge on API calls, which some users consider acceptable for the convenience of unified access and billing caps, a feature many model providers still lack.

hackernews · freeCandy · May 30, 17:27 · [Discussion](https://news.ycombinator.com/item?id=48338660)

**Background**: OpenRouter is a proxy service that provides a single API endpoint to access hundreds of LLMs from various providers, including both open-source and proprietary models. It simplifies the developer experience by handling authentication, billing, and routing, and offers features like billing caps and observability. The company aims to reduce friction for AI builders and enable experimentation across models.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/enterprise">Enterprise AI Infrastructure Made Simple | OpenRouter</a></li>
<li><a href="https://github.com/pmbstyle/openrouter-proxy">GitHub - pmbstyle/ openrouter - proxy : Nodejs OpenRouter proxy ...</a></li>

</ul>
</details>

**Discussion**: Community members generally praised OpenRouter for reducing API friction and enabling easy model experimentation, though some questioned the long-term value once the model landscape consolidates. The co-founder clarified that the company remains founder-led and focused on building products for developers.

**Tags**: `#AI Infrastructure`, `#Funding`, `#LLM APIs`, `#OpenRouter`, `#Developer Tools`

---

<a id="item-7"></a>
## [Anthropic Details Sandboxing Techniques for Claude Across Products](https://simonwillison.net/2026/May/30/how-we-contain-claude/#atom-everything) ⭐️ 8.0/10

Anthropic published a detailed technical overview of sandboxing techniques used to contain Claude across Claude.ai, Claude Code, and Cowork, including gVisor, Seatbelt, Bubblewrap, and full VM isolation. This documentation addresses a common trust gap in sandboxing products by providing concrete implementation details, which is crucial for AI safety and enterprise adoption of agentic AI tools. Claude.ai uses gVisor, Claude Code uses Seatbelt on macOS and Bubblewrap on Linux, and Claude Cowork runs a full VM (Apple's Virtualization framework on macOS, HCS on Windows). The post also reveals a previously missed exfiltration vector via api.anthropic.com/v1/files.

rss · Simon Willison · May 30, 21:36

**Background**: Sandboxing is a security technique that isolates applications or processes to limit the damage they can cause if compromised. gVisor is a container sandbox developed by Google that implements Linux system calls in userspace for added security. Seatbelt is macOS's built-in sandbox framework, and Bubblewrap is a lightweight Linux sandboxing tool used by Flatpak. These tools help prevent AI agents from accessing sensitive data or performing unauthorized actions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GVisor">gVisor - Wikipedia</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged sandboxing tool used by Flatpak and similar projects · GitHub</a></li>
<li><a href="https://github.com/bkircher/seatbelt">GitHub - bkircher/ seatbelt : Simple macOS Seatbelt wrapper that runs...</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#sandboxing`, `#Anthropic`, `#Claude`, `#security`

---

<a id="item-8"></a>
## [Running Python ASGI Apps in Browser via Pyodide + Service Worker](https://simonwillison.net/2026/May/30/pyodide-asgi-browser/#atom-everything) ⭐️ 8.0/10

Simon Willison demonstrated a method to run Python ASGI apps in the browser using Pyodide and service workers, enabling JavaScript execution in generated HTML. This approach overcomes the limitation of the previous Web Worker-based approach where <script> tags were not executed. This technique allows full-featured Python web applications like Datasette to run entirely in the browser with JavaScript support, expanding the capabilities of browser-based Python apps. It enables plugins and features that rely on JavaScript to work in Datasette Lite and similar projects. The implementation uses a service worker to intercept network requests and serve responses generated by the Python ASGI app running in Pyodide. Simon Willison used Claude Opus 4.8 to help prototype the solution, and provided demos for a basic ASGI app and Datasette 1.0a31.

rss · Simon Willison · May 30, 21:02

**Background**: Pyodide is a port of CPython to WebAssembly, allowing Python to run in the browser. ASGI (Asynchronous Server Gateway Interface) is a specification for asynchronous Python web servers and applications. Service workers are scripts that run in the browser background and can intercept network requests, acting as a programmable proxy.

<details><summary>References</summary>
<ul>
<li><a href="https://pyodide.org/">Pyodide — Version 0.29.4</a></li>
<li><a href="https://en.wikipedia.org/wiki/Asynchronous_Server_Gateway_Interface">Asynchronous Server Gateway Interface - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API/Using_Service_Workers">Using Service Workers - Web APIs | MDN - MDN Web Docs</a></li>

</ul>
</details>

**Tags**: `#Pyodide`, `#WebAssembly`, `#ASGI`, `#Service Workers`, `#Datasette`

---

<a id="item-9"></a>
## [Blue Origin's New Glenn Rocket Explodes During Static Fire Test](https://arstechnica.com/space/2026/05/blue-origins-new-glenn-rocket-just-exploded-during-a-static-fire-test/) ⭐️ 8.0/10

On May 28, 2026, Blue Origin's New Glenn rocket exploded during a static fire test at Cape Canaveral, destroying the vehicle and damaging the launch pad. The explosion occurred during ignition of the seven BE-4 methane engines, resulting in a total loss of the rocket and significant ground infrastructure damage. This incident severely impacts NASA's Artemis lunar program, as Blue Origin is contracted to provide lunar lander and rover launch services. It also delays Amazon's Project Kuiper satellite internet constellation, as the NG-4 mission was set to deploy 48 Kuiper satellites. The explosion occurred during a static fire test for the NG-4 mission, which was intended to launch 48 Amazon Kuiper broadband satellites. No injuries were reported, but the launch pad's lightning protection tower collapsed and ground infrastructure was severely damaged.

telegram · zaihuapd · May 29, 11:08

**Background**: New Glenn is Blue Origin's heavy-lift orbital rocket, powered by seven BE-4 engines that burn liquefied natural gas (methane) and liquid oxygen. The BE-4 is an oxygen-rich staged combustion engine, the first of its kind built in the U.S. Project Kuiper (now rebranded as Amazon Leo) is Amazon's satellite internet constellation designed to compete with Starlink.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nasaspaceflight.com/2026/05/blue-origin-new-glenn-explodes/">Blue Origin's New Glenn explodes during Static Fire test at ...</a></li>
<li><a href="https://aviationweek.com/space/launch-vehicles-propulsion/new-glenn-explodes-during-static-test-fire">New Glenn Explodes During Static Test Fire | Aviation Week</a></li>
<li><a href="https://en.wikipedia.org/wiki/BE-4">BE-4 - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Blue Origin`, `#New Glenn`, `#rocket explosion`, `#NASA Artemis`, `#space industry`

---

<a id="item-10"></a>
## [SpaceX Wins $4.16B U.S. Space Force Satellite Contract](https://www.bloomberg.com/news/articles/2026-05-29/spacex-wins-4-billion-contract-for-us-golden-dome-satellites) ⭐️ 8.0/10

SpaceX has been awarded a $4.16 billion contract by the U.S. Space Force to build a low-Earth orbit satellite network for tracking airborne threats such as aircraft and cruise missiles, as part of the Golden Dome defense system. This contract marks a major expansion of SpaceX's role in national security space programs and demonstrates the growing importance of commercial space capabilities for military missile tracking and defense. The satellite constellation will integrate space-based sensors, communication systems, and ground processing to reduce blind spots of existing ground-based radars and aircraft monitoring. SpaceX previously worked on space-based interceptor prototypes for Golden Dome and joined a multi-company alliance for the program's software layer.

telegram · zaihuapd · May 30, 01:53

**Background**: The Golden Dome is a proposed multi-layer missile defense system announced by U.S. President Donald Trump in May 2025, intended to shield the United States from long-range and hypersonic missiles. It draws inspiration from Israel's Iron Dome but is planned to be far larger in scale. The system aims to leverage space-based sensors and interceptors for global coverage.

<details><summary>References</summary>
<ul>
<li><a href="https://spacenews.com/space-force-awards-spacex-4-16-billion-to-build-satellite-network-for-airborne-target-tracking/">Space Force awards SpaceX $4.16 billion to build satellite ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Golden_Dome_(missile_defense_system)">Golden Dome (missile defense system) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#defense`, `#satellite`, `#missile tracking`, `#Golden Dome`

---

<a id="item-11"></a>
## [Huawei's 'Tao's Law' Proposes Time Scaling to Replace Geometric Scaling](https://t.me/zaihuapd/41648) ⭐️ 8.0/10

At the 2026 International Symposium on Circuits and Systems (ISCAS) in Shanghai, Huawei introduced 'Tao's Law' (τ-law), a new semiconductor scaling principle that replaces traditional geometric scaling with time scaling. Over the past six years, Huawei has designed and mass-produced 381 chips based on this law, and plans to launch a new Kirin chip this fall using logic folding technology. Tao's Law offers a potential path beyond Moore's Law, which is approaching physical limits, by focusing on reducing time constants rather than transistor dimensions. This could enable continued performance improvements without requiring extreme ultraviolet (EUV) lithography, benefiting the entire semiconductor industry and particularly Chinese firms facing export restrictions. The law is named after the Greek letter τ (tau), which represents the time constant in circuit theory. Huawei's logic folding technology vertically stacks active silicon layers to physically 'fold' critical paths, reducing horizontal wiring and RC delay, and Huawei expects chips based on this law to reach transistor density equivalent to 1.4nm process by 2031.

telegram · zaihuapd · May 30, 02:18

**Background**: Moore's Law, the observation that the number of transistors on a chip doubles approximately every two years, has driven semiconductor advancement for decades but is now slowing due to physical and economic constraints. Geometric scaling—shrinking transistor dimensions—has been the primary method to improve performance, but it requires increasingly expensive lithography tools like EUV. Tao's Law proposes an alternative: systematically reducing the time constant τ across device, circuit, chip, and system levels to achieve performance gains without relying solely on lithographic scaling.

<details><summary>References</summary>
<ul>
<li><a href="https://baike.baidu.com/item/韬定律/67839953">韬定律 - 百度百科</a></li>
<li><a href="https://baike.baidu.com/item/逻辑折叠技术/67870423">逻辑折叠技术 - 百度百科</a></li>
<li><a href="https://www.huxiu.com/article/4861353.html">华为提出韬定律挑战摩尔定律，芯片设计新路径浮出水面</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#Moore's Law`, `#Huawei`, `#chip design`, `#scaling`

---

<a id="item-12"></a>
## [Voxel Space Algorithm Explained](https://s-macke.github.io/VoxelSpace/) ⭐️ 7.0/10

A detailed technical explanation of the Voxel Space rendering algorithm used in the 1992 game Comanche has been published, including interactive demos and source code. This deep dive preserves a historically significant 2.5D rendering technique that achieved realistic terrain on limited hardware, inspiring modern implementations and retro game development. The algorithm uses a height map and color map to render terrain via ray casting, but it is not true voxel rendering; it is a 2.5D engine that lacks full 3D freedom.

hackernews · davikr · May 30, 14:25 · [Discussion](https://news.ycombinator.com/item?id=48336564)

**Background**: Voxel Space is a proprietary engine developed by NovaLogic for the 1992 helicopter simulator Comanche: Maximum Overkill. It was written entirely in assembly language and used a height-map-based ray casting technique to render smooth, organic terrain, which was impressive for its time compared to polygon-based games.

<details><summary>References</summary>
<ul>
<li><a href="https://s-macke.github.io/VoxelSpace/">Voxel Space | VoxelSpace</a></li>
<li><a href="https://github.com/s-macke/VoxelSpace">GitHub - s-macke/VoxelSpace: Terrain rendering algorithm in ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Comanche_(video_game_series)">Comanche (video game series) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the algorithm is technically a height-map ray caster, not true voxel rendering. One user shared a practical analogy for minimal testing, and others linked modern ports and implementations in C++ and AGS Engine.

**Tags**: `#rendering`, `#retro-gaming`, `#algorithms`, `#voxels`

---

<a id="item-13"></a>
## [Openrsync: OpenBSD's Secure Rsync Implementation](https://github.com/kristapsdz/openrsync) ⭐️ 7.0/10

The OpenBSD team has released openrsync, a reimplementation of the widely-used rsync file synchronization tool, with a focus on security and correctness. This matters because rsync is a critical tool for system administration and file transfers, and openrsync aims to reduce vulnerabilities by leveraging OpenBSD's security features like pledge and unveil, potentially offering a safer alternative for network-facing operations. Openrsync is not yet a complete drop-in replacement for rsync; users have reported issues with certain flags and behaviors, such as the --rsync-path option not working as expected. The project is currently being developed as part of an RPKI validator.

hackernews · sph · May 30, 10:51 · [Discussion](https://news.ycombinator.com/item?id=48334854)

**Background**: Rsync is a utility for efficiently transferring and synchronizing files across computers by comparing modification times and sizes. The native rsync protocol does not encrypt data, making it suitable only for trusted networks. OpenBSD's pledge and unveil are security mechanisms that restrict process capabilities and filesystem access, respectively, to limit the impact of potential exploits.

<details><summary>References</summary>
<ul>
<li><a href="https://www.openbsdhandbook.com/rsync/">rsync | OpenBSD Handbook</a></li>
<li><a href="https://hn.nuxt.dev/item/48334854">Nuxt HN | Openrsync: An implementation of rsync , by the OpenBSD ...</a></li>
<li><a href="https://docs.ircnow.org/openbsd/openrsync/">openrsync</a></li>

</ul>
</details>

**Discussion**: Community members have shared practical experiences, noting improvements over time but also pointing out limitations like incomplete flag support. Some users express interest in using openrsync exclusively once it matures, while others mention alternative implementations in Go. There is also discussion about the importance of pledge and unveil for security, and whether these features are available on other platforms like Linux.

**Tags**: `#rsync`, `#OpenBSD`, `#security`, `#file synchronization`, `#open source`

---

<a id="item-14"></a>
## [Pope Leo's First Encyclical Criticizes Technological Messianism](https://www.economist.com/europe/2026/05/28/leos-first-encyclical-attacks-technological-messianism) ⭐️ 7.0/10

Pope Leo XIV released his first encyclical, Magnifica Humanitas, which criticizes technological messianism and warns against the concentration of power through artificial intelligence. This encyclical adds a powerful religious voice to the global debate on AI ethics and control, challenging the narrative that technology alone can solve humanity's problems. The encyclical, titled Magnifica Humanitas, is approximately 42,300 words in English and addresses AI as a central theme, calling for the protection of human dignity and agency.

hackernews · 1vuio0pswjnm7 · May 30, 10:30 · [Discussion](https://news.ycombinator.com/item?id=48334710)

**Background**: Technological messianism is the belief that technology will bring about a utopian future or save humanity. Pope Leo's encyclical follows the tradition of Catholic social teaching, which often addresses contemporary ethical issues. The Vatican has previously engaged with AI ethics, including hosting conferences on the topic.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ncronline.org/vatican/vatican-news/pope-leo-calls-disarm-ai-major-document-warns-technologic-threats-humanity">Pope Leo calls to 'disarm' AI in major document, warns of technologic threats to humanity | National Catholic Reporter</a></li>
<li><a href="https://www.vaticannews.va/en/pope/news/2026-05/pope-leo-xiv-encyclical-magnifica-humanitas-ai.html">Pope Leo’s ‘Magnifica humanitas’: AI must serve humanity not concentrate power - Vatican News</a></li>
<li><a href="https://www.nytimes.com/2026/05/25/world/europe/pope-leo-encyclical.html">Pope Leo Warns of Risks From A.I. in 42,300-Word Encyclical - The New York Times</a></li>

</ul>
</details>

**Discussion**: Community comments highlight the debate over who should control technology, with some pointing to tech CEOs like Sam Altman and Dario Amodei as exhibiting 'AI psychosis.' Others reference Peter Thiel's views on the Antichrist, linking technological messianism to religious concepts.

**Tags**: `#AI ethics`, `#religion and technology`, `#technology control`, `#Vatican`, `#technological messianism`

---

<a id="item-15"></a>
## [Chad Whitacre Retires from Tech, Cites AI as Last Straw](https://simonwillison.net/2026/May/30/retiring-from-tech-to-live-offline/#atom-everything) ⭐️ 7.0/10

Chad Whitacre, creator of Sentry, announced his retirement from tech and open source, planning to live an offline life inspired by the Amish. He cited AI as the final straw, describing it as an invasive presence in his mind. This personal decision from a prominent open source figure highlights growing unease about AI's impact on mental health and lifestyle. It may inspire others to reconsider their relationship with technology and accelerate discussions around digital detox and AI ethics. Whitacre's retirement is accompanied by a typewritten, scanned letter and a video essay. He previously experimented with AI tools like Claude Code and Opus 4.5, which left him feeling intoxicated and disturbed.

rss · Simon Willison · May 30, 19:39

**Background**: The Sentinelese are an uncontacted indigenous people on North Sentinel Island who violently reject outsiders. The Amish are a Christian denomination known for selectively rejecting modern technology to preserve their way of life. Whitacre draws parallels between these groups and his own desire to step away from tech, aiming for a 'Neo-Amish' lifestyle that rejects AI and doomscrolling while accepting cars and electricity.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sentinelese">Sentinelese - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Amish_way_of_life">Amish way of life - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Hacker News comments on the article were mixed, with some expressing sympathy for Whitacre's stance and others questioning the practicality of his plan. Several commenters noted the irony of announcing an offline retirement via an online platform.

**Tags**: `#AI impact`, `#tech career`, `#open source`, `#digital detox`, `#personal essay`

---

<a id="item-16"></a>
## [Datasette 1.0a31 Adds Write Queries and Stored Queries](https://simonwillison.net/2026/May/29/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a31 introduces the ability to execute write queries (INSERT/UPDATE/DELETE) and save stored queries (renamed from 'canned queries') for users with appropriate permissions. This release transforms Datasette from a read-only exploration tool into a full-featured database application platform, enabling users to edit data and share reusable queries within their instance. Write queries are executed via a new interface that provides templated insert/update/delete statements, and permissions are granular (e.g., create-table permission is separate). Stored queries can be saved privately or shared with other instance members.

rss · Simon Willison · May 29, 03:32

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases. Previously, it only supported read-only queries. This alpha release marks a significant step toward Datasette 1.0, adding write capabilities that were previously available only via plugins like datasette-write.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/sql-write-queries/">SQL write queries and stored queries in Datasette ... - Datasette Blog</a></li>
<li><a href="https://simonwillison.net/2026/May/29/datasette/">Release: datasette 1.0a31 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#release`, `#sql`, `#database`, `#open-source`

---

<a id="item-17"></a>
## [Delivery Rider Oversupply: 20M Riders for 4M Needed](https://m.sohu.com/a/1029514455_122135404) ⭐️ 7.0/10

China's instant delivery industry now has nearly 20 million riders, but only about 4 million skilled riders are needed to support the daily 110 million orders, leaving over 16 million riders as redundant capacity. This massive oversupply of riders highlights severe labor market distortion and economic inefficiency in the gig economy, leading to fierce competition among riders and huge financial losses for platforms like Meituan, JD, and Alibaba. The subsidy war that began in February 2025 added over 8 million new riders, while platforms collectively lost billions: Meituan 23.4 billion yuan, JD New Business 46.6 billion yuan, and Alibaba instant retail 87 billion yuan in 2025.

telegram · zaihuapd · May 30, 09:52

**Background**: Instant delivery platforms like Meituan, JD, and Alibaba engaged in a fierce subsidy war starting in early 2025, offering huge discounts to attract users and riders. This led to a surge in rider numbers far beyond actual demand. As subsidies recede, order volumes have not kept pace, resulting in oversupply and intense competition among riders.

<details><summary>References</summary>
<ul>
<li><a href="https://www.163.com/dy/article/KU6JGDUE0556N7I6.html">外卖大战退潮后，2000万骑手挤在路上，1600万是“冗余运力”|单量|扩张...</a></li>
<li><a href="https://www.sohu.com/a/962694058_121385340">三大平台外卖大战：每分钟“烧钱”40万，谁在为“非理性买单”？_补贴_利...</a></li>
<li><a href="https://www.bcbay.com/news/2026/05/30/1020516.html">中国外卖大战后骑手过剩 需400万人涌进2000万人-新闻中心-温哥华港湾...</a></li>

</ul>
</details>

**Tags**: `#gig economy`, `#labor market`, `#platform economics`, `#delivery industry`, `#China`

---

<a id="item-18"></a>
## [Codex Now Supports Cross-Device Remote Control](https://developers.openai.com/codex/changelog#codex-2026-05-28-app) ⭐️ 7.0/10

OpenAI's Codex now allows users to remotely control a Windows-hosted Codex instance from iOS, Android, or Mac devices, and view progress in real time. The update also introduces enhanced collaboration features, including thread coordination in local projects and worktrees, and expanded search that covers conversation content and Git branch names. This update significantly improves Codex's utility for developers who work across multiple devices, enabling seamless remote coding and monitoring. The expanded search and thread coordination features make it easier to manage complex projects and retrieve context, boosting productivity for teams using Codex as an AI coding assistant. Remote control requires Codex running on a Windows host, and the controlling device can be a Mac, iPhone, or Android phone via the ChatGPT mobile app. The new thread coordination allows adding independent background threads to worktrees for flexible multitasking, and the personal profile page now shows detailed usage statistics and token activity.

telegram · zaihuapd · May 30, 10:37

**Background**: Codex is an AI coding assistant developed by OpenAI that can understand and generate code, automate tasks, and interact with desktop applications. Previously, Codex was limited to local use on a single device; this update extends its reach to remote and mobile access, making it more versatile for developers who need to work from different locations or devices.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/work-with-codex-from-anywhere/">Work with Codex from anywhere | OpenAI</a></li>
<li><a href="https://developers.openai.com/codex/remote-connections">Remote connections – Codex | OpenAI Developers</a></li>
<li><a href="https://developers.openai.com/codex/app/worktrees">Worktrees – Codex app | OpenAI Developers</a></li>

</ul>
</details>

**Tags**: `#Codex`, `#remote control`, `#AI coding assistant`, `#collaboration`, `#search`

---