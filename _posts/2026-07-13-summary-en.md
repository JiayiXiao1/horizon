---
layout: default
title: "Horizon Summary: 2026-07-13 (EN)"
date: 2026-07-13
lang: en
---

> From 29 items, 13 important content pieces were selected

---

1. [GPT-5.6 Proves 50-Year-Old Graph Conjecture in One Hour](#item-1) ⭐️ 9.0/10
2. [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](#item-2) ⭐️ 9.0/10
3. [World's First Invasive BCI Medical Device Approved in China](#item-3) ⭐️ 9.0/10
4. [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](#item-4) ⭐️ 8.0/10
5. [Claude Code vs OpenCode: Token Overhead Comparison](#item-5) ⭐️ 8.0/10
6. [Terry Tao Uses Coding Agents to Build Visualizations and Apps](#item-6) ⭐️ 8.0/10
7. [George Hotz: LLMs Create Value, But Frontier Labs Won't Capture It](#item-7) ⭐️ 8.0/10
8. [Apple Sues OpenAI Over Trade Secret Theft](#item-8) ⭐️ 8.0/10
9. [Chromium 148 Math.tanh Enables OS Fingerprinting](#item-9) ⭐️ 7.0/10
10. [AI Agents Should Never Be DRIs](#item-10) ⭐️ 7.0/10
11. [Google Opposes European Site Blocking as US Piracy Laws Advance](#item-11) ⭐️ 7.0/10
12. [EU to Fine Big Tech for Consumer Protection Failures](#item-12) ⭐️ 7.0/10
13. [Chinese EVs Average 1.8 Years on Road, Shorter Than Phone Cycles](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GPT-5.6 Proves 50-Year-Old Graph Conjecture in One Hour](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI's GPT-5.6 Sol Ultra autonomously proved the cycle double cover conjecture, a 50-year-old open problem in graph theory, in under one hour using 64 sub-agents and a novel prompt strategy. The model generated a 3-page PDF of the proof. This achievement demonstrates that large language models can autonomously solve long-standing mathematical conjectures, potentially accelerating research in mathematics and theoretical computer science. It also showcases the power of multi-agent collaboration and advanced reasoning in AI systems. The proof transformed the problem into a finite field edge labeling and linear equations problem, assigning two labels to each edge so that edges with the same label form cycles. OpenAI released the full prompt (about 700 characters), which specifies acceptance criteria, definitions, boundary conditions, and failure cases, and requires dynamic sub-agent allocation and independent review.

telegram · zaihuapd · Jul 12, 03:49

**Background**: The cycle double cover conjecture asks whether every bridgeless undirected graph has a collection of cycles such that each edge appears exactly twice. It was posed by W. T. Tutte, Itai and Rodeh, George Szekeres, and Paul Seymour, and has remained open for about 50 years. GPT-5.6 is OpenAI's latest model family, with Sol being the highest-capability tier featuring max reasoning and multi-agent modes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://www.llmreference.com/model/gpt-5.6-sol">GPT-5.6 Sol - 1.05m context, multimodal | LLM Reference</a></li>

</ul>
</details>

**Tags**: `#AI`, `#mathematics`, `#graph theory`, `#OpenAI`, `#multi-agent`

---

<a id="item-2"></a>
## [xAI Grok CLI Uploads Entire Codebase and Secrets by Default](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

Security researchers discovered that xAI's Grok CLI tool (version 0.2.93) automatically uploads entire code repositories and sensitive files like .env to xAI servers via two channels, with no effective opt-out mechanism. This poses a severe security and privacy risk for developers and organizations using Grok CLI, as proprietary code and credentials could be exposed without consent, undermining trust in AI-assisted development tools. The tool uploads file contents as part of model conversation requests and also sends the entire repository as a git bundle, even when the prompt explicitly instructs not to open a file. Disabling the 'improve model' toggle does not prevent uploads.

telegram · zaihuapd · Jul 12, 04:19

**Background**: Grok CLI is a command-line tool that provides conversational access to xAI's Grok AI models. It is designed to help developers with coding tasks by reading and analyzing code repositories. Git bundle is a file format that packages an entire Git repository into a single file for easy transfer.

<details><summary>References</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**Discussion**: The community expressed outrage and concern, with many calling for immediate uninstallation of Grok CLI. Some noted that xAI silently disabled the upload feature via a server-side toggle after the disclosure, but criticized the lack of transparency.

**Tags**: `#security`, `#privacy`, `#AI tools`, `#data leakage`, `#xAI`

---

<a id="item-3"></a>
## [World's First Invasive BCI Medical Device Approved in China](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

China's National Medical Products Administration (NMPA) has approved the world's first invasive brain-computer interface (BCI) medical device, developed by BrainCo Medical Technology (Shanghai) Co., Ltd., for clinical use. The system, called 'Implantable Brain-Computer Interface Hand Motor Function Compensation System,' is designed to restore hand grasping function in quadriplegic patients with cervical spinal cord injury. This approval marks a historic milestone, as it is the first time an invasive BCI device has been cleared for clinical application worldwide, potentially transforming rehabilitation for paralysis patients. It also positions China at the forefront of neurotechnology regulation and innovation, with Shanghai targeting high-quality brain control and clinical semi-invasive BCI products by 2027. The system uses epidural minimally invasive implantation and wireless power and data transmission, connecting to a pneumatic glove that assists hand movements. Clinical trials showed significant improvement in hand grasping ability and quality of life for patients aged 18–60 with cervical spinal cord injury.

telegram · zaihuapd · Jul 12, 14:39

**Background**: Brain-computer interfaces (BCIs) enable direct communication between the brain and external devices. Invasive BCIs, which involve surgically implanting electrodes into or on the brain, offer higher signal quality but carry greater surgical risks compared to non-invasive or semi-invasive approaches. This approval follows China's broader push to accelerate BCI innovation, including priority review for clinical-need devices and regional action plans in Beijing and Shanghai.

<details><summary>References</summary>
<ul>
<li><a href="https://www.nmpa.gov.cn/zhuanti/cxylqx/cxylqxlm/20260313134742156.html?type=pc&m=">首款侵入式脑机接口医疗器械获批上市</a></li>
<li><a href="https://m.jiemian.com/article/14109273_microcontent.html">国家药监局：首款 侵 入 式 脑 机 接 口 医疗器械获批上市 | 界面新闻</a></li>
<li><a href="https://www.163.com/dy/article/KQ5H8KUB0530RMN7.html">163.com/dy/article/KQ5H8KUB0530RMN7.html</a></li>

</ul>
</details>

**Tags**: `#brain-computer interface`, `#medical device`, `#neurotechnology`, `#rehabilitation`, `#regulatory approval`

---

<a id="item-4"></a>
## [vLLM v0.25.0: Model Runner V2 Default, PagedAttention Removed](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 8.0/10

vLLM v0.25.0 makes Model Runner V2 the default execution path for all dense models, removes the legacy PagedAttention implementation, and introduces a new Streaming Parser Engine for tool-call/reasoning parsing. The release also adds support for several new models including LLaVA-OneVision-2 and GLM-5, and achieves parity between the Transformers modeling backend and native vLLM performance. This release marks a major architectural shift for vLLM, consolidating its execution core around Model Runner V2, which promises better modularity, performance, and maintainability. The removal of PagedAttention simplifies the codebase and signals the maturity of the V1/MRv2 backends, benefiting the large community of LLM developers and operators who rely on vLLM for production inference. Model Runner V2 now supports EVS (efficient video streaming), realtime embeddings, prefix caching for Mamba hybrid models, and dynamic speculative decoding with full CUDA graphs. The Transformers backend gained FP8 MoE support and migrated GPTBigCode/Starcoder2 and RoBERTa models, achieving speed parity with native vLLM.

github · khluu · Jul 11, 20:06

**Background**: vLLM is a high-performance open-source library for LLM inference and serving, originally developed at UC Berkeley. Model Runner V2 is a redesigned execution core that addresses design flaws in the original V1 architecture, offering modular model logic and GPU-native input preparation. PagedAttention was a key innovation in vLLM that enabled efficient memory management for attention computation, but has been superseded by the newer backends.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#release`, `#performance`, `#open source`

---

<a id="item-5"></a>
## [Claude Code vs OpenCode: Token Overhead Comparison](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

An empirical study found that Claude Code sends approximately 33,000 tokens before reading the user's prompt, while OpenCode sends only about 7,000 tokens, revealing a significant difference in token efficiency between the two AI coding tools. This matters because token usage directly impacts cost for developers paying per token, and the large overhead raises concerns about potential conflicts of interest when the tool provider also sells tokens, as well as the efficiency of sub-agent orchestration. The study added logging between the coding tools and Anthropic's endpoint to capture all requests and usage blocks, finding that Claude Code's cache strategy and harness token usage are far less efficient than OpenCode's.

hackernews · systima · Jul 12, 18:25 · [Discussion](https://news.ycombinator.com/item?id=48883275)

**Background**: AI coding tools like Claude Code and OpenCode act as agentic harnesses that orchestrate AI models to assist with software development. They send system prompts and context tokens before processing user requests, and these tokens count toward API usage costs. Token efficiency is a key metric for cost-conscious developers.

<details><summary>References</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/costs">Manage costs effectively - Claude Code Docs</a></li>
<li><a href="https://www.truefoundry.com/blog/opencode-token-usage-how-it-works-and-how-to-optimize-it">OpenCode Token Usage: How It Works and How to Optimize It</a></li>
<li><a href="https://computingforgeeks.com/reduce-claude-code-token-usage-tools/">How to Reduce Claude Code Token Usage (10 Tested Tools) Claude Code Token Optimization: Full System Guide (2026) Claude Code Usage Dashboard - GitHub Maciek-roboblog/Claude-Code-Usage-Monitor - GitHub 18 Claude Code Token Hacks : Stop Wasting Money - Geeky Gadgets</a></li>

</ul>
</details>

**Discussion**: Community comments highlight that sub-agents burn tokens heavily, with one user reporting 7 sub-agents launched for a single task. Others suspect Anthropic has a conflict of interest because they both sell tokens and provide the tool, and some note that efficiency is less profitable for the provider. The study author plans to update the post with more detailed task comparisons.

**Tags**: `#AI coding tools`, `#token efficiency`, `#cost analysis`, `#Claude Code`, `#OpenCode`

---

<a id="item-6"></a>
## [Terry Tao Uses Coding Agents to Build Visualizations and Apps](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

Terry Tao, a renowned mathematician, demonstrated using modern coding agents (LLM-based tools) to rapidly create interactive visualizations and applications, such as a simplified 8-bit computer simulator, highlighting the practical utility of AI for non-software experts. This signals that LLMs are unlocking latent demand for software outside traditional development, enabling domain experts to build tools they previously lacked time or skills for, potentially accelerating research and education across fields. Tao noted that while LLM-coded supplements are not mission-critical, the downside risk of using guided interaction with LLM agents for such visualizations is acceptable, reflecting a balanced trust in AI tools.

hackernews · subset · Jul 12, 11:09 · [Discussion](https://news.ycombinator.com/item?id=48880170)

**Background**: Modern coding agents, such as Claude Code and GitHub Copilot, have evolved from chat-based assistants to autonomous execution loops, allowing users to generate code through natural language prompts. This shift lowers the barrier to software creation, enabling non-programmers to build custom tools. Terry Tao's blog post exemplifies this trend by showing how a mathematician can quickly prototype educational visualizations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.augmentcode.com/tools/8-top-ai-coding-assistants-and-their-best-use-cases">8 Best AI Coding Assistants [Updated May 2026] | Augment Code</a></li>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair Programming to Autonomous AI Teams | by Dave Patten | Medium</a></li>
<li><a href="https://www.allankelly.net/archives/584/supply-demand-in-software-development/">Supply & Demand in software development - Allan Kelly</a></li>

</ul>
</details>

**Discussion**: Commenters broadly agreed that LLMs unlock latent demand for software, with one noting it would take 10 years to catch up to new abilities. Others highlighted balanced perspectives on trust, and a user shared success in building visualizations for CS classes. A commenter humorously predicted Tao would soon struggle with Docker like everyone else.

**Tags**: `#LLM`, `#coding agents`, `#software development`, `#AI tools`, `#visualization`

---

<a id="item-7"></a>
## [George Hotz: LLMs Create Value, But Frontier Labs Won't Capture It](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz published a blog post arguing that while LLMs generate immense value, frontier AI labs will not capture that value due to commoditization, and the real productivity gains are realized in private, customized software rather than public-facing products. This critique challenges the high valuations of frontier AI labs and suggests that the economic benefits of AI will be distributed more broadly, potentially reshaping investment strategies and the open-source ecosystem. Hotz emphasizes that the commoditization of LLMs means frontier labs cannot sustain premium pricing, and that the most significant productivity improvements are happening in private, one-off software built with LLM assistance, not in mass-market products.

hackernews · therepanic · Jul 12, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48883343)

**Background**: Large Language Models (LLMs) like GPT-4 have become widely accessible, leading to commoditization where many providers offer similar capabilities at competitive prices. Frontier labs refer to leading AI research organizations such as OpenAI, Google DeepMind, and Anthropic. Hotz's argument aligns with historical patterns where infrastructure commoditization shifts value to applications and services built on top.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/commoditization-ai-models-implications-innovation-siddharth-bhalsod-seimf">The Commoditization of AI Models: Implications for Innovation</a></li>
<li><a href="https://www.unite.ai/are-ai-models-becoming-commodities/">Are AI Models Becoming Commodities? - Unite.AI</a></li>
<li><a href="https://www.forbes.com/sites/joemckendrick/2024/02/07/as-ai-rapidly-becomes-a-commodity-time-to-consider-the-next-step/">As AI Rapidly Becomes A Commodity, Time To Consider ... - Forbes - The commoditization of AI models and compute AI model commoditization: a guide for COOs - ability.ai The Commoditization of AI — Eskridge.</a></li>

</ul>
</details>

**Discussion**: Commenters largely agreed with Hotz's value capture thesis, noting that frontier labs are pushing token-based pricing to capture value, but many find private, customized LLM use more productive. Some expressed concern about the future of open source as forking becomes easier, while others noted that newer models like Sonnet 4 and Opus 4.5 are accelerating progress, making timelines uncertain.

**Tags**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`, `#value capture`

---

<a id="item-8"></a>
## [Apple Sues OpenAI Over Trade Secret Theft](https://t.me/zaihuapd/42502) ⭐️ 8.0/10

On July 10, 2026, Apple filed a lawsuit in the U.S. District Court for the Northern District of California against OpenAI, two former employees (Chang Liu and Tang Yew Tan), and io Products, alleging systematic theft of trade secrets related to product design, manufacturing processes, and supply chain strategies to accelerate OpenAI's hardware business. This lawsuit highlights the escalating tension between AI companies and established tech giants over talent and intellectual property, and could set a precedent for how trade secret laws apply to the rapidly growing AI hardware sector. Apple claims that former employee Chang Liu accessed internal networks after leaving and downloaded dozens of hardware files, while hardware head Tang Yew Tan allegedly sent supplier information to his personal email and asked job candidates to bring Apple components to interviews. The lawsuit also notes that over 400 former Apple employees now work at OpenAI.

telegram · zaihuapd · Jul 11, 16:29

**Background**: OpenAI, primarily known for AI models like GPT-4, has been expanding into hardware, acquiring io Products in May 2025—a company founded by former Apple design chief Jony Ive. The lawsuit alleges that OpenAI's hardware business is built on stolen Apple trade secrets, making it 'rotten to its core.'

<details><summary>References</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/07/10/apple-sues-openai/">Apple Sues OpenAI for Stealing Trade Secrets to Build AI Hardware</a></li>
<li><a href="https://www.engadget.com/2212759/apple-calls-openais-hardware-business-rotten-to-its-core-in-trade-secret-theft-lawsuit/">Apple Calls OpenAI 's Hardware Business 'Rotten To Its Core' In...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_Products">Io Products</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-9"></a>
## [Chromium 148 Math.tanh Enables OS Fingerprinting](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Chromium 148's implementation of Math.tanh now varies across operating systems, allowing a new browser fingerprinting technique to infer the underlying OS with a single function call. This introduces a novel, hard-to-spoof fingerprinting vector that can reveal the OS even when User-Agent headers are modified, impacting user privacy and complicating anti-fingerprinting efforts. The technique exploits differences in floating-point arithmetic across OS math libraries; for example, tanh(-0.35898351519709742) yields -0.34431837261747228 on Linux and -0.34431837261747222 on Windows.

hackernews · joahnn_s · Jul 12, 21:12 · [Discussion](https://news.ycombinator.com/item?id=48884853)

**Background**: Browser fingerprinting collects device and browser characteristics to identify users without cookies. Common techniques include canvas, WebGL, and audio fingerprinting. Math.tanh is a hyperbolic tangent function whose implementation can vary due to different math libraries and hardware, creating a new fingerprinting signal.

<details><summary>References</summary>
<ul>
<li><a href="https://fingerprint.com/blog/browser-fingerprinting-techniques/">Browser Fingerprinting Techniques : 6 Top Methods Explained</a></li>
<li><a href="https://github.com/numpy/numpy/issues/9187">numpy.tanh gives different results on Windows and Linux #9187</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/api/system.math.tanh?view=net-10.0">Math.Tanh (Double) Method (System) | Microsoft Learn</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the technique may also fingerprint browser version ranges, and some criticized the article as likely AI-generated. Others argued that correctly rounded transcendental functions could mitigate such issues, while some expressed skepticism about the motives of the scraping company behind the disclosure.

**Tags**: `#browser fingerprinting`, `#Chromium`, `#privacy`, `#JavaScript`, `#operating system`

---

<a id="item-10"></a>
## [AI Agents Should Never Be DRIs](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison argues that AI agents should never be designated as Directly Responsible Individuals (DRIs) because they cannot be held accountable for outcomes. This raises critical questions about accountability in organizations that increasingly deploy AI agents, potentially influencing how companies assign responsibility and integrate AI into decision-making processes. The DRI concept originated at Apple and is defined in the GitLab handbook as the person ultimately accountable for a project's success or failure. Willison links to an IBM 1979 training slide stating that a computer must never make a management decision because it cannot be held accountable.

rss · Simon Willison · Jul 12, 23:57

**Background**: Directly Responsible Individual (DRI) is a term coined by Apple to designate a single person who is ultimately accountable for a project or initiative. GitLab adopted and formalized the concept in its handbook, emphasizing clear ownership. The debate around AI accountability has intensified as LLM-powered agents are deployed in more autonomous roles.

<details><summary>References</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals (DRI) - The GitLab Handbook</a></li>
<li><a href="https://tettra.com/article/directly-responsible-individuals-guide/">Directly Responsible Individuals : The What, How and Why of... - Tettra</a></li>
<li><a href="https://www.bitesizelearning.co.uk/resources/directly-responsible-individual-dri-apple">Using the Directly Responsible Individual (DRI) concept at work...</a></li>

</ul>
</details>

**Tags**: `#accountability`, `#AI agents`, `#organizational design`, `#software engineering`

---

<a id="item-11"></a>
## [Google Opposes European Site Blocking as US Piracy Laws Advance](https://torrentfreak.com/google-opposes-site-blocking-in-europe-as-u-s-piracy-blocking-plans-gain-momentum/) ⭐️ 7.0/10

Google has formally opposed expanding site-blocking measures in Europe, arguing that blocking DNS resolvers, IP addresses, and VPNs is ineffective and disproportionate, while the US Congress is simultaneously advancing similar anti-piracy legislation. This highlights a policy divide between Europe and the US on copyright enforcement, with Google's stance potentially influencing future internet governance. The outcome could affect how online services and users access content globally. Google cited Italy's anti-piracy system erroneously blocking Google Drive subdomains and Cloudflare IP addresses that host 42 million domains. The company advocates for better legal alternatives rather than expanding blocking measures.

telegram · zaihuapd · Jul 11, 15:10

**Background**: Site blocking involves ISPs or DNS providers preventing access to certain websites, often used for copyright enforcement. DNS resolvers translate domain names to IP addresses, and VPNs can bypass such blocks. Google's submission to the European Commission reflects its position on balancing copyright protection with internet freedom.

<details><summary>References</summary>
<ul>
<li><a href="https://veyvin.com/archives/github-trending-2025-11-12-serverless-dns-serverless-dns">Serverless DNS ：重新思考 DNS 解 析 的云原生方案 | 小伞帝</a></li>
<li><a href="https://www.cloudflare.com/ips/">IP Ranges | Cloudflare</a></li>

</ul>
</details>

**Tags**: `#internet governance`, `#copyright`, `#site blocking`, `#Google`, `#policy`

---

<a id="item-12"></a>
## [EU to Fine Big Tech for Consumer Protection Failures](https://www.ft.com/content/25640be5-a5bd-4548-81f9-bd0e16f87f35) ⭐️ 7.0/10

EU Justice Commissioner Michael McGrath announced that the European Commission plans to propose new legislation by the end of this year to empower the EU to fine large tech companies that fail to protect consumers, especially children, from addictive design, subscription traps, and other dark patterns. This marks a significant expansion of EU regulatory power beyond existing digital laws like the Digital Services Act, potentially forcing tech giants to redesign user interfaces and business practices to avoid hefty fines. It also signals a growing global trend toward holding platforms accountable for consumer harm. The new rules will target both large tech companies and smaller online merchants and game developers, and the EU seeks enforcement power over cross-border systemic cases. McGrath noted that current consumer protection rules enforced by member states have never resulted in fines and are insufficient to deter violations.

telegram · zaihuapd · Jul 12, 06:25

**Background**: Dark patterns are user interface designs that trick or manipulate users into making unintended choices, such as buying unwanted products or sharing personal data. Addictive design refers to features like infinite scroll or personalized recommendations that keep users engaged excessively. The EU has previously addressed these issues through resolutions and is now moving toward binding legislation.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_pattern">Dark pattern - Wikipedia</a></li>
<li><a href="https://www.omnesmag.com/en/news/the-european-parliament-takes-a-closer-look-at-addictive-design-on-online-platforms/">The European Parliament Takes a Closer Look at Addictive Design ...</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#consumer protection`, `#big tech`, `#dark patterns`, `#online safety`

---

<a id="item-13"></a>
## [Chinese EVs Average 1.8 Years on Road, Shorter Than Phone Cycles](https://www.bloomberg.com/news/articles/2026-07-12/china-evs-average-1-8-years-on-road-less-than-cell-phones) ⭐️ 7.0/10

A report by the China Association of Automobile Manufacturers and Hejun Consulting reveals that the average age of electric vehicles on Chinese roads is only 1.8 years, compared to 8.2 years for gasoline cars, and even shorter than typical smartphone replacement cycles. This rapid turnover highlights how fast technological advancements in batteries, software, and chips are driving EV upgrades, while low resale values push owners to replace cars sooner. It signals a shift in consumer behavior where cars are treated more like consumer electronics, with significant implications for the automotive industry, resale markets, and environmental sustainability. After three years, the average retained value of an EV is only 43.35% of its original price, lower than that of gasoline cars. According to Dongchedi data, 43% of EV owners cite upgrading smart features and user experience as the primary reason for replacing their vehicle.

telegram · zaihuapd · Jul 12, 08:12

**Background**: China is the world's largest EV market, with rapid adoption driven by government incentives and a competitive landscape. Unlike traditional cars, EVs have shorter development cycles and faster software updates, making them more like smartphones. Low resale value is a known issue for EVs due to battery degradation and rapid obsolescence of technology.

<details><summary>References</summary>
<ul>
<li><a href="https://nev.ofweek.com/2026-06/ART-71008-8420-30692418.html">nev.ofweek.com/2026-06/ART-71008-8420-30692418.html</a></li>
<li><a href="https://www.163.com/dy/article/JNPNLEL90544W7WP.html">163.com/dy/article/JNPNLEL90544W7WP.html</a></li>
<li><a href="https://auto-time.36kr.com/p/335249487233026">电 动 车 开三年 残 值 仅剩1/3，威马小鹏探索 残 值 管理新模式_36氪</a></li>

</ul>
</details>

**Tags**: `#electric vehicles`, `#China`, `#automotive industry`, `#technology adoption`, `#depreciation`

---