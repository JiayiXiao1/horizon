---
layout: default
title: "Horizon Summary: 2026-06-19 (ZH)"
date: 2026-06-19
lang: zh
---

> From 39 items, 18 important content pieces were selected

---

1. [1 万个 GitHub 仓库传播木马恶意软件](#item-1) ⭐️ 9.0/10
2. [Noam Shazeer 离开谷歌加入 OpenAI](#item-2) ⭐️ 9.0/10
3. [GLM-5.2：领先的开权重 LLM 发布](#item-3) ⭐️ 9.0/10
4. [医院和大学药物再利用降低成本 90%](#item-4) ⭐️ 8.0/10
5. [强制同意投诉导致 Elkjop 被罚 180 万欧元](#item-5) ⭐️ 8.0/10
6. [新工具检查你的数据是否在 LLM 训练集中](#item-6) ⭐️ 8.0/10
7. [Modos 彩色电子纸显示器达到 60Hz 刷新率](#item-7) ⭐️ 8.0/10
8. [Charity Majors：AI 要求更强的工程纪律](#item-8) ⭐️ 8.0/10
9. [苹果与英特尔达成初步芯片代工协议](#item-9) ⭐️ 8.0/10
10. [国家网信办就分布式数字身份互通互认规定征求意见](#item-10) ⭐️ 8.0/10
11. [Ubiquiti 推出基于 ZFS 的企业级 NAS](#item-11) ⭐️ 7.0/10
12. [康奈尔 CS 6120 高级编译器自学课程](#item-12) ⭐️ 7.0/10
13. [瑞士议会解除新建核电站禁令](#item-13) ⭐️ 7.0/10
14. [W Social：欧洲数字主权还是政治作秀？](#item-14) ⭐️ 7.0/10
15. [Datasette Apps：沙盒化 HTML/JS 应用支持 SQL 查询](#item-15) ⭐️ 7.0/10
16. [多款婴幼儿纸尿裤检出生殖毒性物质甲酰胺](#item-16) ⭐️ 7.0/10
17. [小米开源智能家居方案 Miloco 2.0](#item-17) ⭐️ 7.0/10
18. [华为设定 Wi-Fi 7 专利费每台 0.5 美元](#item-18) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [1 万个 GitHub 仓库传播木马恶意软件](https://orchidfiles.com/github-repositories-distributing-malware/) ⭐️ 9.0/10

一项分析发现超过 1 万个 GitHub 仓库通过克隆仓库和自动提交更新来传播木马恶意软件，且数月未被检测到。 这种广泛的供应链攻击威胁着开源生态系统，可能感染那些无意中克隆或依赖这些仓库的开发者和用户。 每个仓库都包含一个带有木马的 zip 压缩包；攻击者克隆合法仓库，注入恶意软件，并频繁推送提交以保持在搜索结果中的可见性。

hackernews · theorchid · Jun 18, 11:45 · [社区讨论](https://news.ycombinator.com/item?id=48583928)

**背景**: GitHub 是一个流行的开源代码托管平台，但其协作性质可能被利用。攻击者经常克隆合法项目，添加恶意软件，然后以相似名称重新上传，诱骗用户下载被感染的代码。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://orchidfiles.com/github-repositories-distributing-malware/">How I found 10,000 GitHub repositories distributing Trojan malware</a></li>
<li><a href="https://checkmarx.com/blog/github-repos-used-for-distributing-malware/">GitHub Repos Used for Distributing Malware</a></li>
<li><a href="https://gbhackers.com/109-fake-github-repos/">109 Fake GitHub Repos Spread SmartLoader, StealC Malware</a></li>

</ul>
</details>

**社区讨论**: 评论者指出，攻击针对的是自动化代理而非人类，一些人报告了他们的名字被用于虚假仓库的个人经历。其他人认为频繁提交有助于仓库出现在“最近更新”的搜索结果中。

**标签**: `#security`, `#malware`, `#github`, `#supply chain attack`, `#open source`

---

<a id="item-2"></a>
## [Noam Shazeer 离开谷歌加入 OpenAI](https://twitter.com/NoamShazeer/status/2067400851438932297) ⭐️ 9.0/10

Noam Shazeer，开创性论文《Attention Is All You Need》的合著者、前谷歌 Gemini 联合负责人，宣布离开谷歌加入 OpenAI。 此举标志着 AI 行业的一次重大人才转移，因为 Shazeer 是支撑现代大语言模型的 Transformer 架构的关键人物。他从谷歌跳槽到直接竞争对手，可能加速 OpenAI 的研究，并加剧两家公司之间的竞争。 Shazeer 最初于 2021 年离开谷歌，共同创立了 Character.AI，随后于 2024 年通过一项据报道价值 27 亿美元的许可协议回归，并担任 Gemini 联合负责人。如今，仅一年多后，他再次离开，加入 OpenAI。

hackernews · lukasgross · Jun 18, 00:26 · [社区讨论](https://news.ycombinator.com/item?id=48578913)

**背景**: Noam Shazeer 是谷歌的长期研究员，于 2000 年加入公司。他是 2017 年论文《Attention Is All You Need》的八位合著者之一，该论文提出了 Transformer 架构——这是大多数现代大语言模型（如 GPT-4 和 Gemini）的基础。在本次跳槽前，他共同领导了谷歌的 Gemini 模型开发。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Noam_Shazeer">Noam Shazeer</a></li>
<li><a href="https://www.reuters.com/technology/googles-gemini-co-lead-noam-shazeer-join-openai-2026-06-18/">Google Gemini co-lead Noam Shazeer to join IPO-bound OpenAI | Reuters</a></li>
<li><a href="https://en.wikipedia.org/wiki/Attention_Is_All_You_Need">Attention Is All You Need - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 社区讨论非常热烈，许多人强调 Shazeer 在谷歌的传奇地位以及他在 Transformer 论文中的关键作用。一些人对他回归谷歌后迅速离开表示惊讶，而另一些人则认为，鉴于 OpenAI 在 AI 竞赛中的领先地位，此举是自然的。

**标签**: `#AI`, `#OpenAI`, `#Google`, `#transformers`, `#industry news`

---

<a id="item-3"></a>
## [GLM-5.2：领先的开权重 LLM 发布](https://simonwillison.net/2026/Jun/17/glm-52/#atom-everything) ⭐️ 9.0/10

Z.ai 发布了 GLM-5.2，这是一个拥有 753B 参数、采用 MIT 许可证的开权重 LLM，具有 100 万 token 的上下文窗口和顶尖的基准测试性能。 GLM-5.2 在 Artificial Analysis Intelligence Index 上成为领先的开权重模型，超越了 MiniMax-M3 和 DeepSeek V4 Pro 等竞争对手，并在 Code Arena WebDev 排行榜上排名第二，这使其成为开源 AI 领域的一项重大进步。 该模型采用混合专家架构，在 753B 总参数中有 40 个活跃参数，大小为 1.51TB。它仅支持文本输入，且 token 消耗较高，每个任务使用 43k 输出 token，而 MiniMax-M3 为 24k。

rss · Simon Willison · Jun 17, 23:58

**背景**: 开权重 LLM 公开其训练参数，允许研究人员和开发者使用和修改。混合专家架构每次只激活部分参数，提高了效率。100 万 token 的上下文窗口可以处理非常长的文档或对话。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.ai21.com/glossary/foundational-llm/open-weights-model/">What is an Open-Weights Model? | AI21</a></li>
<li><a href="https://developer.nvidia.com/blog/applying-mixture-of-experts-in-llm-architectures/">Applying Mixture of Experts in LLM Architectures | NVIDIA Technical...</a></li>

</ul>
</details>

**社区讨论**: 社区反响热烈，独立基准测试验证了 GLM-5.2 的领先性能。但有人指出其 token 消耗较高，以及一个在前端编码任务中表现出色的模型缺乏图像输入能力。

**标签**: `#LLM`, `#open-weights`, `#AI`, `#GLM-5.2`, `#benchmark`

---

<a id="item-4"></a>
## [医院和大学药物再利用降低成本 90%](https://www.kcl.ac.uk/news/hospitals-and-universities-repurposing-drugs-at-90-lower-cost) ⭐️ 8.0/10

医院和大学通过后期试验对现有药物进行再利用，成本比制药行业试验低 90%，为失明和罕见病等疾病提供可负担的治疗方案。 这种方法可以大幅降低医疗成本并扩大治疗可及性，尤其对于制药公司缺乏开发新药动力的罕见病。 成本节省源于使用已获批用于其他适应症的药物，绕过了早期开发阶段。然而，没有监管途径可以在未经制造商同意或自己成为制造商的情况下扩展用途。

hackernews · giuliomagnifico · Jun 18, 10:33 · [社区讨论](https://news.ycombinator.com/item?id=48583386)

**背景**: 药物再利用（或重定位）涉及研究现有药物的新治疗用途。这是一种成本效益高的策略，因为安全性数据已经存在，减少了临床试验的时间和费用。该方法在 COVID-19 大流行期间因紧急授权使用再利用药物而受到关注。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.news-medical.net/news/20260616/Universities-and-hospitals-repurpose-existing-drugs-at-significantly-lower-costs.aspx">Universities and hospitals repurpose existing drugs at significantly...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Drug_repurposing">Drug repurposing</a></li>
<li><a href="https://pmc.ncbi.nlm.nih.gov/articles/PMC9336118/">Drug repurposing : a systematic review on root causes, barriers and...</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了个人经历，例如使用阿瓦斯汀（贝伐珠单抗）治疗黄斑变性每剂 50 美元，而 Lucentis 每剂 1500 美元，并指出美国医疗体系中激励机制的扭曲，例如艾司氯胺酮（Spravato）尽管不如普通氯胺酮有效却获得专利。一些人指出没有制造商参与时再利用存在监管障碍。

**标签**: `#drug repurposing`, `#healthcare`, `#cost reduction`, `#pharmaceuticals`, `#innovation`

---

<a id="item-5"></a>
## [强制同意投诉导致 Elkjop 被罚 180 万欧元](https://www.thatprivacyguy.com/blog/elkjop-forced-consent-fine/) ⭐️ 8.0/10

一名隐私倡导者关于强制同意营销的投诉，导致挪威零售商 Elkjop 根据 GDPR 被罚款 180 万欧元，此时距离最初投诉已有五年。 此案表明，个人投诉可以导致重大的 GDPR 执法，赋予消费者挑战非法数据实践的权利，并为欧洲各地的类似案件树立了先例。 该罚款由挪威数据保护局（Datatilsynet）处以，原因是要求客户加入忠诚俱乐部才能接收营销信息，这构成了强制同意。投诉人记录了违规行为并坚持了五年。

hackernews · speckx · Jun 18, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48589501)

**背景**: 根据 GDPR，同意必须自由给予、具体、知情且明确。强制同意，即服务以同意数据处理为条件，通常是非法的。此案凸显了个人通过战略诉讼在维护隐私权方面的作用。

**社区讨论**: 评论者赞扬了投诉人的坚持，并指出个人执法的重要性。一些人强调了公司忽视明显违法行为的荒谬性，而另一些人则提供了官方决定和翻译的链接。

**标签**: `#GDPR`, `#privacy`, `#data protection`, `#enforcement`, `#consent`

---

<a id="item-6"></a>
## [新工具检查你的数据是否在 LLM 训练集中](https://www.intheweights.com/) ⭐️ 8.0/10

新网站 intheweights.com 并行查询多个大型语言模型，检测它们对给定用户名的识别强度，从而揭示个人数据是否出现在训练集中。 该工具凸显了个人在线内容可能在未经同意的情况下被嵌入 LLM 训练数据的隐私问题，并为用户提供了一种检测其在 AI 模型中数字足迹的方法。 该工具并行查询前沿和小型模型，对响应进行聚类，并输出识别分数；结果是非确定性的，添加更多关于自己的关键词可以提高分数。

hackernews · turtlesoup · Jun 18, 20:49 · [社区讨论](https://news.ycombinator.com/item?id=48591348)

**背景**: 大型语言模型（LLM）在从互联网抓取的大量文本数据上进行训练，这些数据通常包含个人信息。神经网络的“权重”是训练过程中学习到的参数，编码了数据中的模式。该工具探测特定用户名是否被记忆在这些权重中，从而指示相关数据在训练集中的存在。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Large_language_model">Large language model - Wikipedia</a></li>
<li><a href="https://www.geeksforgeeks.org/deep-learning/the-role-of-weights-and-bias-in-neural-networks/">Weights and Bias in Neural Networks - GeeksforGeeks</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了复杂情绪：有人对自己过去的文字出现在训练数据中感到不安，也有人对识别结果感到有趣。还有关于工具非确定性以及添加关键词如何提高分数的技术讨论。

**标签**: `#LLM`, `#privacy`, `#data recognition`, `#AI ethics`, `#web tool`

---

<a id="item-7"></a>
## [Modos 彩色电子纸显示器达到 60Hz 刷新率](https://spectrum.ieee.org/modos-e-paper-monitor) ⭐️ 8.0/10

两人初创公司 Modos 正在开发 Modos Flow，这是一款 13.3 英寸彩色电子纸显示器，原生分辨率 3200x2400，刷新率 60Hz，由新型显示控制器实现。 这推动电子纸技术更接近主流应用，提供高分辨率彩色显示和适合通用计算的刷新率，相比传统 LCD 可能减少眼疲劳和功耗。 Modos Flow 具备触摸输入和低于 100 毫秒的延迟，公司正在 Crowd Supply 上众筹。以往的电子纸显示器刷新率较低或仅为灰度显示。

hackernews · Vinnl · Jun 18, 11:41 · [社区讨论](https://news.ycombinator.com/item?id=48583897)

**背景**: 电子纸显示器（如采用 E Ink 技术的产品）反射环境光，仅在图像变化时耗电，因此非常适合阅读和低功耗应用。然而，传统电子纸刷新率慢（通常低于 30Hz）且缺乏色彩，限制了其在视频或交互任务中的使用。最近的进展，如 Dasung 的 60Hz 灰度面板，已开始解决这些限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://spectrum.ieee.org/modos-e-paper-monitor">Modos Color Monitor Pushes E-Paper Displays Further - IEEE Spectrum</a></li>
<li><a href="https://www.tomshardware.com/monitors/portable-monitors/hands-on-with-modos-tech-13-3-inch-e-paper-monitors">Hands-on with Modos Tech 13.3-inch e-paper monitors — we tried the current Dev Kit model and the next-gen Modos Flow touch | Tom's Hardware</a></li>
<li><a href="https://www.crowdsupply.com/modos-tech/modos-paper-monitor">Modos Paper Monitor | Crowd Supply</a></li>

</ul>
</details>

**社区讨论**: 评论者对这一进展感到兴奋，认为这是多年来最有前景的电子纸突破之一。一些人担心高刷新率下面板的寿命，另一些人则将其与 RLCD 和其他替代显示技术进行了有利比较。

**标签**: `#e-paper`, `#display technology`, `#hardware`, `#startup`

---

<a id="item-8"></a>
## [Charity Majors：AI 要求更强的工程纪律](https://simonwillison.net/2026/Jun/17/charity-majors/#atom-everything) ⭐️ 8.0/10

Charity Majors 认为，AI 使代码生成变得廉价且可丢弃，这要求更强的工程纪律，而非更少。 这一观点挑战了普遍认为 AI 会降低对严格工程实践需求的假设，强调了代码变得可丢弃、工程纪律变得更加关键的范式转变。 Majors 指出，2025 年代码生产的经济学被颠覆：代码从难以生成且昂贵变为几乎免费且即时，使其变得可丢弃和可重新生成。

rss · Simon Willison · Jun 17, 17:12

**背景**: 传统上，编写代码是劳动密集且昂贵的，因此代码被精心策划和重用。借助生成式 AI，代码可以快速且廉价地生成，但这种新的创作便利性要求在测试、审查和维护代码质量方面有更强的纪律。

**标签**: `#AI-assisted programming`, `#software engineering`, `#generative AI`, `#engineering discipline`

---

<a id="item-9"></a>
## [苹果与英特尔达成初步芯片代工协议](https://t.me/zaihuapd/42031) ⭐️ 8.0/10

据报道，苹果与英特尔已达成初步协议，由英特尔代工生产部分苹果设备所需的芯片，这可能减少苹果对台积电的依赖。 该协议可能重塑半导体供应链，为英特尔的代工业务带来重要客户，同时让苹果在芯片生产上拥有更多议价能力和多元化选择。 谈判历时一年有余，并在近几个月敲定，美国政府在其中发挥了重要推动作用。目前尚不清楚哪些苹果产品（iPhone、iPad 或 Mac）将使用英特尔制造的芯片。

telegram · zaihuapd · Jun 18, 09:19

**背景**: 苹果历来依赖台积电和三星进行芯片制造，因为它自行设计芯片但不运营晶圆厂。英特尔一直在扩展其代工服务，旨在与台积电和三星竞争，并已与英伟达和 SpaceX 建立了合作伙伴关系。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zh.wikipedia.org/wiki/Apple晶片">Apple晶片 - 维基百科，自由的百科全书</a></li>
<li><a href="https://letschuhai.com/yingteerjiangtou200yimeiyuanxinjianjingyuanchangkaizhanjingyuandaigongyewu">英特尔将投200亿美元新建晶圆厂，开展晶圆 代 工 业 务 | 36氪出海</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Intel`, `#chip manufacturing`, `#semiconductors`, `#supply chain`

---

<a id="item-10"></a>
## [国家网信办就分布式数字身份互通互认规定征求意见](https://www.cac.gov.cn/2026-06/18/c_1783525605384124.htm) ⭐️ 8.0/10

该规定可能为中国分布式数字身份互通互认建立国家标准，并影响全球区块链身份标准。其目标是推动金融、交通、海关、税务、数字人民币等领域的跨平台身份互通互认，对境内外个人和机构均产生影响。 规定提出依托国家区块链网络建设身份链，境内外个人、机构和工业设备均可自愿申请注册。相关机构需履行数据安全和个人信息保护义务。

telegram · zaihuapd · Jun 19, 01:39

**背景**: 分布式数字身份（DID）是一种基于区块链的身份系统，让用户掌控自己的身份数据，不同于传统的集中式系统。它利用密码学技术实现安全、可验证的声明，无需依赖中央机构。W3C 一直在制定 DID 标准，中国的举措既顺应全球趋势，又结合了自身监管环境。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://zhuanlan.zhihu.com/p/689030887">【深度】DID分布式数字身份(1/5)--什么是DID - 知乎</a></li>
<li><a href="https://blog.csdn.net/wangzelong046/article/details/135659699">数字身份是啥？_分布式数字身份-CSDN博客</a></li>

</ul>
</details>

**标签**: `#blockchain`, `#digital identity`, `#regulation`, `#China`, `#interoperability`

---

<a id="item-11"></a>
## [Ubiquiti 推出基于 ZFS 的企业级 NAS](https://blog.ui.com/article/introducing-enterprise-nas) ⭐️ 7.0/10

Ubiquiti 发布了一款基于 ZFS 文件系统的新企业级 NAS 设备，采用 3U 机架式机箱，配备十六个 SATA 硬盘位、双 25 Gbps SFP28 端口和冗余电源。 这标志着 Ubiquiti 进入企业级 NAS 市场，为已投资 UniFi 生态系统的用户提供集成解决方案，并具备 ZFS 的数据完整性和高级功能。 该 NAS 售价 3999 美元，支持 M.2 NVMe 缓存，但社区成员质疑机械硬盘能否饱和 25 Gbps 网络链路，并对 Ubiquiti 的软件质量和过去的安全事件表示担忧。

hackernews · ksec · Jun 18, 14:24 · [社区讨论](https://news.ycombinator.com/item?id=48585866)

**背景**: ZFS 是一种高级文件系统和卷管理器，以数据完整性、快照和高效复制而闻名。Ubiquiti 以其网络设备和 UniFi 软件生态系统著称，这款 NAS 旨在为企业客户提供紧密集成的存储解决方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://store.ui.com/us/en/products/enas">Enterprise NAS - Ubiquiti Store</a></li>
<li><a href="https://news.ycombinator.com/item?id=48585866">Ubiquiti : Enterprise NAS , Built on ZFS | Hacker News</a></li>

</ul>
</details>

**社区讨论**: Hacker News 社区反应不一：一些人称赞 Ubiquiti 的无订阅模式和采用 ZFS，而另一些人则批评过去的软件质量问题，并质疑硬件能否充分利用高速网络。

**标签**: `#Ubiquiti`, `#NAS`, `#ZFS`, `#enterprise storage`, `#hardware`

---

<a id="item-12"></a>
## [康奈尔 CS 6120 高级编译器自学课程](https://www.cs.cornell.edu/courses/cs6120/2025fa/self-guided/) ⭐️ 7.0/10

康奈尔大学的 CS 6120 高级编译器课程现已作为免费的在线自学资源开放，涵盖从基本优化到动态编译的主题。 该课程为全球编译器爱好者和学生提供了高质量、易获取的资源，填补了高级编译器教育的空白。 课程包括讲座视频、阅读材料和作业，但一些社区成员指出，像跟踪编译这样的主题可能已经过时，且内容可能与入门编译器课程重叠。

hackernews · ibobev · Jun 18, 11:04 · [社区讨论](https://news.ycombinator.com/item?id=48583606)

**背景**: 编译器设计是计算机科学的核心领域，涉及源代码如何转换为可执行程序。高级编译器课程通常探讨超越入门内容的优化技术、代码生成和运行时系统。

**社区讨论**: 社区评论包括对课程可用性的赞扬，但也有批评反馈：一些人认为跟踪编译是死胡同，另一些人质疑这些主题是否真正高级。还提到了与其他资源（如 Nora Sandler 的书）的比较。

**标签**: `#compilers`, `#online course`, `#programming languages`, `#computer science education`

---

<a id="item-13"></a>
## [瑞士议会解除新建核电站禁令](https://www.bluewin.ch/en/news/switzerland/parliament-lifts-ban-on-new-nuclear-power-plants-3257535.html) ⭐️ 7.0/10

瑞士议会投票决定解除新建核电站的禁令，推翻了 2017 年公投中逐步淘汰核能的决定。该变化仍需在全民公投中获得批准。 这一政策转变可能重塑瑞士的能源战略，通过新建核项目解决该国夏季与冬季的能源不平衡问题。同时，它也标志着欧洲在能源安全担忧下对核能的重新审视。 该禁令最初是在 2011 年福岛核事故后实施的，并在 2017 年通过公投禁止新建核电站。新决定预计将面临左翼和绿党的强烈反对，最终结果取决于未来的公投。

hackernews · leonidasrup · Jun 18, 14:17 · [社区讨论](https://news.ycombinator.com/item?id=48585746)

**背景**: 瑞士目前有四座核反应堆，提供约 30%的电力。该国严重依赖水力发电，但在冬季水电出力下降时面临季节性能源短缺。核能是一种低碳能源，但安全和废物处理问题仍令人担忧。

**社区讨论**: 评论者表达了不同观点：一些人强调核能每太瓦时死亡率低和能源安全优势，而另一些人则质疑铀矿开采和废物处理的清洁性。鉴于政治分歧，人们对公投能否通过持怀疑态度。

**标签**: `#nuclear energy`, `#Switzerland`, `#energy policy`, `#technology`, `#politics`

---

<a id="item-14"></a>
## [W Social：欧洲数字主权还是政治作秀？](https://blog.elenarossini.com/w-social-public-institutions-and-the-theater-of-european-digital-sovereignty/) ⭐️ 7.0/10

Elena Rossini 发表博文批评欧洲社交媒体平台 W Social，认为它是一个缺乏透明度的表演性项目，并将其与开放且非营利的替代方案 Eurosky 进行对比。 这一批评揭示了欧洲数字主权的政治言论与实际执行之间的差距，质疑 W Social 是为公共利益服务还是为政治议程服务。 W Social 是一家有限责任公司，以盈利为目的，其创始人具有金融背景。相比之下，Eurosky 由非营利基金会基于 AT Protocol 构建，完全透明。

hackernews · nemoniac · Jun 18, 12:46 · [社区讨论](https://news.ycombinator.com/item?id=48584497)

**背景**: 欧洲数字主权是指欧盟通过发展自己的数字基础设施来减少对非欧洲科技巨头依赖的雄心。W Social 和 Eurosky 是创建欧洲社交媒体平台的两种尝试，但它们在治理和透明度上存在根本差异。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://eurosky.tech/">Eurosky - Building a thriving open social web for Europe</a></li>

</ul>
</details>

**社区讨论**: 评论者对 W Social 的真实性表示怀疑，有人称其为“带有欧洲口音的 Truth Social”，并指出其与 Eurosky 相比缺乏透明度。其他人则质疑其盈利动机和政治背景。

**标签**: `#digital sovereignty`, `#social media`, `#European politics`, `#tech criticism`

---

<a id="item-15"></a>
## [Datasette Apps：沙盒化 HTML/JS 应用支持 SQL 查询](https://simonwillison.net/2026/Jun/18/datasette-apps/#atom-everything) ⭐️ 7.0/10

Simon Willison 发布了 datasette-apps 插件，允许在 Datasette 内部托管沙盒化的 HTML+JavaScript 应用，这些应用可以对底层数据执行只读和配置好的写入 SQL 查询。 该插件将 Datasette 从数据探索工具转变为一个直接在 SQLite 数据库之上构建自定义交互式 Web 应用的平台，极大地扩展了其使用场景。 应用在沙盒化的 iframe 中运行，带有 `allow-scripts allow-forms` 和注入的 CSP 头，阻止出站 HTTP 请求，防止数据泄露。该插件还注册了创建、查看、编辑和删除应用的权限。

rss · Simon Willison · Jun 18, 23:58

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具，拥有扩展其功能的插件系统。datasette-apps 插件最初是为了给 Datasette Agent 构建类似 Claude Artifacts 的机制，但后来被泛化为一个独立功能。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://pypi.org/project/datasette-apps/">Create apps that live inside Datasette</a></li>
<li><a href="https://datasette.io/tools/datasette-app">datasette - app - a tool for Datasette</a></li>
<li><a href="https://architecturenotes.co/p/datasette-simon-willison">Arc Note: Datasette - Simon Willison - by Mahdi Yusuf</a></li>

</ul>
</details>

**标签**: `#datasette`, `#plugin`, `#sql`, `#web-applications`, `#sandbox`

---

<a id="item-16"></a>
## [多款婴幼儿纸尿裤检出生殖毒性物质甲酰胺](https://www.sohu.com/a/1038121771_122014422) ⭐️ 7.0/10

《经济参考报》委托专业机构检测发现，好奇、碧芭宝贝、Babycare 等品牌婴幼儿纸尿裤中检出生殖毒性物质甲酰胺，部分婴幼儿血液和尿液中也有检出，一名记者穿戴一款纸尿裤一夜后血液浓度飙升近一倍。 这一发现暴露了中国纸尿裤国家标准的关键监管空白——尽管甲酰胺已知具有生殖毒性，但现行标准未设限值。由于婴幼儿对毒性物质蓄积尤为敏感，该发现构成严重的公共健康风险，并引发修订标准的迫切呼声。 甲酰胺被欧盟归类为 1B 类生殖毒性物质，在中国化妆品中明令禁用，但现行纸尿裤国标 GB/T 28004.1-2021 未将其纳入检测。该物质可通过皮肤吸收并在体内蓄积，婴幼儿器官发育不健全、代谢能力弱，风险更高。

telegram · zaihuapd · Jun 18, 07:09

**背景**: 甲酰胺是一种用于某些工业过程的化学物质，也可能是某些材料的副产物。此前已在婴儿爬行垫等儿童产品中检出，持续引发对婴童用品安全的担忧。中国现行婴儿纸尿裤国标（GB/T 28004.1-2021）未对甲酰胺设定限值或检测要求，存在监管空白，业内人士和专家呼吁尽快填补。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.21jingji.com/article/20260618/herald/ec6cf982d003c7201f79a2a2ea409195.html">从爬行地垫到纸尿裤， 甲 酰 胺 反复“现身”拷问 婴 童用品质量安全 - 21...</a></li>
<li><a href="https://www.bjnews.com.cn/detail/1781760045169406.html">多款婴儿 纸 尿 裤 检 出 甲 酰 胺 ？ “好奇”等品牌回应， 国 标 尚无限值 — 新京报</a></li>
<li><a href="https://news.cnr.cn/rebang/20260618/t20260618_527666495.shtml">专业检测机构检出有毒物质 多款纸尿裤被指侵 害 婴 幼 儿 健康_央广网</a></li>

</ul>
</details>

**标签**: `#public health`, `#consumer safety`, `#regulatory gap`, `#infant products`, `#toxicology`

---

<a id="item-17"></a>
## [小米开源智能家居方案 Miloco 2.0](https://github.com/XiaoMi/xiaomi-miloco) ⭐️ 7.0/10

小米发布了 Miloco 2.0，这是一个开源的智能家居方案，利用摄像头输入和 MiMo 大模型来主动观察、推理并控制全屋设备。 此次发布标志着将大语言模型集成到实用智能家居系统的重要一步，有望实现更直观、更主动的家庭自动化。同时，它也降低了开发者构建 AI 驱动的智能家居应用的门槛。 Miloco 2.0 作为 OpenClaw 插件运行，需要 macOS 或 Linux（Windows 通过 WSL），至少 4 GB 内存和 256 GB 存储，并依赖云端 MiMo API，会产生持续费用。该项目仅限于非商业用途。

telegram · zaihuapd · Jun 18, 12:23

**背景**: Miloco 是小米的开源智能家居框架，利用 MiMo 大语言模型——一个轻量级、MIT 许可的 LLM 系列，专为智能体设计。OpenClaw 是一个开源 AI 智能体框架，允许通过插件扩展其功能。通过结合这些技术，Miloco 2.0 可以处理摄像头输入以理解家庭环境，并主动控制 IoT 设备。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://hyperosinsider.com/xiaomi-miloco-2-0-released-before-hyperos-4-smart-ai-open-source-solution/">Xiaomi Miloco 2 . 0 Released Before HyperOS... - HyperOS Insider</a></li>
<li><a href="https://en.wikipedia.org/wiki/Xiaomi_MiMo">Xiaomi MiMo - Wikipedia</a></li>
<li><a href="https://open-claw.bot/docs/tools/plugins/">OpenClaw Plugins : Extend Your AI Agent | OpenClaw</a></li>

</ul>
</details>

**标签**: `#smart home`, `#open source`, `#LLM`, `#Xiaomi`, `#IoT`

---

<a id="item-18"></a>
## [华为设定 Wi-Fi 7 专利费每台 0.5 美元](https://36kr.com/newsflashes/3858656955847687) ⭐️ 7.0/10

华为宣布 Wi-Fi 7 设备专利许可费率为每台 0.5 美元，可通过双边协议或专利池以 FRAND 原则获取授权。 这一费率为 Wi-Fi 7 许可设定了先例，可能影响设备制造商的成本并塑造行业标准。 截至 2024 年底，超过 12 亿部消费类电子设备获得了华为的 Wi-Fi 专利授权。该费率专门适用于 Wi-Fi 7 设备。

telegram · zaihuapd · Jun 19, 00:09

**背景**: Wi-Fi 7 是下一代无线标准，提供更高速度和更低延迟。FRAND（公平、合理、无歧视）原则确保专利持有人以公平条款许可标准必要专利。专利池提供一站式许可解决方案，降低交易成本。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.huawei.com/en/news/2026/6/ipr-license-wifi7">Huawei Announces Wi - Fi 7 Patent Licensing Rates... - Huawei</a></li>
<li><a href="https://en.wikipedia.org/wiki/Reasonable_and_non-discriminatory_licensing">Reasonable and non-discriminatory licensing - Wikipedia</a></li>

</ul>
</details>

**标签**: `#Wi-Fi 7`, `#patent licensing`, `#Huawei`, `#FRAND`

---