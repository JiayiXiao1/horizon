---
layout: default
title: "Horizon Summary: 2026-05-24 (EN)"
date: 2026-05-24
lang: en
---

> From 31 items, 16 important content pieces were selected

---

1. [80386 Microcode Disassembled and Analyzed](#item-1) ⭐️ 9.0/10
2. [Anthropic's Project Glasswing: AI Finds 10K+ Critical Vulnerabilities](#item-2) ⭐️ 9.0/10
3. [Apple Open-Sources corecrypto with Formal Verification for Quantum-Safe Algorithms](#item-3) ⭐️ 9.0/10
4. [Microsoft reveals OpenAI's $115B quarterly loss](#item-4) ⭐️ 9.0/10
5. [Trump admin ends adjustment of status for most green card seekers](#item-5) ⭐️ 8.0/10
6. [SpaceX Launches Starship V3 in First Test Flight](#item-6) ⭐️ 8.0/10
7. [Deep Learning Optimization from First Principles](#item-7) ⭐️ 8.0/10
8. [AI memory demand drives up consumer electronics prices](#item-8) ⭐️ 8.0/10
9. [China Cracks Down on Illegal Cross-Border Securities Trading](#item-9) ⭐️ 8.0/10
10. [Cloudflare 25-Minute Outage Hits 28% of HTTP Traffic](#item-10) ⭐️ 8.0/10
11. [Microsoft Widely Deploys Claude Code, Urges Non-Tech Staff to Use AI Coding](#item-11) ⭐️ 8.0/10
12. [Corsair Adopts CXMT Chips, DDR5 Prices May Drop](#item-12) ⭐️ 8.0/10
13. [Critique of HTML <dl> Element Sparks Debate on Semantic HTML](#item-13) ⭐️ 7.0/10
14. [FTC Fines Cox Media Group for Fake AI 'Active Listening' Ads](#item-14) ⭐️ 7.0/10
15. [Tencent's Ximalaya Acquisition Approved with Conditions](#item-15) ⭐️ 7.0/10
16. [China's Daily Token Calls Surge 1000x in Two Years, Exceed 140 Trillion](#item-16) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [80386 Microcode Disassembled and Analyzed](https://www.reenigne.org/blog/80386-microcode-disassembled/) ⭐️ 9.0/10

Reenigne has published a detailed disassembly and analysis of the 80386's microcode, based on a high-resolution image of the microcode ROM provided by Ken Shirriff. This reverse engineering effort reveals how the 80386 implemented complex x86 instructions at the microarchitectural level, providing invaluable insight for retrocomputing enthusiasts and CPU architecture researchers. The disassembly covers the entire microcode ROM, documenting the micro-operations that execute instructions like MOV, ADD, and memory segmentation. The work builds on reenigne's earlier 8086 microcode disassembly.

hackernews · nand2mario · May 23, 12:11 · [Discussion](https://news.ycombinator.com/item?id=48247004)

**Background**: Microcode is a layer of low-level instructions that control the internal hardware of a CPU, translating complex machine instructions into simpler micro-operations. The 80386, released in 1985, was Intel's first 32-bit x86 processor and a landmark in CPU design. Reverse engineering its microcode helps demystify how classic processors worked internally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.reenigne.org/blog/80386-microcode-disassembled/">80386 Microcode Disassembled - Reenigne blog</a></li>
<li><a href="https://nand2mario.github.io/posts/2026/z386/">z386: An Open-Source 80386 Built Around Original Microcode</a></li>
<li><a href="https://en.wikipedia.org/wiki/Microarchitecture">Microarchitecture - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The Hacker News community expressed fascination and appreciation for the reverse engineering work. Comments included technical questions about the process of extracting microcode from die images, references to related projects like the open-source z386, and recommendations for further reading on microprogramming.

**Tags**: `#reverse engineering`, `#microcode`, `#80386`, `#CPU architecture`, `#retrocomputing`

---

<a id="item-2"></a>
## [Anthropic's Project Glasswing: AI Finds 10K+ Critical Vulnerabilities](https://www.anthropic.com/research/glasswing-initial-update) ⭐️ 9.0/10

Anthropic announced initial results from Project Glasswing, where its Claude Mythos Preview model identified over 10,000 high-severity vulnerabilities in one month across critical software and thousands of open-source projects, with a 90.6% true positive rate among reviewed findings. This demonstrates that AI can now discover vulnerabilities at a scale and speed far beyond human capability, shifting the bottleneck from discovery to verification and patching, which has significant implications for software security and the open-source ecosystem. The model scanned thousands of open-source projects, finding 6,202 high-severity vulnerabilities, with 90.6% true positive rate among 1,752 reviewed. Partners like Cloudflare reported a 10x improvement in vulnerability discovery speed.

telegram · zaihuapd · May 23, 03:16

**Background**: Project Glasswing is an industry-wide cybersecurity initiative by Anthropic, launched alongside the gated preview of Claude Mythos Preview, a general-purpose frontier model not available to the public. The model can autonomously identify and exploit vulnerabilities, raising both security benefits and concerns.

<details><summary>References</summary>
<ul>
<li><a href="https://www.helpnetsecurity.com/2026/04/08/anthropic-claude-mythos-preview-identify-vulnerabilities/">Anthropic's new AI model finds and exploits... - Help Net Security</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/anthropics-latest-ai-model-identifies-thousands-of-zero-day-vulnerabilities-in-every-major-operating-system-and-every-major-web-browser-claude-mythos-preview-sparks-race-to-fix-critical-bugs-some-unpatched-for-decades">Anthropic's latest AI model identifies 'thousands of... | Tom's H...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability discovery`, `#Anthropic`, `#open source`

---

<a id="item-3"></a>
## [Apple Open-Sources corecrypto with Formal Verification for Quantum-Safe Algorithms](https://security.apple.com/blog/formal-verification-corecrypto/) ⭐️ 9.0/10

Apple has open-sourced its corecrypto library, including implementations of the quantum-safe algorithms ML-KEM and ML-DSA, along with end-to-end formal verification proofs that mathematically guarantee correctness against the NIST standards. This is a major milestone for cryptographic assurance, as formal verification provides the highest level of confidence in the correctness of code that will run on over 2.5 billion active Apple devices, protecting future communications against quantum computer attacks. The formal proofs cover both C code and hand-optimized ARM64 assembly, and Apple has also released its custom verification tools and Isabelle theory libraries for independent evaluation.

telegram · zaihuapd · May 23, 04:49

**Background**: ML-KEM (formerly Kyber) and ML-DSA (formerly Dilithium) are post-quantum cryptographic algorithms standardized by NIST in 2024, designed to resist attacks from future quantum computers. Formal verification uses mathematical proofs to ensure that software implementations exactly match their specifications, eliminating entire classes of bugs. Apple's corecrypto library provides fundamental cryptographic operations for iOS, macOS, and other Apple platforms.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Kyber">ML - KEM - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Isabelle_(proof_assistant)">Isabelle (proof assistant) - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#cryptography`, `#formal verification`, `#quantum-safe`, `#open source`, `#Apple`

---

<a id="item-4"></a>
## [Microsoft reveals OpenAI's $115B quarterly loss](https://t.me/zaihuapd/41537) ⭐️ 9.0/10

Microsoft's latest earnings report inadvertently disclosed that OpenAI suffered a net loss of approximately $115 billion in a single quarter, based on Microsoft's equity method investment accounting. This loss is nearly three times OpenAI's $4.3 billion revenue in the first half of 2025. This disclosure highlights the extreme capital intensity of leading AI research, raising questions about the financial sustainability of frontier AI development. It also underscores the significant financial risk for major investors like Microsoft, which has already committed $13 billion to OpenAI. Microsoft holds approximately 27% of OpenAI's equity, and the $115 billion loss is derived from a $3.1 billion reduction in Microsoft's net income due to equity method losses. If calculated based on pre-tax losses and Microsoft's actual 32.5% stake, the loss could exceed $120 billion.

telegram · zaihuapd · May 23, 07:40

**Background**: Equity method accounting requires investors to recognize their share of the investee's profits or losses. OpenAI's massive losses are driven by enormous capital expenditures on computing infrastructure, including GPU clusters, to maintain its lead in large language model development. The company's revenue from subscriptions and API services has not kept pace with these costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.qbitai.com/2025/11/347840.html">微软独家：OpenAI最新季度净亏损115亿美元</a></li>
<li><a href="https://www.zhihu.com/question/1967900167182181978">媒体曝 OpenAI 单季度亏损 120 亿美元，具体情况如何？目前 OpenAI 发展面临哪些问题？ - 知乎</a></li>
<li><a href="https://www.ifanr.com/1653377">OpenAI 再不上市，财务窟窿就要把巨头们拖垮了 | 爱范儿</a></li>

</ul>
</details>

**Discussion**: Community comments on platforms like Zhihu express shock at the loss magnitude, with many noting that OpenAI's spending is unsustainable and questioning the long-term viability of the current AI investment model. Some commenters suggest that OpenAI may need to go public or seek additional funding to cover its cash burn.

**Tags**: `#OpenAI`, `#Microsoft`, `#AI Economics`, `#Financial Disclosure`, `#Artificial Intelligence`

---

<a id="item-5"></a>
## [Trump admin ends adjustment of status for most green card seekers](https://www.nytimes.com/2026/05/22/us/politics/green-card-changes-trump.html) ⭐️ 8.0/10

On May 22, 2026, the Trump administration announced that most green card applicants must leave the U.S. and apply through consular processing abroad, ending the practice of adjusting status from within the country except in extraordinary circumstances. This policy dramatically disrupts the lives of hundreds of thousands of legal immigrants, especially H-1B tech workers, who now face prolonged separation from families and jobs, potentially driving talent away from the U.S. tech industry. The USCIS memo (PM-602-0199) specifies that adjustment of status will only be granted in extraordinary circumstances, effectively requiring most applicants to use consular processing, which can involve multi-year waits at U.S. embassies abroad.

hackernews · tlhunter · May 22, 21:27 · [Discussion](https://news.ycombinator.com/item?id=48241890)

**Background**: Adjustment of status (AOS) has long allowed immigrants already in the U.S. on temporary visas to apply for a green card without leaving the country. Consular processing, the alternative, requires applicants to return to their home country or a third country for an interview at a U.S. embassy or consulate. This change reverses decades of standard practice and adds significant uncertainty and hardship for applicants.

<details><summary>References</summary>
<ul>
<li><a href="https://www.uscis.gov/newsroom/news-releases/us-citizenship-and-immigration-services-will-grant-adjustment-of-status-only-in-extraordinary">U.S. Citizenship and Immigration Services Will Grant ‘Adjustment of Status’ Only in Extraordinary Circumstances | USCIS</a></li>

</ul>
</details>

**Discussion**: Commenters expressed shock and anger, calling the policy insane and reckless. Many highlighted practical nightmares: U.S.-born children needing visas to leave, multi-year consulate backlogs, and the risk of being stranded abroad. Some who recently obtained green cards felt relief but also fear for future citizenship applications.

**Tags**: `#immigration`, `#US policy`, `#tech workers`, `#green card`, `#H-1B`

---

<a id="item-6"></a>
## [SpaceX Launches Starship V3 in First Test Flight](https://www.space.com/space-exploration/launches-spacecraft/spacex-starship-v3-megarocket-first-test-flight) ⭐️ 8.0/10

SpaceX launched the first Starship V3 prototype on May 22, 2026, from its Starbase facility in Texas. The upper stage successfully landed on target, but the Super Heavy booster experienced engine failures during return and the ship's engine bay showed signs of damage. This test flight marks a critical milestone in SpaceX's iterative development of the world's most powerful rocket, bringing it closer to full reusability and operational capability. The successful ship landing and improved heat shield performance demonstrate significant progress, while the booster issues highlight remaining challenges. During ascent, one engine on the Super Heavy booster shut down prematurely. The booster's boost-back burn failed, and its landing burn resulted in a hard splashdown off target. The Starship upper stage lost one engine shortly after stage separation, with visible red glow and venting in the engine bay, yet still landed precisely on target.

hackernews · busymom0 · May 22, 23:41 · [Discussion](https://news.ycombinator.com/item?id=48242959)

**Background**: Starship is a two-stage, fully reusable super heavy-lift launch vehicle being developed by SpaceX. It consists of the Super Heavy booster and the Starship spacecraft, both powered by Raptor engines burning liquid methane and liquid oxygen. The V3 version is larger and more powerful than previous iterations, designed to eventually carry crew and cargo to the Moon, Mars, and beyond.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Starship_prototypes">Starship prototypes</a></li>
<li><a href="https://en.wikipedia.org/wiki/SpaceX_Starship">SpaceX Starship - Wikipedia</a></li>
<li><a href="https://arstechnica.com/space/2026/05/spacexs-starship-v3-still-a-work-in-progress-mostly-successful-on-first-flight/">SpaceX's Starship V3—still a work in progress—mostly... - Ars Technica</a></li>

</ul>
</details>

**Discussion**: Community comments praised the successful ship landing and heat shield improvements, with one user noting no visible hot spots during reentry. However, there was disappointment over the booster's failure to complete its return, and some expressed concern about the engine bay damage. Overall, the sentiment was positive, appreciating SpaceX's rapid iteration approach.

**Tags**: `#SpaceX`, `#Starship`, `#rocket launch`, `#space exploration`, `#engineering`

---

<a id="item-7"></a>
## [Deep Learning Optimization from First Principles](https://horace.io/brrr_intro.html) ⭐️ 8.0/10

A comprehensive blog post explains how to optimize deep learning systems for maximum hardware utilization by breaking down efficiency into compute, memory, and overhead components. This post provides a foundational understanding that helps practitioners identify bottlenecks and apply targeted optimizations, which is critical as deep learning models grow in size and complexity. The post uses a first-principles approach, illustrating that in the time Python performs one FLOP, an A100 GPU could have executed 9.75 million FLOPs, highlighting the massive gap between high-level code and hardware capability.

hackernews · tosh · May 23, 11:50 · [Discussion](https://news.ycombinator.com/item?id=48246889)

**Background**: Deep learning training and inference often suffer from low hardware utilization due to overhead from Python, data movement, and suboptimal kernel configurations. Understanding the three regimes—compute-bound, memory-bound, and overhead-bound—enables developers to prioritize the most impactful optimizations.

<details><summary>References</summary>
<ul>
<li><a href="https://horace.io/brrr_intro.html">Making Deep Learning go Brrrr From First Principles</a></li>

</ul>
</details>

**Discussion**: Commenters praised the post as a classic and highlighted NVIDIA's sustained lead in TFLOPs, bandwidth, and interconnect. Others noted the complexity of performance portability, where models behave differently across runtimes and hardware, and expressed interest in failure modes for production systems.

**Tags**: `#deep learning`, `#performance optimization`, `#NVIDIA`, `#ML systems`, `#GPU computing`

---

<a id="item-8"></a>
## [AI memory demand drives up consumer electronics prices](https://simonwillison.net/2026/May/22/memory-shortage/#atom-everything) ⭐️ 8.0/10

Memory manufacturers are reallocating wafer capacity from DDR and LPDDR to HBM for AI data centers, causing a shortage of consumer memory and price increases, especially in sub-$100 smartphones. This shift means consumer electronics like smartphones, laptops, and gaming consoles will become more expensive for years, disproportionately affecting low-income markets in Africa and South Asia. HBM consumes over three times the wafer capacity per gigabyte compared to DDR or LPDDR, and its allocation is expected to rise from 2% to 20% by end of 2026. Memory companies deliberately under-provision capacity to maintain profits.

rss · Simon Willison · May 22, 22:01

**Background**: DRAM memory comes in three main types: DDR (used in desktops/servers), LPDDR (mobile/low-power devices), and HBM (high-bandwidth memory for GPUs). All are manufactured on the same wafer fabrication lines, so increasing HBM output reduces capacity for other types. The memory industry is dominated by just three companies (Samsung, SK Hynix, Micron), which have learned to avoid over-investment after past boom-bust cycles.

<details><summary>References</summary>
<ul>
<li><a href="https://semiwiki.com/wikis/semiconductor-ip-wikis/ddr-vs-lpddr-vs-hbm-wiki/">DDR vs. LPDDR vs. HBM Wiki - SemiWiki</a></li>

</ul>
</details>

**Tags**: `#memory`, `#AI`, `#hardware`, `#market analysis`, `#supply chain`

---

<a id="item-9"></a>
## [China Cracks Down on Illegal Cross-Border Securities Trading](https://t.me/zaihuapd/41525) ⭐️ 8.0/10

China's eight ministries jointly issued a plan to crack down on illegal cross-border securities, futures, and fund operations, allowing only existing investors to sell and withdraw funds over a two-year cleanup period. The CSRC has initiated investigations into Tiger Brokers, Futu Holdings, and Changqiao for illegal cross-border operations. This crackdown signals a major regulatory tightening on cross-border securities trading, affecting millions of Chinese investors using offshore platforms. It could reshape the fintech landscape and force platforms to comply or exit the Chinese market. Futu Holdings faces a proposed fine of 18.5 billion yuan, and Tiger Securities subsidiaries are fined about 4.11 billion yuan. The plan targets not only offshore platforms but also domestic partners, intermediaries, and information platforms that facilitate illegal cross-border operations.

telegram · zaihuapd · May 22, 13:55

**Background**: Many Chinese investors use offshore brokerages like Futu and Tiger to trade Hong Kong and US stocks, which is not explicitly legal under Chinese securities laws. The CSRC has long warned against such practices, but enforcement has been limited. This new plan provides a clear timeline and penalties.

<details><summary>References</summary>
<ul>
<li><a href="https://m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml">m.guancha.cn/GuanJinRong/2026_05_22_818035.shtml</a></li>
<li><a href="https://m.jiemian.com/article/14471841.html">m.jiemian.com/article/14471841.html</a></li>
<li><a href="https://www.21jingji.com/article/20260523/herald/e7eb58bb6994d891f986fd9d06c85b1d.html">中国 证 监会拟对 富 途 罚 款18.5亿， 老 虎 证 券 罚 没4.112亿 - 21经济网</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#China`, `#cross-border trading`, `#securities`, `#fintech`

---

<a id="item-10"></a>
## [Cloudflare 25-Minute Outage Hits 28% of HTTP Traffic](https://t.me/zaihuapd/41527) ⭐️ 8.0/10

On December 5, 2025, at 08:47 UTC, Cloudflare experienced a 25-minute global outage that affected approximately 28% of HTTP traffic, caused by a WAF managed ruleset update intended to patch a Next.js security vulnerability (CVE-2025-55182). This outage underscores the fragility of centralized web infrastructure, as Cloudflare protects a significant portion of global internet traffic. The incident also highlights the risks of deploying security patches at scale without sufficient testing. The outage primarily affected customers using the legacy FL1 proxy and the Cloudflare Managed Ruleset. The problematic WAF update was deployed to mitigate CVE-2025-55182, a critical unauthenticated remote code execution vulnerability in React Server Components exploited via Next.js.

telegram · zaihuapd · May 22, 16:15

**Background**: Cloudflare is a major content delivery network (CDN) and web security provider, handling a large share of global HTTP traffic. Its Web Application Firewall (WAF) uses managed rulesets to block malicious requests. The vulnerability CVE-2025-55182, also known as React2Shell, allows attackers to execute arbitrary code on servers running React Server Components without authentication.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.cloudflare.com/waf/managed-rules/">Managed Rules · Cloudflare Web Application Firewall ( WAF ) docs</a></li>
<li><a href="https://react.dev/blog/2025/12/03/critical-security-vulnerability-in-react-server-components">Critical Security Vulnerability in React Server Components – React</a></li>
<li><a href="https://medium.com/@pnadheem/your-next-js-app-might-be-fine-until-one-weird-request-hits-it-react2shell-cve-2025-55182-3a6d0ed214e0">Your Next . js App Might Be “Fine”… Until One Weird Request... | Medium</a></li>

</ul>
</details>

**Tags**: `#Cloudflare`, `#outage`, `#WAF`, `#Next.js`, `#security`

---

<a id="item-11"></a>
## [Microsoft Widely Deploys Claude Code, Urges Non-Tech Staff to Use AI Coding](https://t.me/zaihuapd/41535) ⭐️ 8.0/10

Microsoft is widely deploying Anthropic's Claude Code across key engineering teams, including the CoreAI team and teams responsible for Windows, Microsoft 365, and Outlook, and is encouraging non-technical employees to use it for prototyping. Engineers are now required to use both Claude Code and GitHub Copilot and provide comparative feedback. This move signals a major shift in Microsoft's AI-assisted development strategy, as it adopts a competitor's tool alongside its own GitHub Copilot, potentially influencing industry practices. It also lowers the barrier for non-technical staff to participate in software prototyping, which could accelerate innovation across the company. Claude Code is an AI coding agent developed by Anthropic that runs in the terminal or IDE, while GitHub Copilot is Microsoft's own AI pair programmer. The requirement for engineers to compare both tools suggests Microsoft is evaluating which performs better for different tasks.

telegram · zaihuapd · May 23, 06:05

**Background**: Claude Code is part of Anthropic's Claude model series, which uses constitutional AI for ethical alignment. GitHub Copilot, developed by GitHub and OpenAI, is a widely used code completion tool integrated into popular IDEs. Microsoft's adoption of a competitor's tool alongside its own reflects the rapidly evolving landscape of AI-assisted development.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Claude_Code">Claude Code</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#Microsoft`, `#Claude Code`, `#GitHub Copilot`, `#software engineering`

---

<a id="item-12"></a>
## [Corsair Adopts CXMT Chips, DDR5 Prices May Drop](https://thenextweb.com/news/chinese-dram-cxmt-corsair-ddr5-memory-prices) ⭐️ 8.0/10

Corsair has started using DRAM chips from Chinese manufacturer ChangXin Memory Technologies (CXMT) in its DDR5 memory modules, with 6000 MT/s kits already on the market. This shift diversifies the DRAM supply chain and could lower DDR5 prices as Chinese capacity expands, especially amid AI-driven demand for HBM squeezing consumer DRAM supply. The CXMT-based DDR5 modules operate at 6000 MT/s with performance matching mainstream international products. CXMT plans to go public in 2026 after a strong Q1 performance.

telegram · zaihuapd · May 23, 11:17

**Background**: DRAM is a type of memory used in computers and servers. The global DRAM market is dominated by three major players: Samsung, SK Hynix, and Micron. Recently, these companies have shifted production capacity to high-bandwidth memory (HBM) for AI applications, reducing supply of consumer DDR5. CXMT is a Chinese DRAM manufacturer that has been ramping up production to fill the gap.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/ChangXin_Memory_Technologies">ChangXin Memory Technologies - Wikipedia</a></li>
<li><a href="https://www.cxmt.com/en/">About cxmt - cxmt</a></li>

</ul>
</details>

**Tags**: `#DDR5`, `#DRAM`, `#Corsair`, `#CXMT`, `#supply chain`

---

<a id="item-13"></a>
## [Critique of HTML <dl> Element Sparks Debate on Semantic HTML](https://benmyers.dev/blog/on-the-dl/) ⭐️ 7.0/10

Ben Myers published a detailed critique of the HTML <dl> element, arguing that its design and usage are flawed for modern web development. The article has generated significant discussion on Hacker News, with 106 comments and 346 points. This critique challenges the practical value of semantic HTML, a cornerstone of web accessibility and SEO. The debate highlights tensions between theoretical semantics and real-world development needs, influencing how developers approach markup choices. The <dl> element lacks an implicit ARIA role, and aria-label is not allowed on it without an explicit role. Developers often find <dl> too rigid for complex layouts, such as needing multiple wrappers or dividers between sections.

hackernews · ravenical · May 23, 13:03 · [Discussion](https://news.ycombinator.com/item?id=48247325)

**Background**: Semantic HTML uses elements that convey meaning about the structure of content, improving accessibility and SEO. The <dl> element was originally designed for definition lists, such as glossaries, but is now used for various key-value pair displays. Critics argue that its constraints make it impractical for modern web interfaces.

<details><summary>References</summary>
<ul>
<li><a href="https://frontman.sh/glossary/semantic-html/">Semantic HTML | Frontman Glossary</a></li>
<li><a href="https://www.codecademy.com/resources/blog/semantic-html/">codecademy.com/resources/blog/ semantic - html</a></li>
<li><a href="https://academi.dev/html-semantics-and-accessibility/">HTML Semantics and Accessibility Explained: Building... | Academi</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed views: some agreed that semantic HTML is poorly designed and impractical, while others defended its historical roots and accessibility benefits. One commenter noted that <dl> has been used since before the web, referencing a 1985 IBM manual.

**Tags**: `#HTML`, `#semantic web`, `#accessibility`, `#web development`

---

<a id="item-14"></a>
## [FTC Fines Cox Media Group for Fake AI 'Active Listening' Ads](https://simonwillison.net/2026/May/22/ftc-active-listening/#atom-everything) ⭐️ 7.0/10

The FTC announced that Cox Media Group, MindSift, and 1010 Digital Works will pay nearly $1 million to settle charges that they falsely marketed an 'Active Listening' AI service that claimed to eavesdrop on smart device conversations for ad targeting. This enforcement action sets a precedent against deceptive AI marketing claims, reinforcing that companies cannot exaggerate AI capabilities to sell services, especially those involving invasive surveillance of consumers. The FTC found that the 'Active Listening' service did not actually listen to conversations or use voice data; instead, it resold email lists from data brokers at a markup. The FTC also stated that hiding opt-in consent in terms of service does not constitute adequate consent.

rss · Simon Willison · May 22, 04:48

**Background**: In 2024, Cox Media Group marketed an 'Active Listening' service claiming smart devices capture real-time intent data by listening to conversations. This fueled conspiracy theories that phones spy on users via microphones for ads. The FTC's action debunks those claims, showing the service was a resold email list.

**Tags**: `#FTC`, `#AI`, `#privacy`, `#regulation`, `#marketing`

---

<a id="item-15"></a>
## [Tencent's Ximalaya Acquisition Approved with Conditions](https://mp.weixin.qq.com/s/xnx31SOS6NMozZXnHeaaQg) ⭐️ 7.0/10

China's State Administration for Market Regulation approved Tencent's acquisition of Ximalaya, requiring Tencent to abandon exclusive audio copyright agreements and terminate existing exclusive contracts within a set period. This decision dismantles Ximalaya's exclusive content barriers, allowing competing platforms to access the same audio content, which could reshape competition in China's online audio market and improve cross-platform listening convenience for users. Tencent must not enter into or indirectly create exclusive online audio copyright agreements, and must phase out existing exclusive deals. Tencent stated it will cooperate with the termination of exclusive contracts and seek non-exclusive partnerships going forward.

telegram · zaihuapd · May 22, 10:33

**Background**: Ximalaya is a leading online audio platform in China, known for its extensive library of exclusive content such as audiobooks and podcasts. Exclusive copyright agreements have been a key competitive advantage, but also a barrier for users who want to access content across different platforms. The regulator's condition aims to promote fair competition and consumer choice.

**Tags**: `#antitrust`, `#China`, `#online audio`, `#acquisition`, `#regulation`

---

<a id="item-16"></a>
## [China's Daily Token Calls Surge 1000x in Two Years, Exceed 140 Trillion](https://t.me/zaihuapd/41542) ⭐️ 7.0/10

China's National Data Bureau disclosed that daily token call volume exceeded 140 trillion in March 2025, up from 100 billion in early 2024, representing a more than 1000-fold increase in two years. This explosive growth signals rapid commercialization of AI in China and the formation of a data market around token-based pricing and settlement, which could accelerate AI adoption across industries. Token is the smallest unit of information processed by large language models, and its call volume is a key metric for AI usage. The data was disclosed by the National Data Bureau, a government agency, adding credibility.

telegram · zaihuapd · May 23, 14:36

**Background**: Tokens are the basic units that large language models use to process text; they can be words, subwords, or characters. The token economy refers to the emerging system where tokens are metered, priced, and traded, enabling commercial AI services. China's data market reforms aim to facilitate the flow and pricing of data as a production factor.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/docs/transformers/zh/main_classes/tokenizer">Tokenizer - Hugging Face</a></li>
<li><a href="https://www.moomoo.com/news/post/70293298/china-galaxy-securities-operators-introduction-of-token-based-plans-opens">China Galaxy Securities: Operators' Introduction of Token-Based Plans ...</a></li>
<li><a href="https://qwen.readthedocs.io/zh-cn/latest/getting_started/concepts.html">核心概念 - Qwen</a></li>

</ul>
</details>

**Tags**: `#AI`, `#China`, `#token economy`, `#data market`, `#industry growth`

---