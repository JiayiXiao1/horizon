---
layout: default
title: "Horizon Summary: 2026-06-25 (ZH)"
date: 2026-06-25
lang: zh
---

> From 34 items, 20 important content pieces were selected

---

1. [OpenAI 携手 Broadcom 发布首款定制 AI 推理芯片 Jalapeno](#item-1) ⭐️ 9.0/10
2. [NVIDIA 45°C 冷却方案将数据中心用水降至接近零](#item-2) ⭐️ 8.0/10
3. [Nub：一个类似 Bun 的 Node.js 一体化工具包](#item-3) ⭐️ 8.0/10
4. [Krea 2：开源权重 12B 图像模型达到 SOTA](#item-4) ⭐️ 8.0/10
5. [LLM 生成的求职申请削弱真实性](#item-5) ⭐️ 8.0/10
6. [用生成式 AI 写作业可能降低中国学生考试成绩](#item-6) ⭐️ 8.0/10
7. [Cloudflare 联合浏览器厂商提议用 PACT 替代验证码](#item-7) ⭐️ 8.0/10
8. [美光 26Q3 营收暴增 346%，达 414.6 亿美元](#item-8) ⭐️ 8.0/10
9. [RubyLLM：一个覆盖所有主要 AI 提供商的 Ruby 框架](#item-9) ⭐️ 7.0/10
10. [GitHub 上的 PR 垃圾信息堪比 2000 年代初的邮件垃圾](#item-10) ⭐️ 7.0/10
11. [谷歌为 Gemini 3.5 Flash 添加计算机使用功能](#item-11) ⭐️ 7.0/10
12. [卡马克反思 id Software 早期错误](#item-12) ⭐️ 7.0/10
13. [Bunny.net 推出免费 DNS 服务，无查询限制](#item-13) ⭐️ 7.0/10
14. [Datasette 1.0a35 新增创建/修改表界面和 JSON API](#item-14) ⭐️ 7.0/10
15. [不精准洗牌需 14 次才能随机化一副牌](#item-15) ⭐️ 7.0/10
16. [LastPass 客服数据因 Klue 泄露被盗](#item-16) ⭐️ 7.0/10
17. [特朗普不再视 Anthropic 为国安威胁](#item-17) ⭐️ 7.0/10
18. [台积电先进制程全线涨价](#item-18) ⭐️ 7.0/10
19. [字节跳动否认与博通合作开发 AI 芯片的报道](#item-19) ⭐️ 7.0/10
20. [新版 Siri 拖累 Spotlight 搜索，用户不满](#item-20) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [OpenAI 携手 Broadcom 发布首款定制 AI 推理芯片 Jalapeno](https://techcrunch.com/2026/06/24/openai-unveils-its-first-custom-chip-built-by-broadcom/) ⭐️ 9.0/10

OpenAI 与 Broadcom 联合发布了专为大语言模型设计的定制 AI 推理芯片 Jalapeno，该芯片由台积电制造，并在 OpenAI 自身模型的辅助下于九个月内完成开发。 这标志着 OpenAI 战略性进入定制 AI 硬件领域，有望减少对 NVIDIA GPU 的依赖，并提升其服务的推理效率和降低成本。 该芯片针对大语言模型推理而非训练进行了优化，由 Broadcom 和 Celestica 共同开发，负责芯片实现、板卡及机架系统集成。OpenAI 声称其自身 AI 模型加速了设计过程。

hackernews · jamdesk · Jun 24, 17:47 · [社区讨论](https://news.ycombinator.com/item?id=48663324)

**背景**: AI 推理芯片是运行已训练好的 AI 模型以生成响应的专用处理器，与用于训练模型的训练芯片不同。目前大多数 AI 公司依赖 NVIDIA 的 GPU 进行训练和推理。像 Google 的 TPU 和 Amazon 的 Trainium 等定制芯片已在特定工作负载上展现出显著的效率提升。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://openai.com/index/openai-broadcom-jalapeno-inference-chip/">OpenAI and Broadcom unveil LLM-optimized inference chip</a></li>
<li><a href="https://seekingalpha.com/news/4606697-broadcom-and-openai-heat-up-ai-chip-market-with-inference-processor-jalapeno">Broadcom and OpenAI heat up AI chip market with inference processor Jalapeño | Seeking Alpha</a></li>
<li><a href="https://interestingengineering.com/ai-robotics/openai-jalapeno-ai-inference-chip-broadcom">OpenAI unveils Jalapeño chip for large-scale inference workloads</a></li>

</ul>
</details>

**社区讨论**: 评论者对 OpenAI 声称其模型加速了芯片设计表示怀疑，认为这可能是营销噱头。其他人则讨论了推理芯片的技术优势，包括将权重固化到 ROM 以实现极致效率的想法，并将 Jalapeno 与 Google 的 TPU 和 Taalas 等其他定制芯片进行了比较。

**标签**: `#AI hardware`, `#OpenAI`, `#semiconductors`, `#inference chip`, `#Broadcom`

---

<a id="item-2"></a>
## [NVIDIA 45°C 冷却方案将数据中心用水降至接近零](https://blogs.nvidia.com/blog/liquid-cooling-ai-factories/) ⭐️ 8.0/10

NVIDIA 推出了一种用于 AI 数据中心的 45°C 直接芯片液冷架构，大幅降低用水量，并可能实现区域供热集成。 这一创新解决了 AI 基础设施日益增长的用水和能源需求，使数据中心更加可持续，并通过废热回收开辟新的收入来源。 冷却液温度高达 45°C（113°F），高于传统液冷系统，在适宜气候下可完全消除水消耗。

hackernews · nitin_flanker · Jun 24, 14:10 · [社区讨论](https://news.ycombinator.com/item?id=48660178)

**背景**: 传统数据中心冷却依赖高能耗空调或低温液冷，蒸发过程消耗大量水。直接芯片液冷将冷却液直接流过发热组件，提高效率。区域供热网络从中央热源向建筑分配热量，数据中心废热可替代化石燃料使用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.guru3d.com/story/nvidia-unveils-liquid-cooling-design-for-ai-data-centers/">NVIDIA Unveils 45 ° C Liquid Cooling Design for AI Data Centers</a></li>
<li><a href="https://www.techbuzz.ai/articles/nvidia-s-45-c-liquid-cooling-redefines-ai-data-center-energy">NVIDIA's 45 ° C Liquid Cooling Redefines AI Data Center Energy</a></li>
<li><a href="https://www.araner.com/blog/data-center-and-district-heating-an-outstanding-combination">Data center and district heating: an outstanding combination</a></li>

</ul>
</details>

**社区讨论**: 评论者注意到区域供热的协同潜力，有人建议数据中心可向社区免费供热。其他人质疑“适宜气候”的定义，并希望获得更多关于温度与效率权衡的细节。还有人提到了 NASA 类似的高温冷却设施。

**标签**: `#data center cooling`, `#liquid cooling`, `#energy efficiency`, `#NVIDIA`, `#district heating`

---

<a id="item-3"></a>
## [Nub：一个类似 Bun 的 Node.js 一体化工具包](https://github.com/nubjs/nub) ⭐️ 8.0/10

Nub 是一个新的开源工具包，通过预加载钩子添加转译、模块解析和 polyfill，在原生 Node.js 上运行，从而提供类似 Bun 的开发体验。 Nub 弥合了 Node.js 与 Bun 开发体验之间的差距，无需切换运行时，使开发者能够在 Node 上无缝使用 TypeScript 和现代 API。 Nub 使用基于 oxc 的转译器（打包为 Node-API 插件），注册模块解析钩子，并为 Worker、Temporal 等 API 注入 polyfill。它由 Zod 的作者 Colin McDonnell 创建。

hackernews · colinmcd · Jun 24, 14:14 · [社区讨论](https://news.ycombinator.com/item?id=48660267)

**背景**: Bun 是一个快速的一体化 JavaScript 运行时，包含转译器、打包器和包管理器，提供无缝的开发体验。Node.js 传统上需要单独的工具进行 TypeScript 转译和模块解析。Nub 使用内置钩子将这些能力添加到原生 Node.js 中，成为切换运行时的轻量级替代方案。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://github.com/oxc-project/oxc">GitHub - oxc-project/oxc: ⚓ A collection of high-performance JavaScript tools.</a></li>

</ul>
</details>

**社区讨论**: 社区反应积极，用户称赞这个想法并报告成功采用。一些用户询问了 ESM 支持以及考虑到 Node 最近对 TypeScript 的支持是否需要转译器，作者对此进行了澄清。

**标签**: `#Node.js`, `#tooling`, `#TypeScript`, `#developer-experience`, `#open-source`

---

<a id="item-4"></a>
## [Krea 2：开源权重 12B 图像模型达到 SOTA](https://www.krea.ai/blog/krea-2-technical-report) ⭐️ 8.0/10

Krea 发布了开源权重的 Krea 2 Raw 和 Turbo 模型，这是一个 120 亿参数的扩散变换器，可在 2 秒内生成 2K 分辨率图像，并附有详细的技术报告，涵盖数据整理、架构和训练基础设施。 此次发布通过提供可在本地部署的顶级性能模型，使最先进的图像生成技术民主化，其性能优于所有其他本地可托管模型，并与 Ideogram 4 等仅限云端的解决方案相媲美。 该模型使用 Qwen Image VAE、12B 密集 DiT 主干网络和具有多层特征聚合的 Qwen3-VL 文本编码器；Turbo 变体经过引导和时间步蒸馏，可在 8 步内实现更快的推理。

hackernews · mattnewton · Jun 23, 15:31 · [社区讨论](https://news.ycombinator.com/item?id=48646659)

**背景**: 开源权重模型允许用户下载并在本地运行训练好的参数，提供隐私和定制化优势。扩散变换器（DiT）是一类将扩散过程与变换器架构相结合的生成模型，能够实现高质量的图像合成。Krea 2 的发布包含一个商业友好的许可证，鼓励更广泛的采用。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://alphasignal.ai/news/krea-opens-krea-2-s-12b-image-model-so-anyone-can-train-and-deploy">Krea Opens Krea 2's 12B Image Model So Anyone Can Train and Deploy | AlphaSignal</a></li>
<li><a href="https://www.krea.ai/krea-2-open-source">Krea 2 Open-Source: RAW and Turbo Image Models</a></li>
<li><a href="https://aiweekly.co/alerts/krea-releases-12b-image-weights-for-2-second-2k-generation">Krea Releases 12B Image Weights for 2-Second 2K Generation | AI Weekly</a></li>

</ul>
</details>

**社区讨论**: 社区称赞了详细的技术报告和模型的性能，指出它在本地可托管模型中得分最高，仅被速度慢得多的 Ideogram 4 击败。一些评论者对模型在更新的“代理组合”模型面前的相关性表示担忧，但总体情绪是积极的。

**标签**: `#image generation`, `#open-weights`, `#AI research`, `#machine learning`, `#deep learning`

---

<a id="item-5"></a>
## [LLM 生成的求职申请削弱真实性](https://simonwillison.net/2026/Jun/24/tom-macwright/#atom-everything) ⭐️ 8.0/10

Tom MacWright 观察到，越来越多的求职申请和作品集由 LLM 共同撰写，导致候选人变得难以区分且缺乏个性。 这一趋势侵蚀了真实性，削弱了招聘流程，使雇主更难评估候选人的真实匹配度，并可能贬低人类在专业环境中的创造力。 MacWright 指出，LLM 生成的作品集通常链接到 LLM 生成的 GitHub 项目，其提交信息也完全由 LLM 生成，让他对申请者本人毫无了解。

rss · Simon Willison · Jun 24, 18:13

**背景**: 大型语言模型（LLM），如 GPT-4，可以生成类似人类的文本，包括简历、求职信和代码。它们在求职申请中的广泛使用引发了关于真实性和招聘中个人声音丧失的担忧。

**标签**: `#AI`, `#careers`, `#hiring`, `#authenticity`, `#LLM`

---

<a id="item-6"></a>
## [用生成式 AI 写作业可能降低中国学生考试成绩](https://cepr.org/publications/dp21577) ⭐️ 8.0/10

一项对 26,811 名中国 7-12 年级学生、持续 30 个月的研究发现，使用生成式 AI 做作业使作业成绩平均提高 18%、完成时间减少 30%，但 6 个月内闭卷月考成绩平均下降约 20%，中考、高考等高风险考试成绩降低 18%–24%。 这项大规模纵向研究提供了有力证据，表明生成式 AI 可能削弱深度学习和长期学业表现，尤其是对那些将作业外包给 AI 的学生，这对教育者和政策制定者在课堂中整合 AI 具有重要启示。 负面影响因科目而异，社科科目损失最大，其次是理工科和语言；低年级、高成就学生和男生受影响更明显。约 80%的 AI 用户表现出“作业外包”特征——作业时间极短但分数高——这些学生承担了主要的成绩下降。

telegram · zaihuapd · Jun 24, 05:15

**背景**: 生成式 AI（如大型语言模型）能生成类似人类的文本并解决问题，因此对学生做作业很有吸引力。然而，当学生依赖 AI 完成作业而不深入理解材料时，他们可能无法发展闭卷考试所需的知识和技能。这项研究追踪学生 30 个月，全面展示了 AI 对学习的影响。

**标签**: `#generative AI`, `#education`, `#academic performance`, `#China`, `#research`

---

<a id="item-7"></a>
## [Cloudflare 联合浏览器厂商提议用 PACT 替代验证码](https://www.techtimes.com/articles/318891/20260623/cloudflare-chrome-firefox-plan-replace-captchas-cryptographic-tokens.htm) ⭐️ 8.0/10

Cloudflare 联合 Chrome、Firefox、Edge 及 Shopify 提出了 PACT 协议，拟用匿名加密令牌替代 CAPTCHA 进行用户验证。 该提案有望消除 CAPTCHA 令人沮丧的用户体验，同时增强整个网络的隐私保护和机器人检测能力，涉及主要浏览器厂商和领先的 CDN 提供商。 该协议基于 IETF 的 Privacy Pass，采用盲签名技术，也覆盖合法 AI 代理与恶意爬虫的区分；但目前仍是提案，未确定标准组织与时间表，苹果未加入。

telegram · zaihuapd · Jun 24, 06:30

**背景**: CAPTCHA 广泛用于区分人类与机器人，但常降低用户体验并引发隐私担忧。PACT 协议利用可信站点颁发的加密令牌，让用户在不泄露身份或浏览历史的情况下证明自己是人类，其基础是 Privacy Pass 框架和盲签名技术。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://privacypass.github.io/">Privacy Pass</a></li>
<li><a href="https://en.wikipedia.org/wiki/Blind_signature">Blind signature</a></li>

</ul>
</details>

**标签**: `#privacy`, `#security`, `#web standards`, `#CAPTCHA`, `#cryptographic tokens`

---

<a id="item-8"></a>
## [美光 26Q3 营收暴增 346%，达 414.6 亿美元](https://www.globenewswire.com/news-release/2026/06/24/3317151/14450/en/micron-technology-inc-reports-record-results-for-the-third-quarter-of-fiscal-2026.html) ⭐️ 8.0/10

美光科技公布 2026 财年第三季度财报，营收达 414.6 亿美元，同比增长 346%，净利润 282.4 亿美元（约每天净赚 3.1 亿美元）。 这一爆炸性增长凸显了 AI 基础设施对高带宽内存（HBM）的巨大需求，使美光成为 AI 热潮的主要受益者，并预示着内存紧缺将持续到 2027 年以后。 Non-GAAP 毛利率从去年同期的 39%飙升至 84.9%，数据中心营收暴增 653%至 115.2 亿美元。美光已大规模量产 HBM4，预计 HBM4E 将于 2027 年投产。

telegram · zaihuapd · Jun 24, 22:22

**背景**: 高带宽内存（HBM）是一种用于高性能 GPU 和 AI 加速器的 3D 堆叠 DRAM 接口。HBM4 和 HBM4E 是最新一代产品，提供更高的带宽和容量。Non-GAAP 毛利率剔除了股权激励等成本，更清晰地反映运营盈利能力。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/High_Bandwidth_Memory">High Bandwidth Memory - Wikipedia</a></li>
<li><a href="https://www.tomshardware.com/pc-components/dram/rambus-announces-hbm4-memory-controller-for-ai-gpus-controller-enables-up-to-of-256-tbs-per-hbm4-memory-stack-across-a-2048-bit-memory-bus">Rambus announces HBM 4 memory controller for AI... | Tom's Hardware</a></li>
<li><a href="https://nerds.xyz/2026/06/samsung-hbm4e-memory/">Samsung ships industry-first HBM 4 E memory as AI infrastructure race...</a></li>

</ul>
</details>

**标签**: `#semiconductors`, `#AI infrastructure`, `#memory`, `#Micron`, `#earnings`

---

<a id="item-9"></a>
## [RubyLLM：一个覆盖所有主要 AI 提供商的 Ruby 框架](https://rubyllm.com/) ⭐️ 7.0/10

RubyLLM 是一个 Ruby 框架，为 OpenAI、Anthropic 和 Ollama 等主要 AI 提供商提供统一接口，使开发者能够通过单一 API 构建 AI 驱动的应用程序。它在 Hacker News 上获得了大量社区关注，获得了 345 分和 55 条评论。 该框架简化了 Ruby 开发者的 AI 集成工作，减少了学习多个提供商特定 SDK 的需求。它的流行反映了 Ruby 生态中对 AI 工具日益增长的需求，可能加速 AI 在 Rails 应用中的采用。 RubyLLM 支持流式和非流式响应，并包含内置缓存，但用户报告在某些提供商（如 xAI）上存在缓存可靠性问题。该框架设计为有主见且高效，类似于 Rails 的理念。

hackernews · doener · Jun 24, 14:41 · [社区讨论](https://news.ycombinator.com/item?id=48660711)

**背景**: Ruby 开发者历来缺乏统一的 AI 客户端，通常需要为每个提供商使用单独的 gem。RubyLLM 通过提供单一、一致的 API 来填补这一空白，该 API 抽象了提供商的差异，使得在模型之间切换或在同一个项目中使用多个提供商变得更加容易。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://rubyllm.com/">RubyLLM | One beautiful Ruby framework for all major AI providers.</a></li>
<li><a href="https://github.com/crmne/ruby_llm">GitHub - crmne/ ruby _ llm : One delightful Ruby framework for every...</a></li>
<li><a href="https://medium.com/airtribe/rubyllm-and-the-return-of-rails-superpower-notes-from-euruko-2025-b72eeeb6b185">RubyLLM and the Return of Rails’ Superpower — Notes... | Medium</a></li>

</ul>
</details>

**社区讨论**: 社区反馈褒贬不一：许多人称赞 RubyLLM 的易用性和设计，但一些人对维护者的响应速度和缓存可靠性表示失望。用户还注意到 Responses API 现已原生支持，解决了之前的痛点。

**标签**: `#Ruby`, `#AI`, `#framework`, `#LLM`, `#developer tools`

---

<a id="item-10"></a>
## [GitHub 上的 PR 垃圾信息堪比 2000 年代初的邮件垃圾](https://www.greptile.com/blog/prs-on-openclaw) ⭐️ 7.0/10

Greptile 的一篇博文将 GitHub 上激增的垃圾拉取请求（PR）与 2000 年代初的邮件垃圾信息泛滥相类比，呼吁开发更好的审核工具。 这一对比凸显了开源维护者面临的一个日益严重的问题：低质量或自动化的 PR 泛滥成灾，威胁到项目健康和贡献者士气。 GitHub 最近引入了可配置的 PR 限制来帮助维护者管理贡献，但文章认为需要更复杂的审核手段，就像当年对付邮件垃圾一样。

hackernews · dakshgupta · Jun 24, 14:32 · [社区讨论](https://news.ycombinator.com/item?id=48660579)

**背景**: 拉取请求（PR）是 GitHub 上为开源项目做贡献的核心机制。近年来，AI 工具和自动化机器人的兴起导致垃圾 PR 大量涌入，这些 PR 通常包含琐碎或不相关的更改，浪费了维护者的时间。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.github.com/en/communities/maintaining-your-safety-on-github/reporting-abuse-or-spam">Reporting abuse or spam - GitHub Docs</a></li>
<li><a href="https://www.coderabbit.ai/blog/github-gives-maintainers-a-throttle-for-the-ai-pull-request">GitHub Adds PR Caps to Help Maintainers Combat AI Slop</a></li>

</ul>
</details>

**社区讨论**: 评论者指出了 PR 垃圾与邮件垃圾的区别，例如 PR 缺乏发送者信誉系统。有人建议采取非文字介绍或向项目捐赠代币积分等解决方案。

**标签**: `#open source`, `#spam`, `#GitHub`, `#maintainer tools`, `#community`

---

<a id="item-11"></a>
## [谷歌为 Gemini 3.5 Flash 添加计算机使用功能](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/) ⭐️ 7.0/10

谷歌宣布 Gemini 3.5 Flash 现在支持内置的计算机使用功能，使开发者能够构建可在浏览器、移动和桌面环境中观察、推理并执行操作的智能体。 该功能使 Gemini 3.5 Flash 成为 Anthropic 的 Claude 计算机使用 API 的竞争对手，可能扩展 LLM 在自主完成任务方面的应用。然而，社区对其可靠性和性能的怀疑可能减缓采用速度。 计算机使用功能内置于 Gemini 3.5 Flash 中，该模型已擅长函数调用和使用搜索、地图等内置工具。社区评论指出了任务失败、缺乏 MCP 支持以及基准测试图表可疑等问题。

hackernews · swolpers · Jun 24, 17:21 · [社区讨论](https://news.ycombinator.com/item?id=48662999)

**背景**: 计算机使用是指 LLM 通过截取屏幕截图并执行点击或键入等操作来与图形用户界面（GUI）交互的能力。这种方法比直接 API 调用更慢且更容易出错，但允许智能体无需集成即可与任何软件协作。Anthropic 的 Claude 3.5 Sonnet 是首批提供此类功能的模型之一。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-computer-use-gemini-3-5-flash/">Introducing computer use in Gemini 3 . 5 Flash</a></li>
<li><a href="https://deepmind.google/models/gemini/flash/">Gemini 3 . 5 Flash — Google DeepMind</a></li>
<li><a href="https://9to5google.com/2026/06/24/gemini-chrome-select-screen/">Gemini in Chrome adds ‘Select from screen’ tool</a></li>

</ul>
</details>

**社区讨论**: 社区评论大多持批评态度：用户报告了任务失败、缺乏 MCP 支持以及误导性的基准测试图表。一些人担心计算机使用本质上缓慢、不安全且容易出错，而另一些人则指出 Gemini 仍然缺乏与 Codex 或 Claude Code 相当的编码智能体。

**标签**: `#Gemini`, `#AI`, `#Google`, `#computer use`, `#LLM`

---

<a id="item-12"></a>
## [卡马克反思 id Software 早期错误](https://twitter.com/ID_AA_Carmack/status/2069799283369345247) ⭐️ 7.0/10

约翰·卡马克在 Twitter 上发文反思他在 id Software 早期犯下的错误，包括对团队施加过大压力，以及未能随着公司成熟调整管理风格。 卡马克的反思罕见地揭示了追求技术突破所带来的人员和文化代价，对创业文化和游戏开发领导力具有重要启示。 卡马克特别提到，持续以创业强度要求员工会让他们精疲力竭，而成熟的公司需要更多宽松空间。他还向受其高强度风格影响的同事 Sandy Petersen 道歉。

hackernews · shadowtree · Jun 24, 15:56 · [社区讨论](https://news.ycombinator.com/item?id=48661825)

**背景**: 约翰·卡马克是传奇游戏开发者、id Software 联合创始人，以创作《毁灭战士》和《雷神之锤》等标志性游戏而闻名。他的技术创新（如 3D 图形引擎）树立了行业标准。这条推文反思了追求突破性技术与维护健康公司文化之间的权衡。

**社区讨论**: 评论者普遍赞赏卡马克的坦诚，有人认为《雷神之锤》的成功或许证明了高强度管理的合理性，而另一些人则强调可持续工作文化的重要性。也有评论提及了 Sandy Petersen 的视角。

**标签**: `#startup-culture`, `#game-development`, `#leadership`, `#technical-debt`

---

<a id="item-13"></a>
## [Bunny.net 推出免费 DNS 服务，无查询限制](https://bunny.net/blog/were-making-bunny-dns-free/) ⭐️ 7.0/10

Bunny.net 取消了所有 DNS 查询费用，现在为每个账户提供最多 500 个域名的免费 DNS 托管，无查询限制、无按请求计费，也无隐藏的企业功能。 此举使 Bunny.net 成为 Cloudflare 的有力欧盟替代方案，通过消除中小型网站的成本障碍，可能颠覆 DNS 市场并促进竞争。 免费套餐包括智能记录和健康监控，这些功能在其他服务商通常仅限企业计划。Bunny.net 是一家私营公司，仅在 2022 年进行过一轮 600 万美元的小额融资，表明其更注重有机增长而非投资者驱动的扩张。

hackernews · dabinat · Jun 24, 08:50 · [社区讨论](https://news.ycombinator.com/item?id=48657030)

**背景**: DNS（域名系统）是互联网的电话簿，将域名转换为 IP 地址。许多 DNS 提供商按查询量收费，这对高流量网站来说成本可能很高。Cloudflare 提供流行的免费 DNS 套餐，但它是美国公司，引发了欧盟用户对数据主权和地缘政治风险的担忧。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://bunny.net/blog/were-making-bunny-dns-free/">We’re making Bunny DNS free</a></li>
<li><a href="https://alternativeto.net/news/2026/6/bunny-dns-is-now-free-with-unlimited-queries-500-free-domains-and-ipv6-and-dnssec-support/">Bunny DNS is now free with unlimited queries, 500 free... | AlternativeTo</a></li>

</ul>
</details>

**社区讨论**: 评论者普遍称赞此举，一些人强调 Bunny.net 是 Cloudflare 受欢迎的欧盟替代方案。然而，也有人担心流量激增（例如 LLM 爬虫）可能导致意外收费，以及非 CDN 产品缺乏账单上限。其他人则指出 Bunny.net 的小额融资和有机增长模式是可持续性的积极信号。

**标签**: `#DNS`, `#CDN`, `#Cloudflare`, `#Free Service`, `#Bunny.net`

---

<a id="item-14"></a>
## [Datasette 1.0a35 新增创建/修改表界面和 JSON API](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 引入了新的“创建表”和“修改表”界面，并配有 JSON API 支持，用户可以直接在 UI 中修改数据库模式。 此版本显著提升了 Datasette 的易用性，无需编写 SQL 或使用外部工具即可进行模式更改，使数据探索和发布更加便捷。 创建表 API 支持定义列、主键、自定义类型、NOT NULL 约束、默认值和单列外键。修改表 API 支持添加、重命名、重新排序和删除列，以及更改类型、默认值、约束、主键、外键和表名。

rss · Simon Willison · Jun 23, 21:34

**背景**: Datasette 是一个用于探索和发布 SQLite 数据库的开源工具，提供 Web 界面和 JSON API 来查询数据。此前，模式更改需要直接 SQL 访问或外部工具。此 alpha 版本将模式管理引入 UI，并由新的 JSON 端点支持。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://docs.datasette.io/en/stable/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://simonwillison.net/2026/jun/23/datasette/">Release: datasette 1.0a35 | Simon Willison’s Weblog</a></li>

</ul>
</details>

**标签**: `#datasette`, `#data tools`, `#open source`, `#release`

---

<a id="item-15"></a>
## [不精准洗牌需 14 次才能随机化一副牌](https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/) ⭐️ 7.0/10

新研究扩展了 1992 年的经典结论（7 次完美鸽尾式洗牌足以随机化一副 52 张牌），表明在更现实的非精准洗牌场景下——即切牌位置随机而非精确对半——大约需要 14 次鸽尾式洗牌才能达到充分随机化。 这一发现完善了我们对日常场景中随机化的理解，对纸牌游戏中的洗牌算法、密码学以及马尔可夫链混合理论都有启示意义。 研究人员为每张牌分配二进制“条形码”以追踪其在左右牌堆间的路径，并识别出残留有序的“冷点”区域，从而证明不精准洗牌也存在“截止现象”。不过，当前模型仍假设牌是一张张交错落下，而非成沓掉落。

telegram · zaihuapd · Jun 23, 16:04

**背景**: 鸽尾式洗牌是一种常见方法，将牌堆分成两叠然后交错合并。1992 年 Bayer 和 Diaconis 的结果表明，7 次完美鸽尾式洗牌（精确对半切牌）足以随机化一副牌。新研究放宽了完美切牌的假设，以模拟普通人洗牌的方式。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Shuffling">Shuffling - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Markov_chain_mixing_time">Markov chain mixing time - Wikipedia</a></li>

</ul>
</details>

**标签**: `#mathematics`, `#randomization`, `#card shuffling`, `#Markov chains`, `#probability`

---

<a id="item-16"></a>
## [LastPass 客服数据因 Klue 泄露被盗](https://techcrunch.com/2026/06/23/password-manager-maker-lastpass-says-hackers-stole-customer-support-case-data-during-klue-breach/) ⭐️ 7.0/10

LastPass 披露，其合作伙伴 Klue 在 2026 年 6 月 12 日遭黑客入侵，导致客户支持工单记录和个人信息被盗。黑客组织 Icarus 声称对此负责，并威胁若不支付赎金将公开数据。 此次泄露虽未影响密码库，但进一步削弱了用户对 LastPass 的信任——该公司在 2022 年曾发生严重的密码库泄露事件。这凸显了安全行业中第三方集成和供应链攻击的连锁风险。 被盗数据包括姓名、电话号码、邮箱地址、物理地址、客户支持案例详情和销售相关信息。LastPass 表示其自身基础设施和密码库仍然安全，泄露仅限于 Klue 平台。

telegram · zaihuapd · Jun 24, 00:49

**背景**: LastPass 是一款流行的密码管理器，截至 2024 年拥有超过 3300 万用户和约 160 万付费客户。2022 年，该公司曾遭遇严重泄露，攻击者窃取了加密的密码库。Klue 是 LastPass 的第三方供应商，提供客户支持工具；此次泄露利用了基于 OAuth 的集成漏洞，访问了多家公司的 Salesforce 数据。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.androidauthority.com/lastpass-data-breach-klue-3680836/">LastPass customer data exposed in new third-party vendor breach</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/klue-oauth-breach-victim-list-grows-as-icarus-hackers-claim-attack/">Klue OAuth breach victim list grows as Icarus hackers claim attack</a></li>
<li><a href="https://cybersecuritynews.com/klue-hack-cybersecurity-companies/">Klue Hack Leads to Data Breach Across Multiple Cybersecurity...</a></li>

</ul>
</details>

**标签**: `#security`, `#data breach`, `#LastPass`, `#password manager`, `#privacy`

---

<a id="item-17"></a>
## [特朗普不再视 Anthropic 为国安威胁](https://t.me/zaihuapd/42148) ⭐️ 7.0/10

前总统唐纳德·特朗普在接受 Axios 采访时表示，不再将人工智能公司 Anthropic 视为国家安全威胁，并暗示可能放松对其 Fable 5 和 Mythos 5 模型的限制，称 Anthropic“表现非常负责任”。 这一政策转变可能减轻对 Anthropic 的监管压力，并预示着更广泛的 AI 模型限制放松，从而可能加速美国 AI 的开发和部署。 尽管特朗普发表了上述言论，但美国商务部 6 月 12 日要求 Anthropic 限制外国人接触其最强模型的命令尚未正式撤销，五角大楼的供应链风险认定也仍然有效。

telegram · zaihuapd · Jun 24, 03:45

**背景**: Anthropic 是一家以开发 Claude 系列大语言模型而闻名的 AI 安全公司。其 Fable 5 和 Mythos 5 是先进的 AI 模型；Mythos 旨在发现软件漏洞，因安全顾虑尚未公开发布。美国政府此前曾基于国家安全担忧对 Anthropic 施加限制。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>
<li><a href="https://www.anthropic.com/claude/fable">Claude Fable \ Anthropic</a></li>
<li><a href="https://en.wikipedia.org/wiki/Mythos_(model)">Mythos (model)</a></li>

</ul>
</details>

**标签**: `#AI regulation`, `#Anthropic`, `#national security`, `#policy`

---

<a id="item-18"></a>
## [台积电先进制程全线涨价](https://36kr.com/newsflashes/3866472254411779) ⭐️ 7.0/10

台积电已通知客户，将对 3nm 至 7nm 所有先进制程涨价 5%至 10%，影响约 75%的晶圆营收。 此次涨价将影响依赖台积电先进制程的苹果、英伟达、AMD 等科技巨头，可能推高消费电子和 AI 芯片的成本。 涨价范围不仅包括 3nm，还涵盖 5nm 和 7nm 节点，整体涨幅在 5%至 10%之间。

telegram · zaihuapd · Jun 24, 05:45

**背景**: 台积电是全球领先的半导体代工厂，为苹果、英伟达等公司制造芯片。先进制程（3nm、5nm、7nm）采用尖端技术生产更小、更节能的晶体管。代工定价受合同协议、市场需求和生产成本影响。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://www.anandtech.com/show/16732/tsmc-manufacturing-update">TSMC Manufacturing Update: N6 to Match N7 Output by EOY...</a></li>
<li><a href="https://www.tomshardware.com/news/tsmc-5nm-4nm-3nm-process-node-introduces-3dfabric-technology">TSMC Dishes on 5 nm and 3 nm Process Nodes ... | Tom's Hardware</a></li>
<li><a href="https://www.smbom.com/news/38168">TSMC Plans 10% Increase in Wafer Foundry Prices - SmBom</a></li>

</ul>
</details>

**标签**: `#semiconductor`, `#TSMC`, `#chip manufacturing`, `#pricing`, `#supply chain`

---

<a id="item-19"></a>
## [字节跳动否认与博通合作开发 AI 芯片的报道](https://t.me/zaihuapd/42153) ⭐️ 7.0/10

路透社报道称，字节跳动正与博通合作开发一款由台积电制造的 5nm AI 处理器，但字节跳动已否认该报道。 如果属实，这一合作将使字节跳动在美国出口限制下减少对英伟达芯片的依赖，但否认声明给该公司的芯片战略蒙上不确定性。 据报道，该芯片是一款 5nm AI 处理器，但流片（制造前的最终设计阶段）尚未开始。字节跳动此前曾花费 20 亿美元购买英伟达芯片，并购买了华为的昇腾 910B 芯片。

telegram · zaihuapd · Jun 24, 07:01

**背景**: AI 芯片是专门用于加速机器学习工作负载的处理器。流片是芯片设计最终确定并送交制造的关键步骤，需要大量投资。美国的出口管制限制了中国公司获取先进半导体，促使许多公司开发定制芯片。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tape-out">Tape - out - Wikipedia</a></li>
<li><a href="https://macropolo.org/digital-projects/supply-chain/ai-chips/inside-an-ai-chip/">Inside an AI Chip - MacroPolo</a></li>

</ul>
</details>

**标签**: `#AI chips`, `#ByteDance`, `#Broadcom`, `#semiconductors`, `#US-China tech`

---

<a id="item-20"></a>
## [新版 Siri 拖累 Spotlight 搜索，用户不满](https://www.theregister.com/ai-and-ml/2026/06/16/the-new-siri-makes-one-of-apples-most-convenient-os-features-a-cumbersome-mess/5256591) ⭐️ 7.0/10

苹果在 iOS 27 和 macOS 27 测试版中让 AI 版 Siri 接管了 Spotlight 搜索，导致网页搜索需要额外步骤，并且对话记录被永久保存，用户体验变得繁琐。 这一变化降低了数百万用户使用的核心系统功能的可用性，优先考虑 AI 集成而非用户体验，可能为苹果在其生态系统中实施 AI 树立一个令人担忧的先例。 在测试版中，Spotlight 不再直接打开网页搜索结果，而是通过 Siri 路由查询，增加了额外点击。此外，Siri 的对话记录被永久保存，造成信息冗余。

telegram · zaihuapd · Jun 24, 14:31

**背景**: Spotlight 是苹果在 macOS、iOS、iPadOS 和 visionOS 上的系统级搜索功能，允许用户快速查找文件、应用和网页结果。苹果在 WWDC 上发布的新 AI Siri 支持连续对话，但被批评降低了 Spotlight 的效率，类似于对 Google AI Overviews 的抱怨。

<details><summary>参考链接</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Spotlight_(Apple)">Spotlight (Apple) - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews</a></li>

</ul>
</details>

**标签**: `#Apple`, `#Siri`, `#AI`, `#Spotlight`, `#User Experience`

---