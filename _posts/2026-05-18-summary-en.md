---
layout: default
title: "Horizon Summary: 2026-05-18 (EN)"
date: 2026-05-18
lang: en
---

> From 33 items, 15 important content pieces were selected

---

1. [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](#item-1) ⭐️ 9.0/10
2. [Semble: Code search for agents with 98% fewer tokens](#item-2) ⭐️ 8.0/10
3. [Native vs Web: Text Rendering on iOS](#item-3) ⭐️ 8.0/10
4. [GDS Opposes NHS Retreat from Open Source](#item-4) ⭐️ 8.0/10
5. [OpenClaw Developer Burns $1.3M in OpenAI API Tokens in One Month](#item-5) ⭐️ 8.0/10
6. [Turning an $80 Android Tablet into a Debian Workstation](#item-6) ⭐️ 7.0/10
7. [AI Won't Speed Up Software Processes](#item-7) ⭐️ 7.0/10
8. [Tesla Solar Roof Deprioritized for Panels](#item-8) ⭐️ 7.0/10
9. [Mozilla Defends VPNs Against UK Age-Gating Proposals](#item-9) ⭐️ 7.0/10
10. [AI Is a Technology, Not a Product](#item-10) ⭐️ 7.0/10
11. [Apple Silicon LLM Costs Exceed OpenRouter](#item-11) ⭐️ 7.0/10
12. [Malta Offers Free ChatGPT Plus to All Citizens](#item-12) ⭐️ 7.0/10
13. [EU to Act Against TikTok and Meta Over Addictive Design](#item-13) ⭐️ 7.0/10
14. [GitHub Copilot Desktop App Enters Technical Preview](#item-14) ⭐️ 7.0/10
15. [Changxin Technology Files for IPO with 719% Revenue Surge](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.12) ⭐️ 9.0/10

SGLang v0.5.12 introduces comprehensive inference support for DeepSeek V4, including tensor, expert, context, and data parallel attention, along with optimized DeepGemm and FlashMLA kernels for MegaMoE. It also adds support for new models like Intern-S2-Preview, MiniCPM-V 4.6, and Gemma 4 MTP. This release significantly enhances the efficiency and scalability of serving DeepSeek V4, a major large language model, by leveraging advanced parallelism and kernel optimizations. It enables lower latency and higher throughput for AI inference, benefiting the broader AI/ML community. Key technical additions include HiSparse for offloading inactive KV cache to CPU memory, W4A4 MegaMoE kernels for faster speed with negligible accuracy drop, and a unified Docker tag for all Nvidia GPUs. The release also features TokenSpeed MLA attention backend with FP8 KV cache on Blackwell GPUs.

github · Fridge003 · May 16, 18:23

**Background**: SGLang is an open-source inference engine for large language models, designed for high performance and flexibility. DeepSeek V4 is a state-of-the-art MoE (Mixture-of-Experts) model that requires sophisticated parallelism and kernel optimizations for efficient inference. Techniques like tensor parallelism and expert parallelism distribute computation across multiple GPUs, while DeepGemm and FlashMLA are specialized kernels that accelerate matrix operations and attention mechanisms.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/deepseek-ai/DeepGEMM">GitHub - deepseek-ai/DeepGEMM: DeepGEMM: clean and efficient ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek V4`, `#inference`, `#SGLang`, `#LLM`, `#kernel optimization`

---

<a id="item-2"></a>
## [Semble: Code search for agents with 98% fewer tokens](https://github.com/MinishLab/semble) ⭐️ 8.0/10

Semble is an open-source code search tool that combines static Model2Vec embeddings with BM25, achieving 98% fewer tokens than grep while running on CPU. It indexes a typical repo in ~250ms and queries in ~1.5ms, reaching 99% of the retrieval quality of a 137M-parameter transformer. This significantly reduces token costs for AI agents like Claude Code when navigating large codebases, addressing a key inefficiency in agent-based code search. Its CPU-only operation and zero-config setup make it accessible without GPU or API keys. Semble uses the potion-code-16M static model from Model2Vec, combined with BM25, fused via Reciprocal Rank Fusion (RRF) and reranked with code-aware signals. It achieves 0.854 NDCG@10 on a benchmark of ~1250 query/document pairs across 63 repos and 19 languages.

hackernews · Bibabomas · May 17, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48169874)

**Background**: AI agents often fall back to grep when they cannot find relevant code, which reads entire files and consumes many tokens. Existing alternatives like transformer-based embeddings are slow on CPU or require GPU/API keys. Model2Vec is a technique that converts sentence transformers into small static embedding models, reducing size by up to 50x and increasing speed by 500x with minimal performance loss. BM25 is a classic probabilistic ranking function used in information retrieval.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/MinishLab/model2vec">GitHub - MinishLab/model2vec: Fast State-of-the-Art Static ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Okapi_BM25">Okapi BM25 - Wikipedia</a></li>
<li><a href="https://minish.ai/packages/model2vec/introduction/">Model2Vec | Minish</a></li>

</ul>
</details>

**Discussion**: Commenters raised concerns about probabilistic search vs deterministic grep, and whether agents trust results from non-grep tools. Others compared Semble to LSPs and suggested semantic search could also benefit human developers.

**Tags**: `#code search`, `#AI agents`, `#embeddings`, `#open source`, `#efficiency`

---

<a id="item-3"></a>
## [Native vs Web: Text Rendering on iOS](https://justsitandgrin.im/posts/native-all-the-way-until-you-need-text/) ⭐️ 8.0/10

A developer shares their experience building a performant iOS text editor, finding that while TextKit 2 can handle 5,000-line files with sub-8ms keystroke restyling, complex Markdown rendering led them to adopt WebKit as a pragmatic choice. This article highlights the ongoing tension between native and web rendering for text-heavy apps, challenging the assumption that native always outperforms web views, especially as browser engines mature and SwiftUI still has performance gaps. The author tested TextKit 2 with Moby Dick, achieving 25x faster visible-range rendering than full-document styling, but found WebKit more practical for rich Markdown features like inline images and bidirectional text.

hackernews · dive · May 17, 11:49 · [Discussion](https://news.ycombinator.com/item?id=48168058)

**Background**: TextKit 2 is Apple's modern text engine introduced in iOS 15, designed for better performance and flexibility than TextKit 1. WebKit, while often associated with web browsers, is a native macOS/iOS framework that can render HTML and CSS efficiently. The debate centers on whether to use native frameworks for text or rely on WebKit for complex rendering tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/videos/play/wwdc2021/10061/">Meet TextKit 2 - WWDC21 - Videos - Apple Developer</a></li>
<li><a href="https://developer.apple.com/videos/play/wwdc2022/10090/">What's new in TextKit and text views - WWDC22 - Videos - Apple Developer</a></li>
<li><a href="https://news.ycombinator.com/item?id=48168455">If you're on macOS, WebKit is a native OS framework. | Hacker News</a></li>

</ul>
</details>

**Discussion**: Commenters debated the trade-offs: some argued WebKit is a native framework on macOS and appropriate for Markdown rendering, while others pointed out that SwiftUI still has performance issues and that mature SwiftUI Markdown renderers exist. A developer shared their positive experience with TextKit 2 for large files.

**Tags**: `#text rendering`, `#native vs web`, `#iOS development`, `#performance`, `#SwiftUI`

---

<a id="item-4"></a>
## [GDS Opposes NHS Retreat from Open Source](https://simonwillison.net/2026/May/17/gds-weighs-in/#atom-everything) ⭐️ 8.0/10

The UK Government Digital Service (GDS) published guidance on May 14, 2026, recommending that public sector organizations keep open source repositories public by default, directly countering the NHS's recent decision to close its GitHub repositories in response to security vulnerabilities reported via Project Glasswing. This public disagreement between two major UK government bodies highlights a critical policy debate about openness versus security in public sector software, with implications for transparency, cost, and reuse across government IT. GDS's guidance, titled 'AI, open code and vulnerability risk in the public sector,' emphasizes that making repositories private adds delivery and policy costs while reducing reuse and scrutiny. Terence Eden interprets this as a rare public escalation within the civil service, likening it to 'being invited to a meeting without biscuits.'

rss · Simon Willison · May 17, 15:59

**Background**: The NHS decided to close its public GitHub repositories after vulnerabilities were reported through Project Glasswing, an Anthropic-led cybersecurity initiative using advanced AI. GDS, as the digital center of government, typically advocates for open source to promote transparency and efficiency. This incident marks a significant policy rift between the two organizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.gov.uk/government/organisations/government-digital-service">Government Digital Service - GOV.UK</a></li>
<li><a href="https://shkspr.mobi/blog/2026/05/nhs-goes-to-war-against-open-source/">NHS Goes To War Against Open Source</a></li>
<li><a href="https://www.theregister.com/2026/05/05/nhs_to_closesource_hundreds_of_repos/">NHS to close-source hundreds of GitHub repos over AI, security concerns</a></li>

</ul>
</details>

**Discussion**: The article's comments are not provided, but the broader community discussion on Terence Eden's blog and other outlets shows support for GDS's stance, with many criticizing the NHS's reaction as an overreaction that undermines the benefits of open source.

**Tags**: `#open source`, `#government policy`, `#security`, `#public sector`

---

<a id="item-5"></a>
## [OpenClaw Developer Burns $1.3M in OpenAI API Tokens in One Month](https://www.tomshardware.com/tech-industry/artificial-intelligence/openclaw-creator-burns-through-1-3-million-in-openai-api-tokens-in-a-single-month) ⭐️ 8.0/10

Peter Steinberger, the developer of OpenClaw, revealed that his team consumed $1.3 million worth of OpenAI API tokens in 30 days, involving 603 billion tokens and 7.6 million requests from about 100 Codex agents. This case highlights the enormous operational costs of AI agent automation at scale, with implications for the economics of AI development and the sustainability of autonomous coding agents. The high cost was driven by Codex's 'fast mode' pricing; disabling it would have reduced the raw API cost to about $300,000. The bill also showed usage of the GPT-5.5 model dated April 23, 2026.

telegram · zaihuapd · May 17, 13:38

**Background**: OpenClaw is a free, open-source autonomous AI agent that executes tasks via large language models, using messaging platforms as its main interface. Codex is an AI coding agent from OpenAI that assists with software development tasks. GPT-5.5 is a large language model released by OpenAI on April 23, 2026, known for its advanced coding capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenClaw">OpenClaw</a></li>
<li><a href="https://en.wikipedia.org/wiki/Codex_(AI_agent)">Codex (AI agent) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>

</ul>
</details>

**Tags**: `#AI`, `#OpenAI`, `#API costs`, `#Codex`, `#automation`

---

<a id="item-6"></a>
## [Turning an $80 Android Tablet into a Debian Workstation](https://github.com/tech4bot/rk3562deb) ⭐️ 7.0/10

A developer published a guide on GitHub showing how to convert an $80 RK3562 Android tablet into a functional Debian Linux workstation, leveraging AI-assisted reverse engineering to enable hardware support. This project demonstrates the potential of repurposing cheap, widely available hardware for Linux, lowering the barrier to entry for tinkerers and developers. It also highlights how AI can accelerate reverse engineering, making device hacking more accessible. The tablet uses a Rockchip RK3562 quad-core processor and 4 GB RAM, which limits multitasking but is sufficient for lightweight desktop environments or terminal-based workflows. The guide includes steps for booting Debian with most devices functional.

hackernews · tech4bot · May 17, 13:16 · [Discussion](https://news.ycombinator.com/item?id=48168668)

**Background**: The RK3562 is a low-power quad-core application processor from Rockchip, commonly used in budget Android tablets. AI-assisted reverse engineering uses machine learning to automate the analysis of hardware and software, making it easier to port operating systems to new devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rockchips.net/product/rk3562/">RK3562 - Rockchips.net</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI-assisted_reverse_engineering">AI-assisted reverse engineering - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters expressed enthusiasm for the project, with some noting that 4 GB RAM is adequate for lightweight tasks like terminal-based development or VAX emulation. Others asked for educational resources on using AI for reverse engineering, and one warned that such breakthroughs could drive up prices of cheap tablets.

**Tags**: `#Linux`, `#Embedded Systems`, `#Hardware Hacking`, `#Debian`, `#AI-assisted Reverse Engineering`

---

<a id="item-7"></a>
## [AI Won't Speed Up Software Processes](https://frederickvanbrabant.com/blog/2026-05-15-i-dont-think-ai-will-make-your-processes-go-faster/) ⭐️ 7.0/10

Frederick Van Brabant argues that AI will not accelerate software development processes because the primary bottleneck is unclear requirements, which AI cannot resolve without human input. This challenges the prevailing hype that AI will dramatically boost software productivity, highlighting that fundamental human-centric issues like requirement ambiguity remain critical. The article notes that software developers have long sought detailed problem outlines, but vague feature requests are the norm; AI cannot clarify these without human intervention.

hackernews · TheEdonian · May 17, 12:13 · [Discussion](https://news.ycombinator.com/item?id=48168221)

**Background**: In software engineering, requirements gathering is often the most time-consuming and error-prone phase. AI tools like LLMs can generate code quickly but still depend on precise specifications to produce correct outputs.

**Discussion**: Commenters largely agree that requirements are the bottleneck, with some noting AI can still help in ideation, documentation, and deployment. Others argue AI is more transformative for tasks outside one's expertise.

**Tags**: `#AI`, `#software engineering`, `#productivity`, `#requirements`

---

<a id="item-8"></a>
## [Tesla Solar Roof Deprioritized for Panels](https://electrek.co/2026/05/14/tesla-solar-roof-promise-vs-reality-pivot-panels/) ⭐️ 7.0/10

Tesla is pivoting away from its Solar Roof product toward traditional solar panels, effectively putting the Solar Roof on life support due to high costs and poor economics. This strategic shift signals that Tesla's ambitious integrated solar roofing solution has failed to achieve mass-market viability, potentially reshaping the residential solar market and impacting consumer choices. An average Tesla Solar Roof costs approximately $106,000 before incentives, compared to roughly $60,000 for a traditional roof replacement plus conventional solar panels, with a payback period of 15-25 years versus 7-12 years for panels.

hackernews · celsoazevedo · May 17, 04:09 · [Discussion](https://news.ycombinator.com/item?id=48165980)

**Background**: Tesla's Solar Roof was introduced as a premium product that integrates solar cells into roof tiles, aiming to replace traditional roofing while generating electricity. However, high installation costs and complex logistics hindered adoption compared to conventional solar panels, which are cheaper and easier to install.

**Discussion**: Commenters expressed disappointment over the product's decline, noting its aesthetic appeal but agreeing that the economics never worked. Some speculated the Solar Roof was initially used to boost Tesla's stock during financial struggles.

**Tags**: `#Tesla`, `#solar energy`, `#renewable energy`, `#business strategy`, `#clean tech`

---

<a id="item-9"></a>
## [Mozilla Defends VPNs Against UK Age-Gating Proposals](https://blog.mozilla.org/netpolicy/2026/05/15/mozilla-to-uk-regulators-vpns-are-essential-privacy-and-security-tools-and-should-not-be-undermined/) ⭐️ 7.0/10

Mozilla submitted a response to a UK government consultation on age-gating online content, arguing that VPNs are essential privacy and security tools and should not be undermined. This matters because the UK's proposed age verification requirements for VPNs could set a global precedent for undermining online privacy and security, affecting millions of users who rely on VPNs for protection. The consultation, titled 'Growing up in the online world,' includes a specific question about age-gating VPNs buried about 30 pages deep. Mozilla's response emphasizes that regulators should hold platforms accountable for online harm rather than targeting VPNs.

hackernews · WithinReason · May 17, 06:17 · [Discussion](https://news.ycombinator.com/item?id=48166459)

**Background**: VPNs (Virtual Private Networks) encrypt internet traffic and hide users' IP addresses, providing privacy and security online. The UK government has been exploring age verification measures to protect children from harmful content, but critics argue that requiring VPNs to verify age would compromise their core privacy function and could lead to surveillance.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.mozilla.org/netpolicy/2026/05/15/mozilla-to-uk-regulators-vpns-are-essential-privacy-and-security-tools-and-should-not-be-undermined/">Mozilla to UK regulators: VPNs are essential privacy and security tools and should not be undermined – Open Policy & Advocacy</a></li>
<li><a href="https://www.youtube.com/watch?v=uzmR4nt1rpE">UK Proposes 24/7 Phone Surveillance & VPN Age Verification</a></li>
<li><a href="https://outbyte.com/blog/the-uk-debates-age-checks-for-vpns-will-it-protect-kids-or-destroy-adult-privacy/">The UK Debates Age Checks for VPNs : Will It... - Outbyte Official Blog</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that the Australian government surprisingly recommends VPN usage, and one user notes that Mozilla's response is to a specific UK consultation. Another user questions whether Google has made a similar statement, while a comment references George Orwell's '1984' as a warning against the UK's digital policies.

**Tags**: `#privacy`, `#VPN`, `#UK regulation`, `#digital rights`, `#Mozilla`

---

<a id="item-10"></a>
## [AI Is a Technology, Not a Product](https://daringfireball.net/2026/05/ai_is_technology_not_a_product) ⭐️ 7.0/10

An article argues that AI should be viewed as an underlying technology that enhances products like Siri, rather than a standalone product, drawing parallels to the 'Dropbox is a feature' debate. This perspective challenges the current AI hype cycle, urging companies to focus on integrating AI into user-centric products rather than marketing AI as a separate offering, which could reshape product strategy across the tech industry. The article references Apple's customer-centric approach and the historical example of iTunes Ping's failure to illustrate that technology must serve a clear user need. It also echoes the earlier 'Dropbox is a feature' argument, suggesting AI companies may struggle to build sustainable ecosystems.

hackernews · ch_sm · May 17, 13:11 · [Discussion](https://news.ycombinator.com/item?id=48168626)

**Background**: The debate over whether AI is a product or a technology mirrors earlier discussions in tech, such as the 'Dropbox is a feature' argument, where cloud storage was seen as a commodity rather than a standalone product. Apple has historically focused on integrating technology into polished user experiences, as Steve Jobs emphasized working backwards from the customer experience.

**Discussion**: Commenters largely agree with the article, noting that Apple's ideal AI implementation would be making Siri work seamlessly without feeling like AI. One commenter references Steve Jobs' philosophy of working backwards from the customer experience, while another draws a direct parallel to the 'Dropbox is a feature' argument, warning that AI companies risk becoming disposable without hardware integration.

**Tags**: `#AI`, `#product design`, `#Apple`, `#technology strategy`

---

<a id="item-11"></a>
## [Apple Silicon LLM Costs Exceed OpenRouter](https://www.williamangel.net/blog/2026/05/17/offline-llm-energy-use.html) ⭐️ 7.0/10

A blog post by William Angel compares the cost of running large language models on Apple Silicon hardware versus using cloud APIs like OpenRouter, concluding that local inference is more expensive. The analysis factors in hardware depreciation, electricity, and token throughput. This challenges the common assumption that local inference is cheaper, with implications for developers and businesses deciding between on-device and cloud AI. The debate also highlights potential underpricing by cloud providers, which may not be sustainable long-term. The author estimates that even under optimistic assumptions (50W power, 40 tokens/sec, 10-year lifespan), a MacBook Pro Max is only as cheap as OpenRouter's Gemma4 31b pricing of ~38-50 cents per million tokens. However, the analysis rounds up electricity costs and assumes 24/7 dedicated use, which may not reflect real-world scenarios.

hackernews · datadrivenangel · May 17, 12:09 · [Discussion](https://news.ycombinator.com/item?id=48168198)

**Background**: Running LLMs locally on Apple Silicon (e.g., M4 Max) is popular for privacy and offline use, but hardware costs are significant. Cloud APIs like OpenRouter aggregate multiple models and charge per token, often subsidized by venture capital. The comparison is relevant as both approaches are used for AI inference.

<details><summary>References</summary>
<ul>
<li><a href="https://www.williamangel.net/blog/2026/05/17/offline-llm-energy-use.html">Apple Silicon costs more than OpenRouter</a></li>
<li><a href="https://openrouter.ai/pricing">Pricing - OpenRouter</a></li>
<li><a href="https://www.compute-market.com/blog/mac-mini-m4-for-ai-apple-silicon-2026">Mac Mini M4 for AI 2026 — LLM Benchmarks & Review | Compute Market</a></li>

</ul>
</details>

**Discussion**: Commenters criticize the methodology: bastawhiz points out rounding errors and unrealistic 24/7 usage assumptions; applfanboysbgon notes the analysis ignores the dual-use value of a laptop; dijit argues that cloud APIs are sold at a loss, making the comparison unfair. Others suggest using more efficient models like Qwen3.6 27B for better speed and cost.

**Tags**: `#LLM`, `#Apple Silicon`, `#cost analysis`, `#inference`, `#cloud vs local`

---

<a id="item-12"></a>
## [Malta Offers Free ChatGPT Plus to All Citizens](https://openai.com/index/malta-chatgpt-plus-partnership/) ⭐️ 7.0/10

OpenAI and the Maltese government announced a national partnership to provide every citizen with a free one-year subscription to ChatGPT Plus, after completing an AI literacy course developed by the University of Malta. This is the first national-level partnership for ChatGPT Plus, setting a precedent for government-led AI accessibility and education initiatives worldwide. The program, called 'AI for All,' starts in May 2026, managed by the Malta Digital Innovation Authority, and will later extend to overseas citizens.

telegram · zaihuapd · May 16, 10:40

**Background**: Malta launched a national AI strategy in 2019, aiming to drive AI adoption and innovation. The Malta Digital Innovation Authority (MDIA) oversees digital innovation and AI governance. This partnership combines AI access with mandatory education to promote responsible use.

<details><summary>References</summary>
<ul>
<li><a href="https://gagadget.com/en/710697-malta-is-giving-citizens-free-chatgpt-plus-if-they-take-an-ai-class-first/">Malta is giving citizens free ChatGPT Plus — if they take an AI class first</a></li>
<li><a href="https://de.euronews.com/next/2026/05/16/malta-burger-erhalten-chatgpt-plus-gratis-uber-nationales-ki-programm">Malta : Bürger erhalten ChatGPT Plus gratis über... | Euronews</a></li>
<li><a href="https://mdia.gov.mt/">Malta Digital Innovation Authority</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#AI policy`, `#education`, `#partnership`

---

<a id="item-13"></a>
## [EU to Act Against TikTok and Meta Over Addictive Design](https://unwire.hk/2026/05/16/eu-tiktok-meta-addictive-design-child-protection/life-tech/social-network/) ⭐️ 7.0/10

European Commission President Ursula von der Leyen announced at a summit in Denmark that the EU will take action against TikTok and Meta (Instagram, Facebook) over addictive design features and inadequate enforcement of the 13-year-old age limit, with legal advice expected by summer 2026. This marks a significant escalation in EU regulation of platform design under the Digital Services Act, potentially forcing major social media companies to redesign core engagement features globally and setting a precedent for other jurisdictions. The EU has preliminarily found TikTok's addictive design and Meta's age verification mechanisms in breach of the DSA, and has already released an open-source anonymous age verification app. Australia has banned social media for under-16s, with many countries following suit.

telegram · zaihuapd · May 16, 14:33

**Background**: The Digital Services Act (DSA) is a landmark EU regulation that imposes stricter obligations on large online platforms to address illegal content, systemic risks, and user safety. Addictive design refers to features like infinite scroll, autoplay, and push notifications that are designed to maximize user engagement and time spent on the platform. Age verification has become a key focus as governments seek to protect minors online.

<details><summary>References</summary>
<ul>
<li><a href="https://digital-strategy.ec.europa.eu/en/news/commission-preliminarily-finds-tiktoks-addictive-design-breach-digital-services-act">Commission preliminarily finds TikTok's addictive design in ...</a></li>
<li><a href="https://www.technobezz.com/news/eu-plans-new-rules-targeting-addictive-design-on-tiktok-and-meta-to-protect-children">EU Plans New Rules Targeting Addictive Design on TikTok and ...</a></li>
<li><a href="https://www.freevacy.com/news/politico/von-der-leyen-hints-social-media-ban-and-age-verification-possible-by-summer/7372">Von der Leyen hints social media ban and age verification possible...</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#addictive design`, `#TikTok`, `#Meta`, `#Digital Services Act`

---

<a id="item-14"></a>
## [GitHub Copilot Desktop App Enters Technical Preview](https://github.blog/changelog/2026-05-14-github-copilot-app-is-now-available-in-technical-preview/) ⭐️ 7.0/10

GitHub Copilot is now available as a desktop app in technical preview, allowing users to launch isolated development sessions directly from issues, pull requests, prompts, or history, view diffs, run tests, create PRs, and use Agent Merge to automatically handle review comments and merges. This update transforms Copilot from a code completion tool into a full-fledged development environment, enabling developers to perform complex workflows without leaving the app. It significantly reduces context switching and automates tedious tasks like merge conflict resolution, boosting productivity for Copilot Pro and Pro+ subscribers. The technical preview is available immediately for Copilot Pro and Pro+ subscribers, while Business and Enterprise users will gain access later this week, provided their organization admin enables the preview and CLI permissions in policies. Agent Merge, which automates review handling, was previously introduced as a cloud agent feature in April 2026.

telegram · zaihuapd · May 16, 15:07

**Background**: GitHub Copilot is an AI-powered code completion and programming assistant developed by GitHub and OpenAI, integrated into popular IDEs like VS Code and JetBrains. The new desktop app extends Copilot's capabilities beyond inline suggestions, providing an isolated environment for tasks such as running tests, reviewing diffs, and managing pull requests. Agent Merge is a feature that uses a cloud-based agent to automatically resolve merge conflicts and handle review comments, reducing manual effort.

<details><summary>References</summary>
<ul>
<li><a href="https://github.blog/changelog/2026-04-13-fix-merge-conflicts-in-three-clicks-with-copilot-cloud-agent/">Fix merge conflicts in three clicks with Copilot cloud agent - GitHub Changelog</a></li>
<li><a href="https://github.blog/changelog/2026-03-26-ask-copilot-to-resolve-merge-conflicts-on-pull-requests/">Ask @copilot to resolve merge conflicts on pull requests - GitHub Changelog</a></li>
<li><a href="https://en.wikipedia.org/wiki/GitHub_Copilot">GitHub Copilot - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#GitHub Copilot`, `#AI coding assistant`, `#developer tools`, `#technical preview`

---

<a id="item-15"></a>
## [Changxin Technology Files for IPO with 719% Revenue Surge](https://api3.cls.cn/share/article/2373399?os=android&amp;sv=8.7.8&amp;app=cailianpress) ⭐️ 7.0/10

Changxin Technology (CXMT) has filed for an IPO on Shanghai's STAR Market, disclosing Q1 2026 revenue of 50.8 billion yuan (up 719.13% YoY) and net profit of 33.01 billion yuan, reversing prior losses. The company also guided H1 2026 revenue of 110-120 billion yuan. This IPO filing highlights the rapid growth of China's domestic DRAM industry amid a global memory shortage driven by AI demand. If successful, it would provide a major funding channel for CXMT to expand capacity and compete with Samsung, SK Hynix, and Micron. The company's Q1 2026 net profit attributable to parent was 24.76 billion yuan, with non-recurring items excluded net profit of 26.34 billion yuan. The H1 guidance implies continued strong momentum, with revenue growth of 612-677% YoY.

telegram · zaihuapd · May 17, 11:05

**Background**: DRAM (Dynamic Random-Access Memory) is a type of semiconductor memory widely used as main memory in computers and servers. The global DRAM market is currently dominated by three players: Samsung, SK Hynix, and Micron. Changxin Technology is a leading Chinese DRAM manufacturer, and its IPO on the STAR Market (China's Nasdaq-style board for tech firms) would be a milestone for China's semiconductor self-sufficiency efforts.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dynamic_random-access_memory">Dynamic random-access memory - Wikipedia</a></li>
<li><a href="https://baike.kuaiji.com/v231914478.html">扣非归母净利润 (财会术语) - 会计百科</a></li>

</ul>
</details>

**Tags**: `#semiconductor`, `#IPO`, `#DRAM`, `#China tech`, `#finance`

---