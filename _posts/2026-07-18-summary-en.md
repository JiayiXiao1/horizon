---
layout: default
title: "Horizon Summary: 2026-07-18 (EN)"
date: 2026-07-18
lang: en
---

> From 38 items, 21 important content pieces were selected

---

1. [Firefox Compiled to WebAssembly Runs Inside Browser](#item-1) ⭐️ 9.0/10
2. [Kimi K3: 2.8 Trillion Parameter Open-Source Model Released](#item-2) ⭐️ 9.0/10
3. [Huawei Ascend 950 SuperPod Debuts, Claims 6.7x Nvidia Compute](#item-3) ⭐️ 9.0/10
4. [First Atmosphere Found on Rocky Exoplanet in Habitable Zone](#item-4) ⭐️ 8.0/10
5. [Open-source AI models surge, threatening closed rivals](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex Bug Can Delete $HOME Directory](#item-6) ⭐️ 8.0/10
7. [Thinking Machines Lab Releases Open-Weight Inkling Model](#item-7) ⭐️ 8.0/10
8. [Linus Torvalds Declares Linux Not Anti-AI](#item-8) ⭐️ 8.0/10
9. [Truth Social to Sell Real-Time Access to Trump's Posts to Wall Street](#item-9) ⭐️ 8.0/10
10. [Tesla Cybercab enters mass production in North America](#item-10) ⭐️ 8.0/10
11. [OpenAI CFO Proposes 'Useful Intelligence per Dollar' as AI ROI Metric](#item-11) ⭐️ 8.0/10
12. [Doubao Phone Pivots from GUI Automation to MCP Strategy](#item-12) ⭐️ 8.0/10
13. [Kaiser Nurses Blame AI and Surveillance for Worse Care](#item-13) ⭐️ 7.0/10
14. [Zilog Z80 Microprocessor Celebrates 50th Anniversary](#item-14) ⭐️ 7.0/10
15. [Practical Tips for Running SQLite](#item-15) ⭐️ 7.0/10
16. [Kaggle Competition Integrity Under Fire Over AI Submissions](#item-16) ⭐️ 7.0/10
17. [Offset Data Center Water Use by Converting Golf Courses](#item-17) ⭐️ 7.0/10
18. [EU Proposes Opening Android to Rival AI Assistants](#item-18) ⭐️ 7.0/10
19. [1Password integrates Claude for secure AI login](#item-19) ⭐️ 7.0/10
20. [Trump proposes drastic cuts to student, journalist visa durations](#item-20) ⭐️ 7.0/10
21. [US Lawmakers Urge Ban on Chinese Memory Chips in Allied Supply Chains](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Firefox Compiled to WebAssembly Runs Inside Browser](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter Labs has compiled the full Firefox browser (Gecko engine) to WebAssembly, allowing it to run inside another browser via a WebSocket-based network proxy using the Wisp protocol. This demonstrates that even complex native applications like a full browser can be ported to the web platform, potentially enabling new use cases for in-browser sandboxing, legacy software access, and cross-platform compatibility. The project used an estimated $25,000 worth of Claude Opus and Fable tokens (cost reduced via subscription), and the demo proxies all network traffic through Puter's servers to bypass browser network restrictions.

rss · Simon Willison · Jul 16, 23:34

**Background**: WebAssembly (WASM) is a low-level binary instruction format that runs in modern browsers at near-native speed. Compiling a full browser like Firefox to WASM is a massive engineering challenge because browsers are complex, multi-process applications with deep OS dependencies. Puter chose Firefox/Gecko for its strong single-process support, simplifying the porting effort.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/HeyPuter/firefox-wasm">GitHub - HeyPuter/ firefox -wasm: Firefox in WebAssembly · GitHub</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/">Firefox in WebAssembly</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion was highly positive, with many impressed by the technical achievement. Some raised concerns about the cost of proxying traffic, and the team noted they had to scale servers to handle the traffic spike.

**Tags**: `#WebAssembly`, `#Firefox`, `#browser`, `#compilation`, `#demo`

---

<a id="item-2"></a>
## [Kimi K3: 2.8 Trillion Parameter Open-Source Model Released](https://t.me/zaihuapd/42619) ⭐️ 9.0/10

Moonshot AI released Kimi K3, a 2.8 trillion parameter open-source model with 1 million token context, claiming performance second only to Claude Fable 5 and GPT-5.6 Sol. Kimi K3 is the largest open-source model to date, challenging proprietary models and potentially democratizing access to frontier AI capabilities. The model uses a sparse Mixture of Experts architecture with 896 experts, activating 16 per token, and introduces Kimi Delta Attention and Attention Residuals for improved efficiency.

telegram · zaihuapd · Jul 17, 00:02

**Background**: Large language models (LLMs) are typically measured by parameter count and context length. Mixture of Experts (MoE) allows models to have many parameters while keeping inference costs manageable by activating only a subset per token. Kimi K3's 2.8T parameters make it the largest open-weight model, surpassing DeepSeek's 1.6T V4 Pro.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">KIMI LINEAR: AN EXPRESSIVE, EFFICIENT ATTENTION ARCHITECTURE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments highlight that the 'pelican on a bicycle' test may be contaminated in training data, and note the model's high tokenizer count suggests a hidden system prompt. Others propose more rigorous benchmarks for agentic tasks.

**Tags**: `#AI`, `#LLM`, `#open-source`, `#Kimi`, `#Mixture of Experts`

---

<a id="item-3"></a>
## [Huawei Ascend 950 SuperPod Debuts, Claims 6.7x Nvidia Compute](https://www.ithome.com/0/978/019.htm) ⭐️ 9.0/10

At WAIC 2026, Huawei publicly demonstrated the Ascend 950 SuperPod (Atlas 950 SuperPoD) for the first time, claiming 1 EFLOPS FP8 and 2 EFLOPS FP4 compute with a 1024-card scale and 256 TB unified memory. According to a China Securities report, its total compute is 6.7 times that of Nvidia's NVL144 system with 144 cards. This marks a significant milestone in AI hardware, potentially reducing reliance on Nvidia GPUs for large-scale AI training in China. The performance claim, if validated, could reshape the competitive landscape of AI accelerators and impact global supply chains. The SuperPod is based on Huawei's Lingqu (UnifiedBus) interconnect protocol and supernode architecture, enabling 1024-card scaling with 2.1 microsecond ultra-low latency. Additionally, the Ascend 384 SuperPod has been commercially deployed in over 750 units across internet, telecom, and finance sectors, and is the only supernode in China that has trained SOTA models.

telegram · zaihuapd · Jul 17, 10:27

**Background**: Supernodes are high-density AI computing architectures that interconnect dozens or hundreds of AI chips via high-speed links, enabling large model training and inference. Huawei's Lingqu protocol is designed to overcome interconnect challenges, offering 100x reliability improvement and supporting distances over 200 meters. The Ascend 950 SuperPod competes directly with Nvidia's NVL series, which uses NVLink for GPU-to-GPU communication.

<details><summary>References</summary>
<ul>
<li><a href="https://www.itbear.com.cn/html/2025-09/960596.html">华为发布灵衢互联协议与系列超节点，引领AI算力基础设施新变革-人工智能-ITBear科技资讯</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1953935616661255083">华为这一突破，意义非同寻常 - 知乎</a></li>
<li><a href="https://www.qbitai.com/2025/09/333834.html">华为发布AI超节点服务器Atlas 850，支持128台1024卡超节点集群</a></li>

</ul>
</details>

**Tags**: `#AI Hardware`, `#Huawei`, `#Ascend`, `#SuperPod`, `#Compute Performance`

---

<a id="item-4"></a>
## [First Atmosphere Found on Rocky Exoplanet in Habitable Zone](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

JWST has confirmed the presence of an atmosphere on LHS 1140b, a rocky exoplanet about 48 light-years away orbiting within the habitable zone of its red dwarf star. This marks the first confirmed atmosphere on a relatively rocky exoplanet in a habitable zone. This discovery challenges previous assumptions that rocky planets around red dwarfs cannot retain atmospheres due to intense stellar stripping. It provides a prime target for further atmospheric characterization and raises new questions about habitability around M-dwarf stars. LHS 1140b is about 5.6 times Earth's mass and 70% larger in radius, placing it in the super-Earth category. JWST emission spectroscopy ruled out a mini-Neptune interpretation, confirming a rocky composition with an atmosphere.

hackernews · neversaydie · Jul 17, 14:06 · [Discussion](https://news.ycombinator.com/item?id=48947560)

**Background**: LHS 1140b was discovered in 2017 by the MEarth Project and orbits a red dwarf star much smaller and cooler than the Sun. Red dwarfs are known for frequent flares and intense stellar activity, which can strip atmospheres from close-in planets. The habitable zone around such stars is much closer than around Sun-like stars, making atmospheric retention challenging.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b</a></li>

</ul>
</details>

**Discussion**: Community comments highlight surprise that a rocky planet in a red dwarf's habitable zone could retain an atmosphere, with one user noting JWST data ruled out a mini-Neptune. Others discuss future directions like solar lens telescopes and the Fermi paradox, while some express skepticism about the 'Earth-like' label.

**Tags**: `#exoplanets`, `#JWST`, `#astronomy`, `#habitable zone`, `#red dwarf`

---

<a id="item-5"></a>
## [Open-source AI models surge, threatening closed rivals](https://stateofopensource.ai/) ⭐️ 8.0/10

Open-source AI models have overtaken closed models in market share on OpenRouter, growing from 40% to 63% in four months, with token processing increasing nearly 5x. This shift threatens companies like OpenAI and Anthropic, as open models enable cost-free deployment by hyperscalers and on-device optimization by Apple, commoditizing AI. The data from OpenRouter shows open models processed 888B tokens on March 19 and 4.19T tokens recently, a 5x increase in four months, indicating explosive adoption.

hackernews · rellem · Jul 17, 14:31 · [Discussion](https://news.ycombinator.com/item?id=48947825)

**Background**: Open-source AI models are publicly available with permissive licenses, allowing anyone to use, modify, and deploy them without paying licensing fees. Closed models, like those from OpenAI and Anthropic, are proprietary and require API access or subscriptions. The rise of open models challenges the business model of closed AI companies.

**Discussion**: Commenters highlight the rapid market shift, with one noting open models now lead 63%-37% on OpenRouter. Some argue open models will commoditize AI, while others criticize the presentation as LLM-generated and lacking substance.

**Tags**: `#open source`, `#AI`, `#machine learning`, `#market trends`, `#LLMs`

---

<a id="item-6"></a>
## [GPT-5.6 Codex Bug Can Delete $HOME Directory](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI confirmed a bug in GPT-5.6 Codex where, under full access mode without sandboxing, the model may mistakenly delete the user's $HOME directory instead of a temporary directory. This bug highlights critical safety risks in AI coding agents with unrestricted file system access, potentially causing irreversible data loss for developers who rely on such tools. The bug occurs when full access mode is enabled, sandboxing and auto review are disabled, and the model attempts to override $HOME to point to a temp directory but mistakenly deletes the real $HOME. OpenAI has promised a post-mortem and harness fixes.

rss · Simon Willison · Jul 16, 17:45

**Background**: GPT-5.6 Codex is OpenAI's latest AI coding agent that can execute terminal commands and access the file system. Full access mode disables the sandbox, giving the model unrestricted file system access. The $HOME environment variable points to the user's home directory, which contains personal files and configurations.

<details><summary>References</summary>
<ul>
<li><a href="https://openai-codex.mintlify.app/concepts/sandboxing">Sandboxing - Codex CLI</a></li>
<li><a href="https://explainx.ai/blog/openai-codex-gpt-5-6-home-deletion-full-access-july-2026">Codex GPT-5.6 $HOME Deletion — Full Access | explainx.ai</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**Tags**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-7"></a>
## [Thinking Machines Lab Releases Open-Weight Inkling Model](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

Thinking Machines Lab, led by Mira Murati, released Inkling, an open-weights 975B parameter Mixture-of-Experts multimodal model under the Apache-2.0 license, trained on 45 trillion tokens of text, images, audio, and video. Inkling strengthens the US open-weights ecosystem, offering a competitive alternative to Chinese open models and enabling fine-tuning via the Tinker platform, despite not being a frontier model. Inkling has 975B total parameters with 41B active per token, and a smaller 276B (12B active) variant called Inkling-Small is promised but not yet released. The model card and training data documentation are notably sparse.

rss · Simon Willison · Jul 16, 15:35

**Background**: Mixture-of-Experts (MoE) is a neural architecture that uses multiple parallel expert subnetworks and a gating mechanism to activate only a subset of parameters per input, improving efficiency. Open-weights models release trained parameters publicly, allowing download and fine-tuning, but may not include full training data or code. The Apache-2.0 license permits free use, modification, and distribution.

**Tags**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-8"></a>
## [Linus Torvalds Declares Linux Not Anti-AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linus Torvalds, the creator of Linux, stated on the Linux Media Mailing List that Linux is not an anti-AI project and that AI is a clearly useful tool, dismissing objections and inviting dissenters to fork the project or walk away. This strong endorsement from the top Linux maintainer signals a major shift in the project's stance on AI, potentially influencing the broader open-source community to embrace AI tools in development. Torvalds emphasized that AI's usefulness is no longer in question, though he acknowledged other open questions about AI's economy. He made these remarks on the linux-media mailing list in response to ongoing debates.

rss · Simon Willison · Jul 16, 13:26

**Background**: The Linux kernel is one of the largest open-source projects, with Linus Torvalds as its creator and top maintainer. Recently, some open-source projects have adopted anti-AI policies, restricting AI-generated code contributions. Torvalds' statement clarifies Linux's position and rejects such restrictions.

**Tags**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`

---

<a id="item-9"></a>
## [Truth Social to Sell Real-Time Access to Trump's Posts to Wall Street](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

Trump Media & Technology Group announced on Thursday that Truth Social will launch Truth API on August 1, providing institutional clients with millisecond-speed access to real-time posts from the platform's top 10 accounts, including President Trump's account. This move monetizes Trump's social media influence, potentially enabling algorithmic traders to gain an information edge based on his policy announcements, which have previously caused significant market volatility in stocks and oil. The API targets high-frequency algorithmic traders, offering data at millisecond latency. TMTG has not disclosed pricing, and the service will cover only the top 10 accounts, not all users.

telegram · zaihuapd · Jul 17, 01:02

**Background**: Truth Social is a social media platform launched by Trump after being banned from major platforms. It has become his primary channel for policy announcements, with posts on tariffs, Iran, and the Strait of Hormuz previously moving markets. CNN investigations have also found Trump using Truth Social to promote stocks he recently purchased.

<details><summary>References</summary>
<ul>
<li><a href="https://fisf.fudan.edu.cn/show-80-3700.html?tid=0">施东辉： 高 频 交 易 ，天使还是魔鬼？ | 复旦大学国际金融学院(FISF)...</a></li>
<li><a href="https://invest.cnyes.com/usstock/detail/DJT">Trump Media & Technology Group Corp.</a></li>

</ul>
</details>

**Tags**: `#Truth Social`, `#API`, `#financial markets`, `#algorithmic trading`, `#politics`

---

<a id="item-10"></a>
## [Tesla Cybercab enters mass production in North America](https://t.me/zaihuapd/42621) ⭐️ 8.0/10

Tesla has announced that its driverless Cybercab, a vehicle designed without a steering wheel or pedals, has started mass production in North America. This marks a major milestone in autonomous vehicle production, bringing Tesla closer to launching its Robotaxi service and potentially reshaping urban transportation. The Cybercab is a two-passenger, fully autonomous vehicle with no steering wheel, pedals, or mirrors, relying entirely on its onboard AI for driving. Pilot production began in February 2026, with volume production targeted by end of 2026.

telegram · zaihuapd · Jul 17, 03:06

**Background**: A robotaxi is an autonomous vehicle used for ride-hailing services without a human driver. Tesla's Cybercab is purpose-built for this role, aiming to reduce transportation costs and increase accessibility. The concept was unveiled in October 2024, and Tesla plans to produce up to 2 million units annually.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cybercab">Cybercab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Robotaxi">Robotaxi</a></li>

</ul>
</details>

**Tags**: `#Tesla`, `#autonomous driving`, `#electric vehicles`, `#robotaxi`

---

<a id="item-11"></a>
## [OpenAI CFO Proposes 'Useful Intelligence per Dollar' as AI ROI Metric](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 8.0/10

OpenAI CFO Sarah Friar introduced a new framework called 'useful intelligence per dollar' to measure AI ROI, shifting focus from token cost to value delivered. This was announced alongside the release of the GPT-5.6 series, whose flagship model Sol set a new coding record with 54% fewer output tokens than a leading competitor. This metric could reshape how enterprises evaluate AI investments, emphasizing task completion cost over raw token pricing. It provides a more holistic view of AI productivity, potentially influencing adoption strategies and vendor selection across industries. The framework includes four dimensions: useful work completed, full cost per successful task, reliability of AI outputs, and whether each dollar generates more value with increased usage. Friar noted that the lowest token price does not equal the lowest task cost, as a more powerful model might give the correct answer in one shot, saving money overall.

telegram · zaihuapd · Jul 17, 15:00

**Background**: Traditionally, software ROI was measured by adoption metrics like user count or license renewals. For AI, many companies focus on token cost per query, but this ignores the value of the work completed. The new metric aims to capture the actual business value generated by AI, aligning with the trend of outcome-based pricing.

<details><summary>References</summary>
<ul>
<li><a href="https://blog.laozhang.ai/zh/posts/gpt-5-6-sol-vs-terra-vs-luna">GPT - 5 . 6 Sol 、Terra、Luna... | LaoZhang AI Blog</a></li>
<li><a href="https://juejin.cn/post/7661971304589901875">GPT - 5 . 6 Sol 、Terra、Luna...</a></li>

</ul>
</details>

**Tags**: `#AI ROI`, `#OpenAI`, `#GPT-5.6`, `#enterprise AI`, `#productivity metrics`

---

<a id="item-12"></a>
## [Doubao Phone Pivots from GUI Automation to MCP Strategy](https://www.latepost.com/news/dj_detail?id=3648) ⭐️ 8.0/10

Doubao phone has abandoned its previous GUI automation approach that simulated clicks on super apps, and now requires apps like Alibaba and Tencent to provide MCP services and open data access. Production has been increased from 30,000 to hundreds of thousands of units. This shift reflects a broader industry trend where AI devices seek standardized protocols like MCP for app integration, moving away from fragile GUI automation. It also highlights the power struggle between phone makers and super apps over AI ecosystem control. The Doubao phone assistant software received generative AI service备案 on July 15, 2025, and its first technical preview was released in December 2025. Earlier versions were blocked by WeChat and Taobao due to GUI automation.

telegram · zaihuapd · Jul 18, 00:29

**Background**: GUI automation involves an AI agent reading the screen and simulating taps to control apps, which is fragile and often blocked by app developers. MCP (Model Context Protocol) is an open standard that allows AI applications to securely access tools and data from services, reducing development complexity and improving reliability.

<details><summary>References</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://mcp.so/">MCP .so - MCP Marketplace</a></li>
<li><a href="https://eu.36kr.com/en/p/3896193801602697">Half a Year Post-Debut of the Doubao Phone : Why Are Step and...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#MCP`, `#smartphone`, `#ecosystem`, `#strategy`

---

<a id="item-13"></a>
## [Kaiser Nurses Blame AI and Surveillance for Worse Care](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

Kaiser Permanente nurses report that AI and workplace surveillance tools are worsening their jobs and patient care, according to a CalMatters article. The nurses say metrics penalize longer calls and limit advice to three pieces per call. This highlights growing tensions between cost optimization and quality care in healthcare, as AI-driven surveillance becomes more common. The debate underscores the need for ethical AI deployment that supports rather than undermines clinical work. The article mentions a 2024 pilot of an AI empathy tool that was discontinued, and community comments note that many complaints are about call center metrics rather than AI itself. Some nurses find value in AI tools like live translation and note summarization.

hackernews · gnabgib · Jul 17, 22:26 · [Discussion](https://news.ycombinator.com/item?id=48952880)

**Background**: Workplace surveillance tools, often called 'bossware,' are increasingly used in healthcare to monitor worker productivity and adherence to protocols. These tools can track call durations, patient interactions, and even emotional tone, aiming to reduce costs but sometimes compromising care quality.

<details><summary>References</summary>
<ul>
<li><a href="https://rbfirehose.com/2026/07/16/local-news-matters-kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/">Local News Matters: Kaiser nurses say AI, workplace surveillance ...</a></li>
<li><a href="https://www.nytimes.com/2026/03/01/business/bossware-work-surveillance-tools.html">Are ‘Bossware’ Tools Tracking You? - The New York Times</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree that the real problem is metric-driven cost optimization, not AI itself. Some nurses report positive experiences with AI tools, while others criticize the misuse of metrics to ration care. A commenter notes similar issues at UHC.

**Tags**: `#AI ethics`, `#healthcare`, `#workplace surveillance`, `#nurses`, `#Kaiser`

---

<a id="item-14"></a>
## [Zilog Z80 Microprocessor Celebrates 50th Anniversary](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

The Zilog Z80 microprocessor, first released in 1976, has turned 50 years old, marking a significant milestone in computing history. The Z80's longevity and influence on early personal computing, embedded systems, and hobbyist electronics make its anniversary a moment to reflect on the foundations of modern computing. The Z80 was binary compatible with the Intel 8080 but had differences in flag register behavior and repurposed undefined opcodes, which could cause compatibility issues.

hackernews · st_goliath · Jul 17, 19:41 · [Discussion](https://news.ycombinator.com/item?id=48951461)

**Background**: The Z80 was an 8-bit microprocessor designed by Zilog and widely used in home computers like the Timex Sinclair, as well as in embedded systems and game consoles. Its instruction set and register architecture made it popular for hobbyist programming and education.

**Discussion**: Community comments express nostalgia and technical appreciation, with users sharing personal stories of learning assembly and building Z80-based kits. Some discuss compatibility nuances between the Z80 and 8080.

**Tags**: `#Z80`, `#retrocomputing`, `#microprocessor`, `#history`, `#embedded systems`

---

<a id="item-15"></a>
## [Practical Tips for Running SQLite](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

A blog post shares practical tips for running SQLite, including backup strategies and using the .expert mode for automatic index recommendations. These tips help developers improve SQLite performance and data safety, addressing common pain points like slow deletes and backup complexity. The .expert mode analyzes queries and suggests indexes, while backup strategies include using .dump with compression and WAL mode to avoid blocking writers.

hackernews · surprisetalk · Jul 17, 17:45 · [Discussion](https://news.ycombinator.com/item?id=48950122)

**Background**: SQLite is a lightweight, embedded database engine widely used in applications. The .expert mode is a CLI feature that recommends indexes based on query analysis. WAL (Write-Ahead Logging) allows concurrent reads and writes.

<details><summary>References</summary>
<ul>
<li><a href="https://databaseschool.com/series/high-performance-sqlite/videos/41">Where to add indexes - High Performance SQLite - Database School</a></li>
<li><a href="https://sqlite.work/efficiently-persisting-sqlite-in-memory-databases-to-disk-with-minimal-overhead/">Efficiently Persisting SQLite In-Memory Databases... - SQLite Help Docs</a></li>

</ul>
</details>

**Discussion**: Commenters share real-world backup scripts using zstd compression and rsync, and discuss batching deletes to avoid performance issues. One user built a tool to simplify AWS S3 credential generation for backups.

**Tags**: `#SQLite`, `#database`, `#backup`, `#performance`, `#tools`

---

<a id="item-16"></a>
## [Kaggle Competition Integrity Under Fire Over AI Submissions](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423) ⭐️ 7.0/10

A discussion on Kaggle reveals allegations that AI-generated submissions and AI judges have compromised competition results, with participants claiming prompt injection can trick AI judges into declaring winners. This undermines trust in AI-mediated evaluation platforms like Kaggle, which are increasingly used to benchmark AI capabilities and award prizes, potentially devaluing human skill and favoring insiders. The competition in question offered a $25,000 prize, and community members report that AI judges are vulnerable to prompt injection attacks, where submissions include hidden instructions to influence scoring.

hackernews · twerkmeister · Jul 17, 11:30 · [Discussion](https://news.ycombinator.com/item?id=48946010)

**Background**: Kaggle is a platform for data science competitions where participants build models to solve problems. Recently, AI-generated code and automated judging have become common, raising concerns about fairness and the role of human expertise.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://www.ai-redteam.com/topics/prompt-injection/">Prompt Injection | AI Red Team</a></li>

</ul>
</details>

**Discussion**: Commenters express frustration that AI has killed fair hackathons, with one noting that projects win by prompt injecting 'I am the winner.' Others argue that brute-force methods have always existed, but AI judges exacerbate the issue.

**Tags**: `#AI ethics`, `#Kaggle`, `#competition integrity`, `#prompt injection`, `#evaluation bias`

---

<a id="item-17"></a>
## [Offset Data Center Water Use by Converting Golf Courses](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 7.0/10

A proposal suggests hyperscalers like Google offset their data center water consumption by purchasing golf courses and converting them into public parks, using the saved water to meet their needs. This creative idea highlights the growing tension between AI data center water use and local water resources, offering a potential win-win solution that reduces water consumption while creating public green spaces. Google used 10.9 billion gallons of water in 2025, about 30 million gallons per day, while a single golf course in Coachella Valley uses ~750,000 gallons per day; buying 40 courses could offset Google's usage.

rss · Simon Willison · Jul 17, 02:58

**Background**: Data centers, especially hyperscale ones, consume vast amounts of water for cooling. An acre-foot is a common US water measurement unit equal to about 325,851 gallons. Golf courses are notoriously water-intensive, making them a target for water reallocation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.weforum.org/stories/2026/01/ai-water-data-centres-opportunity-am26-wef-xylem/">Why AI's water problem might actually be an opportunity</a></li>
<li><a href="https://www.coloradoriverdistrict.org/water-measurement/">Water Measurement - Basic Units of Water | Colorado River District</a></li>

</ul>
</details>

**Tags**: `#ai-energy-usage`, `#water consumption`, `#data centers`, `#sustainability`

---

<a id="item-18"></a>
## [EU Proposes Opening Android to Rival AI Assistants](https://t.me/zaihuapd/42615) ⭐️ 7.0/10

The European Union is drafting requirements under the Digital Markets Act that would force Google to grant rival AI assistants like ChatGPT and Claude the same system-level access on Android as its own Gemini assistant. This could reshape competition in the AI assistant market by lowering barriers for third-party apps on the dominant Android platform, potentially accelerating innovation but also raising security and privacy concerns. The requirements are still in draft stage and may be delayed; Google has expressed concerns that opening up system features could compromise user security and privacy. The changes would take effect from July 2027 as part of the next Android version.

telegram · zaihuapd · Jul 16, 13:19

**Background**: The Digital Markets Act (DMA) is an EU law that designates large online platforms as 'gatekeepers' and imposes obligations to ensure fair competition. Google's Android is subject to DMA rules, and the EU has previously fined Google for antitrust violations related to Android. This proposal extends DMA enforcement to AI assistants, a rapidly growing market.

<details><summary>References</summary>
<ul>
<li><a href="https://www.heise.de/en/news/EU-Requirements-Android-must-fully-open-up-for-third-party-AI-assistants-11367823.html">EU Requirements : Android must fully open up for... | heise online</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://techeconomy.ng/google-eu-digital-markets-act-android-search-data-ai-openai/">EU Orders Google to Share Android Features, Search Data with...</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#Android`, `#AI assistants`, `#antitrust`, `#Google`

---

<a id="item-19"></a>
## [1Password integrates Claude for secure AI login](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 7.0/10

1Password launched a Mac integration with Anthropic's Claude that allows the AI agent to log into websites on behalf of users without ever exposing passwords or 2FA codes to the AI system. This is the first browser integration that lets an AI agent use credentials without granting direct access to them, addressing a key security concern in agentic AI and potentially setting a new standard for credential management in AI assistants. Credentials are injected directly into the target webpage via a secure channel, and users must approve each login task with biometric authentication on a per-session basis; if auto-fill submission fails, the filled content is immediately erased.

telegram · zaihuapd · Jul 16, 15:54

**Background**: Password managers like 1Password store and autofill credentials for users, but AI agents typically require direct access to credentials to perform tasks, raising security risks. 1Password's zero-exposure architecture ensures the AI model never sees the secrets, maintaining the password manager as the single source of truth.

<details><summary>References</summary>
<ul>
<li><a href="https://1password.com/blog/1password-for-claude?cjdata=MXxOfDB8WXww&cjevent=521ad2f581fa11f1839802ae0a82b82c">1 Password for Claude : Give Claude access without giving up your...</a></li>
<li><a href="https://thenextweb.com/news/1password-claude-credential-zero-exposure-agentic-mode">1 Password lets Claude log you into websites without ever seeing your...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/17/1password-anthropic-claude-integration/">Claude can now sign into websites with... - Help Net Security</a></li>

</ul>
</details>

**Tags**: `#password management`, `#AI integration`, `#security`, `#Claude`, `#1Password`

---

<a id="item-20"></a>
## [Trump proposes drastic cuts to student, journalist visa durations](https://t.me/zaihuapd/42623) ⭐️ 7.0/10

The Trump administration proposed new regulations on Wednesday that would cap student and exchange visitor visas at four years, and journalist visas at 240 days, with Chinese journalists limited to just 90 days. This policy could significantly disrupt international student enrollment and academic exchange programs, and restrict press freedom, especially for Chinese journalists covering the U.S. The proposed rule would apply to F-1 student visas, J-1 exchange visitor visas, and I-1 media visas; visa holders may apply for extensions but must repeatedly submit additional paperwork.

telegram · zaihuapd · Jul 17, 04:41

**Background**: Currently, F-1, J-1, and I-1 visas typically remain valid for the duration of the program or assignment. The U.S. hosts about 1.6 million international students on F visas, and in fiscal 2024 issued roughly 355,000 exchange visitor visas and 13,000 media visas.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chineseherald.co.nz/news/education/trump-tightens-foreign-student-journalist-visa-rules/">chineseherald.co.nz/news/education/trump-tightens-foreign-student...</a></li>

</ul>
</details>

**Tags**: `#immigration policy`, `#international students`, `#journalist visas`, `#US politics`, `#tech talent`

---

<a id="item-21"></a>
## [US Lawmakers Urge Ban on Chinese Memory Chips in Allied Supply Chains](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 7.0/10

U.S. House China Committee Chairman John Moolenaar and Representative George Whitesides sent a letter to Commerce Secretary Howard Lutnick urging a ban on U.S. companies purchasing Chinese memory chips and calling for CXMT to be added to the Entity List with additional restrictions on YMTC. This move could significantly disrupt global semiconductor supply chains, particularly for DRAM and NAND flash, and may force companies like Apple to seek alternative sources, potentially impacting AI infrastructure development. The lawmakers argue that Chinese memory chip makers have close ties to the People's Liberation Army, and each purchase directly funds dual-use technology development. They also urge coordination with Japan, South Korea, and the EU to prevent Chinese manufacturers from embedding in allied supply chains.

telegram · zaihuapd · Jul 17, 14:00

**Background**: CXMT is a leading Chinese DRAM manufacturer not yet on the U.S. Entity List, while YMTC, a major NAND flash producer, is already under restrictions. The U.S. has increasingly targeted Chinese semiconductor firms over national security concerns, especially regarding dual-use technologies that could benefit the military.

<details><summary>References</summary>
<ul>
<li><a href="https://www.rfi.fr/cn/经贸/20260716-众议员致信美商务部长促禁购中国存储芯片-参议员提法案加强对中国在美制药业投资审查">rfi.fr/cn/经贸/20260716...</a></li>
<li><a href="https://gaohaojun.cn/Blog/2026/01/21/红色内存潮流长鑫存储的战略分析和围绕DRAM的地缘政治斗争/">内 存 的赤色潮流： 长 鑫 存 储 （ CXMT ... - Gao Haojun</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#trade policy`, `#supply chain`, `#China`, `#memory chips`

---