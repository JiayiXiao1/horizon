---
layout: default
title: "Horizon Summary: 2026-06-20 (EN)"
date: 2026-06-20
lang: en
---

> From 31 items, 18 important content pieces were selected

---

1. [Project Valhalla Arrives in JDK 28 After a Decade](#item-1) ⭐️ 9.0/10
2. [ATProto Has No Instances: A Clarification](#item-2) ⭐️ 8.0/10
3. [Norway Bans AI for Elementary Students](#item-3) ⭐️ 8.0/10
4. [China Proposes Rules for Interoperable Decentralized Digital IDs](#item-4) ⭐️ 8.0/10
5. [Zhipu Founder Claims Model Could Reach Mythos Level by Q1 Next Year](#item-5) ⭐️ 8.0/10
6. [US Pressures ASML Over Alleged EUV Leak to China](#item-6) ⭐️ 8.0/10
7. [Infant Diapers Found to Contain Reproductive Toxicant Formamide](#item-7) ⭐️ 8.0/10
8. [China-EU Reach Solution on EV Import Dispute, EU Issues Price Guidance](#item-8) ⭐️ 8.0/10
9. [Apple Agrees to Open Third-Party App Stores in Brazil](#item-9) ⭐️ 8.0/10
10. [SpaceX sold shares to Chinese investors before IPO](#item-10) ⭐️ 8.0/10
11. [Beihang PhD Alum Accuses Two Professors of Data Fabrication](#item-11) ⭐️ 8.0/10
12. [Hyundai fully acquires Boston Dynamics from SoftBank](#item-12) ⭐️ 7.0/10
13. [Google Workspace Can Block Firefox, But It's Admin Choice](#item-13) ⭐️ 7.0/10
14. [EFF Argues Court Records Should Be Free](#item-14) ⭐️ 7.0/10
15. [Datasette Apps: Host Sandboxed HTML Apps Inside Datasette](#item-15) ⭐️ 7.0/10
16. [Google Introduces 24-Hour Wait for Sideloading Unverified Apps](#item-16) ⭐️ 7.0/10
17. [India Blocks Telegram to Curb Cheating, VPN Registrations Surge 150%](#item-17) ⭐️ 7.0/10
18. [UK Attorney General Orders Department to Stop Using X](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Project Valhalla Arrives in JDK 28 After a Decade](https://www.jvm-weekly.com/p/project-valhalla-explained-how-a) ⭐️ 9.0/10

Project Valhalla's value types are finally arriving in JDK 28, fundamentally changing how Java handles memory and performance by allowing objects to be stored inline without heap headers or pointers. This is a major paradigm shift for Java, enabling developers to write more efficient code with better memory locality and reduced garbage collection pressure, bringing Java closer to the performance of languages like C or Rust. Value types use the same 'L' descriptor as object references but are stored inline in arrays and fields, with a possible null flag. However, heap flattening only works for objects with 64-bit or smaller representations.

hackernews · philonoist · Jun 19, 06:35 · [Discussion](https://news.ycombinator.com/item?id=48595511)

**Background**: Project Valhalla is a long-running OpenJDK project aimed at augmenting the Java object model with value objects, combining object-oriented abstractions with the performance of primitives. Traditionally, all Java objects are reference types, requiring heap allocation and pointer indirection, which adds overhead. Value types eliminate this overhead by storing data directly in the memory layout.

<details><summary>References</summary>
<ul>
<li><a href="https://openjdk.org/projects/valhalla/">Project Valhalla - OpenJDK</a></li>
<li><a href="https://www.jvm-weekly.com/p/project-valhalla-explained-how-a">Project Valhalla, Explained: How a Decade of... - JVM Weekly vol. 180</a></li>
<li><a href="https://dev.to/adaumircosta/understanding-value-types-project-valhalla-faf">Understanding Value Types (Project Valhalla) - DEV Community</a></li>

</ul>
</details>

**Discussion**: The community discussion shows mixed reactions: some appreciate the hard work but criticize the complexity and missed opportunities for null safety, while others defend Java's evolution and note that many critics have outdated views of the JVM. There is also debate about the technical limitations of heap flattening for larger objects.

**Tags**: `#Java`, `#JVM`, `#Project Valhalla`, `#value types`, `#performance`

---

<a id="item-2"></a>
## [ATProto Has No Instances: A Clarification](https://overreacted.io/there-are-no-instances-in-atproto/) ⭐️ 8.0/10

Dan Abramov published a blog post explaining that ATProto, the protocol behind Bluesky, does not have 'instances' like Mastodon; instead, it separates concerns into Personal Data Servers (PDS), Relays, and AppViews for scalability. This clarification addresses a common misconception in the decentralized social media community, highlighting ATProto's architectural difference from ActivityPub-based systems like Mastodon. It helps developers and users understand the trade-offs between centralized and decentralized designs. In ATProto, a PDS hosts user data, a Relay aggregates data from many PDSs into a firehose, and an AppView consumes that firehose to build application-specific views (e.g., Bluesky's social feed). This separation allows each component to scale independently.

hackernews · danabramov · Jun 19, 15:10 · [Discussion](https://news.ycombinator.com/item?id=48599515)

**Background**: Mastodon and other platforms using ActivityPub are organized into 'instances'—servers that each host user accounts, content, and moderation. Users join an instance, and instances communicate with each other. ATProto, by contrast, decouples data storage (PDS), data aggregation (Relay), and data presentation (AppView), aiming for greater flexibility and scalability.

<details><summary>References</summary>
<ul>
<li><a href="https://atproto.wiki/en/wiki/reference/core-architecture/appview">AppViews | AT Protocol Community Wiki</a></li>
<li><a href="https://getskyscraper.com/blog/atprotocol-federation-architecture-guide">ATProtocol Federation Architecture: PDS, Relay, AppView & How ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/AT_Protocol">AT Protocol - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters debated the analogy with RSS and Google Reader, with some arguing that RSS was less dependent on a central service than ATProto's Relays. Others noted that while the protocol is decentralized, Bluesky the corporation still runs most of the infrastructure, leading to practical centralization.

**Tags**: `#ATProto`, `#Bluesky`, `#decentralization`, `#protocol design`, `#ActivityPub`

---

<a id="item-3"></a>
## [Norway Bans AI for Elementary Students](https://www.reuters.com/technology/norway-imposes-near-ban-ai-elementary-school-2026-06-19/) ⭐️ 8.0/10

Norway's government announced a near-total ban on AI use for students aged 6 to 13, and restricted use for ages 14 to 16 under teacher supervision, effective from the 2026-2027 school year. This is one of the first national-level policies to explicitly restrict generative AI in primary education, setting a precedent for how governments might balance technological adoption with foundational learning skills. The ban applies to all AI tools, including generative AI like ChatGPT, for elementary school students; older students may use AI cautiously under teacher guidance. The policy aims to protect children's development of reading, writing, and critical thinking.

hackernews · ilreb · Jun 19, 16:03 · [Discussion](https://news.ycombinator.com/item?id=48600093)

**Background**: Generative AI tools like ChatGPT can produce human-like text, images, and code, raising concerns about academic integrity and the erosion of fundamental skills. Many educators worry that over-reliance on AI may hinder students' ability to learn core subjects independently.

**Discussion**: Commenters largely supported the ban, drawing analogies to not giving calculators before students learn arithmetic. Some highlighted the broader issue of AI creating an "echo chamber" in education, where teachers and students both rely on AI for assignments and grading.

**Tags**: `#AI policy`, `#education`, `#Norway`, `#generative AI`, `#regulation`

---

<a id="item-4"></a>
## [China Proposes Rules for Interoperable Decentralized Digital IDs](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

On June 18, 2026, China's Cyberspace Administration released a draft regulation titled "Provisions on Promoting Interoperable and Mutually Recognized Applications of Decentralized Digital Identities" for public comment, with a deadline of July 18. The regulation defines decentralized digital identities based on blockchain technology, enabling user-controlled identity management through identifiers, keys, verifiable credentials, and verifiable claims. This proposal signals a major policy direction for blockchain-based identity systems in China, potentially enabling cross-platform identity interoperability in finance, transportation, customs, taxation, and digital yuan. If enacted, it could accelerate the adoption of decentralized identity across both public and private sectors, impacting how individuals and organizations manage digital identities. The regulation proposes building a public service system for decentralized digital identities, leveraging a national blockchain network to establish an "identity chain." Both domestic and foreign individuals, organizations, and industrial devices can voluntarily register, while relevant entities must fulfill data security and personal information protection obligations.

telegram · zaihuapd · Jun 19, 01:39

**Background**: Decentralized digital identity (DID) is a blockchain-based identity model that allows users to own and control their identity data without relying on a central authority. It typically consists of a decentralized identifier (DID), public-private key pairs, verifiable credentials (e.g., digital certificates), and verifiable claims (statements about an entity). The concept is aligned with W3C standards and is seen as a key enabler for Web3 and metaverse applications. China has been exploring blockchain-based identity solutions, such as the eID digital identity chain, to improve security and interoperability.

<details><summary>References</summary>
<ul>
<li><a href="https://cloud.tencent.com/developer/article/2488015">基于区块链的数字身份认证：重塑身份安全的新范式-腾讯云开发者社区-腾讯云</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/425859804">区块链数字身份：数字经济时代基础设施 ——火链科技研究院产业应用系列报告之五 - 知乎</a></li>

</ul>
</details>

**Tags**: `#decentralized identity`, `#blockchain`, `#regulation`, `#China`, `#digital identity`

---

<a id="item-5"></a>
## [Zhipu Founder Claims Model Could Reach Mythos Level by Q1 Next Year](https://x.com/jietang/status/2067580270078030088) ⭐️ 8.0/10

Zhipu AI founder Tang Jie stated that their model could reach the 'Mythos level' by Q1 next year, responding to a user's estimate that Chinese AI models lag behind US models by about 7 months. Elon Musk also commented 'Probably Q1' on the same discussion. This debate highlights the narrowing gap between US and Chinese AI capabilities, with implications for global AI leadership and competition. The timeline for reaching advanced AI levels directly affects industry investment and policy decisions. The user estimated Zhipu's GLM-5.2 model to be roughly equivalent to Claude Opus 4.7-4.8, and predicted Chinese models would reach Anthropic's Mythos (Fable) level by November-December 2026. Tang Jie responded 'won't take that long', suggesting faster progress.

telegram · zaihuapd · Jun 19, 02:24

**Background**: Mythos level is a term used by Anthropic to describe its most advanced AI models, such as Claude Fable 5, which represent a new tier of capability beyond previous generations. GLM-5.2 is Zhipu's latest open-source model with 744 billion parameters and a 1-million-token context window, ranking second only to Claude Opus 4.8 on some benchmarks.

<details><summary>References</summary>
<ul>
<li><a href="https://ia.acs.org.au/article/2026/anthropic-releases--mythos-level--chatbot-to-public.html">Anthropic releases ‘ Mythos - level ’ chatbot to public | Information Age</a></li>
<li><a href="https://www.deeplearning.ai/the-batch/zhipus-glm-5-2-is-the-new-top-open-model">Data Points: Zhipu’s GLM-5.2 is the new top open model</a></li>
<li><a href="https://benchlm.ai/compare/claude-opus-4-7-adaptive-vs-claude-opus-4-8">Claude Opus 4.7 (Adaptive) vs Claude Opus 4.8: AI Benchmark ...</a></li>

</ul>
</details>

**Discussion**: The discussion reflects active debate on the US-China AI gap, with Musk's 'Probably Q1' interpreted as Q1 2027, while Tang Jie's response suggests an earlier timeline. The community appears divided on whether Chinese models can close the gap faster than estimated.

**Tags**: `#AI`, `#LLM`, `#China AI`, `#Zhipu`, `#model comparison`

---

<a id="item-6"></a>
## [US Pressures ASML Over Alleged EUV Leak to China](https://www.bloomberg.com/news/articles/2026-06-19/us-tells-asml-it-s-concerned-china-may-have-top-chip-tool) ⭐️ 8.0/10

U.S. Commerce Secretary Lutnick told ASML executives that a top EUV lithography machine may have been illegally exported to China, violating U.S.-led export controls. ASML strongly denies the allegation, stating it has never shipped a complete EUV system to China. This incident escalates US-China tech tensions and could lead to stricter export controls on semiconductor equipment. It also strains US-Europe relations, as ASML is a Dutch company, and may influence pending U.S. legislation targeting Chinese chip manufacturing. ASML claims that none of the 314 EUV machines in operation worldwide are located in China. U.S. officials allege they have evidence that ASML exported EUV-related shipping equipment to China, but have not disclosed it.

telegram · zaihuapd · Jun 19, 03:09

**Background**: EUV (extreme ultraviolet) lithography is the most advanced chipmaking technology, essential for manufacturing sub-7nm chips. ASML is the sole global supplier of EUV machines, which are subject to strict export controls to prevent China from acquiring advanced semiconductor capabilities.

<details><summary>References</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/极紫外光刻">极紫外光刻 - 维基百科，自由的百科全书</a></li>
<li><a href="https://www.eet-china.com/mp/a299998.html">【科普】芯片制造工艺：光刻 (下)--euv极紫外光刻-电子工程专辑</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1948833673634887034">极紫外光刻机(EUV)中国"卡脖子"深度解析：核心技术壁垒与突围路径</a></li>

</ul>
</details>

**Tags**: `#semiconductors`, `#export controls`, `#EUV lithography`, `#US-China tech war`, `#ASML`

---

<a id="item-7"></a>
## [Infant Diapers Found to Contain Reproductive Toxicant Formamide](https://t.me/zaihuapd/42051) ⭐️ 8.0/10

A commissioned test by the Economic Information Daily detected the reproductive toxic substance formamide in infant diapers from brands including HUGGIES, Bebaby, and Babycare, with the chemical also found in some infants' blood and urine samples. This exposes a critical regulatory gap in China's national standards for diapers, which do not currently limit formamide, posing long-term health risks to infants through skin absorption and accumulation. Formamide is classified as a reproductive toxicant and is banned in Chinese cosmetics, but no limit exists for diapers. A reporter who wore a diaper overnight saw their blood formamide level nearly double.

telegram · zaihuapd · Jun 19, 06:05

**Background**: Formamide is a chemical used in some industrial processes and can be released from diaper materials. It has been shown in animal studies to cause reproductive and developmental toxicity, including fetal abnormalities and reduced fertility. The European Union classifies it as a Category 1B reproductive toxicant.

<details><summary>References</summary>
<ul>
<li><a href="https://www.sohu.com/a/1038359743_539932">“好奇”、“碧芭宝贝”、“Babycare”多款知名婴儿纸尿裤检测出甲酰胺生殖...</a></li>
<li><a href="https://k.sina.cn/article_7880068208_1d5b04c7006801ef46.html">为何国标对纸尿裤甲酰胺含量没有规定？|Baby|检测|标准|毒性|监管_新...</a></li>
<li><a href="https://www.sohu.com/a/1038369618_100117963">曝多款婴儿纸尿裤含有毒物质，Babycare等紧急回应_检测_国家标准_相关</a></li>

</ul>
</details>

**Tags**: `#public health`, `#consumer safety`, `#regulatory gap`, `#toxicology`, `#infant products`

---

<a id="item-8"></a>
## [China-EU Reach Solution on EV Import Dispute, EU Issues Price Guidance](https://t.me/zaihuapd/42056) ⭐️ 8.0/10

On January 12, 2025, China and the EU announced a resolution to the dispute over EU imports of Chinese-made electric vehicles, with the EU issuing a guidance document that includes minimum import prices (MIP) as an alternative to the previous tariffs of up to 35.3%. This agreement de-escalates a major trade conflict between China and the EU, potentially stabilizing the European EV market and providing Chinese automakers with a predictable framework for exports and investments in Europe. The MIP mechanism sets a price floor for Chinese EV imports, and the EU will consider Chinese automakers' investment plans in Europe when setting specific prices. The agreement replaces the previous anti-subsidy tariffs that were imposed in 2024.

telegram · zaihuapd · Jun 19, 08:57

**Background**: In 2024, the EU imposed anti-subsidy tariffs of up to 35.3% on Chinese EVs, alleging unfair subsidies. This led to trade tensions. The new MIP mechanism allows Chinese automakers to avoid these tariffs by committing to a minimum export price, aiming to offset subsidy advantages while encouraging local investment in Europe.

<details><summary>References</summary>
<ul>
<li><a href="https://news.qq.com/rain/a/20260113A01LYD00">中欧电动汽车关税达成"价格承诺"框架，2026年销量会如何？</a></li>
<li><a href="https://www.sohu.com/a/883920608_121124378">取代欧盟对华汽车关税的"最低进口价格机制"妙在哪？</a></li>
<li><a href="https://wallstreetcn.com/articles/3763155">中欧电动汽车关税达成"价格承诺"框架，2026年销量会如何？</a></li>

</ul>
</details>

**Tags**: `#trade policy`, `#electric vehicles`, `#China-EU relations`, `#automotive industry`

---

<a id="item-9"></a>
## [Apple Agrees to Open Third-Party App Stores in Brazil](https://t.me/zaihuapd/42059) ⭐️ 8.0/10

Apple has reached a settlement with Brazil's antitrust regulator, agreeing to allow iPhone users in Brazil to purchase apps and services outside the App Store and support third-party app stores. The agreement ends a three-year antitrust investigation into Apple's anti-competitive practices. This marks a significant regulatory victory for open app distribution, potentially influencing antitrust actions in other jurisdictions. Developers in Brazil will gain more freedom in payment processing and distribution, while Apple retains some fee collection. Apple must implement the changes within 105 days, and the agreement is valid for three years. Developers can display external payment methods and alternative purchase links, and Apple's payment system will be decoupled from the App Store, though Apple may still charge fees on related transactions.

telegram · zaihuapd · Jun 19, 11:15

**Background**: Apple's App Store has faced global antitrust scrutiny over its mandatory use of Apple's in-app payment system and 30% commission. Similar concessions were previously made in the EU and Japan, reflecting a trend of regulatory pressure forcing Apple to open its ecosystem.

<details><summary>References</summary>
<ul>
<li><a href="https://m.163.com/dy/article/KHIARRBT0514R9OJ.html">m.163.com/dy/article/KHIARRBT0514R9OJ.html</a></li>
<li><a href="https://finance.sina.com.cn/tech/discovery/2025-12-24/doc-inhcwtcp4520356.shtml">苹果与巴西反垄断机构和解 将开放第三方应用商店|巴西|反垄断|第三方应用_新浪科技_新浪网</a></li>
<li><a href="https://finance.sina.com.cn/tech/roll/2025-12-24/doc-inhcwxmf5844889.shtml">苹果巴西反垄断调查终结：同意开放外部支付与第三方应用商店|反垄断|苹果|巴西_新浪科技_新浪网</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#antitrust`, `#App Store`, `#Brazil`, `#regulation`

---

<a id="item-10"></a>
## [SpaceX sold shares to Chinese investors before IPO](https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china) ⭐️ 8.0/10

Court documents unsealed by ProPublica reveal that SpaceX sold shares to at least a dozen investors with addresses in China, Hong Kong, and Russia between 2018 and 2021, despite later barring such investors from its IPO. This raises serious national security and regulatory compliance concerns because SpaceX is a major defense contractor for the U.S. military, and foreign ownership from restricted countries could violate export control laws. The intermediary, Tomales Bay Capital, facilitated the sales and promised investors quarterly updates, facility tours, and access to the CFO. One investor had ties to Chinese military contractors.

telegram · zaihuapd · Jun 19, 12:00

**Background**: SpaceX is a private aerospace company that provides launch services for U.S. national security missions. Its IPO in 2026 excluded investors from China and Hong Kong due to regulatory risks. The company's valuation surged from $33.3 billion in 2019 to $2.7 trillion.

<details><summary>References</summary>
<ul>
<li><a href="https://www.propublica.org/article/spacex-elon-musk-ipo-foreign-investors-china">Before SpaceX IPO, Investors in China Secretly Acquired Stakes — ProPublica</a></li>
<li><a href="https://www.warren.senate.gov/newsroom/press-releases/warren-kim-warn-that-undisclosed-investments-in-spacex-by-chinese-interests-may-threaten-national-security-raise-questions-about-compliance-with-national-security-law">Warren, Kim Warn That Undisclosed Investments in SpaceX by Chinese Interests May Threaten National Security, Raise Questions about Compliance with National Security Law | U.S. Senator Elizabeth Warren of Massachusetts</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#national security`, `#foreign investment`, `#regulatory compliance`, `#investigative journalism`

---

<a id="item-11"></a>
## [Beihang PhD Alum Accuses Two Professors of Data Fabrication](https://www.zaobao.com.sg/news/china/story20260619-9231002) ⭐️ 8.0/10

Former Beihang PhD student Geng Jiangtao publicly accused two professors—Chang Lingqian and Wang Jun—of fabricating data in papers published in Nature and other journals, prompting a flood of visitors that temporarily crashed Beihang's website. This incident highlights growing concerns over research integrity in China's top universities and the power of individual whistleblowers to trigger institutional scrutiny, potentially leading to retractions and policy changes. Geng, who runs the science communication account 'Geng Tongxue Jiang Gushi,' previously reported five scholars from four other universities, all of whom have been sanctioned. The accused professors include Chang Lingqian, vice dean of Beihang's School of Medical Science and Engineering, and Wang Jun from the School of Aeronautic Science and Engineering.

telegram · zaihuapd · Jun 19, 16:02

**Background**: Geng Jiangtao was a PhD student at Beihang University who dropped out in 2025 to become a science communicator. Since April 2026, he has been publicly challenging the integrity of published research, using data analysis to flag anomalies. His latest accusations target two Beihang professors, with Chang's Nature paper on a flexible implantable electronic patch being questioned for 'perfectly suspicious' experimental data.

<details><summary>References</summary>
<ul>
<li><a href="https://ygy.buaa.edu.cn/info/1087/4350.htm">常凌乾-北航医学科学与工程学院</a></li>
<li><a href="https://news.buaa.edu.cn/info/1005/65745.htm">《Nature》报道北航常凌乾教授团队与合作者破解给药难题：一种柔性可...</a></li>
<li><a href="https://www.sinchew.com.my/news/20260601/international/7552269">耿同学停学术打假 社媒遭限流 学者：平台或担心愈演愈烈</a></li>

</ul>
</details>

**Tags**: `#academic integrity`, `#research misconduct`, `#China`, `#university`, `#data fabrication`

---

<a id="item-12"></a>
## [Hyundai fully acquires Boston Dynamics from SoftBank](https://startupfortune.com/hyundai-takes-full-control-of-boston-dynamics-as-softbank-exits-for-325-million/) ⭐️ 7.0/10

Hyundai Motor Group exercised a put option to buy SoftBank's remaining 9% stake in Boston Dynamics, gaining full control of the robotics company for $325 million. This acquisition positions Hyundai to commercialize advanced humanoid robots like Atlas, addressing labor shortages in South Korea and competing with Tesla in general-purpose robotics. The deal values Boston Dynamics at about $3.6 billion, and Hyundai previously acquired an 80% stake for $880 million in December 2020, valuing the company at $1.1 billion at that time.

hackernews · ck2 · Jun 19, 16:28 · [Discussion](https://news.ycombinator.com/item?id=48600312)

**Background**: Boston Dynamics is known for highly mobile robots like Spot, Atlas, and Handle. Hyundai plans to integrate Atlas into its factories and develop AI-driven robotics for logistics and future work, aligning with its physical AI strategy unveiled at CES 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Boston_Dynamics">Boston Dynamics - Wikipedia</a></li>
<li><a href="https://bostondynamics.com/">The World's Leading Robotics Company | Boston Dynamics</a></li>
<li><a href="https://www.theaibulletin.com/post/hyundai-s-ai-robotics-strategy-debuts-atlas-at-ces-2026">Hyundai 's AI Robotics Strategy Debuts Atlas at CES 2026</a></li>

</ul>
</details>

**Discussion**: Commenters debated the utility of humanoid robots versus purpose-built machines, with some questioning the efficiency of the human form for manufacturing. Others linked the acquisition to South Korea's declining working-age population, suggesting a strategic move to address labor shortages.

**Tags**: `#robotics`, `#acquisition`, `#Hyundai`, `#Boston Dynamics`, `#humanoid robots`

---

<a id="item-13"></a>
## [Google Workspace Can Block Firefox, But It's Admin Choice](https://tales.fromprod.com/2026/169/google-workspace-threatening-to-block-firefox.html) ⭐️ 7.0/10

A blog post revealed that Google Workspace's Context-Aware Access product can block Firefox browser access, but this is an enterprise admin configuration, not a Google-wide policy. This clarifies a common misconception that Google is anti-Firefox, highlighting the role of enterprise IT policies in browser restrictions and sparking broader discussion about browser detection and user-agent manipulation. Context-Aware Access is only available on Google Workspace Enterprise editions, not on Business Plus, which the blog author uses. The feature allows admins to set policies based on device attributes like browser type.

hackernews · birdculture · Jun 19, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48600345)

**Background**: Google Workspace's Context-Aware Access lets admins create granular access control policies based on user identity, device security, location, and IP address. It is a security feature for enterprise environments, not a consumer-facing restriction.

<details><summary>References</summary>
<ul>
<li><a href="https://knowledge.workspace.google.com/admin/security/protect-your-business-with-context-aware-access">Protect your business with Context-Aware Access - Google</a></li>
<li><a href="https://knowledge.workspace.google.com/admin/security/create-context-aware-access-levels">Create Context-Aware access levels | Security & data ... - Google</a></li>
<li><a href="https://workspaceupdates.googleblog.com/2025/08/context-aware-access-openid-connect-apps.html">Google Workspace Updates: Context-Aware Access policies can ...</a></li>

</ul>
</details>

**Discussion**: The community quickly corrected the initial impression that Google was blocking Firefox, noting it's an admin-configurable feature. The blog author confirmed they are the admin and use Business Plus, which lacks Context-Aware Access, so the block was likely due to other settings. Some commenters expressed broader concerns about browser detection and the desire to eliminate user-agent strings.

**Tags**: `#Google Workspace`, `#Firefox`, `#browser detection`, `#enterprise IT`, `#privacy`

---

<a id="item-14"></a>
## [EFF Argues Court Records Should Be Free](https://www.eff.org/deeplinks/2026/06/court-records-should-be-free) ⭐️ 7.0/10

The Electronic Frontier Foundation (EFF) published an article arguing that public access to court records should be free, criticizing the high fees charged by PACER, the federal court records system. This matters because PACER fees create a financial barrier to accessing legal information, undermining transparency and equal access to justice. The debate highlights the tension between funding court systems and the public's right to know. PACER charges $0.10 per page, with a maximum of $3.00 per document, but frequent users can incur significant costs. The EFF points to initiatives like CourtListener and RECAP, which crowdsource free access to PACER documents.

hackernews · hn_acker · Jun 19, 17:34 · [Discussion](https://news.ycombinator.com/item?id=48600946)

**Background**: PACER (Public Access to Court Electronic Records) is the federal judiciary's system for accessing court documents electronically. While the system is funded primarily through user fees, critics argue that these fees restrict public access to legal materials that should be freely available. CourtListener, a project of Free Law Project, provides a free search engine for legal opinions and, through the RECAP browser extension, archives PACER documents shared by users.

<details><summary>References</summary>
<ul>
<li><a href="https://www.eff.org/deeplinks/2026/06/court-records-should-be-free">Court Records Should Be Free | Electronic Frontier Foundation</a></li>
<li><a href="https://pacer.uscourts.gov/pacer-pricing-how-fees-work">PACER Pricing: How fees work | PACER: Federal Court Records</a></li>
<li><a href="https://free.law/projects/courtlistener/">CourtListener Research and Awareness Website | Free Law Project | Making the legal ecosystem more equitable and competitive.</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted practical issues: one noted that state court fees can be even higher than PACER's, with Idaho charging $10 per page. Another praised CourtListener and RECAP for filling a vital niche, hoping they become obsolete when free access is achieved. A third commenter argued that financial cost is one of many ways the government limits access to rights.

**Tags**: `#legal tech`, `#open government`, `#PACER`, `#public records`, `#access to justice`

---

<a id="item-15"></a>
## [Datasette Apps: Host Sandboxed HTML Apps Inside Datasette](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

The datasette-apps plugin allows users to host custom HTML+JavaScript applications inside Datasette, running in a sandboxed iframe with read-only SQL access and optional configured write queries. This plugin transforms Datasette from a data exploration tool into a full application platform, enabling developers to build interactive data-driven apps without separate hosting. Apps are sandboxed using iframe sandbox attributes and a CSP header that blocks external HTTP requests, preventing data exfiltration. Write queries require explicit configuration via stored queries.

rss · Simon Willison · Jun 18, 23:58

**Background**: Datasette is an open-source tool for exploring and publishing data, offering a JSON API for custom frontends. Previously, developers had to host their HTML/JS apps separately; this plugin integrates them directly into Datasette instances.

<details><summary>References</summary>
<ul>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette Apps</a></li>
<li><a href="https://simonwillison.net/2026/Jun/18/datasette-apps/">Datasette Apps: Host custom HTML applications inside Datasette</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#plugin`, `#sql`, `#web-applications`, `#sandbox`

---

<a id="item-16"></a>
## [Google Introduces 24-Hour Wait for Sideloading Unverified Apps](https://t.me/zaihuapd/42054) ⭐️ 7.0/10

Google announced a new "advanced process" for sideloading unverified apps on Android, requiring users to wait 24 hours and complete multi-step verification before installation. This update significantly raises the friction for sideloading, aiming to reduce fraud and malware risks for millions of Android users, while impacting developers who distribute apps outside Google Play. Users must enable developer mode, confirm they are not being coerced, restart the device, re-authenticate, wait 24 hours, then use fingerprint, face recognition, or PIN to proceed; after installation, the permission can be set to 7 days or permanent.

telegram · zaihuapd · Jun 19, 07:59

**Background**: Sideloading refers to installing apps from sources other than the official app store, which can expose users to unverified software. Google has been increasing security measures, including developer verification announced in August 2025, to combat malicious apps.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sideloading">Sideloading - Wikipedia</a></li>
<li><a href="https://developer.android.com/developer-verification">Android developer verification | Android Developers</a></li>
<li><a href="https://developer.android.com/studio/debug/dev-options">Configure on-device developer options | Android Studio ...</a></li>

</ul>
</details>

**Tags**: `#Android`, `#security`, `#sideloading`, `#Google`, `#mobile`

---

<a id="item-17"></a>
## [India Blocks Telegram to Curb Cheating, VPN Registrations Surge 150%](https://t.me/zaihuapd/42058) ⭐️ 7.0/10

India temporarily blocked Telegram from June 16 to June 22, 2024, to prevent cheating during the NEET-UG medical entrance exam, leading to a 150% surge in VPN registrations from India, as reported by Proton VPN. This incident highlights the tension between government censorship and digital rights, and the unintended consequences of using BGP hijacking for blocking, which affected users beyond India. The blockade was reportedly enforced via BGP hijacking by Indian telecom operators, which inadvertently disrupted Telegram access in other countries like the UAE. Telegram CEO criticized the move.

telegram · zaihuapd · Jun 19, 10:30

**Background**: BGP hijacking is a malicious rerouting of internet traffic by corrupting routing tables. NEET-UG is a national medical entrance exam in India. Proton VPN is a Swiss VPN service that saw a 150% increase in hourly registrations from India during the block.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/BGP_hijacking">BGP hijacking - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Proton_VPN">Proton VPN</a></li>
<li><a href="https://neet.nta.nic.in/">NATIONAL ELIGIBILITY CUM ENTRANCE TEST | NEET | India</a></li>

</ul>
</details>

**Tags**: `#censorship`, `#VPN`, `#BGP hijacking`, `#India`, `#Telegram`

---

<a id="item-18"></a>
## [UK Attorney General Orders Department to Stop Using X](https://www.theguardian.com/technology/2026/jun/18/uk-attorney-general-tells-staff-stop-using-x-disinformation-concerns) ⭐️ 7.0/10

UK Attorney General Richard Hermer has ordered his office to stop posting on X (formerly Twitter), making it the first UK government body to abandon the platform over disinformation and hate speech concerns. This move signals a potential shift in UK government policy toward social media regulation, as it is the first government body to leave X over disinformation concerns, potentially influencing other departments and setting a precedent for public sector engagement with the platform. The decision followed violent incidents in Southampton and Belfast in early June 2026, with Hermer expressing growing concern that X is used to spread racial hatred and divide communities. The UK government has already announced a ban on social media for under-16s and plans to amend the Online Safety Act to require faster removal of inflammatory content during crises.

telegram · zaihuapd · Jun 19, 15:30

**Background**: The Attorney General for England and Wales is the chief legal adviser to the UK government. The Online Safety Act 2023 imposes a duty of care on online platforms to tackle illegal and harmful content, with fines of up to £18 million or 10% of annual turnover. X has faced widespread criticism for being a hotbed of disinformation since Elon Musk's acquisition, including an EU investigation and major media outlets leaving the platform.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Attorney_General_for_England_and_Wales">Attorney General for England and Wales - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Online_Safety_Act_2023">Online Safety Act 2023</a></li>
<li><a href="https://tech.co/news/x-worst-platform-disinformation">Here's Why X is The Worst Platform for Disinformation - Tech.co</a></li>

</ul>
</details>

**Tags**: `#social media`, `#disinformation`, `#UK government`, `#X`, `#regulation`

---