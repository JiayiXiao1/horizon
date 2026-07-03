---
layout: default
title: "Horizon Summary: 2026-07-03 (EN)"
date: 2026-07-03
lang: en
---

> From 31 items, 21 important content pieces were selected

---

1. [Virginia Bans Sale of Geolocation Data](#item-1) ⭐️ 8.0/10
2. [Podman v6.0.0 Released with Major Networking Overhaul](#item-2) ⭐️ 8.0/10
3. [Immich 3.0 Sparks Encryption Debate](#item-3) ⭐️ 8.0/10
4. [Understand to Participate: Key to Avoiding Cognitive Debt](#item-4) ⭐️ 8.0/10
5. [Cloudflare to Block Mixed-Use AI Crawlers by Default from September](#item-5) ⭐️ 8.0/10
6. [OpenAI Proposes 5% US Government Stake in AI Giants](#item-6) ⭐️ 8.0/10
7. [Citibank Bans GPT-5.5 as AI Costs Surge for Enterprises](#item-7) ⭐️ 8.0/10
8. [PS3 Store to Close in 2027, Archivists Race to Save Games](#item-8) ⭐️ 8.0/10
9. [Linux 6.9 LUKS Suspend Fails to Wipe Encryption Keys](#item-9) ⭐️ 7.0/10
10. [PeerTube: Decentralized Video Platform Gains Traction](#item-10) ⭐️ 7.0/10
11. [How to Ask Strangers for Help Effectively](#item-11) ⭐️ 7.0/10
12. [Using DSPy to Evaluate and Improve Datasette Agent's SQL Prompts](#item-12) ⭐️ 7.0/10
13. [ChatGPT Doubles Weekly Users to 200 Million in Under a Year](#item-13) ⭐️ 7.0/10
14. [Yageo to Hike Capacitor Prices ~50% from July 1](#item-14) ⭐️ 7.0/10
15. [Sony to End Physical Game Discs for New PlayStation Titles by 2028](#item-15) ⭐️ 7.0/10
16. [Apple Reveals iCloud Anonymous Email User to FBI](#item-16) ⭐️ 7.0/10
17. [Meta Plans to Sell Surplus AI Compute, Enter Cloud Market](#item-17) ⭐️ 7.0/10
18. [Android 17 Drastically Limits Password Attempts to 20](#item-18) ⭐️ 7.0/10
19. [CSRC Approves Unitree Technology's STAR Market IPO Registration](#item-19) ⭐️ 7.0/10
20. [Anthropic in Talks with Samsung for Custom AI Chip](#item-20) ⭐️ 7.0/10
21. [Kernel.org Mirror Error Empties /pub, Data Intact](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Virginia Bans Sale of Geolocation Data](https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data) ⭐️ 8.0/10

On April 13, 2026, Virginia Governor Abigail Spanberger signed SB 388 into law, amending the Virginia Consumer Data Protection Act to prohibit the sale of precise geolocation data, effective July 1, 2026. This makes Virginia the third state to ban the sale of geolocation data, reflecting a growing trend in privacy legislation that could pressure other states and the federal government to act, and will impact data brokers and tech companies that rely on location data for advertising and analytics. The ban applies to precise geolocation data within a 1,750-foot radius, a buffer large enough to prevent pinpointing consumers' homes, workplaces, or places of worship. The law amends the VCDPA and takes effect on July 1, 2026.

hackernews · toomuchtodo · Jul 2, 21:03 · [Discussion](https://news.ycombinator.com/item?id=48767347)

**Background**: Geolocation data tracks a device's physical location and can reveal sensitive information about individuals, such as visits to medical clinics or political rallies. Data brokers often collect and sell this data without explicit consent, raising privacy concerns. The Virginia Consumer Data Protection Act (VCDPA) is a state privacy law that gives consumers rights over their personal data. This new ban adds a specific prohibition on the sale of geolocation data to the existing framework.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hunton.com/privacy-and-cybersecurity-law-blog/virginia-bans-sale-of-geolocation-data">Virginia Bans Sale of Geolocation Data</a></li>
<li><a href="https://therecord.media/virginia-enacts-ban-on-precise-geolocation-data">Virginia enacts ban on precise geolocation data sales as momentum for similar prohibitions builds | The Record from Recorded Future News</a></li>
<li><a href="https://www.regulatoryoversight.com/2026/04/virginia-becomes-third-state-to-ban-sale-of-consumers-precise-geolocation-data/">Virginia Becomes Third State to Ban Sale of Consumers' Precise Geolocation Data | Regulatory Oversight</a></li>

</ul>
</details>

**Discussion**: Commenters generally support the ban, citing examples of misuse such as tracking visits to Planned Parenthood and car insurance companies using location data. However, some raise enforcement challenges, such as how to handle out-of-state companies or data processed in Virginia's AWS servers. Others note the law's effective date and call for stronger enforcement.

**Tags**: `#privacy`, `#geolocation data`, `#legislation`, `#data protection`, `#Virginia`

---

<a id="item-2"></a>
## [Podman v6.0.0 Released with Major Networking Overhaul](https://blog.podman.io/2026/07/introducing-podman-v6-0-0/) ⭐️ 8.0/10

Podman v6.0.0 has been released, introducing significant networking improvements including the adoption of Netavark and Aardvark for container networking, and dropping support for CNI, cgroups v1, iptables, and slirp4netns. This release marks a major step forward for Podman as a daemonless Docker alternative, with improved networking performance and simplified configuration, potentially accelerating adoption among developers and DevOps teams. Podman v6.0.0 also drops support for Windows 10 and Intel Macs, while adding new machine and Quadlet features. The update includes breaking changes that require migration from older networking stacks.

hackernews · soheilpro · Jul 2, 14:23 · [Discussion](https://news.ycombinator.com/item?id=48762098)

**Background**: Podman is an open-source, daemonless container engine that allows users to run containers without a central daemon, offering rootless mode and compatibility with Docker commands. It uses Buildah for image building and Conmon for monitoring OCI runtimes.

<details><summary>References</summary>
<ul>
<li><a href="https://lxer.com/module/newswire/view/365824/index.html">LXer: Podman 6 . 0 Lands with Breaking Changes, AMD GPUs Support</a></li>
<li><a href="https://github.com/podman-container-tools/podman">GitHub - podman -container-tools/ podman : Podman : A tool for...</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, with users praising Podman's ease of migration from Docker and improved networking. However, some users express frustration over limited distro support and reliance on outdated distro repositories for installation.

**Tags**: `#Podman`, `#containers`, `#Docker`, `#open source`, `#devops`

---

<a id="item-3"></a>
## [Immich 3.0 Sparks Encryption Debate](https://github.com/immich-app/immich/discussions/29439) ⭐️ 8.0/10

Immich 3.0, a major update to the self-hosted photo management platform, has been released, generating significant community discussion about encryption and usability. This release highlights the ongoing tension between privacy features like end-to-end encryption and practical usability in self-hosted alternatives to Google Photos and Apple Photos. The community debate centers on the absence of end-to-end encryption, with some users arguing it is unnecessary for self-hosted setups while others consider it a deal-breaker.

hackernews · hashier · Jul 2, 14:13 · [Discussion](https://news.ycombinator.com/item?id=48761944)

**Background**: Immich is a high-performance, open-source photo and video management solution that users can host on their own servers. It offers features like face recognition, album sharing, and mobile backup, positioning itself as a privacy-focused alternative to cloud services.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/immich-app/immich">GitHub - immich -app/ immich : High performance self - hosted photo ...</a></li>
<li><a href="https://github.com/immich-app/immich/issues/450">[Feature]: Encryption for data at rest · Issue #450 · immich-app/immich</a></li>
<li><a href="https://github.com/immich-app/immich/discussions/2901">[Encryption] Addition of Data Encryption Feature · immich-app/immich · Discussion #2901</a></li>

</ul>
</details>

**Discussion**: Comments show a split: some users praise Immich as a no-brainer replacement for cloud services, while others have switched to competitors like Ente Photos due to encryption concerns. A few users also report technical issues with iOS photo sync.

**Tags**: `#self-hosting`, `#photo management`, `#open source`, `#privacy`, `#software release`

---

<a id="item-4"></a>
## [Understand to Participate: Key to Avoiding Cognitive Debt](https://simonwillison.net/2026/Jul/2/understand-to-participate/#atom-everything) ⭐️ 8.0/10

Simon Willison highlighted Geoffrey Litt's concept of 'understand to participate' from a talk at AIE, arguing that developers must deeply understand AI-generated code to remain active participants and avoid cognitive debt. This framing addresses a critical challenge in AI-assisted coding: as agents produce more code, developers risk losing understanding, leading to cognitive debt that hampers future contributions and code quality. Geoffrey Litt presented this idea at the AIE World's Fair 2026, and his talk is available on YouTube along with 300+ other recordings. He also published a thread on Twitter summarizing his talk.

rss · Simon Willison · Jul 2, 17:07

**Background**: Cognitive debt refers to the mental burden developers accumulate when they don't fully understand code, especially code generated by AI. As AI coding agents become more capable, they can produce large, complex changes faster than humans can comprehend, risking a gap between what the code does and what the developer thinks it does. 'Understand to participate' proposes that developers should actively learn from the agent's output to maintain fluency and creative control.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/jul/2/understand-to-participate/">Understand to participate | Simon Willison’s Weblog</a></li>
<li><a href="https://unrollnow.com/status/2072522251300409556">Thread By @geoffreylitt - Hot take: I think it's still...</a></li>
<li><a href="https://getdx.com/blog/cognitive-debt-the-hidden-risk-in-ai-driven-software-development/">Cognitive debt: The hidden risk in AI-driven software development</a></li>

</ul>
</details>

**Tags**: `#AI-assisted coding`, `#cognitive debt`, `#software engineering`, `#developer productivity`

---

<a id="item-5"></a>
## [Cloudflare to Block Mixed-Use AI Crawlers by Default from September](https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/) ⭐️ 8.0/10

Cloudflare announced that starting September 15, 2026, it will default to blocking mixed-purpose crawlers—bots that collect data for both search indexing and AI training—from accessing ad-supported customer pages. The policy specifically calls out Google for exploiting a loophole where websites block AI crawlers but allow Googlebot, which then uses the data for AI training. This policy shift directly impacts the economics of web publishing and AI data acquisition, forcing AI companies like Google to either separate their crawlers or negotiate payment with publishers. It sets a precedent for how web content is used in the AI era, potentially reshaping the relationship between content creators and AI firms. The default blocking applies only to ad-supported pages; other pages remain unaffected unless site owners configure custom rules. Cloudflare's move is a proposed default change, meaning customers can opt out, but the company hopes it encourages mixed-use crawlers to separate search from AI agent and training use.

telegram · zaihuapd · Jul 2, 05:37

**Background**: Many websites block AI crawlers via robots.txt or other means, but they often allow Googlebot to maintain search visibility. Google has been using data from its search crawler to train its AI models, creating a loophole that Cloudflare's policy aims to close. Cloudflare is a major content delivery network that provides security and performance services to millions of websites, giving it significant influence over web traffic policies.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/07/01/cloudflares-new-policy-pushes-ai-companies-to-pay-for-publishers-content/">Cloudflare's new policy pushes AI companies to pay for publishers' content | TechCrunch</a></li>
<li><a href="https://letsdatascience.com/news/cloudflare-blocks-mixed-use-crawlers-on-monetized-pages-5a9acadb">Cloudflare Blocks Mixed-Use Crawlers on Monetized Pages | Let's Data Science</a></li>

</ul>
</details>

**Discussion**: The discussion highlights that many websites block AI crawlers but not Googlebot, and Google exploits this loophole to train its AI. The sentiment is supportive of Cloudflare's move, with users noting that AI companies should pay for content used in training.

**Tags**: `#Cloudflare`, `#AI`, `#web scraping`, `#Google`, `#content policy`

---

<a id="item-6"></a>
## [OpenAI Proposes 5% US Government Stake in AI Giants](https://www.bloomberg.com/news/articles/2026-07-02/openai-proposes-giving-the-us-government-a-5-stake-ft-says) ⭐️ 8.0/10

OpenAI has proposed that the US government take a 5% equity stake in itself and potentially other major AI companies like Google and Meta, aiming to share the economic gains of AI with the public. This proposal could reshape AI industry governance by creating a direct public benefit mechanism, but it also raises concerns about government control, regulatory conflicts, and potential stifling of innovation. A 5% stake in OpenAI alone would be worth approximately $42.6 billion based on its latest valuation of $852 billion. The proposal is still in early talks and other companies have not yet agreed.

telegram · zaihuapd · Jul 2, 06:02

**Background**: AI companies like OpenAI have built their models on vast public data and human knowledge, leading to debates about how to redistribute AI-generated wealth. Previous proposals include a 'robot tax' or adjusted corporate taxation. The current proposal suggests government equity as a novel mechanism to ensure public benefit from AI productivity gains.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jul/02/openai-stake-us-government-ai-sam-altman">OpenAI ‘in early talks to give 5% stake to US government’ | OpenAI | The Guardian</a></li>
<li><a href="https://www.engadget.com/2206552/openai-ai-companies-give-us-government-stake-businesses-proposal/">OpenAI reportedly wants all AI companies to give the US government a stake in their businesses - Engadget</a></li>
<li><a href="https://www.cnn.com/2026/07/02/business/openai-trump-stake-intl">OpenAI in talks to give Trump administration a 5% stake in the company, FT reports | CNN Business</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI regulation`, `#government equity`, `#tech policy`, `#AI industry`

---

<a id="item-7"></a>
## [Citibank Bans GPT-5.5 as AI Costs Surge for Enterprises](https://www.404media.co/companies-are-throttling-employees-ai-use-because-its-too-expensive/) ⭐️ 8.0/10

Citibank has banned the use of advanced AI models including GPT-5.5, Claude Opus 4.6, and 4.7 as of June 24, 2026, citing excessive consumption of AI credits. Atlassian's AI monthly spending surged from $5 million in August 2025 to over $15 million in May 2026, prompting the company to end unlimited usage and introduce cost-tracking dashboards. This trend signals a major shift in enterprise AI adoption, where the high cost of usage-based pricing for frontier models is forcing companies to rein in employee access. It highlights the tension between AI's potential and its financial sustainability, potentially slowing down the pace of AI integration in the workplace. Adobe has decided not to renew its contract for unlimited Claude usage, which expired on June 30, 2026. Amazon previously shut down an internal leaderboard that encouraged AI use, and employees later discovered previously unknown token usage caps. Consulting giant Accenture is packaging AI cost management as a new business opportunity while pushing clients to adopt AI rapidly.

telegram · zaihuapd · Jul 2, 13:59

**Background**: Enterprise AI tools like GPT-5.5 and Claude Opus are often priced per token or per API call, leading to unpredictable costs as usage scales. AI credits are a common metering mechanism where each model consumes a different number of credits per request. The recent release of more powerful models (GPT-5.5 in April 2026, Claude Opus 4.7 in April 2026) has increased per-request costs, exacerbating budget overruns for companies that previously offered unlimited access.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5.5">GPT-5.5</a></li>
<li><a href="https://www.anthropic.com/news/claude-opus-4-7">Introducing Claude Opus 4.7 \ Anthropic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cost management`, `#enterprise`, `#technology`

---

<a id="item-8"></a>
## [PS3 Store to Close in 2027, Archivists Race to Save Games](http://no-intro.org/) ⭐️ 8.0/10

Sony announced that the PlayStation Store for PS3 and PS Vita will permanently close in July 2027, prompting archivists and the RPCS3 emulator team to urgently back up digital game data. This closure threatens the loss of digital-only games that never received physical releases, highlighting the fragility of digital ownership and the importance of preservation efforts by the community. The RPCS3 team recommends using the no-intro.org database to catalog game metadata such as encryption signatures, file sizes, and serial numbers, helping the community track which titles have been preserved.

telegram · zaihuapd · Jul 2, 15:04

**Background**: The PlayStation 3, released in 2006, had a large digital library including many exclusive titles. RPCS3 is a free and open-source emulator that allows PS3 games to run on PC, with over 70% of games now playable. No-intro.org is a database that catalogs ROMs and digital games for preservation purposes.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/RPCS3">RPCS3</a></li>
<li><a href="https://no-intro.org/">No - Intro . org</a></li>
<li><a href="https://en.wikipedia.org/wiki/Video_game_preservation">Video game preservation - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#digital preservation`, `#gaming`, `#PS3`, `#RPCS3`, `#no-intro`

---

<a id="item-9"></a>
## [Linux 6.9 LUKS Suspend Fails to Wipe Encryption Keys](https://mathstodon.xyz/@iblech/116769502749142438) ⭐️ 7.0/10

A regression in Linux kernel 6.9 causes the LUKS suspend feature to no longer wipe disk-encryption keys from memory during suspend or hibernate, potentially exposing encrypted data. This bug undermines the security guarantee of full-disk encryption during sleep states, as the master key remains in memory and could be accessed via cold boot attacks or other memory forensics. The issue was introduced in Linux 6.9 and affects the cryptsetup luksSuspend command, which is used by Debian and derivatives; the kernel developers have acknowledged the regression and a fix is expected.

hackernews · IngoBlechschmid · Jul 2, 15:25 · [Discussion](https://news.ycombinator.com/item?id=48763035)

**Background**: LUKS (Linux Unified Key Setup) is a disk encryption specification that stores encryption keys in kernel memory during operation. When suspending to RAM, the key is normally kept in memory, but during suspend-to-disk (hibernate), the key should be wiped to prevent it from being written to swap. The luksSuspend command allows safely suspending encrypted devices by removing the key from memory.

<details><summary>References</summary>
<ul>
<li><a href="https://eucloudservers.com/security-encryption/since-linux-6-9-luks-suspend-stopped-wiping-disk-encryption-keys-from-memory/">Since Linux 6.9, LUKS Suspend Stopped Wiping Disk- encryption ...</a></li>
<li><a href="https://github.com/nailfarmer/debian-luks-suspend">GitHub - nailfarmer/debian- luks - suspend : Lock encrypted root volume...</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights mixed opinions: some argue the title is clickbait since luksSuspend is a Debian extension not officially supported upstream, while others emphasize the severity of the security regression. There is appreciation for NixOS testing that caught the bug, and debate over whether the kernel or distribution bears responsibility.

**Tags**: `#security`, `#linux`, `#kernel`, `#encryption`, `#bug`

---

<a id="item-10"></a>
## [PeerTube: Decentralized Video Platform Gains Traction](https://github.com/Chocobozzz/PeerTube) ⭐️ 7.0/10

PeerTube, a free and open-source decentralized video platform using ActivityPub federation, has gained significant community attention with a high-scoring discussion on Hacker News highlighting its potential and challenges. PeerTube offers a viable alternative to centralized platforms like YouTube, promoting data privacy and user control, but faces hurdles in monetization and content discovery that could limit mainstream adoption. PeerTube uses peer-to-peer technology to reduce server load for popular videos, and its federation via ActivityPub allows instances to share content. However, monetization options are limited, and the platform lacks the network effects of larger services.

hackernews · doener · Jul 2, 11:17 · [Discussion](https://news.ycombinator.com/item?id=48759634)

**Background**: PeerTube is a free and open-source video platform that is decentralized and federated, meaning anyone can run their own instance and connect with others. It uses the ActivityPub protocol to share videos across instances, and can leverage peer-to-peer streaming to distribute bandwidth costs. This contrasts with centralized platforms like YouTube, where a single company controls all content and infrastructure.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PeerTube">PeerTube - Wikipedia</a></li>
<li><a href="https://docs.joinpeertube.org/api/activitypub">ActivityPub | PeerTube documentation</a></li>

</ul>
</details>

**Discussion**: Community comments express enthusiasm for PeerTube's technical progress but highlight practical issues: professional creators worry about lack of monetization, users note sparse content in mainstream categories, and some suggest onboarding news agencies could boost adoption. Overall sentiment is cautiously optimistic, with recognition of both the platform's promise and its current limitations.

**Tags**: `#decentralization`, `#video platform`, `#open source`, `#federation`, `#PeerTube`

---

<a id="item-11"></a>
## [How to Ask Strangers for Help Effectively](https://pradyuprasad.com/writings/how-to-ask-for-help/) ⭐️ 7.0/10

A practical guide outlines key strategies for asking help from strangers, emphasizing proof of work and concise communication. This advice helps professionals and job seekers build networks and get assistance more effectively, reducing friction in help-seeking interactions. The guide stresses showing proof of work upfront and keeping requests brief, as strangers are more likely to help those who demonstrate genuine effort.

hackernews · FigurativeVoid · Jul 2, 13:19 · [Discussion](https://news.ycombinator.com/item?id=48761118)

**Background**: Asking for help from strangers is common in professional networking, but many people fail because they don't respect the recipient's time or show they've done their homework. The concept of 'proof of work' means demonstrating that you have already tried to solve the problem yourself before reaching out.

**Discussion**: Commenters agree with the core advice, adding that proof of work must be genuine and deep, not superficial. Some note that people often overestimate how frequently others receive requests, so a well-crafted ask can stand out.

**Tags**: `#career advice`, `#networking`, `#communication`, `#professional development`

---

<a id="item-12"></a>
## [Using DSPy to Evaluate and Improve Datasette Agent's SQL Prompts](https://simonwillison.net/2026/Jul/2/dspy-datasette-agent-prompts/#atom-everything) ⭐️ 7.0/10

Simon Willison used the DSPy framework to automatically evaluate and improve the system prompts for Datasette Agent's SQL query feature, identifying issues like column-name guessing and suggesting prompt refinements. This demonstrates a practical, automated approach to prompt engineering that can reduce manual trial-and-error, making LLM-powered tools more reliable and easier to maintain. The experiment used GPT-4.1 mini and nano as test models, and found that including column names in schema listings and softening advice against calling describe_table could reduce error-retry loops.

rss · Simon Willison · Jul 2, 18:25

**Background**: DSPy (Declarative Self-improving Python) is a framework that replaces brittle prompts with structured signatures and automated optimization. Datasette Agent is an AI assistant that generates SQL queries to answer user questions about data in Datasette. Prompt optimization aims to improve LLM output quality through automated evaluation and refinement.

<details><summary>References</summary>
<ul>
<li><a href="https://dspy.ai/">DSPy</a></li>
<li><a href="https://agent.datasette.io/">Datasette Agent : an AI assistant for Datasette to help explore and...</a></li>
<li><a href="https://github.com/stanfordnlp/dspy">GitHub - stanfordnlp/ dspy : DSPy : The framework for...</a></li>

</ul>
</details>

**Tags**: `#DSPy`, `#prompt engineering`, `#LLM`, `#Datasette`, `#SQL`

---

<a id="item-13"></a>
## [ChatGPT Doubles Weekly Users to 200 Million in Under a Year](https://t.me/zaihuapd/42298) ⭐️ 7.0/10

OpenAI announced that ChatGPT now has over 200 million weekly active users, doubling from 100 million in November 2023. Additionally, 92% of Fortune 500 companies are using OpenAI's products, and API usage has doubled since the release of the GPT-4o Mini model. This milestone underscores OpenAI's dominant position in the AI chatbot market despite increasing competition from Google, Microsoft, and Meta. The rapid adoption by Fortune 500 companies signals that AI is becoming integral to enterprise operations, potentially reshaping industries. The GPT-4o Mini model, a cost-effective alternative with a 128K context window, costs $0.15 per million input tokens and $0.60 per million output tokens. Rumors suggest Apple and Nvidia may be among OpenAI's next round of investors.

telegram · zaihuapd · Jul 1, 13:01

**Background**: ChatGPT, launched in November 2022, quickly became the fastest-growing consumer application in history. OpenAI has since released multiple model iterations, including GPT-4 and GPT-4o, with GPT-4o Mini being a smaller, cheaper variant designed for broader accessibility. Competitors like Google's Gemini, Microsoft's Copilot, and Meta's Llama have entered the market, but OpenAI maintains a strong lead.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenAI_o4-mini">OpenAI o4- mini - Wikipedia</a></li>
<li><a href="https://agentbreaking.com/models/openai--gpt-4o-mini/">OpenAI: GPT - 4 o - mini — AgentBreaking</a></li>

</ul>
</details>

**Tags**: `#AI`, `#ChatGPT`, `#OpenAI`, `#user growth`, `#industry adoption`

---

<a id="item-14"></a>
## [Yageo to Hike Capacitor Prices ~50% from July 1](https://www.trendforce.com/news/2026/07/01/news-passive-component-prices-rise-as-yageo-reportedly-begins-broadest-capacitor-hike-in-years-on-july-1/) ⭐️ 7.0/10

Yageo, a major passive component supplier, announced a broad price increase of approximately 50% on its entire capacitor product line, including MLCCs, aluminum electrolytic capacitors, and tantalum capacitors, effective July 1. This is the largest price hike in recent years. This price hike will significantly impact the electronics supply chain, raising costs for manufacturers of AI servers, electric vehicles, and consumer electronics. It also highlights the growing importance of passive components in AI server BOM costs, now second only to GPUs and memory. The official price increase is about 50%, but spot market prices for high-end capacitors have surged nearly tenfold in the past month. Yageo is raising prices for direct customers for the first time, and capacitors account for roughly half of Yageo's revenue.

telegram · zaihuapd · Jul 1, 14:34

**Background**: Capacitors are essential passive components used in nearly all electronic devices to store and release electrical energy. MLCCs (multilayer ceramic capacitors) are the most common type, while tantalum capacitors offer higher capacitance in smaller sizes but are more expensive. The price increase is driven by geopolitical tensions, rising energy and raw material costs, and surging demand from AI servers and EVs.

**Tags**: `#passive components`, `#capacitors`, `#supply chain`, `#price hike`, `#electronics`

---

<a id="item-15"></a>
## [Sony to End Physical Game Discs for New PlayStation Titles by 2028](https://blog.playstation.com/2026/07/01/physical-disc-production-ending-in-january-2028-for-new-games-releasing-on-playstation-consoles/) ⭐️ 7.0/10

Sony Interactive Entertainment announced on July 1, 2026, that starting January 2028, all new PlayStation games will be released exclusively as digital downloads, ceasing production of physical discs. This marks a major industry shift toward digital-only distribution for PlayStation, reflecting consumer trends and potentially impacting game ownership, resale, and preservation. The decision affects only new games released after January 2028; previously released physical discs remain unaffected. Sony will continue to offer digital purchases through the PlayStation Store and retail partners.

telegram · zaihuapd · Jul 1, 15:04

**Background**: Sony's PlayStation has long offered both physical disc and digital download options for games. In recent years, digital sales have grown significantly, with many players preferring the convenience of downloads. Sony's subsidiary, Sony Digital Audio Disc Corporation, is the sole manufacturer of PlayStation discs, making the transition logistically feasible.

<details><summary>References</summary>
<ul>
<li><a href="https://arstechnica.com/gaming/2026/07/sony-will-stop-making-physical-copies-of-playstation-games-in-2028/">Sony announces end of PlayStation discs, parts of digital store in the...</a></li>
<li><a href="https://www.player.one/sony-kills-physical-discs-playstation-platform-alongside-ps3-ps-vita-storefronts-163495">Sony Kills Physical Discs on the PlayStation Platform, Alongside...</a></li>
<li><a href="https://www.gematsu.com/2026/07/sony-interactive-entertainment-to-end-physical-game-disc-production-in-january-2028">Sony Interactive Entertainment to end physical game disc... - Gematsu</a></li>

</ul>
</details>

**Tags**: `#PlayStation`, `#digital distribution`, `#gaming industry`, `#Sony`

---

<a id="item-16"></a>
## [Apple Reveals iCloud Anonymous Email User to FBI](https://t.me/zaihuapd/42302) ⭐️ 7.0/10

Apple provided the FBI with the real iCloud account details behind an anonymous email address generated by its iCloud+ Hide My Email feature, in a threat investigation against FBI Director Kash Patel's girlfriend. This case demonstrates that Apple's Hide My Email feature is not fully anonymous in law enforcement investigations, challenging user assumptions about privacy and highlighting the limits of Apple's privacy promises. The suspect, Alden Ruml, created 134 anonymous email addresses using the iCloud+ feature and later admitted to sending threatening emails. The FBI obtained the real account information through a legal request to Apple.

telegram · zaihuapd · Jul 2, 01:03

**Background**: Apple's iCloud+ subscription includes a 'Hide My Email' feature that generates unique, random email addresses to forward emails to the user's real inbox, intended to protect privacy when signing up for services. However, Apple retains the mapping between anonymous and real addresses and can disclose it in response to valid legal requests.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnbeta.com.tw/articles/tech/1555430.htm">iCloud+ 隐 藏 邮 件 地 址 可不能乱用 苹果帮助FBI... - cnBeta.COM</a></li>
<li><a href="https://www.myzaker.com/article/6a45c04b8e9f09472f75e51d">iCloud+ 隐 藏 邮 箱 现严重漏洞，苹果多次修复未果_ZAKER新闻</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#privacy`, `#law enforcement`, `#iCloud`, `#anonymity`

---

<a id="item-17"></a>
## [Meta Plans to Sell Surplus AI Compute, Enter Cloud Market](https://www.bloomberg.com/news/articles/2026-07-02/south-korean-stocks-tumble-6-as-ai-jitters-hurt-chipmakers) ⭐️ 7.0/10

Meta is planning to sell excess AI computing capacity and AI model services to external customers, effectively entering the cloud computing market. This news, combined with Apple's talks to buy chips from Chinese memory makers, triggered a sharp drop in South Korean stocks on July 2, 2026. This move signals a potential shift in AI infrastructure dynamics, as major tech companies may repurpose surplus AI compute capacity rather than slowing investment. It also intensifies competition in the cloud market, challenging incumbents like AWS, Azure, and Google Cloud. Meta's capital expenditure for 2025 is $66-72 billion, with similar increases expected in 2026, leading to surplus compute capacity. The company is exploring two cloud business models: selling raw computing power and offering AI model access.

telegram · zaihuapd · Jul 2, 02:29

**Background**: Meta has been investing heavily in AI infrastructure, procuring data centers and chips at a pace that has outpaced its own AI workload consumption. This has created spare capacity that can now be monetized externally. The cloud computing market is currently dominated by Amazon (nearly 50% share), Microsoft, and Google.

<details><summary>References</summary>
<ul>
<li><a href="https://qz.com/meta-cloud-business-ai-computing-power-070126">Meta building cloud business to sell excess AI computing capacity</a></li>
<li><a href="https://247wallst.com/investing/2026/07/02/senior-analyst-meta-is-chasing-a-2-trillion-ai-compute-opportunity-but-its-years-behind/">Senior Analyst: Meta Is Chasing A $2 Trillion AI Compute Opportunity...</a></li>
<li><a href="https://www.marketbeat.com/articles/metas-ai-compute-push-could-turn-its-massive-capex-bill-into-a-competitive-weapon/">META Stock Turns Surplus AI Compute Into a New Revenue Stream</a></li>

</ul>
</details>

**Tags**: `#Meta`, `#AI`, `#Cloud Computing`, `#Semiconductors`, `#Market Impact`

---

<a id="item-18"></a>
## [Android 17 Drastically Limits Password Attempts to 20](https://www.digitaltrends.com/phones/android-17-makes-it-harder-for-bad-actors-to-guess-and-crack-the-pin-on-your-phone/) ⭐️ 7.0/10

Android 17 introduces a new lockout policy that allows only 6 incorrect attempts in the first minute, 7 in 6 minutes, 8 in 25 minutes, 12 in 24 hours, 19 in 5 years, and permanently locks the device after 20 consecutive errors. This change significantly reduces the risk of brute-force attacks on Android devices, making it much harder for attackers to guess PINs or passwords. It enhances user security and privacy, especially for devices that may be lost or stolen. Android 17 also includes duplicate error detection: if a user repeatedly enters the same wrong password, it is not counted as multiple failures. The lock screen now shows clearer prompts to prevent accidental lockouts due to confusing countdowns.

telegram · zaihuapd · Jul 2, 07:35

**Background**: Brute-force attacks involve trying many password combinations until the correct one is found. Previous Android versions allowed many more attempts before lockout (e.g., Android 16 allowed up to 1,800 guesses in 5 years). The new policy drastically reduces this window to protect user data.

<details><summary>References</summary>
<ul>
<li><a href="https://www.androidauthority.com/android-17-pin-password-protection-3683166/">Android 17 slashes PIN guess attempts from 1,800 to just 20</a></li>

</ul>
</details>

**Tags**: `#Android`, `#security`, `#mobile`, `#privacy`

---

<a id="item-19"></a>
## [CSRC Approves Unitree Technology's STAR Market IPO Registration](https://www.csrc.gov.cn/csrc/c105906/c7642867/content.shtml) ⭐️ 7.0/10

On July 1, 2026, the China Securities Regulatory Commission (CSRC) approved the IPO registration of Unitree Technology Co., Ltd. on the STAR Market, marking a critical step toward its listing. Unitree is a leading robotics unicorn in China, and its STAR Market listing will provide capital for expansion and signal strong policy support for the robotics industry, potentially accelerating the commercialization of humanoid robots. The CSRC requires Unitree to strictly follow the prospectus and underwriting plan submitted to the Shanghai Stock Exchange, and to report any major events during the period from registration to issuance.

telegram · zaihuapd · Jul 2, 09:57

**Background**: Unitree Technology is known for its quadruped robots and humanoid robots, such as the G1 and R1 models. The company has deployed NVIDIA's full-stack robotics technology in its R1 humanoid robot, which is priced at 39,900 yuan and expected to enter mass production by the end of 2026. The STAR Market is China's Nasdaq-style board for tech companies, and IPO registration is the final regulatory hurdle before listing.

<details><summary>References</summary>
<ul>
<li><a href="https://eu.36kr.com/zh/p/3419294583000457">eu.36kr.com/zh/p/3419294583000457</a></li>
<li><a href="https://c.m.163.com/news/a/JO7AAQTE051100B9.html">在强者云集的机器人高地，王兴兴的 宇 树 凭什么出人头地</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#科创板`, `#机器人`, `#宇树科技`

---

<a id="item-20"></a>
## [Anthropic in Talks with Samsung for Custom AI Chip](https://www.theinformation.com/articles/anthropic-talks-samsung-manufacture-custom-ai-chip) ⭐️ 7.0/10

Anthropic has begun developing its own AI chip and is in early-stage talks with Samsung Electronics for manufacturing, aiming to gain more control over the computing infrastructure for its Claude models. This move signals a growing trend among major AI labs to reduce reliance on external chip suppliers like Nvidia, potentially reshaping the AI hardware landscape and giving Anthropic more leverage in optimizing performance and cost. The project is still in early stages, and Anthropic has not confirmed a manufacturing order with Samsung. The company is entering the custom chip race later than peers like OpenAI and Google.

telegram · zaihuapd · Jul 2, 15:57

**Background**: Anthropic is an AI safety company best known for its Claude large language models. Developing custom AI chips allows AI companies to tailor hardware to their specific model architectures, improving efficiency and reducing dependence on general-purpose chips like Nvidia's GPUs. Samsung is a major semiconductor foundry competing with TSMC.

<details><summary>References</summary>
<ul>
<li><a href="https://winbuzzer.com/2026/06/04/samsung-foundry-pursues-anthropic-as-openai-path-cools-xcxwbn/">Samsung Foundry Pursues Anthropic as OpenAI Path Cools</a></li>
<li><a href="https://en.theblockbeats.news/news/62945">Anthropic Taps Samsung to Make AI Chip : Another Ace in the...</a></li>

</ul>
</details>

**Tags**: `#Anthropic`, `#AI chip`, `#Samsung`, `#hardware`, `#AI infrastructure`

---

<a id="item-21"></a>
## [Kernel.org Mirror Error Empties /pub, Data Intact](http://kernel.org/) ⭐️ 7.0/10

On July 2, an error during the switch of kernel.org's primary/secondary mirror infrastructure caused the /pub directory to become empty, but no data was lost and recovery is underway. Kernel.org is a critical resource for the Linux ecosystem, hosting the official kernel source code and related files; this incident temporarily disrupted access to essential downloads, affecting developers and users worldwide. The deletion was fast but recovery is slow, so full restoration will take time; users can track progress via the Linux Foundation status page at status.linuxfoundation.org.

telegram · zaihuapd · Jul 3, 00:28

**Background**: Kernel.org is the official repository for the Linux kernel source code and related archives. The /pub directory contains publicly accessible files such as kernel tarballs and patches. Mirror infrastructure ensures high availability and load distribution across multiple servers worldwide.

<details><summary>References</summary>
<ul>
<li><a href="https://lwn.net/Articles/1081015/">Kernel archive /pub tree restoring [LWN.net]</a></li>
<li><a href="https://www.kernel.org/">The Linux Kernel Archives</a></li>
<li><a href="https://habr.com/ru/news/1055006/">Из-за досадной ошибки на ресурсе kernel . org удалили со... / Хабр</a></li>

</ul>
</details>

**Tags**: `#kernel.org`, `#Linux`, `#infrastructure`, `#incident`, `#recovery`

---