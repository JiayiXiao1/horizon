---
layout: default
title: "Horizon Summary: 2026-07-04 (EN)"
date: 2026-07-04
lang: en
---

> From 46 items, 19 important content pieces were selected

---

1. [European Parliament Spy Probe Member Hacked with Pegasus](#item-1) ⭐️ 8.0/10
2. [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](#item-2) ⭐️ 8.0/10
3. [Open Source AI Gap Map Launched](#item-3) ⭐️ 8.0/10
4. [Josh Comeau Reports 50%+ Drop in Developer Course Sales Due to AI](#item-4) ⭐️ 8.0/10
5. [Understand to Participate: Avoiding Cognitive Debt with AI](#item-5) ⭐️ 8.0/10
6. [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](#item-6) ⭐️ 8.0/10
7. [Huawei Launches Atlas 350 with Ascend 950PR, Claims 2.87x H20 Performance](#item-7) ⭐️ 8.0/10
8. [NASA Launches Rescue Satellite to Save Failing Space Telescope](#item-8) ⭐️ 8.0/10
9. [Tencent Atuin AI beats Mythos in CyberGym benchmark](#item-9) ⭐️ 8.0/10
10. [Karpathy Launches NanoChat: ChatGPT for $100](#item-10) ⭐️ 7.0/10
11. [Guide to Running SOTA LLMs Locally Sparks Cost Debate](#item-11) ⭐️ 7.0/10
12. [Costco as the Anti-Amazon: A Retail Model Analysis](#item-12) ⭐️ 7.0/10
13. [Factories Are Just Rooms: Rethinking Manufacturing](#item-13) ⭐️ 7.0/10
14. [Wordgard: New Rich-Text Editor by ProseMirror Creator](#item-14) ⭐️ 7.0/10
15. [Using DSPy to Evaluate and Improve Datasette Agent Prompts](#item-15) ⭐️ 7.0/10
16. [Google Gemini Omni Flash Tops Video Arena](#item-16) ⭐️ 7.0/10
17. [Claude Fable 5 Relaunch Disappoints with Nerfed Performance](#item-17) ⭐️ 7.0/10
18. [China Proposes Account Deactivation After 6 Months of Inactivity](#item-18) ⭐️ 7.0/10
19. [Huawei Mate 80 Pro gaming efficiency beats Snapdragon 8 Gen3](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [European Parliament Spy Probe Member Hacked with Pegasus](https://citizenlab.ca/research/member-of-committee-investigating-spyware-hacked-with-pegasus/) ⭐️ 8.0/10

Citizen Lab confirmed that a member of the European Parliament's committee investigating spyware was infected with Pegasus spyware on multiple occasions in 2022 and 2023. This incident reveals a coordinated multi-country espionage campaign targeting EU institutions, undermining democratic oversight and raising serious concerns about state-sponsored surveillance. The first infection on October 21, 2022, overlaps with a known Pegasus campaign against exiled journalists, suggesting a customer with cross-border spying authorization. The device also contained confidential medical and government documents.

hackernews · ledoge · Jul 3, 20:38 · [Discussion](https://news.ycombinator.com/item?id=48779683)

**Background**: Pegasus is a powerful spyware developed by Israeli firm NSO Group, capable of remotely compromising mobile devices. Citizen Lab is a University of Toronto research group that investigates digital threats. The European Parliament has been probing the misuse of spyware like Pegasus across member states.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Pegasus_(spyware)">Pegasus (spyware)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Citizen_Lab">Citizen Lab</a></li>

</ul>
</details>

**Discussion**: Commenters noted the irony of an EU parliament member being spied on by the same spyware used against journalists, and linked the incident to ongoing Greek and Italian spyware scandals. Some questioned why the parliament lacks policies separating work and personal devices.

**Tags**: `#cybersecurity`, `#spyware`, `#Pegasus`, `#European Parliament`, `#surveillance`

---

<a id="item-2"></a>
## [Ubicloud Advocates Strict Memory Overcommit for PostgreSQL](https://www.ubicloud.com/blog/postgresql-and-the-oom-killer-why-we-use-strict-memory-overcommit) ⭐️ 8.0/10

Ubicloud published a blog post explaining why they use strict memory overcommit (vm.overcommit_memory=2) for PostgreSQL to prevent the OOM killer from terminating the postmaster process. This practice improves PostgreSQL stability in production environments, but the trade-offs—such as potential fork failures—spark debate among database operators about the best memory management strategy. Strict overcommit (mode 2) prevents the kernel from overcommitting memory, reducing OOM killer risks but requiring careful tuning of vm.overcommit_ratio to avoid process fork failures.

hackernews · furkansahin · Jul 3, 13:00 · [Discussion](https://news.ycombinator.com/item?id=48774509)

**Background**: Linux uses memory overcommit by default, allowing processes to allocate more virtual memory than physical RAM. When memory runs out, the OOM killer terminates processes to free memory, which can kill critical database processes like PostgreSQL's postmaster. Disabling overcommit (mode 2) forces the kernel to respect actual memory limits, but can cause allocation failures if not configured properly.

<details><summary>References</summary>
<ul>
<li><a href="https://linuxhandbook.com/oom-killer/">What is Out of Memory Killer (OOM Killer) in Linux?</a></li>
<li><a href="https://www.cybertec-postgresql.com/en/what-you-should-know-about-linux-memory-overcommit-in-postgresql/">Memory overcommit and PostgreSQL | CYBERTEC PostgreSQL</a></li>
<li><a href="https://www.hivelocity.net/kb/how-does-memory-overcommit-affect-postgresql/">How does memory overcommit affect PostgreSQL ?</a></li>

</ul>
</details>

**Discussion**: Commenters noted that Linux default memory settings are problematic, with some cautioning that strict overcommit can cause fork failures if overcommit_ratio is not adjusted. The author acknowledged the title was too strong, emphasizing that strict overcommit is suitable for managed PostgreSQL but not all scenarios.

**Tags**: `#PostgreSQL`, `#Linux`, `#memory management`, `#OOM killer`, `#database administration`

---

<a id="item-3"></a>
## [Open Source AI Gap Map Launched](https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/#atom-everything) ⭐️ 8.0/10

Current AI, a non-profit founded at the AI Action Summit in Paris in February 2025, launched the Open Source AI Gap Map v0.1, indexing 421 products across software, models, datasets, and hardware, with the underlying data released under an MIT license on GitHub. This comprehensive mapping of the open-source AI ecosystem helps identify critical gaps, guiding researchers and practitioners on where to focus efforts and investment, thereby accelerating the development of open-source AI. The map details 266 software tools, 85 models, 50 datasets, and 20 hardware projects from 228 organizations, organized into 14 categories across 3 stack layers, while over 24,000 additional artifacts remain uncategorized.

rss · Simon Willison · Jul 3, 22:04

**Background**: Current AI is a global non-profit partnership backed by $400 million in committed capital, aiming to build a public option for AI. The Gap Map builds on work from leading open-source AI experts at the Columbia Convening, MOF, Hugging Face, and others, evaluating over 24,626 projects across openness, capability, and adoption.

<details><summary>References</summary>
<ul>
<li><a href="https://map.currentai.org/">Current AI - Open Source AI Gap Map</a></li>
<li><a href="https://simonwillison.net/2026/Jul/3/open-source-ai-gap-map/">Open Source AI Gap Map - simonwillison.net</a></li>
<li><a href="https://www.currentai.org/blogs/introducing-the-gap-map-v0-1">Introducing the Gap Map v0.1 - currentai.org</a></li>

</ul>
</details>

**Tags**: `#open source`, `#AI`, `#ecosystem mapping`, `#non-profit`, `#Current AI`

---

<a id="item-4"></a>
## [Josh Comeau Reports 50%+ Drop in Developer Course Sales Due to AI](https://simonwillison.net/2026/Jul/3/josh-w-comeau/#atom-everything) ⭐️ 8.0/10

Josh W. Comeau, a respected front-end developer educator, reported that sales for his newly launched course 'Whimsical Animations' are on track to be roughly one-third of a typical launch, and his existing courses have seen revenue declines of over 50% compared to last year. This signals a major shift in the developer education market, as AI-generated job uncertainty and the availability of LLM-based personalized tutoring reduce demand for paid courses. It highlights a broader trend affecting technical educators and content creators who rely on course sales. Comeau noted a 'double whammy' from AI: people are hesitant to invest time and money in learning new developer skills due to job uncertainty, and LLMs can provide personalized tutoring, reducing the incentive to buy paid courses. He also mentioned that other course creators are seeing similar declines of 50% or more.

rss · Simon Willison · Jul 3, 21:25

**Background**: Josh W. Comeau is a well-known front-end developer and educator, famous for his interactive courses on CSS and React. His new course 'Whimsical Animations' teaches animation techniques using CSS, JavaScript, SVG, and Canvas. The rise of large language models (LLMs) like GPT-4 has enabled AI-powered tutoring systems that can adapt to individual learners, potentially competing with traditional online courses.

<details><summary>References</summary>
<ul>
<li><a href="https://whimsy.joshwcomeau.com/">Whimsical Animations , a new course from Josh W. Comeau</a></li>

</ul>
</details>

**Tags**: `#AI impact`, `#developer education`, `#online courses`, `#industry trends`

---

<a id="item-5"></a>
## [Understand to Participate: Avoiding Cognitive Debt with AI](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Simon Willison highlights Geoffrey Litt's concept of 'understand to participate' as a strategy to avoid cognitive debt when collaborating with coding agents, emphasizing the need for developers to maintain deep understanding of AI-generated code. As AI coding agents produce increasingly large and complex changes, developers risk accumulating cognitive debt—a loss of shared understanding that hinders safe and effective collaboration. This concept provides a framework for maintaining human agency and code quality in AI-assisted development. Geoffrey Litt presented this idea at the AI Engineer World's Fair (AIE) 2026, and his talk is expected to be released on YouTube within three weeks. He also published a thread version of his talk on Twitter.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the erosion of shared understanding across a software system over time, leading to inadequate mental models for reasoning about and safely changing the system. As AI agents write code faster than humans can absorb it, developers must actively understand the code to participate creatively and avoid falling behind.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Jul/2/understand-to-participate/">Understand to participate | Simon Willison’s Weblog</a></li>
<li><a href="https://www.geoffreylitt.com/2026/07/02/understanding-is-the-new-bottleneck.html">Understanding is the new bottleneck</a></li>
<li><a href="https://margaretstorey.com/blog/2026/02/09/cognitive-debt/">How Generative and Agentic AI Shift Concern from Technical Debt to Cognitive Debt</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#cognitive debt`, `#human-AI collaboration`, `#software engineering`

---

<a id="item-6"></a>
## [Anthropic Accuses Alibaba of Massive Distillation Attack on Claude](https://t.me/zaihuapd/42327) ⭐️ 8.0/10

Anthropic has accused Alibaba of orchestrating a massive 'distillation attack' using approximately 25,000 fraudulent accounts to extract capabilities from its Claude AI model, with over 28.8 million interactions between April 22 and June 5, 2026. Alibaba subsequently ordered all employees to uninstall Claude-related products, effective July 10. This incident highlights escalating tensions in AI security and intellectual property protection, with potential geopolitical implications as a Chinese tech giant is accused of systematically extracting proprietary AI capabilities. It underscores the vulnerability of large language models to distillation attacks and the need for robust defenses. Anthropic claims this is the largest known distillation attack against the company, involving Alibaba and its AI lab Qwen. The attack targeted Claude's capabilities, and Alibaba's internal ban on Claude products includes models like Sonnet, Opus, Fable, and agent products like Claude Code.

telegram · zaihuapd · Jul 3, 06:21

**Background**: Knowledge distillation is a technique where a smaller 'student' model learns from a larger 'teacher' model to replicate its performance, often used for model compression. In a 'distillation attack,' an adversary uses unauthorized access to query a proprietary model extensively and train a competing model. Qwen is Alibaba's family of large language models, some of which are open-source.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Knowledge_distillation">Knowledge distillation - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Qwen_(Alibaba_Cloud)">Qwen (Alibaba Cloud)</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#distillation attack`, `#Anthropic`, `#Alibaba`

---

<a id="item-7"></a>
## [Huawei Launches Atlas 350 with Ascend 950PR, Claims 2.87x H20 Performance](https://t.me/zaihuapd/42329) ⭐️ 8.0/10

Huawei announced and launched the Atlas 350 AI accelerator card featuring the new Ascend 950PR processor at the Huawei China Partner Conference 2026, claiming 2.87 times the compute power of Nvidia's H20 and support for FP4 low-precision inference. This marks Huawei's most aggressive challenge to Nvidia's dominance in the Chinese AI chip market, offering a domestic alternative with competitive performance for training and inference. The support for FP4 inference could significantly reduce costs and latency for large language model deployment. The Atlas 350 features 112 GB of HBM memory and can load a 70B parameter model on a single card. The Ascend 950PR chip delivers 1.56 petaflops of AI inference performance, and Huawei plans to ship 750,000 units this year.

telegram · zaihuapd · Jul 3, 08:35

**Background**: Huawei's Ascend series is a line of AI processors designed to compete with Nvidia's GPUs in China, especially under US export restrictions. FP4 (4-bit floating point) is a low-precision format that can accelerate inference while maintaining accuracy, and Nvidia's Blackwell architecture also supports a similar format called NVFP4. The H20 is a China-specific Nvidia chip with reduced performance to comply with US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huaweicentral.com/ascend-950pr-ai-chip-everything-you-need-to-know/">Ascend 950PR AI Chip: Everything you need to know - Huawei Central</a></li>
<li><a href="https://tech-insider.org/huawei-ascend-950pr-ai-chip-nvidia-china-2026/">Huawei Ascend 950PR: The 1.56 PFLOP AI Chip vs Nvidia [2026]</a></li>
<li><a href="https://developer.nvidia.com/blog/introducing-nvfp4-for-efficient-and-accurate-low-precision-inference/">Introducing NVFP4 for Efficient and Accurate Low-Precision Inference | NVIDIA Technical Blog</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#AI hardware`, `#Ascend`, `#Atlas 350`, `#Nvidia H20`

---

<a id="item-8"></a>
## [NASA Launches Rescue Satellite to Save Failing Space Telescope](https://apnews.com/article/swift-nasa-satellite-rescue-katalyst-a7ddd740ca099587c58865f583c7245a) ⭐️ 8.0/10

On July 3, 2026, NASA launched the LINK spacecraft, built by Katalyst Space Technologies, to rendezvous with and boost the aging Swift space telescope to a higher orbit, preventing its uncontrolled reentry into Earth's atmosphere. This mission marks the first time a private spacecraft will attempt to capture and service a US government satellite not designed for docking, potentially revolutionizing on-orbit servicing and space debris management. The LINK spacecraft will use a robotic arm to secure the telescope and then fire thrusters to raise its orbit by about 240 kilometers. If successful, Swift could resume observations as early as September 2026.

telegram · zaihuapd · Jul 3, 15:43

**Background**: The Neil Gehrels Swift Observatory, launched in 2004, studies gamma-ray bursts and other cosmic phenomena. Its orbit has been decaying due to increased solar activity, and without intervention, it would have burned up in the atmosphere by late 2026. On-orbit satellite servicing involves robotic spacecraft performing maintenance or orbit adjustments on existing satellites, a capability that has been limited to government missions until now.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LINK_spacecraft">LINK spacecraft</a></li>
<li><a href="https://en.wikipedia.org/wiki/Swift_rescue_mission">Swift Boost Mission - Wikipedia</a></li>
<li><a href="https://easternherald.com/2026/07/03/swift-telescope-rescue-launch-delay-pegasus-xl/">NASA Swift Telescope Rescue Delayed by Rocket Anomaly</a></li>

</ul>
</details>

**Tags**: `#space`, `#satellite servicing`, `#NASA`, `#space debris`, `#private space industry`

---

<a id="item-9"></a>
## [Tencent Atuin AI beats Mythos in CyberGym benchmark](https://mp.weixin.qq.com/s/BzU7g-2iG7d6h4ViwMhxyg) ⭐️ 8.0/10

Tencent Xuanwu Lab's Atuin AI achieved an 84.0% score on the CyberGym cybersecurity benchmark, surpassing Anthropic's Claude Mythos Preview, while costing less than 0.1% of Mythos's Project Glasswing budget. This demonstrates that open-source, locally deployable AI models can outperform proprietary frontier models in vulnerability detection at a fraction of the cost, potentially democratizing advanced cybersecurity AI. Atuin AI is built on the open-source GLM-5.1 model and discovered multiple critical logic vulnerabilities in projects like curl, OpenSSL, and Python cryptography that Mythos missed, with severity scores up to 9.3. It ranked 1st in severe vulnerability severity and 5th in total count on the Berkeley BVI real-world vulnerability list.

telegram · zaihuapd · Jul 3, 16:12

**Background**: CyberGym is a cybersecurity benchmark led by UC Berkeley that evaluates AI models on vulnerability detection. GLM-5.1 is an open-source large language model designed for agentic tasks and long-horizon reasoning. Project Glasswing is Anthropic's initiative to provide Claude Mythos Preview to select organizations for defensive security.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/zai-org/GLM-5.1">zai-org/GLM-5.1 · Hugging Face</a></li>
<li><a href="https://blog.cloudflare.com/cyber-frontier-models/">Project Glasswing: what Mythos showed us</a></li>
<li><a href="https://www.softwareimprovementgroup.com/blog/mythos-project-glasswing-security/">Mythos and project Glasswing explained - SIG</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cybersecurity`, `#vulnerability detection`, `#benchmark`, `#open-source`

---

<a id="item-10"></a>
## [Karpathy Launches NanoChat: ChatGPT for $100](https://github.com/karpathy/nanochat) ⭐️ 7.0/10

Andrej Karpathy created a new branch in the nanochat repository on GitHub, aiming to build a ChatGPT-like model for just $100. This project demonstrates that large language models can be trained cost-effectively, potentially democratizing AI development and making it accessible to individuals and small teams. The nanochat project is written in approximately 8,000 lines of PyTorch and focuses on achieving a 'time to GPT-2' metric, outperforming GPT-2 (1.6B) on an 8xH100 GPU node.

github · karpathy · Jul 3, 17:47

**Background**: Large language models like ChatGPT typically require massive computational resources and millions of dollars to train. Karpathy's nanochat aims to show that with careful engineering and compute-optimal scaling, a capable model can be trained on a budget of $100.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/karpathy/nanochat">GitHub - karpathy / nanochat : The best ChatGPT that $100 can buy.</a></li>
<li><a href="https://www.analyticsvidhya.com/blog/2025/10/andrej-karpathys-nanochat/">Build ChatGPT Clone with Andrej Karpathy 's nanochat</a></li>

</ul>
</details>

**Tags**: `#AI`, `#LLM`, `#open-source`, `#cost-efficiency`

---

<a id="item-11"></a>
## [Guide to Running SOTA LLMs Locally Sparks Cost Debate](https://github.com/jamesob/local-llm) ⭐️ 7.0/10

Jamesob published a comprehensive guide on building and running state-of-the-art large language models locally, including a $40K+ hardware build for near-Claude Opus performance. This guide highlights the growing interest in local AI inference but also exposes the prohibitive costs and practical limitations, sparking debate on whether local setups are worth the investment compared to cloud subscriptions. The guide's flagship build uses 4 GPUs at $12K each, totaling $50-55K, and relies on quantization and pruning techniques like REAP to reduce model size. A more affordable option is 2x RTX 3090s with 48GB VRAM for running Qwen3.6-27B.

hackernews · livestyle · Jul 3, 15:03 · [Discussion](https://news.ycombinator.com/item?id=48775921)

**Background**: Local LLM inference means running trained models on personal hardware instead of cloud servers. SOTA (state-of-the-art) models require massive computational resources, often necessitating expensive GPUs and techniques like quantization to fit into available VRAM.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/blog/daya-shankar/sota-ai-models">SOTA AI Models: Benchmarks, Metrics & Deployment Guide</a></li>
<li><a href="https://prajnaaiwisdom.medium.com/what-is-local-llm-inference-a-beginners-guide-b31043768d4f">What Is Local LLM Inference? A Beginner’s Guide | by PrajnaAI | Medium</a></li>
<li><a href="https://www.redhat.com/en/topics/ai/ai-infrastructure-explained">AI infrastructure explained</a></li>

</ul>
</details>

**Discussion**: Commenters widely agree that local setups are still far more expensive and lower quality than cloud subscriptions like Claude Opus at $200/month, with one noting $40K equals 16.8 years of subscription. Others point out that even with expensive hardware, pruned models may perform poorly outside benchmarks, and suggest mid-range options like 128GB unified memory for DeepSeek V4 flash.

**Tags**: `#LLM`, `#local inference`, `#hardware`, `#open-source`, `#AI infrastructure`

---

<a id="item-12"></a>
## [Costco as the Anti-Amazon: A Retail Model Analysis](https://phenomenalworld.org/analysis/the-anti-amazon/) ⭐️ 7.0/10

An article argues that Costco's warehouse club model, which relies on bulk sales and customer self-transport, is more efficient and socially beneficial than Amazon's home delivery model, highlighting differences in logistics and consumer behavior. This analysis challenges the prevailing e-commerce paradigm by questioning the societal costs of last-mile delivery, offering a counterpoint that could influence retail strategy and consumer choices. Costco avoids the last-mile delivery problem by having customers transport goods themselves, reducing logistical complexity and environmental impact compared to Amazon's single-package home deliveries.

hackernews · bookofjoe · Jul 3, 15:14 · [Discussion](https://news.ycombinator.com/item?id=48776044)

**Background**: Costco operates warehouse stores where members buy in bulk at low prices, while Amazon dominates e-commerce with home delivery of individual items. The article contrasts their supply chains: Costco uses freight trucks to stores, Amazon uses a vast delivery network to homes.

**Discussion**: Commenters debated the trade-offs, with some noting that home delivery can be more efficient for dense populations, while others praised Costco for avoiding last-mile complexity. A user highlighted that they use a mix of shopping methods, reflecting diverse consumer strategies.

**Tags**: `#retail`, `#logistics`, `#e-commerce`, `#business strategy`, `#consumer behavior`

---

<a id="item-13"></a>
## [Factories Are Just Rooms: Rethinking Manufacturing](https://interconnected.org/home/2026/07/03/factories) ⭐️ 7.0/10

An essay and discussion on Hacker News argue that factories can be as simple as a single room, challenging the assumption that manufacturing requires massive scale and complex infrastructure. This perspective encourages innovation in small-scale, local manufacturing, potentially lowering barriers to entry for entrepreneurs and reshaping how we think about production and supply chains. The discussion includes real-world examples of small factories operating out of single rooms, but also highlights challenges such as inconsistent business and the need for specialized knowledge.

hackernews · arbesman · Jul 3, 15:13 · [Discussion](https://news.ycombinator.com/item?id=48776035)

**Background**: Traditional manufacturing often involves large factories with specialized machinery and assembly lines. The idea that a factory can be just a room challenges this paradigm, emphasizing flexibility and simplicity.

**Discussion**: Commenters share mixed experiences: some romanticize small-scale manufacturing, while others point out practical difficulties like inconsistent demand and the need for process optimization. A few compare fast-food kitchens to efficient factories.

**Tags**: `#manufacturing`, `#production`, `#innovation`, `#philosophy`, `#engineering`

---

<a id="item-14"></a>
## [Wordgard: New Rich-Text Editor by ProseMirror Creator](https://wordgard.net/) ⭐️ 7.0/10

Wordgard is a new in-browser rich-text editor framework released by Marijn Haverbeke, the creator of ProseMirror, with a different architecture and no upgrade path from ProseMirror. This matters because it introduces a fresh approach to rich-text editing from a highly respected developer, potentially influencing the future of web-based content editors and sparking debate among developers who rely on ProseMirror-based tools like Tiptap. Wordgard shares many concepts with ProseMirror but is not backward-compatible, meaning existing ProseMirror users would need to rewrite their editor implementations to switch. The project is hosted on code.haverbeke.berlin and is open source.

hackernews · indy · Jul 3, 08:50 · [Discussion](https://news.ycombinator.com/item?id=48772573)

**Background**: ProseMirror is a widely-used, battle-tested rich-text editor framework that powers many editors like Tiptap. It focuses on producing clean, semantic documents and has a lightweight core but a steep learning curve. Wordgard is a new project by the same author that rethinks some design decisions.

<details><summary>References</summary>
<ul>
<li><a href="https://wordgard.net/">Wordgard</a></li>
<li><a href="https://prosemirror.net/">ProseMirror</a></li>
<li><a href="https://code.haverbeke.berlin/wordgard/wordgard">wordgard / wordgard : The Wordgard rich text... - code.haverbeke.berlin</a></li>

</ul>
</details>

**Discussion**: The community is intrigued but cautious; many appreciate the design and concepts but note the lack of an upgrade path from ProseMirror. Some developers express frustration with ProseMirror's complexity and see Wordgard as a potential improvement, while others question the need for a new framework.

**Tags**: `#rich-text editor`, `#ProseMirror`, `#web development`, `#open source`

---

<a id="item-15"></a>
## [Using DSPy to Evaluate and Improve Datasette Agent Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used the DSPy framework to evaluate and improve the SQL system prompts for Datasette Agent, automating the research process with Claude Code (Claude Fable 5). This demonstrates a practical workflow for systematically optimizing LLM prompts using DSPy, which can be replicated by other developers to improve AI agent reliability and accuracy. DSPy identified that the schema listing only gave table names, causing the agent to guess column names and enter error-retry loops; suggested including column names in the prompt or softening the advice to avoid guessing.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy is a Python framework for programming language models, allowing optimization of prompts and weights without manual prompt engineering. Datasette Agent is an LLM-powered assistant for exploring and querying data in Datasette. Claude Code is an AI coding agent that can read codebases and execute tasks autonomously.

<details><summary>References</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/ dspy : DSPy : The framework for ...</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help ...</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#LLM`, `#Datasette Agent`, `#AI research`

---

<a id="item-16"></a>
## [Google Gemini Omni Flash Tops Video Arena](https://x.com/Designarena/status/2072759122366509130) ⭐️ 7.0/10

Google DeepMind's Gemini Omni Flash video generation model achieved a score of 1404 points on the Video Arena blind test leaderboard, surpassing ByteDance's Seedance 2.0 Mini by 101 points. This marks a significant advancement in AI video generation, with Google reclaiming the top spot from ByteDance. The wide margin indicates a notable leap in quality, potentially reshaping the competitive landscape for video generation models. Video Arena ranks models based on blind user preference votes, and Google's overall video model ranking improved by 7 positions compared to the Veo series era. Seedance 2.0 Mini had previously held the top spot with 1303 points.

telegram · zaihuapd · Jul 3, 05:51

**Background**: Video Arena is a community-driven benchmarking platform created by UC Berkeley researchers that evaluates AI video models based on real human preferences. Google's Gemini Omni Flash is a native multimodal video generation model announced at Google I/O 2026, trained on Google's TPUs. ByteDance's Seedance 2.0 Mini is a faster, cost-efficient variant of the Seedance 2.0 model designed for short-form video drafting.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bracai.eu/post/video-arena">Best AI video models in 2026 (ranked by real users) - Bracai</a></li>
<li><a href="https://deepmind.google/models/model-cards/gemini-omni-flash/">Gemini Omni Flash - Model Card — Google DeepMind</a></li>
<li><a href="https://www.seedance20.com/">Generate Cinematic Videos with Seedance 2 . 0 Model | Seedio</a></li>

</ul>
</details>

**Tags**: `#AI`, `#video generation`, `#Google DeepMind`, `#benchmark`

---

<a id="item-17"></a>
## [Claude Fable 5 Relaunch Disappoints with Nerfed Performance](https://www.bleepingcomputer.com/news/artificial-intelligence/claude-fable-relaunch-disappoints-users-with-nerfed-performance/) ⭐️ 7.0/10

Anthropic's flagship model Claude Fable 5 has relaunched after US export controls were lifted, but users report significantly reduced performance due to overly aggressive safety filters that frequently downgrade the model to Opus 4.8 when processing low-level code or security-related keywords. This backlash highlights the tension between AI safety measures and developer productivity, potentially eroding trust in Anthropic's flagship model and impacting adoption among professional developers who rely on Claude for complex coding tasks. Until July 7, Pro and Max subscribers can only use 50% of their weekly quota for Fable 5; after that date, the model will no longer be included in subscriptions and will be billed per usage. The API and enterprise pay-per-use plans still offer full access to Fable 5 without safety downgrades.

telegram · zaihuapd · Jul 3, 07:20

**Background**: Claude Fable 5 is a Mythos-class model from Anthropic, designed for long-running, complex tasks with built-in safeguards. Anthropic is known for its focus on AI safety, but this relaunch shows that excessive safety filters can hinder legitimate use cases, especially in software development where security-related terms are common.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/news/claude-fable-5-mythos-5">Claude Fable 5 and Claude Mythos 5 \ Anthropic</a></li>
<li><a href="https://aws.amazon.com/blogs/aws/anthropic-claude-fable-5-on-aws-mythos-class-capabilities-with-built-in-safeguards-now-available/">Anthropic Claude Fable 5 on AWS: Mythos-class capabilities with built-in safeguards now available | Amazon Web Services</a></li>

</ul>
</details>

**Discussion**: Developer forums and social media are filled with complaints about the safety overreach, with many calling the model 'unusable' for serious coding work. Some users suggest that Anthropic should provide a toggle to adjust safety levels, while others express frustration that the API version works fine but the subscription version is crippled.

**Tags**: `#AI`, `#Claude`, `#Anthropic`, `#safety`, `#developer experience`

---

<a id="item-18"></a>
## [China Proposes Account Deactivation After 6 Months of Inactivity](https://mp.weixin.qq.com/s/TfYZaC8ULPvu9JeTqYGkKg) ⭐️ 7.0/10

China's Cyberspace Administration released a revised draft of the Internet Information Service Management Measures on July 3, 2025, proposing that platforms may deactivate accounts inactive for over six months and must support unbinding accounts when phone numbers change. The draft also mandates labeling of AI-generated content, bans manipulation of rankings and fake trends, and requires large platforms to handle complaints within 24 hours. This regulation significantly impacts user privacy and platform accountability in China, potentially affecting billions of internet users and all major online platforms. It addresses growing concerns over dormant accounts, AI transparency, and online manipulation, setting a precedent for internet governance globally. The draft is open for public comment until August 2, 2026, and follows a previous version released in January 2025. It also prohibits platforms from forcing users to use AI services and requires an option to turn off personalized recommendations.

telegram · zaihuapd · Jul 3, 11:29

**Background**: The Internet Information Service Management Measures are a foundational regulation governing online content and services in China. The new draft builds on existing rules and aligns with the AI-Generated Synthetic Content Labeling Measures that took effect on September 1, 2025, which require explicit and implicit labeling of AI-generated content.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cac.gov.cn/2025-09/04/c_1758702660213189.htm">专家解读｜从制度破冰到体系完善AI生成内容标识打造可信网络空间_中央网络安全和信息化委员会办公室</a></li>
<li><a href="http://www.news.cn/legal/20250901/a12108b0b10249e5bae4435269e40c91/c.html">9月1日起 AI生成合成内容必须添加标识-新华网</a></li>
<li><a href="https://dun.163.com/news/p/795bd25960d1422c9d40871f05420446">dun.163.com/news/p/795bd25960d1422c9d40871f05420446</a></li>

</ul>
</details>

**Tags**: `#internet regulation`, `#privacy`, `#AI`, `#China`, `#policy`

---

<a id="item-19"></a>
## [Huawei Mate 80 Pro gaming efficiency beats Snapdragon 8 Gen3](https://www.bilibili.com/video/BV1F7T46wEyT) ⭐️ 7.0/10

Geekerwan's review shows that the Huawei Mate 80 Pro series, powered by the Kirin 9030 chipset, achieves better gaming energy efficiency than the Snapdragon 8 Gen3, thanks to native HarmonyOS optimizations. This demonstrates that software-hardware co-optimization can overcome raw performance gaps, potentially reshaping competition in mobile chipsets and OS ecosystems. The Kirin 9030 Pro features a 9-core, 14-thread CPU and a 6-core Maleoon 935 GPU with about 15 billion transistors. In Genshin Impact at 60fps, the Mate 80 Pro Max consumes only 4.9W, outperforming the Snapdragon 8 Gen3 in energy efficiency.

telegram · zaihuapd · Jul 3, 13:27

**Background**: Huawei's Kirin chipsets have faced restrictions due to US sanctions, limiting their access to advanced manufacturing. HarmonyOS is Huawei's proprietary operating system designed to integrate seamlessly with its hardware. The Mate 80 Pro series represents Huawei's latest flagship, emphasizing native app optimizations and system-level efficiency.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ithome.com/0/972/456.htm">华为 Mate 80 Pro 性能解禁：麒麟 9030 Pro GPU 相比 9020 提升 76...</a></li>

</ul>
</details>

**Tags**: `#Huawei`, `#chipset`, `#gaming`, `#energy efficiency`, `#HarmonyOS`

---