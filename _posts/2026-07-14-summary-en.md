---
layout: default
title: "Horizon Summary: 2026-07-14 (EN)"
date: 2026-07-14
lang: en
---

> From 13 items, 8 important content pieces were selected

---

1. [Telegram's t.me Domain Suspended](#item-1) ⭐️ 8.0/10
2. [Samsung Health Threatens Data Deletion Over AI Training Opt-Out](#item-2) ⭐️ 8.0/10
3. [Open Data Saved Climate.gov After Government Removal](#item-3) ⭐️ 8.0/10
4. [DOOMQL: A Doom-like Game Built Entirely in SQLite](#item-4) ⭐️ 8.0/10
5. [Build and Ship Apple Apps Without Xcode](#item-5) ⭐️ 7.0/10
6. [Apple SpeechAnalyzer API Benchmarked vs Whisper](#item-6) ⭐️ 7.0/10
7. [Sega CD Silpheed: Art and Engineering of FMV 3D](#item-7) ⭐️ 7.0/10
8. [Datasette Code Frequency Chart Shows AI Agent Impact](#item-8) ⭐️ 7.0/10

---

<a id="item-1"></a>
## [Telegram's t.me Domain Suspended](https://www.whois.com/whois/t.me) ⭐️ 8.0/10

Telegram's t.me domain was suspended, likely due to legal investigations in Russia, France, or India, and the domain registrar GoDaddy may have enforced the suspension. This suspension could disrupt Telegram's link-sharing services and highlights the risks of relying on third-party domain registrars like GoDaddy, which can suspend domains under legal pressure. The domain status codes include 'clientRenewProhibited' and 'serverDeleteProhibited', which are typically used during legal disputes or when a domain is subject to deletion, according to ICANN.

hackernews · Tiberium · Jul 13, 19:52 · [Discussion](https://news.ycombinator.com/item?id=48897878)

**Background**: Telegram is a popular messaging app that uses t.me for short links to channels and users. Domain registrars like GoDaddy can suspend domains for policy violations or legal reasons. Telegram is currently under legal scrutiny in multiple countries, including Russia, France, and India.

<details><summary>References</summary>
<ul>
<li><a href="https://news.ycombinator.com/item?id=48897878">Telegram's t . me domain has been suspended | Hacker News</a></li>
<li><a href="https://www.igoldrush.com/author/toekneetv">toekneetv | iGoldRush Domain News and Resources</a></li>
<li><a href="https://www.nolo.com/legal-encyclopedia/works-public-domain-permission-29523.html">How Can I Use Copyright-Free Works (in the Public Domain )?</a></li>

</ul>
</details>

**Discussion**: Community comments express surprise that Telegram relied on GoDaddy, known for lack of transparency, and some users note they are moving to alternative platforms like Zulip. One commenter mentions using a redirect from a third-party domain to mitigate such risks.

**Tags**: `#Telegram`, `#domain suspension`, `#GoDaddy`, `#legal investigations`, `#internet governance`

---

<a id="item-2"></a>
## [Samsung Health Threatens Data Deletion Over AI Training Opt-Out](https://neow.in/cWsyMTV3) ⭐️ 8.0/10

Samsung Health updated its privacy settings, requiring users to consent to AI training on their health data or face permanent deletion of synced data and account termination. This policy forces users to choose between privacy and functionality, setting a concerning precedent for how tech companies handle sensitive health data and user consent. The data categories include sleep, medications, medical records, and cycle tracking; opting out triggers a pop-up warning that the app will delete the user's data.

hackernews · bundie · Jul 13, 20:01 · [Discussion](https://news.ycombinator.com/item?id=48897991)

**Background**: Samsung Health is a fitness and health tracking app pre-installed on Galaxy devices. AI training on user data can improve features like personalized insights, but requires access to sensitive biometric information. The updated policy effectively makes consent mandatory for continued use.

<details><summary>References</summary>
<ul>
<li><a href="https://cybernews.com/news/samsung-health-ai-training-delete-user-data/">Opt out of Samsung AI training, lose health data | Cybernews</a></li>
<li><a href="https://www.androidheadlines.com/2026/07/samsung-health-ai-data-training-deletion-policy.html">Samsung Health to Delete Data If Users Opt Out of AI</a></li>
<li><a href="https://9to5google.com/2026/07/13/samsung-health-ai-training-data-consent/">Samsung Health will delete your data without AI training consent</a></li>

</ul>
</details>

**Discussion**: Users expressed strong backlash, with some questioning the fairness of losing device functionality if they refuse consent, and others criticizing Samsung Health's poor user experience and data export issues. A few users sarcastically noted that data deletion could be seen as a privacy benefit.

**Tags**: `#privacy`, `#Samsung`, `#health data`, `#AI training`, `#data deletion`

---

<a id="item-3"></a>
## [Open Data Saved Climate.gov After Government Removal](https://werd.io/climate-gov-was-destroyed-open-data-saved-it/) ⭐️ 8.0/10

A blog post reports that open data efforts successfully preserved climate.gov data after it was removed from government websites, ensuring continued public access to taxpayer-funded climate information. This highlights the critical role of open data and decentralized archiving in preserving government information, especially when political changes threaten public access. It sparks debate on data ownership, funding, and the need for systemic preservation solutions. The preservation effort relied on donations and volunteer work, raising questions about long-term sustainability. The community discussed using decentralized systems like IPFS for default government publication of static content.

hackernews · benwerd · Jul 13, 19:57 · [Discussion](https://news.ycombinator.com/item?id=48897945)

**Background**: Climate.gov is a U.S. government website providing climate data and resources. Open data refers to data that is freely available for anyone to access, use, and share. The removal of such data from official sites can occur due to policy changes, and preservation efforts by volunteers and organizations aim to maintain public access.

**Discussion**: Commenters expressed gratitude for the data rescue but questioned long-term funding, with one noting that donations are not a substitute for tax dollars. Others debated whether government data should be public domain by default and suggested using IPFS for distributed archiving.

**Tags**: `#open data`, `#government transparency`, `#data preservation`, `#climate`, `#archiving`

---

<a id="item-4"></a>
## [DOOMQL: A Doom-like Game Built Entirely in SQLite](https://simonwillison.net/2026/Jul/13/doomql/#atom-everything) ⭐️ 8.0/10

Peter Gostev created DOOMQL, a Doom-like first-person shooter where the entire game engine—including movement, collision, enemies, combat, and rendering—is implemented using SQLite queries, with the game rendered as pixel art in a terminal via Python. This project demonstrates an extreme and creative misuse of SQLite, pushing the boundaries of what a database can do and inspiring developers to think differently about software architecture. It also showcases the power of recursive CTEs for complex computations like ray tracing. The game uses a single massive SQL query with a recursive CTE to implement a full ray tracer for rendering. The game state is stored in a SQLite database, which can be explored and visualized in real-time using Datasette with a custom HTML+JavaScript app.

rss · Simon Willison · Jul 13, 22:34

**Background**: SQLite is a self-contained, serverless SQL database engine widely used in applications for local storage. Recursive Common Table Expressions (CTEs) allow SQL queries to perform iterative computations, which DOOMQL leverages for ray casting. The original Doom (1993) popularized first-person shooters and used a 2.5D rendering technique.

<details><summary>References</summary>
<ul>
<li><a href="https://digg.com/tech/iuhrpvcu">Peter Gostev builds a Doom-like raycasting engine entirely in SQLite - Digg</a></li>
<li><a href="https://en.wikipedia.org/wiki/Doom_(1993_video_game)">Doom (1993 video game) - Wikipedia</a></li>

</ul>
</details>

**Discussion**: The community expressed delight and amazement at the technical cleverness and absurdity of building a playable game engine entirely in SQL, praising its creativity and the impressive feat of misusing a database.

**Tags**: `#SQLite`, `#game development`, `#creative coding`, `#Python`

---

<a id="item-5"></a>
## [Build and Ship Apple Apps Without Xcode](https://scottwillsey.com/building-and-shipping-mac-and-ios-apps-without-ever-opening-xcode/) ⭐️ 7.0/10

A developer demonstrates how to build, sign, and notarize macOS and iOS apps entirely from the command line and CI/CD pipelines, never opening Xcode. This workflow enables automation and integration with custom CI/CD systems, reducing reliance on Xcode's GUI and potentially speeding up development cycles for teams. The approach uses xcodebuild, codesign, and notarization tools from the command line, along with tools like Fastlane or custom scripts to handle provisioning and distribution.

hackernews · speckx · Jul 13, 18:22 · [Discussion](https://news.ycombinator.com/item?id=48896665)

**Background**: Xcode is Apple's integrated development environment (IDE) for building apps on Apple platforms. However, many developers prefer command-line tools for automation and CI/CD. The command-line tools for Xcode provide the necessary compilers and utilities without the full IDE.

<details><summary>References</summary>
<ul>
<li><a href="https://developer.apple.com/documentation/xcode/installing-the-command-line-tools/">Installing the command-line tools | Apple Developer Documentation</a></li>
<li><a href="https://blog.jetbrains.com/teamcity/2025/08/cicd-for-ios/">How to Build a CI/CD Pipeline for iOS Projects - The JetBrains Blog</a></li>
<li><a href="https://appcircle.io/guides/ios/ios-build">iOS Build Guide: Xcode, IPA, Code Signing & CI/CD Automation | Appcircle</a></li>

</ul>
</details>

**Discussion**: Commenters shared alternative tools like xtool for Linux builds and Axiom for LLM-assisted development, but also raised security concerns about running agents outside sandboxes, especially after xAI's home directory leak.

**Tags**: `#iOS development`, `#macOS`, `#CI/CD`, `#Xcode alternatives`, `#automation`

---

<a id="item-6"></a>
## [Apple SpeechAnalyzer API Benchmarked vs Whisper](https://get-inscribe.com/blog/apple-speech-api-benchmark.html) ⭐️ 7.0/10

A new benchmark compares Apple's SpeechAnalyzer API, introduced at WWDC 2025, against OpenAI's Whisper and Apple's previous speech framework, showing faster performance with slightly lower accuracy. This matters because Apple's on-device API could disrupt third-party transcription apps that rely on Whisper, offering a native, faster alternative for macOS and iOS users. The benchmark tested SpeechAnalyzer against Whisper-Large-V2 on a math lecture, finding it substantially faster and only slightly worse in accuracy. However, some commenters argue that newer models like Nvidia's Nemotron or Mistral's Voxtral are more relevant comparisons.

hackernews · get-inscribe · Jul 13, 16:06 · [Discussion](https://news.ycombinator.com/item?id=48894752)

**Background**: Whisper is an open-source speech recognition model by OpenAI, widely used for transcription. Apple's SpeechAnalyzer API, announced at WWDC 2025, is a modular on-device speech recognition framework designed to replace older Apple speech APIs.

<details><summary>References</summary>
<ul>
<li><a href="https://www.argmaxinc.com/blog/apple-and-argmax">Apple SpeechAnalyzer and Argmax WhisperKit - Argmax</a></li>
<li><a href="https://www.callstack.com/blog/on-device-speech-transcription-with-apple-speechanalyzer">On-Device Speech Transcription with Apple SpeechAnalyzer and AI SDK</a></li>
<li><a href="https://en.wikipedia.org/wiki/Whisper_(speech_recognition_system)">Whisper (speech recognition system)</a></li>

</ul>
</details>

**Discussion**: The Hacker News discussion highlights mixed views: some praise the API's speed for live transcription, while others note that Whisper wrappers may become obsolete if Apple builds a native recorder app. Commenters also suggest comparing against newer models like Voxtral or Nemotron.

**Tags**: `#speech recognition`, `#Apple`, `#benchmark`, `#ASR`, `#Whisper`

---

<a id="item-7"></a>
## [Sega CD Silpheed: Art and Engineering of FMV 3D](https://fabiensanglard.net/silpheed/index.html) ⭐️ 7.0/10

Fabien Sanglard published a detailed technical analysis of how the Sega CD game Silpheed used full-motion video (FMV) and clever engineering to simulate 3D graphics on limited hardware. This deep dive highlights a unique approach to 3D rendering in the early 1990s, offering valuable lessons for retro game developers and enthusiasts interested in hardware limitations and creative problem-solving. Silpheed used pre-rendered computer animation as FMV backgrounds, with the Sega CD mixing line-in audio from the Genesis to achieve synchronized sound. The article also corrects a common misconception about the audio setup, noting that the Genesis expansion port already mixed CD audio.

hackernews · ibobev · Jul 13, 14:52 · [Discussion](https://news.ycombinator.com/item?id=48893639)

**Background**: The Sega CD was a CD-ROM add-on for the Sega Genesis that allowed for larger games and full-motion video. Full-motion video (FMV) games used pre-recorded video files instead of real-time 3D rendering, often resulting in poor quality due to compression and small windows. Silpheed stood out by using pre-rendered 3D animation as the background, creating a convincing 3D experience.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Sega_CD">Sega CD - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Full-motion_video">Full-motion video - Wikipedia</a></li>
<li><a href="https://en.wikipedia.org/wiki/Silpheed">Silpheed - Wikipedia</a></li>

</ul>
</details>

**Discussion**: Commenters praised the article's depth and shared additional insights, such as the impressive demoscene demo 'Overdrive 2' for the Mega Drive. One user corrected the article's description of the audio setup, noting that the Genesis expansion port already handled CD audio mixing. Another pointed out that the submission was a repost due to RSS changes.

**Tags**: `#retro gaming`, `#game development`, `#Sega CD`, `#technical deep-dive`

---

<a id="item-8"></a>
## [Datasette Code Frequency Chart Shows AI Agent Impact](https://simonwillison.net/2026/Jul/13/datasette-code-frequency/#atom-everything) ⭐️ 7.0/10

Simon Willison analyzed the GitHub code frequency chart for his open-source project Datasette, revealing that the largest spike in code additions (37,022 additions in one week) occurred in 2026, coinciding with the use of advanced AI coding agents like Opus 4.8, GPT-5.5, Fable 5, and GPT-5.6 Sol. This analysis provides concrete, data-driven evidence of how AI-assisted coding tools can dramatically boost developer productivity, especially for solo maintainers of open-source projects. It sparks discussion on the evolving role of AI in software development and its potential to accelerate innovation. The chart shows sporadic bursts of activity from 2018 to 2026, with the largest spike being 37,022 additions and -9,528 deletions in 2026, followed by 14,638 additions in late 2025 and 15,998 additions in early 2018. A notable deletion spike of -10,658 occurred in mid-2020.

rss · Simon Willison · Jul 13, 21:45

**Background**: Datasette is an open-source tool for exploring and publishing tabular data, created by Simon Willison. GitHub's code frequency chart visualizes additions and deletions per week, providing a historical view of development activity. AI coding agents, such as Claude Opus 4.5 and GPT-5 series, are advanced language models that can generate code autonomously, potentially increasing development speed.

<details><summary>References</summary>
<ul>
<li><a href="https://azure.microsoft.com/en-us/blog/introducing-claude-opus-4-5-in-microsoft-foundry/">Introducing Claude Opus 4.5 in Microsoft Foundry | Microsoft Azure Blog</a></li>
<li><a href="https://techcrunch.com/2026/07/08/spacexai-releases-grok-4-5-which-elon-describes-as-an-opus-class-model/">SpaceXAI releases Grok 4.5, which Elon describes as an 'Opus-class model' | TechCrunch</a></li>

</ul>
</details>

**Tags**: `#AI-assisted development`, `#open source`, `#productivity`, `#coding agents`, `#data visualization`

---