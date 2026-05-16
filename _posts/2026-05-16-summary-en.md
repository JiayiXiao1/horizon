---
layout: default
title: "Horizon Summary: 2026-05-16 (EN)"
date: 2026-05-16
lang: en
---

> From 38 items, 17 important content pieces were selected

---

1. [Zulip Transitions to Nonprofit Foundation](#item-1) ⭐️ 9.0/10
2. [Pixel 10 Zero-Click Exploit Chain Disclosed](#item-2) ⭐️ 9.0/10
3. [First Public M5 macOS Kernel Exploit in 5 Days](#item-3) ⭐️ 9.0/10
4. [vLLM v0.21.0: Breaking Changes, KV Offload, Spec Decode](#item-4) ⭐️ 8.0/10
5. [Mitchell Hashimoto Warns of 'AI Psychosis' in Companies](#item-5) ⭐️ 8.0/10
6. [DOJ demands Apple and Google unmask 100K+ app users](#item-6) ⭐️ 8.0/10
7. [ABC News Removes All FiveThirtyEight Articles](#item-7) ⭐️ 8.0/10
8. [OCaml in Space: OxCaml Stack Annotations Slash GC Latency](#item-8) ⭐️ 8.0/10
9. [arXiv Bans Unchecked LLM Content for 1 Year](#item-9) ⭐️ 8.0/10
10. [Trump Discusses AI Guardrails and Nvidia H200 with Xi](#item-10) ⭐️ 8.0/10
11. [California bill mandates patches or refunds for dead online games](#item-11) ⭐️ 7.0/10
12. [Radicle: A Decentralized Code Forge Built on Git](#item-12) ⭐️ 7.0/10
13. [ChatGPT Android Teardown Reveals Codex Remote Desktop Feature](#item-13) ⭐️ 7.0/10
14. [China in Talks with Boeing for Up to 500 737 MAX Jets](#item-14) ⭐️ 7.0/10
15. [California Class Action Alleges OpenAI Shared User Data with Meta and Google](#item-15) ⭐️ 7.0/10
16. [Alipay Responds to 1.84M Yuan Donation After Payment Disabled](#item-16) ⭐️ 7.0/10
17. [Apple-OpenAI Partnership Frays, OpenAI Considers Legal Action](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Zulip Transitions to Nonprofit Foundation](https://blog.zulip.com/2026/05/15/announcing-zulip-foundation/) ⭐️ 9.0/10

Zulip's core team, including founder Tim Abbott, is stepping back to join Anthropic, and the company is being donated to a newly created independent nonprofit Zulip Foundation. This governance transition ensures Zulip's long-term independence and trustworthiness, addressing community concerns about commercial pressures and data privacy, and sets a precedent for open source sustainability. The announcement was made on a Friday afternoon, which some community members noted as a typical timing for sensitive news. The move comes shortly after Bun's acquisition by a VC firm, drawing comparisons but with key differences.

hackernews · boramalper · May 15, 18:37 · [Discussion](https://news.ycombinator.com/item?id=48152168)

**Background**: Zulip is an open-source team chat platform known for its unique topic-based threading, combining the best of email and chat. It was created in 2012 and is a popular alternative to Slack. Anthropic is an AI safety company founded by former OpenAI researchers, known for developing the Claude language models.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Zulip">Zulip - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://zulip.com/">Zulip — organized team chat</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: many express sadness over the core team's departure but excitement for the foundation's potential. Some draw comparisons to Bun's acquisition, but others argue this is different because Zulip is being donated to a nonprofit. The timing on a Friday afternoon is noted with skepticism.

**Tags**: `#open source`, `#nonprofit`, `#governance`, `#Zulip`, `#community`

---

<a id="item-2"></a>
## [Pixel 10 Zero-Click Exploit Chain Disclosed](https://projectzero.google/2026/05/pixel-10-exploit.html) ⭐️ 9.0/10

Google Project Zero disclosed a full zero-click exploit chain for the Pixel 10, demonstrating remote code execution from a Dolby audio decoding bug to kernel control. This exploit chain highlights the increased attack surface from AI-powered message analysis, which decodes media before user interaction, and underscores the need for rigorous security review of such features. The chain exploits CVE-2025-54957, a Dolby audio bug affecting all Android devices until patched in January 2026, and a video driver vulnerability in the Pixel 10's VPU for kernel escalation.

hackernews · happyhardcore · May 15, 13:39 · [Discussion](https://news.ycombinator.com/item?id=48148460)

**Background**: A zero-click exploit requires no user interaction, making it highly dangerous. AI features on modern phones often pre-process messages (e.g., decoding audio) to enable search and analysis, inadvertently expanding the attack surface. Project Zero is Google's elite security team that finds and discloses critical vulnerabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://projectzero.google/2026/05/pixel-10-exploit.html">A 0-click exploit chain for the Pixel 10: When a Door Closes ...</a></li>
<li><a href="https://cyberpress.org/zero-click-exploit-chain-for-pixel-10/">Google Project Zero Reveals Zero-Click Exploit Chain for Pixel 10</a></li>
<li><a href="https://gbhackers.com/pixel-10-zero-click-exploit-chain/">Google Project Zero Details Pixel 10 Zero-Click Exploit Chain</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concern about AI features increasing attack surface, with one noting the irony of repeating past mistakes. Others discussed vendor response times, with praise for Google's 90-day patch but worry about other Android OEMs. Some questioned the apparent lack of recent iPhone jailbreaks.

**Tags**: `#security`, `#exploit`, `#mobile`, `#Android`, `#0-click`

---

<a id="item-3"></a>
## [First Public M5 macOS Kernel Exploit in 5 Days](https://blog.calif.io/p/first-public-kernel-memory-corruption) ⭐️ 9.0/10

Calif and Mythos Preview collaborated to create the first public kernel memory corruption exploit for Apple M5 macOS, bypassing Apple's MIE hardware protection in just five days. This exploit demonstrates that even Apple's most advanced memory protection, MIE, can be rapidly bypassed with AI assistance, highlighting a significant shift in the cybersecurity landscape. The exploit chain targets macOS 26.4.1 on M5 hardware, using two vulnerabilities and normal system calls to escalate from a non-privileged user to root shell, with a full 55-page technical report to be released after Apple's fix.

telegram · zaihuapd · May 15, 02:15

**Background**: Apple's M5 chips feature Memory Integrity Enforcement (MIE), a hardware- and software-based memory safety system using ARM's Enhanced Memory Tagging Extension (EMTE). Apple spent five years developing MIE to make memory corruption exploits dramatically harder. Mythos Preview is Anthropic's most advanced frontier AI model, designed for cybersecurity research.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.calif.io/p/first-public-kernel-memory-corruption">First public macOS kernel memory corruption exploit on Apple M5</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_M5">Apple M5 - Wikipedia</a></li>
<li><a href="https://security.apple.com/blog/memory-integrity-enforcement/">Memory Integrity Enforcement: A complete vision for memory safety in Apple devices - Apple Security Research</a></li>

</ul>
</details>

**Tags**: `#Apple M5`, `#kernel exploit`, `#macOS security`, `#AI-assisted hacking`, `#MIE bypass`

---

<a id="item-4"></a>
## [vLLM v0.21.0: Breaking Changes, KV Offload, Spec Decode](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 deprecates transformers v4, requires C++20, integrates KV offload with Hybrid Memory Allocator, adds speculative decoding with thinking budget, and introduces a TOKENSPEED_MLA backend for Blackwell GPUs. This release significantly impacts the LLM inference ecosystem by enforcing migration to transformers v5 and modern C++ standards, while improving memory efficiency and speculative decoding for reasoning models, benefiting developers and users of large language models. The KV offloading subsystem now uses HMA with sliding window support and multi-connector capabilities. Speculative decoding respects reasoning/thinking budgets, and the new MLA backend targets DeepSeek-R1/Kimi-K25 on Blackwell GPUs.

github · khluu · May 15, 08:44

**Background**: vLLM is a high-throughput, memory-efficient inference engine for large language models. KV cache offloading moves key-value cache from GPU to CPU memory to reduce GPU memory pressure. Speculative decoding uses a draft model to predict tokens, verified by the target model, to speed up inference without changing output distribution.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/issues/11382">[RFC]: Hybrid Memory Allocator · Issue #11382 · vllm -project/ vllm</a></li>
<li><a href="https://github.com/lightseekorg/tokenspeed/tree/main">GitHub - lightseekorg/tokenspeed: TokenSpeed is a speed-of ...</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#transformers`, `#speculative decoding`, `#GPU`

---

<a id="item-5"></a>
## [Mitchell Hashimoto Warns of 'AI Psychosis' in Companies](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Mitchell Hashimoto, creator of Vagrant and Terraform, warned on social media that many companies are suffering from 'AI psychosis' by blindly trusting AI-generated code and decisions, leading to unstable systems and unsustainable practices. This critique highlights a growing risk in the software industry where over-reliance on AI without proper oversight can degrade code quality and system reliability, potentially creating long-term technical debt and operational crises. Hashimoto's post sparked a debate with 288 comments, where some argued that using AI for code generation is fine as long as humans verify outputs, while others warned that purely AI-written systems could become incomprehensible and unstable.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: 'AI psychosis' originally refers to a mental health phenomenon where individuals develop psychosis from interacting with chatbots. In this context, Hashimoto uses the term metaphorically to describe companies that blindly trust AI outputs without critical thinking, leading to poor engineering decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Chatbot_psychosis">Chatbot psychosis - Wikipedia</a></li>
<li><a href="https://itsfoss.com/news/mitchell-hashimoto-vouch/">Mitchell Hashimoto Launches 'Vouch' to Fight AI Slop in Open Source Ecosystem</a></li>
<li><a href="https://newsletter.pragmaticengineer.com/p/mitchell-hashimoto">Mitchell Hashimoto’s new way of writing code</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with Hashimoto, sharing examples of AI-generated code causing issues. Some noted that AI rescue consulting may become a new high-value service, while others pointed out that the real problem is outsourcing decision-making to AI, not using AI as a tool.

**Tags**: `#AI`, `#software engineering`, `#AI risks`, `#code quality`, `#industry critique`

---

<a id="item-6"></a>
## [DOJ demands Apple and Google unmask 100K+ app users](https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/) ⭐️ 8.0/10

The U.S. Department of Justice is demanding that Apple, Google, and Amazon provide identities, addresses, and purchase histories of over 100,000 users who downloaded EZ Lynk's Auto Agent app, as part of an emissions crackdown. This case sets a major precedent for government surveillance of app store users, raising serious privacy and legal concerns about overreach and the centralization of app distribution. EZ Lynk denies that its app is primarily for emissions cheating, claiming it can also be used for performance monitoring and software upgrades. The DOJ's request covers at least 100,000 users, escalating a years-long legal battle.

hackernews · tencentshill · May 15, 17:28 · [Discussion](https://news.ycombinator.com/item?id=48151383)

**Background**: EZ Lynk's Auto Agent app allows users to modify vehicle engine control units (ECUs), potentially disabling emissions controls. The Clean Air Act prohibits tampering with emissions systems, and the DOJ is investigating widespread use of such tools. App stores like Apple's and Google's serve as centralized distribution points, making them targets for legal demands.

<details><summary>References</summary>
<ul>
<li><a href="https://macdailynews.com/2026/05/15/u-s-doj-demands-apple-and-google-unmask-over-100000-users-of-popular-car-tinkering-app-in-emissions-crackdown/">U.S. DOJ demands Apple and Google unmask over 100,000 users ...</a></li>
<li><a href="https://9to5mac.com/2026/05/15/doj-reportedly-demands-apple-and-google-identify-over-100000-users-of-car-app/">DOJ reportedly demands Apple and Google identify over 100,000 ...</a></li>
<li><a href="https://www.forbes.com/sites/thomasbrewster/2026/05/14/government-demands-apple-and-google-identify-over-100000-users-of-car-app/">The DOJ Is Demanding Apple And Google Identify Over 100,000 ...</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some argue the app is used for illegal emissions tampering and users deserve scrutiny, while others fear this sets a precedent for broader surveillance, such as targeting car modifications that disable GPS tracking. Several users highlight the risks of centralized app distribution and suggest using anonymous alternatives like F-Droid.

**Tags**: `#privacy`, `#legal`, `#app stores`, `#surveillance`, `#automotive`

---

<a id="item-7"></a>
## [ABC News Removes All FiveThirtyEight Articles](https://twitter.com/baseballot/status/2055309076209492208) ⭐️ 8.0/10

ABC News has taken down all articles from FiveThirtyEight, effectively removing the entire archive of the data journalism brand from the web. This move erases a significant collection of data-driven journalism and visualizations, potentially harming public access to valuable analyses and sparking concerns about brand mismanagement and intellectual property disputes. FiveThirtyEight founder Nate Silver claimed ABC refused to sell the IP back to him, citing his criticism of their brand management. The removal includes acclaimed interactive visualizations on gun deaths, p-hacking, and the gut microbiome.

hackernews · cmsparks · May 15, 19:07 · [Discussion](https://news.ycombinator.com/item?id=48152553)

**Background**: FiveThirtyEight was a data journalism website founded by Nate Silver in 2008, known for its statistical analysis of politics, sports, and science. ABC News acquired the brand in 2013, but after layoffs and declining profitability outside election years, the site was gradually marginalized.

**Discussion**: Community comments express sadness over the loss of high-quality visualizations and criticize ABC's management. Some speculate that Nate Silver might buy back the brand cheaply, which would embarrass ABC if he succeeds.

**Tags**: `#data journalism`, `#media`, `#FiveThirtyEight`, `#ABC News`, `#content removal`

---

<a id="item-8"></a>
## [OCaml in Space: OxCaml Stack Annotations Slash GC Latency](https://gazagnaire.org/blog/2026-05-14-borealis.html) ⭐️ 8.0/10

A blog post reveals that OCaml is used in satellite payload software, and the OxCaml compiler's exclave stack annotations dramatically reduce garbage collection pressure and latency, dropping p99.9 latency from 29 ns to 9 ns per packet and eliminating minor GCs entirely over 25 million packets. This demonstrates that high-level, garbage-collected languages like OCaml can be made suitable for real-time, resource-constrained environments such as space, by using advanced compiler techniques to control memory allocation. It opens the door for safer and more productive systems programming in domains traditionally dominated by C/C++. The performance improvements come from OxCaml's exclave stack annotations, which allow developers to specify that certain values should be stack-allocated instead of heap-allocated, reducing GC pressure. The satellite payload software also uses SystemD services, DBus, and a CCSDS-to-DBus bridge, with symmetric-key encryption for data.

hackernews · yminsky · May 15, 10:55 · [Discussion](https://news.ycombinator.com/item?id=48147058)

**Background**: OCaml is a general-purpose, high-level programming language with a garbage collector that automatically manages memory. In low-latency or real-time systems, GC pauses can be problematic. OxCaml is a performance-focused fork of OCaml that introduces stack allocation annotations, enabling developers to bypass the GC for critical paths, similar to how Rust uses ownership but with opt-in pragmatism.

<details><summary>References</summary>
<ul>
<li><a href="https://oxcaml.org/documentation/stack-allocation/reference/">OxCaml | Stack allocation | Reference</a></li>
<li><a href="https://github.com/oxcaml/oxcaml">GitHub - oxcaml/oxcaml: OCaml - Oxidized! · GitHub</a></li>
<li><a href="https://www.dra27.uk/blog/platform/2025/05/07/oxcaml-toes.html">Dipping toes into OxCaml | Notes from the Windows corner</a></li>

</ul>
</details>

**Discussion**: Community members shared firsthand experience: one commenter noted they were likely the first to put OCaml in space in 2016 on GHGSat-D. Another highlighted that the key advantage is having a GC by default with the ability to reduce heap allocations via stack annotations. Some discussed the difficulty of bending GC languages for low-latency scenarios, while others criticized CCSDS for reinventing the wheel.

**Tags**: `#OCaml`, `#space`, `#garbage collection`, `#systems programming`, `#low-latency`

---

<a id="item-9"></a>
## [arXiv Bans Unchecked LLM Content for 1 Year](https://x.com/tdietterich/status/2055000956144935055) ⭐️ 8.0/10

arXiv announced a policy that imposes a 1-year ban on authors who submit papers containing unchecked LLM-generated content, such as hallucinated citations or placeholder data. The ban applies to submissions that show clear signs of unverified AI output. This policy directly addresses the growing problem of LLM-generated content undermining academic integrity in preprint repositories. It sets a precedent for other platforms and reinforces the principle that authors are fully responsible for their submissions, regardless of how the content was generated. The ban applies to content such as hallucinated references, LLM meta-comments, and placeholder data like "table data is for example only, please replace with real experimental data." After the ban ends, authors must have their paper accepted by a credible peer-reviewed venue before resubmitting to arXiv.

telegram · zaihuapd · May 15, 04:30

**Background**: arXiv is a widely used open-access preprint repository where researchers share papers before peer review. Recently, concerns have grown about authors using large language models (LLMs) to generate content without proper verification, leading to fabricated citations and nonsensical data. This policy update aims to preserve the integrity of the repository by holding authors accountable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ArXiv">arXiv - Wikipedia</a></li>
<li><a href="https://arxiv.org/">arXiv .org e- Print archive</a></li>

</ul>
</details>

**Tags**: `#arXiv`, `#LLM`, `#academic integrity`, `#policy`, `#AI ethics`

---

<a id="item-10"></a>
## [Trump Discusses AI Guardrails and Nvidia H200 with Xi](https://www.bloomberg.com/news/articles/2026-05-15/trump-says-he-discussed-ai-guardrails-nvidia-s-chips-with-xi) ⭐️ 8.0/10

During his visit to China, U.S. President Trump discussed AI guardrails and Nvidia H200 chip exports with President Xi Jinping, noting that China has chosen not to buy the H200 despite U.S. approval. This high-level discussion highlights the ongoing geopolitical tensions over AI chip supply chains, with implications for global AI development and U.S.-China tech competition. The U.S. has allowed Nvidia to supply H200 to Chinese customers, but Beijing has not approved purchases, resulting in zero deliveries so far. China previously rejected the lower-performance H20 chip.

telegram · zaihuapd · May 15, 15:13

**Background**: AI guardrails are safety mechanisms that ensure AI systems operate responsibly and within defined boundaries. The Nvidia H200 is a high-end GPU designed for generative AI and HPC workloads. The discussion also touched on concerns raised by Anthropic's Mythos model, which sparked global cybersecurity alarms.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-guardrails">What are AI guardrails? - IBM</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">H 200 GPU | NVIDIA</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms - The New York Times</a></li>

</ul>
</details>

**Tags**: `#AI`, `#US-China`, `#semiconductors`, `#geopolitics`, `#Nvidia`

---

<a id="item-11"></a>
## [California bill mandates patches or refunds for dead online games](https://arstechnica.com/gaming/2026/05/bill-to-keep-online-games-playable-clears-key-hurdle-in-california/) ⭐️ 7.0/10

A California bill proposes requiring game publishers to either release a patch to make online games playable offline or issue refunds when they shut down servers, with a key committee vote expected soon. This legislation could set a precedent for digital preservation and consumer rights in gaming, potentially forcing publishers to change how they handle end-of-life for online titles and affecting millions of players. The bill exempts games offered solely on a subscription basis, which could push publishers toward subscription models to avoid compliance. It also requires 60-day advance notice before server shutdown.

hackernews · Lihh27 · May 15, 19:48 · [Discussion](https://news.ycombinator.com/item?id=48152994)

**Background**: Many online games become unplayable when servers shut down, even if purchased upfront, because they rely on remote authentication or multiplayer infrastructure. Consumer advocacy groups like Stop Killing Games have pushed for laws requiring offline modes or refunds to protect digital ownership.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stopkillinggames.com/">Stop Killing Games — They Kill Games . We Fight Back.</a></li>
<li><a href="https://gaminghq.eu/2026/03/04/law-offline-mode-digital-games-preservation/">Growing Calls for Laws Requiring Offline Versions of Purchased Games</a></li>

</ul>
</details>

**Discussion**: Commenters are divided: some support open-sourcing server code to let communities run their own servers, while others warn that the bill could increase costs and risk for developers, potentially accelerating the shift to subscription models or making publishers more cautious about launching online games.

**Tags**: `#gaming`, `#legislation`, `#digital preservation`, `#online services`, `#consumer protection`

---

<a id="item-12"></a>
## [Radicle: A Decentralized Code Forge Built on Git](https://radicle.dev/) ⭐️ 7.0/10

Radicle is an open-source, peer-to-peer code collaboration platform built on Git, offering a decentralized alternative to centralized forges like GitHub. It supports both public and private repositories, with private repos visible only to authorized peers. Radicle addresses censorship resistance and user control over data, which are growing concerns in the developer community. Its local-first, peer-to-peer design could reshape how developers collaborate, reducing reliance on centralized services. Private repositories in Radicle are not encrypted at rest but rely on selective replication, meaning they are invisible to the network but could be exposed by a bug or misconfiguration. The project uses a custom license (not AGPL), which some argue could allow SaaS companies to embrace and extend the platform.

hackernews · KolmogorovComp · May 15, 12:07 · [Discussion](https://news.ycombinator.com/item?id=48147603)

**Background**: Traditional code forges like GitHub and GitLab are centralized, meaning a single entity controls access and can impose censorship. Radicle uses a peer-to-peer network where each user retains control over their data and interactions, with cryptographic signatures ensuring authenticity. This approach is part of a broader movement toward decentralized infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://radicle.dev/">Radicle: the sovereign forge</a></li>
<li><a href="https://radicle.dev/guides/protocol">Radicle Protocol Guide</a></li>
<li><a href="https://radicle.dev/guides/user">The Radicle forge is an open source, peer-to-peer code collaboration...</a></li>

</ul>
</details>

**Discussion**: Commenters raised concerns about private repo security, noting that the lack of encryption at rest makes them vulnerable to accidental leaks. Others criticized the non-AGPL license, fearing it could enable SaaS companies to embrace and extend Radicle. Some users praised the local-first design and found it useful for agentic workflows.

**Tags**: `#decentralization`, `#git`, `#code forge`, `#open source`, `#peer-to-peer`

---

<a id="item-13"></a>
## [ChatGPT Android Teardown Reveals Codex Remote Desktop Feature](https://t.me/zaihuapd/41388) ⭐️ 7.0/10

An APK teardown of ChatGPT Android version 1.2026.125 reveals strings indicating OpenAI is developing a remote desktop control feature for Codex, allowing users to find and reconnect to remote sessions from their phone. This feature would enable developers to manage Codex coding sessions remotely from a mobile device, significantly enhancing workflow flexibility and productivity. The feature is still under development with no preview available, and an official release date has not been announced. Users will need to log into the same account on both mobile and desktop.

telegram · zaihuapd · May 14, 21:48

**Background**: Codex is OpenAI's suite of AI-driven coding agents that automate software engineering tasks. Recently, OpenAI brought Codex to the ChatGPT mobile app, and this teardown suggests further integration with remote desktop capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/work-with-codex-from-anywhere/">Work with Codex from anywhere | OpenAI</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2pjcXUtTUVSSEx2bW8yTG4wMUh5Z0FQAQ?hl=en-NG&gl=NG&ceid=NG:en">Google News - OpenAI adds Codex coding tool to ChatGPT mobile...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#Codex`, `#remote desktop`, `#Android`

---

<a id="item-14"></a>
## [China in Talks with Boeing for Up to 500 737 MAX Jets](https://t.me/zaihuapd/41389) ⭐️ 7.0/10

China is negotiating with Boeing to purchase up to 500 737 MAX aircraft, which would be China's first major Boeing order in nearly a decade. The deal is expected to be announced during President Trump's visit to China at the end of this month or early next month. This potential order signals a thaw in US-China trade tensions and could significantly boost Boeing's backlog, especially after the 737 MAX's troubled history. It also underscores China's growing aviation market and its strategic use of aircraft purchases as a diplomatic tool. The deal includes up to 500 737 MAX jets, with additional discussions for about 100 787 and 777X wide-body aircraft that may be announced separately. The agreement is not yet finalized, and the announcement format and binding commitments remain under negotiation.

telegram · zaihuapd · May 15, 01:09

**Background**: The Boeing 737 MAX is a narrow-body aircraft series that was grounded globally from March 2019 to November 2020 after two fatal crashes linked to its MCAS system. China was the first country to ground the MAX and has been slow to approve its return to service, with Chinese airlines only resuming MAX operations in early 2024. The 777X is a long-range wide-body jet with folding wingtips, currently in flight testing and expected to enter service in 2027. The 787 Dreamliner is a composite-structure wide-body aircraft that entered service in 2011.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boeing_737_MAX">Boeing 737 MAX - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_777X">Boeing 777X - Wikipedia Images 777X - The Boeing Company Confirmed: Boeing 777X To Enter Service In 2027 After 7-Year ... Top Stories Lufthansa’s 1st Boeing 777X is now in flight testing Why The Boeing 777X Is Worth Waiting And Waiting And ... - Forbes Boeing 777X Set for 2027 Debut After Costly Delays and ... Boeing 777X: Everything You Need To Know - Dj's Aviation</a></li>
<li><a href="https://en.wikipedia.org/wiki/Boeing_787_Dreamliner">Boeing 787 Dreamliner - Wikipedia Images 787 Dreamliner - The Boeing Company Boeing 787: 5 Things To Know Before Your First Flight On The ... Boeing 787 Overview and Seat Map - Airportix Boeing 787 Seat Map 2026: 106 Layouts from 57+ | Flight Seatmap All About Boeing 787 Dreamliner: Design, Features, Crashes ... Boeing 787 - Aviation Week</a></li>

</ul>
</details>

**Tags**: `#Boeing`, `#China`, `#aviation`, `#trade`, `#737 MAX`

---

<a id="item-15"></a>
## [California Class Action Alleges OpenAI Shared User Data with Meta and Google](https://futurism.com/artificial-intelligence/openai-personal-information-meta-google) ⭐️ 7.0/10

A class-action lawsuit filed in California alleges that OpenAI shared users' chat queries, email addresses, and user IDs with Meta and Google without proper consent, using Meta Pixel and Google Analytics tracking tools. This lawsuit highlights significant privacy concerns regarding how major AI companies handle user data, potentially affecting millions of users and setting a precedent for data sharing practices in the AI industry. The lawsuit claims violations of the California Invasion of Privacy Act and the Electronic Communications Privacy Act, and OpenAI has not yet responded to requests for comment.

telegram · zaihuapd · May 15, 03:45

**Background**: Meta Pixel is a JavaScript tracking code that monitors user actions on websites, while Google Analytics is a web analytics service that tracks and reports website traffic. Both tools are commonly used for advertising and analytics but can transmit personal data to their respective platforms. The California Invasion of Privacy Act prohibits wiretapping and electronic eavesdropping without consent.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Meta_Pixel">Meta Pixel</a></li>
<li><a href="https://en.wikipedia.org/wiki/Google_Analytics">Google Analytics</a></li>
<li><a href="https://taulersmith.com/california-invasion-of-privacy-act">California Invasion of Privacy Act | Tauler Smith LLP</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#lawsuit`, `#OpenAI`, `#data sharing`, `#AI ethics`

---

<a id="item-16"></a>
## [Alipay Responds to 1.84M Yuan Donation After Payment Disabled](https://m.thepaper.cn/newsDetail_forward_33181083) ⭐️ 7.0/10

Alipay stated on May 15, 2026, that it is seeking police assistance after a user reported being charged 1.84 million yuan for charitable donations despite having disabled the payment function three years earlier. This incident raises serious concerns about payment system security and authorization integrity, potentially affecting trust in digital payment platforms and charitable donation mechanisms in China. The user's account was charged six times for donations to the China Foundation for Rural Development, with the largest single donation being 1.84 million yuan. A bank investigation revealed that while general payment functions were disabled, the charitable donation feature remained active.

telegram · zaihuapd · May 15, 07:00

**Background**: Alipay is a leading digital payment platform in China, widely used for online transactions and charitable donations. The China Foundation for Rural Development is a major national charity. The case highlights potential loopholes in payment authorization systems where specific features may remain active even after general functions are disabled.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260515A03G4Y00">支付宝回应关闭支付功能后仍被扣款捐赠184万：不排除涉嫌违法犯罪的可...</a></li>
<li><a href="https://www.163.com/dy/article/KSVGFA460550B6IS.html">支付宝最新回应“关闭支付功能后被扣捐赠184万”：系正常执行支付指令，...</a></li>
<li><a href="https://finance.sina.com.cn/wm/2026-05-15/doc-inhxyccf9379617.shtml">“关闭支付功能后，仍被扣款捐赠184万”，支付宝最新回应：不排除涉嫌违...</a></li>

</ul>
</details>

**Tags**: `#security`, `#payment systems`, `#Alipay`, `#fraud`, `#China`

---

<a id="item-17"></a>
## [Apple-OpenAI Partnership Frays, OpenAI Considers Legal Action](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 7.0/10

Apple and OpenAI's two-year partnership has become strained, with OpenAI accusing Apple of not adequately promoting ChatGPT integration, leading to far lower subscription conversions than expected, and is now exploring legal options including a possible formal notice of breach. This dispute could reshape how AI models are integrated into consumer devices, as Apple plans to open Siri to third-party models like Claude and Gemini in iOS 27, potentially ending ChatGPT's exclusive position and impacting the broader AI ecosystem. OpenAI has hired external lawyers to study legal options and may issue a formal notice of breach soon. Apple is also dissatisfied with OpenAI's privacy standards, hardware business, and engineer poaching, and plans to demonstrate iOS 27's third-party AI model support at WWDC in June.

telegram · zaihuapd · May 15, 12:59

**Background**: Apple and OpenAI announced a partnership in 2024 to integrate ChatGPT into Siri and other Apple Intelligence features. The deal was expected to generate billions in subscription revenue for both companies, but the integration has been criticized for being hidden and limited, with most users still using the standalone ChatGPT app. Apple is now moving to a multi-model strategy with iOS 27, allowing users to choose from various AI assistants.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight">OpenAI - Apple Partnership Frays, Setting Up Possible... - Bloomberg</a></li>
<li><a href="https://techcrunch.com/2026/05/14/openai-is-reportedly-preparing-legal-action-against-apple-it-wouldnt-be-the-first-partner-to-feel-burned/">OpenAI is reportedly preparing legal action against Apple ; it...</a></li>
<li><a href="https://apple.gadgethacks.com/news/ios-27-siri-third-party-ai-assistants-explained-apples-strategy/">iOS 27 Siri Third-Party AI Assistants Explained: Apple's ...</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#OpenAI`, `#AI partnerships`, `#legal dispute`, `#ChatGPT`

---