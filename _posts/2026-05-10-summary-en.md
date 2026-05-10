---
layout: default
title: "Horizon Summary: 2026-05-10 (EN)"
date: 2026-05-10
lang: en
---

> From 35 items, 20 important content pieces were selected

---

1. [Debian mandates reproducible packages for all](#item-1) ⭐️ 9.0/10
2. [Mathematician Tests ChatGPT 5.5 Pro on Research Problems](#item-2) ⭐️ 9.0/10
3. [Bun's Rust rewrite reaches 99.8% test compatibility](#item-3) ⭐️ 8.0/10
4. [Internet Archive Launches Swiss Branch for Resilient Preservation](#item-4) ⭐️ 8.0/10
5. [FreeBSD execve() Local Privilege Escalation Vulnerability](#item-5) ⭐️ 8.0/10
6. [Let-go: A Clojure-like language in Go boots in 7ms](#item-6) ⭐️ 8.0/10
7. [EU Report Labels VPNs a Loophole in Age Verification Laws](#item-7) ⭐️ 8.0/10
8. [LLMs Corrupt Documents When Used as Intermediaries](#item-8) ⭐️ 8.0/10
9. [The Hypocrisy of Cyberlibertarianism](#item-9) ⭐️ 8.0/10
10. [WebRTC's Low-Latency Design Hurts LLM Prompt Accuracy](#item-10) ⭐️ 8.0/10
11. [Using HTML Over Markdown for Claude Prompts](#item-11) ⭐️ 8.0/10
12. [Baidu Releases ERNIE 5.1 with 94% Cost Reduction](#item-12) ⭐️ 8.0/10
13. [Report Exposes Chinese Grey Market for Claude API with Data Theft](#item-13) ⭐️ 8.0/10
14. [Web server in ARM64 assembly for macOS](#item-14) ⭐️ 7.0/10
15. [Apple's macOS distribution frustrates developers](#item-15) ⭐️ 7.0/10
16. [Apple May End TSMC's 12-Year Chip Monopoly](#item-16) ⭐️ 7.0/10
17. [ChatGPT Android APK teardown reveals Codex remote desktop control](#item-17) ⭐️ 7.0/10
18. [Study: Major AI Answers Culturally Biased Toward Japan and US](#item-18) ⭐️ 7.0/10
19. [NASA Advances Rotor Technology for Mars Helicopters](#item-19) ⭐️ 7.0/10
20. [FCC Proposes ID Verification for Phone Number Activation](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Debian mandates reproducible packages for all](https://lists.debian.org/debian-devel-announce/2026/05/msg00001.html) ⭐️ 9.0/10

Debian has announced that all packages in its repository must now be reproducible, meaning the same source code will always produce identical binary packages. This policy change was communicated via a mailing list post in May 2026. This mandate significantly strengthens software supply chain security by ensuring that binaries match their source code, making it much harder for attackers to inject malicious code undetected. It sets a high standard for other Linux distributions and open-source projects to follow. The reproducible builds effort has been a multi-year community project, with Debian's CI now tracking the percentage of packages that build reproducibly. As of the announcement, only a small fraction (estimated 4-5%) of packages still fail to build reproducibly.

hackernews · robalni · May 10, 05:26 · [Discussion](https://news.ycombinator.com/item?id=48081245)

**Background**: Reproducible builds, also known as deterministic compilation, ensure that compiling the same source code with the same build environment always produces bit-for-bit identical binaries. This practice helps verify that distributed binaries are indeed built from the claimed source code, preventing supply chain attacks where binaries are tampered with. Debian has been working toward this goal for many years, and other systems like NetBSD achieved full reproducibility in 2017.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Reproducible_builds">Reproducible builds</a></li>

</ul>
</details>

**Discussion**: The community reaction is overwhelmingly positive, with many praising the achievement as a major milestone for free software. Some commenters noted that the idea was initially dismissed as a waste of time in 2007, highlighting the long journey. Others compared Debian's progress to other systems like NetBSD, which achieved full reproducibility earlier.

**Tags**: `#Debian`, `#reproducible builds`, `#supply chain security`, `#open source`, `#Linux`

---

<a id="item-2"></a>
## [Mathematician Tests ChatGPT 5.5 Pro on Research Problems](https://gowers.wordpress.com/2026/05/08/a-recent-experience-with-chatgpt-5-5-pro/) ⭐️ 9.0/10

Mathematician Timothy Gowers recounts his experience with ChatGPT 5.5 Pro, noting its significantly improved ability to solve gentle research problems and self-correct its reasoning. This advancement could reshape how beginning PhD students are trained, as LLMs can now handle problems previously used as gentle introductions to research, potentially lowering the barrier for idea generation and raising questions about the value of human thinking. Gowers found that ChatGPT 5.5 Pro could solve problems he would give to new PhD students, though it still requires careful guidance and makes mistakes. The model's ability to trace its own reasoning and correct itself is a notable improvement over previous versions.

hackernews · _alternator_ · May 9, 02:41 · [Discussion](https://news.ycombinator.com/item?id=48071262)

**Background**: Large language models (LLMs) like ChatGPT have rapidly improved in reasoning capabilities. ChatGPT 5.5 Pro represents a cutting-edge version that demonstrates enhanced problem-solving in mathematics, a field traditionally considered challenging for AI.

**Discussion**: Commenters noted that while ChatGPT 5.5 Pro is the first LLM they can wrangle into solving tedious problems correctly, it still makes many mistakes and requires rigid guidance. The high cost of token usage was also highlighted as a downside. Some discussed the implications for PhD training and the value of ideas, with physicist John Baez suggesting that if value comes from utility rather than scarcity, automation could be beneficial.

**Tags**: `#AI`, `#LLM`, `#education`, `#research`, `#mathematics`

---

<a id="item-3"></a>
## [Bun's Rust rewrite reaches 99.8% test compatibility](https://twitter.com/jarredsumner/status/2053047748191232310) ⭐️ 8.0/10

Jarred Sumner announced that an experimental Rust rewrite of Bun achieved 99.8% test compatibility on Linux x64 glibc, completed in about 6 days using AI assistance. This milestone demonstrates the potential of AI-assisted porting and could lead to a more stable Bun runtime, addressing long-standing memory safety issues in the original Zig codebase. The rewrite is still experimental and may be discarded; a Bun team member noted that the code does not yet work and there is no commitment to a full rewrite. The port leverages an AI tool called Mythos and unlimited tokens.

hackernews · heldrida · May 9, 10:12 · [Discussion](https://news.ycombinator.com/item?id=48073680)

**Background**: Bun is a fast all-in-one JavaScript runtime written in Zig, known for its speed but also for crashes and memory bugs. Rust is a systems programming language focused on safety and concurrency, often used to replace C/C++ components. AI-assisted porting uses large language models to translate code between languages, which can accelerate rewrites but may introduce risks.

<details><summary>References</summary>
<ul>
<li><a href="https://bun.sh/">Bun — A fast all-in-one JavaScript runtime</a></li>
<li><a href="https://github.com/oven-sh/bun">GitHub - oven-sh/bun: Incredibly fast JavaScript runtime ... Bun Guide: Install, Configure & Deploy the Fast JS Runtime ... Top Stories How to Install Bun - commandlinux.com What Is Bun JS? Ultra-Fast JavaScript Runtime Explained (2025 ... Bun 2026: How the Anthropic Acquisition Reshapes the ...</a></li>
<li><a href="https://linuxfromscratch.org/lfs/view/stable/chapter05/glibc.html">5.5. Glibc -2.42</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some praise the speed of AI-assisted porting, while others express distrust in Bun's direction, citing concerns about AI-generated code quality and the project's stability. A Bun team member clarified that the rewrite is experimental and may be abandoned.

**Tags**: `#Bun`, `#Rust`, `#JavaScript runtime`, `#AI-assisted programming`, `#software engineering`

---

<a id="item-4"></a>
## [Internet Archive Launches Swiss Branch for Resilient Preservation](https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/) ⭐️ 8.0/10

Internet Archive has launched a new independent branch in Switzerland, Internet Archive Switzerland, as a Swiss foundation based in Sankt Gallen, to build a distributed, resilient digital library network alongside existing branches in Canada and Europe. This expansion enhances the resilience of digital preservation by distributing content across multiple jurisdictions, reducing the risk of single-point legal or technical failures, and strengthens the global mission of universal access to knowledge. Internet Archive Switzerland is an independent Swiss foundation, distinct from the US-based Internet Archive, with its own board including Brewster Kahle and Caslon. A UNESCO conference in Paris (November 2026) will explore protection of endangered archives.

hackernews · hggh · May 9, 12:00 · [Discussion](https://news.ycombinator.com/item?id=48074265)

**Background**: Internet Archive is a non-profit digital library founded in 1996, known for the Wayback Machine and archiving web pages, books, and media. It has faced legal challenges and takedown requests, particularly in the US, motivating a distributed approach with independent branches in different countries to ensure content resilience.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.archive.org/2026/05/06/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge/">Internet Archive Switzerland: Expanding a Global Mission to ...</a></li>
<li><a href="https://internetarchive.ch/">Internet Archive Switzerland</a></li>
<li><a href="https://app.daily.dev/posts/internet-archive-switzerland-expanding-a-global-mission-to-preserve-knowledge-rb4murcmr">Internet Archive Switzerland: Expanding a Global Mission...</a></li>

</ul>
</details>

**Discussion**: Commenters suggest that Internet Archive should adopt a Usenet-like model where independent organizations peer and replicate content without sharing takedown requests. Some note that the Swiss site appears to use placeholder text, raising questions about its readiness. Others discuss the degree of independence from the US entity, with past experience at Internet Archive Canada suggesting shared infrastructure despite formal separation.

**Tags**: `#Internet Archive`, `#digital preservation`, `#distributed systems`, `#open access`, `#resilience`

---

<a id="item-5"></a>
## [FreeBSD execve() Local Privilege Escalation Vulnerability](https://www.freebsd.org/security/advisories/FreeBSD-SA-26:13.exec.asc) ⭐️ 8.0/10

FreeBSD released a security advisory (FreeBSD-SA-26:13.exec) for CVE-2026-7270, a local privilege escalation vulnerability in the execve() system call, with a working exploit and write-up published by Ryan of Calif.io. This vulnerability allows any local user to gain full root privileges on a FreeBSD system, posing a severe security risk for servers and desktops running the affected versions. The vulnerability stems from an operator precedence error in the execve() argument handling code, leading to an out-of-bounds write. It affects all supported FreeBSD versions and was patched in 15.0R-p7.

hackernews · Deeg9rie9usi · May 9, 20:31 · [Discussion](https://news.ycombinator.com/item?id=48077971)

**Background**: The execve() system call is a core Unix function that replaces the current process with a new program. It takes arguments (argv) and environment variables (envp) as arrays of strings. A local privilege escalation vulnerability allows an unprivileged user to gain root access, which is critical for multi-user systems.

<details><summary>References</summary>
<ul>
<li><a href="https://www.freebsd.org/security/advisories/FreeBSD-SA-26:13.exec.asc">www.freebsd.org</a></li>
<li><a href="https://news.ycombinator.com/item?id=48077971">Local privilege escalation via execve () | Hacker News</a></li>
<li><a href="https://thecodersblog.com/local-privilege-escalation-via-execve-vulnerability-2026/">Exploiting execve () for Local Privilege Escalation | The ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (156 points, 79 comments) includes insights from the discoverer (Ryan of Calif.io) and notable security researcher tptacek, who praised Calif's work. Commenters also noted the clever CVE name (exeCVE) and the patch timeline.

**Tags**: `#security`, `#FreeBSD`, `#privilege escalation`, `#CVE`, `#exploit`

---

<a id="item-6"></a>
## [Let-go: A Clojure-like language in Go boots in 7ms](https://github.com/nooga/let-go) ⭐️ 8.0/10

Let-go is a Clojure-compatible language (~90% compatible with JVM Clojure) implemented in pure Go, cold booting in ~7ms and shipping as a ~10MB static binary. It includes an nREPL server and is easily embeddable in Go programs. This project offers a fast-starting, embeddable Clojure alternative for CLIs, web servers, and scripting, with startup times 50x faster than JVM Clojure and 3x faster than Babashka. It bridges the gap between Clojure's expressiveness and Go's performance and portability. Under the hood, Let-go uses a handcrafted compiler and stack VM, supporting AOT compilation to portable bytecode and standalone binaries. It does not load JARs or provide full Java API compatibility, so existing Clojure projects may need modifications.

hackernews · marcingas · May 9, 17:52 · [Discussion](https://news.ycombinator.com/item?id=48076815)

**Background**: Clojure is a modern Lisp dialect that runs on the JVM, known for its functional programming features and concurrency support. However, JVM Clojure suffers from slow startup times (often several seconds), which limits its use in scripting and CLI tools. Projects like Babashka and Joker have addressed this by providing fast-starting Clojure interpreters, and Let-go continues this trend with a Go-based implementation.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/nooga/let-go">nooga/let-go: Clojure-esque extension language ...</a></li>
<li><a href="https://news.ycombinator.com/item?id=48076815">Show HN: I made a Clojure-like language in Go, boots in 7ms | Hacker News</a></li>
<li><a href="https://github.com/babashka/babashka">GitHub - babashka/babashka: Native, fast starting Clojure interpreter...</a></li>

</ul>
</details>

**Discussion**: Commenters expressed excitement, with some noting alternatives like Janet, Joker, and Glojure. There was a minor nitpick about inconsistent startup time numbers (7ms vs 6ms), but overall sentiment was positive, praising the project's performance and embeddability.

**Tags**: `#Clojure`, `#Go`, `#programming language`, `#performance`, `#Lisp`

---

<a id="item-7"></a>
## [EU Report Labels VPNs a Loophole in Age Verification Laws](https://cyberinsider.com/eu-calls-vpns-a-loophole-that-needs-closing-in-age-verification-push/) ⭐️ 8.0/10

The European Parliamentary Research Service (EPRS) published a paper suggesting that VPNs may be a loophole in age verification legislation, sparking debate on whether VPNs should also require age verification. This could lead to new EU regulations targeting VPNs, impacting user privacy and internet freedom, while also affecting the growing VPN market driven by age verification laws. The EPRS paper acknowledges that current age-assurance methods are easily bypassed by minors but offers no technical solution to prevent VPN circumvention. Utah became the first U.S. state to target VPN use in age verification laws in March 2025.

hackernews · muse900 · May 9, 05:52 · [Discussion](https://news.ycombinator.com/item?id=48072190)

**Background**: Many countries, including EU member states, have passed or are considering age verification laws for online services to protect minors from harmful content. VPNs allow users to mask their location and bypass such restrictions, creating a loophole that regulators are now examining.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/vpn/eu-research-arm-labels-vpns-a-loophole-as-age-verification-laws-drive-record-adoption">Fears grow that age verification coming to VPNs as... | Tom's Hardware</a></li>
<li><a href="https://www.bbc.com/news/articles/cn438z3ejxyo">Stop children using VPNs to watch porn, ministers told</a></li>
<li><a href="https://en.wikipedia.org/wiki/Social_media_age_verification_laws_by_country">Social media age verification laws by country - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed concerns about privacy and government overreach, with some drawing parallels to China's internet regulations. Others noted the EU's focus on VPNs while ignoring larger fraud issues like the VAT carousel. Some argued the report merely highlights a debate rather than advocating for a ban.

**Tags**: `#VPN`, `#EU policy`, `#privacy`, `#age verification`, `#internet regulation`

---

<a id="item-8"></a>
## [LLMs Corrupt Documents When Used as Intermediaries](https://arxiv.org/abs/2604.15597) ⭐️ 8.0/10

A new paper demonstrates that large language models (LLMs) corrupt documents when used as intermediaries, with each pass degrading the original content. The community has coined the term 'semantic ablation' to describe this algorithmic erosion of high-entropy information. This finding is critical for AI agent design, as it reveals a fundamental limitation of LLMs in tasks requiring faithful document handling. It underscores the risk of 'AI-washing' text, where repeated LLM passes compound degradation, affecting fields like scientific publishing and legal documentation. The paper tested a basic agentic harness with file reading, writing, and code execution tools, but found that tool use did not prevent corruption. Community discussion highlights that LLMs act as 'mean reversion machines,' losing nuance and precision with each pass.

hackernews · rbanffy · May 9, 08:44 · [Discussion](https://news.ycombinator.com/item?id=48073246)

**Background**: Large language models (LLMs) are AI systems trained on vast text data to generate human-like text. When used as intermediaries to process or rewrite documents, they can inadvertently alter content, a phenomenon known as 'semantic ablation'—the algorithmic erosion of high-entropy information. This is analogous to repeatedly saving a JPEG image, where each compression degrades quality.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=47049088">Semantic ablation: Why AI writing is generic and boring - Hacker News</a></li>
<li><a href="https://www.theregister.com/software/2026/02/16/semantic-ablation-why-ai-writing-is-boring-and-dangerous/4414930">Why AI writing is so generic, boring, and dangerous: Semantic ablation</a></li>

</ul>
</details>

**Discussion**: The Hacker News community largely agrees with the paper's findings, with many noting that the degradation is unsurprising and akin to JPEG compression artifacts. Some commenters argue that LLMs should be used as a thin layer for translating intent into deterministic processes, minimizing round trips to avoid corruption.

**Tags**: `#LLM`, `#document corruption`, `#semantic ablation`, `#AI agents`, `#research`

---

<a id="item-9"></a>
## [The Hypocrisy of Cyberlibertarianism](https://matduggan.com/the-intolerable-hypocrisy-of-cyberlibertarianism/) ⭐️ 8.0/10

A critical article by Mat Duggan argues that cyberlibertarian tech leaders abandon their principles when convenient, exposing hypocrisy in the ideology. This critique challenges the foundational beliefs of Silicon Valley and internet governance, prompting reflection on the consistency of tech leaders' political stances. The article references John Perry Barlow's 'Declaration of the Independence of Cyberspace' and notes that many tech figures support regulation when it benefits them.

hackernews · ColinWright · May 9, 13:48 · [Discussion](https://news.ycombinator.com/item?id=48074952)

**Background**: Cyberlibertarianism emerged in the 1990s, advocating minimal government interference in cyberspace. It influenced early internet culture and tech industry politics.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Technolibertarianism">Technolibertarianism - Wikipedia</a></li>
<li><a href="https://en.wiktionary.org/wiki/cyberlibertarianism">cyberlibertarianism - Wiktionary, the free dictionary</a></li>

</ul>
</details>

**Discussion**: Comments show mixed reactions: some agree with the critique, noting personal experiences of hypocrisy, while others defend cyberlibertarian ideals or express distrust in government regulation.

**Tags**: `#cyberlibertarianism`, `#internet governance`, `#tech criticism`, `#politics`

---

<a id="item-10"></a>
## [WebRTC's Low-Latency Design Hurts LLM Prompt Accuracy](https://simonwillison.net/2026/May/9/luke-curley/#atom-everything) ⭐️ 8.0/10

Luke Curley, an engineer at Discord, highlights a fundamental design mismatch: WebRTC aggressively drops audio packets to maintain low latency, which degrades the prompt sent to large language models (LLMs), causing inaccurate responses. He argues that users would prefer a 200ms delay for prompt accuracy over real-time but corrupted audio. This insight reveals a critical flaw in using WebRTC for voice-based LLM interactions, such as OpenAI's Realtime API, where prompt integrity is paramount. As voice AI scales, the industry may need to reconsider transport protocols or implement application-level retransmission to ensure reliable prompt delivery. WebRTC is built on UDP and has no built-in packet retransmission for audio; it uses forward error correction (FEC) and packet loss concealment to mask losses, but these degrade the signal. Curley notes that it is impossible to even retransmit a WebRTC audio packet within a browser, as the implementation is hard-coded for real-time latency.

rss · Simon Willison · May 9, 01:03

**Background**: WebRTC (Web Real-Time Communication) is a standard for peer-to-peer audio/video communication in browsers, designed for low-latency applications like video conferencing. It prioritizes real-time interaction over reliability, using techniques like packet dropping to avoid delays. Large language models (LLMs) require accurate, complete prompts to generate correct responses; corrupted audio can lead to misinterpretation and poor output.

<details><summary>References</summary>
<ul>
<li><a href="http://www.rtcbits.com/2017/03/retransmissions-in-webrtc.html">How are retransmissions implemented in WebRTC</a></li>
<li><a href="https://webrtcforthecurious.com/docs/06-media-communication/">Media Communication | WebRTC for the Curious</a></li>
<li><a href="https://getstream.io/resources/projects/webrtc/advanced/media-resilience/">Media Resilience in WebRTC - GetStream.io</a></li>

</ul>
</details>

**Tags**: `#WebRTC`, `#LLM`, `#audio`, `#real-time`, `#latency`

---

<a id="item-11"></a>
## [Using HTML Over Markdown for Claude Prompts](https://simonwillison.net/2026/May/8/unreasonable-effectiveness-of-html/#atom-everything) ⭐️ 8.0/10

Thariq Shihipar, a member of the Claude Code team at Anthropic, advocates for using HTML instead of Markdown as the output format when prompting Claude, citing richer structure and better rendering for complex tasks like code review. This insight could shift how developers interact with LLMs, enabling more interactive and visually rich outputs—such as SVG diagrams and inline annotations—that improve comprehension and productivity. The article includes example prompts, such as asking Claude to review a PR with HTML artifacts containing inline margin annotations and color-coded findings. The author also demonstrates using GPT-5.5 to generate an interactive HTML explanation of a Linux exploit.

rss · Simon Willison · May 8, 21:00

**Background**: Markdown has been the default output format for LLMs due to its token efficiency, especially during the GPT-4 era with 8,192 token limits. HTML, while more verbose, allows embedding SVG diagrams, interactive widgets, and in-page navigation, making explanations richer and more navigable.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://code.claude.com/docs/en/overview">Claude Code overview - Claude Code Docs</a></li>
<li><a href="https://www.librechat.ai/docs/features/artifacts">Artifacts - Generative UI | LibreChat</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#prompt engineering`, `#HTML`, `#Claude`, `#AI-assisted development`

---

<a id="item-12"></a>
## [Baidu Releases ERNIE 5.1 with 94% Cost Reduction](https://mp.weixin.qq.com/s/_I9ziafHheXiJpA-QY2F7A) ⭐️ 8.0/10

Baidu has launched ERNIE 5.1, a new large language model that uses 'multi-dimensional elastic pre-training' to achieve leading performance at only 6% of the pre-training cost of comparable models. The model ranks first in China and fourth globally on the LMArena search leaderboard with a score of 1223. This release demonstrates a significant breakthrough in cost-efficient AI training, potentially lowering barriers for enterprise adoption of large models. ERNIE 5.1's strong performance in search and agent tasks positions Baidu as a competitive player in the global AI landscape, challenging models from DeepSeek and Gemini. Baidu claims ERNIE 5.1's agent capabilities surpass DeepSeek-V4-Pro, its creative writing is on par with Gemini 3.1 Pro, and its reasoning approaches leading closed-source models. The model is available on Baidu's Qianfan model plaza and Wenxin Yiyan website for enterprise users and developers.

telegram · zaihuapd · May 9, 07:45

**Background**: Large language models typically require massive computational resources for pre-training, making them expensive to develop. Baidu's 'multi-dimensional elastic pre-training' technique aims to reduce this cost while maintaining or improving performance. The LMArena search leaderboard evaluates models on real-time information retrieval and grounded citation tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/948/079.htm">百度发布文心大模型 5.1：搜索能力位居国内首位，预训练成本仅为业界 ...</a></li>
<li><a href="https://www.itbear.com.cn/html/2026-05/1331691.html">百度文心大模型5.1发布：多维弹性预训练加持，搜索能力登顶国内榜首-...</a></li>
<li><a href="https://www.techmami.com/flashdetail/072c0409e21d42a1b3fde159a6a2a582JJPZ9PEEcN">百度文心大模型5.1正式发布！多维弹性预训练技术上线即用 - 科技妈咪...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#Baidu`, `#ERNIE`, `#NLP`

---

<a id="item-13"></a>
## [Report Exposes Chinese Grey Market for Claude API with Data Theft](https://www.tomshardware.com/tech-industry/artificial-intelligence/chinese-grey-market-sells-claude-api-access-at-90-percent-off-through-proxy-networks-that-harvest-user-data) ⭐️ 8.0/10

A report reveals that Chinese grey market proxy services, known as 'transfer stations,' resell Anthropic's Claude API access at up to 90% off official prices, using stolen credentials, model substitution, and harvesting user prompts and outputs for resale as AI training data. This exposes significant security and intellectual property risks for developers and companies using these proxies, as their code and proprietary data can be stolen and used for model distillation, undermining trust in AI API ecosystems. The report, by Oxford China Policy Lab researcher Zilan Qian and covered by Tom's Hardware, documents that these proxy networks operate on platforms like GitHub and Taobao, and often substitute cheaper models (including domestic Chinese models) for Claude Opus.

telegram · zaihuapd · May 10, 01:48

**Background**: Anthropic's Claude models are advanced AI assistants, but direct API access can be expensive or restricted in certain regions. Grey-market proxies exploit this demand by offering discounted access, but they often engage in fraudulent practices like model swapping and data harvesting. Model distillation is a technique where outputs from a large model are used to train smaller, cheaper models, which is a common goal for these data thieves.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/chinese-grey-market-sells-claude-api-access-at-90-percent-off-through-proxy-networks-that-harvest-user-data">Chinese grey market sells Claude API access at 90% off by ...</a></li>
<li><a href="https://letsdatascience.com/news/grey-market-proxies-resell-claude-api-access-at-discount-7a0032fe">Grey-market proxies resell Claude API access at discount</a></li>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Claude`, `#API security`, `#grey market`, `#data theft`, `#AI`

---

<a id="item-14"></a>
## [Web server in ARM64 assembly for macOS](https://github.com/imtomt/ymawky) ⭐️ 7.0/10

A developer created ymawky, a static file web server for macOS written entirely in ARM64 assembly, supporting GET, PUT, DELETE, HEAD, OPTIONS, range requests, directory listing, and slowloris mitigations. This project demonstrates deep low-level programming skill and serves as a nostalgic reminder of craftsmanship in an era increasingly dominated by AI-assisted coding. The server decodes percent-encoded URLs, enforces docroot strictly, serves custom error pages, and includes some mitigations against slowloris attacks. It also supports byte range requests for video streaming.

hackernews · imtomt · May 10, 03:01 · [Discussion](https://news.ycombinator.com/item?id=48080587)

**Background**: Assembly language is a low-level programming language that directly corresponds to machine instructions. ARM64 is the 64-bit instruction set architecture used in modern Apple Silicon Macs. Writing a functional web server in assembly is rare and requires deep understanding of system calls and hardware.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Assembly_language">Assembly language - Wikipedia</a></li>
<li><a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Range_requests">HTTP range requests - HTTP | MDN</a></li>
<li><a href="https://en.wikipedia.org/wiki/Slowloris_(cyber_attack)">Slowloris (cyber attack ) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed nostalgia for the era when such craftsmanship was rewarded, with some mourning the shift toward AI-generated code. Others noted that while assembly is verbose, it is not fundamentally different from higher-level programming once you master abstractions.

**Tags**: `#assembly`, `#web server`, `#ARM64`, `#macOS`, `#low-level programming`

---

<a id="item-15"></a>
## [Apple's macOS distribution frustrates developers](https://blog.kronis.dev/blog/apple-is-increasing-my-cortisol-levels) ⭐️ 7.0/10

A developer detailed frustrations with Apple's increasingly complex macOS software distribution process, including Gatekeeper, notarization, and poor documentation, sparking widespread community discussion. This highlights a persistent pain point for macOS developers, potentially discouraging indie development and pushing developers toward other platforms, which could reduce the diversity of Mac software. The author noted that Apple's notarization process requires an annual $99 developer fee and a D-U-N-S number, and that documentation is often outdated or incomplete, forcing developers to reverse-engineer solutions.

hackernews · LorenDB · May 9, 14:40 · [Discussion](https://news.ycombinator.com/item?id=48075366)

**Background**: Gatekeeper is a macOS security feature that verifies downloaded apps are signed and notarized by Apple before running. Notarization is an automated system that scans apps for malicious content and code-signing issues. Developers must navigate these steps to distribute software outside the Mac App Store.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hexnode.com/blogs/mac-notarization-everything-mac-admins-need-to-know/">Mac notarization : Everything Mac admins need to know</a></li>
<li><a href="https://developer.apple.com/documentation/security/notarizing-macos-software-before-distribution?language=objc">Notarizing macOS software before distribution | Apple Developer ...</a></li>
<li><a href="https://gist.github.com/Jolg42/201f75a3699f5742a9605170dc50bfbc">Code Signing on macOS and Windows + Apple Notarization · GitHub</a></li>

</ul>
</details>

**Discussion**: Commenters expressed sympathy and shared workarounds, such as disabling Gatekeeper via terminal or using third-party guides. Some criticized Apple's backward compatibility and high costs, while others noted that Windows code signing is similarly expensive.

**Tags**: `#macOS`, `#developer experience`, `#software distribution`, `#Apple`, `#Gatekeeper`

---

<a id="item-16"></a>
## [Apple May End TSMC's 12-Year Chip Monopoly](https://t.me/zaihuapd/41292) ⭐️ 7.0/10

Apple is reportedly considering ending TSMC's exclusive chip manufacturing deal since 2014, and may use Intel's 18A process for some Mac, iPad, or iPhone chips as early as 2027. This move would diversify Apple's supply chain, reducing reliance on TSMC amid capacity constraints from AI chip demand, and could reshape the semiconductor foundry landscape by boosting Intel's foundry business. Intel's role would be limited to manufacturing, not chip design. The 18A process (1.8nm equivalent) combines RibbonFET transistors and PowerVia architecture, targeting mobile applications with optimized power efficiency.

telegram · zaihuapd · May 8, 17:18

**Background**: Since 2014, Apple has relied exclusively on TSMC for manufacturing its custom chips (A-series and M-series). TSMC's advanced nodes (e.g., 3nm) have been critical for Apple's performance leadership. However, surging demand from AI companies like Nvidia has strained TSMC's capacity, prompting Apple to seek alternatives. Intel's 18A process is a next-generation node that Intel hopes will revive its foundry business.

<details><summary>References</summary>
<ul>
<li><a href="https://www.intel.com/content/www/us/en/foundry/process/18a.html">Intel 18A | See Our Biggest Process Innovation</a></li>
<li><a href="https://9to5mac.com/2026/05/04/report-apple-considers-intel-and-samsung-to-diversify-chip-manufacturing-away-from-tsmc/">Apple considers Intel and Samsung to diversify chip ...</a></li>
<li><a href="https://www.cultofmac.com/news/apple-looks-beyond-tsmc-make-iphone-mac-chips">Apple looks beyond TSMC to make iPhone and Mac chips</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#TSMC`, `#Intel`, `#chip manufacturing`, `#supply chain`

---

<a id="item-17"></a>
## [ChatGPT Android APK teardown reveals Codex remote desktop control](https://www.androidauthority.com/codex-smartphone-control-3665256/) ⭐️ 7.0/10

An APK teardown of ChatGPT Android version 1.2026.125 reveals strings indicating OpenAI is developing a remote desktop control feature for Codex, allowing users to find and reconnect to remote sessions from their phone. This feature would enable developers to control their Codex-powered desktop environment from a mobile device, significantly enhancing productivity and flexibility for remote work. The feature is still under development with no preview available, and requires the desktop to be logged into the same account. The official release date has not been announced.

telegram · zaihuapd · May 9, 02:18

**Background**: Codex is an AI coding assistant from OpenAI that can operate a user's computer, edit files, and run commands. Remote connections allow Codex to work with projects on SSH-accessible machines. This mobile feature would extend that capability to smartphone control.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/codex/remote-connections">Remote connections – Codex | OpenAI Developers</a></li>
<li><a href="https://openai.com/index/codex-for-almost-everything/">Codex for (almost) everything - OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#Android`, `#remote desktop`, `#AI`

---

<a id="item-18"></a>
## [Study: Major AI Answers Culturally Biased Toward Japan and US](https://cybernews.com/ai-news/every-ai-answer-japan/) ⭐️ 7.0/10

A study by the University of the Basque Country and Cardiff University analyzed 31,680 cultural questions across 8 major AI models in 24 languages, finding that answers are often anchored to Japanese or American cultural norms. This reveals a significant cultural bias in widely used AI models, which could perpetuate cultural dominance and undermine fairness for users from other regions. The bias primarily emerges during supervised fine-tuning, not in the base models; low-resource languages are more likely to produce answers aligned with the user's own country.

telegram · zaihuapd · May 9, 10:02

**Background**: Large language models (LLMs) are trained on vast text data that often overrepresents certain cultures, especially English-speaking and East Asian contexts. Supervised fine-tuning (SFT) is a process where models are further trained on labeled examples to improve task performance, but it can amplify existing biases if the training data is not culturally diverse.

<details><summary>References</summary>
<ul>
<li><a href="https://academic.oup.com/pnasnexus/article/3/9/pgae346/7756548">Cultural bias and cultural alignment of large language models | PNAS Nexus | Oxford Academic</a></li>
<li><a href="https://aiwiki.ai/wiki/Supervised_fine-tuning">Supervised fine - tuning - AI Wiki - Artificial Intelligence Wiki</a></li>

</ul>
</details>

**Tags**: `#AI bias`, `#cultural bias`, `#large language models`, `#fairness`

---

<a id="item-19"></a>
## [NASA Advances Rotor Technology for Mars Helicopters](https://arstechnica.com/space/2026/05/engineers-at-nasas-jet-propulsion-lab-make-a-breakthrough-in-rotor-technology/) ⭐️ 7.0/10

NASA JPL engineers have achieved a breakthrough in rotor technology, enabling rotor blades to reach supersonic speeds (beyond Mach 1) in simulated Martian atmospheric conditions without breaking apart. This breakthrough allows next-generation Mars helicopters to carry heavier payloads and fly farther, expanding the scope of aerial exploration on Mars beyond the capabilities of the Ingenuity helicopter. The tests, conducted in a special chamber simulating Mars conditions, involved 137 runs where the rotor tips exceeded Mach 1, surpassing the previous limit of 2,700 rpm used for Ingenuity.

telegram · zaihuapd · May 9, 14:21

**Background**: Mars has a very thin atmosphere (about 1% of Earth's), making it difficult for rotorcraft to generate lift. NASA's Ingenuity helicopter, which completed 72 flights, was limited in payload and flight duration due to these conditions. The new rotor technology aims to overcome these limitations by allowing higher rotational speeds and improved efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nasa.gov/solar-system/planets/mars/nasa-pushes-next-gen-mars-helicopter-rotor-blades-past-mach-1/">NASA Pushes Next-Gen Mars Helicopter Rotor Blades Past Mach 1 - NASA</a></li>
<li><a href="https://science.nasa.gov/photojournal/nasas-next-gen-mars-helicopter-rotors-are-moving-fast/">NASA’s Next-Gen Mars Helicopter Rotors Are Moving Fast - NASA Science</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ingenuity_(helicopter)">Ingenuity (helicopter) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#NASA`, `#rotor technology`, `#Mars exploration`, `#aerospace engineering`

---

<a id="item-20"></a>
## [FCC Proposes ID Verification for Phone Number Activation](https://reclaimthenet.org/the-fcc-wants-your-id-before-you-get-a-phone-number) ⭐️ 7.0/10

The U.S. Federal Communications Commission (FCC) unanimously approved a proposal requiring telecom providers to verify a customer's identity before activating phone service, including traditional, mobile, and VoIP services. The proposal aims to combat illegal robocalls and may require providers to retain identity records for at least four years after service ends. If enacted, this rule would eliminate the ability to obtain prepaid phones and SIM cards anonymously with cash, affecting privacy advocates and individuals who rely on anonymous communication. It represents a significant shift in U.S. telecom regulation, balancing anti-spam efforts against privacy concerns. The proposal requires government-issued ID, legal name, address, and existing phone number for activation, and may also require checking law enforcement watchlists. The FCC is still seeking public comment on the specifics, and the rule would apply to traditional carriers, mobile operators, and VoIP providers.

telegram · zaihuapd · May 10, 04:12

**Background**: VoIP (Voice over Internet Protocol) is a technology that enables voice calls over the internet, commonly used by services like Skype and Zoom. Prepaid phones and SIM cards have long been available for cash purchase without identity verification, allowing semi-anonymous communication. The FCC's proposal targets illegal robocalls, which have been a persistent nuisance and fraud vector in the U.S.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/VoIP_phone">VoIP phone</a></li>
<li><a href="https://zh.wikipedia.org/wiki/VoIP">VoIP - 维基百科，自由的百科全书</a></li>

</ul>
</details>

**Tags**: `#FCC`, `#telecom regulation`, `#privacy`, `#anti-spam`, `#identity verification`

---