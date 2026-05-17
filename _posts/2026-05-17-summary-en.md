---
layout: default
title: "Horizon Summary: 2026-05-17 (EN)"
date: 2026-05-17
lang: en
---

> From 38 items, 19 important content pieces were selected

---

1. [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](#item-1) ⭐️ 9.0/10
2. [vLLM v0.21.0: Breaking Changes, KV Offload, Spec Decode, Blackwell MLA](#item-2) ⭐️ 8.0/10
3. [NVIDIA's SANA-WM: Open-Source World Model for 1-Min 720p Video](#item-3) ⭐️ 8.0/10
4. [Julia Evans Moves Away from Tailwind CSS](#item-4) ⭐️ 8.0/10
5. [AI Breaks Open CTF Format, Undermines Learning](#item-5) ⭐️ 8.0/10
6. [DeepSeek-V4-Flash Revives LLM Steering](#item-6) ⭐️ 8.0/10
7. [Mitchell Hashimoto warns of 'AI psychosis' in companies](#item-7) ⭐️ 8.0/10
8. [Apple-OpenAI Partnership Frays, OpenAI Considers Legal Action](#item-8) ⭐️ 8.0/10
9. [Trump, Xi Discuss AI Guardrails and Nvidia H200 Chip Exports](#item-9) ⭐️ 8.0/10
10. [SpaceX, OpenAI, Anthropic Prep for Landmark IPOs by 2026](#item-10) ⭐️ 8.0/10
11. [Google bans AI search manipulation in spam policy](#item-11) ⭐️ 8.0/10
12. [Accelerando: A Prophetic Sci-Fi Novel from 2005](#item-12) ⭐️ 7.0/10
13. [δ-mem: Fixed-Size Online Memory for LLMs via Delta-Rule](#item-13) ⭐️ 7.0/10
14. [Reflection on Modern Societal Complexity](#item-14) ⭐️ 7.0/10
15. [US DOJ Demands Apple, Google Identify 100K+ Car App Users](#item-15) ⭐️ 7.0/10
16. [71% of Americans Oppose AI Data Centers Near Homes: Gallup](#item-16) ⭐️ 7.0/10
17. [OpenAI Partners with Malta to Offer Free ChatGPT Plus to All Citizens](#item-17) ⭐️ 7.0/10
18. [EU to Act Against TikTok and Meta Over Addictive Design](#item-18) ⭐️ 7.0/10
19. [GitHub Copilot Desktop App Enters Technical Preview](#item-19) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [SGLang v0.5.12 Adds Full DeepSeek V4 Inference Support](https://github.com/sgl-project/sglang/releases/tag/v0.5.12) ⭐️ 9.0/10

SGLang v0.5.12 introduces comprehensive inference support for DeepSeek V4, including tensor/expert/context parallelism, prefill-decode disaggregation, HiSparse KV cache offloading, and optimized DeepGemm and FlashMLA kernels for MegaMoE. This release enables efficient deployment of the 1-trillion-parameter DeepSeek V4 model, a major milestone in large-scale AI inference, and sets a new standard for serving cutting-edge MoE architectures with low latency and high throughput. Key additions include W4A4 MegaMoE kernels with negligible accuracy loss, Marlin/FlashInfer W4A8 MoE kernels on Hopper, TP16 support on H100/H20, and a unified Docker image for all Nvidia GPUs. The release also adds support for models like Intern-S2-Preview, MiniCPM-V 4.6, and Ring-2.6-1T.

github · Fridge003 · May 16, 18:23

**Background**: SGLang is a high-performance serving framework for large language models and multimodal models, designed for low-latency and high-throughput inference across single GPU to large clusters. DeepSeek V4 is a 1-trillion-parameter Mixture-of-Experts (MoE) model that requires advanced parallelism and kernel optimizations for efficient serving.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/sgl-project/sglang">GitHub - sgl-project/sglang: SGLang is a high-performance serving framework for large language models and multimodal models. · GitHub</a></li>
<li><a href="https://sgl-project.github.io/">SGLang Documentation — SGLang</a></li>
<li><a href="https://deepseek.ai/deepseek-v4">DeepSeek V 4 : 1T Parameter AI Model Guide | Independent DeepSeek ...</a></li>

</ul>
</details>

**Tags**: `#DeepSeek V4`, `#SGLang`, `#inference`, `#parallelism`, `#kernels`

---

<a id="item-2"></a>
## [vLLM v0.21.0: Breaking Changes, KV Offload, Spec Decode, Blackwell MLA](https://github.com/vllm-project/vllm/releases/tag/v0.21.0) ⭐️ 8.0/10

vLLM v0.21.0 deprecates transformers v4, requires C++20, integrates KV offload with Hybrid Memory Allocator (HMA), adds speculative decoding support for reasoning models with thinking budget, and introduces a new TOKENSPEED_MLA attention backend for Blackwell GPUs. This release significantly impacts the LLM inference ecosystem by enabling more efficient memory management and faster inference for reasoning models, while the Blackwell MLA backend unlocks high-performance inference for cutting-edge models like DeepSeek-R1 and Kimi-K25 on NVIDIA's latest hardware. The KV offload with HMA includes scheduler-side sliding window groups and full HMA enablement, while speculative decoding now respects reasoning/thinking budgets for correct spec decode. The TOKENSPEED_MLA backend is specifically optimized for agentic workloads with long contexts and multi-turn interactions on Blackwell GPUs.

github · khluu · May 15, 08:44

**Background**: vLLM is a high-throughput, memory-efficient LLM inference engine widely used in production. KV cache offloading moves key-value cache from GPU to CPU memory to reduce GPU memory pressure, and HMA improves memory allocation efficiency. Speculative decoding accelerates inference by using a smaller draft model to predict outputs of a larger target model. The MLA (Multi-head Latent Attention) backend is a specialized attention implementation for models like DeepSeek-R1.

<details><summary>References</summary>
<ul>
<li><a href="https://github.com/vllm-project/vllm/releases">Releases · vllm -project/ vllm · GitHub</a></li>
<li><a href="https://fenado.ai/articles/lightseek-foundation-unveils-open-source-tokenspeed-llm-engine-with-vllm-integration-for-nvidia-blackwell">LightSeek Foundation Unveils Open-Source TokenSpeed LLM Engine with vLLM Integration for NVIDIA Blackwell | TokenSpeed, LLM inference engine, Fenado AI</a></li>
<li><a href="https://research.google/blog/looking-back-at-speculative-decoding/">Looking back at speculative decoding</a></li>

</ul>
</details>

**Tags**: `#vLLM`, `#LLM inference`, `#GPU optimization`, `#speculative decoding`, `#transformers`

---

<a id="item-3"></a>
## [NVIDIA's SANA-WM: Open-Source World Model for 1-Min 720p Video](https://nvlabs.github.io/Sana/WM/) ⭐️ 8.0/10

NVIDIA released SANA-WM, a 2.6-billion-parameter open-source world model that generates 60-second, 720p videos from a single image and a 6-DoF camera trajectory, running on a single GPU. This marks a significant step toward real-time, controllable video generation for applications like robotics simulation and game development, but the community is skeptical about its 'open-source' claim as model weights are not yet released. SANA-WM uses a hybrid diffusion Transformer architecture and achieves 36× higher throughput than prior open-source baselines on a one-minute world model benchmark, though the model is currently only available for research use with a commercial-friendly license.

hackernews · mjgil · May 16, 12:06 · [Discussion](https://news.ycombinator.com/item?id=48159445)

**Background**: World models are AI systems that learn an internal representation of an environment to predict future states, enabling applications like autonomous driving and video game simulation. 6-DoF (six degrees of freedom) camera control allows adjusting position (x, y, z) and orientation (roll, pitch, yaw) independently.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/html/2605.15178v1">SANA-WM: Efficient Minute-Scale World Modeling with Hybrid ...</a></li>
<li><a href="https://www.marktechpost.com/2026/05/16/nvidia-introduces-sana-wm-a-2-6b-parameter-open-source-world-model-that-generates-minute-scale-720p-video-on-a-single-gpu/">NVIDIA Introduces SANA-WM: A 2.6B-Parameter Open-Source World ...</a></li>
<li><a href="https://thecodersblog.com/sana-wm-world-modeling-at-the-edge-of-real-time-with-hybrid-diffusion/">SANA-WM: World Modeling at the Edge of Real-Time with Hybrid ...</a></li>

</ul>
</details>

**Discussion**: Community comments express skepticism about the 'open-source' label since weights are not yet released, with some calling it 'vaporware'. Others note the generated videos resemble video game graphics, likely due to synthetic training data from Unreal Engine, while some are excited about the potential impact on game development.

**Tags**: `#world model`, `#video generation`, `#open-source`, `#NVIDIA`, `#AI`

---

<a id="item-4"></a>
## [Julia Evans Moves Away from Tailwind CSS](https://jvns.ca/blog/2026/05/15/moving-away-from-tailwind--and-learning-to-structure-my-css-/) ⭐️ 8.0/10

Julia Evans published a blog post detailing her decision to move away from Tailwind CSS and instead focus on writing semantic HTML and structured CSS. This shift highlights a growing debate in the web development community about the trade-offs between utility-first frameworks like Tailwind and traditional semantic markup, with implications for accessibility and long-term maintainability. Evans emphasizes starting with meaningful HTML structure before applying CSS, and notes that Tailwind's utility classes can obscure the document's semantic meaning.

hackernews · mpweiher · May 16, 09:14 · [Discussion](https://news.ycombinator.com/item?id=48158400)

**Background**: Tailwind CSS is a utility-first CSS framework that provides low-level utility classes for rapid styling directly in HTML. Semantic HTML uses HTML elements to convey the meaning and structure of content, which is important for accessibility and SEO.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Tailwind_CSS">Tailwind CSS</a></li>
<li><a href="https://en.wikipedia.org/wiki/Semantic_HTML">Semantic HTML</a></li>
<li><a href="https://tailwindcss.com/">Tailwind CSS - Rapidly build modern websites without ever leaving your HTML.</a></li>

</ul>
</details>

**Discussion**: The community discussion (264 comments) shows strong support for Evans' perspective, with many commenters agreeing that Tailwind can lead to less semantic markup and that CSS Modules offer a simpler alternative. Some commenters also criticized Tailwind advocates for lacking deep CSS knowledge.

**Tags**: `#CSS`, `#Tailwind CSS`, `#semantic HTML`, `#web development`, `#accessibility`

---

<a id="item-5"></a>
## [AI Breaks Open CTF Format, Undermines Learning](https://kabir.au/blog/the-ctf-scene-is-dead) ⭐️ 8.0/10

A blog post argues that frontier AI has broken the traditional open CTF (Capture The Flag) format by enabling quick flag retrieval, thus undermining the collaborative learning experience. The author claims that AI tools can now solve many challenges instantly, reducing the need for human problem-solving. This matters because CTF competitions are a key training ground for cybersecurity skills; if AI trivializes them, it could impact how newcomers learn and how the community evaluates talent. The discussion reflects broader concerns about AI's role in education and skill development. The post notes that AI can now automatically retrieve flags from many challenges, changing the dynamic from hours of collaborative effort to minutes of automated work. Some commenters argue that automating CTF challenges is not cheating but part of the culture, though the author believes it breaks the open format's purpose.

hackernews · frays · May 16, 07:01 · [Discussion](https://news.ycombinator.com/item?id=48157559)

**Background**: Capture The Flag (CTF) is a cybersecurity competition where participants find hidden text strings called 'flags' in vulnerable programs or websites. The open CTF format typically involves publicly available challenges that teams solve collaboratively, often with a focus on learning. AI advancements, especially large language models, have made it possible to solve certain challenge types automatically.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Capture_the_flag_(cybersecurity)">Capture the flag (cybersecurity) - Wikipedia</a></li>
<li><a href="https://news.ycombinator.com/item?id=48157559">Frontier AI has broken the open CTF format | Hacker News</a></li>

</ul>
</details>

**Discussion**: Comments are mixed: some agree that AI ruins the learning experience, while others argue that automation has always been part of CTF culture. A notable point is that the real issue may be the loss of collaborative problem-solving, not just flag retrieval. Some suggest that CTF formats will evolve to remain relevant.

**Tags**: `#AI`, `#CTF`, `#cybersecurity`, `#education`, `#community`

---

<a id="item-6"></a>
## [DeepSeek-V4-Flash Revives LLM Steering](https://www.seangoedecke.com/steering-vectors/) ⭐️ 8.0/10

DeepSeek-V4-Flash, combined with the DwarfStar 4 project, has made LLM steering practical again by enabling effective refusal removal and novel interaction modalities through activation manipulation. This development opens up new possibilities for controlling LLM behavior without retraining, impacting AI safety, uncensoring, and user interaction design. The steering vector technique can remove refusals by targeting a single direction in the residual stream, and DwarfStar 4 is a standalone project (not a stripped-down llama.cpp) that implements this for DeepSeek-V4-Flash.

hackernews · Brajeshwar · May 16, 14:58 · [Discussion](https://news.ycombinator.com/item?id=48160807)

**Background**: LLM steering involves adding a steering vector to the model's activations during inference to guide outputs. Previous work like Golden Gate Claude showed promise, but DeepSeek-V4-Flash's architecture makes steering more effective. Refusal in LLMs is often mediated by a single direction, making it removable via steering.

<details><summary>References</summary>
<ul>
<li><a href="https://www.seangoedecke.com/steering-vectors/">DeepSeek-V4-Flash means LLM steering is interesting again</a></li>
<li><a href="https://www.lesswrong.com/posts/QQP4nq7TXg89CJGBh/a-sober-look-at-steering-vectors-for-llms">A Sober Look at Steering Vectors for LLMs — LessWrong</a></li>
<li><a href="https://www.alignmentforum.org/posts/jGuXSZgv6qfdhMCuJ/refusal-in-llms-is-mediated-by-a-single-direction">Refusal in LLMs is mediated by a single... — AI Alignment Forum</a></li>

</ul>
</details>

**Discussion**: Commenters highlighted the potential for refusal removal (abliteration) and novel interaction modalities, with antirez clarifying that DwarfStar 4 is its own project. Some noted that steering vectors could be used to make models more radical or to explore hidden knobs from frontier labs.

**Tags**: `#LLM`, `#steering vectors`, `#DeepSeek`, `#AI safety`, `#uncensoring`

---

<a id="item-7"></a>
## [Mitchell Hashimoto warns of 'AI psychosis' in companies](https://twitter.com/mitchellh/status/2055380239711457578) ⭐️ 8.0/10

Mitchell Hashimoto, creator of HashiCorp tools like Terraform and Vagrant, posted a warning that many companies are suffering from 'AI psychosis'—an over-reliance on AI tools that undermines core engineering practices. This critique highlights a growing tension in the software industry between leveraging AI for productivity and maintaining rigorous engineering fundamentals, potentially affecting code quality, system reliability, and long-term maintainability. The post gained significant traction with 1858 points and 1050 comments on Hacker News, indicating widespread resonance. Hashimoto's warning comes from his experience building complex infrastructure tools, lending weight to his perspective.

hackernews · reasonableklout · May 15, 20:26 · [Discussion](https://news.ycombinator.com/item?id=48153379)

**Background**: AI coding assistants like GitHub Copilot and Claude have become popular, promising to boost developer productivity. However, critics argue that overuse can lead to shallow understanding of code, increased technical debt, and fragility in systems built without deep engineering insight.

**Discussion**: Commenters shared mixed experiences: some reported management pushing AI usage for bragging rights rather than genuine need, while others expressed concern that AI-generated code introduces hidden risks. A few noted that this trend might force software engineering to become more disciplined, akin to traditional engineering fields.

**Tags**: `#AI`, `#software engineering`, `#productivity`, `#critique`, `#industry trends`

---

<a id="item-8"></a>
## [Apple-OpenAI Partnership Frays, OpenAI Considers Legal Action](https://www.bloomberg.com/news/articles/2026-05-14/openai-apple-partnership-frays-setting-up-possible-legal-fight) ⭐️ 8.0/10

Apple and OpenAI's partnership is deteriorating due to unmet revenue expectations, with OpenAI hiring external lawyers to explore legal options for potential breach of contract. Apple plans to open Siri to other AI models like Claude and Gemini at WWDC in June. This rift could reshape the AI integration landscape in consumer devices, affecting how users access AI assistants on iPhones. It also highlights the challenges of monetizing AI partnerships at scale. ChatGPT integration in Apple's system is deeply hidden in settings, requiring specific keywords to activate, leading to poor user adoption. Apple is also dissatisfied with OpenAI's privacy standards, hardware business, and engineer poaching.

telegram · zaihuapd · May 15, 12:59

**Background**: Apple and OpenAI announced a partnership in 2024 to integrate ChatGPT into Siri and other Apple services. The deal was expected to generate billions in subscription revenue for both companies, but actual conversions have fallen far short.

<details><summary>References</summary>
<ul>
<li><a href="https://news.sina.cn/bignews/insight/2026-05-15/detail-inhxypti3365337.d.html?vt=4">苹果用户抱怨ChatGPT难调用，OpenAI怒告苹果能改变使用体验吗？</a></li>
<li><a href="https://www.moomoo.com/news/post/70040468/overnight-us-stocks-kansas-city-fed-president-warns-of-inflation">Overnight U.S. Stocks | Kansas City Fed President Warns of Inflation Risks</a></li>

</ul>
</details>

**Tags**: `#Apple`, `#OpenAI`, `#AI`, `#partnership`, `#legal`

---

<a id="item-9"></a>
## [Trump, Xi Discuss AI Guardrails and Nvidia H200 Chip Exports](https://www.bloomberg.com/news/articles/2026-05-15/trump-says-he-discussed-ai-guardrails-nvidia-s-chips-with-xi) ⭐️ 8.0/10

President Trump revealed that he discussed AI guardrails and Nvidia H200 chip exports with Chinese President Xi Jinping during his visit to China, noting that China has chosen not to buy the H200 despite US approval. This development highlights the ongoing geopolitical tensions in AI chip supply chains, with implications for global semiconductor markets and AI safety cooperation between the US and China. The US has allowed Nvidia to supply H200 chips to Chinese customers, but Beijing has not yet approved purchases; Commerce Secretary Lutnick noted that no H200 deliveries have occurred due to the Chinese government not releasing enterprises to buy. Previously, China also rejected the lower-performance H20 chip.

telegram · zaihuapd · May 15, 15:13

**Background**: AI guardrails are safeguards that keep AI systems operating safely and responsibly within defined boundaries. The Nvidia H200 GPU, based on the Hopper architecture, offers 141 GB of HBM3e memory and is designed for generative AI and HPC workloads. The discussion also touched on concerns raised by Anthropic's Mythos model, which has triggered global alarms due to its potential risks.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ibm.com/think/topics/ai-guardrails">What Are AI Guardrails? | IBM</a></li>
<li><a href="https://www.nvidia.com/en-us/data-center/h200/">NVIDIA H200 GPU</a></li>
<li><a href="https://www.nytimes.com/2026/04/22/technology/anthropics-mythos-ai.html">Anthropic’s New Mythos A.I. Model Sets Off Global Alarms ...</a></li>

</ul>
</details>

**Tags**: `#AI chips`, `#US-China relations`, `#export controls`, `#Nvidia`, `#AI safety`

---

<a id="item-10"></a>
## [SpaceX, OpenAI, Anthropic Prep for Landmark IPOs by 2026](https://t.me/zaihuapd/41409) ⭐️ 8.0/10

SpaceX, OpenAI, and Anthropic are preparing for initial public offerings as early as 2026, aiming to raise hundreds of billions of dollars collectively. SpaceX is expected to go public within 12 months barring market volatility, while Anthropic has engaged legal advisors to begin preparations. These IPOs could be among the largest in history, potentially surpassing the total proceeds of all U.S. IPOs in 2025. The listings would provide public market access to three of the most valuable private tech companies, reshaping investment landscapes in space, AI, and frontier technology. OpenAI is reportedly targeting a valuation of up to $1 trillion, while SpaceX's confidential S-1 filing in April 2026 valued the company at $1.75 trillion. The combined fundraising could exceed $200 billion, dwarfing typical IPO sizes.

telegram · zaihuapd · May 16, 03:10

**Background**: SpaceX, founded by Elon Musk, is a private aerospace manufacturer and space transportation company known for its Falcon rockets and Starlink satellite internet. OpenAI, creator of ChatGPT, is an AI research organization transitioning from a non-profit to a for-profit model. Anthropic, founded by former OpenAI employees, develops the Claude family of large language models with a focus on AI safety. IPOs allow private companies to sell shares to the public on stock exchanges, providing liquidity for early investors and raising capital for growth.

<details><summary>References</summary>
<ul>
<li><a href="https://www.cointribune.com/en/openai-eyes-1-trillion-valuation-with-2026-ipo-plans-amid-rising-ai-competition/">OpenAI Eyes $1 Trillion Valuation with 2026 IPO Plans ... - Cointribune</a></li>
<li><a href="https://www.fool.com/investing/2026/04/27/spacex-ipo-timeline-every-important-date-need-know/">The SpaceX IPO Timeline: Every Important Date and Time Frame ...</a></li>
<li><a href="https://en.wikipedia.org/wiki/Anthropic">Anthropic - Wikipedia</a></li>

</ul>
</details>

**Tags**: `#IPO`, `#SpaceX`, `#OpenAI`, `#Anthropic`, `#venture capital`

---

<a id="item-11"></a>
## [Google bans AI search manipulation in spam policy](https://www.theverge.com/tech/931416/google-ai-search-spam-policy) ⭐️ 8.0/10

Google has updated its search spam policy to explicitly prohibit manipulating AI-generated search responses, including AI Overviews and AI Mode. This targets GEO (Generative Engine Optimization) tactics that attempt to game AI search results. This policy update signals a major shift in search quality enforcement, directly impacting SEO and AI communities. It aims to preserve the integrity of AI-powered search results and prevent spammy tactics from undermining user trust. Violating sites may be demoted or removed from search results entirely. Common GEO tactics include mass-generating biased 'best of' content or embedding prompt-like text to manipulate AI models into citing a site as authoritative.

telegram · zaihuapd · May 16, 06:31

**Background**: AI Overviews and AI Mode are Google features that generate AI-powered summaries and responses in search results. GEO (Generative Engine Optimization) is an emerging practice where websites optimize content specifically to appear in AI-generated answers, similar to traditional SEO for search rankings.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/AI_Overviews">AI Overviews - Wikipedia</a></li>
<li><a href="https://blog.berocket.com/8-geo-tactics-in-2025/">8 GEO Tactics to Boost Your AI Search Visibility in... - BeRocket Blog</a></li>

</ul>
</details>

**Tags**: `#Google`, `#AI search`, `#spam policy`, `#SEO`, `#GEO`

---

<a id="item-12"></a>
## [Accelerando: A Prophetic Sci-Fi Novel from 2005](https://www.antipope.org/charlie/blog-static/fiction/accelerando/accelerando.html) ⭐️ 7.0/10

Charlie Stross's 2005 novel Accelerando is being re-evaluated as a prophetic work that accurately foresaw many aspects of today's AI-driven world, including AI agents and technological dependency. The novel's themes of AI agents, neural networks, and the technological singularity resonate strongly with current developments in AI, making it a valuable lens for understanding the societal and ethical implications of rapid technological change. The story follows a family over several generations as humanity transitions to a posthuman future, with characters relying heavily on AI agents for daily tasks. The novel was originally published as a series of short stories in Asimov's Science Fiction magazine between 2001 and 2004.

hackernews · eamag · May 16, 11:36 · [Discussion](https://news.ycombinator.com/item?id=48159241)

**Background**: The technological singularity is a hypothetical future point where artificial intelligence surpasses human intelligence, leading to unpredictable changes. AI agents are autonomous systems that can perform tasks and make decisions with varying degrees of independence. Accelerando explores these concepts through a narrative that blends hard science fiction with social commentary.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Technological_singularity">Technological singularity</a></li>
<li><a href="https://en.wikipedia.org/wiki/AI_agent">AI agent</a></li>
<li><a href="https://en.wikipedia.org/wiki/Posthuman_future">Posthuman future</a></li>

</ul>
</details>

**Discussion**: Commenters note that the novel's predictions about AI agents and technological dependency are eerily accurate, with one user comparing the protagonist's glasses to modern AI assistants. Another reader reinterprets the story as a tragedy about the loss of humanity in the pursuit of progress, while others praise its plausible depiction of a weird future.

**Tags**: `#science fiction`, `#AI`, `#singularity`, `#technology`, `#literature`

---

<a id="item-13"></a>
## [δ-mem: Fixed-Size Online Memory for LLMs via Delta-Rule](https://arxiv.org/abs/2605.12357) ⭐️ 7.0/10

δ-mem introduces a fixed-size state matrix that is updated using delta-rule learning to compress past information, enabling efficient online memory for large language models without expanding the context window. This approach addresses the fundamental limitation of fixed context windows in LLMs, potentially reducing memory and computational costs for long-context tasks like multi-turn conversations and agent interactions. The fixed-size memory matrix is updated via delta-rule learning, which adjusts weights based on prediction errors. The paper does not specify the exact memory requirements or computational overhead, leaving practical feasibility open for further evaluation.

hackernews · 44za12 · May 16, 09:30 · [Discussion](https://news.ycombinator.com/item?id=48158506)

**Background**: Large language models (LLMs) typically have a fixed context window, limiting their ability to process long sequences. Online memory mechanisms aim to compress and store past information for later retrieval, but existing methods often suffer from growing memory size or high computational cost. Delta-rule learning is a classic neural network update rule that minimizes error by adjusting weights proportionally to the difference between desired and actual output.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Delta_rule">Delta rule - Wikipedia</a></li>
<li><a href="https://medium.com/@neuralnets/delta-learning-rule-gradient-descent-neural-networks-f880c168a804">Delta Learning Rule & Gradient Descent | Neural Networks - Medium</a></li>
<li><a href="https://www.memobase.io/">AI Memory for LLMs | Build Personalized Agents with Memobase</a></li>

</ul>
</details>

**Discussion**: Commenters expressed mixed opinions: some praised the fixed-size memory idea but questioned its capacity limits and practical cost, while others noted the approach resembles DeltaNet hypernetworks and may not be groundbreaking. There was also interest in whether this could enable agents to remember guidelines without re-feeding context each session.

**Tags**: `#LLM`, `#memory`, `#efficiency`, `#deep learning`, `#context window`

---

<a id="item-14"></a>
## [Reflection on Modern Societal Complexity](https://user8.bearblog.dev/the-world-is-too-complicated/) ⭐️ 7.0/10

A reflective essay argues that modern society has become overly complex, sparking a community discussion on the nature of complexity and human adaptation. This piece resonates with many people who feel overwhelmed by modern life, prompting a valuable conversation about whether complexity is inherent or a human creation. The essay scores 7.0/10 with 164 points and 166 comments, indicating strong engagement. Community comments explore themes such as the meaning of life, civilization's adaptation, and the trade-offs of remote work.

hackernews · James72689 · May 16, 08:25 · [Discussion](https://news.ycombinator.com/item?id=48158065)

**Background**: The essay is a philosophical reflection on societal complexity, touching on how humans have adapted their environment rather than themselves. It contrasts immediate, local work with long-term, abstract ends, a common theme in discussions about modern life.

**Discussion**: Commenters offer diverse perspectives: some argue complexity is inherent to existence, while others see it as a human expression under specific conditions. One commenter notes the appeal of immediate, tangible work over abstract, long-term goals.

**Tags**: `#society`, `#complexity`, `#philosophy`, `#technology`, `#humanity`

---

<a id="item-15"></a>
## [US DOJ Demands Apple, Google Identify 100K+ Car App Users](https://9to5mac.com/2026/05/15/doj-reportedly-demands-apple-and-google-identify-over-100000-users-of-car-app/) ⭐️ 7.0/10

The US Department of Justice has subpoenaed Apple, Google, and Amazon to identify over 100,000 users of the EZ Lynk car tuning app, including their identities, addresses, and purchase records, as part of a Clean Air Act investigation. This mass data request raises significant privacy concerns and could set a legal precedent for how tech companies handle government demands for user information. It also impacts the automotive tuning community and companies involved in vehicle emissions modifications. The subpoenas were issued in March and April 2026, and EZ Lynk denies that its products are primarily used to bypass emissions controls. Apple and Google are reportedly preparing to challenge the request as overly broad and invasive of user privacy.

telegram · zaihuapd · May 16, 05:34

**Background**: EZ Lynk is a platform that allows users to reprogram vehicle engine control units (ECUs) to modify performance, which can potentially disable emissions controls. The Clean Air Act prohibits tampering with emissions systems, and the DOJ has been investigating EZ Lynk since 2021 for allegedly selling devices that violate this law.

<details><summary>References</summary>
<ul>
<li><a href="https://www.ezlynk.com/">EZ LYNK®: The Future of Vehicle Diagnostics & Control</a></li>

</ul>
</details>

**Tags**: `#privacy`, `#legal`, `#automotive`, `#data request`, `#DOJ`

---

<a id="item-16"></a>
## [71% of Americans Oppose AI Data Centers Near Homes: Gallup](https://news.gallup.com/poll/709772/americans-oppose-data-centers-area.aspx) ⭐️ 7.0/10

A March Gallup poll found that 71% of Americans oppose building AI data centers near their homes, with 48% strongly opposed; only 7% strongly support. This is the first time Gallup has asked about local AI data center construction. The survey reveals strong public resistance to AI data centers, driven by concerns over energy, water, pollution, and noise, which could complicate industry expansion and policy decisions. This opposition is even higher than that for nuclear power plants, signaling a major challenge for AI infrastructure development. Among opponents, about half cited high electricity and water consumption, while others worried about pollution, noise, traffic, and rising living costs. Supporters most frequently mentioned job creation and tax revenue.

telegram · zaihuapd · May 16, 07:59

**Background**: AI data centers require enormous amounts of electricity and water to power and cool servers, leading to environmental and resource concerns. As AI adoption grows, data center construction has surged, sparking community pushback in many regions. Gallup's survey is the first to quantify U.S. public opinion on this issue at the local level.

<details><summary>References</summary>
<ul>
<li><a href="https://www.remio.ai/post/ai-data-centers-the-hidden-energy-and-water-crisis-behind-the-ai-boom">AI Data Centers : The Hidden Energy and Water Crisis Behind the AI ...</a></li>
<li><a href="https://news.ucsb.edu/2025/021835/power-ai-data-centers-need-more-and-more-energy">To power AI , data centers need more and more energy | The Current</a></li>

</ul>
</details>

**Tags**: `#AI`, `#data centers`, `#public opinion`, `#environment`, `#Gallup`

---

<a id="item-17"></a>
## [OpenAI Partners with Malta to Offer Free ChatGPT Plus to All Citizens](https://openai.com/index/malta-chatgpt-plus-partnership/) ⭐️ 7.0/10

OpenAI and the Government of Malta announced a first-of-its-kind national partnership to provide one year of free ChatGPT Plus access to all Maltese citizens who complete an AI literacy course developed by the University of Malta. This initiative marks the first national-level government partnership with OpenAI to democratize AI access, potentially setting a precedent for other countries and accelerating AI literacy and adoption at a population scale. The program, called 'AI for All,' will launch in May 2026, managed by the Malta Digital Innovation Authority, and will eventually extend to Maltese citizens living abroad.

telegram · zaihuapd · May 16, 10:40

**Background**: ChatGPT Plus is a premium subscription tier that offers faster response times, priority access to new features, and access to advanced models like GPT-4. The AI literacy course, 'AI for Everyone,' is designed to equip citizens with a comprehensive understanding of AI capabilities and responsibilities.

<details><summary>References</summary>
<ul>
<li><a href="https://openai.com/index/malta-chatgpt-plus-partnership/">OpenAI and Malta partner to bring ChatGPT Plus to all citizens | OpenAI</a></li>
<li><a href="https://www.independent.com.mt/articles/2026-05-16/local-news/Online-course-AI-for-Everyone-launched-6736289783">Online course ‘ AI for Everyone’ launched - The Malta Independent</a></li>
<li><a href="https://www.cryptobreaking.com/malta-openai-free-chatgpt-plus/">Malta OpenAI Free ChatGPT Plus for All Citizens Could Boost Crypto</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#ChatGPT`, `#AI policy`, `#government partnership`, `#AI literacy`

---

<a id="item-18"></a>
## [EU to Act Against TikTok and Meta Over Addictive Design](https://unwire.hk/2026/05/16/eu-tiktok-meta-addictive-design-child-protection/life-tech/social-network/) ⭐️ 7.0/10

European Commission President Ursula von der Leyen announced at a summit in Denmark that the EU will take action against TikTok and Meta (Instagram, Facebook) over addictive design features and failure to enforce age restrictions, with legal proposals expected by summer 2026. This marks a major regulatory escalation under the Digital Services Act, potentially forcing platforms to redesign core features globally and setting a precedent for child protection online. The EU has already preliminarily ruled that TikTok's addictive design and Meta's age verification mechanisms violate the DSA, and has launched an open-source anonymous age verification app. Australia has already banned social media for under-16s, with many countries following suit.

telegram · zaihuapd · May 16, 14:33

**Background**: The Digital Services Act (DSA) is a comprehensive EU regulation that holds large platforms accountable for systemic risks, including addictive design and inadequate child protection. Addictive design techniques like infinite scroll and autoplay are designed to maximize user engagement, often at the expense of mental health, especially among minors.

<details><summary>References</summary>
<ul>
<li><a href="https://indianexpress.com/article/technology/eu-tiktok-doom-scrolling-ban-addictive-design-dsa-10538701/">End of the ‘Endless Scroll’? Why the EU is Forcing TikTok to Redesign...</a></li>
<li><a href="https://www.europeaninterest.eu/eu-accuses-tiktok-of-addictive-design-that-harms-children-in-breach-of-the-digital-services-act/">EU accuses TikTok of ' addictive design ' that harms children in breach....</a></li>
<li><a href="https://www.medianama.com/2026/05/223-eu-social-media-giants-new-law-addictive-design/">EU targets social media giants with new ' addictive design ' law</a></li>

</ul>
</details>

**Tags**: `#EU regulation`, `#addictive design`, `#child protection`, `#TikTok`, `#Meta`

---

<a id="item-19"></a>
## [GitHub Copilot Desktop App Enters Technical Preview](https://github.blog/changelog/2026-05-14-github-copilot-app-is-now-available-in-technical-preview/) ⭐️ 7.0/10

GitHub Copilot desktop app is now available in technical preview, allowing users to launch isolated development sessions from issues, pull requests, prompts, or history, view diffs, run tests, and create pull requests within the app, along with Agent Merge for automated review handling and merging. This marks a significant step toward a native, agentic desktop experience for GitHub Copilot, enabling developers to perform complex workflows without leaving the app, which could boost productivity and streamline AI-assisted development. Copilot Pro and Pro+ subscribers can immediately request early access, while Business and Enterprise users will get access within the week, provided their organization admin enables the preview and CLI permissions in policies.

telegram · zaihuapd · May 16, 15:07

**Background**: GitHub Copilot is an AI-powered code completion and assistant tool developed by GitHub and OpenAI, integrated into popular IDEs. The new desktop app extends Copilot's capabilities beyond IDE plugins, offering a standalone client with agentic features like isolated sessions and automated PR merging.

<details><summary>References</summary>
<ul>
<li><a href="https://pasqualepillitteri.it/en/news/2544/github-copilot-app-technical-preview-2026">GitHub Copilot App: Microsoft's Agentic Desktop Client Opens Waitlist...</a></li>
<li><a href="https://github.com/features/copilot">GitHub Copilot · Your AI pair programmer · GitHub</a></li>

</ul>
</details>

**Tags**: `#GitHub Copilot`, `#AI-assisted development`, `#developer tools`, `#technical preview`

---