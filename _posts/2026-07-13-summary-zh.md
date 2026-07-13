---
layout: default
title: "Horizon Summary: 2026-07-13 (ZH)"
date: 2026-07-13
lang: zh
---

> From 29 items, 13 important content pieces were selected

---

1. [GPT-5.6 一小时内证明 50 年图论猜想](#item-1) ⭐️ 9.0/10
2. [xAI Grok CLI 默认上传整个代码库及密钥文件](#item-2) ⭐️ 9.0/10
3. [全球首款侵入式脑机接口医疗器械在中国获批上市](#item-3) ⭐️ 9.0/10
4. [vLLM v0.25.0：Model Runner V2 成为默认，移除 PagedAttention](#item-4) ⭐️ 8.0/10
5. [Claude Code 与 OpenCode 的 Token 开销对比](#item-5) ⭐️ 8.0/10
6. [陶哲轩用编码代理构建可视化应用](#item-6) ⭐️ 8.0/10
7. [George Hotz：LLM 创造价值，但前沿实验室无法捕获](#item-7) ⭐️ 8.0/10
8. [苹果起诉 OpenAI 窃取商业机密](#item-8) ⭐️ 8.0/10
9. [Chromium 148 的 Math.tanh 可识别操作系统](#item-9) ⭐️ 7.0/10
10. [AI 代理不应成为直接责任人](#item-10) ⭐️ 7.0/10
11. [谷歌反对欧洲网站屏蔽，美国反盗版立法加速](#item-11) ⭐️ 7.0/10
12. [欧盟拟对消费者保护失职的大型科技公司罚款](#item-12) ⭐️ 7.0/10
13. [中国电动汽车平均车龄仅 1.8 年，比手机还短](#item-13) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [GPT-5.6 一小时内证明 50 年图论猜想](https://www.qbitai.com/2026/07/447873.html) ⭐️ 9.0/10

OpenAI 的 GPT-5.6 Sol Ultra 使用 64 个子代理和一种新颖的提示策略，在一小时内自主证明了图论中存在 50 年之久的循环双覆盖猜想，并生成了 3 页 PDF 的证明。 这一成就表明，大型语言模型可以自主解决长期存在的数学猜想，可能加速数学和理论计算机科学的研究。它也展示了多智能体协作和高级推理在 AI 系统中的强大能力。 该证明将问题转化为有限域上的边标号和线性方程组问题，为每条边分配两个标签，使相同标签的边组成圈。OpenAI 公布了完整的提示（约 700 个字符），其中明确了验收标准、定义、边界条件和失败情形，并要求动态分配子代理和独立审查。

telegram · zaihuapd · Jul 12, 03:49

**背景**: 循环双覆盖猜想询问是否每个无桥无向图都存在一组圈，使得每条边恰好出现两次。该猜想由 W. T. Tutte、Itai 和 Rodeh、George Szekeres 以及 Paul Seymour 提出，已悬而未决约 50 年。GPT-5.6 是 OpenAI 的最新模型系列，其中 Sol 是最高能力层级，具备最大推理和多智能体模式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cycle_double_cover_conjecture">Cycle double cover conjecture</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT‑5.6: Frontier intelligence that scales with your ambition</a></li>
<li><a href="https://www.llmreference.com/model/gpt-5.6-sol">GPT-5.6 Sol - 1.05m context, multimodal | LLM Reference</a></li>

</ul>
</details>

**标签**: `#AI`, `#mathematics`, `#graph theory`, `#OpenAI`, `#multi-agent`

---

<a id="item-2"></a>
## [xAI Grok CLI 默认上传整个代码库及密钥文件](https://gist.github.com/cereblab/dc9a40bc26120f4540e4e09b75ffb547) ⭐️ 9.0/10

安全研究人员发现，xAI 的 Grok CLI 工具（版本 0.2.93）默认通过两个渠道自动将整个代码仓库和 .env 等敏感文件上传至 xAI 服务器，且没有有效的退出机制。 这对使用 Grok CLI 的开发者和组织构成严重的安全和隐私风险，因为专有代码和凭证可能在未经同意的情况下被泄露，削弱了对 AI 辅助开发工具的信任。 该工具将文件内容作为模型对话请求的一部分上传，同时将整个仓库以 git bundle 形式发送，即使提示词明确要求不要打开某个文件。关闭“改进模型”开关无法阻止上传。

telegram · zaihuapd · Jul 12, 04:19

**背景**: Grok CLI 是一个命令行工具，提供对 xAI 的 Grok AI 模型的对话式访问。它旨在通过读取和分析代码仓库来帮助开发者完成编码任务。Git bundle 是一种将整个 Git 仓库打包成单个文件以便传输的文件格式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://x.ai/cli">Grok Build | SpaceXAI</a></li>
<li><a href="https://git-scm.com/docs/git-bundle">Git - git-bundle Documentation</a></li>

</ul>
</details>

**社区讨论**: 社区表达了愤怒和担忧，许多人呼吁立即卸载 Grok CLI。一些人指出，xAI 在披露后通过服务端开关悄悄禁用了上传功能，但批评其缺乏透明度。

**标签**: `#security`, `#privacy`, `#AI tools`, `#data leakage`, `#xAI`

---

<a id="item-3"></a>
## [全球首款侵入式脑机接口医疗器械在中国获批上市](https://t.me/zaihuapd/42515) ⭐️ 9.0/10

国家药监局批准了全球首款侵入式脑机接口医疗器械——博睿康医疗科技（上海）有限公司的“植入式脑机接口手部运动功能代偿系统”上市。该系统旨在帮助颈段脊髓损伤所致四肢瘫患者恢复手部抓握功能。 此次批准标志着全球首个侵入式脑机接口医疗器械进入临床应用，可能彻底改变瘫痪患者的康复治疗。同时，它使中国处于神经技术监管和创新的前沿，上海计划到 2027 年实现高质量脑控和半侵入式脑机接口产品的临床应用。 该系统采用硬脑膜外微创植入和无线供能通信技术，连接气动手套辅助手部运动。临床试验显示，18 至 60 岁颈段脊髓损伤患者的手部抓握能力和生活质量显著提高。

telegram · zaihuapd · Jul 12, 14:39

**背景**: 脑机接口（BCI）实现大脑与外部设备的直接通信。侵入式 BCI 通过手术将电极植入大脑内部或表面，信号质量更高，但手术风险也大于非侵入式或半侵入式方式。此次获批是在中国加速脑机接口创新的背景下实现的，包括对临床急需设备给予优先审评审批，以及北京、上海等地推出行动方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.nmpa.gov.cn/zhuanti/cxylqx/cxylqxlm/20260313134742156.html?type=pc&m=">首款侵入式脑机接口医疗器械获批上市</a></li>
<li><a href="https://m.jiemian.com/article/14109273_microcontent.html">国家药监局：首款 侵 入 式 脑 机 接 口 医疗器械获批上市 | 界面新闻</a></li>
<li><a href="https://www.163.com/dy/article/KQ5H8KUB0530RMN7.html">163.com/dy/article/KQ5H8KUB0530RMN7.html</a></li>

</ul>
</details>

**标签**: `#brain-computer interface`, `#medical device`, `#neurotechnology`, `#rehabilitation`, `#regulatory approval`

---

<a id="item-4"></a>
## [vLLM v0.25.0：Model Runner V2 成为默认，移除 PagedAttention](https://github.com/vllm-project/vllm/releases/tag/v0.25.0) ⭐️ 8.0/10

vLLM v0.25.0 将 Model Runner V2 设为所有稠密模型的默认执行路径，移除了旧的 PagedAttention 实现，并引入了新的 Streaming Parser Engine 用于工具调用/推理解析。该版本还新增了对 LLaVA-OneVision-2 和 GLM-5 等多个新模型的支持，并使 Transformers 建模后端达到了与原生 vLLM 相当的性能。 此版本标志着 vLLM 的重大架构转变，将其执行核心整合到 Model Runner V2 上，有望带来更好的模块化、性能和可维护性。移除 PagedAttention 简化了代码库，并标志着 V1/MRv2 后端的成熟，使依赖 vLLM 进行生产推理的广大 LLM 开发者和运维人员受益。 Model Runner V2 现在支持 EVS（高效视频流）、实时嵌入、Mamba 混合模型的前缀缓存，以及带有完整 CUDA 图的动态推测解码。Transformers 后端获得了 FP8 MoE 支持，并迁移了 GPTBigCode/Starcoder2 和 RoBERTa 模型，达到了与原生 vLLM 相当的速度。

github · khluu · Jul 11, 20:06

**背景**: vLLM 是一个高性能的开源 LLM 推理和服务库，最初由加州大学伯克利分校开发。Model Runner V2 是一个重新设计的执行核心，解决了原始 V1 架构中的设计缺陷，提供了模块化的模型逻辑和 GPU 原生的输入准备。PagedAttention 是 vLLM 中的一项关键创新，实现了注意力计算的高效内存管理，但已被更新的后端所取代。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.vllm.ai/en/latest/design/model_runner_v2/">Model Runner V2 Design Document - vLLM</a></li>
<li><a href="https://vllm.ai/blog/2026-03-24-mrv2">Model Runner V2: A Modular and Faster Core for vLLM</a></li>
<li><a href="https://docs.vllm.ai/en/latest/design/paged_attention/">Paged Attention - vLLM</a></li>

</ul>
</details>

**标签**: `#vLLM`, `#LLM inference`, `#release`, `#performance`, `#open source`

---

<a id="item-5"></a>
## [Claude Code 与 OpenCode 的 Token 开销对比](https://systima.ai/blog/claude-code-vs-opencode-token-overhead) ⭐️ 8.0/10

一项实证研究发现，Claude Code 在读取用户提示前会发送约 33,000 个 token，而 OpenCode 仅发送约 7,000 个 token，揭示了两款 AI 编码工具在 token 效率上的显著差异。 这很重要，因为 token 使用量直接影响按 token 付费的开发者的成本，而巨大的开销引发了关于工具提供商同时销售 token 时潜在利益冲突的担忧，以及子代理编排的效率问题。 该研究在编码工具与 Anthropic 端点之间添加了日志记录，以捕获所有请求和使用情况，发现 Claude Code 的缓存策略和 harness token 使用效率远低于 OpenCode。

hackernews · systima · Jul 12, 18:25 · [社区讨论](https://news.ycombinator.com/item?id=48883275)

**背景**: 像 Claude Code 和 OpenCode 这样的 AI 编码工具充当代理编排器，协调 AI 模型以辅助软件开发。它们在处理用户请求之前会发送系统提示和上下文 token，这些 token 会计入 API 使用成本。Token 效率是注重成本的开发者的关键指标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://code.claude.com/docs/en/costs">Manage costs effectively - Claude Code Docs</a></li>
<li><a href="https://www.truefoundry.com/blog/opencode-token-usage-how-it-works-and-how-to-optimize-it">OpenCode Token Usage: How It Works and How to Optimize It</a></li>
<li><a href="https://computingforgeeks.com/reduce-claude-code-token-usage-tools/">How to Reduce Claude Code Token Usage (10 Tested Tools) Claude Code Token Optimization: Full System Guide (2026) Claude Code Usage Dashboard - GitHub Maciek-roboblog/Claude-Code-Usage-Monitor - GitHub 18 Claude Code Token Hacks : Stop Wasting Money - Geeky Gadgets</a></li>

</ul>
</details>

**社区讨论**: 社区评论指出，子代理会大量消耗 token，有用户报告单个任务启动了 7 个子代理。其他人怀疑 Anthropic 存在利益冲突，因为他们既销售 token 又提供工具，并且有人指出效率对提供商来说利润较低。研究作者计划用更详细的任务比较来更新帖子。

**标签**: `#AI coding tools`, `#token efficiency`, `#cost analysis`, `#Claude Code`, `#OpenCode`

---

<a id="item-6"></a>
## [陶哲轩用编码代理构建可视化应用](https://terrytao.wordpress.com/2026/07/11/old-and-new-apps-via-modern-coding-agents/) ⭐️ 8.0/10

著名数学家陶哲轩展示了使用现代编码代理（基于 LLM 的工具）快速创建交互式可视化和应用程序，例如一个简化的 8 位计算机模拟器，突显了 AI 对非软件专家的实际效用。 这表明 LLM 正在释放传统软件开发之外的潜在需求，使领域专家能够构建他们以前缺乏时间或技能的工具，可能加速各领域的研究和教育。 陶哲轩指出，虽然 LLM 编码的补充内容并非关键任务，但使用与 LLM 代理的引导式交互来生成此类可视化的风险是可接受的，这反映了对 AI 工具的平衡信任。

hackernews · subset · Jul 12, 11:09 · [社区讨论](https://news.ycombinator.com/item?id=48880170)

**背景**: 现代编码代理，如 Claude Code 和 GitHub Copilot，已从基于聊天的助手演变为自主执行循环，允许用户通过自然语言提示生成代码。这一转变降低了软件创建的门槛，使非程序员能够构建自定义工具。陶哲轩的博文通过展示一位数学家如何快速原型化教育可视化，体现了这一趋势。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.augmentcode.com/tools/8-top-ai-coding-assistants-and-their-best-use-cases">8 Best AI Coding Assistants [Updated May 2026] | Augment Code</a></li>
<li><a href="https://medium.com/@dave-patten/the-state-of-ai-coding-agents-2026-from-pair-programming-to-autonomous-ai-teams-b11f2b39232a">The State of AI Coding Agents (2026): From Pair Programming to Autonomous AI Teams | by Dave Patten | Medium</a></li>
<li><a href="https://www.allankelly.net/archives/584/supply-demand-in-software-development/">Supply & Demand in software development - Allan Kelly</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为 LLM 释放了软件的潜在需求，有人指出需要 10 年才能赶上新能力。其他人强调了关于信任的平衡观点，一位用户分享了为计算机科学课程构建可视化的成功。一位评论者幽默地预测陶哲轩很快会像其他人一样为 Docker 发愁。

**标签**: `#LLM`, `#coding agents`, `#software development`, `#AI tools`, `#visualization`

---

<a id="item-7"></a>
## [George Hotz：LLM 创造价值，但前沿实验室无法捕获](https://geohot.github.io//blog/jekyll/update/2026/07/12/i-love-llms.html) ⭐️ 8.0/10

George Hotz 发表博客文章，认为虽然 LLM 创造了巨大价值，但由于商品化，前沿 AI 实验室无法捕获这些价值，真正的生产力提升体现在私有的定制化软件中，而非面向公众的产品。 这一批评挑战了前沿 AI 实验室的高估值，并表明 AI 的经济效益将更广泛地分布，可能重塑投资策略和开源生态系统。 Hotz 强调，LLM 的商品化意味着前沿实验室无法维持高价，最显著的生产力提升发生在借助 LLM 构建的私有一次性软件中，而非大众市场产品。

hackernews · therepanic · Jul 12, 18:31 · [社区讨论](https://news.ycombinator.com/item?id=48883343)

**背景**: 像 GPT-4 这样的大型语言模型（LLM）已广泛可用，导致商品化，许多提供商以竞争性价格提供类似能力。前沿实验室指 OpenAI、Google DeepMind 和 Anthropic 等领先 AI 研究机构。Hotz 的观点与历史模式一致，即基础设施商品化将价值转移到基于其构建的应用和服务上。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.linkedin.com/pulse/commoditization-ai-models-implications-innovation-siddharth-bhalsod-seimf">The Commoditization of AI Models: Implications for Innovation</a></li>
<li><a href="https://www.unite.ai/are-ai-models-becoming-commodities/">Are AI Models Becoming Commodities? - Unite.AI</a></li>
<li><a href="https://www.forbes.com/sites/joemckendrick/2024/02/07/as-ai-rapidly-becomes-a-commodity-time-to-consider-the-next-step/">As AI Rapidly Becomes A Commodity, Time To Consider ... - Forbes - The commoditization of AI models and compute AI model commoditization: a guide for COOs - ability.ai The Commoditization of AI — Eskridge.</a></li>

</ul>
</details>

**社区讨论**: 评论者大多同意 Hotz 的价值捕获论点，指出前沿实验室正在推动基于 token 的定价以捕获价值，但许多人发现私有的定制化 LLM 使用更高效。一些人担心开源未来，因为分叉变得更容易，而另一些人指出 Sonnet 4 和 Opus 4.5 等新模型正在加速进展，使时间线变得不确定。

**标签**: `#LLMs`, `#AI hype`, `#open source`, `#productivity`, `#value capture`

---

<a id="item-8"></a>
## [苹果起诉 OpenAI 窃取商业机密](https://t.me/zaihuapd/42502) ⭐️ 8.0/10

2026 年 7 月 10 日，苹果在美国加州北区联邦法院对 OpenAI、两名前员工（Chang Liu 和 Tang Yew Tan）以及 io Products 提起诉讼，指控其系统性窃取与产品设计、制造工艺和供应链策略相关的商业机密，以加速 OpenAI 的硬件业务。 这起诉讼凸显了 AI 公司与老牌科技巨头之间在人才和知识产权方面的紧张关系升级，并可能为商业秘密法如何适用于快速增长的 AI 硬件领域树立先例。 苹果声称，前员工 Chang Liu 在离职后仍访问内部网络并下载了数十份硬件文件，而硬件负责人 Tang Yew Tan 被指将供应商信息发送至个人邮箱，并要求求职者携带苹果零部件参加面试。诉讼还指出，目前有超过 400 名前苹果员工在 OpenAI 工作。

telegram · zaihuapd · Jul 11, 16:29

**背景**: OpenAI 主要以 GPT-4 等 AI 模型闻名，近年来正扩展至硬件领域，于 2025 年 5 月收购了由前苹果设计总监 Jony Ive 创立的 io Products。诉讼指控 OpenAI 的硬件业务建立在窃取的苹果商业机密之上，使其“从核心开始腐烂”。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.macrumors.com/2026/07/10/apple-sues-openai/">Apple Sues OpenAI for Stealing Trade Secrets to Build AI Hardware</a></li>
<li><a href="https://www.engadget.com/2212759/apple-calls-openais-hardware-business-rotten-to-its-core-in-trade-secret-theft-lawsuit/">Apple Calls OpenAI 's Hardware Business 'Rotten To Its Core' In...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Io_Products">Io Products</a></li>

</ul>
</details>

**标签**: `#Apple`, `#OpenAI`, `#lawsuit`, `#trade secrets`, `#hardware`

---

<a id="item-9"></a>
## [Chromium 148 的 Math.tanh 可识别操作系统](https://scrapfly.dev/posts/browser-math-os-fingerprint/) ⭐️ 7.0/10

Chromium 148 中 Math.tanh 的实现因操作系统而异，使得一种新的浏览器指纹技术可以通过单次函数调用推断底层操作系统。 这引入了一种新颖且难以伪造的指纹向量，即使修改了 User-Agent 标头也能揭示操作系统，影响用户隐私并使反指纹技术复杂化。 该技术利用了不同操作系统数学库中浮点运算的差异；例如，tanh(-0.35898351519709742) 在 Linux 上得到 -0.34431837261747228，在 Windows 上得到 -0.34431837261747222。

hackernews · joahnn_s · Jul 12, 21:12 · [社区讨论](https://news.ycombinator.com/item?id=48884853)

**背景**: 浏览器指纹技术通过收集设备和浏览器特征来识别用户，无需使用 Cookie。常见技术包括 Canvas、WebGL 和音频指纹。Math.tanh 是双曲正切函数，其实现因不同数学库和硬件而异，从而产生新的指纹信号。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fingerprint.com/blog/browser-fingerprinting-techniques/">Browser Fingerprinting Techniques : 6 Top Methods Explained</a></li>
<li><a href="https://github.com/numpy/numpy/issues/9187">numpy.tanh gives different results on Windows and Linux #9187</a></li>
<li><a href="https://learn.microsoft.com/en-us/dotnet/api/system.math.tanh?view=net-10.0">Math.Tanh (Double) Method (System) | Microsoft Learn</a></li>

</ul>
</details>

**社区讨论**: 评论者指出该技术可能还能识别浏览器版本范围，并批评文章可能是 AI 生成的。其他人认为正确舍入的超越函数可以缓解此类问题，而一些人则对披露该技术的抓取公司的动机表示怀疑。

**标签**: `#browser fingerprinting`, `#Chromium`, `#privacy`, `#JavaScript`, `#operating system`

---

<a id="item-10"></a>
## [AI 代理不应成为直接责任人](https://simonwillison.net/2026/Jul/12/directly-responsible-individuals/#atom-everything) ⭐️ 7.0/10

Simon Willison 认为，AI 代理永远不应被指定为直接责任人（DRI），因为它们无法对结果负责。 这引发了关于在越来越多部署 AI 代理的组织中问责制的关键问题，可能影响公司如何分配责任以及将 AI 整合到决策过程中。 DRI 概念起源于 Apple，在 GitLab 手册中被定义为对项目成败最终负责的人。Willison 引用了 IBM 1979 年的一张培训幻灯片，其中指出计算机绝不能做出管理决策，因为它无法被问责。

rss · Simon Willison · Jul 12, 23:57

**背景**: 直接责任人（DRI）是 Apple 提出的术语，指对项目或计划最终负责的单一人员。GitLab 在其手册中采纳并正式化了这一概念，强调明确的归属。随着基于大语言模型的代理在更自主的角色中部署，关于 AI 问责制的辩论日益激烈。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://handbook.gitlab.com/handbook/people-group/directly-responsible-individuals/">Directly Responsible Individuals (DRI) - The GitLab Handbook</a></li>
<li><a href="https://tettra.com/article/directly-responsible-individuals-guide/">Directly Responsible Individuals : The What, How and Why of... - Tettra</a></li>
<li><a href="https://www.bitesizelearning.co.uk/resources/directly-responsible-individual-dri-apple">Using the Directly Responsible Individual (DRI) concept at work...</a></li>

</ul>
</details>

**标签**: `#accountability`, `#AI agents`, `#organizational design`, `#software engineering`

---

<a id="item-11"></a>
## [谷歌反对欧洲网站屏蔽，美国反盗版立法加速](https://torrentfreak.com/google-opposes-site-blocking-in-europe-as-u-s-piracy-blocking-plans-gain-momentum/) ⭐️ 7.0/10

谷歌正式反对在欧洲扩大网站屏蔽措施，称屏蔽 DNS 解析器、IP 地址和 VPN 的做法无效且不成比例；与此同时，美国国会正在推进类似的反盗版立法。 这凸显了欧美在版权执法上的政策分歧，谷歌的立场可能影响未来的互联网治理。结果将影响全球在线服务和用户访问内容的方式。 谷歌举例称，意大利的反盗版系统曾误封 Google Drive 子域名以及托管 4200 万域名的 Cloudflare IP 地址。该公司主张提供更好的合法替代服务，而非扩大屏蔽措施。

telegram · zaihuapd · Jul 11, 15:10

**背景**: 网站屏蔽是指互联网服务提供商或 DNS 提供商阻止访问特定网站，常用于版权执法。DNS 解析器将域名转换为 IP 地址，VPN 可绕过此类屏蔽。谷歌向欧盟委员会提交的文件反映了其在版权保护与互联网自由之间寻求平衡的立场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://veyvin.com/archives/github-trending-2025-11-12-serverless-dns-serverless-dns">Serverless DNS ：重新思考 DNS 解 析 的云原生方案 | 小伞帝</a></li>
<li><a href="https://www.cloudflare.com/ips/">IP Ranges | Cloudflare</a></li>

</ul>
</details>

**标签**: `#internet governance`, `#copyright`, `#site blocking`, `#Google`, `#policy`

---

<a id="item-12"></a>
## [欧盟拟对消费者保护失职的大型科技公司罚款](https://www.ft.com/content/25640be5-a5bd-4548-81f9-bd0e16f87f35) ⭐️ 7.0/10

欧盟司法专员 Michael McGrath 宣布，欧盟委员会计划在今年年底前提出新立法，赋予欧盟对未能保护消费者（尤其是儿童）免受成瘾性设计、订阅陷阱及其他暗黑模式侵害的大型科技公司处以罚款的权力。 这标志着欧盟监管权力在现有数字服务法案等法律之外的显著扩展，可能迫使科技巨头重新设计用户界面和商业实践以避免巨额罚款。这也表明全球范围内追究平台对消费者伤害责任的趋势日益增强。 新规则将同时针对大型科技公司和小型在线商家及游戏开发商，欧盟寻求对跨境系统性案件的执法权。McGrath 指出，目前由成员国执行的消费者保护规则从未导致罚款，不足以威慑违法行为。

telegram · zaihuapd · Jul 12, 06:25

**背景**: 暗黑模式是欺骗或操纵用户做出非本意选择的用户界面设计，例如购买不需要的产品或分享个人数据。成瘾性设计指无限滚动或个性化推荐等功能，使用户过度沉迷。欧盟此前已通过决议关注这些问题，现在正转向具有约束力的立法。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dark_pattern">Dark pattern - Wikipedia</a></li>
<li><a href="https://www.omnesmag.com/en/news/the-european-parliament-takes-a-closer-look-at-addictive-design-on-online-platforms/">The European Parliament Takes a Closer Look at Addictive Design ...</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#consumer protection`, `#big tech`, `#dark patterns`, `#online safety`

---

<a id="item-13"></a>
## [中国电动汽车平均车龄仅 1.8 年，比手机还短](https://www.bloomberg.com/news/articles/2026-07-12/china-evs-average-1-8-years-on-road-less-than-cell-phones) ⭐️ 7.0/10

中国汽车工业协会与和君咨询的报告显示，中国上路电动汽车的平均车龄仅为 1.8 年，而燃油车为 8.2 年，这一数字甚至比智能手机的更换周期还短。 这种快速更替凸显了电池、软件和芯片的技术进步如何推动电动汽车升级，同时低残值促使车主更早换车。这标志着消费者行为正在转变，汽车被更多地视为消费电子产品，对汽车行业、二手车市场和环境可持续性产生重大影响。 使用三年后，电动汽车的平均残值仅为原价的 43.35%，低于燃油车。懂车帝数据显示，43%的电动车车主更换车辆的首要原因是升级智能功能与用户体验。

telegram · zaihuapd · Jul 12, 08:12

**背景**: 中国是全球最大的电动汽车市场，政府激励政策和激烈的竞争推动了快速普及。与传统汽车不同，电动汽车开发周期更短、软件更新更快，使其更像智能手机。由于电池衰减和技术快速过时，电动汽车低残值是一个已知问题。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://nev.ofweek.com/2026-06/ART-71008-8420-30692418.html">nev.ofweek.com/2026-06/ART-71008-8420-30692418.html</a></li>
<li><a href="https://www.163.com/dy/article/JNPNLEL90544W7WP.html">163.com/dy/article/JNPNLEL90544W7WP.html</a></li>
<li><a href="https://auto-time.36kr.com/p/335249487233026">电 动 车 开三年 残 值 仅剩1/3，威马小鹏探索 残 值 管理新模式_36氪</a></li>

</ul>
</details>

**标签**: `#electric vehicles`, `#China`, `#automotive industry`, `#technology adoption`, `#depreciation`

---