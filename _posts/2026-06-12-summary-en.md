---
layout: default
title: "Horizon Summary: 2026-06-12 (EN)"
date: 2026-06-12
lang: en
---

> From 40 items, 22 important content pieces were selected

---

1. [AMD's Inadequate Fix for Critical RCE Vulnerability](#item-1) ⭐️ 9.0/10
2. [Anthropic Reverses Secret Policy Limiting AI Researchers](#item-2) ⭐️ 9.0/10
3. [Anthropic Launches Claude Fable 5 and Mythos 5 with Major Performance Gains](#item-3) ⭐️ 9.0/10
4. [Homebrew 6.0.0 Released with Security and Performance Upgrades](#item-4) ⭐️ 8.0/10
5. [Demand Human Effort for Human Attention](#item-5) ⭐️ 8.0/10
6. [Xiaomi Open-Sources MiMo Code Coding Agent](#item-6) ⭐️ 8.0/10
7. [Lines of Code: A Vanity Metric in the AI Era](#item-7) ⭐️ 8.0/10
8. [Google Releases DiffusionGemma Open-Weight Model](#item-8) ⭐️ 8.0/10
9. [Android 17 Enforces Per-App Memory Limits, Killing Over-Limit Processes](#item-9) ⭐️ 8.0/10
10. [China Reviews Meta's Manus Acquisition, Founders Restricted](#item-10) ⭐️ 8.0/10
11. [macOS 27 Will Be Last to Fully Support Rosetta 2](#item-11) ⭐️ 8.0/10
12. [Petition to Withdraw Canada's Bill C-22](#item-12) ⭐️ 7.0/10
13. [DeltaDB Captures Code Changes Between Commits](#item-13) ⭐️ 7.0/10
14. [Waymo Premier Subscription Launches at $30/Month](#item-14) ⭐️ 7.0/10
15. [Datasette 1.0a33 Extends JSON Extras API](#item-15) ⭐️ 7.0/10
16. [Datasette Agent 0.2a0 Adds Interactive Tool Execution](#item-16) ⭐️ 7.0/10
17. [Jeremy Howard proposes counterintuitive AI safety approach](#item-17) ⭐️ 7.0/10
18. [Anthropic seeks new funding, valuation may hit $40B](#item-18) ⭐️ 7.0/10
19. [Meituan, Taobao Flash, JD Delivery Sign Pact on Cross-Platform Blacklist](#item-19) ⭐️ 7.0/10
20. [Instacart and OpenAI Launch In-Chat Checkout in ChatGPT](#item-20) ⭐️ 7.0/10
21. [Apple Shares Stolen iPhone Data with London Police](#item-21) ⭐️ 7.0/10
22. [SpaceX Orbital Data Center Plan Faces China Supply Hurdles](#item-22) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [AMD's Inadequate Fix for Critical RCE Vulnerability](https://mrbruh.com/amd2/) ⭐️ 9.0/10

A researcher disclosed a remote code execution vulnerability in AMD software that AMD initially refused to fix, then patched with a non-cryptographic CRC-32 check instead of proper cryptographic signature verification. This vulnerability could allow attackers to compromise servers via MITM or webserver compromise, affecting AMD's supply chain and user trust. The inadequate fix highlights ongoing security negligence in vendor responses. The patch uses CRC-32, which is designed for error detection, not cryptographic security, making it trivial for attackers to forge valid checksums. AMD also claimed signature verification was implemented, which was false.

hackernews · MrBruh · Jun 11, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48492215)

**Background**: CRC-32 is a cyclic redundancy check used to detect accidental data corruption, but it is not cryptographically secure and can be easily bypassed by an attacker. Cryptographic signature verification, such as RSA or ECDSA, is required to ensure the integrity and authenticity of downloaded executables.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cyclic_redundancy_check">Cyclic redundancy check - Wikipedia</a></li>
<li><a href="https://medium.com/@mark.benly/understanding-the-crc32-header-a-deep-dive-into-cyclic-redundancy-check-3b34d31585c7">Understanding the CRC32 Header: A Deep Dive into Cyclic Redundancy Check | by Mark Benly | Medium</a></li>

</ul>
</details>

**Discussion**: Commenters expressed frustration at AMD's response, calling the CRC-32 fix 'hilariously clueless' and noting AMD's history of poor software quality. Some debated the scope of bug bounty programs and the practicality of MITM attacks.

**Tags**: `#security`, `#vulnerability`, `#AMD`, `#RCE`, `#supply chain`

---

<a id="item-2"></a>
## [Anthropic Reverses Secret Policy Limiting AI Researchers](https://simonwillison.net/2026/Jun/11/anthropic-walks-back-policy/#atom-everything) ⭐️ 9.0/10

Anthropic has reversed a policy in Claude Fable 5 that secretly limited the effectiveness of responses for users engaged in frontier LLM development, making the safeguards visible and transparent. This reversal restores trust in Anthropic's commitment to transparency and ethical AI development, as the original policy could have silently sabotaged AI research and undermined user autonomy. Flagged requests will now visibly fall back to Opus 4.8 instead of silently limiting responses, and API users will receive a reason for refusal. Anthropic apologized for the wrong tradeoff between speed and transparency.

rss · Simon Willison · Jun 11, 03:45

**Background**: Claude Fable 5 is Anthropic's most capable widely released model, designed for demanding reasoning and agentic tasks. The original policy, hidden in the system card, would identify requests targeting frontier LLM development and limit effectiveness without notifying users, raising concerns about paternalism and trust.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://www.datacamp.com/blog/frontier-models">Frontier Models Explained: What Defines the Cutting Edge of AI | DataCamp</a></li>

</ul>
</details>

**Discussion**: Community comments expressed strong disapproval of the original policy, comparing it to Excel silently altering formulas and criticizing Anthropic's paternalistic approach. Some users remain skeptical, noting that invisible safeguards could still be secretly retained, and trust has been damaged.

**Tags**: `#AI ethics`, `#Anthropic`, `#policy`, `#AI research`, `#transparency`

---

<a id="item-3"></a>
## [Anthropic Launches Claude Fable 5 and Mythos 5 with Major Performance Gains](https://t.me/zaihuapd/41892) ⭐️ 9.0/10

Anthropic has released Claude Fable 5, a Mythos-class model made safe for general use, alongside Claude Mythos 5 for vetted cybersecurity partners. The new models deliver state-of-the-art performance across software engineering, knowledge work, vision, and scientific research benchmarks, while pricing for Fable 5 is more than 50% lower than the previous Mythos Preview. This release marks a significant step in making cutting-edge AI capabilities more accessible and affordable, potentially reshaping the competitive landscape for large language models. The built-in safety classifier that redirects sensitive queries to a less capable model (Opus 4.8) demonstrates a new approach to balancing performance and safety. Claude Fable 5 includes a safety classifier that, when triggered on topics like cybersecurity and biochemistry, switches responses to Opus 4.8, affecting about 5% of conversations. Claude Mythos 5, with fewer restrictions, is available only to a small group of vetted customers for tasks like vulnerability discovery.

telegram · zaihuapd · Jun 11, 07:45

**Background**: Anthropic's Claude models are large language models (LLMs) designed for safe and capable AI assistance. The 'Mythos' class represents Anthropic's most powerful models, previously reserved for specialized security research. 'Fable' is a new tier that brings Mythos-level capabilities to general users with additional safety guardrails.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://platform.claude.com/docs/en/about-claude/models/introducing-claude-fable-5-and-claude-mythos-5">Introducing Claude Fable 5 and Claude Mythos 5 - Claude API Docs</a></li>
<li><a href="https://aws.amazon.com/blogs/aws/anthropic-claude-fable-5-on-aws-mythos-class-capabilities-with-built-in-safeguards-now-available/">Anthropic Claude Fable 5 on AWS: Mythos-class capabilities with built-in safeguards now available | Amazon Web Services</a></li>

</ul>
</details>

**Discussion**: Community comments on Hacker News report mixed experiences: some praise Fable 5 for frontend tasks and reliability, while others note it still leaves small bugs and is expensive. A benchmark test recorded record timeouts and high cheating volume due to memorization of training data, raising concerns about benchmark validity.

**Tags**: `#Anthropic`, `#Claude`, `#AI模型`, `#大语言模型`, `#发布`

---

<a id="item-4"></a>
## [Homebrew 6.0.0 Released with Security and Performance Upgrades](https://brew.sh/2026/06/11/homebrew-6.0.0/) ⭐️ 8.0/10

Homebrew 6.0.0 introduces a new tap trust security mechanism, a faster default JSON API, Linux sandboxing, and initial support for macOS 27 (Golden Gate). As a widely-used package manager on macOS and Linux, this major release enhances security and performance, benefiting millions of developers. The new features address long-standing community requests and improve the user experience across platforms. The tap trust mechanism verifies the authenticity of third-party repositories, while the new JSON API reduces response size and latency. Linux sandboxing uses Bubblewrap to isolate build processes, and macOS 27 support is preliminary.

hackernews · mikemcquaid · Jun 11, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48490024)

**Background**: Homebrew is a free and open-source package manager that simplifies installing software on macOS and Linux. It uses 'taps' (third-party repositories) to extend its package collection, and the new trust mechanism helps prevent malicious packages. The JSON API is used by Homebrew's internal commands and external tools for faster data retrieval.

**Discussion**: Community members expressed gratitude for the maintainers' long-term dedication, with one user noting 16+ years of service. Some users discussed switching to or from alternatives like Nix and mise, citing trade-offs in reproducibility, package support, and UX. Others highlighted Homebrew's role in immutable Linux distributions like Bazzite.

**Tags**: `#homebrew`, `#package-manager`, `#macos`, `#linux`, `#security`

---

<a id="item-5"></a>
## [Demand Human Effort for Human Attention](https://tombedor.dev/human-attention-and-human-effort/) ⭐️ 8.0/10

A blog post argues that when requesting human attention, such as code reviews, one must demonstrate human effort, criticizing the flood of unrefined AI-generated pull requests that burden reviewers. This highlights a growing problem in collaborative software development where AI-generated content, if not refined, can overwhelm reviewers and reduce productivity, potentially harming team dynamics and code quality. The post emphasizes that reviewers are more likely to engage with PRs that show the author has invested effort, such as clear descriptions, focused changes, and thoughtful responses to feedback.

hackernews · jjfoooo4 · Jun 11, 23:01 · [Discussion](https://news.ycombinator.com/item?id=48497609)

**Background**: Code review is a critical practice in software development where team members examine each other's code changes before merging. With the rise of AI coding assistants like Claude and ChatGPT, developers can generate large volumes of code quickly, but this can lead to low-quality PRs that lack human oversight.

**Discussion**: Commenters share experiences of coworkers flooding teams with AI-generated PRs, leading to resentment and avoidance. Some suggest sharing prompts alongside AI output for reproducibility, while others argue the core issue is that many tasks are inherently meaningless, making AI use tempting but resulting in poor outcomes.

**Tags**: `#AI in software engineering`, `#code review`, `#collaboration`, `#productivity`, `#LLM usage`

---

<a id="item-6"></a>
## [Xiaomi Open-Sources MiMo Code Coding Agent](https://mimo.xiaomi.com/mimocode) ⭐️ 8.0/10

Xiaomi has released MiMo Code, a terminal-native AI coding agent, as open-source under the MIT license. It is a fork of OpenCode and adds persistent memory, subagent orchestration, and goal-driven autonomous loops. This move from a major tech company like Xiaomi signals a shift toward open-source AI developer tools, challenging closed-source alternatives like Claude Code. It could accelerate adoption of AI coding agents by reducing switching costs and increasing transparency. MiMo Code includes persistent memory for cross-session project understanding, intelligent context management, and self-improvement via dream/distill cycles. It supports multiple LLM providers, TUI, LSP, MCP, and plugins, and is available on GitHub.

hackernews · apeters · Jun 11, 14:27 · [Discussion](https://news.ycombinator.com/item?id=48490826)

**Background**: AI coding agents are tools that assist developers by writing, reading, and debugging code autonomously. OpenCode is an open-source terminal-based coding agent that MiMo Code forked from. Xiaomi's MiMo team previously developed the MiMo 2.5 language model.

<details><summary>References</summary>
<ul>
<li><a href="https://mimo.xiaomi.com/blog/mimo-code-long-horizon">mimo .xiaomi.com/blog/ mimo - code -long-horizon</a></li>
<li><a href="https://www.gizmochina.com/2026/06/11/xiaomi-mimo-code-open-source-terminal-ai-coding-agent/">Xiaomi announces new AI coding agent that actually remembers what...</a></li>

</ul>
</details>

**Discussion**: The community largely welcomes the open-source release, with users praising the added features like persistent memory and subagent orchestration. Some commenters argue that coding harnesses should be open-source, criticizing closed-source tools like Claude Code. A few users also promote their own compatible tools.

**Tags**: `#open-source`, `#AI coding agent`, `#Xiaomi`, `#LLM`, `#developer tools`

---

<a id="item-7"></a>
## [Lines of Code: A Vanity Metric in the AI Era](https://curlewis.co.nz/posts/lines-of-code-got-a-better-publicist/) ⭐️ 8.0/10

A blog post argues that lines of code (LoC) is a vanity metric, especially when inflated by AI agents, and calls for evidence of actual productivity gains rather than raw output. This critique challenges the growing trend of using LoC as a productivity metric in AI-assisted development, urging the industry to focus on quality and maintainability over sheer volume. The post highlights that AI agents can generate massive amounts of code quickly, but without evidence of corresponding value or quality, LoC becomes misleading. It calls for metrics that reflect actual problem-solving and user impact.

hackernews · RyeCombinator · Jun 11, 12:26 · [Discussion](https://news.ycombinator.com/item?id=48489402)

**Background**: Lines of code has long been criticized as a poor measure of software productivity because it rewards verbosity over efficiency. With the rise of AI code generation tools like GitHub Copilot, the metric has seen a resurgence in management discussions, often without the necessary context of code quality or business value.

**Discussion**: Commenters largely agree that LoC is a vanity metric, with some noting that AI-generated code often lacks maintainability. One commenter sarcastically referenced a Microsoft executive's proposal of 1 million LoC per engineer per month, while another pointed out that companies use AI as an excuse for layoffs rather than genuine productivity gains.

**Tags**: `#AI code generation`, `#software metrics`, `#productivity`, `#engineering culture`

---

<a id="item-8"></a>
## [Google Releases DiffusionGemma Open-Weight Model](https://simonwillison.net/2026/Jun/10/diffusiongemma/#atom-everything) ⭐️ 8.0/10

Google has released DiffusionGemma, an open-weight diffusion model for fast text generation, under the Apache 2 license, and NVIDIA is hosting it for free on their NIM cloud API. This release marks a significant return to diffusion-based text generation from Google, offering high-speed performance (over 500 tokens/second) and open accessibility, which could accelerate research and application development in efficient text generation. The model is named google/diffusiongemma-26B-A4B-it on Hugging Face, with 26 billion total parameters and 4 billion active parameters per token. In a test, it generated 2,409 tokens in 4.4 seconds, achieving at least 500 tokens/second.

rss · Simon Willison · Jun 10, 20:00

**Background**: Diffusion models are typically used for image generation, but they can also be applied to text by iteratively refining random noise into coherent sequences. Google previously experimented with a Gemini Diffusion model in May 2025, which achieved 857 tokens/second but was not further developed. The new DiffusionGemma is an open-weight model under the Gemma family, making it freely available for modification and use.

<details><summary>References</summary>
<ul>
<li><a href="https://build.nvidia.com/">Try NVIDIA NIM APIs</a></li>
<li><a href="https://developer.nvidia.com/nim">NIM for Developers | NVIDIA Developer</a></li>
<li><a href="https://free-llm.com/provider/nvidia-nim">NVIDIA NIM Free API (2026) | Models & Guide - Free-LLM</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (linked in the article) likely includes excitement about the open license and high speed, though no specific comments are provided here.

**Tags**: `#AI`, `#open-source`, `#text generation`, `#Google`, `#diffusion model`

---

<a id="item-9"></a>
## [Android 17 Enforces Per-App Memory Limits, Killing Over-Limit Processes](https://android-developers.googleblog.com/2026/06/prioritizing-memory-efficiency-steps-for-android-17.html) ⭐️ 8.0/10

Starting from Android 17, the system will set a per-app memory limit based on total device RAM, and processes exceeding the limit will be terminated immediately without a stack trace. Google also introduced the ProfilingManager API to collect heap dumps during exceptions or OOM in production. This policy change significantly impacts app development and memory management, forcing developers to optimize memory usage to prevent app termination. It improves overall device stability and multitasking experience by preventing a single app from degrading system performance. Google recommends enabling R8 optimization, using low-memory image formats like RGB_565, promptly recycling bitmaps, fixing memory leaks with LeakCanary, and responding to onTrimMemory callbacks. The ProfilingManager API is available on Android 15+ devices and supports heap dump collection in production.

telegram · zaihuapd · Jun 11, 05:30

**Background**: Android has long faced challenges with memory management, where a single app consuming excessive memory can slow down the entire system or cause other apps to be killed. Per-app memory limits have been discussed for years, but Android 17 is the first version to enforce them strictly. The new policy aims to balance app functionality with overall system health, especially on devices with limited RAM.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.android.com/reference/android/os/ProfilingManager">ProfilingManager | API reference | Android Developers</a></li>
<li><a href="https://android-developers.googleblog.com/2026/06/datadog-profilingmanager-performance-insights.html">Android Developers Blog: Datadog delivers millions of in-depth...</a></li>

</ul>
</details>

**Tags**: `#Android`, `#memory management`, `#app development`, `#performance`

---

<a id="item-10"></a>
## [China Reviews Meta's Manus Acquisition, Founders Restricted](https://t.me/zaihuapd/41895) ⭐️ 8.0/10

Chinese regulators are reviewing Meta's acquisition of AI startup Manus for potential investment violations, and have restricted Manus CEO Xiao Hong and Chief Scientist Ji Yichao from leaving the country. This marks a significant regulatory intervention in a major tech acquisition, highlighting China's tightening control over AI-related deals and potential geopolitical tensions between the US and China. The deal, announced in December 2024, was reportedly valued at around $2 billion. The founders were told they cannot leave China after meeting with the National Development and Reform Commission in Beijing this month.

telegram · zaihuapd · Jun 11, 10:00

**Background**: Manus is an autonomous AI agent developed by Butterfly Effect, a company founded in China and based in Singapore. Meta's acquisition aims to boost its AI offerings, but China's review suggests concerns over technology transfer or national security.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Manus_(AI_agent)">Manus ( AI agent) - Wikipedia</a></li>
<li><a href="https://news.google.com/stories/CAAqNggKIjBDQklTSGpvSmMzUnZjbmt0TXpZd1NoRUtEd2lCOTdxakVCR2FRVHVzSFJ3dm1pZ0FQAQ?hl=en-NG&gl=NG&ceid=NG:en">Google News - News about Manus • AI • Meta - Overview</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#Manus`, `#AI regulation`, `#acquisition`, `#China`

---

<a id="item-11"></a>
## [macOS 27 Will Be Last to Fully Support Rosetta 2](https://www.macrumors.com/2026/06/10/macos-golden-gate-last-to-support-intel-apps/) ⭐️ 8.0/10

Apple has announced that macOS 27 Golden Gate will be the last version to fully support Rosetta 2, with macOS 28 retaining only limited support for legacy Intel-dependent games. Additionally, macOS 27 will be the first version to require Apple silicon, meaning Intel Macs cannot upgrade to it. This marks the definitive end of Intel app compatibility on macOS, forcing developers and users to migrate to Universal or Apple silicon-native applications. It signals the final phase of Apple's transition away from Intel processors, which began in 2020. Rosetta 2 will remain fully functional in macOS 27, but from macOS 28 onward, only a subset of legacy Intel-based games that rely on unmaintained frameworks will be supported. Intel-based Macs will be unable to run macOS 27 or later versions.

telegram · zaihuapd · Jun 11, 10:45

**Background**: Rosetta 2 is a dynamic binary translator introduced in macOS Big Sur (2020) that allows Intel-based applications to run on Apple silicon Macs. It was part of Apple's transition from Intel processors to its own ARM-based chips. Universal 2 binaries, introduced at the same time, contain code for both Intel and Apple silicon architectures, enabling native performance on either platform.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rosetta_(software)">Rosetta (software)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_silicon">Apple silicon</a></li>
<li><a href="https://en.wikipedia.org/wiki/Universal_binary">Universal binary</a></li>

</ul>
</details>

**Tags**: `#macOS`, `#Rosetta 2`, `#Apple Silicon`, `#Intel Mac`, `#Software Compatibility`

---

<a id="item-12"></a>
## [Petition to Withdraw Canada's Bill C-22](https://www.ourcommons.ca/petitions/en/Petition/Sign/e-7416) ⭐️ 7.0/10

A petition has been launched on the Canadian House of Commons website calling for the withdrawal of Bill C-22, which critics argue threatens privacy and the tech sector. If passed, Bill C-22 could compel tech companies to build encryption backdoors, undermining digital security and privacy for Canadians and potentially affecting cross-border data flows with the U.S. The petition is part of ongoing parliamentary review, with the SECU Committee conducting clause-by-clause review and voting on amendments. Critics also link Bill C-22 to Bill C-34, which they say further erodes privacy.

hackernews · hmokiguess · Jun 11, 15:37 · [Discussion](https://news.ycombinator.com/item?id=48491830)

**Background**: Bill C-22 is a Canadian legislative proposal that would expand surveillance and data access powers. Critics argue it forces tech companies to weaken encryption, harming privacy and innovation. The bill is currently under parliamentary review.

<details><summary>References</summary>
<ul>
<li><a href="https://www.todayville.com/bill-c-22-surveils-ordinary-canadians-while-leaving-cartel-networks-untouched/">Bill C - 22 Surveils Ordinary Canadians While Leaving... - Todayville</a></li>
<li><a href="https://news.spreely.com/canada-c-22-compels-tech-firms-to-build-encryption-backdoors/">Canada C - 22 Compels Tech Firms To Build Encryption Backdoors</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about the petition's impact but emphasize the importance of raising noise. They note a SECU committee meeting on C-22 and link to related bills like C-34, warning that Canada's tech sector will suffer if the bill passes.

**Tags**: `#privacy`, `#Canada`, `#legislation`, `#technology policy`

---

<a id="item-13"></a>
## [DeltaDB Captures Code Changes Between Commits](https://zed.dev/blog/introducing-deltadb) ⭐️ 7.0/10

Zed blog introduces DeltaDB, a tool that records every operation between Git commits to capture the full process of writing software, arguing that this intermediate state is more informative than the final commits. This challenges the common practice of only reviewing final commits, potentially improving code review and collaboration by revealing the true evolution of code. It could also influence how developers think about version control and documentation of their work. DeltaDB captures every keystroke and edit, not just snapshots, providing a granular timeline of changes. The tool is designed to be used alongside Git, not as a replacement, and aims to make the 'messy soup' of development visible and analyzable.

hackernews · jeremy_k · Jun 11, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48492533)

**Background**: Traditional version control systems like Git record commits as snapshots of the codebase at specific points. However, the actual process of writing code involves many intermediate steps, experiments, and deletions that are lost in the final commit. DeltaDB aims to preserve this process for better understanding and collaboration.

**Discussion**: Comments are mixed: some argue that intermediate changes are messy and not useful, preferring to craft clean commits via rebase. Others express privacy concerns, feeling that recording every keystroke is intrusive. A few suggest that Git already supports frequent auto-commits and merging strategies to achieve similar goals.

**Tags**: `#software engineering`, `#version control`, `#code review`, `#developer tools`, `#git`

---

<a id="item-14"></a>
## [Waymo Premier Subscription Launches at $30/Month](https://waymo.com/blog/2026/06/waymo-premier/) ⭐️ 7.0/10

Waymo has launched Waymo Premier, a $30/month subscription service that offers priority access and cashback on rides. This marks a significant step in autonomous ride-hailing monetization, potentially reshaping how users access and pay for self-driving services. The subscription costs $30 per month and includes priority ride access and cashback on fares, with the cashback benefit being particularly attractive for business travelers who expense rides.

hackernews · boulos · Jun 11, 16:10 · [Discussion](https://news.ycombinator.com/item?id=48492304)

**Background**: Waymo is a leading autonomous vehicle company that operates a ride-hailing service in select U.S. cities. Subscription models are common in software and transportation, but this is one of the first for autonomous ride-hailing.

**Discussion**: Community comments are mixed: some see the cashback as a perk for business travelers, while others question the value compared to public transit. Concerns about safety and the inability to control the vehicle in emergencies were also raised.

**Tags**: `#autonomous vehicles`, `#subscription service`, `#ride-hailing`, `#Waymo`, `#transportation`

---

<a id="item-15"></a>
## [Datasette 1.0a33 Extends JSON Extras API](https://simonwillison.net/2026/Jun/11/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a33 extends the `?_extra=` pattern to queries and rows, and the feature is now documented in the JSON API documentation. This release is a significant step toward a stable 1.0, providing a more consistent and powerful API for Datasette users, and improving developer experience with better documentation. The `?_extra=` pattern was originally introduced in Datasette 1.0a3 for tables; this alpha extends it to queries and rows, allowing users to request additional metadata in JSON responses.

rss · Simon Willison · Jun 11, 15:26

**Background**: Datasette is an open-source tool for exploring and publishing tabular data. It provides a JSON API for querying databases. The `?_extra=` parameter lets users request additional fields like column types or row counts in API responses.

**Tags**: `#datasette`, `#python`, `#open-source`, `#API`, `#release`

---

<a id="item-16"></a>
## [Datasette Agent 0.2a0 Adds Interactive Tool Execution](https://simonwillison.net/2026/Jun/10/datasette-agent/#atom-everything) ⭐️ 7.0/10

Datasette Agent 0.2a0 introduces the ability for tools to ask users questions mid-execution via a new ToolContext object and ask_user() method, with conversation persistence across server restarts. It also includes a new built-in save_query tool that requires human approval before saving SQL queries as Datasette stored queries. This release enables a novel interactive pattern for AI agents, allowing them to pause and request user input during execution, which improves safety and user control. The persistence feature ensures that suspended conversations survive server restarts, making the tool more robust for real-world data exploration workflows. Tools declare a context parameter to receive a ToolContext object, and can call await context.ask_user(...) with options for yes/no, multiple-choice, or free-text questions. While a question is unanswered, the agent turn suspends and the question renders as a form in the chat UI, persisting to the internal database. Once answered, the tool re-executes from the top with stored answers replayed.

rss · Simon Willison · Jun 10, 23:57

**Background**: Datasette Agent is an AI-powered tool for exploring and querying data in Datasette, an open-source data exploration and publishing tool. The new ask_user() feature was enabled by a recent LLM alpha release built with Claude Fable 5. This release is an early alpha (0.2a0), indicating it is still experimental.

**Tags**: `#datasette`, `#AI agents`, `#tool interaction`, `#open source`, `#data exploration`

---

<a id="item-17"></a>
## [Jeremy Howard proposes counterintuitive AI safety approach](https://simonwillison.net/2026/Jun/10/jeremy-howard/#atom-everything) ⭐️ 7.0/10

Jeremy Howard proposed that the lab with the top-ranked AI model must refrain from using it for frontier AI research, while granting access to everyone else, to slow recursive self-improvement and reduce power imbalance. This proposal challenges the dominant approach to AI safety, where leading labs like Anthropic use their own models for frontier research, potentially accelerating advancement and concentrating power. If adopted, it could fundamentally alter the dynamics of AI development and governance. Howard specifically criticized Anthropic for choosing the opposite path: allowing themselves to use their top model for frontier research while sabotaging others. He clarified that he personally favors democratizing AI rather than slowing it, but argues that those who claim to want slowdown should lead by example.

rss · Simon Willison · Jun 10, 15:23

**Background**: Recursive self-improvement (RSI) refers to a process where an AI system rewrites its own code to enhance its capabilities, potentially leading to an intelligence explosion. Frontier AI research involves pushing the boundaries of AI capabilities, often using the most advanced models. The debate around AI safety includes concerns about uncontrolled acceleration and concentration of power among a few labs.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Recursive_self-improvement">Recursive self-improvement</a></li>

</ul>
</details>

**Tags**: `#AI safety`, `#recursive self-improvement`, `#power imbalance`, `#frontier AI`, `#Anthropic`

---

<a id="item-18"></a>
## [Anthropic seeks new funding, valuation may hit $40B](https://t.me/zaihuapd/41888) ⭐️ 7.0/10

Anthropic is in talks to raise a new funding round that could value the company between $30 billion and $40 billion, doubling its valuation from earlier this year. This funding round underscores the intense competition in the AI industry, with Anthropic and OpenAI both raising massive capital to scale their large language models and capture market share. Anthropic generates revenue primarily by providing access to its conversational AI, Claude. Meanwhile, OpenAI is also raising $5-7 billion at a valuation near $150 billion.

telegram · zaihuapd · Jun 11, 04:45

**Background**: Anthropic is a leading AI company founded by former OpenAI employees, focused on building safe and capable AI systems. Its flagship product, Claude, competes directly with OpenAI's GPT models. The company's rapid valuation growth reflects strong investor confidence in the AI sector.

**Tags**: `#Anthropic`, `#funding`, `#AI`, `#valuation`, `#Claude`

---

<a id="item-19"></a>
## [Meituan, Taobao Flash, JD Delivery Sign Pact on Cross-Platform Blacklist](https://finance.sina.com.cn/jjxw/2026-06-11/doc-iniazpqt0741536.shtml) ⭐️ 7.0/10

Meituan, Taobao Flash Purchase, and JD Delivery jointly signed the Guangdong Province Online Catering Industry High-Quality Development and Food Safety Self-Discipline Convention, which for the first time proposes a cross-platform blacklist sharing mechanism to enforce joint restrictions on severely violating merchants, achieving 'one violation, restricted across all networks'. This marks a significant step in platform governance and food safety, as it creates a unified deterrent across major food delivery platforms, potentially reducing repeat offenses and improving consumer trust. It also signals a shift from passive compliance to proactive self-regulation in the industry. The convention consists of five chapters and 21 articles, covering platform responsibilities, merchant management, delivery personnel care, and social co-governance. It was signed under the witness of the Guangdong Provincial Market Supervision Administration.

telegram · zaihuapd · Jun 11, 11:30

**Background**: Online food delivery platforms in China have faced challenges with rogue merchants that violate food safety or other regulations, often moving between platforms to evade penalties. The new cross-platform blacklist sharing mechanism aims to close this loophole by ensuring that a merchant banned on one platform is also restricted on others.

<details><summary>References</summary>
<ul>
<li><a href="https://news.dayoo.com/guangdong/202606/11/139996_54968763.htm">news.dayoo.com/guangdong/202606/11/139996_54968763.htm</a></li>

</ul>
</details>

**Tags**: `#platform governance`, `#food safety`, `#e-commerce`, `#regulation`

---

<a id="item-20"></a>
## [Instacart and OpenAI Launch In-Chat Checkout in ChatGPT](https://t.me/zaihuapd/41900) ⭐️ 7.0/10

On December 8, 2025, Instacart and OpenAI announced a deeper partnership, launching the first integrated grocery shopping app with instant checkout within ChatGPT, allowing users to browse, add to cart, and complete payment without leaving the chat interface. This marks a significant shift in e-commerce by embedding a full purchasing flow inside an AI chatbot, potentially transforming how users shop online and challenging traditional e-commerce platforms by reducing friction and keeping users within the AI ecosystem. The feature leverages Instacart's real-time delivery network and OpenAI's advanced models; it is the first such integration to enable checkout directly in ChatGPT, with OpenAI reportedly taking a small commission from each sale instead of charging per click.

telegram · zaihuapd · Jun 11, 13:15

**Background**: Instacart is North America's largest online grocery and instant delivery platform, offering end-to-end service from selection to delivery. OpenAI's ChatGPT has evolved from a conversational AI into a platform capable of executing tasks like shopping, with the new instant checkout feature representing a move toward 'conversational commerce' where purchases happen seamlessly within chat.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eesel.ai/blog/chatgpt-instant-checkout">A guide to ChatGPT Instant Checkout : What it means for... | eesel AI</a></li>
<li><a href="https://www.eesel.ai/blog/chatgpt-checkout">ChatGPT Checkout is changing e-commerce: Here's what... - eesel AI</a></li>
<li><a href="https://www.linkedin.com/posts/modern-retail_marketplace-briefing-why-chatgpt-checkout-activity-7379961068925902848-B259">OpenAI launches ChatGPT checkout feature , challenges... | LinkedIn</a></li>

</ul>
</details>

**Tags**: `#AI`, `#e-commerce`, `#ChatGPT`, `#Instacart`, `#OpenAI`

---

<a id="item-21"></a>
## [Apple Shares Stolen iPhone Data with London Police](https://www.express.co.uk/life-style/science-technology/2215942/apple-launches-major-iphone-update) ⭐️ 7.0/10

Apple has entered a data-sharing agreement with the London Metropolitan Police, providing stolen device identifiers to track reconnection to networks, and has enabled 'Stolen Device Protection' by default in recent software updates. This collaboration has contributed to an 18% reduction in phone thefts in London (14,000 fewer incidents from June 2025 to May 2026), highlighting the potential of public-private data sharing to combat crime while raising privacy concerns. The police provide Apple with identifiers of stolen devices, which Apple uses to block reactivation or track resale. The Metropolitan Police is now pushing for legislation requiring phone companies to share theft data and render stolen devices unusable.

telegram · zaihuapd · Jun 12, 00:24

**Background**: Stolen iPhone data sharing involves law enforcement providing unique device identifiers (like IMEI) to Apple, which then flags those devices in its activation servers. 'Stolen Device Protection' is a feature that requires biometric authentication for sensitive actions, making stolen iPhones harder to use or resell.

**Tags**: `#Apple`, `#privacy`, `#law enforcement`, `#data sharing`, `#security`

---

<a id="item-22"></a>
## [SpaceX Orbital Data Center Plan Faces China Supply Hurdles](https://www.bloomberg.com/opinion/articles/2026-06-11/spacex-s-critical-minerals-plan-runs-through-china) ⭐️ 7.0/10

SpaceX plans to launch 100 GW of solar-powered AI data centers into orbit annually starting in 2030, requiring thousands of launches and about 1 million tons of payload capacity, but the plan is challenged by China's dominance in critical minerals like gallium and polysilicon. This highlights a significant geopolitical and supply chain risk for SpaceX's ambitious orbital infrastructure, which could delay or complicate the deployment of space-based AI computing. It also underscores the broader challenge of reducing reliance on Chinese materials for advanced technology projects. Space solar cells may involve gallium arsenide or polysilicon, and China dominates global production of gallium and solar-grade polysilicon. SpaceX also holds U.S. military contracts, making reliance on Chinese hardware a potential security concern.

telegram · zaihuapd · Jun 12, 01:14

**Background**: Orbital data centers are proposed facilities in space that use space-based solar power to run AI computations, overcoming Earth's energy and land constraints. The concept builds on upgraded Starlink satellites and has roots in military space architectures like the Strategic Defense Initiative's Brilliant Pebbles program. Critical minerals such as gallium are essential for high-efficiency solar cells used in space.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Orbital_data_center">Orbital data center</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#orbital data center`, `#supply chain`, `#critical minerals`, `#AI`

---