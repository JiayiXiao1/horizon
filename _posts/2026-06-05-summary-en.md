---
layout: default
title: "Horizon Summary: 2026-06-05 (EN)"
date: 2026-06-05
lang: en
---

> From 30 items, 17 important content pieces were selected

---

1. [Cloudflare acquires VoidZero, integrates Vite into Workers](#item-1) ⭐️ 9.0/10
2. [Anthropic's open-source framework for AI-powered vulnerability discovery](#item-2) ⭐️ 8.0/10
3. [Meta Ships Facial Recognition on Smart Glasses](#item-3) ⭐️ 8.0/10
4. [Gaussian Point Splatting: A New 3D Rendering Technique](#item-4) ⭐️ 8.0/10
5. [AI Enthusiasts vs. Skeptics: A Race Against Time and Entropy](#item-5) ⭐️ 8.0/10
6. [Tiger Brokers Halts New Positions for China Accounts from June 12](#item-6) ⭐️ 8.0/10
7. [DeepSeek tops US enterprise software charts as firms seek cheaper AI](#item-7) ⭐️ 8.0/10
8. [Apple's New Siri to Use Google, Nvidia Chips for Cloud AI](#item-8) ⭐️ 8.0/10
9. [AI Agent Traffic Surpasses Human Traffic for First Time](#item-9) ⭐️ 8.0/10
10. [Google Removes 'Humans in the Loop' After Employee Memes](#item-10) ⭐️ 7.0/10
11. [Uber Caps AI Coding Tool Usage to $1,500/Month Per Tool](#item-11) ⭐️ 7.0/10
12. [Sam Altman: OpenAI's top user consumes ~100B tokens monthly](#item-12) ⭐️ 7.0/10
13. [WeChat Partners with Phone Makers for A2A Assistant](#item-13) ⭐️ 7.0/10
14. [First Lychee-Longan Hybrid 'Huaishi' Bears Fruit](#item-14) ⭐️ 7.0/10
15. [US Bipartisan GUARD Act Targets Chinese Robot Imports](#item-15) ⭐️ 7.0/10
16. [ChatGPT Memory Upgrade: Auto-Learns Preferences, Stays Fresh](#item-16) ⭐️ 7.0/10
17. [US Tech Layoffs Hit 2-Year High in May, AI Cited as Top Reason](#item-17) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Cloudflare acquires VoidZero, integrates Vite into Workers](https://www.cloudflare.com/press/press-releases/2026/cloudflare-acquires-voidzero-to-build-the-future-of-the-ai-native-web/) ⭐️ 9.0/10

Cloudflare announced the acquisition of VoidZero, the company behind Vite, Vitest, Rolldown, and Oxc, on June 4, 2026. The tools will be deeply integrated into Cloudflare Workers, enabling one-click deployment from local code to the global network. This acquisition brings a widely adopted frontend toolchain (Vite has over 130 million weekly downloads) directly into a major cloud platform, simplifying the path from development to deployment. It also signals a strategic move to capture the AI-native web trend, where AI coding agents increasingly rely on Vite. VoidZero's team will join Cloudflare and continue to advance the open-source roadmap. Cloudflare has committed a $1 million independent Vite ecosystem fund to support community contributors, and all tools (Vite, Rolldown, Oxc, Vitest) will remain under MIT open-source license and vendor-neutral.

telegram · zaihuapd · Jun 5, 00:39

**Background**: Vite is a next-generation JavaScript build tool that provides fast development server startup and hot module replacement. It is part of a broader toolchain that includes Vitest (testing), Rolldown (bundler), and Oxc (Rust-based parser/linter). Cloudflare Workers is a serverless edge computing platform that allows developers to run code globally. This acquisition aims to combine these tools to offer a seamless developer experience from local development to edge deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance ...</a></li>

</ul>
</details>

**Discussion**: Community sentiment is mixed: some express unease about the acquisition, fearing that open-source projects may lose independence or that Cloudflare's UX issues could affect the tools. Others see it as a natural business move, noting that Vite's popularity with AI agents makes it a strategic asset. A few commenters also draw parallels to earlier acquisitions like Astro.

**Tags**: `#Cloudflare`, `#Vite`, `#acquisition`, `#frontend`, `#open-source`

---

<a id="item-2"></a>
## [Anthropic's open-source framework for AI-powered vulnerability discovery](https://github.com/anthropics/defending-code-reference-harness) ⭐️ 8.0/10

Anthropic released an open-source framework for AI-powered vulnerability discovery, designed to help security researchers build custom harnesses for automated code analysis. The framework is based on their Claude model and aims to lower the barrier for using AI in security research. This release democratizes access to advanced AI vulnerability discovery tools, previously only available to large organizations, and could significantly accelerate the identification of security flaws in open-source software. It also signals Anthropic's commitment to open-source security tools, potentially influencing industry practices. The framework is hosted on GitHub under the name 'defending-code-reference-harness' and includes guidelines for building custom harnesses. According to the repository, running the framework costs roughly hundreds of dollars with Opus and thousands with Mythos, with each agent consuming ~10K uncached input tokens/min and ~2K output tokens/min.

hackernews · binyu · Jun 4, 20:11 · [Discussion](https://news.ycombinator.com/item?id=48403980)

**Background**: Anthropic has been using its Claude model, particularly the Mythos preview, to find vulnerabilities in open-source software. In February 2026, they began using Mythos for vulnerability discovery, and as of May 2026, they have identified over 23,000 issues, including more than 6,200 high- or critical-severity vulnerabilities across 1,000+ projects. This framework is part of their broader effort to share tools with the security community.

<details><summary>References</summary>
<ul>
<li><a href="https://www.anthropic.com/coordinated-vulnerability-disclosure">Coordinated vulnerability disclosure for Claude-discovered vulnerabilities \ Anthropic</a></li>
<li><a href="https://red.anthropic.com/2026/cvd/">Anthropic's coordinated vulnerability disclosure dashboard</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/05/26/anthropic-project-glasswing-update/">Anthropic: Claude Mythos identified 10,000+ software flaws - Help Net Security</a></li>

</ul>
</details>

**Discussion**: The community discussion highlights mixed reactions: some users compare the framework to a 'shop jig' that researchers can adapt, while others question the cost of running it, estimating hundreds to thousands of dollars. There is also confusion about the repository name 'Anthropics' versus 'Anthropic', and a note about a potential flagging issue affecting GitHub links.

**Tags**: `#AI`, `#security`, `#open-source`, `#vulnerability discovery`, `#Anthropic`

---

<a id="item-3"></a>
## [Meta Ships Facial Recognition on Smart Glasses](https://www.buchodi.com/meta-glasses-facial-recognition/) ⭐️ 8.0/10

Meta has integrated facial recognition into its Ray-Ban smart glasses, reportedly under the name 'Name Tag', allowing the device to identify people and display their names. The feature is currently being tested and has sparked significant privacy and legal debates. This move reignites concerns about pervasive surveillance and biometric data collection in public spaces, especially as smart glasses become more common. It also highlights the tension between accessibility benefits for individuals with prosopagnosia and the potential for privacy violations. The feature reportedly uses an offline database of photos to recognize friends and acquaintances, but the exact implementation details remain unclear. Legal risks include potential violations of the Biometric Information Privacy Act (BIPA) in Illinois, which regulates the collection of biometric data.

hackernews · buchodi · Jun 4, 19:36 · [Discussion](https://news.ycombinator.com/item?id=48403588)

**Background**: Facial recognition technology identifies or verifies a person from an image or video. Meta's Ray-Ban smart glasses are a wearable device with a camera and AI capabilities, previously criticized for privacy issues such as recording people without consent. Prosopagnosia, or face blindness, is a neurological condition affecting face recognition, which could benefit from such technology if implemented with privacy safeguards.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prosopagnosia">Prosopagnosia</a></li>
<li><a href="https://www.linkedin.com/posts/ho-mun-fei_meta-ai-privacy-activity-7433846422187237376-Ldb4">Meta 's Name Tag: Facial Recognition in Smart Glasses ... | LinkedIn</a></li>
<li><a href="https://www.bbc.com/news/articles/cj37z8357e5o">Smart glasses are 'an invasion of privacy ' - Meta 's are selling b...</a></li>

</ul>
</details>

**Discussion**: Comments express mixed reactions: some see accessibility benefits for prosopagnosia, while others strongly oppose the privacy implications. Users also reference legal risks under BIPA and past incidents of Meta employees viewing private recordings from the glasses.

**Tags**: `#facial recognition`, `#privacy`, `#smart glasses`, `#Meta`, `#ethics`

---

<a id="item-4"></a>
## [Gaussian Point Splatting: A New 3D Rendering Technique](https://momentsingraphics.de/Siggraph2026.html) ⭐️ 8.0/10

Gaussian Point Splatting introduces a novel approach to 3D rendering that uses Gaussian splats instead of traditional polygons, building on the recent 3D Gaussian Splatting method for real-time radiance field rendering. This technique could enable real-time photorealistic rendering from sparse image inputs, potentially transforming AAA game development and other real-time graphics applications by offering a new way to represent and render complex scenes. The method optimizes anisotropic 3D Gaussians and uses a fast visibility-aware rendering algorithm, achieving real-time performance. Community comments compare it to older point splatting techniques from the 1990s and to mesh splatting, noting that Gaussians may struggle with sharp features.

hackernews · ibobev · Jun 4, 10:48 · [Discussion](https://news.ycombinator.com/item?id=48396792)

**Background**: Gaussian splatting is a volume rendering technique originally introduced in the early 1990s for direct rendering of volume data. It was revitalized with 3D Gaussian Splatting (2023), which enables real-time rendering of photorealistic scenes learned from small image samples. Traditional AAA game rendering relies on polygon meshes and techniques like LOD and occlusion culling.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Gaussian_splatting">Gaussian splatting - Wikipedia</a></li>
<li><a href="https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/">3D Gaussian Splatting for Real-Time Radiance Field Rendering</a></li>
<li><a href="https://huggingface.co/blog/gaussian-splatting">Introduction to 3D Gaussian Splatting</a></li>

</ul>
</details>

**Discussion**: The community shows high engagement, with users expressing interest in AAA game adoption and asking for tutorials on point splatting. Some compare it to the 1994 game Ecstatica and question its ability to handle sharp features compared to mesh splatting.

**Tags**: `#computer graphics`, `#rendering`, `#3D splatting`, `#gaussian splatting`, `#real-time rendering`

---

<a id="item-5"></a>
## [AI Enthusiasts vs. Skeptics: A Race Against Time and Entropy](https://simonwillison.net/2026/Jun/4/ai-enthusiasts-ai-skeptics/#atom-everything) ⭐️ 8.0/10

Charity Majors published an analysis highlighting the conflicting pressures between AI enthusiasts racing to adopt AI for rapid capability gains and AI skeptics focused on preserving code quality, reliability, and institutional trust. This commentary captures a real, nuanced debate in software engineering that affects team dynamics, product quality, and long-term business viability. It underscores the need for organizational design that bridges the gap between these two perspectives. Majors argues that both groups are not wrong: enthusiasts see real capability leaps from AI, while skeptics warn of reliability degradation and loss of institutional knowledge. She recommends designing feedback loops to connect the two groups.

rss · Simon Willison · Jun 4, 23:55

**Background**: The article discusses the tension between rapid AI adoption and maintaining software engineering best practices. AI enthusiasts push for faster iteration and leveraging AI tools, while skeptics emphasize code review, testing, and documentation to prevent technical debt and system failures.

**Tags**: `#AI`, `#software engineering`, `#code quality`, `#technology adoption`

---

<a id="item-6"></a>
## [Tiger Brokers Halts New Positions for China Accounts from June 12](https://t.me/zaihuapd/41762) ⭐️ 8.0/10

Tiger Brokers announced that starting June 12, 2026, it will suspend new position openings and additional trades for all securities in mainland Chinese accounts, allowing only sell and close operations. Domestic fund transfers into accounts will also be halted, while withdrawals remain normal. This move signals the enforcement of China's crackdown on unlicensed cross-border securities services, affecting thousands of mainland investors using overseas brokerages. It highlights the regulatory push to contain capital outflows and ensure compliance with domestic securities laws. The suspension applies to all existing mainland Chinese accounts, but does not affect overseas services or the safety of existing assets. Investors can still hold, query, and sell their positions, and withdraw funds from their accounts.

telegram · zaihuapd · Jun 4, 07:51

**Background**: In May 2026, China's securities regulator and seven other departments jointly issued a notice to crack down on illegal cross-border securities, futures, and fund activities, setting a two-year rectification period. Overseas brokerages like Tiger Brokers and Futu were required to phase out services to mainland clients. This action is part of a broader effort to enforce the requirement that cross-border securities services be provided only by licensed institutions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.yicai.com/news/103212592.html">老虎国际：6月12日起，暂停存量投资者账户在中国境内所有品种的新开仓...</a></li>
<li><a href="https://www.csrc.gov.cn/csrc/c100028/c7634328/content.shtml">中国证监会有关部门负责人就《综合整治非法跨境证券期货基金经营活动...</a></li>
<li><a href="https://news.qq.com/rain/a/20260522A094J000">监管全面升级！跨境券商境内展业被全面取缔，协助展业者将被同步整顿_...</a></li>

</ul>
</details>

**Tags**: `#fintech`, `#regulation`, `#cross-border securities`, `#China`

---

<a id="item-7"></a>
## [DeepSeek tops US enterprise software charts as firms seek cheaper AI](https://www.scmp.com/tech/tech-trends/article/3355927/more-us-firms-turn-chinas-deepseek-over-pricey-silicon-valley-ai) ⭐️ 8.0/10

DeepSeek has topped Ramp's 'Hot Software Vendors' list in June 2026, as more US companies pay directly for its AI services, sending data to servers in China. The company also made its V4 Pro model's 75% price cut permanent and is nearing a $60 billion valuation in its first funding round. This marks a significant shift in the AI industry, as cost-conscious US enterprises increasingly adopt Chinese AI models over pricier Silicon Valley alternatives. DeepSeek's rise could pressure US AI providers to lower prices and accelerate open-source model adoption. DeepSeek's V4 Pro is a Mixture-of-Experts model with 1.6 trillion total parameters and 49 billion activated parameters, supporting a 1-million-token context window. Its permanent pricing is $0.435 per million input tokens and $0.87 per million output tokens, significantly cheaper than many competitors.

telegram · zaihuapd · Jun 4, 10:26

**Background**: DeepSeek is a Chinese AI company that develops large language models, gaining attention for its cost-effective open-source models. Ramp is a US enterprise spend management platform that tracks software vendor adoption among its 50,000+ customers. The trend reflects growing price sensitivity in enterprise AI adoption, with open-source models like DeepSeek challenging proprietary offerings from US tech giants.

<details><summary>References</summary>
<ul>
<li><a href="https://openrouter.ai/deepseek/deepseek-v4-pro">DeepSeek V4 Pro - API Pricing & Benchmarks | OpenRouter</a></li>
<li><a href="https://apidog.com/blog/deepseek-v4-pro-permanent-price-cut/">DeepSeek V4-Pro 75% Price Cut Is Now Permanent: What It Means ...</a></li>

</ul>
</details>

**Tags**: `#AI`, `#DeepSeek`, `#enterprise software`, `#cost optimization`, `#China tech`

---

<a id="item-8"></a>
## [Apple's New Siri to Use Google, Nvidia Chips for Cloud AI](https://www.macrumors.com/2026/06/04/apple-siri-rely-on-google-nvidia-chips/) ⭐️ 8.0/10

Apple's upcoming Siri, launching in September 2026, will route cloud-based AI queries to Google data centers powered by Nvidia Blackwell B200 chips, with data encrypted via Nvidia hardware. This marks a departure from Apple's tradition of using in-house hardware for core components. This strategic shift signals Apple's acknowledgment that its own silicon is insufficient for large-scale cloud AI, potentially reshaping its relationship with competitors Google and Nvidia. It also highlights the growing importance of cloud AI processing for consumer devices. The move is reportedly due to Apple's own servers being too slow to run Google's Gemini model. Apple will emphasize on-device AI at WWDC next week, and the new Siri is expected to reintroduce long-delayed personalized features.

telegram · zaihuapd · Jun 4, 11:37

**Background**: Apple Intelligence, launched in 2024, has received lukewarm reception, and Apple has been working to distill Google's massive Gemini model for on-device processing. However, running full Gemini on iPhone remains challenging, necessitating cloud support. Nvidia's Blackwell B200 GPU delivers up to 20 petaflops of FP4 compute, making it suitable for large AI workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Blackwell_(microarchitecture)">Blackwell (microarchitecture) - Wikipedia</a></li>
<li><a href="https://arstechnica.com/ai/2026/05/apple-reportedly-trying-to-distill-googles-multi-trillion-parameter-gemini-ai-to-run-on-iphone/">Apple working to cram massive Gemini model into iPhone to power new Siri - Ars Technica</a></li>
<li><a href="https://en.wikipedia.org/wiki/Apple_Intelligence">Apple Intelligence - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Siri`, `#AI`, `#Nvidia`, `#Google`

---

<a id="item-9"></a>
## [AI Agent Traffic Surpasses Human Traffic for First Time](https://www.tomshardware.com/tech-industry/artificial-intelligence/bots-have-now-passed-human-traffic-online-cloudflare-boss-laments-says-agentic-traffic-wasnt-expected-to-eclipse-real-people-until-next-year) ⭐️ 8.0/10

Cloudflare reports that AI agent traffic now accounts for 57.5% of web requests, surpassing human traffic for the first time, earlier than CEO Matthew Prince's 2027 prediction. This milestone signals a fundamental shift in internet usage, with implications for web infrastructure, bot detection, and cybersecurity, as AI agents increasingly perform tasks like price comparison and content retrieval. Cloudflare notes that while AI agents generate more page requests, humans still dominate total usage time, as streaming and social apps produce fewer requests per minute. The company's AI Crawl Control tool helps websites manage bot traffic.

telegram · zaihuapd · Jun 4, 16:49

**Background**: AI agents are automated programs that perform multi-step tasks like browsing, comparing prices, or answering customer service queries, mimicking human behavior. Cloudflare, a major content delivery network, has broad visibility into global web traffic and uses its AI Crawl Control to detect and manage such agents.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cnet.com/tech/services-and-software/its-official-agentic-bots-surf-the-web-more-than-real-people-do/">AI Agents Now Generate More Web Traffic Than Humans</a></li>
<li><a href="https://www.cloudflare.com/ai-crawl-control/">AI Crawl Control | Cloudflare</a></li>
<li><a href="https://matomo.org/blog/2026/03/humans-agents-understanding-ai-web-traffic/">From humans to AI agents: understanding the new web traffic</a></li>

</ul>
</details>

**Tags**: `#AI`, `#web traffic`, `#bots`, `#Cloudflare`, `#internet trends`

---

<a id="item-10"></a>
## [Google Removes 'Humans in the Loop' After Employee Memes](https://simonwillison.net/2026/Jun/4/a-slightly-different-version/#atom-everything) ⭐️ 7.0/10

Google removed the phrase 'it's critical that we maintain humans in the loop' from a statement after employees internally shared memes mocking the quality of the company's AI. This incident signals a potential shift in Google's commitment to human oversight in AI, raising concerns about transparency and ethical accountability in the industry. The original statement was published by 404 Media, and after the story broke, Google's spokesperson requested a revised version that no longer included the human-in-the-loop commitment.

rss · Simon Willison · Jun 4, 16:38

**Background**: The 'human-in-the-loop' approach involves human oversight in AI systems to ensure accuracy and ethical decision-making. It is widely considered a best practice, especially in high-stakes fields like healthcare. Google's removal of this commitment suggests a possible move toward more automated AI deployment.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48400311">Google employees internally share memes about how its AI sucks</a></li>

</ul>
</details>

**Discussion**: Hacker News commenters noted that the memes reflect internal frustration with Google's AI quality, with some arguing that the removal of human oversight is a worrying trend for AI ethics.

**Tags**: `#ai-ethics`, `#google`, `#ai`, `#journalism`

---

<a id="item-11"></a>
## [Uber Caps AI Coding Tool Usage to $1,500/Month Per Tool](https://simonwillison.net/2026/Jun/3/uber-caps-usage/#atom-everything) ⭐️ 7.0/10

Uber has implemented a $1,500 monthly spending cap per AI coding tool for all employees, after blowing its entire 2026 AI budget in just four months. The policy applies to agentic coding tools like Cursor and Anthropic's Claude Code. This is one of the first concrete examples of a major company imposing strict cost controls on AI coding tools, highlighting the tension between developer productivity gains and rapidly escalating token costs. It signals that enterprise AI adoption may require careful budgeting and usage governance. The $1,500 cap applies per tool, meaning an engineer using both Cursor and Claude Code could spend up to $3,000 per month. Uber's median software engineer compensation is $330,000, making the AI spending cap roughly 11% of that figure.

rss · Simon Willison · Jun 3, 12:01

**Background**: AI coding tools like Claude Code and Cursor are 'agentic' — they can understand entire codebases, edit files, and run commands autonomously. These tools consume tokens (units of AI computation) that are priced by providers like Anthropic and OpenAI. The rapid adoption of such tools has led to unexpected cost overruns at many companies.

<details><summary>References</summary>
<ul>
<li><a href="https://claude.com/product/claude-code">Claude Code by Anthropic | AI Coding Agent, Terminal, IDE</a></li>
<li><a href="https://www.zerohedge.com/ai/uber-introduces-1500-monthly-cap-ai-coding-tools-after-budget-blowout">Uber Introduces $1,500 Monthly Cap On AI Coding Tools ... | ZeroHedge</a></li>

</ul>
</details>

**Tags**: `#AI`, `#cost management`, `#enterprise`, `#coding agents`, `#Uber`

---

<a id="item-12"></a>
## [Sam Altman: OpenAI's top user consumes ~100B tokens monthly](https://www.businessinsider.com/sam-altman-openai-top-token-spender-ai-costs-issue-2026-6) ⭐️ 7.0/10

Sam Altman revealed that OpenAI's top internal user now consumes about 100 billion tokens per month, up from 100,000 tokens 6.5 years ago, and external users consume even more. He also noted that AI cost pressures have become a major issue in 2026. This data highlights the explosive growth in AI token usage, signaling both the increasing adoption of AI and the rising cost burden on providers like OpenAI. It underscores the need for more efficient models and cost management strategies across the industry. Altman mentioned that 6.5 years ago, 100,000 tokens per month was likely a global leading level, but now it is roughly the global per capita average. OpenAI has a culture of encouraging high token usage but is actively seeking ways to deliver more value at lower cost.

telegram · zaihuapd · Jun 4, 02:31

**Background**: Tokens are the basic units of text that AI models process; they can be words, parts of words, or characters. Higher token consumption indicates more extensive use of AI models for tasks like reasoning, generation, and analysis. As AI adoption grows, token usage has skyrocketed, leading to significant infrastructure and operational costs for providers.

<details><summary>References</summary>
<ul>
<li><a href="https://blogs.nvidia.com/blog/ai-tokens-explained/">What Are AI Tokens ? The Language and Currency... | NVIDIA Blog</a></li>
<li><a href="https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them">What are tokens and how to count them? | OpenAI Help Center</a></li>
<li><a href="https://help.openai.com/en/articles/6614209-how-do-i-check-my-token-usage">How do I check my token usage? - OpenAI Help Center</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI costs`, `#token usage`, `#Sam Altman`, `#industry trends`

---

<a id="item-13"></a>
## [WeChat Partners with Phone Makers for A2A Assistant](https://36kr.com/newsflashes/3838138218662404) ⭐️ 7.0/10

WeChat is collaborating with Huawei, Honor, Xiaomi, OPPO, and vivo to launch an Agent-to-Agent (A2A) capability that allows users to initiate voice or video calls and send messages via their phone's voice assistant. Honor's YOYO intelligent agent already supports this feature on select devices. This marks a significant step toward AI agent interoperability between major mobile platforms and a dominant messaging app, potentially setting a precedent for agent-to-agent communication in the ecosystem. It could enhance user convenience and drive adoption of voice-controlled interactions. The A2A capability is based on the open Agent2Agent protocol, initially introduced by Google in April 2025, which enables AI agents built on different frameworks to communicate. Currently, only Honor devices with updated YOYO agent and WeChat support the feature, with other manufacturers expected to follow.

telegram · zaihuapd · Jun 4, 04:53

**Background**: Agent-to-Agent (A2A) is an open communication protocol that allows AI agents from different platforms to collaborate and perform tasks together. Unlike MCP (Model Context Protocol), which focuses on connecting agents to tools, A2A enables direct agent-to-agent interaction. WeChat's integration with phone manufacturers' voice assistants exemplifies this protocol in a real-world consumer application.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/a2aproject/A2A">GitHub - a2aproject/A2A: Agent2Agent (A2A) is an open protocol enabling ...</a></li>
<li><a href="https://www.ibm.com/think/topics/agent2agent-protocol">What is A2A protocol (Agent2Agent)? - IBM</a></li>
<li><a href="https://min.news/en/tech/6076456ce940abc960efc06e75ca8a57.html">Magic OS 9 YOYO Intelligent Body The more AI understands you, the...</a></li>

</ul>
</details>

**Tags**: `#AI agents`, `#WeChat`, `#mobile assistants`, `#interoperability`, `#voice commands`

---

<a id="item-14"></a>
## [First Lychee-Longan Hybrid 'Huaishi' Bears Fruit](https://news.ycwb.com/ikimvkmtkh/content_54155752.htm) ⭐️ 7.0/10

Chinese researchers from the Guangdong Academy of Agricultural Sciences have successfully bred the world's first lychee-longan hybrid, named 'Huaishi', which has fruited for the first time in June 2025. The hybrid uses lychee as the maternal parent and longan as the paternal parent, breaking the intergeneric reproductive barrier. This breakthrough demonstrates the feasibility of intergeneric hybridization between lychee and longan, opening new possibilities for fruit breeding. The hybrid exhibits early ripening and superior taste, potentially offering economic benefits to growers and consumers. The parents are late-maturing lychee 'Huaizhi' and longan 'Shixia', but the hybrid shows early maturity, with crisp, sweet flesh and strong aroma. Currently in variety comparison trials, it is expected to reach the market in five to six years.

telegram · zaihuapd · Jun 4, 12:31

**Background**: Lychee and longan are closely related fruits in the Sapindaceae family, but they belong to different genera, making natural hybridization extremely rare due to reproductive isolation. Intergeneric hybridization requires overcoming barriers such as genetic incompatibility and hybrid sterility. The National Lychee Germplasm Resource Garden in Guangzhou, which preserves over 700 lychee accessions, provided the genetic resources for this research.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycwb.com/ikimvkmtkh/content_54155752.htm">今年首次挂果！荔枝龙眼杂交新品种“怀石”来了</a></li>
<li><a href="https://news.qq.com/rain/a/20260603A05W9400">全球首个！荔枝×龙眼杂交新品种“怀石”来了：是荔枝，却有龙眼味</a></li>
<li><a href="https://www.sohu.com/a/1032111060_99990677">令人振奋的消息：全球首个荔枝龙眼杂交品种“怀石”来了</a></li>

</ul>
</details>

**Tags**: `#agriculture`, `#biotechnology`, `#hybrid`, `#fruit breeding`, `#China`

---

<a id="item-15"></a>
## [US Bipartisan GUARD Act Targets Chinese Robot Imports](http://chinaselectcommittee.house.gov/media/press-releases/moolenaar-obernolte-mcclellan-introduce-legislation-to-ban-dangerous-chinese-robots) ⭐️ 7.0/10

US lawmakers introduced the GUARD Act, requiring a national security review of humanoid and quadruped robots from adversarial nations like China, with potential import restrictions. This bill could significantly impact Chinese robotics companies like Unitree, which is preparing for its IPO, and may reshape global robotics trade dynamics. The bill mandates a one-year review by national security agencies; if incomplete, the FCC automatically adds the robots to a 'covered list' restricting market access. Critics note potential conflicts of interest with US robotics firms like Agility Robotics.

telegram · zaihuapd · Jun 4, 13:16

**Background**: The GUARD Act (Guarding US Autonomy from Robotic Dominance) targets humanoid and quadruped robots from China, Russia, and other adversarial nations. It follows growing US concern over Chinese tech dominance and national security risks, though no public evidence supports claims of backdoors or remote hijacking.

<details><summary>References</summary>
<ul>
<li><a href="https://techmarketbriefs.com/pre-ipo/unitree/">Unitree Stock & IPO 2026: Valuation, Risks & Bull Case | TMB</a></li>
<li><a href="https://en.wikipedia.org/wiki/Agility_Robotics">Agility Robotics - Wikipedia</a></li>
<li><a href="https://www.cnbc.com/2025/09/09/chinas-unitree-plans-7-billion-ipo-valuation-as-humanoid-robot-race-heats-up.html">China’s Unitree heats up humanoid robot race as IPO ... - CNBC</a></li>

</ul>
</details>

**Tags**: `#geopolitics`, `#robotics`, `#trade policy`, `#China`, `#regulation`

---

<a id="item-16"></a>
## [ChatGPT Memory Upgrade: Auto-Learns Preferences, Stays Fresh](https://openai.com/index/chatgpt-memory-dreaming/) ⭐️ 7.0/10

OpenAI has rolled out a new memory system for ChatGPT that automatically learns user preferences from conversations and updates over time, starting with US Plus and Pro subscribers. This upgrade addresses a key limitation of the previous manual, static memory, making ChatGPT more personalized and context-aware without requiring explicit commands, which significantly improves user experience. The system uses a technique called 'dreaming' to automatically curate memories in the background by referencing chat history, and it can update memories dynamically—for example, stopping restaurant recommendations after a trip ends.

telegram · zaihuapd · Jun 4, 16:22

**Background**: ChatGPT's previous memory system required users to explicitly tell the model to remember something, and those memories remained static until manually changed. The new 'dreaming' architecture allows the model to reference past conversations automatically, supplementing the note-taking memory system.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/chatgpt-memory-dreaming/">Dreaming: Better memory for a more helpful ChatGPT - OpenAI</a></li>
<li><a href="https://www.makeuseof.com/chatgpt-now-remembers-your-preferences-automatically-and-it-actually-works/">ChatGPT now remembers your preferences automatically - MUO</a></li>
<li><a href="https://www.engadget.com/2187811/chatgpt-s-memory-is-getting-better-especially-if-you-re-on-the-free-tier/">ChatGPT's Memory Is Getting Better, Especially If You're On ...</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#memory`, `#AI`, `#product update`

---

<a id="item-17"></a>
## [US Tech Layoffs Hit 2-Year High in May, AI Cited as Top Reason](https://www.tomshardware.com/tech-industry/artificial-intelligence/tech-sector-cut-us-jobs-by-38242-in-may) ⭐️ 7.0/10

US tech sector announced 38,242 layoffs in May, the highest monthly total in nearly two years, with AI cited as the most common reason for the third consecutive month. This highlights a major industry shift where companies are reallocating budgets from traditional roles to AI infrastructure, potentially reshaping the tech job market and raising concerns about AI's impact on employment. Despite the layoffs, unemployment claims have not risen significantly, and tech giants' combined capital expenditure is projected at $725 billion this year, with about three-quarters directed to AI infrastructure.

telegram · zaihuapd · Jun 5, 01:00

**Background**: Tech layoffs have been rising in 2026 as AI investment surges. Some experts suggest companies may be 'AI-washing' layoffs, using AI as a convenient excuse for other factors like slowing demand or rising costs. Meanwhile, major cloud and AI providers are committing hundreds of billions to AI infrastructure, nearly doubling previous spending levels.

<details><summary>References</summary>
<ul>
<li><a href="https://futurumgroup.com/insights/ai-capex-2026-the-690b-infrastructure-sprint/">AI Capex 2026: The $690B Infrastructure Sprint - Futurum</a></li>
<li><a href="https://www.theguardian.com/technology/2026/apr/06/tech-layoffs-ai-work">Tech companies are cutting jobs and betting on AI . The... | The Guardian</a></li>

</ul>
</details>

**Tags**: `#tech layoffs`, `#AI impact`, `#job market`, `#capital expenditure`

---