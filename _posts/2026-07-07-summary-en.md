---
layout: default
title: "Horizon Summary: 2026-07-07 (EN)"
date: 2026-07-07
lang: en
---

> From 27 items, 13 important content pieces were selected

---

1. [OpenWrt One: Open Hardware Router Launched](#item-1) ⭐️ 8.0/10
2. [Anthropic Finds 'Global Workspace' Neurons in LLMs](#item-2) ⭐️ 8.0/10
3. [Tencent Releases Hy3: 295B MoE Model, Apache 2.0](#item-3) ⭐️ 8.0/10
4. [China to Cut SCI Publication Incentives for Security](#item-4) ⭐️ 8.0/10
5. [FBI Tracks Hacker via Microsoft GDID Device Identifier](#item-5) ⭐️ 8.0/10
6. [Bilibili Sends Legal Letter to BiliRoaming Open-Source Project](#item-6) ⭐️ 8.0/10
7. [Microsoft Reshapes Xbox for Profitability](#item-7) ⭐️ 7.0/10
8. [Hard Tech Majors Overtake Software in Graduate Salaries](#item-8) ⭐️ 7.0/10
9. [Wealthy US families spend thousands on AI education for kids](#item-9) ⭐️ 7.0/10
10. [Microsoft Books 40% of Profits in Ireland with 3% of Staff](#item-10) ⭐️ 7.0/10
11. [SpaceX Falcon 9 Debris Creates Metal Pollution in Upper Atmosphere](#item-11) ⭐️ 7.0/10
12. [China Plans Asteroid Defense System with Ground and Space Monitoring](#item-12) ⭐️ 7.0/10
13. [Claude Cowork Sandbox Escape Vulnerability Disclosed](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenWrt One: Open Hardware Router Launched](https://openwrt.org/toh/openwrt/one) ⭐️ 8.0/10

OpenWrt and the Software Freedom Conservancy have jointly launched the OpenWrt One, the first fully upstream-supported open hardware router design, announced in late 2024. This project empowers users to extend router lifespan and gain advanced capabilities beyond manufacturer support, promoting the right to repair and open source hardware in networking. The OpenWrt One is based on Banana Pi boards and is organized through the Software Freedom Conservancy. It aims to provide a fully open and supported hardware platform for OpenWrt.

hackernews · peter_d_sherman · Jul 6, 18:23 · [Discussion](https://news.ycombinator.com/item?id=48808482)

**Background**: OpenWrt is an open-source Linux-based operating system for embedded devices, primarily used for network routing. It has historically been installed as third-party firmware on various routers, but the OpenWrt One is the first official hardware designed specifically for it.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/OpenWrt">OpenWrt - Wikipedia</a></li>
<li><a href="https://lwn.net/Articles/957255/">The OpenWrt One project [LWN.net]</a></li>
<li><a href="https://www.theregister.com/2024/12/02/openwrt_one_foss_wifi_router/">Open source router firmware OpenWrt ships its own hardware</a></li>

</ul>
</details>

**Discussion**: Community comments are generally positive, with users praising OpenWrt for extending router life and gaining capabilities. Some note installation complexity and desire for faster LAN ports, while others share personal experiences with the device.

**Tags**: `#OpenWrt`, `#open hardware`, `#router`, `#networking`, `#open source`

---

<a id="item-2"></a>
## [Anthropic Finds 'Global Workspace' Neurons in LLMs](https://www.anthropic.com/research/global-workspace) ⭐️ 8.0/10

Anthropic's research identifies a set of 'global workspace' neurons in language models that integrate information across diverse tasks, drawing a parallel to the cognitive science concept of global workspace theory. This work advances mechanistic interpretability by revealing how language models achieve coherent, context-aware behavior, potentially leading to safer and more controllable AI systems. The 'global workspace' neurons are identified through a method that measures how much a small change in a layer's activation affects the final output, forming a 'J-space' that represents shared reasoning across contexts.

hackernews · in-silico · Jul 6, 17:44 · [Discussion](https://news.ycombinator.com/item?id=48808002)

**Background**: Global workspace theory (GWT) is a cognitive architecture proposed in the 1980s that posits a central workspace where information from specialized modules is broadcast to the rest of the brain, enabling conscious awareness. Anthropic's research applies this concept to large language models, suggesting that similar integration mechanisms exist in artificial neural networks. This is part of Anthropic's broader interpretability efforts to understand and ensure the safety of deployed models like Claude.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Global_workspace_theory">Global workspace theory - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/research/mapping-mind-language-model">Mapping the Mind of a Large Language Model \ Anthropic</a></li>

</ul>
</details>

**Discussion**: Commenters generally appreciate the interpretability work but question the parallels to human consciousness, noting that the identified 'J-space' may simply reflect an abstract reasoning subspace rather than true awareness. Some users recall related experiments, such as duplicating math-solving layers to improve performance, suggesting this area will yield further insights.

**Tags**: `#interpretability`, `#language models`, `#AI research`, `#neural networks`, `#cognitive science`

---

<a id="item-3"></a>
## [Tencent Releases Hy3: 295B MoE Model, Apache 2.0](https://simonwillison.net/2026/Jul/6/hy3/#atom-everything) ⭐️ 8.0/10

Tencent has released Hy3, a 295-billion-parameter Mixture-of-Experts (MoE) language model with 21 billion active parameters and 3.8B MTP layer parameters, under the Apache 2.0 license. The model supports a 256K context length and is available on Hugging Face and OpenRouter. Hy3 outperforms similar-sized models and rivals flagship open-source models with 2-5x more parameters, making it a significant addition to the open-source AI ecosystem. Its Apache 2.0 license encourages broad adoption and further development. The full-precision model is 598GB on Hugging Face, while an FP8 quantized version is 300GB. The model is available for free on OpenRouter until July 21st, 2026.

rss · Simon Willison · Jul 6, 23:57

**Background**: Mixture-of-Experts (MoE) is a machine learning technique that divides a problem into regions handled by specialized expert networks, activating only a subset of parameters per input for efficiency. MTP (Multi-Token Prediction) is a technique that predicts multiple future tokens simultaneously to improve inference speed. FP8 quantization reduces model size and speeds up inference by using 8-bit floating-point numbers.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>
<li><a href="https://huggingface.co/blog/moe">Mixture of Experts Explained - Hugging Face</a></li>
<li><a href="https://verl.readthedocs.io/en/latest/advance/mtp.html">Guide to Using MTP in SFT/RL Training and Inference</a></li>

</ul>
</details>

**Tags**: `#AI`, `#open-source`, `#LLM`, `#Mixture-of-Experts`, `#Tencent`

---

<a id="item-4"></a>
## [China to Cut SCI Publication Incentives for Security](https://www.ft.com/content/64a811f1-b132-4211-8a8c-2252cf964039?syn-25a6b1a6=1) ⭐️ 8.0/10

Chinese policymakers are discussing reducing incentives for researchers to publish in international journals like SCI, and may lower the weight of SCI papers in academic promotion and tenure decisions. The National Natural Science Foundation now requires at least 20% of representative papers from funded projects to be published in Chinese journals. This policy shift could significantly alter global scientific publishing dynamics, as China is a major contributor to international journals. It also raises concerns about academic freedom and the balance between national security and open science. The Ministry of State Security recently accused a researcher of leaking core equipment structures and key experimental data in a submission to an international journal. A materials scientist reported stopping submissions to foreign journals due to vague and tightening security review standards.

telegram · zaihuapd · Jul 6, 01:03

**Background**: SCI (Science Citation Index) is a widely used database for indexing scientific journals, and publishing in SCI journals has been a key metric for academic evaluation in China. The government has been promoting the development of domestic journals to reduce reliance on foreign platforms and prevent technology leakage.

<details><summary>References</summary>
<ul>
<li><a href="https://www.edu.cn/rd/gai_kuang/zhuan_jia_ping_shu/202004/t20200408_1720343.shtml">破除“SCI至上”，要从质量与分类评价入手-高校科技-中国教育和科研计算机网CERNET</a></li>
<li><a href="https://epaper.gmw.cn/gmrb/html/2025-06/26/nw.D110000gmrb_20250626_2-16.htm">打造自主可控的学术出版平台-光明日报-光明网</a></li>
<li><a href="https://www.nppa.gov.cn/xxfb/zcfg/gfxwj/202106/t20210623_4514.html">中共中央宣传部 教育部 科技部印发 《关于推动学术期刊繁荣发展的意见》的通知</a></li>

</ul>
</details>

**Discussion**: A commenter speculated that the policy might be aimed at combating academic fraud. The discussion reflects mixed views, with some supporting the security rationale and others concerned about potential negative impacts on research quality and international collaboration.

**Tags**: `#science policy`, `#national security`, `#academic publishing`, `#China`, `#technology transfer`

---

<a id="item-5"></a>
## [FBI Tracks Hacker via Microsoft GDID Device Identifier](https://www.itnews.com.au/news/microsoft-device-telemetry-key-to-unmasking-alleged-scattered-spider-hacker-627148) ⭐️ 8.0/10

The FBI arrested 19-year-old hacker Peter Stokes by leveraging Microsoft's Global Device Identifier (GDID), a persistent device-level identifier that remains unchanged even when using a VPN. This case reveals that Microsoft's GDID can be used by law enforcement to track users across VPNs, raising significant privacy concerns for Windows users worldwide. The GDID is generated during Windows installation and persists across updates; users cannot easily change it without reinstalling Windows. The FBI cross-referenced GDID with proxy logs and account data from Snapchat, Apple, and Facebook.

telegram · zaihuapd · Jul 6, 04:15

**Background**: GDID stands for Global Device Identifier, a unique string tied to each Windows installation that Microsoft uses for device telemetry. Unlike IP addresses or browser fingerprints, GDID is not easily spoofed or changed, making it a powerful tracking tool.

<details><summary>References</summary>
<ul>
<li><a href="https://www.tomshardware.com/software/windows-11-identifier-used-to-track-scattered-spider-perp-after-microsoft-shared-info-with-fbi-19-year-old-us-estonian-hacker-arrested-over-alleged-ties-to-infamous-extortion-group">Windows 11 identifier code used to track Scattered Spider perp after Microsoft shared info with FBI — 19-year-old US-Estonian hacker arrested over alleged ties to infamous extortion group | Tom's Hardware</a></li>
<li><a href="https://securityonline.info/microsoft-gdid-tracking/">Microsoft GDID Tracking: How Windows Caught a Hacker</a></li>
<li><a href="https://www.pcmag.com/news/a-hackers-arrest-reveals-microsoft-can-track-users-via-a-windows-device">A Hacker's Arrest Reveals Microsoft Can Track Users Via a Windows Device ID | PCMag</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#security`, `#Microsoft`, `#device tracking`, `#law enforcement`

---

<a id="item-6"></a>
## [Bilibili Sends Legal Letter to BiliRoaming Open-Source Project](https://github.com/yujincheng08/BiliRoaming) ⭐️ 8.0/10

Bilibili, through a law firm, sent a cease-and-desist letter to the BiliRoaming open-source project, demanding it stop reverse engineering and remove code that bypasses regional restrictions and payment protections. This legal action highlights the tension between copyright enforcement and open-source reverse engineering, potentially setting a precedent for how platforms handle third-party tools that modify client behavior. The letter specifically cites playback authentication hooking, rewriting paid episodes as viewable, bypassing secure transport locking, and rewriting CDN origin-pull to steal platform distribution resources.

telegram · zaihuapd · Jul 6, 08:21

**Background**: BiliRoaming is an Xposed module for Android that removes regional restrictions on Bilibili's bangumi (anime) content and provides other small features. Xposed is a framework that allows modifying the behavior of Android apps without altering their APK files. CDN origin-pull refers to the process where a CDN fetches content from the origin server when not cached.

<details><summary>References</summary>
<ul>
<li><a href="https://www.chiphell.com/thread-2842265-1-1.html">付费番剧解限制工具“哔哩漫游”收到 B 站 律师函，GitHub...</a></li>
<li><a href="https://modules.lsposed.org/module/me.iacn.biliroaming/">哔哩漫游/ BiliRoaming · Xposed Module Repository</a></li>
<li><a href="https://sourceforge.net/projects/biliroaming.mirror/">BiliRoaming download | SourceForge.net</a></li>

</ul>
</details>

**Tags**: `#open-source`, `#reverse engineering`, `#legal`, `#Bilibili`, `#DMCA`

---

<a id="item-7"></a>
## [Microsoft Reshapes Xbox for Profitability](https://news.xbox.com/en-us/2026/07/06/resetting-xbox/) ⭐️ 7.0/10

Microsoft announced a major restructuring of its Xbox division, aiming to improve profit margins and return to growth, as revealed in a July 2026 blog post. This move signals a strategic shift for Xbox from market share expansion to sustainable profitability, reflecting broader industry trends toward cost discipline and could reshape Microsoft's gaming ecosystem. The restructuring includes layoffs and studio closures, with CEO Asha acknowledging past corporate mismanagement and allowing some studios to return to independence.

hackernews · dijksterhuis · Jul 6, 14:18 · [Discussion](https://news.ycombinator.com/item?id=48804993)

**Background**: Xbox generates about $5 billion in quarterly revenue but has thin, non-growing profit margins of around $150-160 million. The gaming industry has seen increasing costs and a shift toward service-based models like Game Pass, while competitors like Nintendo focus on lower-cost, high-selling titles.

**Discussion**: Community comments are highly critical, with users calling the restructuring a 'mess' and blaming former leadership for poor strategy. Some express sympathy for laid-off workers and appreciate the new CEO's candor, while others doubt Microsoft will ever succeed in gaming due to its engineering-focused culture.

**Tags**: `#Xbox`, `#Microsoft`, `#gaming industry`, `#business strategy`, `#restructuring`

---

<a id="item-8"></a>
## [Hard Tech Majors Overtake Software in Graduate Salaries](https://news.sina.com.cn/c/2026-07-05/doc-inifuaqy8947308.shtml) ⭐️ 7.0/10

According to the 2026 Chinese Undergraduate Employment Report by MyCOS, microelectronics and electronic science and technology topped the salary rankings for 2025 graduates, while computer science and software engineering dropped out of the top ten. This shift signals that China's industrial upgrade is moving from internet-based services to hard tech and smart manufacturing, which will influence students' major choices and university resource allocation. The average monthly income for 2025 graduates was 6,435 yuan, with microelectronics at 7,814 yuan and electronic science at 7,752 yuan. The report reflects a broader trend where hardware-related fields are gaining economic value.

telegram · zaihuapd · Jul 6, 06:34

**Background**: For years, computer science and software engineering dominated high-paying majors due to the booming internet industry. However, as China prioritizes semiconductor self-sufficiency and advanced manufacturing, demand for hardware talent has surged, driving up salaries in microelectronics and electronic science.

<details><summary>References</summary>
<ul>
<li><a href="https://www.peopleapp.com/rmharticle/30049394366">哪些 专 业 就 业 好、收入高？_ 教育在线</a></li>
<li><a href="https://www.gk100.com/read_1212041133466.htm">电子科学与技术专业就业方向及前景!附2025大学排名及分数线-高考100</a></li>

</ul>
</details>

**Tags**: `#education`, `#industry trends`, `#salary report`, `#hard tech`

---

<a id="item-9"></a>
## [Wealthy US families spend thousands on AI education for kids](https://www.theverge.com/ai-artificial-intelligence/961505/wealthy-ai-schools-alpha-forge-prep) ⭐️ 7.0/10

Wealthy US families are enrolling children in AI-driven private schools like Forge Prep and Alpha School, paying up to $75,000 per year, but critics argue children are being used as test subjects for unproven technology. This trend raises ethical concerns about unregulated AI adoption in education, potential inequality, and lack of transparency, as schools do not publish outcome data to prove AI's superiority over traditional methods. Alpha School's co-founder stated that controversial social topics like women's rights and slavery history are excluded from the curriculum, and some campuses cover K-12. Forge Prep received 600 applications for only 34 spots in its first year.

telegram · zaihuapd · Jul 6, 07:19

**Background**: AI in education refers to using artificial intelligence to personalize learning, often replacing traditional teachers with software. Forge Prep and Alpha School are private institutions that rely heavily on AI for instruction, with human 'guides' instead of teachers. Critics worry about the lack of evidence and potential harm to children.

<details><summary>References</summary>
<ul>
<li><a href="https://forgeprep.org/ai-head-of-school/">AI Head of School - Forge Prep</a></li>
<li><a href="https://alpha.school/learn-more/">Learn More About Alpha School | AI -Powered 2-Hour Learning</a></li>
<li><a href="https://en.wikipedia.org/wiki/Alpha_School">Alpha School - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#AI in education`, `#ethics`, `#EdTech`, `#inequality`, `#privacy`

---

<a id="item-10"></a>
## [Microsoft Books 40% of Profits in Ireland with 3% of Staff](https://www.techspot.com/news/113001-microsoft-new-eu-disclosure-shows-exactly-how-tech.html) ⭐️ 7.0/10

Microsoft's EU disclosure reveals that nearly 40% of its global pretax profits for the fiscal year ending June 2025 were booked in Ireland, where only about 3% of its global employees are based. This disclosure highlights aggressive profit-shifting strategies by major tech companies, undermining tax bases in high-tax countries and fueling debates on global tax reform and corporate transparency. In Germany, France, and Italy, profit margins were in the single digits, with Germany reporting less than 0.5% of profits; Luxembourg's 34 employees generated $283 million in pretax income, a 142% profit margin.

telegram · zaihuapd · Jul 6, 09:19

**Background**: Profit shifting involves multinational corporations moving profits from high-tax jurisdictions to low-tax ones like Ireland (12.5% corporate tax rate) to reduce tax liabilities. The EU's 2021 transparency directive requires large companies to disclose revenues and taxes country-by-country, exposing such practices. The OECD's BEPS project aims to combat base erosion and profit shifting through coordinated rules.

<details><summary>References</summary>
<ul>
<li><a href="https://time.com/6326583/tax-shelters-multinational-corporations/">How Corporations Shift Profits to Avoid Taxes - TIME</a></li>
<li><a href="https://www.oecd.org/en/topics/base-erosion-and-profit-shifting-beps.html">Base erosion and profit shifting (BEPS) | OECD</a></li>
<li><a href="https://en.wikipedia.org/wiki/Ireland_as_a_tax_haven">Ireland as a tax haven - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#tax avoidance`, `#Microsoft`, `#corporate transparency`, `#EU regulation`, `#profit shifting`

---

<a id="item-11"></a>
## [SpaceX Falcon 9 Debris Creates Metal Pollution in Upper Atmosphere](https://t.me/zaihuapd/42387) ⭐️ 7.0/10

A new study published in a Nature sub-journal directly detected a lithium plume from a SpaceX Falcon 9 rocket reentry, with lithium concentrations spiking 10-fold at 96 km altitude. This is the first direct evidence that rocket reentry debris introduces measurable metal pollution into the upper atmosphere, potentially threatening the ozone layer and raising environmental concerns for the growing space industry. The lithium plume was detected about 20 hours after the uncontrolled reentry of a Falcon 9 upper stage over Europe, using high-precision lidar. The lithium concentration was approximately 10 times higher than normal background levels.

telegram · zaihuapd · Jul 6, 11:17

**Background**: Rocket stages that reenter Earth's atmosphere burn up, releasing metals like lithium, aluminum, and copper. These metals can accumulate in the upper atmosphere and potentially catalyze reactions that deplete the ozone layer. Lidar (light detection and ranging) is a remote sensing technique that uses laser pulses to measure atmospheric composition at high altitudes.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sciencenews.org/article/rocket-reentry-metal-pollution-detected">Metal pollution from a rocket reentry detected for the first time</a></li>
<li><a href="https://theconversation.com/spacex-rocket-left-behind-a-plume-of-chemical-pollution-as-it-burnt-up-in-the-atmosphere-276266">SpaceX rocket left behind a plume of chemical pollution as it ...</a></li>
<li><a href="https://gizmodo.com/study-confirms-reentering-spacex-rockets-are-peppering-the-upper-atmosphere-with-metal-pollution-2000723932">Study Confirms: Reentering SpaceX Rockets Are Peppering the Upper ...</a></li>

</ul>
</details>

**Tags**: `#space pollution`, `#SpaceX`, `#atmospheric science`, `#rocket reentry`, `#environmental impact`

---

<a id="item-12"></a>
## [China Plans Asteroid Defense System with Ground and Space Monitoring](http://paper.people.com.cn/rmrb/pc/content/202607/06/content_30166956.html) ⭐️ 7.0/10

China is officially planning to build an asteroid defense system that integrates ground-based telescopes and a space-based constellation for continuous day-and-night monitoring, and is developing kinetic impact and gravity tractor technologies for deflection. This announcement marks a significant step in global planetary defense, as China joins the United States and Europe in developing active mitigation capabilities. It addresses the critical gap in detecting medium-sized near-Earth objects (140 meters), of which only about 45% have been found. The system will use a combination of instantaneous techniques like kinetic impact and sustained techniques like gravity tractor, ion beam deflection, and laser ablation. China has already preliminarily developed an impact risk warning model and is building an operational early warning system.

telegram · zaihuapd · Jul 6, 13:36

**Background**: Near-Earth objects (NEOs) are asteroids and comets with orbits that bring them close to Earth. While large asteroids (over 1 km) have been mostly cataloged, smaller ones (140 m) are harder to detect and could cause regional devastation. Planetary defense involves detecting, tracking, and deflecting potentially hazardous objects. The United States has NASA's DART mission, which successfully demonstrated kinetic impact in 2022, and Europe's Hera mission to follow up.

<details><summary>References</summary>
<ul>
<li><a href="https://news.youth.cn/gn/202606/t20260630_16739416.htm">news.youth.cn/gn/202606/t20260630_16739416.htm</a></li>
<li><a href="https://www.chinanews.com/gn/2026/07-06/10653371.shtml">天外来客 防 范有策 我国正在论证 小 行 星 防 御 系统-中新网</a></li>

</ul>
</details>

**Tags**: `#asteroid defense`, `#space technology`, `#planetary defense`, `#China space program`, `#near-Earth objects`

---

<a id="item-13"></a>
## [Claude Cowork Sandbox Escape Vulnerability Disclosed](https://cyberpress.org/claude-cowork-flaw/) ⭐️ 7.0/10

A security researcher discovered a sandbox escape chain in Anthropic's Claude Desktop for Windows, exploiting DLL sideloading and unfiltered parameters in the Claude Cowork feature to gain root access in the Ubuntu VM and exfiltrate /etc/shadow. Anthropic dismissed the report as not a security issue because it requires prior code execution on the host. This vulnerability highlights the risks of sandbox isolation in AI coding tools, as a successful escape could allow attackers to access sensitive host data. The disclosure also raises questions about Anthropic's security response, as they dismissed a well-documented exploit chain. The attack chain uses DLL sideloading on claude.exe and two unfiltered parameters (isResume and allowedDomains) in the spawn interface, combined with nsenter to escape the bubblewrap sandbox. The exploit was reported in March 2026 and scored 7.0/10 on Cyber Press.

telegram · zaihuapd · Jul 6, 14:53

**Background**: DLL sideloading is a technique where an attacker places a malicious DLL in a directory that a legitimate application loads from, exploiting Windows' search order. Bubblewrap is a lightweight sandbox tool used by Flatpak and other container systems to isolate applications. nsenter is a Linux command that allows entering another process's namespaces, often used to escape containers.

<details><summary>References</summary>
<ul>
<li><a href="https://techzone.bitdefender.com/en/tech-explainers/what-is-dll-sideloading.html">What is DLL Sideloading – Bitdefender TechZone</a></li>
<li><a href="https://github.com/containers/bubblewrap">GitHub - containers/bubblewrap: Low-level unprivileged ...</a></li>
<li><a href="https://man7.org/linux/man-pages/man1/nsenter.1.html">nsenter(1) - Linux manual page</a></li>

</ul>
</details>

**Tags**: `#security`, `#vulnerability`, `#sandbox escape`, `#Anthropic`, `#Claude`

---