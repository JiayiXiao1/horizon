---
layout: default
title: "Horizon Summary: 2026-07-18 (ZH)"
date: 2026-07-18
lang: zh
---

> From 38 items, 21 important content pieces were selected

---

1. [Firefox 被编译为 WebAssembly 在浏览器中运行](#item-1) ⭐️ 9.0/10
2. [Kimi K3：2.8 万亿参数开源模型发布](#item-2) ⭐️ 9.0/10
3. [华为昇腾 950 超节点首次亮相，算力达英伟达 6.7 倍](#item-3) ⭐️ 9.0/10
4. [首次在宜居带岩质系外行星发现大气层](#item-4) ⭐️ 8.0/10
5. [开源 AI 模型崛起，威胁闭源对手](#item-5) ⭐️ 8.0/10
6. [GPT-5.6 Codex 漏洞可删除 $HOME 目录](#item-6) ⭐️ 8.0/10
7. [Thinking Machines Lab 发布开源权重模型 Inkling](#item-7) ⭐️ 8.0/10
8. [Linus Torvalds 声明 Linux 不反 AI](#item-8) ⭐️ 8.0/10
9. [Truth Social 将向华尔街出售特朗普帖子的实时访问权限](#item-9) ⭐️ 8.0/10
10. [特斯拉 Cybercab 在北美启动量产](#item-10) ⭐️ 8.0/10
11. [OpenAI CFO 提出“每美元有用智能”衡量 AI 投资回报](#item-11) ⭐️ 8.0/10
12. [豆包手机从 GUI 自动化转向 MCP 策略](#item-12) ⭐️ 8.0/10
13. [凯撒护士指责 AI 与监控导致护理质量下降](#item-13) ⭐️ 7.0/10
14. [Zilog Z80 微处理器迎来 50 周年纪念](#item-14) ⭐️ 7.0/10
15. [运行 SQLite 的实用技巧](#item-15) ⭐️ 7.0/10
16. [Kaggle 竞赛公正性因 AI 提交而受质疑](#item-16) ⭐️ 7.0/10
17. [通过改造高尔夫球场抵消数据中心用水](#item-17) ⭐️ 7.0/10
18. [欧盟拟要求 Android 向竞争对手 AI 助手开放](#item-18) ⭐️ 7.0/10
19. [1Password 集成 Claude，AI 安全代登录](#item-19) ⭐️ 7.0/10
20. [特朗普拟大幅缩短学生和记者签证有效期](#item-20) ⭐️ 7.0/10
21. [美议员要求封禁中国存储芯片并阻止其进入盟友供应链](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Firefox 被编译为 WebAssembly 在浏览器中运行](https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/#atom-everything) ⭐️ 9.0/10

Puter Labs 已将完整的 Firefox 浏览器（Gecko 引擎）编译为 WebAssembly，使其能够通过基于 WebSocket 的网络代理（使用 Wisp 协议）在另一个浏览器中运行。 这表明即使是像完整浏览器这样复杂的原生应用也可以移植到 Web 平台，可能为浏览器内沙箱、遗留软件访问和跨平台兼容性带来新的用例。 该项目使用了价值约 25,000 美元的 Claude Opus 和 Fable tokens（通过订阅降低了实际成本），演示通过 Puter 的服务器代理所有网络流量以绕过浏览器的网络限制。

rss · Simon Willison · Jul 16, 23:34

**背景**: WebAssembly (WASM) 是一种低级二进制指令格式，能在现代浏览器中以接近原生的速度运行。将像 Firefox 这样的完整浏览器编译为 WASM 是一项巨大的工程挑战，因为浏览器是复杂的多进程应用，且深度依赖操作系统。Puter 选择 Firefox/Gecko 是因为其强大的单进程支持，简化了移植工作。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/HeyPuter/firefox-wasm">GitHub - HeyPuter/ firefox -wasm: Firefox in WebAssembly · GitHub</a></li>
<li><a href="https://github.com/MercuryWorkshop/wisp-protocol">GitHub - MercuryWorkshop/ wisp - protocol : Wisp is a low-overhead...</a></li>
<li><a href="https://simonwillison.net/2026/Jul/16/firefox-in-webassembly/">Firefox in WebAssembly</a></li>

</ul>
</details>

**社区讨论**: Hacker News 上的讨论非常积极，许多人对这一技术成就印象深刻。一些人担心代理流量的成本，团队表示他们不得不扩展服务器以应对流量激增。

**标签**: `#WebAssembly`, `#Firefox`, `#browser`, `#compilation`, `#demo`

---

<a id="item-2"></a>
## [Kimi K3：2.8 万亿参数开源模型发布](https://t.me/zaihuapd/42619) ⭐️ 9.0/10

Moonshot AI 发布了 Kimi K3，这是一个拥有 2.8 万亿参数和 100 万 token 上下文长度的开源模型，声称综合水平仅次于 Claude Fable 5 和 GPT-5.6 Sol。 Kimi K3 是迄今为止最大的开源模型，挑战了闭源模型，可能使前沿 AI 能力更加普及。 该模型采用稀疏 MoE 架构，包含 896 个专家，每个 token 激活 16 个，并引入了 Kimi Delta Attention 和 Attention Residuals 以提高效率。

telegram · zaihuapd · Jul 17, 00:02

**背景**: 大型语言模型通常以参数数量和上下文长度衡量。混合专家模型 (MoE) 允许模型拥有大量参数，但每次推理只激活部分专家，从而控制成本。Kimi K3 的 2.8 万亿参数使其成为最大的开源权重模型，超过了 DeepSeek 的 1.6 万亿参数 V4 Pro。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://arxiv.org/pdf/2510.26692">KIMI LINEAR: AN EXPRESSIVE, EFFICIENT ATTENTION ARCHITECTURE</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mixture_of_experts">Mixture of experts - Wikipedia</a></li>

</ul>
</details>

**社区讨论**: 评论指出，“骑自行车的鹈鹕”测试可能已被训练数据污染，并注意到模型的高 tokenizer 计数暗示存在隐藏的系统提示。其他人则提出了更严格的智能体任务基准。

**标签**: `#AI`, `#LLM`, `#open-source`, `#Kimi`, `#Mixture of Experts`

---

<a id="item-3"></a>
## [华为昇腾 950 超节点首次亮相，算力达英伟达 6.7 倍](https://www.ithome.com/0/978/019.htm) ⭐️ 9.0/10

在 2026 世界人工智能大会上，华为首次公开展示了昇腾 950 超节点（Atlas 950 SuperPoD），宣称具备 1 EFLOPS FP8 和 2 EFLOPS FP4 算力，支持 1024 卡规模及 256 TB 全局统一内存。据中银证券报告，其总算力达到英伟达 144 卡 NVL144 系统的 6.7 倍。 这标志着 AI 硬件领域的一个重要里程碑，可能减少中国大规模 AI 训练对英伟达 GPU 的依赖。如果该性能声明得到验证，将重塑 AI 加速器的竞争格局，并影响全球供应链。 该超节点基于华为灵衢互联协议和超节点架构，实现 1024 卡规模扩展，时延低至 2.1 微秒。此外，昇腾 384 超节点已在互联网、运营商、金融等行业商用落地 750 多套，是国内唯一训练出 SOTA 模型的超节点。

telegram · zaihuapd · Jul 17, 10:27

**背景**: 超节点是一种高密度 AI 计算架构，通过高速互联将数十甚至上百个 AI 芯片整合在一起，用于大模型训练和推理。华为的灵衢协议旨在解决互联挑战，可靠性提升 100 倍，支持 200 米以上传输距离。昇腾 950 超节点直接对标英伟达使用 NVLink 的 NVL 系列。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.itbear.com.cn/html/2025-09/960596.html">华为发布灵衢互联协议与系列超节点，引领AI算力基础设施新变革-人工智能-ITBear科技资讯</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1953935616661255083">华为这一突破，意义非同寻常 - 知乎</a></li>
<li><a href="https://www.qbitai.com/2025/09/333834.html">华为发布AI超节点服务器Atlas 850，支持128台1024卡超节点集群</a></li>

</ul>
</details>

**标签**: `#AI Hardware`, `#Huawei`, `#Ascend`, `#SuperPod`, `#Compute Performance`

---

<a id="item-4"></a>
## [首次在宜居带岩质系外行星发现大气层](https://www.bbc.com/news/articles/cy4kdd1e0ejo) ⭐️ 8.0/10

詹姆斯·韦伯空间望远镜确认了 LHS 1140b 上存在大气层，这是一颗距地球约 48 光年的岩质系外行星，位于其红矮星的宜居带内。这是首次在宜居带内相对岩质的系外行星上确认大气层。 这一发现挑战了此前认为红矮星周围的岩质行星因强烈的恒星剥离作用而无法保留大气层的假设。它为后续大气特征研究提供了绝佳目标，并引发了关于 M 型矮星周围宜居性的新问题。 LHS 1140b 的质量约为地球的 5.6 倍，半径约为地球的 1.7 倍，属于超级地球类别。JWST 的发射光谱排除了迷你海王星的解释，确认了其岩质成分并存在大气层。

hackernews · neversaydie · Jul 17, 14:06 · [社区讨论](https://news.ycombinator.com/item?id=48947560)

**背景**: LHS 1140b 于 2017 年由 MEarth 项目发现，围绕一颗比太阳小得多且更冷的红矮星运行。红矮星以频繁的耀斑和强烈的恒星活动著称，这可能会剥离近距离行星的大气层。此类恒星周围的宜居带比类日恒星近得多，使得大气层的保留极具挑战性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/LHS_1140_b">LHS 1140 b</a></li>
<li><a href="https://science.nasa.gov/exoplanet-catalog/lhs-1140-b/">LHS 1140 b - NASA Science</a></li>
<li><a href="https://www.bbc.com/news/articles/cy4kdd1e0ejo">First atmosphere found around Earth-like planet LHS 1140b</a></li>

</ul>
</details>

**社区讨论**: 社区评论对红矮星宜居带内的岩质行星能够保留大气层表示惊讶，有用户指出 JWST 数据排除了迷你海王星的可能性。其他人讨论了太阳透镜望远镜和费米悖论等未来方向，也有人对“类地”标签表示怀疑。

**标签**: `#exoplanets`, `#JWST`, `#astronomy`, `#habitable zone`, `#red dwarf`

---

<a id="item-5"></a>
## [开源 AI 模型崛起，威胁闭源对手](https://stateofopensource.ai/) ⭐️ 8.0/10

开源 AI 模型在 OpenRouter 上的市场份额已超过闭源模型，四个月内从 40%增长到 63%，代币处理量增长了近 5 倍。 这一转变威胁到 OpenAI 和 Anthropic 等公司，因为开源模型使超大规模企业可以免费部署，苹果可以进行设备端优化，从而使 AI 商品化。 OpenRouter 的数据显示，开源模型在 3 月 19 日处理了 8880 亿个代币，最近处理了 4.19 万亿个代币，四个月内增长了 5 倍，表明采用率激增。

hackernews · rellem · Jul 17, 14:31 · [社区讨论](https://news.ycombinator.com/item?id=48947825)

**背景**: 开源 AI 模型以宽松许可证公开提供，允许任何人免费使用、修改和部署。闭源模型（如 OpenAI 和 Anthropic 的模型）是专有的，需要 API 访问或订阅。开源模型的崛起挑战了闭源 AI 公司的商业模式。

**社区讨论**: 评论者强调了市场的快速转变，有人指出开源模型现在在 OpenRouter 上以 63%-37%领先。一些人认为开源模型将使 AI 商品化，而另一些人则批评该演示文稿是 LLM 生成的，缺乏实质内容。

**标签**: `#open source`, `#AI`, `#machine learning`, `#market trends`, `#LLMs`

---

<a id="item-6"></a>
## [GPT-5.6 Codex 漏洞可删除 $HOME 目录](https://simonwillison.net/2026/Jul/16/bad-codex-bug/#atom-everything) ⭐️ 8.0/10

OpenAI 确认 GPT-5.6 Codex 存在一个漏洞：在启用完全访问模式且无沙箱保护的情况下，模型可能错误地删除用户的 $HOME 目录而非临时目录。 该漏洞凸显了具有无限制文件系统访问权限的 AI 编码代理的关键安全风险，可能导致依赖此类工具的开发者遭受不可逆的数据丢失。 该漏洞发生在启用完全访问模式、禁用沙箱和自动审查时，模型尝试将 $HOME 覆盖为临时目录路径，但错误地删除了真实的 $HOME。OpenAI 承诺将发布事后分析报告并修复工具。

rss · Simon Willison · Jul 16, 17:45

**背景**: GPT-5.6 Codex 是 OpenAI 最新的 AI 编码代理，能够执行终端命令并访问文件系统。完全访问模式会禁用沙箱，使模型获得无限制的文件系统访问权限。$HOME 环境变量指向用户的主目录，其中包含个人文件和配置。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai-codex.mintlify.app/concepts/sandboxing">Sandboxing - Codex CLI</a></li>
<li><a href="https://explainx.ai/blog/openai-codex-gpt-5-6-home-deletion-full-access-july-2026">Codex GPT-5.6 $HOME Deletion — Full Access | explainx.ai</a></li>
<li><a href="https://openai.com/index/gpt-5-6/">GPT-5.6: Frontier intelligence that scales with your ambition | OpenAI</a></li>

</ul>
</details>

**标签**: `#codex`, `#coding-agents`, `#generative-ai`, `#ai-safety`, `#bug`

---

<a id="item-7"></a>
## [Thinking Machines Lab 发布开源权重模型 Inkling](https://simonwillison.net/2026/Jul/16/inkling/#atom-everything) ⭐️ 8.0/10

由 Mira Murati 领导的 Thinking Machines Lab 发布了 Inkling，这是一个采用 Apache-2.0 许可的开源权重 975B 参数混合专家多模态模型，在 45 万亿个文本、图像、音频和视频 token 上训练而成。 Inkling 增强了美国开源权重生态系统，为中国开源模型提供了有竞争力的替代方案，并支持通过 Tinker 平台进行微调，尽管它并非前沿模型。 Inkling 总参数为 975B，每个 token 激活 41B 参数，并承诺推出更小的 276B（12B 激活）变体 Inkling-Small，但尚未发布。模型卡和训练数据文档明显简略。

rss · Simon Willison · Jul 16, 15:35

**背景**: 混合专家（MoE）是一种神经网络架构，使用多个并行专家子网络和门控机制，每个输入仅激活部分参数，从而提高效率。开源权重模型公开发布训练后的参数，允许下载和微调，但可能不包含完整的训练数据或代码。Apache-2.0 许可允许自由使用、修改和分发。

**标签**: `#AI`, `#open-weights`, `#multimodal`, `#Mixture-of-Experts`, `#Mira Murati`

---

<a id="item-8"></a>
## [Linus Torvalds 声明 Linux 不反 AI](https://simonwillison.net/2026/Jul/16/linus-torvalds/#atom-everything) ⭐️ 8.0/10

Linux 创始人 Linus Torvalds 在 Linux Media 邮件列表中声明，Linux 不是一个反 AI 的项目，AI 是一个明显有用的工具，他驳斥了反对意见，并邀请异议者分叉项目或离开。 来自 Linux 顶级维护者的强力支持标志着该项目在 AI 立场上的重大转变，可能影响更广泛的开源社区在开发中拥抱 AI 工具。 Torvalds 强调 AI 的有用性已不再有疑问，尽管他承认关于 AI 经济性等其他问题仍待解答。他是在 linux-media 邮件列表中针对持续辩论发表上述言论的。

rss · Simon Willison · Jul 16, 13:26

**背景**: Linux 内核是最大的开源项目之一，Linus Torvalds 是其创始人和顶级维护者。近期，一些开源项目采取了反 AI 政策，限制 AI 生成的代码贡献。Torvalds 的声明明确了 Linux 的立场，并拒绝了此类限制。

**标签**: `#Linux`, `#AI`, `#Open Source`, `#Kernel Development`

---

<a id="item-9"></a>
## [Truth Social 将向华尔街出售特朗普帖子的实时访问权限](https://www.cnn.com/2026/07/16/business/truth-social-data-wall-street) ⭐️ 8.0/10

特朗普媒体科技集团周四宣布，Truth Social 将于 8 月 1 日推出 Truth API，为机构客户提供毫秒级速度访问平台排名前 10 账号（包括特朗普总统账号）的实时帖子。 此举将特朗普的社交媒体影响力货币化，可能使算法交易者基于其政策声明获得信息优势——特朗普的帖子此前曾多次引发股市和油市剧烈波动。 该 API 面向高频算法交易者，提供毫秒级延迟的数据。TMTG 尚未公布定价，且该服务仅覆盖排名前 10 的账号，并非所有用户。

telegram · zaihuapd · Jul 17, 01:02

**背景**: Truth Social 是特朗普在被主流平台封禁后推出的社交媒体平台，已成为他宣布政策决定的主要渠道。其关于关税、伊朗及霍尔木兹海峡的帖子曾多次引发市场波动。CNN 调查还发现，特朗普曾利用 Truth Social 宣传自己刚买入的股票。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://fisf.fudan.edu.cn/show-80-3700.html?tid=0">施东辉： 高 频 交 易 ，天使还是魔鬼？ | 复旦大学国际金融学院(FISF)...</a></li>
<li><a href="https://invest.cnyes.com/usstock/detail/DJT">Trump Media & Technology Group Corp.</a></li>

</ul>
</details>

**标签**: `#Truth Social`, `#API`, `#financial markets`, `#algorithmic trading`, `#politics`

---

<a id="item-10"></a>
## [特斯拉 Cybercab 在北美启动量产](https://t.me/zaihuapd/42621) ⭐️ 8.0/10

特斯拉宣布其无方向盘、无踏板的无人驾驶电动车 Cybercab 已在北美启动量产。 这标志着自动驾驶汽车生产的重要里程碑，使特斯拉更接近推出 Robotaxi 服务，并可能重塑城市交通。 Cybercab 是一款双座全自动驾驶车辆，没有方向盘、踏板或后视镜，完全依靠车载 AI 驾驶。试生产于 2026 年 2 月开始，目标在 2026 年底前实现大规模生产。

telegram · zaihuapd · Jul 17, 03:06

**背景**: Robotaxi 是一种用于网约车服务的自动驾驶车辆，无需人类驾驶员。特斯拉的 Cybercab 专为此角色设计，旨在降低交通成本并提高可及性。该概念于 2024 年 10 月发布，特斯拉计划年产量高达 200 万辆。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Cybercab">Cybercab</a></li>
<li><a href="https://en.wikipedia.org/wiki/Robotaxi">Robotaxi</a></li>

</ul>
</details>

**标签**: `#Tesla`, `#autonomous driving`, `#electric vehicles`, `#robotaxi`

---

<a id="item-11"></a>
## [OpenAI CFO 提出“每美元有用智能”衡量 AI 投资回报](https://openai.com/index/a-scorecard-for-the-ai-age) ⭐️ 8.0/10

OpenAI 首席财务官 Sarah Friar 提出了一个名为“每美元有用智能”的新框架来衡量 AI 投资回报，将关注点从 token 成本转向交付的价值。该框架与 GPT-5.6 系列的发布一同宣布，其旗舰模型 Sol 在编码任务上创下新纪录，输出 token 比另一领先模型减少 54%。 这一指标可能重塑企业评估 AI 投资的方式，强调任务完成成本而非原始 token 定价。它提供了更全面的 AI 生产力视角，可能影响各行业的采用策略和供应商选择。 该框架包含四个维度：完成的有用工作量、每个成功任务的全成本、AI 输出的可靠性，以及随使用增长每美元投入是否产生更多价值。Friar 指出，最低 token 单价不等于最低任务成本，更强大的模型可能一次性给出正确答案，从而整体上更省钱。

telegram · zaihuapd · Jul 17, 15:00

**背景**: 传统上，软件投资回报通过用户数或许可证续签等采用指标来衡量。对于 AI，许多公司关注每次查询的 token 成本，但这忽略了完成工作的价值。新指标旨在捕捉 AI 产生的实际业务价值，与基于结果的定价趋势相一致。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.laozhang.ai/zh/posts/gpt-5-6-sol-vs-terra-vs-luna">GPT - 5 . 6 Sol 、Terra、Luna... | LaoZhang AI Blog</a></li>
<li><a href="https://juejin.cn/post/7661971304589901875">GPT - 5 . 6 Sol 、Terra、Luna...</a></li>

</ul>
</details>

**标签**: `#AI ROI`, `#OpenAI`, `#GPT-5.6`, `#enterprise AI`, `#productivity metrics`

---

<a id="item-12"></a>
## [豆包手机从 GUI 自动化转向 MCP 策略](https://www.latepost.com/news/dj_detail?id=3648) ⭐️ 8.0/10

豆包手机放弃了此前模拟点击超级应用的 GUI 自动化方式，转而要求阿里、腾讯等应用提供 MCP 服务并开放数据权限。备货量从 3 万台提升至数十万台。 这一转变反映了 AI 设备从脆弱的 GUI 自动化转向 MCP 等标准化协议进行应用集成的行业趋势，也凸显了手机厂商与超级应用之间对 AI 生态控制权的争夺。 豆包手机助手软件于 2025 年 7 月 15 日获得生成式人工智能服务备案，首个技术预览版于 2025 年 12 月发布。早期版本因 GUI 自动化被微信和淘宝封禁。

telegram · zaihuapd · Jul 18, 00:29

**背景**: GUI 自动化是指 AI 代理读取屏幕并模拟点击来控制应用，这种方式脆弱且常被应用开发者封禁。MCP（模型上下文协议）是一种开放标准，允许 AI 应用安全地访问服务的工具和数据，降低了开发复杂度并提高了可靠性。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://modelcontextprotocol.io/">What is the Model Context Protocol ( MCP )? - Model Context Protocol</a></li>
<li><a href="https://mcp.so/">MCP .so - MCP Marketplace</a></li>
<li><a href="https://eu.36kr.com/en/p/3896193801602697">Half a Year Post-Debut of the Doubao Phone : Why Are Step and...</a></li>

</ul>
</details>

**标签**: `#AI`, `#MCP`, `#smartphone`, `#ecosystem`, `#strategy`

---

<a id="item-13"></a>
## [凯撒护士指责 AI 与监控导致护理质量下降](https://localnewsmatters.org/2026/07/15/kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/) ⭐️ 7.0/10

据 CalMatters 报道，凯撒医疗集团的护士报告称，AI 和职场监控工具正在恶化他们的工作条件和患者护理质量。护士们表示，指标系统惩罚长时间通话，并将每次通话的建议限制在三条以内。 这凸显了医疗行业中成本优化与护理质量之间日益紧张的关系，因为 AI 驱动的监控正变得普遍。这场辩论强调了需要以道德方式部署 AI，以支持而非削弱临床工作。 文章提到 2024 年试点的 AI 共情工具已被终止，社区评论指出许多投诉是关于呼叫中心指标而非 AI 本身。一些护士认为 AI 工具（如实时翻译和笔记摘要）有价值。

hackernews · gnabgib · Jul 17, 22:26 · [社区讨论](https://news.ycombinator.com/item?id=48952880)

**背景**: 职场监控工具（常被称为“老板软件”）越来越多地被用于医疗行业，以监控员工生产力和协议遵守情况。这些工具可以追踪通话时长、患者互动甚至情绪语气，旨在降低成本，但有时会损害护理质量。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rbfirehose.com/2026/07/16/local-news-matters-kaiser-nurses-say-ai-workplace-surveillance-are-making-their-jobs-and-patient-care-worse/">Local News Matters: Kaiser nurses say AI, workplace surveillance ...</a></li>
<li><a href="https://www.nytimes.com/2026/03/01/business/bossware-work-surveillance-tools.html">Are ‘Bossware’ Tools Tracking You? - The New York Times</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍认为真正的问题是指标驱动的成本优化，而非 AI 本身。一些护士报告了使用 AI 工具的积极体验，而另一些则批评滥用指标来限制护理。一位评论者指出联合健康集团也存在类似问题。

**标签**: `#AI ethics`, `#healthcare`, `#workplace surveillance`, `#nurses`, `#Kaiser`

---

<a id="item-14"></a>
## [Zilog Z80 微处理器迎来 50 周年纪念](https://goliath32.com/blog/z80.html) ⭐️ 7.0/10

Zilog Z80 微处理器于 1976 年首次发布，现已迎来 50 岁生日，标志着计算史上的一个重要里程碑。 Z80 的长寿命及其对早期个人计算、嵌入式系统和业余电子领域的影响，使其周年纪念成为反思现代计算基础的重要时刻。 Z80 与 Intel 8080 二进制兼容，但在标志寄存器行为上存在差异，并重新利用了未定义的操作码，这可能导致兼容性问题。

hackernews · st_goliath · Jul 17, 19:41 · [社区讨论](https://news.ycombinator.com/item?id=48951461)

**背景**: Z80 是 Zilog 设计的 8 位微处理器，广泛应用于 Timex Sinclair 等家用电脑，以及嵌入式系统和游戏机。其指令集和寄存器架构使其在业余编程和教育中广受欢迎。

**社区讨论**: 社区评论表达了怀旧和技术赞赏，用户分享了学习汇编语言和构建基于 Z80 的套件的个人故事。一些人讨论了 Z80 与 8080 之间的兼容性细节。

**标签**: `#Z80`, `#retrocomputing`, `#microprocessor`, `#history`, `#embedded systems`

---

<a id="item-15"></a>
## [运行 SQLite 的实用技巧](https://jvns.ca/blog/2026/07/17/learning-about-running-sqlite/) ⭐️ 7.0/10

一篇博文分享了运行 SQLite 的实用技巧，包括备份策略和使用.expert 模式自动推荐索引。 这些技巧帮助开发者提升 SQLite 性能和数据安全性，解决了删除慢和备份复杂等常见痛点。 .expert 模式分析查询并建议索引，备份策略包括使用.dump 配合压缩以及 WAL 模式以避免阻塞写入者。

hackernews · surprisetalk · Jul 17, 17:45 · [社区讨论](https://news.ycombinator.com/item?id=48950122)

**背景**: SQLite 是一种轻量级嵌入式数据库引擎，广泛应用于应用程序中。.expert 模式是 CLI 的一个功能，可根据查询分析推荐索引。WAL（预写日志）允许并发读写。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://databaseschool.com/series/high-performance-sqlite/videos/41">Where to add indexes - High Performance SQLite - Database School</a></li>
<li><a href="https://sqlite.work/efficiently-persisting-sqlite-in-memory-databases-to-disk-with-minimal-overhead/">Efficiently Persisting SQLite In-Memory Databases... - SQLite Help Docs</a></li>

</ul>
</details>

**社区讨论**: 评论者分享了使用 zstd 压缩和 rsync 的实际备份脚本，并讨论了分批删除以避免性能问题。一位用户构建了一个工具来简化 AWS S3 凭证生成以用于备份。

**标签**: `#SQLite`, `#database`, `#backup`, `#performance`, `#tools`

---

<a id="item-16"></a>
## [Kaggle 竞赛公正性因 AI 提交而受质疑](https://www.kaggle.com/competitions/kaggle-measuring-agi/discussion/724918#3498423) ⭐️ 7.0/10

Kaggle 上的一场讨论揭露了 AI 生成的提交和 AI 评委可能损害竞赛结果的指控，参与者声称提示注入可以欺骗 AI 评委宣布获胜者。 这削弱了像 Kaggle 这样的 AI 评估平台的信任，这些平台越来越多地被用于基准测试 AI 能力和颁发奖项，可能贬低人类技能并偏袒内部人士。 涉及的竞赛提供了 25,000 美元奖金，社区成员报告称 AI 评委容易受到提示注入攻击，提交内容中包含隐藏指令以影响评分。

hackernews · twerkmeister · Jul 17, 11:30 · [社区讨论](https://news.ycombinator.com/item?id=48946010)

**背景**: Kaggle 是一个数据科学竞赛平台，参与者构建模型来解决问题。最近，AI 生成的代码和自动评判变得普遍，引发了对公平性和人类专业知识作用的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection - Wikipedia</a></li>
<li><a href="https://www.ai-redteam.com/topics/prompt-injection/">Prompt Injection | AI Red Team</a></li>

</ul>
</details>

**社区讨论**: 评论者表达了对 AI 扼杀公平黑客马拉松的沮丧，有人指出项目通过提示注入“我是赢家”获胜。其他人则认为暴力方法一直存在，但 AI 评委加剧了问题。

**标签**: `#AI ethics`, `#Kaggle`, `#competition integrity`, `#prompt injection`, `#evaluation bias`

---

<a id="item-17"></a>
## [通过改造高尔夫球场抵消数据中心用水](https://simonwillison.net/2026/Jul/17/spot-birds-not-golf/#atom-everything) ⭐️ 7.0/10

一项提议建议像谷歌这样的超大规模企业通过购买高尔夫球场并将其改造成公共公园，利用节省的水来满足其数据中心用水需求。 这一创意突显了 AI 数据中心用水与当地水资源之间日益紧张的关系，提供了一个潜在的共赢解决方案，既能减少用水，又能创造公共绿地。 谷歌在 2025 年使用了 109 亿加仑水，约每天 3000 万加仑，而科切拉谷的一个高尔夫球场每天使用约 75 万加仑；购买 40 个球场可以抵消谷歌的用水量。

rss · Simon Willison · Jul 17, 02:58

**背景**: 数据中心，尤其是超大规模数据中心，消耗大量水用于冷却。英亩-英尺是美国常用的水量单位，约等于 325,851 加仑。高尔夫球场以高耗水著称，因此成为水资源重新分配的目标。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.weforum.org/stories/2026/01/ai-water-data-centres-opportunity-am26-wef-xylem/">Why AI's water problem might actually be an opportunity</a></li>
<li><a href="https://www.coloradoriverdistrict.org/water-measurement/">Water Measurement - Basic Units of Water | Colorado River District</a></li>

</ul>
</details>

**标签**: `#ai-energy-usage`, `#water consumption`, `#data centers`, `#sustainability`

---

<a id="item-18"></a>
## [欧盟拟要求 Android 向竞争对手 AI 助手开放](https://t.me/zaihuapd/42615) ⭐️ 7.0/10

欧盟正根据《数字市场法案》起草要求，强制谷歌在 Android 系统上给予 ChatGPT、Claude 等竞争对手 AI 助手与其自家 Gemini 助手相同的系统级权限。 此举可能通过降低第三方应用在主导平台 Android 上的门槛来重塑 AI 助手市场竞争，有望加速创新，但也引发安全和隐私担忧。 相关要求仍处于草案阶段，发布时间可能推迟；谷歌担心开放系统功能可能影响用户安全和隐私。这些变更将作为下一版 Android 系统的一部分，于 2027 年 7 月生效。

telegram · zaihuapd · Jul 16, 13:19

**背景**: 《数字市场法案》（DMA）是欧盟的一项法律，将大型在线平台指定为“守门人”，并施加义务以确保公平竞争。谷歌的 Android 系统受 DMA 规则约束，欧盟此前曾因 Android 相关反垄断违规行为对谷歌处以罚款。该提案将 DMA 执法范围扩展到快速增长的 AI 助手市场。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.heise.de/en/news/EU-Requirements-Android-must-fully-open-up-for-third-party-AI-assistants-11367823.html">EU Requirements : Android must fully open up for... | heise online</a></li>
<li><a href="https://digital-markets-act.ec.europa.eu/index_en">Digital Markets Act</a></li>
<li><a href="https://techeconomy.ng/google-eu-digital-markets-act-android-search-data-ai-openai/">EU Orders Google to Share Android Features, Search Data with...</a></li>

</ul>
</details>

**标签**: `#EU regulation`, `#Android`, `#AI assistants`, `#antitrust`, `#Google`

---

<a id="item-19"></a>
## [1Password 集成 Claude，AI 安全代登录](https://9to5mac.com/2026/07/16/1password-now-lets-claude-sign-in-to-websites-without-seeing-your-passwords/) ⭐️ 7.0/10

1Password 推出了与 Anthropic 旗下 Claude 的 Mac 端集成，允许 AI 代理代用户登录网站，且密码和二次验证码全程不暴露给 AI 系统。 这是首个允许 AI 代理使用凭证但又不直接暴露凭证的浏览器集成，解决了代理式 AI 中的关键安全问题，可能为 AI 助手的凭证管理树立新标准。 凭证通过安全通道直接注入目标网页，用户需通过生物识别逐条审批当前会话的登录任务；若自动填充后提交失败，已填内容会被立即擦除。

telegram · zaihuapd · Jul 16, 15:54

**背景**: 像 1Password 这样的密码管理器为用户存储并自动填充凭证，但 AI 代理通常需要直接访问凭证才能执行任务，这带来了安全风险。1Password 的零暴露架构确保 AI 模型永远看不到秘密，保持密码管理器作为唯一可信源。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://1password.com/blog/1password-for-claude?cjdata=MXxOfDB8WXww&cjevent=521ad2f581fa11f1839802ae0a82b82c">1 Password for Claude : Give Claude access without giving up your...</a></li>
<li><a href="https://thenextweb.com/news/1password-claude-credential-zero-exposure-agentic-mode">1 Password lets Claude log you into websites without ever seeing your...</a></li>
<li><a href="https://www.helpnetsecurity.com/2026/07/17/1password-anthropic-claude-integration/">Claude can now sign into websites with... - Help Net Security</a></li>

</ul>
</details>

**标签**: `#password management`, `#AI integration`, `#security`, `#Claude`, `#1Password`

---

<a id="item-20"></a>
## [特朗普拟大幅缩短学生和记者签证有效期](https://t.me/zaihuapd/42623) ⭐️ 7.0/10

特朗普政府周三提出新规，将学生和交流访问签证最长有效期限制为四年，记者签证最长 240 天，中国公民记者仅为 90 天。 该政策可能严重干扰国际学生入学和学术交流项目，并限制新闻自由，尤其是针对报道美国的中国记者。 拟议规则将适用于 F-1 学生签证、J-1 交流访问签证和 I-1 媒体签证；签证持有者可申请延期，但需反复提交额外申请。

telegram · zaihuapd · Jul 17, 04:41

**背景**: 目前，F-1、J-1 和 I-1 签证通常在学习或工作任务期间有效。美国约有 160 万名持 F 类签证的国际学生，2024 财年共签发约 35.5 万份交流访问签证和 1.3 万份媒体签证。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.chineseherald.co.nz/news/education/trump-tightens-foreign-student-journalist-visa-rules/">chineseherald.co.nz/news/education/trump-tightens-foreign-student...</a></li>

</ul>
</details>

**标签**: `#immigration policy`, `#international students`, `#journalist visas`, `#US politics`, `#tech talent`

---

<a id="item-21"></a>
## [美议员要求封禁中国存储芯片并阻止其进入盟友供应链](https://www.tomshardware.com/pc-components/dram/lawmakers-want-us-government-to-ban-memory-chips-from-china-even-in-allied-supply-chains-citing-unacceptable-risk-to-national-economic-and-supply-chain-security) ⭐️ 7.0/10

美国众议院中国委员会主席 John Moolenaar 与民主党议员 George Whitesides 致信商务部长 Howard Lutnick，要求禁止美国公司采购中国存储芯片，并呼吁将长鑫存储（CXMT）列入实体清单，对长江存储（YMTC）施加额外限制。 此举可能严重扰乱全球半导体供应链，尤其是 DRAM 和 NAND 闪存领域，并可能迫使苹果等公司寻找替代来源，进而影响 AI 基础设施的发展。 议员们指出，中国存储芯片制造商与中国人民解放军关系密切，每笔采购都直接资助军民两用技术开发。他们还敦促与日本、韩国和欧盟协调，防止中国制造商在盟友供应链中扎根。

telegram · zaihuapd · Jul 17, 14:00

**背景**: 长鑫存储是中国领先的 DRAM 制造商，尚未被列入美国实体清单；而长江存储作为主要的 NAND 闪存生产商，已受到限制。美国出于国家安全考虑，越来越多地针对中国半导体公司，尤其是可能用于军事的军民两用技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.rfi.fr/cn/经贸/20260716-众议员致信美商务部长促禁购中国存储芯片-参议员提法案加强对中国在美制药业投资审查">rfi.fr/cn/经贸/20260716...</a></li>
<li><a href="https://gaohaojun.cn/Blog/2026/01/21/红色内存潮流长鑫存储的战略分析和围绕DRAM的地缘政治斗争/">内 存 的赤色潮流： 长 鑫 存 储 （ CXMT ... - Gao Haojun</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#trade policy`, `#supply chain`, `#China`, `#memory chips`

---