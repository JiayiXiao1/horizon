---
layout: default
title: "Horizon Summary: 2026-06-19 (EN)"
date: 2026-06-19
lang: en
---

> From 39 items, 18 important content pieces were selected

---

1. [10k GitHub Repos Distribute Trojan Malware](#item-1) ⭐️ 9.0/10
2. [Noam Shazeer Leaves Google for OpenAI](#item-2) ⭐️ 9.0/10
3. [GLM-5.2: Leading Open-Weights LLM Released](#item-3) ⭐️ 9.0/10
4. [Drug Repurposing by Hospitals and Universities Cuts Costs 90%](#item-4) ⭐️ 8.0/10
5. [Forced Consent Complaint Leads to €1.8M GDPR Fine for Elkjop](#item-5) ⭐️ 8.0/10
6. [New Tool Checks If Your Data Is in LLM Training Sets](#item-6) ⭐️ 8.0/10
7. [Modos Color E-Paper Monitor Hits 60Hz](#item-7) ⭐️ 8.0/10
8. [Charity Majors: AI Demands More Engineering Discipline](#item-8) ⭐️ 8.0/10
9. [Apple and Intel Reach Preliminary Chip Manufacturing Deal](#item-9) ⭐️ 8.0/10
10. [China Seeks Comments on Decentralized Digital ID Rules](#item-10) ⭐️ 8.0/10
11. [Ubiquiti Launches Enterprise NAS Built on ZFS](#item-11) ⭐️ 7.0/10
12. [Cornell CS 6120 Advanced Compilers Self-Guided Course](#item-12) ⭐️ 7.0/10
13. [Swiss Parliament Lifts Ban on New Nuclear Plants](#item-13) ⭐️ 7.0/10
14. [W Social: European Digital Sovereignty or Political Theater?](#item-14) ⭐️ 7.0/10
15. [Datasette Apps: Sandboxed HTML/JS Apps with SQL Queries](#item-15) ⭐️ 7.0/10
16. [Infant Diapers Found to Contain Reproductive Toxicant Formamide](#item-16) ⭐️ 7.0/10
17. [Xiaomi Open-Sources Miloco 2.0 Smart Home Solution](#item-17) ⭐️ 7.0/10
18. [Huawei Sets Wi-Fi 7 Patent Fee at $0.50 per Device](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [10k GitHub Repos Distribute Trojan Malware](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

An analysis found over 10,000 GitHub repositories distributing Trojan malware through cloned repos and automated commit updates, evading detection for months. This widespread supply chain attack threatens the open-source ecosystem, potentially infecting developers and users who unknowingly clone or depend on these repositories. Each repository contains a zip archive with a Trojan; attackers clone legitimate repos, inject malware, and push frequent commits to stay visible in search results.

hackernews · theorchid · Jun 18, 11:45 · [Discussion](https://news.ycombinator.com/item?id=48583928)

**Background**: GitHub is a popular platform for hosting open-source code, but its collaborative nature can be exploited. Attackers often clone legitimate projects, add malware, and re-upload them under similar names to trick users into downloading infected code.

<details><summary>References</summary>
<ul>
<li><a href="https://orchidfiles.com/github-repositories-distributing-malware/">How I found 10,000 GitHub repositories distributing Trojan malware</a></li>
<li><a href="https://checkmarx.com/blog/github-repos-used-for-distributing-malware/">GitHub Repos Used for Distributing Malware</a></li>
<li><a href="https://gbhackers.com/109-fake-github-repos/">109 Fake GitHub Repos Spread SmartLoader, StealC Malware</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the attack targets automated agents rather than humans, and some reported personal experiences of their names being used on fake repos. Others suggested that frequent commits help repos appear in 'last updated' searches.

**Tags**: `#security`, `#malware`, `#github`, `#supply chain attack`, `#open source`

---

<a id="item-2"></a>
## [Noam Shazeer Leaves Google for OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer, co-author of the seminal 'Attention Is All You Need' paper and former Gemini co-lead at Google, has announced he is leaving Google to join OpenAI. This move signals a major talent shift in the AI industry, as Shazeer is a key figure behind the transformer architecture that underpins modern large language models. His departure from Google to a direct competitor could accelerate OpenAI's research and intensify the rivalry between the two companies. Shazeer originally left Google in 2021 to co-found Character.AI, then returned in 2024 via a licensing deal reportedly worth $2.7 billion, becoming Gemini co-lead. Now, just over a year later, he is leaving again for OpenAI.

hackernews · lukasgross · Jun 18, 00:26 · [Discussion](https://news.ycombinator.com/item?id=48578913)

**Background**: Noam Shazeer is a long-time Google researcher who joined the company in 2000. He was one of eight co-authors of the 2017 paper 'Attention Is All You Need', which introduced the Transformer architecture—the foundation of most modern large language models like GPT-4 and Gemini. He co-led Google's Gemini model development before this move.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noam_Shazeer">Noam Shazeer</a></li>
<li><a href="https://www.reuters.com/technology/googles-gemini-co-lead-noam-shazeer-join-openai-2026-06-18/">Google Gemini co-lead Noam Shazeer to join IPO-bound OpenAI | Reuters</a></li>
<li><a href="https://en.wikipedia.org/wiki/Attention_Is_All_You_Need">Attention Is All You Need - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community is highly engaged, with many highlighting Shazeer's legendary status at Google and his critical role in the transformer paper. Some express surprise at his quick departure after returning to Google, while others view it as a natural move given OpenAI's leading position in the AI race.

**Tags**: `#AI`, `#OpenAI`, `#Google`, `#transformers`, `#industry news`

---

<a id="item-3"></a>
## [GLM-5.2: Leading Open-Weights LLM Released](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai released GLM-5.2, a 753B-parameter open-weights LLM under MIT license, with a 1M token context window and top benchmark performance. GLM-5.2 is the leading open-weights model on the Artificial Analysis Intelligence Index, surpassing competitors like MiniMax-M3 and DeepSeek V4 Pro, and ranks 2nd on the Code Arena WebDev leaderboard, making it a significant advancement in open-source AI. The model uses Mixture of Experts with 40 active parameters out of 753B total, and has a 1.51TB size. It is text-only and token-hungry, using 43k output tokens per task compared to 24k for MiniMax-M3.

rss · Simon Willison · Jun 17, 23:58

**Background**: Open-weights LLMs make trained parameters publicly available, allowing researchers and developers to use and modify them. Mixture of Experts (MoE) architectures activate only a subset of parameters per token, improving efficiency. A 1M token context window enables processing of very long documents or conversations.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical...</a></li>

</ul>
</details>

**Discussion**: The community buzz is strong, with independent benchmark validation confirming GLM-5.2's leading performance. However, some note its higher token usage and the lack of image input for a model that excels at frontend coding tasks.

**Tags**: `#LLM`, `#open-weights`, `#AI`, `#GLM-5.2`, `#benchmark`

---

<a id="item-4"></a>
## [Drug Repurposing by Hospitals and Universities Cuts Costs 90%](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

Hospitals and universities are repurposing existing drugs through late-stage trials at costs up to 90% lower than pharmaceutical industry trials, offering affordable treatments for conditions like blindness and rare diseases. This approach could dramatically reduce healthcare costs and expand access to treatments, especially for rare diseases where pharmaceutical companies have little incentive to develop new drugs. The cost savings come from using drugs already approved for other indications, bypassing early-stage development. However, there is no regulatory pathway to extend use without manufacturer consent or becoming a manufacturer oneself.

hackernews · giuliomagnifico · Jun 18, 10:33 · [Discussion](https://news.ycombinator.com/item?id=48583386)

**Background**: Drug repurposing (or repositioning) involves investigating existing drugs for new therapeutic purposes. It is a cost-effective strategy because safety data already exists, reducing the time and expense of clinical trials. The approach gained attention during the COVID-19 pandemic when repurposed drugs were used under emergency authorization.

<details><summary>References</summary>
<ul>
<li><a href="https://www.news-medical.net/news/20260616/Universities-and-hospitals-repurpose-existing-drugs-at-significantly-lower-costs.aspx">Universities and hospitals repurpose existing drugs at significantly...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9336118/">Drug repurposing : a systematic review on root causes, barriers and...</a></li>

</ul>
</details>

**Discussion**: Commenters shared personal experiences, such as using Avastin (bevacizumab) for macular degeneration at $50/dose versus Lucentis at $1,500/dose, and highlighted the broken incentives in the US healthcare system, exemplified by esketamine (Spravato) being patented despite being less effective than generic ketamine. Some noted regulatory barriers to repurposing without manufacturer involvement.

**Tags**: `#drug repurposing`, `#healthcare`, `#cost reduction`, `#pharmaceuticals`, `#innovation`

---

<a id="item-5"></a>
## [Forced Consent Complaint Leads to €1.8M GDPR Fine for Elkjop](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

A privacy advocate's complaint about forced consent for marketing led to a €1.8 million fine against Norwegian retailer Elkjop under GDPR, five years after the initial complaint. This case demonstrates that individual complaints can lead to significant GDPR enforcement, empowering consumers to challenge unlawful data practices and setting a precedent for similar cases across Europe. The fine was imposed by the Norwegian Data Protection Authority (Datatilsynet) for requiring customers to join a loyalty club to receive marketing, which constitutes forced consent. The complainant documented the violation and pursued the case for five years.

hackernews · speckx · Jun 18, 18:31 · [Discussion](https://news.ycombinator.com/item?id=48589501)

**Background**: Under GDPR, consent must be freely given, specific, informed, and unambiguous. Forced consent, where a service is conditional on agreeing to data processing, is generally unlawful. The case highlights the role of strategic litigation by individuals in enforcing privacy rights.

**Discussion**: Commenters praised the complainant's persistence and noted the importance of individual enforcement. Some highlighted the absurdity of companies ignoring clear legal violations, while others provided links to the official decision and translations.

**Tags**: `#GDPR`, `#privacy`, `#data protection`, `#enforcement`, `#consent`

---

<a id="item-6"></a>
## [New Tool Checks If Your Data Is in LLM Training Sets](https://www.intheweights.com/) ⭐️ 8.0/10

A new website, intheweights.com, queries multiple large language models in parallel to determine how strongly they recognize a given username, revealing whether personal data appears in their training sets. This tool highlights the growing privacy concern that personal online content may be embedded in LLM training data without consent, and it gives users a way to detect their digital footprint in AI models. The tool queries frontier and small models in parallel, clusters responses, and outputs a recognition score; it is non-deterministic, and adding more keywords about yourself can increase the score.

hackernews · turtlesoup · Jun 18, 20:49 · [Discussion](https://news.ycombinator.com/item?id=48591348)

**Background**: Large language models (LLMs) are trained on vast amounts of text data scraped from the internet, which often includes personal information. The 'weights' of a neural network are the parameters learned during training that encode patterns from the data. This tool probes whether specific usernames are memorized in those weights, indicating the presence of associated data in the training set.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/the-role-of-weights-and-bias-in-neural-networks/">Weights and Bias in Neural Networks - GeeksforGeeks</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed feelings: some found it unsettling that their old writings are in training data, while others were amused by the recognition results. There was also technical discussion about the tool's non-deterministic nature and how adding keywords boosts scores.

**Tags**: `#LLM`, `#privacy`, `#data recognition`, `#AI ethics`, `#web tool`

---

<a id="item-7"></a>
## [Modos Color E-Paper Monitor Hits 60Hz](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

Modos, a two-person startup, is developing the Modos Flow, a 13.3-inch color e-paper monitor with a native resolution of 3200x2400 and a 60Hz refresh rate, enabled by a new display controller. This pushes e-paper technology closer to mainstream use, offering a high-resolution color display with a refresh rate suitable for general computing, potentially reducing eye strain and power consumption compared to traditional LCDs. The Modos Flow features touch input and sub-100ms latency, and the company is currently fundraising on Crowd Supply. Previous e-paper monitors have been limited to lower refresh rates or grayscale.

hackernews · Vinnl · Jun 18, 11:41 · [Discussion](https://news.ycombinator.com/item?id=48583897)

**Background**: E-paper displays, like those using E Ink technology, reflect ambient light and consume power only when changing the image, making them ideal for reading and low-power applications. However, traditional e-paper has been limited by slow refresh rates (typically under 30Hz) and lack of color, hindering its use for video or interactive tasks. Recent advances, such as Dasung's 60Hz grayscale panel, have begun to address these limitations.

<details><summary>References</summary>
<ul>
<li><a href="https://spectrum.ieee.org/modos-e-paper-monitor">Modos Color Monitor Pushes E-Paper Displays Further - IEEE Spectrum</a></li>
<li><a href="https://www.tomshardware.com/monitors/portable-monitors/hands-on-with-modos-tech-13-3-inch-e-paper-monitors">Hands-on with Modos Tech 13.3-inch e-paper monitors — we tried the current Dev Kit model and the next-gen Modos Flow touch | Tom's Hardware</a></li>
<li><a href="https://www.crowdsupply.com/modos-tech/modos-paper-monitor">Modos Paper Monitor | Crowd Supply</a></li>

</ul>
</details>

**Discussion**: Commenters are excited about the development, noting it's one of the most promising e-paper advances in years. Some express concern about panel longevity at higher refresh rates, while others compare it favorably to RLCD and other alternative display technologies.

**Tags**: `#e-paper`, `#display technology`, `#hardware`, `#startup`

---

<a id="item-8"></a>
## [Charity Majors: AI Demands More Engineering Discipline](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors argues that AI has made code generation cheap and disposable, demanding more engineering discipline, not less. This insight challenges the common assumption that AI reduces the need for rigorous engineering practices, highlighting a paradigm shift where code becomes disposable and engineering discipline becomes more critical. Majors notes that in 2025, the economics of code production were upended: code went from being hard and expensive to generate to being effectively free and instant, making it disposable and regenerable.

rss · Simon Willison · Jun 17, 17:12

**Background**: Traditionally, writing code was labor-intensive and costly, so code was carefully curated and reused. With generative AI, code can be generated quickly and cheaply, but this new ease of creation requires even more discipline in testing, reviewing, and maintaining code quality.

**Tags**: `#AI-assisted programming`, `#software engineering`, `#generative AI`, `#engineering discipline`

---

<a id="item-9"></a>
## [Apple and Intel Reach Preliminary Chip Manufacturing Deal](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

Apple has reportedly reached a preliminary agreement with Intel for Intel to manufacture some chips for Apple devices, potentially reducing Apple's reliance on TSMC. This deal could reshape the semiconductor supply chain by bringing a major customer to Intel's foundry business, while giving Apple more leverage and diversification in chip production. The negotiations lasted over a year and were finalized in recent months, with the U.S. government playing a significant role in pushing the deal forward. It is unclear which specific Apple products (iPhone, iPad, or Mac) will use Intel-made chips.

telegram · zaihuapd · Jun 18, 09:19

**Background**: Apple has historically relied on TSMC and Samsung for chip manufacturing, as it designs its own chips but does not operate fabrication plants. Intel has been expanding its foundry services, aiming to compete with TSMC and Samsung, and has already secured partnerships with Nvidia and SpaceX.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Apple晶片">Apple晶片 - 维基百科，自由的百科全书</a></li>
<li><a href="https://letschuhai.com/yingteerjiangtou200yimeiyuanxinjianjingyuanchangkaizhanjingyuandaigongyewu">英特尔将投200亿美元新建晶圆厂，开展晶圆 代 工 业 务 | 36氪出海</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Intel`, `#chip manufacturing`, `#semiconductors`, `#supply chain`

---

<a id="item-10"></a>
## [China Seeks Comments on Decentralized Digital ID Rules](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

On June 18, 2026, China's Cyberspace Administration released a draft regulation titled 'Provisions on Promoting Interoperable Decentralized Digital Identity Applications' for public comment until July 18. The regulation defines decentralized digital identities based on blockchain, supporting user-controlled identity management via identifiers, keys, verifiable credentials, and verifiable claims. This regulation could establish a national standard for decentralized digital identity interoperability in China, potentially influencing global blockchain identity standards. It aims to enable cross-platform identity verification across finance, transportation, customs, taxation, and digital currency sectors, impacting both domestic and international entities. The regulation proposes building a national identity chain (身份链) based on the national blockchain network, supporting voluntary registration for individuals, institutions, and industrial devices. Relevant entities must fulfill data security and personal information protection obligations.

telegram · zaihuapd · Jun 19, 01:39

**Background**: Decentralized digital identity (DID) is a blockchain-based identity system that gives users control over their own identity data, unlike traditional centralized systems. It uses cryptographic techniques to enable secure, verifiable claims without relying on a central authority. The W3C has been developing DID standards, and China's move aligns with global trends while tailoring to its regulatory environment.

<details><summary>References</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/689030887">【深度】DID分布式数字身份(1/5)--什么是DID - 知乎</a></li>
<li><a href="https://blog.csdn.net/wangzelong046/article/details/135659699">数字身份是啥？_分布式数字身份-CSDN博客</a></li>

</ul>
</details>

**Tags**: `#blockchain`, `#digital identity`, `#regulation`, `#China`, `#interoperability`

---

<a id="item-11"></a>
## [Ubiquiti Launches Enterprise NAS Built on ZFS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 7.0/10

Ubiquiti has announced a new enterprise NAS appliance built on the ZFS file system, featuring a 3U rack-mount chassis with sixteen SATA bays, dual 25 Gbps SFP28 ports, and redundant power supplies. This marks Ubiquiti's entry into the enterprise NAS market, offering an integrated solution for users already invested in the UniFi ecosystem, with the data integrity and advanced features of ZFS. The NAS is priced at $3,999 and supports M.2 NVMe caching, but community members question whether spinning hard drives can saturate the 25 Gbps network links, and express concerns about Ubiquiti's software quality and past security incidents.

hackernews · ksec · Jun 18, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48585866)

**Background**: ZFS is an advanced file system and volume manager known for data integrity, snapshots, and efficient replication. Ubiquiti is best known for its networking equipment and UniFi software ecosystem, and this NAS aims to provide a tightly integrated storage solution for enterprise customers.

<details><summary>References</summary>
<ul>
<li><a href="https://store.ui.com/us/en/products/enas">Enterprise NAS - Ubiquiti Store</a></li>
<li><a href="https://news.ycombinator.com/item?id=48585866">Ubiquiti : Enterprise NAS , Built on ZFS | Hacker News</a></li>

</ul>
</details>

**Discussion**: The Hacker News community shows mixed sentiment: some praise Ubiquiti's no-subscription model and ZFS adoption, while others criticize past software quality issues and question the hardware's ability to fully utilize high-speed networking.

**Tags**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#enterprise storage`, `#hardware`

---

<a id="item-12"></a>
## [Cornell CS 6120 Advanced Compilers Self-Guided Course](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 7.0/10

Cornell University's CS 6120 advanced compilers course is now available as a free, self-guided online resource, covering topics from basic optimizations to dynamic compilation. This course provides a high-quality, accessible resource for compiler enthusiasts and students worldwide, filling a gap in advanced compiler education. The course includes lecture videos, reading materials, and assignments, but some community members note that topics like trace compilation may be outdated, and the content may overlap with introductory compiler courses.

hackernews · ibobev · Jun 18, 11:04 · [Discussion](https://news.ycombinator.com/item?id=48583606)

**Background**: Compiler design is a core area of computer science, covering how source code is translated into executable programs. Advanced compilers courses typically explore optimization techniques, code generation, and runtime systems beyond introductory material.

**Discussion**: Community comments include praise for the course's availability, but also critical feedback: some argue that trace compilation is a dead end, and others question whether the topics are truly advanced. Comparisons to other resources like Nora Sandler's book are also raised.

**Tags**: `#compilers`, `#online course`, `#programming languages`, `#computer science education`

---

<a id="item-13"></a>
## [Swiss Parliament Lifts Ban on New Nuclear Plants](https://www.bluewin.ch/en/news/switzerland/parliament-lifts-ban-on-new-nuclear-power-plants-3257535.html) ⭐️ 7.0/10

The Swiss parliament has voted to lift a ban on building new nuclear power plants, reversing a 2017 referendum decision to phase out nuclear energy. The change still requires approval in a public referendum. This policy shift could reshape Switzerland's energy strategy, potentially enabling new nuclear projects to address the country's summer-winter energy imbalance. It also signals a broader European reconsideration of nuclear power amid energy security concerns. The ban was originally enacted after the 2011 Fukushima disaster, leading to a 2017 referendum that prohibited new nuclear plants. The new decision is expected to face strong opposition from left-leaning and green parties, and the final outcome depends on a future referendum.

hackernews · leonidasrup · Jun 18, 14:17 · [Discussion](https://news.ycombinator.com/item?id=48585746)

**Background**: Switzerland currently has four nuclear reactors that provide about 30% of its electricity. The country relies heavily on hydropower, but faces seasonal energy shortages in winter when hydro output drops. Nuclear power is a low-carbon energy source, but concerns about safety and waste disposal remain.

**Discussion**: Commenters expressed mixed views: some highlighted nuclear's low death rate per TWh and energy security benefits, while others questioned the cleanliness of uranium mining and waste disposal. There was skepticism about whether the referendum would pass given political divisions.

**Tags**: `#nuclear energy`, `#Switzerland`, `#energy policy`, `#technology`, `#politics`

---

<a id="item-14"></a>
## [W Social: European Digital Sovereignty or Political Theater?](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 7.0/10

A blog post by Elena Rossini critiques W Social, a European social media platform, as a performative project lacking transparency, contrasting it with the open and non-profit alternative Eurosky. This critique highlights the gap between political rhetoric on European digital sovereignty and actual implementation, questioning whether W Social serves public interest or political agendas. W Social is an LLC with profit motives, and its founder has a background in finance. In contrast, Eurosky is built on AT Protocol by a non-profit foundation with full transparency.

hackernews · nemoniac · Jun 18, 12:46 · [Discussion](https://news.ycombinator.com/item?id=48584497)

**Background**: European digital sovereignty refers to the EU's ambition to reduce dependence on non-European tech giants by developing its own digital infrastructure. W Social and Eurosky are two attempts at creating a European social media platform, but they differ fundamentally in governance and transparency.

<details><summary>References</summary>
<ul>
<li><a href="https://eurosky.tech/">Eurosky - Building a thriving open social web for Europe</a></li>

</ul>
</details>

**Discussion**: Commenters express skepticism about W Social's authenticity, with some calling it 'Truth Social with a European accent' and noting its lack of transparency compared to Eurosky. Others question its profit motives and political backing.

**Tags**: `#digital sovereignty`, `#social media`, `#European politics`, `#tech criticism`

---

<a id="item-15"></a>
## [Datasette Apps: Sandboxed HTML/JS Apps with SQL Queries](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

Simon Willison launched the datasette-apps plugin, which allows hosting sandboxed HTML+JavaScript applications inside Datasette that can execute read-only and configured write SQL queries against the underlying data. This plugin transforms Datasette from a data exploration tool into a platform for building custom, interactive web applications directly on top of SQLite databases, expanding its use cases significantly. Apps run in a sandboxed iframe with `allow-scripts allow-forms` and an injected CSP header that blocks outbound HTTP requests, preventing data exfiltration. The plugin also registers permissions for creating, viewing, editing, and deleting apps.

rss · Simon Willison · Jun 18, 23:58

**Background**: Datasette is an open-source tool for exploring and publishing SQLite databases, with a plugin system that extends its functionality. The datasette-apps plugin originated from an attempt to build a Claude Artifacts-like mechanism for Datasette Agent, but was generalized into a standalone feature.

<details><summary>References</summary>
<ul>
<li><a href="https://pypi.org/project/datasette-apps/">Create apps that live inside Datasette</a></li>
<li><a href="https://datasette.io/tools/datasette-app">datasette - app - a tool for Datasette</a></li>
<li><a href="https://architecturenotes.co/p/datasette-simon-willison">Arc Note: Datasette - Simon Willison - by Mahdi Yusuf</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#plugin`, `#sql`, `#web-applications`, `#sandbox`

---

<a id="item-16"></a>
## [Infant Diapers Found to Contain Reproductive Toxicant Formamide](https://www.sohu.com/a/1038121771_122014422) ⭐️ 7.0/10

A professional testing agency commissioned by the Economic Information Daily detected the reproductive toxicant formamide in several brands of infant diapers, including HUGGIES, Bebaby, and Babycare. The substance was also found in the blood and urine of some infants, and a reporter's blood concentration nearly doubled after wearing one diaper overnight. This discovery exposes a critical regulatory gap in China's national standards for infant diapers, which currently do not limit formamide despite its known reproductive toxicity. Given that infants are especially vulnerable to toxic accumulation, the finding poses a serious public health risk and has sparked urgent calls for standard revision. Formamide is classified as a 1B reproductive toxicant under EU regulations and is banned in cosmetics in China, but the current national standard GB/T 28004.1-2021 for infant diapers does not include testing for formamide. The substance can be absorbed through the skin and accumulates in the body, with infants being at higher risk due to their immature organs and weaker metabolic capacity.

telegram · zaihuapd · Jun 18, 07:09

**Background**: Formamide is a chemical used in some industrial processes and can be a byproduct of certain materials. It has been previously found in baby crawling mats and other children's products, raising ongoing concerns about infant product safety. In China, the national standard for infant diapers (GB/T 28004.1-2021) currently lacks any limit or testing requirement for formamide, leaving a regulatory gap that industry insiders and experts are urging to be closed.

<details><summary>References</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260618/herald/ec6cf982d003c7201f79a2a2ea409195.html">从爬行地垫到纸尿裤， 甲 酰 胺 反复“现身”拷问 婴 童用品质量安全 - 21...</a></li>
<li><a href="https://www.bjnews.com.cn/detail/1781760045169406.html">多款婴儿 纸 尿 裤 检 出 甲 酰 胺 ？ “好奇”等品牌回应， 国 标 尚无限值 — 新京报</a></li>
<li><a href="https://news.cnr.cn/rebang/20260618/t20260618_527666495.shtml">专业检测机构检出有毒物质 多款纸尿裤被指侵 害 婴 幼 儿 健康_央广网</a></li>

</ul>
</details>

**Tags**: `#public health`, `#consumer safety`, `#regulatory gap`, `#infant products`, `#toxicology`

---

<a id="item-17"></a>
## [Xiaomi Open-Sources Miloco 2.0 Smart Home Solution](https://github.com/XiaoMi/xiaomi-miloco) ⭐️ 7.0/10

Xiaomi has released Miloco 2.0, an open-source smart home solution that uses camera input and the MiMo large language model to proactively observe, reason, and control devices throughout the home. This release marks a major step in integrating large language models into practical smart home systems, potentially enabling more intuitive and proactive home automation. It also lowers the barrier for developers to build AI-powered smart home applications. Miloco 2.0 runs as an OpenClaw plugin, requires macOS or Linux (Windows via WSL), at least 4 GB RAM and 256 GB storage, and relies on cloud-based MiMo API, incurring ongoing costs. The project is limited to non-commercial use.

telegram · zaihuapd · Jun 18, 12:23

**Background**: Miloco is Xiaomi's open-source smart home framework that leverages the MiMo large language model, a lightweight, MIT-licensed LLM family designed for agents. OpenClaw is an open-source AI agent framework that allows plugins to extend its capabilities. By combining these, Miloco 2.0 can process camera input to understand home context and control IoT devices proactively.

<details><summary>References</summary>
<ul>
<li><a href="https://hyperosinsider.com/xiaomi-miloco-2-0-released-before-hyperos-4-smart-ai-open-source-solution/">Xiaomi Miloco 2 . 0 Released Before HyperOS... - HyperOS Insider</a></li>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi_MiMo">Xiaomi MiMo - Wikipedia</a></li>
<li><a href="https://open-claw.bot/docs/tools/plugins/">OpenClaw Plugins : Extend Your AI Agent | OpenClaw</a></li>

</ul>
</details>

**Tags**: `#smart home`, `#open source`, `#LLM`, `#Xiaomi`, `#IoT`

---

<a id="item-18"></a>
## [Huawei Sets Wi-Fi 7 Patent Fee at $0.50 per Device](https://36kr.com/newsflashes/3858656955847687) ⭐️ 7.0/10

Huawei announced a Wi-Fi 7 patent licensing rate of $0.50 per device, available through bilateral agreements or patent pools under FRAND principles. This rate sets a precedent for Wi-Fi 7 licensing, potentially influencing costs for device manufacturers and shaping industry standards. As of end 2024, over 1.2 billion consumer electronic devices have received Huawei's Wi-Fi patent licenses. The fee applies to Wi-Fi 7 devices specifically.

telegram · zaihuapd · Jun 19, 00:09

**Background**: Wi-Fi 7 is the next-generation wireless standard offering higher speeds and lower latency. FRAND (Fair, Reasonable, and Non-Discriminatory) principles ensure patent holders license standard-essential patents on fair terms. Patent pools provide a one-stop licensing solution with lower transaction costs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/6/ipr-license-wifi7">Huawei Announces Wi - Fi 7 Patent Licensing Rates... - Huawei</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reasonable_and_non-discriminatory_licensing">Reasonable and non-discriminatory licensing - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Wi-Fi 7`, `#patent licensing`, `#Huawei`, `#FRAND`

---