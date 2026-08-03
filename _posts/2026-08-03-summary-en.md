---
layout: default
title: "Horizon Summary: 2026-08-03 (EN)"
date: 2026-08-03
lang: en
---

> From 35 items, 17 important content pieces were selected

---

1. [OpenAI's Astra Model Achieves Breakthroughs on Ten Long-Standing Math Problems](#item-1) ⭐️ 9.0/10
2. [Kakehashi: Running macOS Binaries on Linux ARM](#item-2) ⭐️ 8.0/10
3. [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](#item-3) ⭐️ 8.0/10
4. [AI Giants Push Back on Open-Weight Model Restrictions](#item-4) ⭐️ 8.0/10
5. [China Promotes Open-Weight AI Models to Global South at UN Summit](#item-5) ⭐️ 8.0/10
6. [Microsoft Confirms Copilot 'Super App' Launch This Year](#item-6) ⭐️ 8.0/10
7. [Karpathy Stars sqliteai/waste: Streaming Kimi K3 from NVMe](#item-7) ⭐️ 7.0/10
8. [Karpathy's AI Pelican Sparks Debate on Physical World Benchmarks](#item-8) ⭐️ 7.0/10
9. [F*: A General-Purpose Proof-Oriented Programming Language](#item-9) ⭐️ 7.0/10
10. [EA to Be Acquired by Saudi-Led Consortium for $55B, Deal Closes Next Week](#item-10) ⭐️ 7.0/10
11. [CXMT Unveils DDR5 and LPDDR5X, DDR5 Hits 8000Mbps](#item-11) ⭐️ 7.0/10
12. [AI Chip Count Doubles Every 9 Months, Set to Reach 200 Million by 2028](#item-12) ⭐️ 7.0/10
13. [Apple Limits Bug Reports to Curb AI-Generated Slop](#item-13) ⭐️ 7.0/10
14. [Chinese AI Framework Detects Bitcoin Money Laundering with 90% Accuracy](#item-14) ⭐️ 7.0/10
15. [China Issues Mandatory Standard for Public Warning SMS](#item-15) ⭐️ 7.0/10
16. [Microplastics Found in 92% of Animals Near Deep-Sea Hydrothermal Vents](#item-16) ⭐️ 7.0/10
17. [U.S. States Move to Repeal Data Center Tax Breaks, Raising AI Infrastructure Costs](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI's Astra Model Achieves Breakthroughs on Ten Long-Standing Math Problems](https://openai.com/index/ten-advances-in-mathematics/) ⭐️ 9.0/10

OpenAI announced that an internal version of its next-generation model, Astra, has achieved new results on ten long-standing open problems in mathematics and theoretical computer science, including high-dimensional sphere packing, non-sofic groups, and a counterexample to Connes' rigidity conjecture. The proofs were formalized in Lean and cost less than $2,000 per problem in token expenses. This marks a significant milestone in AI-assisted mathematical research, demonstrating that AI can contribute to solving problems that have resisted progress for decades. It could accelerate the pace of discovery in mathematics and theoretical computer science, and raises important questions about attribution and the role of AI in research. The problems include high-dimensional sphere packing, existence of non-sofic groups, a counterexample to Connes' rigidity conjecture, arithmetic circuit lower bounds, quantum parallel repetition, hardness of the nearest vector problem, and multicolor Ramsey numbers. OpenAI has released Lean 4 formalizations in a GitHub repository and a paper describing the solutions, but has not disclosed the prompts used.

telegram · zaihuapd · Aug 1, 07:59

**Background**: Sphere packing is a classic problem in mathematics that asks how to arrange spheres in a given dimension to maximize the fraction of space they occupy. Optimal solutions are known only for dimensions 1, 2, 3, 8, and 24, and the problem remains open in other dimensions. Formal verification in Lean is a method of proving mathematical statements using a computer-checked proof assistant, ensuring correctness. The results are part of a broader trend of AI being used in mathematical research, as highlighted by Terence Tao's concept of 'big mathematics'.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/zh-hans/克卜勒猜想">克卜勒猜想 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1571316.htm">OpenAI下一代模型Astra：10... - cnBeta.COM</a></li>
<li><a href="https://news.marsbit.co/20260802090912297284.html">突发！ OpenAI下一代AI攻克10项菲尔兹奖级难题 | Mars Finance</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion reflects a mix of awe and skepticism. Some commenters express excitement about the potential of AI in mathematics, while others question the significance of the results and the lack of transparency regarding the prompts used. There is also discussion about the 'Deep Blue moment' for mathematics, drawing parallels to the famous chess match.

**Tags**: `#AI`, `#mathematics`, `#OpenAI`, `#formal verification`, `#research`

---

<a id="item-2"></a>
## [Kakehashi: Running macOS Binaries on Linux ARM](https://github.com/wie-project/kakehashi) ⭐️ 8.0/10

Kakehashi, an experimental userspace translation layer, now successfully runs macOS CLI binaries on Linux ARM, with working prototypes for 7-Zip, curl, and Xcode Tools Git. The project loads Darwin Mach-O binaries on Linux aarch64 and translates BSD syscalls without a JIT. This project addresses a significant technical challenge in cross-OS binary compatibility, potentially enabling macOS applications to run natively on Linux ARM hardware. It could expand the Linux ecosystem by providing access to macOS-only tools and applications, similar to how Wine/Proton did for Windows applications. The current implementation is CLI-first and lacks a JIT, and performance is still slower than native execution—for example, 7-Zip runs about 5.2x slower. The project maps a freestanding libSystem and translates BSD syscalls, and it can be installed via cargo install kakehashi.

hackernews · vlad_kalinkin · Aug 2, 16:26 · [Discussion](https://news.ycombinator.com/item?id=49145937)

**Background**: macOS binaries use the Mach-O format, which is not natively supported by Linux. The Darling project is a more extensive solution aiming to run macOS applications on Linux, and it has an open PR for ARM64 support. Kakehashi takes a different, userspace-only approach, focusing on CLI binaries and avoiding kernel-level modifications.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/wie-project/kakehashi">wie-project/ kakehashi : Userspace macOS translation layer for Linux ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mach-O">Mach-O - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is enthusiastic about the project's potential, with some comparing it to Wine/Proton and suggesting collaboration with the Darling project. Others express cautious optimism, noting the project is still early and wondering about future directions, such as supporting AU binaries for audio plugins.

**Tags**: `#macOS`, `#Linux`, `#ARM`, `#binary compatibility`, `#userspace`

---

<a id="item-3"></a>
## [eBay Harassment Campaign Leads to $56M Payout and Prison Sentences](https://www.ft.com/content/06ec1b03-d4af-40cf-b12a-4ba5a410f6d2) ⭐️ 8.0/10

eBay has agreed to pay $56 million to David and Ina Steiner, a couple targeted by a harassment campaign orchestrated by eBay's security team. Several former security executives, including Jim Baugh, were sentenced to prison, with Baugh receiving 57 months. This case highlights serious corporate accountability issues, showing how a major tech company's security team abused power to target critics. It raises questions about oversight and ethical conduct within corporate security departments, and may prompt other companies to review their practices. The harassment campaign included sending disturbing deliveries, surveillance, and threats. Seven members of eBay's security team, including former police captains, were involved, and the sentencing varied from time served to 57 months in prison.

hackernews · JumpCrisscross · Aug 2, 19:19 · [Discussion](https://news.ycombinator.com/item?id=49147435)

**Background**: eBay is a global e-commerce platform where users buy and sell goods. The Steiners published a newsletter critical of eBay, which allegedly triggered the harassment. This case underscores the potential for corporate security teams to overstep legal and ethical boundaries, especially when targeting perceived threats to the company's reputation.

**Discussion**: Commenters expressed skepticism that the harassment was limited to one couple, suggesting other critics may have been targeted. Some also questioned the behavior of former police officers involved, and others noted eBay's high seller fees as a separate concern.

**Tags**: `#eBay`, `#harassment`, `#corporate accountability`, `#legal`, `#security`

---

<a id="item-4"></a>
## [AI Giants Push Back on Open-Weight Model Restrictions](https://simonwillison.net/2026/Aug/2/open-letters/#atom-everything) ⭐️ 8.0/10

In late July 2026, Microsoft, NVIDIA, Amazon, OpenAI, and over 230 other companies signed an open letter advocating for open-weight AI models, countering potential US government restrictions. Anthropic declined to sign and published its own position, while a separate letter from 1,324 AI employees called for pacing frontier AI development. This coordinated industry push could shape US AI regulation, balancing innovation and safety concerns. The debate highlights a growing divide between companies favoring open models and those worried about misuse and national security. The Microsoft-led letter explicitly supports distillation, a technique where models train on outputs from other models, which some see as enabling copying. Anthropic's response, led by CEO Dario Amodei, warns of authoritarian governments building powerful AI and calls for cracking down on industrial-scale distillation, while denying any advocacy for a ban on open-weights models.

rss · Simon Willison · Aug 2, 04:16

**Background**: Open-weight models are AI models whose trained parameters are publicly released, allowing developers to run, modify, and audit them, unlike closed models that are only accessible via APIs. The debate is part of a broader policy discussion about AI safety, competition, and national security, especially in the context of US-China rivalry.

**Tags**: `#AI policy`, `#open-weight models`, `#regulation`, `#industry`, `#Simon Willison`

---

<a id="item-5"></a>
## [China Promotes Open-Weight AI Models to Global South at UN Summit](https://www.semafor.com/article/07/28/2026/token-diplomacy-how-china-is-shaping-the-worlds-ai-future) ⭐️ 8.0/10

At the UN 'AI for Good' summit in Geneva in late July, a Chinese delegation promoted China's open-weight AI models to Global South countries including Pakistan, Russia, and Zambia. Alibaba Cloud architect Wang Jian stated that Chinese AI could serve as a 'cornerstone' for other nations' development, similar to energy. This move positions China as an alternative to US closed AI models, potentially shaping global AI infrastructure and standards. It could increase China's geopolitical influence among developing nations and create dependencies on Chinese technology, challenging US dominance in AI. The US State Department expressed concern, warning that such initiatives could lead to dependence on Chinese infrastructure and standards. Notably, US frontier labs and Trump administration officials were largely absent from the summit, highlighting the geopolitical divide.

telegram · zaihuapd · Aug 1, 10:06

**Background**: Open-weight models make trained parameters publicly available, allowing anyone to download, use, or fine-tune them without retraining, though they do not necessarily disclose the full training code or data. This contrasts with closed models like those from OpenAI, which keep weights proprietary. China's 'token diplomacy' strategy aims to export AI infrastructure at lower costs, including training and support, to win influence in the Global South.

<details><summary>References</summary>
<ul>
<li><a href="https://www.wbolt.com/open-weight-models.html">开放源码和开放权重模型之间有何区别？</a></li>
<li><a href="https://www.sina.cn/news/detail/5208191114938882.html">什么是开源模型？什么是开放权重模型？虽然两者的概念经常被混淆，但它们之间是有很大区别的。开放权重模型指的是把模型训练好的参数公开出来，大家直接下载就能用，上手很方便。但它并不公开底层代码和完整的训练细节，所以你能用、能微调到一定程度，但想彻底看懂或大改架构就比较难。例如 Meta 的 _新浪新闻</a></li>
<li><a href="https://m.cls.cn/detail/1989989">OpenAI这次要open了，奥尔特曼所说的“开放权重模型”是什么？</a></li>

</ul>
</details>

**Tags**: `#AI geopolitics`, `#open-source AI`, `#China`, `#global south`, `#AI governance`

---

<a id="item-6"></a>
## [Microsoft Confirms Copilot 'Super App' Launch This Year](https://www.theverge.com/tech/972927/microsoft-copilot-super-app-confirmed) ⭐️ 8.0/10

Microsoft CEO Satya Nadella confirmed on an earnings call that the company will launch an AI 'super app' this year, integrating Copilot's chat, coding, and agentic capabilities for both consumers and businesses. The app will merge experiences including code features into a single application this quarter. This consolidation positions Microsoft to compete directly with OpenAI's ChatGPT Work and other integrated AI platforms, potentially reshaping how developers and enterprises access AI tools. It signals a trend toward unified AI workspaces, which could impact software engineering workflows and enterprise productivity. The super app will combine Copilot chat, GitHub Copilot, Copilot Cowork, and Autopilot systems, as previously reported by Fortune. Microsoft's quarterly revenue rose to $90 billion, driven by AI and cloud businesses. OpenAI recently launched ChatGPT Work, which integrates ChatGPT with Codex, indicating a competitive landscape.

telegram · zaihuapd · Aug 1, 13:18

**Background**: Copilot is Microsoft's AI assistant integrated across its products, evolving from a chat tool to 'Cowork' and 'Autopilots' for automation. A 'super app' consolidates multiple functionalities into one platform, similar to WeChat. GitHub Copilot is a coding assistant, while Copilot Cowork is an AI automation layer in Microsoft 365, and Autopilot refers to agentic AI systems that automate tasks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/microsoft-launches-copilot-cowork-built-anthropic-cross-m365-bora-g2xzc?tl=en">Microsoft launches Copilot Cowork , built with Anthropic...</a></li>
<li><a href="https://theplanettools.ai/blog/microsoft-copilot-cowork-ga-runs-on-anthropic-claude-not-mai-2026">Copilot Cowork Runs on Claude, Not MAI — Why... | ThePlanetTools.ai</a></li>
<li><a href="https://openai.com/chatgpt-work/">ChatGPT Work for every team | OpenAI</a></li>

</ul>
</details>

**Tags**: `#Microsoft`, `#Copilot`, `#AI`, `#Super App`, `#Product Announcement`

---

<a id="item-7"></a>
## [Karpathy Stars sqliteai/waste: Streaming Kimi K3 from NVMe](https://github.com/sqliteai/waste) ⭐️ 7.0/10

Andrej Karpathy starred the GitHub repository sqliteai/waste, which enables running the full 2.78-trillion-parameter Kimi K3 model on consumer hardware by streaming activated weights directly from NVMe storage. This project addresses the constraint that the model (1.42 TB published, 982 GB after conversion) does not fit in the RAM of mainstream systems. Karpathy's endorsement signals high interest in a technique that could democratize access to state-of-the-art large language models, allowing researchers and hobbyists to run massive models without expensive hardware. This could accelerate innovation in local AI inference and influence future model deployment strategies. The project is written in C and licensed under Apache License 2.0. It streams only the activated weights from NVMe, reducing memory requirements, and is specifically designed for the Kimi K3 model.

github · karpathy · Aug 2, 17:19

**Background**: Large language models (LLMs) like Kimi K3 have billions or trillions of parameters, requiring massive amounts of memory for inference. Traditional approaches load the entire model into RAM or GPU memory, which is often infeasible for consumer hardware. Streaming weights from storage, such as NVMe SSDs, allows the model to run by fetching only the necessary parts at each step, trading storage bandwidth for memory capacity.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sqliteai/waste">GitHub - sqliteai / waste : Run the full 2.78-trillion-parameter Kimi...</a></li>
<li><a href="https://trendshift.io/repositories/96638">sqliteai / waste — GitHub trending stats & insights | Trendshift</a></li>

</ul>
</details>

**Tags**: `#SQLite`, `#AI`, `#data management`, `#open source`, `#Karpathy`

---

<a id="item-8"></a>
## [Karpathy's AI Pelican Sparks Debate on Physical World Benchmarks](https://twitter.com/karpathy/status/2083749667410727319) ⭐️ 7.0/10

Andrej Karpathy shared an AI-generated 3D animation of a pelican on Twitter, which quickly sparked a community discussion about using such outputs as benchmarks for AI's understanding of the physical world. The tweet gained significant engagement with 421 points and 333 comments. This discussion highlights a shift in AI evaluation from static image generation to dynamic 3D animations, which better expose a model's grasp of physical laws and spatial reasoning. It underscores the growing importance of benchmarks that measure physical world understanding, a key step toward more capable AI systems. Community members noted that the pelican animation was likely generated using three.js, a JavaScript 3D graphics library, and some suspected Anthropic models are specifically trained to excel at three.js code generation. The lack of a disclosed prompt for the animation was a point of contention, as it affects reproducibility.

hackernews · delichon · Aug 2, 04:05 · [Discussion](https://news.ycombinator.com/item?id=49140998)

**Background**: Physical AI refers to AI systems that can perceive, understand, and act in the real world, combining models with sensors and actuators. Traditional benchmarks often focus on text or static images, but 3D animations require models to reason about spatial relationships, object interactions, and physical plausibility, offering a more holistic test of understanding.

<details><summary>References</summary>
<ul>
<li><a href="https://artificialanalysis.ai/microevals/threejs-3d-modeling-and-animation-benchmark-1755135878779">Three.js 3 D Modeling and Animation Benchmark | Artificial Analysis</a></li>
<li><a href="https://venturebeat.com/technology/three-ways-ai-is-learning-to-understand-the-physical-world">Three ways AI is learning to understand the physical world | VentureBeat</a></li>
<li><a href="https://www.nvidia.com/en-us/glossary/generative-physical-ai/">What is Physical AI? | NVIDIA Glossary</a></li>

</ul>
</details>

**Discussion**: The community was divided: some praised the animation as a new benchmark for physical world understanding, while others criticized the lack of reproducibility and questioned whether three.js generation truly indicates physical understanding. Some commenters shared personal experiences with AI-generated 3D animations, noting the need for custom tuning and the limitations of current models in creating fully functional scenes.

**Tags**: `#AI`, `#3D animation`, `#benchmarks`, `#Karpathy`, `#machine learning`

---

<a id="item-9"></a>
## [F*: A General-Purpose Proof-Oriented Programming Language](https://fstar-lang.org/) ⭐️ 7.0/10

F* is a general-purpose, proof-oriented programming language that integrates formal verification, allowing developers to write programs together with machine-checked proofs of their properties. The language has been used in academic and industrial settings, with recent work including the Steel language for concurrent separation logic. F* matters because it enables high-assurance software development, particularly for critical systems where correctness is paramount. Its proof-oriented approach can reduce bugs and security vulnerabilities, and its practical use in migrating C codebases shows its real-world applicability. F* is pronounced 'F star' and is designed for writing programs with machine-checked proofs. The homepage lacks immediate code examples, which drew criticism from the community, but a tutorial is available at fstar-lang.org/tutorial.

hackernews · ducktective · Aug 2, 12:31 · [Discussion](https://news.ycombinator.com/item?id=49143925)

**Background**: Formal verification is a technique that uses mathematical methods to prove the correctness of systems, such as cryptographic protocols and software. Traditional languages rely on testing and debugging, but proof-oriented languages like F* integrate mathematical proof techniques into the development process, allowing for machine-checked proofs of program properties.

<details><summary>References</summary>
<ul>
<li><a href="https://fstar-lang.org/">F *: A Proof - Oriented Programming Language</a></li>
<li><a href="https://www.linkedin.com/pulse/f-general-purpose-proof-oriented-programming-language-kusho-4bipc">F * : A general-purpose proof - oriented programming language</a></li>
<li><a href="https://www.linuxlinks.com/f-general-purpose-proof-oriented-programming-language/">F * - general-purpose, proof - oriented programming language</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights both praise and criticism: some users appreciate F*'s utility for migrating C codebases, while others complain about the lack of code examples on the homepage. There is also curiosity about its industrial usage and a humorous comment about side effects in responsive stylesheets.

**Tags**: `#formal verification`, `#programming language`, `#proof-oriented`, `#functional programming`, `#F*`

---

<a id="item-10"></a>
## [EA to Be Acquired by Saudi-Led Consortium for $55B, Deal Closes Next Week](https://www.gamersky.com/news/202607/2180618.shtml) ⭐️ 7.0/10

Electronic Arts (EA) has announced that its sale to a consortium led by Saudi Arabia's Public Investment Fund (PIF), along with Silver Lake and Affinity Partners, has received all regulatory approvals. The $55 billion deal is expected to close on August 4, 2026, after which EA will become a private company. This acquisition is the second-largest in gaming history, underscoring Saudi Arabia's aggressive push into the global gaming industry. It will significantly expand PIF's gaming portfolio and could reshape industry dynamics, as EA's financials will no longer be public, reducing transparency for investors and competitors. The consortium includes PIF, Silver Lake, and Affinity Partners. The deal values EA at $55 billion, surpassing Microsoft's $75.4 billion acquisition of Activision Blizzard in 2023 as the second-largest gaming deal ever. PIF has previously acquired Scopely and Niantic outright, and holds stakes in other gaming companies.

telegram · zaihuapd · Aug 1, 09:10

**Background**: Saudi Arabia's Public Investment Fund has been aggressively investing in gaming as part of its Vision 2030 economic diversification plan. The fund has acquired stakes in major publishers like Nintendo and Take-Two, and has fully acquired mobile developers Scopely and Niantic. Silver Lake is a prominent technology-focused private equity firm, while Affinity Partners is an investment firm founded by Jared Kushner.

<details><summary>References</summary>
<ul>
<li><a href="https://english.indianews.in/tech-auto/from-riyadh-to-silicon-valley-how-ea-became-the-jewel-of-saudi-arabias-gaming-vision-840036/">From Riyadh to Silicon Valley: How EA became the jewel of Saudi ...</a></li>
<li><a href="https://www.nairaland.com/8533217/why-saudi-investing-heavily-gaming">Why Saudi Is Investing Heavily In Gaming : The $38B Gaming Drive...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Silver_Lake_(investment_firm)">Silver Lake (investment firm) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Affinity_Partners">Affinity Partners - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#EA`, `#acquisition`, `#gaming`, `#Saudi PIF`, `#industry news`

---

<a id="item-11"></a>
## [CXMT Unveils DDR5 and LPDDR5X, DDR5 Hits 8000Mbps](https://t.me/zaihuapd/42925) ⭐️ 7.0/10

At IC China, CXMT (ChangXin Memory Technologies) showcased its latest DDR5 and LPDDR5X product lines for the first time. The DDR5 series reaches a maximum speed of 8000Mbps, while the LPDDR5X tops out at 10667Mbps. This marks a significant milestone for China's semiconductor industry, as CXMT's DDR5 speed now enters the international top tier, potentially reshaping the global memory market. The 25% speed improvement over mainstream 6400Mbps products could pressure competitors and offer more options for data centers and mobile devices. The DDR5 series also includes a 24Gb high-capacity die for data center expansion, while the LPDDR5X offers 16Gb dies and packaging solutions from 12GB to 32GB. These products are already in mass production, with CXMT reportedly producing 24Gb DDR5 modules at 8000Mbps and 16Gb LPDDR5X at 10667Mbps.

telegram · zaihuapd · Aug 1, 15:30

**Background**: DDR5 is the latest generation of DRAM memory, offering higher speeds and bandwidth compared to DDR4. LPDDR5X is a low-power variant designed for mobile devices. CXMT is China's first IDM company to achieve large-scale DRAM production, and its progress is closely watched amid global supply chain dynamics and technology restrictions.

<details><summary>References</summary>
<ul>
<li><a href="https://larcomse.com/news/shownews.php?id=84">长鑫存储官宣发布 LPDDR 5 X ！ 速 率 登顶 10667 Mbps ...</a></li>
<li><a href="https://www.csdn.net/article/2025-12-05/155597521">全球存储格局或将重塑！ 长鑫 LPDDR 5 X 以 10667 Mbps ...</a></li>
<li><a href="https://www.chiphell.com/thread-2846391-1-1.html">长 鑫 存 储 产能快速飙升 预计年末达每月35...</a></li>

</ul>
</details>

**Tags**: `#半导体`, `#DDR5`, `#存储`, `#长鑫存储`, `#LPDDR5X`

---

<a id="item-12"></a>
## [AI Chip Count Doubles Every 9 Months, Set to Reach 200 Million by 2028](https://www.nytimes.com/interactive/2026/07/29/technology/ai-chips-data-center-boom.html) ⭐️ 7.0/10

According to Epoch AI, the global number of AI chips is currently around 20 million and is doubling every nine months, projected to reach approximately 200 million by the end of 2028. IDC forecasts that global AI infrastructure investment will surpass $1 trillion by 2029, up from $318 billion last year. This explosive growth in AI chip deployment signals an unprecedented scale of infrastructure investment, driven by the scaling law that more compute leads to more capable AI. It has significant implications for energy consumption, environmental impact, and the economic sustainability of AI, as well as geopolitical competition, with the US controlling about 80% of global AI compute. The US controls about 80% of global AI compute, and Google alone is believed to have four times as many AI chips as all Chinese companies combined. China is accelerating its efforts through self-developed semiconductors and AI infrastructure, but the massive buildout is causing electricity price increases and environmental disputes, with economists warning that current spending may exceed profitability.

telegram · zaihuapd · Aug 2, 01:01

**Background**: The scaling law in AI refers to the empirical observation that increasing model size, training data, and compute leads to predictable improvements in AI performance. This has driven tech giants to invest heavily in data centers and specialized AI chips, such as GPUs and TPUs, to train and run increasingly powerful models. The rapid growth in AI infrastructure is reminiscent of historical infrastructure booms, which have sometimes ended in bubbles.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Epoch_AI">Epoch AI</a></li>
<li><a href="https://en.wikipedia.org/wiki/Neural_scaling_law">Neural scaling law - Wikipedia</a></li>
<li><a href="https://www.linkedin.com/posts/alejandro-antunez_idc-explosive-growth-in-ai-infrastructure-activity-7249459714709692416-KJVo">IDC : Explosive Growth in AI Infrastructure Investment | Official...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#infrastructure`, `#scaling laws`, `#data centers`, `#investment`

---

<a id="item-13"></a>
## [Apple Limits Bug Reports to Curb AI-Generated Slop](https://www.ft.com/content/4532122d-90f2-4433-9df6-ca99d8a141d2?syn-25a6b1a6=1) ⭐️ 7.0/10

Apple has restricted the number of vulnerability reports researchers can submit simultaneously, imposing a 30-day cooldown period, to counter a surge of low-quality, AI-generated security reports. Italian startup Bynario, using ChatGPT, discovered over 50 macOS vulnerabilities in three weeks, including a privilege escalation chain, but was blocked from reporting them due to the new limits. This highlights the dual impact of AI on cybersecurity: while AI can accelerate vulnerability discovery, it also floods vendors with low-quality reports, forcing policy changes that may inadvertently hinder legitimate researchers. The incident underscores the need for balanced disclosure policies that filter noise without blocking genuine findings. Bynario's CEO Alfredo Pesoli estimates the unreported flaw's black-market value at $100,000 to $200,000. Apple has since contacted Bynario to review their submissions, and its latest security update fixed about five times the usual number of vulnerabilities, crediting Anthropic and OpenAI tools.

telegram · zaihuapd · Aug 2, 05:50

**Background**: Apple's bug bounty program encourages researchers to report vulnerabilities for rewards, but the influx of AI-generated reports has overwhelmed reviewers. Similar issues have affected other projects; for example, Linux kernel maintainer Linus Torvalds has complained about AI-generated bug report spam. AI tools like ChatGPT can now assist in finding real vulnerabilities, but they also produce many false positives.

<details><summary>References</summary>
<ul>
<li><a href="https://the-decoder.com/a-real-macos-flaw-worth-200k-went-unreported-because-apples-bug-bounty-inbox-was-full-of-ai-slop/">A real macOS flaw worth $200K went unreported because Apple's bug...</a></li>
<li><a href="https://bugflation.com/systems/bynario-ai/">BynarIO AI - Bugflation</a></li>
<li><a href="https://www.artofsm.art/t/linus-torvalds-blasts-ai-security-bug-reports/18906">Linus Torvalds Blasts AI Security Bug Reports - security - Art of Smart</a></li>

</ul>
</details>

**Discussion**: The discussion is likely to be active given the controversy over limiting reports. Some may argue that Apple's policy is necessary to manage AI slop, while others may criticize it for hindering legitimate researchers and potentially leaving vulnerabilities unpatched.

**Tags**: `#cybersecurity`, `#AI`, `#vulnerability disclosure`, `#Apple`, `#macOS`

---

<a id="item-14"></a>
## [Chinese AI Framework Detects Bitcoin Money Laundering with 90% Accuracy](https://www.scmp.com/news/china/science/article/3362493/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-90-accuracy) ⭐️ 7.0/10

Researchers from the People's Public Security University of China have developed an AI framework that combines memory modules and large language models to detect illicit Bitcoin transactions with nearly 90% accuracy. The findings were published in the May issue of the peer-reviewed journal Intelligence Journal. This development provides law enforcement and financial regulators with a powerful tool to combat cryptocurrency-related money laundering, which has been a growing concern globally. It demonstrates the practical application of AI in enhancing financial crime detection and could influence future regulatory approaches. The framework reportedly achieves nearly 90% overall accuracy in identifying illicit transactions. According to China's Supreme People's Procuratorate, prosecutors indicted 3,259 individuals in 2025 for money laundering involving virtual currencies and underground banks.

telegram · zaihuapd · Aug 2, 08:22

**Background**: Bitcoin and other cryptocurrencies offer pseudonymity, making them attractive for money laundering and other illicit activities. Traditional detection methods often struggle with the scale and anonymity of blockchain transactions. This new AI framework leverages advanced machine learning techniques to analyze transaction patterns and identify suspicious activities, providing a more efficient and explainable approach for regulators.

<details><summary>References</summary>
<ul>
<li><a href="https://www.scmp.com/news/china/science/article/3362493/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-90-accuracy?pgtype=live">Chinese police AI algorithm tracks bitcoin money laundering with 90 ...</a></li>
<li><a href="https://dallasgazettenews.com/2026/08/01/chinese-police-ai-algorithm-tracks-bitcoin-money-laundering-with-90-accuracy/">Chinese police AI algorithm tracks bitcoin money laundering with 90 ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cryptocurrency`, `#money laundering`, `#law enforcement`, `#research`

---

<a id="item-15"></a>
## [China Issues Mandatory Standard for Public Warning SMS](https://t.me/zaihuapd/42937) ⭐️ 7.0/10

China's State Administration for Market Regulation approved and released the mandatory national standard GB 32634-2025 for public warning short message service, which will take effect on May 1, 2026. This standard replaces the previous recommended standard GB/T 32634-2016, upgrading it from a voluntary to a mandatory requirement. This upgrade makes compliance mandatory for telecom operators and device manufacturers, ensuring more reliable and standardized public warning SMS across China. It strengthens national disaster alert capabilities, particularly for earthquakes and other natural disasters, potentially saving lives through more effective emergency communication. The standard is administered by the Ministry of Industry and Information Technology, with major drafting units including the China Academy of Information and Communications Technology (CAICT), China Telecom, China Mobile, and China Unicom. It covers overall requirements, business processes, and terminal specifications for public warning SMS, supporting national-level emergency alerts for natural disasters.

telegram · zaihuapd · Aug 2, 10:16

**Background**: In China, national standards are divided into mandatory (GB) and recommended (GB/T) categories. Mandatory standards have legal force and must be followed, while recommended standards are voluntary. Public warning SMS is a service that uses cell broadcast or point-to-point messaging to deliver emergency alerts to mobile users, and this new mandatory standard aims to ensure consistent and reliable implementation across networks and devices.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bzpt.com/gb/425984.html">GB 32634 - 2025 公 共 预 警 短 消 息 业 务 技 术 要 求 .pdf_标准平台</a></li>
<li><a href="https://www.antpedia.com/standard/1764613859.html">GB 32634 - 2025 公 共 预 警 短 消 息 业 务 技 术 要 求 标准</a></li>
<li><a href="http://deweixiansz.com/list_27/1174.html">deweixiansz.com/list_27/1174.html</a></li>

</ul>
</details>

**Tags**: `#public warning`, `#SMS`, `#standard`, `#China`, `#telecommunications`

---

<a id="item-16"></a>
## [Microplastics Found in 92% of Animals Near Deep-Sea Hydrothermal Vents](https://www.yahoo.com/news/science/articles/most-isolated-environments-microplastics-finding-020000452.html) ⭐️ 7.0/10

A study led by the Korea Research Institute of Bioscience and Biotechnology, published in Water Research, detected microplastics in 11 out of 12 animals (92%) sampled near deep-sea hydrothermal vents at about 2000 meters depth in the Southwest Pacific and Indian Oceans. The average concentration was 3.42 pieces per animal, with polystyrene being the most common polymer. This finding demonstrates that microplastic pollution has reached even the most remote and pristine deep-sea ecosystems, highlighting the global scale of plastic contamination. It underscores the urgent need for source reduction, as cleanup in deep-sea environments is practically impossible, and provides critical data for deep-sea monitoring and conservation policies. The study examined four animal species, including filter-feeding mussels and herbivorous snails. Microplastics were evenly distributed in mussels but concentrated in the digestive organs of snails, and concentrations were higher in Indian Ocean samples than in Pacific ones.

telegram · zaihuapd · Aug 2, 11:00

**Background**: Deep-sea hydrothermal vents are extreme environments discovered only in 1977, supporting unique ecosystems that rely on chemosynthesis rather than sunlight. Microplastics are tiny plastic particles less than 5mm in size, which can be ingested by marine organisms and enter the food chain. Previous research has shown that filter-feeding animals, such as whales and shellfish, can ingest large quantities of microplastics, posing risks to both marine life and human health.

<details><summary>References</summary>
<ul>
<li><a href="https://news.sciencenet.cn/htmlpaper/2025/5/2025512155355670132746.shtm">99.999%的 深 海 海 底仍未被人类探索—论文—科学网</a></li>
<li><a href="https://news.sciencenet.cn/htmlnews/2022/11/488718.shtm">国际最新研究：美海岸 滤 食 性 鲸每天 摄 入 最多1000...</a></li>

</ul>
</details>

**Tags**: `#microplastics`, `#deep-sea`, `#environmental science`, `#pollution`, `#marine biology`

---

<a id="item-17"></a>
## [U.S. States Move to Repeal Data Center Tax Breaks, Raising AI Infrastructure Costs](https://theinformation.com/articles/exclusive-data-center-costs-set-rise-u-s-states-move-repeal-tax-breaks) ⭐️ 7.0/10

Several U.S. states are considering repealing or tightening tax breaks for data centers, which could increase the cost of building AI infrastructure. The Information reports that this policy shift comes as data centers' electricity demand and fiscal pressures mount. This policy shift could significantly raise the cost of data center construction in the U.S., affecting the economics of AI infrastructure deployment. It may influence where companies choose to build data centers and could slow the pace of AI expansion, impacting cloud providers and AI startups alike. The report notes that states previously exempted server and electricity costs to attract data center investment, but now some are reconsidering these incentives. The exact states and timelines are not specified in the summary, but the trend suggests a broader reassessment of tax incentives amid rising AI-driven demand.

telegram · zaihuapd · Aug 3, 00:42

**Background**: Data centers are facilities that house computer systems and associated components, such as telecommunications and storage. They are critical for cloud computing and AI training, which require massive computational power and electricity. To attract these facilities, many U.S. states have offered tax exemptions on equipment and utilities, but the rapid growth of AI has led to soaring energy demands and infrastructure costs, prompting some states to reconsider these incentives. According to a Data Center Watch project, about 20 data center projects were blocked or delayed between March and June last year, involving nearly $98 billion in investment, reflecting growing local resistance.

<details><summary>References</summary>
<ul>
<li><a href="https://m.cnbeta.com.tw/view/1557568.htm">威斯康星小城全民公投叫停 数 据 中 心 税 收 优 惠 - cnBeta.COM 移动版</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#data centers`, `#tax policy`, `#cloud computing`, `#regulation`

---