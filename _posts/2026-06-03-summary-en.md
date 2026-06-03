---
layout: default
title: "Horizon Summary: 2026-06-03 (EN)"
date: 2026-06-03
lang: en
---

> From 36 items, 15 important content pieces were selected

---

1. [Hackers Trick Meta AI Bot to Hijack Instagram Accounts](#item-1) ⭐️ 9.0/10
2. [Anthropic Expands Project Glasswing to 15 Countries](#item-2) ⭐️ 8.0/10
3. [Microsoft Unveils MAI-Thinking-1 and MAI-Code-1-Flash LLMs](#item-3) ⭐️ 8.0/10
4. [Tencent Secretly Builds AI Agent for WeChat Mini-Programs](#item-4) ⭐️ 8.0/10
5. [Tiger Brokers Halts New Positions for China Mainland Accounts](#item-5) ⭐️ 8.0/10
6. [Trump Signs AI Executive Order with Voluntary Model Review](#item-6) ⭐️ 8.0/10
7. [iOS 27 May Bring Split-Screen for Foldable iPhone](#item-7) ⭐️ 8.0/10
8. [CT Scans Reveal BYD Car Parts Engineering](#item-8) ⭐️ 7.0/10
9. [User Leaves Gmail Over Intrusive AI Features](#item-9) ⭐️ 7.0/10
10. [Seattle Surveillance Walking Tour Exposes Hidden Cameras](#item-10) ⭐️ 7.0/10
11. [Why You Should Love systemd Timers](#item-11) ⭐️ 7.0/10
12. [Wise Investigated in Belgium Over Suspicious Transactions](#item-12) ⭐️ 7.0/10
13. [CVD Protocol in Clash Verge Rev Sparks Privacy and Compatibility Debate](#item-13) ⭐️ 7.0/10
14. [Rural Elderly Trapped in 'Ancient Trap': Who Pays for Dignified Aging?](#item-14) ⭐️ 7.0/10
15. [OpenAI Launches Sites: Codex Turns Ideas into Interactive Apps](#item-15) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Hackers Trick Meta AI Bot to Hijack Instagram Accounts](https://simonwillison.net/2026/Jun/1/hackers-simply-asked-meta-ai/#atom-everything) ⭐️ 9.0/10

Hackers exploited Meta's AI support chatbot by simply asking it to link a new email address to high-profile Instagram accounts, successfully taking over accounts including the Obama White House account. This incident reveals a critical security flaw in integrating AI chatbots with sensitive account recovery systems, potentially affecting millions of users and eroding trust in AI-driven customer support. The attack is a form of prompt injection, where the bot was tricked into bypassing standard verification steps like two-factor authentication. Meta has not yet released a fix or official statement.

rss · Simon Willison · Jun 1, 21:14

**Background**: Prompt injection is a technique where attackers craft inputs that override an AI chatbot's intended behavior. In this case, Meta's AI support bot was given the ability to perform account recovery actions, which the hackers exploited by simply asking it to link a new email.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theguardian.com/technology/2026/jun/01/meta-ai-hack-obama-sephora-instagram">Hackers trick Meta AI support bot to infiltrate Obama White House Instagram account | Meta | The Guardian</a></li>
<li><a href="https://techcrunch.com/2026/06/01/hackers-hijacked-instagram-accounts-by-tricking-meta-ai-support-chatbot-into-granting-access/">Hackers hijacked Instagram accounts by tricking Meta AI support chatbot ...</a></li>
<li><a href="https://cybersecuritynews.com/metas-ai-support-bot-instagram/">Hackers Use Meta's AI Bot to Reset Passwords and Hijack Instagram Accounts</a></li>

</ul>
</details>

**Discussion**: The community expressed shock and criticism, with many pointing out that this was an obvious design flaw. Some cybersecurity experts noted that the attack barely qualifies as prompt injection, as the bot was explicitly designed to perform the action it was tricked into doing.

**Tags**: `#security`, `#AI`, `#Meta`, `#prompt injection`, `#account takeover`

---

<a id="item-2"></a>
## [Anthropic Expands Project Glasswing to 15 Countries](https://www.anthropic.com/news/expanding-project-glasswing) ⭐️ 8.0/10

Anthropic announced the expansion of Project Glasswing, a security scanning initiative using its Claude Mythos AI model, to critical infrastructure in 15 countries. This expansion broadens the use of advanced AI for vulnerability detection in essential systems, potentially improving global cybersecurity but also raising concerns about access and reliability. Claude Mythos is a large language model designed to find software vulnerabilities, but it has not been publicly released due to safety concerns. Community feedback highlights issues with false positives and limited compute capacity.

hackernews · surprisetalk · Jun 2, 13:15 · [Discussion](https://news.ycombinator.com/item?id=48369863)

**Background**: Project Glasswing is Anthropic's cybersecurity initiative launched in April 2026 to secure critical software infrastructure using AI. Claude Mythos is an advanced model internally described as a 'step change' in capabilities, but its gated preview has drawn mixed reactions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Project_Glasswing">Project Glasswing</a></li>
<li><a href="https://www.anthropic.com/research/glasswing-initial-update">Project Glasswing: An initial update \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Claude_Mythos">Claude Mythos</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism: some users report excessive false positives and noise from the tool, while others question Anthropic's motives, suggesting compute capacity shortages are masked as security concerns. Additionally, some security professionals note difficulty in gaining access even for large organizations.

**Tags**: `#AI`, `#security`, `#Anthropic`, `#critical infrastructure`, `#Claude`

---

<a id="item-3"></a>
## [Microsoft Unveils MAI-Thinking-1 and MAI-Code-1-Flash LLMs](https://simonwillison.net/2026/Jun/2/microsofts-new-models/#atom-everything) ⭐️ 8.0/10

Microsoft announced two new text LLMs: MAI-Thinking-1, a 1-trillion-parameter reasoning model with 35 billion active parameters, and MAI-Code-1-Flash, a 137-billion-parameter code model with 5 billion active parameters, purpose-built for GitHub Copilot. These models demonstrate Microsoft's push into efficient, specialized AI with Mixture-of-Experts architectures, claiming competitive performance against larger models like Claude Opus 4.6. The code model's integration into GitHub Copilot could significantly impact developer workflows. MAI-Thinking-1 is a sparse MoE model with 1 trillion total parameters but only 35 billion active, trained on enterprise-grade data without distillation from third-party models. MAI-Code-1-Flash is rolling out to GitHub Copilot individual users in VS Code, built end-to-end by Microsoft using clean and appropriately licensed data.

rss · Simon Willison · Jun 2, 22:21

**Background**: Mixture-of-Experts (MoE) models activate only a subset of parameters per token, enabling larger total capacity with lower inference cost. Microsoft's MAI models are part of a broader trend toward specialized, efficient LLMs for specific tasks like reasoning and code generation.

<details><summary>References</summary>
<ul>
<li><a href="https://microsoft.ai/news/introducing-mai-thinking-1/">Introducing MAI-Thinking-1 - Microsoft AI</a></li>
<li><a href="https://microsoft.ai/news/introducingmai-code-1-flash/">Introducing MAI-Code-1-Flash | Microsoft AI</a></li>
<li><a href="https://github.blog/changelog/2026-06-02-mai-code-1-flash-is-now-available-for-github-copilot/">MAI-Code-1-Flash is now available for GitHub Copilot - GitHub Changelog</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#Microsoft`, `#AI models`, `#reasoning`, `#code generation`

---

<a id="item-4"></a>
## [Tencent Secretly Builds AI Agent for WeChat Mini-Programs](https://t.me/zaihuapd/41705) ⭐️ 8.0/10

According to foreign media citing four insiders, Tencent is secretly developing an AI agent for WeChat that aims to connect millions of mini-programs, enabling the agent to perform tasks like taxi booking and grocery ordering on behalf of users. If successful, this AI agent could leverage WeChat's 1.4 billion monthly active users to become a dominant platform for AI-driven services, intensifying competition with Alibaba and ByteDance in China's AI market. The agent is designed to work with the millions of mini-programs already running inside WeChat, potentially automating a wide range of daily tasks. Tencent has not yet responded to requests for comment.

telegram · zaihuapd · Jun 2, 05:03

**Background**: WeChat is a super-app developed by Tencent that integrates messaging, social media, mobile payment, and thousands of third-party mini-programs. Mini-programs are lightweight apps that run within WeChat without requiring separate installation, covering services from e-commerce to transportation. AI agents are software programs that can autonomously perform tasks on behalf of users, and integrating them with messaging platforms is a growing trend in the tech industry.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/WeChat_Mini_Program">WeChat Mini Program</a></li>
<li><a href="https://walkthechat.com/wechat-mini-programs-simple-introduction/">What are WeChat Mini-Programs? A Simple Introduction - WalktheChat</a></li>

</ul>
</details>

**Tags**: `#AI Agent`, `#WeChat`, `#Tencent`, `#Mini Programs`, `#China Tech`

---

<a id="item-5"></a>
## [Tiger Brokers Halts New Positions for China Mainland Accounts](https://mp.weixin.qq.com/s/LgwHvOhuFw338kvWPgPyvw) ⭐️ 8.0/10

Tiger Brokers announced that starting June 12, 2026, it will suspend new positions and additional purchases for all securities in mainland Chinese accounts, allowing only sell and close positions, in compliance with regulatory requirements. This marks a major step in China's crackdown on illegal cross-border securities activities, affecting many mainland investors who use overseas brokerages. It signals tighter enforcement and could reshape the cross-border trading landscape. The suspension applies to all securities types, including stocks, and also halts inbound fund transfers while outbound transfers remain normal. Existing assets and overseas services are unaffected.

telegram · zaihuapd · Jun 2, 12:56

**Background**: China's securities regulator and seven other departments recently issued a comprehensive plan to crack down on illegal cross-border securities activities, targeting overseas brokerages like Tiger Brokers and Futu. The plan requires a two-year cleanup of existing illegal business, prohibiting these firms from soliciting mainland clients or opening new accounts.

<details><summary>References</summary>
<ul>
<li><a href="https://www.stcn.com/article/detail/3922656.html">中国证监会等八部门联合印发《综合整治非法跨境证券期货基金经营活动实施方案》</a></li>
<li><a href="https://www.news.cn/fortune/20260522/d155e2db294442bfb63d0bddb97cc9cc/c.html">财经深一度丨强监管聚合力 8部门重拳整治非法跨境证券期货基金经营活动-新华网</a></li>
<li><a href="https://www.yicai.com/news/103198159.html">八部门联手综合整治非法跨境展业，境外券商无牌经营“灰色时代”终结</a></li>

</ul>
</details>

**Tags**: `#regulatory`, `#fintech`, `#cross-border trading`, `#China`, `#securities`

---

<a id="item-6"></a>
## [Trump Signs AI Executive Order with Voluntary Model Review](https://www.whitehouse.gov/presidential-actions/2026/06/promoting-advanced-artificial-intelligence-innovation-and-security/) ⭐️ 8.0/10

President Trump signed an executive order on June 2, 2026, establishing a voluntary framework for AI developers to submit advanced models for cybersecurity review 30 days before public release, and creating an AI cybersecurity clearinghouse. This order signals a shift toward voluntary, industry-friendly AI regulation in the U.S., balancing national security concerns with the goal of maintaining American AI leadership. It could set a precedent for future AI governance and impact global regulatory trends. The final order reduced the review period from an earlier draft's 90 days to 30 days, and explicitly prohibits mandatory government licensing or pre-approval mechanisms. The AI cybersecurity clearinghouse will coordinate vulnerability discovery and patching across government and critical infrastructure.

telegram · zaihuapd · Jun 2, 16:44

**Background**: The executive order is part of ongoing U.S. efforts to regulate AI, following earlier attempts like the Biden administration's AI executive order. The voluntary framework aims to address cybersecurity risks from advanced AI models without stifling innovation, amid industry pushback against mandatory requirements.

<details><summary>References</summary>
<ul>
<li><a href="https://federalnewsnetwork.com/cybersecurity/2026/06/ai-executive-order-sets-stage-for-new-cybersecurity-directives/">AI executive order sets stage for new cybersecurity directives | Federal News Network</a></li>
<li><a href="https://www.cybersecuritydive.com/news/trump-ai-security-executive-order/821755/">Trump signs EO seeking early government access to powerful AI models | Cybersecurity Dive</a></li>
<li><a href="https://www.csoonline.com/article/4180205/trump-revives-parts-of-canceled-ai-order-with-cybersecurity-focused-directive.html">Trump revives parts of canceled AI order with cybersecurity-focused directive | CSO Online</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the order's substance, with some calling it a 'door-shutting' step toward eventual prohibition of open-source models. Others question the practical implementation of the voluntary review and note the reduction from 90 to 30 days as a win for industry.

**Tags**: `#AI regulation`, `#executive order`, `#cybersecurity`, `#US policy`, `#AI safety`

---

<a id="item-7"></a>
## [iOS 27 May Bring Split-Screen for Foldable iPhone](https://www.macrumors.com/2026/06/02/ios-27-split-screen-app-adaptation-feature/) ⭐️ 8.0/10

According to MacRumors, Apple is developing a system-level landscape adaptation feature in iOS 27 that automatically adjusts portrait apps to widescreen layouts, enabling split-screen multitasking on the rumored foldable iPhone with a 7.8-inch inner display. The feature is expected to be announced at WWDC 2026. This would address a long-standing iOS limitation on large screens, potentially accelerating foldable iPhone adoption and aligning the iOS ecosystem with iPadOS multitasking capabilities. It could also reduce developer burden by eliminating the need for manual app redesigns. The feature is system-level, meaning it works automatically without developer intervention, similar to how iPadOS handles app scaling. The rumored foldable iPhone is said to feature a 5.5-inch outer display and a 7.8-inch inner display, with a thickness of 9.5mm folded and 4.5mm unfolded.

telegram · zaihuapd · Jun 3, 02:02

**Background**: iOS has historically lacked robust split-screen multitasking, a feature Android foldables have offered for years. Apple's iPadOS already supports split-view and slide-over, but iPhone apps are typically designed for portrait orientation. A system-level adaptation would bridge this gap without requiring developers to create separate layouts.

<details><summary>References</summary>
<ul>
<li><a href="https://post.smzdm.com/p/aggzp65w/">等了 6 年！ 苹果 折 叠 屏 iPhone ...</a></li>

</ul>
</details>

**Tags**: `#iOS`, `#foldable`, `#split-screen`, `#WWDC`, `#Apple`

---

<a id="item-8"></a>
## [CT Scans Reveal BYD Car Parts Engineering](https://www.lumafield.com/scan-of-the-month/byd) ⭐️ 7.0/10

Lumafield published high-resolution CT scans of BYD car parts, including a key fob, drive unit, and battery pack, providing an unprecedented look at their internal engineering. This challenges the negative perception of Chinese automotive quality by revealing robust, well-engineered components, and highlights BYD's vertical integration and manufacturing scale. The scans show a BYD key fob with a mechanical backup key, a drive unit with integrated motor and inverter, and a Blade Battery pack. BYD produces about 75% of its components in-house, similar to Tesla but at a larger scale.

hackernews · viasfo · Jun 2, 20:30 · [Discussion](https://news.ycombinator.com/item?id=48375824)

**Background**: BYD is a Chinese automaker and battery manufacturer that vertically integrates production from lithium mining to vehicle assembly. CT scanning uses X-rays to create cross-sectional images, allowing non-destructive inspection of internal structures.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BYD_Auto">BYD Auto - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Comments are largely positive, with a master technician praising the heavy-duty build quality of a BYD Shark. One user corrected a detail about the key fob's mechanical key mechanism, and another noted BYD's production volume exceeds Tesla's.

**Tags**: `#BYD`, `#EV`, `#engineering`, `#teardown`, `#automotive`

---

<a id="item-9"></a>
## [User Leaves Gmail Over Intrusive AI Features](https://moddedbear.com/gmail-thinks-im-stupid-so-i-left) ⭐️ 7.0/10

A user publicly announced their departure from Gmail, citing frustration with Google's aggressive integration of AI features like smart reply and email drafting, and switched to Fastmail. This reflects growing user backlash against AI features that prioritize convenience over user autonomy, and highlights the trade-offs between free services and paid alternatives like Fastmail. The user praised Fastmail for its speed, instant operations, and features like app passwords and hide-my-email, while noting the calendar lacks address autocomplete.

hackernews · speckx · Jun 2, 19:27 · [Discussion](https://news.ycombinator.com/item?id=48375016)

**Background**: Gmail has been integrating AI features powered by Gemini, such as smart compose and suggested replies, which some users find intrusive and unnecessary. Fastmail is a paid email hosting service known for speed and privacy, offering a clean interface without AI-driven suggestions.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Fastmail">Fastmail - Wikipedia</a></li>
<li><a href="https://www.fastmail.com/">Email and calendar made better | Fastmail</a></li>
<li><a href="https://www.expressvpn.com/blog/gmail-ai-privacy-risks/">Your guide to understanding Google Gmail AI security</a></li>

</ul>
</details>

**Discussion**: Commenters debated the value of AI in email, with some finding smart replies useful for simple responses but criticizing verbose LLM-generated drafts. Others noted that many 'Gmail killers' are just paid services, while Fastmail and HEY offer distinct mental models.

**Tags**: `#email`, `#AI`, `#privacy`, `#user experience`, `#Gmail`

---

<a id="item-10"></a>
## [Seattle Surveillance Walking Tour Exposes Hidden Cameras](https://coveillance.org/a-walking-tour-of-surveillance-infrastructure-in-seattle/) ⭐️ 7.0/10

A walking tour in Seattle, documented at coveillance.org, maps out the city's extensive surveillance infrastructure including cameras, license plate readers, and Amazon Go tracking technologies, highlighting their impact on privacy and social norms. This tour raises critical awareness about the normalization of surveillance in public spaces, prompting public debate on privacy, civil liberties, and the subtle ways technology enforces social conformity. The tour covers various surveillance technologies such as automated license plate readers, traffic-monitoring devices, and store tracking systems, with a focus on how cameras encode 'ways of seeing' that enforce social norms.

hackernews · eustoria · Jun 2, 13:24 · [Discussion](https://news.ycombinator.com/item?id=48369980)

**Background**: Surveillance infrastructure in cities like Seattle has expanded significantly since 9/11, with cameras and sensors becoming ubiquitous. These systems are often justified for public safety but raise concerns about privacy and the erosion of civil liberties. The walking tour serves as a field guide to make these hidden technologies visible to the public.

<details><summary>References</summary>
<ul>
<li><a href="https://all-waterparks.com/general/a-walking-tour-of-surveillance-infrastructure-in-seattle/">A walking tour of surveillance infrastructure in Seattle - All Waterparks</a></li>
<li><a href="https://flipso.com/p/9wdryxgwl">A walking tour of surveillance infrastructure in Seattle · Flipso | Flipso</a></li>
<li><a href="https://www.kaggle.com/datasets/city-of-seattle/seattle-surveillance-technologies">Seattle Surveillance Technologies | Kaggle</a></li>

</ul>
</details>

**Discussion**: Comments express mixed views: some see surveillance as the 'new normal' and question its effectiveness (e.g., prosecutors requiring video evidence), while others criticize the tour's academic language as inaccessible. A few commenters lament the loss of freedom and collusion between government and corporations.

**Tags**: `#surveillance`, `#privacy`, `#Seattle`, `#civil liberties`, `#technology`

---

<a id="item-11"></a>
## [Why You Should Love systemd Timers](https://blog.tjll.net/you-dont-love-systemd-timers-enough/) ⭐️ 7.0/10

A blog post argues that systemd timers are superior to cron for Linux task scheduling, highlighting advantages like predictable paths, resilience to system startup times, and better integration with systemd's ecosystem. This matters because systemd timers address key limitations of cron, such as missed jobs during system downtime, and offer tighter integration with modern Linux systems, making them a more robust choice for system administrators. systemd timers require two files (a .timer unit and a .service unit) compared to cron's single crontab entry, which some see as a drawback. However, they support features like monotonic timers, randomized delays, and persistent timers that run missed jobs after boot.

hackernews · yacin · Jun 2, 09:34 · [Discussion](https://news.ycombinator.com/item?id=48367904)

**Background**: Cron is the traditional Linux task scheduler that runs jobs at fixed times, but it skips jobs if the system is off. systemd timers are part of the systemd init system, offering more flexible scheduling, logging via journalctl, and dependency management.

<details><summary>References</summary>
<ul>
<li><a href="https://xtom-dev.pages.dev/blog/systemd-vs-cron-linux-task-scheduling/">Systemd Timers vs . Cron : Which One Should You Use? | xTom</a></li>
<li><a href="https://medium.com/@tolulinux/linux-scheduled-cron-vs-systemd-timer-738dedcc6a71">Linux Scheduled: Cron vs Systemd timers | by Tolulope... | Medium</a></li>
<li><a href="https://unix.stackexchange.com/questions/278564/cron-vs-systemd-timers">Cron vs systemd timers - Unix & Linux Stack Exchange</a></li>

</ul>
</details>

**Discussion**: Comments show mixed opinions: some praise timers for resilience and journalctl integration, while others criticize the two-file requirement as cumbersome. A user shares a practical use case for backup automation, and another humorously describes using a timer to print a dog picture weekly.

**Tags**: `#systemd`, `#cron`, `#Linux`, `#scheduling`, `#system administration`

---

<a id="item-12"></a>
## [Wise Investigated in Belgium Over Suspicious Transactions](https://www.thebureauinvestigates.com/stories/2026-06-01/money-transfer-giant-wise-investigated-for-half-a-billion-in-suspicious-transactions) ⭐️ 7.0/10

Belgian prosecutors are investigating Wise for suspected non-compliance with anti-money laundering regulations, involving approximately 500 million euros in suspicious transactions across Europe. This investigation could undermine trust in Wise and the broader fintech industry, highlighting the challenges of enforcing AML compliance across borders. The probe covers hundreds of judicial requests from over 30 European countries, and Wise's U.S. subsidiary was previously fined $4.2 million for similar violations.

telegram · zaihuapd · Jun 2, 03:59

**Background**: Anti-money laundering (AML) regulations require financial institutions to verify customer identities and report suspicious activities. Wise, a UK-based money transfer fintech, has faced regulatory scrutiny in multiple jurisdictions for compliance failures.

<details><summary>References</summary>
<ul>
<li><a href="https://www.bankingdive.com/news/wise-aml-investigation-europe/821721/">Fintech Wise probed over AML concerns | Banking Dive</a></li>
<li><a href="https://fintechnews.sg/132383/payments/wise-money-laundering/">Wise Faces Belgium Probe Over Money Laundering Control...</a></li>

</ul>
</details>

**Tags**: `#fintech`, `#regulatory`, `#anti-money laundering`, `#compliance`, `#investigation`

---

<a id="item-13"></a>
## [CVD Protocol in Clash Verge Rev Sparks Privacy and Compatibility Debate](https://github.com/clash-verge-rev/clash-verge-rev/commit/2cb9c13ab6f0b0fec5ccc622c669843c935942ed) ⭐️ 7.0/10

Clash Verge Rev introduced a new subscription security mechanism called CVD (Clash Verge Device-binding Protocol) in its dev branch, which generates device keys and encrypts subscriptions per device to prevent URL abuse. This protocol addresses the real problem of subscription URL leakage and bulk abuse, but it also introduces privacy risks by creating persistent device identifiers and may reduce compatibility with third-party clients and cross-device synchronization. The CVD protocol is still in early development and largely AI-generated, with no real-world deployment yet; its feasibility requires further community discussion and analysis.

telegram · zaihuapd · Jun 2, 11:07

**Background**: Clash Verge Rev is a popular open-source proxy client based on the Tauri framework, supporting Windows, macOS, and Linux. Traditional subscription URLs, once leaked, can be copied and used by many devices indefinitely, leading to abuse. CVD aims to bind subscriptions to specific devices by requiring clients to report a public key, allowing servers to limit the number of devices and revoke access.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/clash-verge-rev/clash-verge-rev">GitHub - clash - verge - rev / clash - verge - rev : A modern GUI client based...</a></li>
<li><a href="https://talkin.icu/blog/cvd-device-binding-privacy-risks">CVD Device Binding : Privacy Risks Explained</a></li>
<li><a href="https://clash-verge.org/">Clash Verge - Modern Cross-Platform Proxy Client | Open Source...</a></li>

</ul>
</details>

**Discussion**: The community is divided: some appreciate the security improvement against subscription abuse, while others worry about the privacy implications of device fingerprinting and the potential for forced adoption that could break existing workflows.

**Tags**: `#proxy`, `#security`, `#privacy`, `#open-source`, `#protocol`

---

<a id="item-14"></a>
## [Rural Elderly Trapped in 'Ancient Trap': Who Pays for Dignified Aging?](https://www.caixin.com/2026-06-01/102449600.html) ⭐️ 7.0/10

A Caixin analysis reveals that rural elderly in China face a 'seventy-year-old trap' where pensions of about 250 yuan per month are insufficient, forcing continued labor into old age. This highlights a systemic gap in China's social security, affecting 2.6 billion low-income people (90% rural), and raises intergenerational equity concerns as younger workers question the sustainability of the pay-as-you-go system. Rural pension is only 1/15 of urban employee pensions and below the rural minimum living standard of 594 yuan. The 'ancient trap' refers to income dropping sharply after age 70 as labor ability declines without adequate pension replacement.

telegram · zaihuapd · Jun 2, 15:47

**Background**: China's dual-track pension system provides generous benefits to urban employees while rural residents rely on a basic scheme. Traditionally, land and family support served as safety nets, but urbanization and land fragmentation have weakened these. The 'ancient trap' concept was introduced in academic literature to describe the income collapse rural elderly face around age 70.

<details><summary>References</summary>
<ul>
<li><a href="http://njnydxxbskb.paperonce.org/oa/pdfdow.aspx?Sid=20220405">标题</a></li>
<li><a href="https://www.workercn.cn/papers/grrb/2024/07/12/6/grrb202407126.pdf">workercn.cn/papers/grrb/2024/07/12/6/grrb202407126.pdf</a></li>

</ul>
</details>

**Tags**: `#rural aging`, `#social security`, `#China`, `#pension gap`, `#economic inequality`

---

<a id="item-15"></a>
## [OpenAI Launches Sites: Codex Turns Ideas into Interactive Apps](https://x.com/OpenAI/status/2061845949170045346) ⭐️ 7.0/10

OpenAI has launched Sites, a new feature for Codex that enables users to transform work content, ideas, and plans into interactive websites or applications accessible via URL. The feature is initially available to Business and Enterprise users, with broader rollout planned. Sites lowers the barrier to creating interactive web applications, allowing non-developers to turn ideas into functional apps without coding expertise. This could accelerate prototyping and collaboration within organizations, expanding the reach of AI-assisted development. Sites links a local source project to hosting managed through Codex, storing the linkage in a .openai/hosting.json file. The feature is currently limited to Business and Enterprise tiers, with no public pricing or availability date announced for broader access.

telegram · zaihuapd · Jun 2, 17:29

**Background**: OpenAI Codex is an AI system that translates natural language into code, powering tools like GitHub Copilot. Sites extends Codex's capabilities by enabling direct deployment of generated code as interactive web apps, bridging the gap between idea generation and functional software.

<details><summary>References</summary>
<ul>
<li><a href="https://developers.openai.com/codex/sites">Sites – Codex | OpenAI Developers</a></li>
<li><a href="https://grokipedia.com/page/OpenAI_Codex">OpenAI Codex</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#Codex`, `#AI-assisted development`, `#interactive applications`, `#product launch`

---