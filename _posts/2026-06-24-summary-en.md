---
layout: default
title: "Horizon Summary: 2026-06-24 (EN)"
date: 2026-06-24
lang: en
---

> From 32 items, 21 important content pieces were selected

---

1. [Critical FFmpeg Flaw Allows RCE via Malicious Videos](#item-1) ⭐️ 9.0/10
2. [China's LineShine Supercomputer Tops TOP500 After 8 Years](#item-2) ⭐️ 9.0/10
3. [WYSIWYG TikZ Editor with Live Source Sync](#item-3) ⭐️ 8.0/10
4. [The Coming Loop: AI Agents Reshape Software Development](#item-4) ⭐️ 8.0/10
5. [Unlimited OCR: Constant Memory for Long Document Parsing](#item-5) ⭐️ 8.0/10
6. [Google Fires Employee Over Unofficial Workspace CLI](#item-6) ⭐️ 8.0/10
7. [Prompt Injection as Role Confusion: LLMs Prioritize Style Over Content](#item-7) ⭐️ 8.0/10
8. [Moebius 0.2B Inpainting Model Ported to Browser via WebGPU](#item-8) ⭐️ 8.0/10
9. [OpenAI to produce AI-animated film 'Critterz' for under $30M](#item-9) ⭐️ 8.0/10
10. [Valve Announces Steam Machine Console Starting at $1049](#item-10) ⭐️ 8.0/10
11. [US Humanoid Robots Rely on Chinese Components: WSJ](#item-11) ⭐️ 8.0/10
12. [SpaceX Falcon Heavy to Launch ESA Mars Rover in 2028](#item-12) ⭐️ 8.0/10
13. [FUTO Swipe: New Swipe Typing Model Released](#item-13) ⭐️ 7.0/10
14. [Swift Package Index Acquired by Apple](#item-14) ⭐️ 7.0/10
15. [Vitamin D Benefits Real but Limited to Deficient](#item-15) ⭐️ 7.0/10
16. [California AB 2047 Targets 3D Printers with Gun Detection Mandate](#item-16) ⭐️ 7.0/10
17. [Datasette 1.0a35 Adds Create/Alter Table Interfaces](#item-17) ⭐️ 7.0/10
18. [Chinese Universities Cut Foreign Language Programs](#item-18) ⭐️ 7.0/10
19. [Samsung Unveils UFS 5.0 with 10.8 GB/s for On-Device AI](#item-19) ⭐️ 7.0/10
20. [14 Sloppy Shuffles Needed to Randomize a Deck](#item-20) ⭐️ 7.0/10
21. [LastPass Breach Exposes Customer Support Data via Klue](#item-21) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Critical FFmpeg Flaw Allows RCE via Malicious Videos](https://cybernews.com/security/critical-ffmpeg-vulnerability-enables-complete-compromise/) ⭐️ 9.0/10

A critical remote code execution vulnerability, CVE-2026-8461 (dubbed PixelSmash), was discovered in FFmpeg's MagicYUV decoder, allowing attackers to fully compromise systems by playing or storing a malicious 50 KB video file. FFmpeg released version 8.1.2 to fix the issue. FFmpeg is the most widely used media processing library, embedded in applications like VLC, Jellyfin, Kodi, OBS, and Nextcloud, affecting billions of devices including desktops, servers, NAS, and IoT devices. This vulnerability enables silent, no-trace attacks, making immediate updating critical. The flaw is a heap out-of-bounds write in the MagicYUV decoder within libavcodec, with a CVSS score of 8.8. It can be triggered not only by playing a video but also by automatic thumbnail generation or media library scanning, and affects all platforms where FFmpeg is used.

telegram · zaihuapd · Jun 23, 15:00

**Background**: FFmpeg is a free, open-source multimedia framework used by virtually all video players, streaming services, and media servers to decode, encode, and process audio and video. The MagicYUV codec is a lossless video codec designed for high-speed editing, but its decoder in FFmpeg had an out-of-bounds write vulnerability that could be exploited for code execution.

<details><summary>References</summary>
<ul>
<li><a href="https://jfrog.com/blog/pixelsmash-critical-ffmpeg-vulnerability-turns-media-files-into-weapons/">CVE - 2026 - 8461 Turns Video into a Host for Remote Code Execution</a></li>
<li><a href="https://www.bleepingcomputer.com/news/security/ffmpeg-fixes-pixelsmash-flaw-in-widely-used-video-decoder/">FFmpeg fixes PixelSmash flaw in widely used video decoder</a></li>

</ul>
</details>

**Tags**: `#ffmpeg`, `#vulnerability`, `#remote code execution`, `#security`, `#cve`

---

<a id="item-2"></a>
## [China's LineShine Supercomputer Tops TOP500 After 8 Years](https://news.mydrivers.com/1/1131/1131573.htm) ⭐️ 9.0/10

On June 23, the LineShine supercomputer, deployed at the National Supercomputing Center in Shenzhen, achieved first place in the TOP500 list with 2.198 ExaFLOPS on the HPL benchmark, becoming the first pure CPU system to exceed 2 ExaFLOPS. This marks China's return to the top of the supercomputing rankings after an eight-year gap, demonstrating significant progress in domestic CPU technology and national tech autonomy, especially amid US GPU export restrictions. LineShine uses 40,960 LX2 processors, each with 304 Armv9 cores running at 1.55 GHz, totaling 2.45 million cores. It also leads the HPCG benchmark and ranks fourth in HPL-MxP mixed-precision testing.

telegram · zaihuapd · Jun 23, 15:30

**Background**: The TOP500 list ranks the world's most powerful supercomputers based on the High-Performance Linpack (HPL) benchmark, which measures double-precision floating-point performance. The previous top system was the US' El Capitan, which uses GPU accelerators. LineShine's achievement is notable because it relies solely on CPUs, avoiding dependence on advanced GPUs that are subject to US export controls.

<details><summary>References</summary>
<ul>
<li><a href="https://www.hpcwire.com/2026/04/28/china-unveils-2-exaflop-all-cpu-lineshine-supercomputer/">China Unveils 2 Exaflop, All-CPU 'LineShine' Supercomputer - HPCwire</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/artificial-intelligence/china-bypasses-us-gpu-bans-with-1-54-exaflops-lineshine-supercomputer-cpu-only-monster-packs-2-4-million-huawei-designed-armv9-cores">China bypasses US GPU bans with 1.54-exaflops 'LineShine' supercomputer — CPU-only monster packs 2.4 million Huawei-designed Armv9 cores | Tom's Hardware</a></li>
<li><a href="https://www.tomshardware.com/tech-industry/supercomputers/chinas-lineshine-supercomputer-dethrones-us-el-capitan-secures-first-place-in-top-500-list-first-machine-in-the-rankings-to-sustain-more-than-2-exaflops-of-double-precision-performance-using-only-cpus">China's LineShine supercomputer dethrones US' El Capitan, secures first place in Top 500 list — first machine in the rankings to sustain more than 2 ExaFLOPS of double-precision performance using only CPUs | Tom's Hardware</a></li>

</ul>
</details>

**Tags**: `#supercomputing`, `#TOP500`, `#HPC`, `#China`, `#LineShine`

---

<a id="item-3"></a>
## [WYSIWYG TikZ Editor with Live Source Sync](https://tikz.dev/editor/) ⭐️ 8.0/10

An open-source WYSIWYG TikZ editor has been released that allows users to edit TikZ figures by dragging and resizing elements, with the source code and rendered figure staying in sync. The editor was built almost entirely using the Codex coding agent. This tool addresses a major pain point for academics and LaTeX users who manually code TikZ figures, significantly reducing the time spent tweaking coordinates and recompiling. It also demonstrates how AI coding agents can enable the creation of complex software that would otherwise be too tedious to build. The editor parses TikZ code and tracks the exact source location of each object, allowing it to override only the numbers in coordinates when dragging without altering other code structure. It also includes converters from SVG, PPTX, and IPE to TikZ, and reimplements LaTeX hyphenation and line-breaking for multi-line nodes.

hackernews · DominikPeters · Jun 23, 14:24 · [Discussion](https://news.ycombinator.com/item?id=48645437)

**Background**: TikZ is a powerful LaTeX package for creating vector graphics programmatically, widely used in academic papers. Traditionally, users write code with commands like \draw and recompile repeatedly to adjust positions, which is time-consuming. A WYSIWYG (What You See Is What You Get) editor allows direct visual manipulation, but existing tools rarely combine visual editing with live source code synchronization.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/PGF/TikZ">PGF/TikZ - Wikipedia</a></li>
<li><a href="https://www.overleaf.com/learn/latex/TikZ_package">TikZ package - Overleaf, Online LaTeX Editor</a></li>
<li><a href="https://en.wikipedia.org/wiki/WYSIWYG_editor">WYSIWYG editor</a></li>

</ul>
</details>

**Discussion**: Commenters praised the project for addressing a real need, with one user noting they had wanted such a tool as a student. However, some criticized the generated TikZ code for using absolute coordinates unnecessarily, suggesting it could be improved. Others compared it to specialized tools like quiver.app and inquired about support for Typst's cetz package.

**Tags**: `#LaTeX`, `#TikZ`, `#editor`, `#academic tools`, `#open source`

---

<a id="item-4"></a>
## [The Coming Loop: AI Agents Reshape Software Development](https://lucumr.pocoo.org/2026/6/23/the-coming-loop/) ⭐️ 8.0/10

Armin Ronacher, creator of Flask, argues that AI coding agents introduce a new 'loop' where developers must invest more time upfront in writing specifications and iterating with the agent, shifting the development paradigm towards a more biological, lifeform-like relationship with code. This paradigm shift could fundamentally change how software is designed and maintained, placing greater emphasis on specification writing and iterative refinement rather than direct coding, affecting all developers who adopt AI coding agents. Ronacher notes that while agents can generate code quickly, they require clear, detailed specifications to produce quality results, and developers often need multiple iterations to refine both the spec and the output. The essay highlights that this loop mirrors the process of understanding a problem through repeated failed attempts.

hackernews · ingve · Jun 23, 11:06 · [Discussion](https://news.ycombinator.com/item?id=48643180)

**Background**: Armin Ronacher is a prominent open-source developer known for creating the Flask web framework and Jinja templating engine. AI coding agents, such as those built on large language models, can generate code from natural language prompts but often struggle with complex or ambiguous requirements. The 'loop' refers to the iterative cycle of specification writing, agent execution, and refinement that developers experience when using these tools.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Armin_Ronacher">Armin Ronacher</a></li>
<li><a href="https://tosea.ai/blog/loop-engineering-ai-agents-complete-guide-2026">What Is Loop Engineering? A Complete Guide from Prompt... | Tosea. ai</a></li>
<li><a href="https://digg.com/tech/mumvj4el">Geoffrey Litt argues AI coding agents struggle with UI because...</a></li>

</ul>
</details>

**Discussion**: Commenters largely agree with Ronacher's thesis, noting that they are bottlenecked on specification writing rather than code generation. Some observe that the loop is most effective when developers have a clear understanding of what they want, and that agents can excel when given precise specs. Others highlight the paradigm shift towards treating software as a living organism that requires nurturing rather than direct control.

**Tags**: `#AI agents`, `#software development`, `#paradigm shift`, `#specification`, `#programming`

---

<a id="item-5"></a>
## [Unlimited OCR: Constant Memory for Long Document Parsing](https://github.com/baidu/Unlimited-OCR) ⭐️ 8.0/10

Baidu researchers introduced Unlimited OCR, a method that replaces standard attention with causal reference-based sliding window attention (R-SWA) to keep KV cache memory constant regardless of output length, enabling one-shot parsing of entire documents without page-by-page chunking. This breakthrough removes a major bottleneck in end-to-end OCR for long documents, making it feasible to process entire books or reports in a single pass without running out of GPU memory, which could significantly improve efficiency in digitization, archival, and document analysis workflows. The method achieves constant memory usage while maintaining or improving accuracy on parsing tasks, and the paper is available on arXiv (2606.23050). The implementation is open source on GitHub under the Baidu organization.

hackernews · ingve · Jun 23, 11:35 · [Discussion](https://news.ycombinator.com/item?id=48643426)

**Background**: In transformer-based OCR models, the key-value (KV) cache stores past token representations to avoid recomputation, but its memory footprint grows linearly with output length, causing out-of-memory errors on long documents. Traditional workarounds involve chunking documents into pages, which can lose context and reduce accuracy. Unlimited OCR's R-SWA mechanism constrains attention to a fixed-size sliding window, eliminating linear memory growth.

<details><summary>References</summary>
<ul>
<li><a href="https://pandaily.com/baidu-unlimited-ocr-constant-kv-cache-jun2026">Baidu Unveils Unlimited-OCR: Constant KV Cache Delivers SOTA Performance on Long Documents - Pandaily</a></li>
<li><a href="https://www.xugj520.cn/en/archives/unlimited-ocr-constant-memory.html">Unlimited OCR: One-Shot Long-Horizon Document Parsing with Constant Memory | Efficient Coder</a></li>
<li><a href="https://arxiv.org/html/2606.23050v1">Unlimited OCR Works Welcome the Era of One-shot Long-horizon Parsing</a></li>

</ul>
</details>

**Discussion**: The Hacker News community praised the work as a clever architectural hack, with users noting applications like sheet music recognition and expressing appreciation for the team's acknowledgment of DeepSeek-OCR and PaddleOCR. Some also pointed out the Fate/stay night reference in the project name.

**Tags**: `#OCR`, `#AI`, `#memory optimization`, `#deep learning`, `#open source`

---

<a id="item-6"></a>
## [Google Fires Employee Over Unofficial Workspace CLI](https://twitter.com/JPoehnelt/status/2069482265953087602) ⭐️ 8.0/10

Justin Poehnelt, a Google employee, was fired for creating and releasing an unofficial Google Workspace CLI tool that could be mistaken for an official Google product. This incident highlights tensions between employee innovation and corporate bureaucracy, raising questions about open-source policies and the risks of side projects at major tech companies. The tool, released under Poehnelt's personal account, was a GitHub hit but violated Google's policy against releasing projects that could be confused with official offerings. Poehnelt likely received prior warnings before termination.

hackernews · justinwp · Jun 23, 18:13 · [Discussion](https://news.ycombinator.com/item?id=48649011)

**Background**: Google has a history of terminating employees for policy violations related to internal tools, such as a 2019 case where an employee was fired for modifying a security tool. The company's 20% time policy, which once encouraged side projects, has been scaled back. The Google Workspace CLI (gws) is an official tool now, but Poehnelt's unofficial version predated it.

<details><summary>References</summary>
<ul>
<li><a href="https://grokipedia.com/page/Google_Workspace_CLI">Google Workspace CLI</a></li>
<li><a href="https://github.com/googleworkspace/cli">GitHub - googleworkspace/cli: Google Workspace CLI — one command-line tool for Drive, Gmail, Calendar, Sheets, Docs, Chat, Admin, and more. Dynamically built from Google Discovery Service. Includes AI agent skills.</a></li>
<li><a href="https://www.theverge.com/2019/12/17/21024472/google-employee-fired-labor-rights-notification-tool">Google employee says she was fired for sending internal pop-ups about labor rights | The Verge</a></li>

</ul>
</details>

**Discussion**: Comments are divided: some criticize Poehnelt's lack of judgment for releasing a tool that could be confused with an official product, while others see it as a case of bureaucratic overreach, citing Pournelle's Iron Law of Bureaucracy. Some former Googlers note that publishing under personal accounts was common but warn that this case crossed a line.

**Tags**: `#Google`, `#CLI`, `#Open Source`, `#Corporate Policy`, `#Bureaucracy`

---

<a id="item-7"></a>
## [Prompt Injection as Role Confusion: LLMs Prioritize Style Over Content](https://simonwillison.net/2026/Jun/22/prompt-injection-as-role-confusion/#atom-everything) ⭐️ 8.0/10

Research by Charles Ye, Jasmine Cui, and Dylan Hadfield-Menell shows that LLMs cannot reliably distinguish privileged text (e.g., system prompts) from untrusted user input because they prioritize the style of text over its content, leading to effective jailbreaks. This finding reveals a fundamental flaw in LLM security, suggesting that current defenses against prompt injection are inherently fragile and may require a paradigm shift in how models perceive roles. The researchers introduced 'destyling'—rewriting text to look less like the expected format in role tags—which reduced attack success rates from 61% to 10% in their dataset, even though the meaning remained unchanged to humans.

rss · Simon Willison · Jun 22, 23:59

**Background**: Prompt injection is a cybersecurity exploit where malicious inputs cause LLMs to behave unintendedly, often bypassing safety guardrails. LLMs are trained to follow instructions but struggle to distinguish between developer-defined prompts and user inputs, especially when the style mimics internal role tags like <system> or <assistant>.

<details><summary>References</summary>
<ul>
<li><a href="https://role-confusion.github.io/">Prompt Injection as Role Confusion</a></li>
<li><a href="https://arxiv.org/html/2603.12277v2">Prompt Injection as Role Confusion</a></li>
<li><a href="https://en.wikipedia.org/wiki/Prompt_injection">Prompt injection</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlights appreciation for the blog-style writeup and concern that role confusion makes prompt injection a 'perpetual whack-a-mole game.' Some commenters question whether genuine role perception is achievable with current architectures.

**Tags**: `#prompt injection`, `#LLM security`, `#role confusion`, `#jailbreak`, `#AI safety`

---

<a id="item-8"></a>
## [Moebius 0.2B Inpainting Model Ported to Browser via WebGPU](https://simonwillison.net/2026/Jun/22/porting-moebius/#atom-everything) ⭐️ 8.0/10

Simon Willison successfully ported the Moebius 0.2B lightweight image inpainting model to run entirely in the browser using WebGPU, with a live demo available at simonw.github.io/moebius-web/. The port was accomplished using Claude Code and ONNX Runtime Web on the WebGPU backend. This makes advanced image inpainting accessible without requiring a dedicated GPU, enabling users to run the model directly in their browser on any device with WebGPU support. It demonstrates the growing feasibility of running sophisticated AI models client-side, reducing server costs and improving privacy. The original Moebius model required PyTorch and NVIDIA CUDA, but the browser port uses ONNX Runtime Web with the WebGPU backend for inference. The model is only 0.2B parameters yet achieves performance comparable to 10B+ models like FLUX.1 on inpainting benchmarks.

rss · Simon Willison · Jun 22, 23:43

**Background**: Image inpainting is the task of filling in missing or removed regions of an image with plausible content. Moebius is a lightweight framework that achieves high-quality inpainting with only 0.2 billion parameters, challenging the notion that large foundation models are necessary. WebGPU is a modern browser API that enables GPU-accelerated compute and AI inference directly in the browser, maturing into a W3C Recommendation in 2026.

<details><summary>References</summary>
<ul>
<li><a href="https://arxiv.org/abs/2606.19195">[2606.19195] Moebius: 0.2B Lightweight Image Inpainting ...</a></li>
<li><a href="https://github.com/hustvl/Moebius">GitHub - hustvl/Moebius: [ECCV 2026] Moebius: 0.2B ...</a></li>
<li><a href="https://hustvl.github.io/Moebius/">Moebius: 0.2B Lightweight Image Inpainting Framework with 10B ...</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion (referenced in the article) likely praised the practical porting effort and the use of Claude Code for agentic coding. Some commenters may have discussed the trade-offs between browser-based and server-side inference, or the potential for other models to be ported similarly.

**Tags**: `#image inpainting`, `#WebGPU`, `#browser AI`, `#model porting`, `#machine learning`

---

<a id="item-9"></a>
## [OpenAI to produce AI-animated film 'Critterz' for under $30M](https://t.me/zaihuapd/42125) ⭐️ 8.0/10

OpenAI is backing the production of an animated feature film titled 'Critterz', which will be created primarily using OpenAI's own AI tools, including GPT-5. The film has a budget of under $30 million and a production timeline of just 9 months, significantly less than traditional animated films. This marks OpenAI's first foray into feature-length film production, demonstrating the potential of generative AI to drastically reduce costs and production time in the animation industry. If successful, it could disrupt traditional animation workflows and accelerate the adoption of AI in creative industries. The film is scheduled to premiere at the Cannes Film Festival and will be released globally in theaters in 2026. OpenAI's GPT-5, which offers PhD-level capabilities across various tasks, will be a key tool in the production process.

telegram · zaihuapd · Jun 23, 03:11

**Background**: Traditional animated films typically cost over $100 million and take 3-5 years to produce. OpenAI's GPT-5 is a significant leap over previous models, featuring state-of-the-art performance in coding, writing, and visual perception, making it suitable for complex creative tasks like filmmaking.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/GPT-5">GPT-5 - Wikipedia</a></li>
<li><a href="https://openai.com/index/introducing-gpt-5/">Introducing GPT-5 | OpenAI</a></li>
<li><a href="https://openai.com/gpt-5/">GPT-5 is here | OpenAI</a></li>

</ul>
</details>

**Tags**: `#OpenAI`, `#AI filmmaking`, `#animation`, `#GPT-5`, `#generative AI`

---

<a id="item-10"></a>
## [Valve Announces Steam Machine Console Starting at $1049](https://store.steampowered.com/hardware/steammachine) ⭐️ 8.0/10

Valve announced a new Steam Machine, a compact gaming console running SteamOS 3, with a starting price of $1049 and claiming over 6 times the performance of the Steam Deck. This marks Valve's return to the console market after a decade, potentially offering a high-performance, PC-like gaming experience in a living room form factor, challenging traditional consoles and PC gaming. The Steam Machine is a small cube-shaped device designed to connect to a TV or monitor, includes a Steam Controller wireless adapter, and features customizable LED lighting that can show game download progress.

telegram · zaihuapd · Jun 23, 04:53

**Background**: Steam Machines were originally released in 2015 but were discontinued by 2018 due to poor market reception. The new model runs SteamOS 3, which is based on Arch Linux and includes Proton for Windows game compatibility. The Steam Deck, a handheld gaming PC released in 2022, has been a major success for Valve, and the new Steam Machine appears to leverage that success with a more powerful home console form factor.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Steam_Machine">Steam Machine</a></li>
<li><a href="https://en.wikipedia.org/wiki/SteamOS">SteamOS</a></li>
<li><a href="https://store.steampowered.com/steamos/">SteamOS</a></li>

</ul>
</details>

**Tags**: `#gaming`, `#hardware`, `#Valve`, `#SteamOS`, `#console`

---

<a id="item-11"></a>
## [US Humanoid Robots Rely on Chinese Components: WSJ](https://t.me/zaihuapd/42129) ⭐️ 8.0/10

The Wall Street Journal reports that US humanoid robots increasingly depend on Chinese supply chains for critical components such as motors, joints, magnets, and sensors. Disney's 'Olaf' robot uses parts from China's Unitree, and Tesla is working with Chinese suppliers to prepare for Optimus mass production. This dependency highlights a significant geopolitical and industrial trend, where US robotics firms rely on Chinese manufacturing for cost advantages. It raises concerns about supply chain security and competitiveness, prompting US lawmakers to propose legislation assessing risks. China launched 28 humanoid robot models in 2025, nearly three times the number from US companies. Morgan Stanley estimates that Chinese supply chains can reduce manufacturing costs by up to two-thirds.

telegram · zaihuapd · Jun 23, 07:47

**Background**: Humanoid robots require complex components like motors, joints, and sensors to move and interact. China has become a dominant producer of these parts due to its manufacturing scale and cost efficiency. US companies like Tesla and Disney are leveraging Chinese suppliers to accelerate development and reduce costs.

<details><summary>References</summary>
<ul>
<li><a href="https://m.163.com/dy/article/JO7AAQTE051100B9.html">m.163.com/dy/article/JO7AAQTE051100B9.html</a></li>
<li><a href="https://cloud.tencent.com/developer/news/4070576">机构：特斯拉Optimus V3推动人形机器人产业发展，超10家中国供应商已...</a></li>
<li><a href="https://zhuanlan.zhihu.com/p/1988193930685223756">人形机器人关键零部件：电机全景解析 - 知乎</a></li>

</ul>
</details>

**Tags**: `#humanoid robots`, `#supply chain`, `#US-China tech competition`, `#robotics`, `#manufacturing`

---

<a id="item-12"></a>
## [SpaceX Falcon Heavy to Launch ESA Mars Rover in 2028](https://t.me/zaihuapd/42133) ⭐️ 8.0/10

NASA confirmed on Thursday that SpaceX's Falcon Heavy rocket has been selected to launch the European Space Agency's Rosalind Franklin Mars rover in late 2028 from Kennedy Space Center. The mission aims to search for signs of past or present life beneath the Martian surface. This milestone ends over two decades of delays and budget issues for the ExoMars program, securing a ride for Europe's first deep-drilling Mars rover. The collaboration between NASA, ESA, and SpaceX strengthens international ties in Mars exploration and leverages Falcon Heavy's proven heavy-lift capability. The Rosalind Franklin rover is designed to drill up to two meters below the Martian surface, deeper than any previous rover, to collect samples for biosignature analysis. NASA will provide key hardware, including the launch service, the descent module's braking system, and radioisotope heater units.

telegram · zaihuapd · Jun 23, 10:47

**Background**: The Rosalind Franklin rover, originally part of the ExoMars program, was built by ESA with contributions from Roscosmos, but cooperation ended after Russia's invasion of Ukraine. NASA stepped in to provide launch and key components, and the mission is now scheduled for a 2028 launch on Falcon Heavy. Falcon Heavy is a super heavy-lift rocket composed of three Falcon 9 cores, capable of delivering large payloads to Mars.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Rosalind_Franklin_(rover)">Rosalind Franklin (rover)</a></li>
<li><a href="https://en.wikipedia.org/wiki/Falcon_Heavy">Falcon Heavy - Wikipedia Falcon Heavy - SpaceX Images SpaceX Falcon Heavy — 12+ Flights, Specs, Payload & Mission ... SpaceX launch vehicles - Wikipedia Falcon Heavy & Starman - YouTube Starship's Twelfth Flight Test - SpaceX Falcon Heavy Compendium - ElonX.net</a></li>
<li><a href="https://arstechnica.com/space/2026/04/after-a-saga-of-broken-promises-a-european-rover-finally-has-a-ride-to-mars/">After a saga of broken promises, a European rover ... - Ars Technica</a></li>

</ul>
</details>

**Tags**: `#SpaceX`, `#Mars mission`, `#NASA`, `#ESA`, `#space exploration`

---

<a id="item-13"></a>
## [FUTO Swipe: New Swipe Typing Model Released](https://swipe.futo.tech/) ⭐️ 7.0/10

FUTO has released FUTO Swipe, a new swipe typing model for its privacy-focused keyboard, trained on user-contributed data to rival Gboard's accuracy. This addresses a major pain point for privacy-conscious users who previously had to sacrifice swipe typing quality for offline functionality, potentially shifting the mobile keyboard landscape toward open-source, privacy-respecting alternatives. The swipe library is licensed under GPLv3, while the Android keyboard app uses a separate FUTO License. The model is available on Hugging Face and was trained on data from users who opted in.

hackernews · futohq · Jun 23, 17:50 · [Discussion](https://news.ycombinator.com/item?id=48648619)

**Background**: Swipe typing allows users to input words by sliding a finger across letters, relying on a neural model to predict the intended word. FUTO Keyboard is a fully offline, open-source keyboard for Android that prioritizes privacy, but its swipe accuracy lagged behind Gboard. This new model aims to close that gap.

<details><summary>References</summary>
<ul>
<li><a href="https://keyboard.futo.org/">FUTO Keyboard</a></li>
<li><a href="https://huggingface.co/models?other=swipe-typing">Models – Hugging Face</a></li>
<li><a href="https://play.google.com/store/apps/details?id=org.futo.inputmethod.latin.playstore&hl=en_US">FUTO Keyboard - Apps on Google Play</a></li>

</ul>
</details>

**Discussion**: Users report that the new model feels as good as Gboard, with some converting to full-time use. However, issues like random capitalization and lack of context-aware suggestions remain. One commenter noted licensing differences between the swipe library (GPLv3) and the keyboard app (FUTO License).

**Tags**: `#mobile keyboard`, `#swipe typing`, `#machine learning`, `#open source`, `#privacy`

---

<a id="item-14"></a>
## [Swift Package Index Acquired by Apple](https://swiftpackageindex.com/blog/swift-package-index-joins-apple) ⭐️ 7.0/10

Apple has acquired the Swift Package Index (SPI), a community-maintained package search engine for Swift packages. The SPI team will join Apple to work on improving the Swift package ecosystem. This acquisition signals Apple's increased investment in the Swift package ecosystem, but raises concerns about the future openness and governance of the index. The community worries that Apple may impose restrictions or prioritize its own interests over community needs. The SPI team explicitly mentioned developer identity as a future direction, which has sparked unease. The index currently only supports GitHub repositories, and some community members see this as an opportunity to create alternatives.

hackernews · JDevlieghere · Jun 23, 18:00 · [Discussion](https://news.ycombinator.com/item?id=48648779)

**Background**: The Swift Package Index is a community-run search engine that helps developers discover Swift packages and check their compatibility with various platforms. It was created to address the lack of a central package registry for Swift, which is Apple's programming language for iOS, macOS, and other platforms. Package registries like npm for JavaScript or PyPI for Python are common in other ecosystems, but Swift has relied on decentralized solutions.

<details><summary>References</summary>
<ul>
<li><a href="https://sesamedisk.com/apple-joins-swift-package-index/">What Happened: Apple Joins Swift Package Index - Sesame Disk</a></li>
<li><a href="https://www.swift.org/packages/">Packages | Swift .org</a></li>

</ul>
</details>

**Discussion**: Community reactions are mixed: some are happy for the SPI team's success, while others are skeptical about Apple's track record with open source and developer services. Concerns include potential regulation of indexed packages and the focus on developer identity.

**Tags**: `#Swift`, `#Apple`, `#Package Management`, `#Open Source`, `#Ecosystem`

---

<a id="item-15"></a>
## [Vitamin D Benefits Real but Limited to Deficient](https://dynomight.net/vitamin-d/) ⭐️ 7.0/10

A critical review of vitamin D studies concludes that benefits are real but primarily for those with severe deficiency, countering both hype and dismissal. This nuanced analysis helps clarify the ongoing debate about vitamin D supplementation, guiding both public health recommendations and individual decisions. The review highlights that many studies fail to measure baseline vitamin D levels, and that benefits are most pronounced in those with levels below 30 nmol/L.

hackernews · surprisetalk · Jun 23, 16:30 · [Discussion](https://news.ycombinator.com/item?id=48647486)

**Background**: Vitamin D is a fat-soluble vitamin essential for bone health and immune function. Deficiency is common in regions with limited sunlight, and supplementation is widely debated.

**Discussion**: Commenters praised the balanced analysis, with some noting that vitamin K2 may aid absorption and that individual dosing varies. Others pointed out methodological flaws in earlier studies.

**Tags**: `#nutrition`, `#vitamin D`, `#health research`, `#evidence-based medicine`

---

<a id="item-16"></a>
## [California AB 2047 Targets 3D Printers with Gun Detection Mandate](https://www.the3dprintingnerd.com/ab2047) ⭐️ 7.0/10

California Assembly Bill 2047, introduced in 2025, would require all 3D printers sold in the state to include firearm blueprint detection software by July 1, 2028, and criminalize the use of open-source alternatives. If passed, AB 2047 would set a precedent for regulating 3D printing technology in the US, potentially stifling innovation in education and small businesses while raising serious concerns about censorship and technical feasibility. The bill mandates manufacturers to submit an attestation for each printer model confirming the inclusion of a firearm blueprint detection algorithm, and it explicitly prohibits the use of open-source firmware that bypasses this requirement.

hackernews · Buildstarted · Jun 23, 22:12 · [Discussion](https://news.ycombinator.com/item?id=48652184)

**Background**: 3D printers can be used to manufacture plastic firearm components, including so-called 'ghost guns' that lack serial numbers. California has previously passed laws restricting 3D-printed firearms, but AB 2047 is the first to mandate detection technology directly in printers. Critics argue that such software is technically infeasible because 3D printers read geometric data, not intent, and can be easily circumvented.

<details><summary>References</summary>
<ul>
<li><a href="https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260AB2047">Bill Text - AB-2047 Firearms: 3-dimensional printing blocking technology.</a></li>
<li><a href="https://www.eff.org/deeplinks/2026/04/dangers-californias-legislation-censor-3d-printing">The Dangers of California’s Legislation to Censor 3D Printing</a></li>
<li><a href="https://www.techspot.com/news/112594-california-assembly-passes-bill-requiring-gun-blocking-software.html">California passes bill requiring gun-blocking software in 3D ...</a></li>

</ul>
</details>

**Discussion**: Community comments express strong opposition, with users drawing analogies to failed content filtering systems and noting that motivated individuals can easily bypass such restrictions. Some speculate that the bill is funded by Bloomberg-backed lobbying, while others question the actual threat of 3D-printed weapons, suggesting they are statistical outliers.

**Tags**: `#3D printing`, `#regulation`, `#California law`, `#education`, `#technology policy`

---

<a id="item-17"></a>
## [Datasette 1.0a35 Adds Create/Alter Table Interfaces](https://simonwillison.net/2026/Jun/23/datasette/#atom-everything) ⭐️ 7.0/10

Datasette 1.0a35 introduces a new 'Create table' interface and 'Alter table' interface, both backed by JSON APIs, allowing users to define columns, primary keys, constraints, and more via the web UI or programmatically. This release is a major step toward Datasette 1.0, significantly expanding its capabilities as a data exploration and publishing tool by enabling schema management through the UI and API, which was previously only possible via SQLite commands. The 'Create table' API supports defining columns, primary keys, custom column types, NOT NULL constraints, literal defaults, expression defaults, and single-column foreign keys. The 'Alter table' API supports adding, renaming, reordering, and dropping columns, as well as changing column types, defaults, constraints, primary keys, foreign keys, and renaming the table.

rss · Simon Willison · Jun 23, 21:34

**Background**: Datasette is an open-source tool for exploring and publishing tabular data. It provides a web interface and JSON API for querying SQLite databases. Prior to this release, creating or altering table schemas required direct SQLite commands or external tools, limiting Datasette's usability as a full-featured database management interface.

<details><summary>References</summary>
<ul>
<li><a href="https://docs.datasette.io/en/latest/json_api.html">JSON API - Datasette documentation</a></li>
<li><a href="https://datasette.io/blog/2026/datasette-apps/">Host applications inside Datasette with Datasette ... - Datasette Blog</a></li>

</ul>
</details>

**Tags**: `#datasette`, `#open-source`, `#data-exploration`, `#release`

---

<a id="item-18"></a>
## [Chinese Universities Cut Foreign Language Programs](https://t.me/zaihuapd/42130) ⭐️ 7.0/10

Multiple Chinese universities, including University of International Business and Economics and Beijing Language and Culture University, have announced the suspension of master's programs in Japanese translation and Italian interpretation, among other languages. Jinan University has stopped enrolling for nine undergraduate language majors such as Korean and German, while Shenyang Aerospace University paused ten programs including English in 2024. This trend reflects a significant shift in higher education priorities, driven by declining enrollment, changing job market demands, and the impact of AI on language professions. It affects thousands of students and faculty, and signals a broader reevaluation of language education in China. From 2018 to 2022, 109 Chinese universities discontinued 28 language-related majors, with Japanese, English, and Korean being the most frequently dropped. The cuts span both undergraduate and graduate levels, and include prestigious institutions.

telegram · zaihuapd · Jun 23, 08:32

**Background**: Foreign language programs in China have faced declining interest due to factors such as lower college entrance exam scores, competition from AI translation tools, and limited job prospects. Many students now prefer to combine language skills with other fields like business or law, leading to a shift toward interdisciplinary programs. The trend is not unique to China; similar declines have been observed in South Korea and other countries.

<details><summary>References</summary>
<ul>
<li><a href="https://m.163.com/dy/article/KOJ0A7UJ0519E3QB.html">m.163.com/dy/article/KOJ0A7UJ0519E3QB.html</a></li>
<li><a href="https://www.thepaper.cn/newsDetail_forward_28451132">多校官宣：外语专业，停招_澎湃号·湃客_澎湃新闻-The Paper</a></li>
<li><a href="https://news.qq.com/rain/a/20240929A05YTL00">多所高校保研结果出炉：小语种本科生跨专业保研是“人才流失”吗？_腾讯新闻</a></li>

</ul>
</details>

**Tags**: `#higher education`, `#foreign language`, `#China`, `#academic trends`, `#policy`

---

<a id="item-19"></a>
## [Samsung Unveils UFS 5.0 with 10.8 GB/s for On-Device AI](https://news.samsung.com/global/samsung-unveils-industrys-fastest-ufs-5-0-solution-for-next-gen-on-device-ai-applications) ⭐️ 7.0/10

Samsung announced UFS 5.0, the industry's fastest universal flash storage solution, achieving sequential read speeds up to 10.8 GB/s and write speeds up to 9.5 GB/s, with mass production planned for Q4 2026. This breakthrough more than doubles the bandwidth of UFS 4.1, enabling faster data loading for on-device AI applications in flagship smartphones, XR headsets, and AI wearables, which is critical as AI processing moves to edge devices. UFS 5.0 is based on the latest JEDEC embedded memory interface standard, offers up to 1 TB capacity, improves power efficiency by over 40% compared to Samsung's UFS 4.1, and reduces package size by 16.7%.

telegram · zaihuapd · Jun 23, 09:17

**Background**: Universal Flash Storage (UFS) is a high-performance storage standard widely used in mobile devices. On-device AI refers to running artificial intelligence models directly on the device rather than in the cloud, requiring fast data access for real-time processing. JEDEC is the standards body that defines UFS specifications.

<details><summary>References</summary>
<ul>
<li><a href="https://news.samsung.com/global/samsung-unveils-industrys-fastest-ufs-5-0-solution-for-next-gen-on-device-ai-applications">Samsung Unveils Industry’s Fastest UFS 5.0 Solution for Next-Gen On-Device AI Applications</a></li>
<li><a href="https://semiconductor.samsung.com/estorage/ufs/ufs-5-0/">UFS 5.0 | Universal Flash Storage | Samsung Semiconductor Global</a></li>
<li><a href="https://www.sammobile.com/2026/06/23/samsung-worlds-fastest-ufs-5-0-storage-chip-announced-debut-galaxy-s27/">Samsung unveils UFS 5.0 storage chip, could debut with... - SamMobile</a></li>

</ul>
</details>

**Tags**: `#storage`, `#Samsung`, `#UFS`, `#AI`, `#hardware`

---

<a id="item-20"></a>
## [14 Sloppy Shuffles Needed to Randomize a Deck](https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/) ⭐️ 7.0/10

New research extends the classic 1992 result that 7 perfect riffle shuffles randomize a 52-card deck, showing that under realistic, imprecise shuffling conditions, about 14 shuffles are required. This finding refines our understanding of randomization in real-world scenarios, with implications for probability theory, algorithm design, and any field relying on random permutations. The researchers assigned binary barcodes to each card to track their paths through the shuffle and identified 'cold spots' of residual order, proving a cutoff phenomenon exists even for imprecise shuffles. However, the current model still assumes cards interleave one by one, not in clumps.

telegram · zaihuapd · Jun 23, 16:04

**Background**: The Gilbert–Shannon–Reeds model is a standard mathematical model for riffle shuffles, assuming a deck is split into two piles of approximately equal size and then interleaved. The cutoff phenomenon describes a sharp transition from ordered to random as the number of shuffles increases. Classic work by Bayer and Diaconis in 1992 showed that 7 perfect riffle shuffles suffice for a 52-card deck under ideal conditions.

<details><summary>References</summary>
<ul>
<li><a href="https://www.quantamagazine.org/seven-perfect-shuffles-randomize-a-deck-of-cards-but-how-many-sloppy-ones-20260617/">Seven Perfect Shuffles Randomize a Deck of Cards . | Quanta Magazine</a></li>
<li><a href="https://nadialafreniere.github.io/Snapshot_cutoff_first_submission_english.pdf">Cutoff phenomenon : Surprising behaviour in card shuffling and other...</a></li>

</ul>
</details>

**Tags**: `#mathematics`, `#probability`, `#randomization`, `#card shuffling`

---

<a id="item-21"></a>
## [LastPass Breach Exposes Customer Support Data via Klue](https://techcrunch.com/2026/06/23/password-manager-maker-lastpass-says-hackers-stole-customer-support-case-data-during-klue-breach/) ⭐️ 7.0/10

LastPass disclosed that customer support case data and personal information were stolen in a breach of its partner Klue, which was hacked by the Icarus group on June 12, 2026. This incident underscores the cascading risks of third-party integrations, especially for a password manager with over 33 million users, though password vaults remain secure. Stolen data includes names, phone numbers, email addresses, physical addresses, support case records, and sales-related data. LastPass stated its own infrastructure and password vaults were not compromised.

telegram · zaihuapd · Jun 24, 00:49

**Background**: LastPass suffered a severe breach in 2022 where attackers exfiltrated encrypted password vaults, leading to a $24.5 million class action settlement. The Klue breach is an OAuth-based supply chain attack, where a compromised integration credential allowed access to Salesforce data across multiple firms.

<details><summary>References</summary>
<ul>
<li><a href="https://techcrunch.com/2026/06/22/klue-hack-results-in-data-breach-at-several-cybersecurity-firms/">Klue hack results in data breach at several cybersecurity... | TechCrunch</a></li>
<li><a href="https://cybersecuritynews.com/klue-hack-cybersecurity-companies/">Klue Hack Leads to Data Breach Across Multiple Cybersecurity...</a></li>
<li><a href="https://en.wikipedia.org/wiki/LastPass_2022_data_breach">LastPass 2022 data breach</a></li>

</ul>
</details>

**Tags**: `#security`, `#data breach`, `#LastPass`, `#password manager`

---