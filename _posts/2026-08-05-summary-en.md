---
layout: default
title: "Horizon Summary: 2026-08-05 (EN)"
date: 2026-08-05
lang: en
---

> From 38 items, 21 important content pieces were selected

---

1. [Keyv and Related npm Packages Compromised in Active Shai-Hulud Supply Chain Attack](#item-1) ⭐️ 9.0/10
2. [Mistral's Shieldstral: 3B Open-Weights Multimodal Moderation Model](#item-2) ⭐️ 8.0/10
3. [DeepSeek V4 Flash Runs on Single AMD MI300X at 150+ tok/s](#item-3) ⭐️ 8.0/10
4. [Oxide Computer Raises $445M in Series D Funding](#item-4) ⭐️ 8.0/10
5. [MiniMax-H3 Runs on Apple Silicon via MLX Port](#item-5) ⭐️ 8.0/10
6. [Huawei Unveils Tau Scaling Law to Replace Moore's Law](#item-6) ⭐️ 8.0/10
7. [Cloudflare Ditches Third-Party Security Tools, Uses $58/Month AI for Bug Bounties](#item-7) ⭐️ 8.0/10
8. [Google Builds $200B Wall Street Financing Machine for Anthropic](#item-8) ⭐️ 8.0/10
9. [China's First Mandatory L3/L4 Autonomous Driving Standard Submitted for Approval](#item-9) ⭐️ 8.0/10
10. [New Color Space Simplifies Diverse Skin Tone Generation](#item-10) ⭐️ 7.0/10
11. [Stephen Wolfram's Heartfelt Tribute to Late Wife Elise Cawley](#item-11) ⭐️ 7.0/10
12. [Waymo Opens Driverless Ride-Hailing to All in Dallas](#item-12) ⭐️ 7.0/10
13. [FedEx's Legit Emails Fuel Phishing Confusion](#item-13) ⭐️ 7.0/10
14. [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and Smarter Logging](#item-14) ⭐️ 7.0/10
15. [Don't Be a Meat Proxy: Read, Understand, Validate AI Output](#item-15) ⭐️ 7.0/10
16. [LLMs Make Open Source Code Modification Practical](#item-16) ⭐️ 7.0/10
17. [Apple Approves Microsoft Request for iPhone-Windows Clipboard Sharing in EU](#item-17) ⭐️ 7.0/10
18. [Russia Mandates Third-Party App Stores on Apple Devices from September 2025](#item-18) ⭐️ 7.0/10
19. [US FCC Bans Imports of New Chinese Humanoid Robots and Inverters](#item-19) ⭐️ 7.0/10
20. [3D-Printed Biomimetic Corpus Cavernosum Restores Erectile Function in Pigs](#item-20) ⭐️ 7.0/10
21. [Nvidia CEO: US should use excellent Chinese open-source AI models](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Keyv and Related npm Packages Compromised in Active Shai-Hulud Supply Chain Attack](https://www.aikido.dev/blog/keyv-and-friends-compromised-in-npm-supply-chain-attack) ⭐️ 9.0/10

An active npm supply chain attack has compromised the popular Keyv package and related packages, with the self-replicating worm 'Shai-Hulud' poisoning hundreds of packages. The attack is ongoing and has prompted urgent community discussion on mitigation strategies. This attack affects a widely used package in the JavaScript ecosystem, potentially compromising developer and CI credentials across many projects. It underscores the fragility of the npm dependency system and highlights the need for stronger supply chain security measures. The Shai-Hulud worm has compromised over 500 packages, including 353 versions across 79 package names, and steals credentials while leaving repository hooks present. The attack exploits pre-install/post-install hooks, which the community is now calling to be restricted or removed.

hackernews · cimi_ · Aug 4, 11:01 · [Discussion](https://news.ycombinator.com/item?id=49166874)

**Background**: Keyv is a simple key-value storage library for Node.js with support for multiple backends, widely used in the npm ecosystem. Supply chain attacks like this one compromise legitimate packages to distribute malware, often through malicious install scripts, and can have cascading effects across the software supply chain.

<details><summary>References</summary>
<ul>
<li><a href="https://thehackernews.com/2026/08/keyv-linked-npm-worm-poisons-hundreds.html">Keyv-Linked npm Worm Poisons Hundreds of Packages, Plants Claude Code ...</a></li>
<li><a href="https://unit42.paloaltonetworks.com/npm-supply-chain-attack/">"Shai-Hulud" Worm Compromises npm Ecosystem in Supply Chain Attack (Updated November 26)</a></li>
<li><a href="https://www.cisa.gov/news-events/alerts/2025/09/23/widespread-supply-chain-compromise-impacting-npm-ecosystem">Widespread Supply Chain Compromise Impacting npm Ecosystem | CISA</a></li>

</ul>
</details>

**Discussion**: Community members expressed concern over the attack, with some calling for a moratorium on new pre-install/post-install hooks and others recommending the use of devcontainers for isolation. Tools like Packj were also mentioned for detecting supply chain attacks, and some users sought practical ways to check their node_modules for compromise.

**Tags**: `#security`, `#supply-chain`, `#npm`, `#open-source`, `#malware`

---

<a id="item-2"></a>
## [Mistral's Shieldstral: 3B Open-Weights Multimodal Moderation Model](https://mistral.ai/news/shieldstral/) ⭐️ 8.0/10

Mistral AI released Shieldstral, a 3B-parameter open-weights multimodal safety classifier, on August 4, 2026. It uses natural-language policy questions at inference time to judge text and images, outperforming models up to 7x its size. This release offers a cost-effective and flexible solution for content moderation, potentially enabling smaller platforms to implement robust safety measures. Its prompt-based policy allows customization without retraining, which could shift how moderation is deployed across the AI ecosystem. Shieldstral supports prompt moderation, response moderation, prompt-response pair classification, refusal detection, and safety filtering across text and image inputs. It returns a yes/no classification based on natural-language policy questions, and is available on Hugging Face.

hackernews · riadsila · Aug 4, 16:36 · [Discussion](https://news.ycombinator.com/item?id=49171268)

**Background**: Content moderation is critical for AI applications to prevent harmful outputs. Traditional moderation models rely on fixed harm categories, but Shieldstral's approach uses plain-language policies at inference time, offering greater flexibility. Mistral also provides a Moderation API and custom guardrails for developers.

<details><summary>References</summary>
<ul>
<li><a href="https://mistral.ai/news/shieldstral/">Introducing Shieldstral. | Mistral AI</a></li>
<li><a href="https://docs.mistral.ai/models/model-cards/shieldstral-1-0">Shieldstral 1.0 - docs.mistral.ai</a></li>
<li><a href="https://www.unite.ai/mistrals-shieldstral-packs-policy-adaptive-safety-screening-into-3b-parameters/">Mistral's Shieldstral Packs Policy-Adaptive Safety Screening Into 3B ...</a></li>

</ul>
</details>

**Discussion**: Community comments show interest in the model's flexibility, with questions about whether it can handle arbitrary rulesets beyond typical big-tech moderation styles. Some users are skeptical about real-world edge cases, while others see it as a practical solution for content moderation in their projects.

**Tags**: `#AI`, `#content moderation`, `#Mistral`, `#open-weights`, `#multimodal`

---

<a id="item-3"></a>
## [DeepSeek V4 Flash Runs on Single AMD MI300X at 150+ tok/s](https://github.com/ryanzhou/deepseek-v4-flash-mi300x) ⭐️ 8.0/10

A new guide demonstrates running DeepSeek V4 Flash on a single AMD MI300X GPU, achieving over 150 tokens per second with full weights and a 256k context window. This is significant because it shows that a large MoE model can be served efficiently on a single high-end GPU, potentially reducing hardware costs and making advanced LLMs more accessible to researchers and smaller organizations. The MI300X has 192GB of HBM3 memory, which is crucial for fitting the 284B-parameter model. The guide notes a tradeoff: the context window is reduced from the original 1M tokens to 256k, though this is still practical for many use cases.

hackernews · zhoutong · Aug 4, 10:00 · [Discussion](https://news.ycombinator.com/item?id=49166386)

**Background**: DeepSeek V4 Flash is a Mixture-of-Experts (MoE) language model with 284B total parameters but only 13B activated per token, making it efficient for inference. The AMD MI300X is a data center GPU with 192GB of HBM3 memory, designed for large AI workloads. Running such a large model on a single GPU requires careful memory management and optimization techniques.

<details><summary>References</summary>
<ul>
<li><a href="https://huggingface.co/deepseek-ai/DeepSeek-V4-Flash">deepseek-ai/DeepSeek-V4-Flash · Hugging Face</a></li>
<li><a href="https://www.amd.com/en/products/accelerators/instinct/mi300/mi300x.html">AMD Instinct™ MI300X Accelerators</a></li>
<li><a href="https://lenovopress.lenovo.com/lp1943-thinksystem-amd-mi300x-192gb-750w-8-gpu-board">ThinkSystem AMD MI300X 192GB 750W 8-GPU Board Product Guide > Lenovo Press</a></li>

</ul>
</details>

**Discussion**: Commenters noted that the MI300X is typically sold as an 8-GPU board, not as a single unit, and suggested the MI350P as a PCIe alternative with 144GB memory. Some also mentioned prior art like DwarfStar and questioned the context window tradeoff, though most agreed the 256k context is a practical compromise.

**Tags**: `#DeepSeek`, `#AMD MI300X`, `#LLM inference`, `#quantization`, `#hardware`

---

<a id="item-4"></a>
## [Oxide Computer Raises $445M in Series D Funding](https://www.sec.gov/Archives/edgar/data/1795071/000179507126000002/xslFormDX01/primary_doc.xml) ⭐️ 8.0/10

Oxide Computer has raised $445 million in a Series D funding round, according to an SEC Form D filing. This follows previous rounds of $44 million (Series A), $100 million (Series B), and $200 million (Series C). This significant funding milestone underscores investor confidence in Oxide's vision of building cloud-scale hardware and software. It could accelerate the company's product development and market adoption, potentially disrupting the traditional server and cloud infrastructure market. The funding was disclosed via an SEC Form D filing, indicating a private placement. The company has not yet publicly announced the round, and details on investors and valuation remain undisclosed. Community comments highlight both excitement and skepticism about product availability and sales responsiveness.

hackernews · depr · Aug 4, 20:13 · [Discussion](https://news.ycombinator.com/item?id=49174407)

**Background**: Oxide Computer is a hardware startup focused on building on-premise cloud infrastructure, offering a rack-scale system that integrates compute, storage, and networking. The company was co-founded by Bryan Cantrill and Adam Leventhal, known for their work at Sun Microsystems and Joyent. Their product aims to provide a more manageable and cost-effective alternative to traditional cloud providers.

**Discussion**: Community sentiment is mixed: some express excitement about the company's progress and product concept, while others question whether Oxide actually ships hardware and note poor sales responsiveness. One commenter mentioned filling out a sales form and never hearing back, despite significant AWS spending. Overall, there is admiration for the team but skepticism about execution.

**Tags**: `#funding`, `#hardware`, `#startup`, `#Oxide Computer`

---

<a id="item-5"></a>
## [MiniMax-H3 Runs on Apple Silicon via MLX Port](https://simonwillison.net/2026/Aug/4/minimax-h3-mlx/#atom-everything) ⭐️ 8.0/10

Simon Willison demonstrated running MiniMax's new omni-modal MiniMax-H3 model on Apple Silicon using an MLX port, PipeNetwork/minimax-h3-mlx. He successfully generated a 15-second video clip with audio from a text prompt on his M5 Max MacBook Pro. This enables developers to run a state-of-the-art omni-modal generative model locally on Apple Silicon, reducing reliance on cloud APIs and enabling offline experimentation. It highlights the growing ecosystem of MLX ports for advanced AI models, making them more accessible to the Apple developer community. The model requires downloading approximately 115 GB of model files, and video generation took just under 45 minutes on the M5 Max. The generated audio was described as 'weird speech-like garbage' because no audio prompt guidance was provided, but the prompting guide offers tips for better results.

rss · Simon Willison · Aug 4, 19:10

**Background**: MiniMax-H3 is a general-purpose omni-modal generative system that accepts text, images, audio, and video inputs and can generate up to 15-second video clips with native stereo audio at up to 2K resolution. MLX is an array framework from Apple designed for efficient machine learning on Apple Silicon, and this port leverages it to run the model locally.

<details><summary>References</summary>
<ul>
<li><a href="https://www.minimax.io/blog/minimax-h3">MiniMax H3: An Open Model Breaking the Boundaries Between Tasks and ...</a></li>
<li><a href="https://kylon.io/blog/minimax-h3-guide-2026">MiniMax H3 Guide: Open-Weight Multimodal Video, API, and License</a></li>
<li><a href="https://opensource.apple.com/projects/mlx/">Apple Open Source</a></li>

</ul>
</details>

**Tags**: `#MLX`, `#MiniMax-H3`, `#omni-modal`, `#Apple Silicon`, `#video generation`

---

<a id="item-6"></a>
## [Huawei Unveils Tau Scaling Law to Replace Moore's Law](https://t.me/zaihuapd/42966) ⭐️ 8.0/10

At the 2026 IEEE International Symposium on Circuits and Systems (ISCAS) in Shanghai, Huawei's HiSilicon president He Tingbo unveiled the 'Tau (τ) Scaling Law,' proposing time-based scaling to replace geometric scaling in semiconductors. Huawei claims to have designed and mass-produced 381 chips using this principle over the past six years, with a new Kirin smartphone chip using LogicFolding technology expected this fall. This announcement is significant because it proposes a post-Moore paradigm that could extend semiconductor progress beyond physical limits, potentially reshaping the industry. It also signals Huawei's strategic move to bypass EUV restrictions and achieve 1.4nm-equivalent transistor density by 2031, which could alter the competitive landscape in chips. The Tau Scaling Law focuses on reducing the time constant (τ) across devices, circuits, chips, and systems for multi-layer co-optimization. Huawei projects that by 2031, chips based on this law will achieve transistor density equivalent to 1.4nm processes, with a claimed 55% higher density than conventional scaling. The LogicFolding architecture folds transistor-level logic into vertical layers, requiring new design tools, such as a 3D chip design tool developed by Peking University.

telegram · zaihuapd · Aug 4, 08:04

**Background**: Moore's Law, which predicts that transistor density doubles roughly every two years, is approaching physical limits due to challenges in geometric scaling. Time scaling offers an alternative by optimizing the time constant rather than physical dimensions. Huawei's proposal is part of a broader trend exploring post-Moore computing paradigms, and it leverages China's push for semiconductor self-sufficiency amid export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/5/ieee-iscas-tau-scaling">HUAWEI Presents the Tau (τ) Scaling Law, Enabling Breakthroughs in Transistor Density and System Performance - Huawei</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/semiconductors/huawei-claims-sanctions-busting-breakthrough-with-1-4nm-class-chips-by-2031-claims-55-percent-higher-transistor-density-firm-claims-new-logicfolding-chip-architecture-can-bypass-euv-restrictions-introduces-tau-scaling-law-to-replace-moores-law">Huawei claims sanctions-busting breakthrough with 1.4nm-class chips by 2031, claims 55% higher transistor density — firm claims new LogicFolding chip architecture can bypass EUV restrictions, introduces 'Tau Scaling Law' to replace Moore's Law | Tom's Hardware</a></li>
<li><a href="https://qz.com/huawei-logicfolding-chip-design-tau-scaling-052626">Huawei LogicFolding chip design aims to match 1.4nm by 2031</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#Huawei`, `#Moore's Law`, `#chip design`, `#technology`

---

<a id="item-7"></a>
## [Cloudflare Ditches Third-Party Security Tools, Uses $58/Month AI for Bug Bounties](https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600) ⭐️ 8.0/10

Cloudflare's CSO Grant Bourzikas revealed at a Sydney conference that the company has automated vulnerability bounty report triage using Anthropic's Claude Sonnet model, costing only $58 per month, compared to about $200,000 per month if using the security-specific Mythos model. Cloudflare has also built over 200 autonomous security agents, replacing almost all third-party security tools with self-developed applications partly written with AI assistance. This demonstrates a significant cost reduction and efficiency gain in security operations through AI automation, potentially reshaping how enterprises approach security tooling. It also highlights the growing role of AI in security, but Cloudflare's cautionary advice suggests that such a strategy may not be universally applicable. The cost comparison is stark: $58/month for Claude Sonnet versus $200,000/month for Mythos, a security-specific model. Cloudflare's CSO advised other companies not to follow suit, noting that not every bank should develop all its own software. Additionally, Cloudflare's chief strategy officer attributed the company's 1,100-person layoff to AI-driven automation and mentioned plans to act as an intermediary between AI companies and publishers for micropayments.

telegram · zaihuapd · Aug 4, 09:24

**Background**: Cloudflare is a major web infrastructure and security company. Vulnerability bounty programs reward security researchers for finding and reporting bugs. AI models like Claude Sonnet can be used to triage these reports by deduplicating and assessing their value. Mythos is Anthropic's advanced AI model with strong security capabilities, but it is much more expensive to run. Cloudflare's move reflects a broader trend of using AI to automate security operations, but its scale and engineering expertise are not typical.

<details><summary>References</summary>
<ul>
<li><a href="https://www.theregister.com/security/2026/08/04/cloudflare-has-mostly-ditched-third-party-security-tools-suggests-not-trying-that-at-home/5282600">Cloudflare has mostly ditched third party security tools, suggests not trying that at home</a></li>
<li><a href="https://www.contrastsecurity.com/glossary/mythos-ai">What Is Mythos AI? Autonomous Exploits and AppSec Defense | Contrast Security</a></li>
<li><a href="https://www.endorlabs.com/learn/what-is-mythos-and-why-it-matters-for-software-security">What Is Mythos and Why It Matters for Software Security | Blog | Endor Labs</a></li>

</ul>
</details>

**Tags**: `#AI`, `#security`, `#Cloudflare`, `#automation`, `#vulnerability management`

---

<a id="item-8"></a>
## [Google Builds $200B Wall Street Financing Machine for Anthropic](https://www.ft.com/content/549f2e23-5aa2-49c7-9ea6-a9784ab7087c) ⭐️ 8.0/10

Google has quietly assembled a massive financing structure worth approximately $200 billion to deliver over $150 billion in AI chips to Anthropic. The structure involves partners like Broadcom, Apollo, Blackstone, and Morgan Stanley, using a vendor-financing model to spread risk. This is one of the largest infrastructure financing deals in history, enabling Anthropic to scale its AI compute without a credit rating. It sets a precedent for how AI companies can secure massive compute resources while offloading balance-sheet risk to financial partners. In June, the special-purpose vehicle Compute SPV completed its first transactions, purchasing about $35 billion in hardware, equivalent to roughly 1 gigawatt of compute and 1 million TPUs. The model is inspired by vendor financing used by Boeing and GE for aircraft and engines, with Google guaranteeing data centers, Broadcom buying and financing chips, and Apollo and Blackstone purchasing hardware to lease back to Anthropic.

telegram · zaihuapd · Aug 4, 10:52

**Background**: Vendor financing is a credit arrangement where the seller of an asset provides a loan to the buyer, often used to facilitate large purchases. In this case, Google and its partners use a similar model to spread the financial risk of building AI infrastructure across multiple parties, avoiding any single company bearing the full cost on its balance sheet. TPUs (Tensor Processing Units) are Google's custom AI chips designed to accelerate machine learning workloads.

<details><summary>References</summary>
<ul>
<li><a href="https://nucleuscommercialfinance.com/finance-glossary/vendor-finance/">Vendor Finance | What is Vendor Finance for Business?</a></li>
<li><a href="https://aiwiki.ai/wiki/tpu_chip">TPU Chip | AI Wiki</a></li>

</ul>
</details>

**Tags**: `#AI infrastructure`, `#Google`, `#Anthropic`, `#finance`, `#chips`

---

<a id="item-9"></a>
## [China's First Mandatory L3/L4 Autonomous Driving Standard Submitted for Approval](https://t.me/zaihuapd/42972) ⭐️ 8.0/10

China's Ministry of Industry and Information Technology (MIIT) has completed the draft of the mandatory national standard 'Safety Requirements for Intelligent Connected Vehicle Autonomous Driving Systems' and started public consultation on June 17. The standard is recommended to take effect on July 1, 2027, marking China's first mandatory standard for L3 and L4 autonomous driving. This standard shifts regulation from vague concept promotion to hard safety constraints, requiring automakers to systematically prove safety via a Safety Case mechanism. It will significantly impact the autonomous driving industry in China, affecting vehicle design, marketing, and compliance strategies. The standard applies to M and N category vehicles equipped with L3 or L4 systems, excluding automated parking systems. For L3, it requires driver takeover capability monitoring; for L4, it includes specific requirements for autonomous risk handling and considers scenarios like standing passengers.

telegram · zaihuapd · Aug 4, 13:06

**Background**: Autonomous driving levels range from L0 to L5, with L3 being conditional automation where the driver must be ready to take over, and L4 being high automation where the system can handle most situations without driver intervention. China has been developing regulations for intelligent connected vehicles, and this standard is a key step in establishing mandatory safety requirements for higher levels of automation.

<details><summary>References</summary>
<ul>
<li><a href="https://www.autohome.com.cn/news/202608/1316205.html">autohome.com.cn/news/202608/1316205.html</a></li>
<li><a href="https://chedongxi.com/p/370544.html">车企营销不能再“乱吹”了！ 自 动 驾 驶 国标出台，明年7月实施 - 车东西</a></li>
<li><a href="https://www.ithome.com/0/985/665.htm">ithome.com/0/985/665.htm</a></li>

</ul>
</details>

**Tags**: `#autonomous driving`, `#regulation`, `#China`, `#safety standard`, `#L3/L4`

---

<a id="item-10"></a>
## [New Color Space Simplifies Diverse Skin Tone Generation](https://toneyalexander.github.io/inclusive-color-space/) ⭐️ 7.0/10

The author introduces a custom color space and algorithm for generating diverse, plausible skin tones, along with interactive demos and detailed explanations. The project includes a JavaScript color picker and a Python procedural generation algorithm. This addresses a practical challenge in digital art and game development, where selecting realistic skin tones is often difficult. The approach could streamline workflows and inspire further research in color science for human-centric applications. The color space is constructed by fitting functions to data, rather than using PCA, and the author acknowledges the methodology is 'shaky' with room for improvement. The page includes a 'Future Work' section and various JavaScript demos.

hackernews · automatoney · Aug 4, 15:16 · [Discussion](https://news.ycombinator.com/item?id=49170165)

**Background**: Skin tone representation in digital media is complex due to human perception and lighting. Traditional color spaces like RGB or HSV are not intuitive for skin tones, and existing approaches like Pantone Skin Tones exist but are not referenced. The project aims to create a dedicated space for this purpose.

<details><summary>References</summary>
<ul>
<li><a href="https://toneyalexander.github.io/inclusive-color-space/">What Colors Are We? Constructing A Color Space For Skin Tones</a></li>

</ul>
</details>

**Discussion**: Comments praise the work for its elegance and the function-fitting approach, while noting the complexity of skin color modeling. Some suggest referencing Pantone Skin Tones and mention that skin tones form a crescent shape in Oklab, which aligns with the article. One commenter observes green, blue, and purple hues in the generated colors, questioning their plausibility.

**Tags**: `#color science`, `#procedural generation`, `#digital art`, `#skin tone`, `#algorithm`

---

<a id="item-11"></a>
## [Stephen Wolfram's Heartfelt Tribute to Late Wife Elise Cawley](https://writings.stephenwolfram.com/2026/08/in-memory-of-my-wife-elise-cawley-1961-2026-with-thanks-for-36-wonderful-years/) ⭐️ 7.0/10

Stephen Wolfram published a deeply personal tribute to his late wife, Elise Cawley (1961–2026), reflecting on their 36 years together and expressing gratitude for their shared life. This tribute offers the tech community a rare glimpse into the personal life of a prominent figure, fostering empathy and connection. It highlights the human side of innovation and resonates with many who have experienced loss. The tribute is noted for its remarkable detail, suggesting Wolfram may have kept a journal or possesses an exceptional memory. Community comments praise its sincerity and emotional depth, transcending his usual writing style.

hackernews · jdcampolargo · Aug 4, 18:51 · [Discussion](https://news.ycombinator.com/item?id=49173165)

**Background**: Stephen Wolfram is a renowned computer scientist, physicist, and creator of Mathematica and Wolfram Alpha. Elise Cawley was his wife for 36 years, and her passing prompted this personal reflection, which has drawn significant community engagement.

**Discussion**: Community comments express deep sympathy and admiration, with many noting the tribute's emotional power and sincerity. Some share personal experiences of loss, while others highlight how the piece transcends Wolfram's typical writing style.

**Tags**: `#tribute`, `#Stephen Wolfram`, `#personal`, `#community`, `#obituary`

---

<a id="item-12"></a>
## [Waymo Opens Driverless Ride-Hailing to All in Dallas](https://waymo.com/blog/shorts/dallas-open-to-all/) ⭐️ 7.0/10

Waymo has officially opened its driverless ride-hailing service to the general public in Dallas, Texas, marking another major city expansion for the autonomous vehicle company. The service is now available to all users in the Dallas area, following earlier launches in other cities. This expansion is significant as it brings autonomous ride-hailing to one of the largest and most car-dependent metro areas in the US, potentially reshaping urban mobility and reducing reliance on personal vehicles. It also signals Waymo's continued scaling and competitive positioning in the autonomous vehicle industry. Dallas is known for its low density, high sprawl, and limited public transit, making it a challenging environment for autonomous vehicles. The service will likely face tests from extreme weather conditions, such as heat and sudden weather shifts, which could affect vehicle durability and sensor reliability.

hackernews · xnx · Aug 4, 18:29 · [Discussion](https://news.ycombinator.com/item?id=49172836)

**Background**: Waymo is a subsidiary of Alphabet Inc. and operates the world's first autonomous ride-hailing service, having served over 20 million rides with a 93% satisfaction rate. The company has been expanding to multiple cities, including San Francisco, Phoenix, and Los Angeles, and plans to launch in London by 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://waymo.com/">Waymo - Self-Driving Cars - Autonomous Vehicles - Ride - Hail</a></li>
<li><a href="https://manufacturingcurated.com/automotive-and-aerospace/waymos-driverless-robotaxis-dallas-expansion-by-2026/">Waymo's Driverless Robotaxis: Dallas Expansion by 2026?</a></li>
<li><a href="https://www.roadtoautonomy.com/waymo-drives-autonomously-dallas/">Waymo Drives Autonomously into Dallas | The Road to Autonomy</a></li>

</ul>
</details>

**Discussion**: Community comments highlight diverse perspectives: some see driverless cars as an effective affordable housing policy by reducing transportation costs, while others express concerns about local economic impacts, such as money leaving the local economy. Many users report positive experiences with Waymo, noting its safety and predictability compared to human drivers, though some mention occasional incidents where vehicles get stuck.

**Tags**: `#autonomous vehicles`, `#Waymo`, `#transportation`, `#urban planning`, `#AI`

---

<a id="item-13"></a>
## [FedEx's Legit Emails Fuel Phishing Confusion](https://www.troyhunt.com/thanks-fedex-this-is-why-we-keep-getting-phished/) ⭐️ 7.0/10

Troy Hunt's article highlights how FedEx's legitimate email practices, such as sending unsolicited customs notices with attachments, make it harder for users to distinguish real communications from phishing scams. The piece uses real-world examples to illustrate the ongoing challenge of email security. This matters because it shows that even reputable companies inadvertently train users to accept risky email behaviors, increasing overall susceptibility to phishing. It underscores the need for better email authentication standards and user education to combat social engineering attacks. The article references FedEx sending customs notices via plain email with PDF attachments, which mirrors common phishing tactics. Community comments also mention similar issues with other organizations like the IRS, and the proliferation of new gTLDs like .xyz complicates domain trust.

hackernews · stymaar · Aug 4, 21:09 · [Discussion](https://news.ycombinator.com/item?id=49175192)

**Background**: Phishing is a form of social engineering where attackers impersonate legitimate entities to trick victims into revealing sensitive information or clicking malicious links. Email remains a primary vector, with over 70% of data breaches starting with phishing or social engineering attacks. Companies like FedEx often send legitimate but poorly formatted emails, which attackers mimic, making it difficult for users to tell real from fake.

<details><summary>References</summary>
<ul>
<li><a href="https://www.mailguard.com.au/blog/dont-fall-for-this-fraudulent-fedex-phishing-email">Don’t fall for this fraudulent FedEx phishing email</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC6334892/">Email fraud: The search for psychological predictors of susceptibility ...</a></li>
<li><a href="https://www.kaspersky.com/resource-center/definitions/what-is-social-engineering">What is Social Engineering ? - Meaning</a></li>

</ul>
</details>

**Discussion**: Community comments share personal experiences with FedEx and other organizations, highlighting the confusion caused by legitimate emails that look like phishing. Some users point out the difficulty of verifying domains like c.gle, and others note that new gTLDs worsen the problem. Overall sentiment is frustration with current email security practices.

**Tags**: `#phishing`, `#security`, `#email`, `#FedEx`, `#social engineering`

---

<a id="item-14"></a>
## [LLM 0.32 Adds Reasoning Traces, Server-Side Tools, and Smarter Logging](https://simonwillison.net/2026/Aug/4/new-release-of-llm/#atom-everything) ⭐️ 7.0/10

LLM 0.32, released on August 4, 2026, introduces visible reasoning traces for reasoning models, server-side tools from providers like OpenAI and Anthropic, redesigned content-addressable SQLite logs, and support for the GPT-5.6 model family with a new default model, GPT-5.6 Luna. It also adds the 'llm openai endpoint' command for one-off prompts against any OpenAI-compatible endpoint. This update significantly enhances the LLM CLI tool, aligning with current AI trends by supporting reasoning traces and server-side tools, which are crucial for building agentic applications. It improves user experience for developers and power users who rely on LLM for interacting with various models, potentially increasing adoption and productivity. Reasoning traces are displayed to standard error by default, with a -R/--hide-reasoning flag to disable. Server-side tools include OpenAI's CodeInterpreter and WebSearch, and Anthropic's WebSearch, WebFetch, CodeExecution, and AnthropicMCP, which can be used via command-line flags. The content-addressable SQLite logs are redesigned for more efficient storage and retrieval.

rss · Simon Willison · Aug 4, 23:58

**Background**: LLM is a command-line tool for interacting with large language models, developed by Simon Willison. It supports various providers and plugins, allowing users to run prompts and integrate tools. The OpenAI Responses API, released in March 2025, simplifies agentic applications by combining chat completions with advanced tool-calling capabilities. Content-addressable storage (CAS) is a method where data is retrieved based on its content rather than its location, which can improve efficiency and deduplication.

<details><summary>References</summary>
<ul>
<li><a href="https://llm.datasette.io/en/stable/usage.html">Usage - LLM</a></li>
<li><a href="https://simonwillison.net/2025/May/27/llm-tools/">Large Language Models can run tools in your terminal with LLM 0.26</a></li>
<li><a href="https://developers.openai.com/api/reference/responses/overview">Responses Overview | OpenAI API Reference</a></li>

</ul>
</details>

**Tags**: `#LLM`, `#CLI`, `#AI`, `#OpenAI`, `#release`

---

<a id="item-15"></a>
## [Don't Be a Meat Proxy: Read, Understand, Validate AI Output](https://simonwillison.net/2026/Aug/3/dont-be-a-meat-proxy/#atom-everything) ⭐️ 7.0/10

Niklas Gruhn coined the term 'meat proxy' to describe people who blindly relay AI output without understanding it. He urges users to read, understand, validate, and rewrite AI responses in their own words. This term highlights a common misuse of AI that undermines professional value and trust. It encourages a more thoughtful integration of AI, promoting accountability and quality in communication. The term was introduced in a blog post by Niklas Gruhn on August 3, 2026, and was highlighted by Simon Willison. The advice emphasizes that adding personal effort is a 'certificate' of having done the necessary validation steps.

rss · Simon Willison · Aug 3, 23:45

**Background**: Large language models (LLMs) generate text that can be fluent but may contain errors or biases. Blindly copying AI output without verification can spread misinformation and reduce the value of human expertise. The term 'meat proxy' draws an analogy to a proxy server that simply forwards data without processing it.

<details><summary>References</summary>
<ul>
<li><a href="https://simonwillison.net/2026/Aug/3/dont-be-a-meat-proxy/">Don't be a meat proxy | Simon Willison’s Weblog</a></li>
<li><a href="https://www.remio.ai/post/simon-willison-says-dont-be-a-meat-proxy-for-ai">Simon Willison Says Don't Be a Meat Proxy for AI</a></li>
<li><a href="https://techplanet.today/post/the-meat-proxy-problem-why-blindly-forwarding-ai-output-undermines-professional-value">The Meat Proxy Problem: Why Blindly Forwarding AI ... | TechPlanet</a></li>

</ul>
</details>

**Discussion**: The Lobste.rs discussion validated the concept, with some noting that the term could be misused to shame junior employees or non-native speakers. Others emphasized using it to diagnose workflows rather than blame individuals.

**Tags**: `#AI`, `#LLMs`, `#AI ethics`, `#productivity`, `#definitions`

---

<a id="item-16"></a>
## [LLMs Make Open Source Code Modification Practical](https://simonwillison.net/2026/Aug/3/devtools-must-be-open-source-exedev/#atom-everything) ⭐️ 7.0/10

Simon Willison argues that LLMs lower the friction of examining and modifying open source code, making the open source ideal more practical. He describes using Claude and Codex to clone, build, and understand projects with minimal time investment. This shift could democratize code contribution and customization, enabling more developers to engage with open source projects. It may accelerate innovation and broaden participation in software development. Willison notes that getting software to compile was previously a major barrier, but now he treats it as a zero-time investment by delegating to AI tools. He admits he is not yet habitually modifying software, but sees a clear path forward.

rss · Simon Willison · Aug 3, 15:30

**Background**: Open source software grants users the freedom to examine and modify code, but in practice, the time required to understand and build projects has limited this to a few experts. LLMs can assist in navigating codebases, explaining functionality, and automating build processes, thereby reducing the barrier to entry.

**Discussion**: The Hacker News discussion likely includes agreement on the practical benefits of LLMs for open source engagement, with some users sharing their own experiences and others expressing concerns about over-reliance on AI. Overall sentiment appears positive, recognizing the potential for increased participation.

**Tags**: `#open source`, `#LLMs`, `#developer tools`, `#workflow`

---

<a id="item-17"></a>
## [Apple Approves Microsoft Request for iPhone-Windows Clipboard Sharing in EU](https://appleinsider.com/articles/26/08/04/iphone-to-windows-clipboard-sharing-coming-to-ios-28-in-the-eu) ⭐️ 7.0/10

Apple has approved Microsoft's interoperability request to develop cross-device clipboard sharing between iPhone and Windows PCs, expected to launch with iOS 28 in fall 2027 for EU users. The feature will allow users to copy on one device and paste on the other without third-party apps. This marks a significant step in cross-platform interoperability driven by the EU's Digital Markets Act (DMA), potentially improving user workflows and reducing reliance on third-party solutions. It could set a precedent for other interoperability requests between major tech ecosystems. Microsoft submitted the request on March 25, 2026, and it was approved on June 26, 2026. Apple's implementation will use the AccessorySetupKit framework for one-time pairing authorization, similar to the accessory notification framework in iOS 26.5. The feature is initially EU-only, but Apple hasn't ruled out a global rollout.

telegram · zaihuapd · Aug 4, 03:15

**Background**: The EU's Digital Markets Act (DMA) requires designated 'gatekeepers' like Apple to allow third parties access to the same OS hardware and software features available to their own services. Article 6(7) of the DMA specifically mandates interoperability for such features. AccessorySetupKit is a framework introduced by Apple at WWDC24 that provides a streamlined, privacy-friendly way for apps to set up and manage Bluetooth and Wi-Fi accessories.

<details><summary>References</summary>
<ul>
<li><a href="https://digital-markets-act.ec.europa.eu/developer-portal/interoperability_en">Interoperability - Digital Markets Act (DMA) - European Commission</a></li>
<li><a href="https://developer-mdn.apple.com/videos/play/wwdc2024/10203/">Meet AccessorySetupKit - WWDC24 - Videos - Apple Developer</a></li>
<li><a href="https://www.macworld.com/article/3205820/apple-is-finally-making-copy-paste-work-between-iphones-and-pcs.html">The feature is currently scheduled as part of iOS 28 in the EU.</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#Microsoft`, `#iOS`, `#Interoperability`, `#DMA`

---

<a id="item-18"></a>
## [Russia Mandates Third-Party App Stores on Apple Devices from September 2025](https://t.me/zaihuapd/42963) ⭐️ 7.0/10

The Russian State Duma passed a new law requiring Apple devices, including iPhone and iPad, to allow installation of third-party app stores like RuStore starting September 1, 2025. The law prohibits Apple and Google from setting installation restrictions or barriers. This regulation challenges Apple's and Google's control over app distribution, potentially setting a precedent for other countries to mandate third-party app stores. It could significantly impact the app store monopoly and force platform holders to alter their business models in Russia. The law also prohibits manufacturers from restricting installation and updates of third-party software, blocking alternative software functions, forcing developers to set prices, or limiting payment methods. RuStore is a Russian app store created by VK with support from the Ministry of Digital Development, pre-installed on Android devices since 2023.

telegram · zaihuapd · Aug 4, 05:25

**Background**: Russia has been pushing for domestic apps on devices sold in the country since 2019, when a law required device makers to offer domestic apps. Apple and Russian authorities have been in a slow-boiling dispute, with Russia opening antitrust proceedings against Apple for failing to preinstall state-backed apps like RuStore and MAX messenger.

<details><summary>References</summary>
<ul>
<li><a href="https://9to5mac.com/2026/08/03/russia-escalates-dispute-with-apple-over-mandatory-app-preinstallation/">Russia escalates dispute with Apple over mandatory app ... - 9to5Mac</a></li>
<li><a href="https://www.msn.com/en-us/news/other/russia-wants-its-apps-on-your-iphone-and-now-it-s-hauling-apple-into-court/ar-AA29nHlM">Russia wants its apps on your iPhone — and now it’s hauling Apple ...</a></li>
<li><a href="https://www.rustore.ru/en">RuStore is the official app store for Android and Harmony OS</a></li>

</ul>
</details>

**Tags**: `#regulation`, `#app store`, `#Apple`, `#Russia`, `#policy`

---

<a id="item-19"></a>
## [US FCC Bans Imports of New Chinese Humanoid Robots and Inverters](https://t.me/zaihuapd/42970) ⭐️ 7.0/10

On July 28, the US Federal Communications Commission (FCC) announced measures banning the import of new Chinese humanoid robots, quadruped robots, and connected power inverters, effective immediately for models not yet released. This move signals escalating US-China tech decoupling, directly impacting the robotics and AI infrastructure supply chains. It could force companies to seek alternative suppliers and may set a precedent for broader restrictions on Chinese tech products. The ban applies only to new models not yet on the market, and the FCC is expected to exempt many non-Chinese suppliers. However, the agency retains authority to revoke authorization for models already approved for sale in the US.

telegram · zaihuapd · Aug 4, 11:29

**Background**: The FCC is an independent US agency regulating communications and technology. Power inverters convert DC to AC electricity, commonly used in solar and battery systems; connected inverters can be networked, posing potential cybersecurity risks. Humanoid and quadruped robots are advanced robotics products often used in industrial and research settings.

<details><summary>References</summary>
<ul>
<li><a href="https://www.kizpow.com/xingyezixun/2568.html">kizpow.com/xingyezixun/2568.html</a></li>
<li><a href="https://ouluwind.com/baike/569.html">ouluwind.com/baike/569.html</a></li>

</ul>
</details>

**Tags**: `#US-China`, `#robotics`, `#regulation`, `#AI`, `#supply chain`

---

<a id="item-20"></a>
## [3D-Printed Biomimetic Corpus Cavernosum Restores Erectile Function in Pigs](https://doi.org/10.1016/j.biomaterials.2026.124491) ⭐️ 7.0/10

A study published in Biomaterials used 3D printing to fabricate a hydrogel-based biomimetic corpus cavernosum with a sinusoidal architecture, seeded with umbilical cord-derived mesenchymal stem cells, and successfully restored erectile function in a pig model. This represents a significant advancement in regenerative medicine for erectile dysfunction (ED), offering a potential alternative to symptomatic treatments that could fundamentally repair damaged tissue. If translated to humans, it could benefit millions of men worldwide who suffer from ED, especially those with severe penile injuries. The study employed single-cell sequencing to reveal the mechanism: stem cells promote endothelial differentiation to rebuild vascular networks, reduce TGF-β secretion to inhibit endothelial-to-mesenchymal transition, and modulate the immune environment by activating anti-inflammatory IL-10. The biomimetic structure can simulate penile erection under fluid pressure in vitro.

telegram · zaihuapd · Aug 4, 13:52

**Background**: Erectile dysfunction (ED) is a common condition where men have difficulty achieving or maintaining an erection. Traditional treatments include oral medications, injections, or surgery, but these often only manage symptoms rather than repair the underlying structural damage. The corpus cavernosum is the erectile tissue in the penis that fills with blood during erection. 3D bioprinting is a technology that creates three-dimensional structures layer by layer using bio-inks, often combined with living cells, to produce tissue-like constructs for regenerative medicine.

<details><summary>References</summary>
<ul>
<li><a href="https://pubmed.ncbi.nlm.nih.gov/42546581/">Development and mechanistic investigation of 3 D - printed biomimetic ...</a></li>
<li><a href="https://www.livescience.com/health/scientists-invent-3d-printed-penis-implant-to-restore-erections-and-it-works-in-rabbits-and-pigs">Scientists invent 3 D - printed penis implant to restore... | Live Science</a></li>
<li><a href="https://www.dailymail.com/sciencetech/article-14472861/3D-printed-PENIS-used-cure-erectile-dysfunction.html">Scientists create the world's first 3 D - printed PENIS... | Daily Mail Online</a></li>

</ul>
</details>

**Tags**: `#3D printing`, `#biomedical engineering`, `#stem cells`, `#erectile dysfunction`, `#regenerative medicine`

---

<a id="item-21"></a>
## [Nvidia CEO: US should use excellent Chinese open-source AI models](https://t.me/zaihuapd/42977) ⭐️ 7.0/10

Nvidia CEO Jensen Huang stated in an interview that Chinese open-source AI models are 'excellent' and that US companies should 'absolutely' be allowed to use them. He also opposed blanket restrictions on open-source models based on national security concerns. Huang's remarks carry significant weight in the AI industry, potentially influencing US policy debates on open-source AI and China-US tech competition. His stance could encourage more open collaboration and affect market dynamics for AI chips and hardware. Huang argued that there is zero chance of Chinese companies squeezing US companies out of the market, and that cheaper or free AI could expand user bases, increasing demand for chips, hardware, and data centers. He suggested using security sandboxes to control downloaded Chinese models and addressing IP disputes on a case-by-case basis rather than through blanket bans.

telegram · zaihuapd · Aug 4, 15:22

**Background**: Open-source AI models, such as those from China's DeepSeek, have gained global attention for their performance and accessibility. Security sandboxes are isolated environments that allow programs to run without affecting the host system, which can be used to safely test and control AI models. The debate over open-source AI and national security has intensified, with some US policymakers calling for restrictions on Chinese models.

<details><summary>References</summary>
<ul>
<li><a href="https://juejin.cn/post/7223305855922995257">juejin.cn/post/7223305855922995257</a></li>
<li><a href="https://gonglue.us/254636">留给 开 源 模 型 的时间，只剩 6 个月了 – 美 国 攻略</a></li>

</ul>
</details>

**Tags**: `#AI`, `#开源模型`, `#黄仁勋`, `#产业政策`, `#中美科技`

---