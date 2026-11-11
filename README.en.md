# Awesome Gemini 4 Carbon

> A community catalog of public [Gemini 4 Carbon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/) use cases. This repository is not an official Google or Google DeepMind project and is not endorsed by them.

[简体中文](README.md) | [English](README.en.md)

Browse the [GitHub Pages catalog](https://xianyu110.github.io/awesome-gemini-4-carbon/).


This list currently has **59** verified cases (as of 2026-11-11, Asia/Shanghai). Carbon was announced on 2026-10-28 for a subset of cybersecurity defenders and opened more widely on 2026-11-10 to paying developers, enterprises, and Google AI Ultra subscribers. Public, checkable primary cases are still accumulating. Every entry has a source URL that was actually opened; we do not invent names, numbers, or URLs.

## What the model is

Google describes **Gemini 4 Carbon** as its strongest model for cybersecurity and long-horizon agentic work: complex multi-step coding and debugging, open-ended scientific research, and dense enterprise knowledge work. **Gemini 4 Argon** remains what Google calls the better default for most software engineering and knowledge work. This list includes a case only when a source clearly says Carbon did the work. Argon-only results are excluded.

Surfaces include the paid Gemini API / [Google AI Studio](https://aistudio.google.com/prompts/new_chat?model=gemini-4-carbon), Gemini for business, Android Studio, Google Antigravity (including `/swarm` in preview), the Gemini app and AI Mode in Search for Google AI Ultra, and the [Fairwind Program](https://deepmind.google/fairwind-program/) for defenders (Carbon for cyber). The model ID is `gemini-4-carbon`.

Introductory price (official, through 2026-11-30): $2 per million input tokens and $10 per million output tokens; $4 / $20 from 2026-12-01. Implicit cached input is discounted on the official pricing page. Carbon is not on the free tier.

## Official links

| Resource | Notes |
| --- | --- |
| [Carbon is now available](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/) | 10 Nov 2026 launch post; primary source for most official demos and partner results |
| [Introducing Gemini 4 Carbon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) | 28 Oct 2026 announcement (Fairwind-first) |
| [Carbon and /swarm in Antigravity](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/) | `/swarm` preview and internal dogfooding |
| [Developer note](https://blog.google/innovation-and-ai/technology/developers-tools/gemini-4-carbon-developers/) | Short developers’ announcement |
| [Developer Guide](https://aistudio.google.com/learn/gemini-4-carbon-developer-guide) / [What's new](https://aistudio.google.com/docs/whats-new-gemini-4-carbon) | API, thinking levels, long decode, migration |
| [Pricing](https://aistudio.google.com/docs/pricing) | Official rates |
| [Model card](https://storage.googleapis.com/deepmind-media/Model-Cards/Gemini-4-Carbon-Model-Card.pdf) / [card page](https://deepmind.google/models/model-cards/gemini-4-carbon/) | Official model card |
| [Safety and Security Report](https://storage.googleapis.com/deepmind-media/gemini/gemini_4_carbon_safety_report.pdf) | Official safety PDF |
| [AlphaProof Code](https://deepmind.google/blog/introducing-alphaproof-code/) · [paper](https://deepmind.google/documents/36/Formal_Verification_of_Signal_4.pdf) · [artifacts](https://google-deepmind.github.io/code-verification) | Signal verification |
| [Fairwind Program](https://deepmind.google/fairwind-program/) | Defender access |

Official playable demos (a Google account may be required):

- [Pelican Quest](https://aistudio.google.com/apps/bundled/pelican-campus-quest)
- [Merchandise Store reimagining](https://aistudio.google.com/apps/bundled/gemini-supply)
- [Koerner Hall fortepiano](https://aistudio.google.com/apps/bundled/koerner-hall)

## Scope

- **59** cases. Breakdown: official demos 8, cybersecurity 6, science 3, software engineering 4, knowledge work / evals 2, community 36.
- One case is one distinct project, demo, or published result, not a restated capability bullet.
- Cybersecurity entries stay high-level (what was found or fixed in public terms). They do not include exploit steps, PoCs, payloads, or reproduction procedures.
- Leaderboard scores (CursorBench, WANDR, AutomationBench, SEC-bench Pro, and so on) are listed under Benchmarks and ecosystem and are not counted as cases.
- Structured data: [`cases.json`](cases.json).

## Contents

- [Official demos and creative engineering](#official-demo) (8)
- [Cybersecurity and formal verification](#cybersecurity) (6)
- [Scientific research](#science) (3)
- [Software engineering (mostly internal)](#engineering) (4)
- [Knowledge work and financial evaluations](#knowledge-work) (2)
- [Community work](#community) (36)
- [Benchmarks and ecosystem](#benchmarks)
- [Contributing](#contributing)

<a id="official-demo"></a>

## Official demos and creative engineering

### 1. Interactive Three.js exhibition of the Eiffel Tower's 1887–1889 construction

Google says a team of Gemini 4 Carbon agents used Antigravity /swarm to turn a single prompt, historical photos, and engineering plates into an interactive Three.js 3D exhibition of the Eiffel Tower’s 1887–1889 construction.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 官方上市博文中的独立演示。未提供单独试玩链接。

### 2. 906K-triangle reconstruction of Google’s Platform 37 office

Google says a multi-agent Carbon team used seven public City Council planning PDFs (206 extracted engineering drawing views) and a single prompt to build an interactive 906K-triangle Three.js reconstruction of Google’s Platform 37 office across 10 overnight loops.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 数字（7 份 PDF、206 张图、906K 三角面、10 轮通宵循环）均来自同一篇官方博文。未提供单独试玩链接。

### 3. Interactive multiscale textile visualizer with 110-fiber tracking

Google says Carbon built an interactive multiscale textile visualizer in Antigravity from an academic paper, with a virtual-fiber finite element framework, interactive 3D yarn meshes, 110-fiber polar tracking, and dynamic stress-strain curves, with minimal prompting. A later Google post says it was based on a 2026 study of knitted textile mechanics.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 补充来源：https://x.com/Google/status/2120279087314837642 （2026-11-11 06:15 Asia/Shanghai）。

### 4. Pelican Quest: open-world campus game of a pelican on a GBike

Google says /swarm coordinated subagents to model 3D assets in Blender from Omni and Nano Banana references, build a browser open-world game in Three.js with WebGL shaders, and pair procedural Web Audio with Lyria music. You explore the Mountain View campus as a pelican on a GBike. The app is playable in Google AI Studio. Sundar Pichai added that builder and critic subagents checked their own renders.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Sundar Pichai
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://aistudio.google.com/apps/bundled/pelican-campus-quest 。补充：https://x.com/Google/status/2120260356413051147 、https://x.com/sundarpichai/status/2120198811297694192 。OrcaRouter 拆解文指出试玩页可能需要 Google 登录。

### 5. Google Merchandise Store reimagined in two prompts

Google says Carbon, in Antigravity, reimagined the Google Merchandise Store in two prompts, proposing five art-direction concepts and generating all-new product imagery with Nano Banana 2.1. A live app and a Gemini front-end design skill are linked from the post.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://aistudio.google.com/apps/bundled/gemini-supply 。商品图由 Nano Banana 2.1 生成，协调与站点构建由 Carbon 完成。

### 6. Cinematic multi-shot underwater Atlantis scene

Google says that, starting from a Gemini Omni video reference in Antigravity, the pipeline modeled procedural ruins, volumetric caustic lighting, and water simulation in Blender, then converted the environment to Three.js for real-time browser rendering of a cinematic multi-shot underwater Atlantis scene.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 视频参考来自 Gemini Omni；场景建模与转到 Three.js 的工作在官方叙述中由 Carbon 完成。未提供单独试玩链接。

### 7. Playable c. 1780 Stein-Schule fortepiano in Koerner Hall

Google says a multi-agent loop in Antigravity reconstructed a playable c. 1780 Stein-Schule fortepiano with 61-key escapement physics from CAD drawings and X-ray radiographs, and placed it in a 3D model of Koerner Hall with seat-specific spatial acoustics. A live app is linked.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://aistudio.google.com/apps/bundled/koerner-hall 。

### 8. Reverse-engineering Theme Park binaries and porting the park to the web

Demis Hassabis wrote that Carbon reverse-engineered his original Theme Park binaries, added a new DeepMind-themed ride, and ported the game to the web in one shot, calling the result “kind of mindblowing to see.” The Verge reported the same claim. No public play URL was attached.

- Source: [https://x.com/demishassabis/status/2120210297948696997](https://x.com/demishassabis/status/2120210297948696997)
- Author / org: Demis Hassabis
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖时间为 2026-11-10 17:41 UTC，即 2026-11-11 01:41 Asia/Shanghai。补充报道：https://www.theverge.com/ai-artificial-intelligence/1031117/demis-hassabis-used-ai-to-reverse-engineer-his-own-game-and-port-it-to-the-web 。原作与 Peter Molyneux / Bullfrog 有关，以 Hassabis 自述为准。

<a id="cybersecurity"></a>

## Cybersecurity and formal verification

### 9. Project Fortify scanning and triage on Google’s internal benchmark

Google says that in Project Fortify, its autonomous system for scanning, triage, and remediation, Carbon hit 100% recall on scanning and 95% precision on triage on an internal benchmark. This entry records only those public figures.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 内部基准，数字来自 Google 自述。与下文开源仓库测试是同一节里的另一项结果。

### 10. Previously undetected real-world logic flaws in open-source repository testing

Google says open-source repository testing showed more than a 25% relative improvement over Argon’s already strong recall, surfacing previously undetected real-world logic flaws. Only the public claim is recorded.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google / Google DeepMind
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 「超过 25% 相对提升」是相对 Argon 召回率的官方表述，不是独立复现结果。

### 11. Cloud Vulnerability Research proved two OSS bugs were exploitable

Google says its Cloud Vulnerability Research team used Carbon to prove that two bugs in a popular open-source project were exploitable, at severity comparable to the recent PHP2Shell exploit, and that a Carbon-built proof of concept helped maintainers reclassify the issue as critical and ship a patch. Details will follow responsible disclosure. No exploit steps are included here.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google Cloud Vulnerability Research
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 软件名称、CVE 与技术细节官方尚未公开。

### 12. Wiz Scan for Good found 0-days in two major SaaS providers

Google says Wiz, in Scan for Good, used Carbon when scanning two major SaaS providers and uncovered 0-day vulnerabilities in under two hours, then worked with the organizations to remediate. This entry records only that public account.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Wiz（经 Google 转述）
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 截至收录时未找到 Wiz 就这两起 Carbon 发现发布的独立技术博客。更早的 Scan for Good 文章写的是 Gemini 3.8 Flash Cyber / Argon，不能当作本条来源。

### 13. AlphaProof Code formally verified libsignal at machine-code level

DeepMind says AlphaProof Code was used to prove key security properties of the actual libsignal implementation down to compiled AArch64 machine code. Humans worked with models (Carbon and, per the paper, also Claude Opus 5.5) on specifications; Carbon-powered prover agents then generated about 6.5 million lines of machine-checked Lean. The work took five researchers about four weeks. Two previously fixed bugs were reintroduced to show the specs catch real flaws. Artifacts are open-sourced. No exploit procedure is included.

- Source: [https://deepmind.google/blog/introducing-alphaproof-code/](https://deepmind.google/blog/introducing-alphaproof-code/)
- Author / org: Google DeepMind（Swarat Chaudhuri、Pushmeet Kohli 等）
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 技术论文：https://deepmind.google/documents/36/Formal_Verification_of_Signal_4.pdf （约 650 万行证明、约 2.6 万行可信规范与 AArch64 语义）。开源站点：https://google-deepmind.github.io/code-verification 。Sundar Pichai 帖：https://x.com/sundarpichai/status/2120207062655549933 。论文也写明结果针对的是其 libsignal-cli 构建，而非 Signal 自家应用；部分分析排除旁路等。不收录任何利用步骤。

### 14. Chrome team reported Carbon produced high-quality patches more than 10× better than another lab’s model

Google’s 28 October post says the Chrome team reported that Carbon performed more than 10× better than another lab’s large frontier model when generating high-quality patches. The other model is unnamed.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)
- Author / org: Google（转述 Chrome 团队）
- Date: 2026-10-28 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 对照模型未点名。属于团队内部使用反馈，不是公开复现实验。

<a id="science"></a>

## Scientific research

### 15. Axiom Bio found novel toxicity mechanisms with Carbon

Google says that for Axiom Bio, Carbon is now the leading model in performance for translational science and found novel mechanisms of toxicity the company had not found previously. Axiom is moving production scientific analyses and agents to both Carbon and Argon.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Axiom Bio（经 Google 转述）
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 截至收录时未找到 Axiom Bio 就 Carbon 结果发布的独立技术文章。迁移对象同时包括 Carbon 与 Argon。

### 16. Enzyme assay development: diagnosing wet-lab artifacts from notebooks and raw data

Google says researchers gave Carbon only lab notebooks and raw data. It surfaced hard-to-interpret anomalies, diagnosed subtle wet-lab artifacts such as incomplete automated mixing in deep wells, improved chromatography peak deconvolution, and caught trace sample carryover, speeding assay development. Multiple findings in one workstream are kept as a single case.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google 研究者
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 同一研究工作流中的多项发现，按官方段落收录为一条，不拆成多条凑数。

### 17. Remote-homolog discovery for low-homolog protein families in CASP17

Google says researchers used Carbon in a multi-agent setup to discover remote homologs in petabase-scale unannotated archives and related catalogs. Across 7 low-homolog protein families from the CASP17 blind test set, Carbon increased homologs retrieved by 40-fold on average, without retraining structure models. Broader benchmarking is still underway.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Google 研究者
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 40 倍为官方对这 7 个家族的平均值；文中写明更广泛基准仍在进行。

<a id="engineering"></a>

## Software engineering (mostly internal)

### 18. Internal dogfooding: multi-package migrations with /swarm

The Antigravity team says that in five weeks of internal /swarm dogfooding, Google engineers used swarms on gnarly multi-package migrations. No public repo is attached.

- Source: [https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- Author / org: The Antigravity Team
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 与下文根因调查、架构重设计同出一篇博文的三类不同任务，分开收录。官方也提醒并行多智能体会更快消耗配额。

### 19. Internal dogfooding: cross-subsystem root-cause investigations

The same post says internal engineers also used swarms for cross-subsystem root-cause investigations.

- Source: [https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- Author / org: The Antigravity Team
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 官方概括性描述，不是可复现的外部项目。

### 20. Internal dogfooding: complex architectural redesigns

The same post also names complex architectural redesigns as a /swarm dogfooding task, with Carbon suited to coordinator, architecture, and auditing roles.

- Source: [https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- Author / org: The Antigravity Team
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 官方概括性描述。上市博文也把多包迁移、跨子系统根因和架构重设计列为 Carbon 擅长的多智能体工程任务。

### 21. Internal teams ran Carbon for days on subtle low-level bugs

The 28 October announcement says internal teams have seen Carbon run for days and persist through dead ends on complex multi-step tasks such as root-causing and patching subtle bugs across large codebases and low-level systems.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)
- Author / org: Google / Google DeepMind
- Date: 2026-10-28 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 没有公开具体仓库或缺陷编号，属内部使用观察。

<a id="knowledge-work"></a>

## Knowledge work and financial evaluations

### 22. Matched the best model on Hebbia’s E2E Financial Agentic evaluation

Google says that in pre-release evaluations, Carbon matched the best model tested on Hebbia’s E2E Financial Agentic evaluation for deep financial research.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Hebbia（经 Google 转述）
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 分数与对照模型名单未在该博文中列出。

### 23. Ranked top of 23 frontier configurations on Balyasny’s GFI benchmark

Google says Carbon ranked at the top of 23 frontier model configurations on Balyasny Asset Management’s General Financial Intelligence benchmark, spanning legal expertise, agentic tool use, coding and data engineering, and perception and context understanding.

- Source: [https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- Author / org: Balyasny Asset Management（经 Google 转述）
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 具体分项分数未在该博文中列出。

<a id="community"></a>

## Community work

### 24. CUDA/C++ meadow of 52,000 wildflowers and grass blades

GlitterPixely wrote that they made a grass meadow from scratch in CUDA and C++ with no game engine or 3D library: 52k blades and wildflowers, and synthesized the wind sound in C++ so the audio follows the same gusts. Google later quoted the same details.

- Source: [https://x.com/GlitterPixely/status/2120264316092022895](https://x.com/GlitterPixely/status/2120264316092022895)
- Author / org: @GlitterPixely
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 21:16 UTC（2026-11-11 05:16 Asia/Shanghai）。Google 转发：https://x.com/Google/status/2120324708826550328 。数字与实现细节为作者自述。

### 25. TIDEFORGE: 1,048,576-particle WebGPU simulation

kimmonismus wrote that for TIDEFORGE they asked for a million particles; it runs 1,048,576, with motion calculated by WebGPU compute, and that all the site code is from Carbon with no follow-up prompts. Google amplified the post.

- Source: [https://x.com/kimmonismus/status/2120186202271945137](https://x.com/kimmonismus/status/2120186202271945137)
- Author / org: @kimmonismus
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 16:05 UTC（2026-11-11 00:05 Asia/Shanghai）。Google 转发：https://x.com/Google/status/2120324710307131464 。

### 26. Stained-glass Jenga with tap-to-ring and shatter physics

AI_Andrew published a playable stained-glass Jenga at vitrail.andrewvoirol.com, with tap-to-sound and a smash sandbox. Google described it as using Carbon to simulate how the tower catches the light, rings when tapped, and shatters.

- Source: [https://x.com/AI_Andrew/status/2120243379388760176](https://x.com/AI_Andrew/status/2120243379388760176)
- Author / org: @AI_Andrew
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://vitrail.andrewvoirol.com 。原帖 2026-11-10 19:53 UTC。Google 转发：https://x.com/Google/status/2120324716238086357 。

### 27. Fourteen hosted apps from messy public datasets

giyu_codes said they had early access, asked Carbon to find underserved industries in public data, and shipped 14 hosted apps testing messy multi-source reconciliation plus 3D WebGL physics, using four existing apps as architectural references. Google pointed to the thread of all 14 builds. Counted as one case.

- Source: [https://x.com/giyu_codes/status/2120201582319190381](https://x.com/giyu_codes/status/2120201582319190381)
- Author / org: @giyu_codes
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 14 个应用按官方转发与作者主题帖收录为一条，不拆成 14 条。原帖 2026-11-10 17:07 UTC。Google 转发：https://x.com/Google/status/2120324719086088676 。

### 28. Interactive 19th-century Parisian optics lab from one reference image

thebuggeddev said Carbon built an interactive 19th-century-inspired Parisian physics lab, Analyse Spectrale (Mod. M1-2-15), from a single reference image, with 92 brass, copper, and borosilicate parts and several live instrument/UI features. Google amplified the post.

- Source: [https://x.com/thebuggeddev/status/2120201759305998343](https://x.com/thebuggeddev/status/2120201759305998343)
- Author / org: @thebuggeddev
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 17:07 UTC。Google 转发：https://x.com/Google/status/2120324721816539520 。零件数量与物理效果为作者自述。

### 29. Biomechanical clockwork heart in Three.js

sunset_evm posted that Gemini 4 Carbon built a biomechanical clockwork heart in Three.js with /swarm in Antigravity, and asked viewers to turn sound on.

- Source: [https://x.com/sunset_evm/status/2120308090180714970](https://x.com/sunset_evm/status/2120308090180714970)
- Author / org: @sunset_evm
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-11 00:10 UTC（2026-11-11 08:10 Asia/Shanghai）。作者自述，未见独立试玩页。

### 30. Working twin-turbo V8 engine built in FreeCAD and Blender

ai_for_success showed a working 1,600 HP twin-turbo V8 you can uncover, rev, and hear, and later said Carbon built it with FreeCAD and Blender in Antigravity in about 6–7 hours including the demo video.

- Source: [https://x.com/ai_for_success/status/2120317619588972867](https://x.com/ai_for_success/status/2120317619588972867)
- Author / org: @ai_for_success
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 细节帖：https://x.com/ai_for_success/status/2120187068634837203 。功率、耗时为作者自述。

### 31. F1 racing game plus Unreal Engine and Blender MCPs

athrix_codes said they had early access and built an F1 racing game in Antigravity with Unreal Engine MCP and Blender MCP, and that both MCPs were also made by Carbon.

- Source: [https://x.com/athrix_codes/status/2120193545344786446](https://x.com/athrix_codes/status/2120193545344786446)
- Author / org: @athrix_codes
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 16:35 UTC。游戏与两个 MCP 由同一作者在同一帖中说明，收录为一条。对比评价为作者观感。

### 32. 3D music visualizer for 12 renowned symphonies

soumyadesign said one of the first things they built with Carbon in Antigravity was a 3D visualizer that spatially represents scores from 12 renowned symphonies, using WebGL, Three.js, Gaussian Splats, and thin-film gradients. A live site is available.

- Source: [https://x.com/soumyadesign/status/2120200838899712246](https://x.com/soumyadesign/status/2120200838899712246)
- Author / org: @soumyadesign
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://music-visualiser.ai.studio/ （从作者帖中的短链解析得到，收录时 HTTP 200）。原帖 2026-11-10 17:04 UTC。

### 33. Destroyed Coventry Cathedral rebuilt from historic plans and photographs

Leslie Nooteboom wrote that Carbon built the destroyed Coventry Cathedral from scratch, scanning historic floorplans and photographs to generate a cinematic walkthrough video.

- Source: [https://x.com/LeslieNooteboom/status/2120204269173563872](https://x.com/LeslieNooteboom/status/2120204269173563872)
- Author / org: @LeslieNooteboom
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 17:17 UTC。作者自述，影片在原帖中。

### 34. Interactive voxel character studio (Sailor)

cgm_ai posted an interactive voxel character with walk cycles, mouse gaze, expressions, three spells, and live slicing in HTML + WebGL2, and linked a playable page.

- Source: [https://x.com/cgm_ai/status/2120327608433102929](https://x.com/cgm_ai/status/2120327608433102929)
- Author / org: @cgm_ai
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 试玩：https://tdgl.codes/games/sailor-voxel-studio/ 。原帖 2026-11-11 01:27 UTC（2026-11-11 09:27 Asia/Shanghai）。

### 35. One-prompt remake of Atari 2600 Pitfall

Glenn Gabe said that while testing Carbon in the Gemini app early-access program, he rebuilt Atari 2600 Pitfall with one prompt in a few minutes and it “worked perfectly.”

- Source: [https://x.com/glenngabe/status/2120195911175254316](https://x.com/glenngabe/status/2120195911175254316)
- Author / org: @glenngabe（Glenn Gabe）
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 16:44 UTC。作者自述，未见单独试玩链接。

### 36. Single-file Three.js New York City cruiser tour

StatsWire posted that Carbon built an interactive 3D New York City cruiser tour in a single HTML file with Three.js and no external 3D models or audio assets, crediting a video inspiration.

- Source: [https://x.com/StatsWire/status/2120344850071540152](https://x.com/StatsWire/status/2120344850071540152)
- Author / org: @StatsWire
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-11 02:36 UTC（2026-11-11 10:36 Asia/Shanghai）。实现细节为发帖者自述。

### 37. Perihelion: pelican ride through a vertical ring at eclipse

kayshen_xu described Perihelion, a Carbon pelican test in which the bird rides into a vertical sea ring and passes inverted in front of an eclipse. They called the Python SDK directly, then finished a truncated output into a standalone HTML file.

- Source: [https://x.com/kayshen_xu/status/2120151206270267864](https://x.com/kayshen_xu/status/2120151206270267864)
- Author / org: @kayshen_xu
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 13:46 UTC（2026-11-10 21:46 Asia/Shanghai）。作者明确写了自己补了被截断后的交互。

### 38. Ethan Mollick reproduced a video clip in Three.js

Ethan Mollick said he had early access to Carbon, found it a strong improvement on Argon, and showed a demo in which Carbon reproduced a video clip in Three.js.

- Source: [https://x.com/emollick/status/2120198832202125322](https://x.com/emollick/status/2120198832202125322)
- Author / org: @emollick（Ethan Mollick）
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 16:56 UTC。评价为作者观感；演示本身有原帖视频。

### 39. Simon Willison’s pelican-on-a-bicycle test at three thinking levels

Simon Willison ran his long-running pelican-on-a-bicycle test at Carbon’s low, medium, and high thinking levels and published the high-effort result in his llm-gemini 0.36 release notes.

- Source: [https://simonwillison.net/2026/Nov/10/llm-gemini/](https://simonwillison.net/2026/Nov/10/llm-gemini/)
- Author / org: Simon Willison
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 文章时间 2026-11-10 20:09（页面未标时区；按文中发布日收录）。这是独立复现，不是 Google 的 Pelican Quest 游戏。

### 40. Yonkers stands up as a mech and stomps around NYC with OSM data

In the same post, Willison used Carbon in Antigravity with a prompt he had tried on Claude Fable 5.2: a Three.js animation of Yonkers standing up as a mech and stomping around Manhattan, Queens, and Brooklyn using OpenStreetMap data, later packed into a standalone HTML file.

- Source: [https://simonwillison.net/2026/Nov/10/llm-gemini/](https://simonwillison.net/2026/Nov/10/llm-gemini/)
- Author / org: Simon Willison
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 与鹈鹕 SVG 测试是同一篇文章中的另一项独立实验。

### 41. Carbon designed a workflow to direct a DeepSeek harness

A Chinese-language post said the author had only 3% of their weekly tokens left, so they used Carbon to direct a DeepSeek harness (Deepseek v41 flash), and that Carbon designed a workflow that let DeepSeek work quickly.

- Source: [https://x.com/StateInterOffic/status/2120237344309841998](https://x.com/StateInterOffic/status/2120237344309841998)
- Author / org: @StateInterOffic
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: 原帖 2026-11-10 19:29 UTC。作者自述的工作流搭配，没有公开仓库。

### 42. Standalone HTML voxel scene with trains and airships (11.3M voxels)

@Adidotdev posted a standalone HTML file with about 11,286,682 voxels at 60fps, including moving viaduct trains, sky-harbor airships, and three live lighting modes. The author attributes the work to Gemini 4 Carbon and says the model was then shadow-routing under “gemini-4-argon”.

- Source: [https://x.com/Adidotdev/status/2120158160074002823](https://x.com/Adidotdev/status/2120158160074002823)
- Author / org: @Adidotdev
- Date: 2026-11-10 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 14:14 UTC (2026-11-10 22:14 Asia/Shanghai). Voxel count and 60fps are the author’s claim. The author later identified the early-access model as Carbon; this entry follows that attribution and does not treat the same video in third-party Argon/Arena catalogs as a separate case.

### 43. One-shot Three.js galloping zebra

@AI_Screening called this a Gemini 4 Carbon output, said Carbon was really good, fast, and cheap, and that it one-shotted this galloping zebra in Three.js.

- Source: [https://x.com/AI_Screening/status/2120185448727462301](https://x.com/AI_Screening/status/2120185448727462301)
- Author / org: @AI_Screening
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:02 UTC (2026-11-11 00:02 Asia/Shanghai). “One-shotted” is the author’s claim.

### 44. A full music video generated with code

@kickingkeys said they used Gemini 4 Carbon to make an entire music video with just code, and that they had had early access for about two weeks. The post also points to more examples and code below.

- Source: [https://x.com/kickingkeys/status/2120185497637024013](https://x.com/kickingkeys/status/2120185497637024013)
- Author / org: @kickingkeys
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:03 UTC (2026-11-11 00:03 Asia/Shanghai). This entry covers the music video shown in the post. It does not split “more examples” into extra unverified cases.

### 45. Pooperman, a Flappy Bird-style Three.js platformer

@SimonasLTU1 prompted Gemini 4 Carbon: “Create a game called pooperman, basically it's a flappy bird, but with a guy that poops on clicks, should be three.js graphics, but platformer style.” The author said it took 14 minutes.

- Source: [https://x.com/SimonasLTU1/status/2120186826451288182](https://x.com/SimonasLTU1/status/2120186826451288182)
- Author / org: @SimonasLTU1
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:08 UTC (2026-11-11 00:08 Asia/Shanghai). The game’s name and rules come from the author’s published prompt. The 14-minute timing is the author’s claim.

### 46. A 3D basketball court built with no premade 3D assets

@LexnLin said they had early access to Gemini 4 Carbon and built this 3D basketball court with it, with no premade 3D assets. The author also said Carbon improved a lot over Argon in areas that involve taste or visuals, such as 3D, websites, and motion graphics.

- Source: [https://x.com/LexnLin/status/2120186998707163533](https://x.com/LexnLin/status/2120186998707163533)
- Author / org: @LexnLin
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:09 UTC (2026-11-11 00:09 Asia/Shanghai). The comparison with Argon is the author’s impression.

### 47. Adiyogi Divya Darshanam 3D demo

@ai_for_success said they had early access, had been using Carbon for coding and 3D work, and showed the first of several things they had built with it: Adiyogi Divya Darshanam.

- Source: [https://x.com/ai_for_success/status/2120187064184664162](https://x.com/ai_for_success/status/2120187064184664162)
- Author / org: @ai_for_success
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:09 UTC (2026-11-11 00:09 Asia/Shanghai). This is a separate project from the same author’s already-listed twin-turbo V8. Only the named Adiyogi demo shown in the post is added; other works mentioned without their own sources are not split out.

### 48. A code-generated animation in a single HTML file

@itsPaulAi said Google had just released Gemini 4 Carbon and that the model produced the video in the post entirely with code, in a single HTML file. The author said they had used the model for the past few days.

- Source: [https://x.com/itsPaulAi/status/2120188198592663935](https://x.com/itsPaulAi/status/2120188198592663935)
- Author / org: @itsPaulAi
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:13 UTC (2026-11-11 00:13 Asia/Shanghai). The post includes a video but does not name the animation’s subject, so the title follows the author’s own description.

### 49. A 3D scene from a custom CUDA C++ VFX engine Carbon wrote

@fofrAI posted on launch day that Gemini 4 Carbon was powerful, and showed a 3D scene Carbon made using a custom CUDA C++ VFX engine it wrote.

- Source: [https://x.com/fofrAI/status/2120188535152222407](https://x.com/fofrAI/status/2120188535152222407)
- Author / org: @fofrAI
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:15 UTC (2026-11-11 00:15 Asia/Shanghai). This is a different author and project from the already-listed GlitterPixely CUDA meadow.

### 50. One star performing the 15 principles of animation in a single shot

@CodeByPoonam said Gemini 4 Carbon made one star performing 15 principles of animation in one continuous shot, with zero edits.

- Source: [https://x.com/CodeByPoonam/status/2120192694622580794](https://x.com/CodeByPoonam/status/2120192694622580794)
- Author / org: @CodeByPoonam
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:31 UTC (2026-11-11 00:31 Asia/Shanghai). “Zero edits” and “15 principles” are the author’s claims.

### 51. A 56-part Grand Celestial Planétarium Automaton in procedural Three.js

@StatsWire said “Gemini Carbon 4” built a 56-part Grand Celestial Planétarium Automaton from scratch in pure procedural Three.js, with zero external 3D models.

- Source: [https://x.com/StatsWire/status/2120199271588737356](https://x.com/StatsWire/status/2120199271588737356)
- Author / org: @StatsWire
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 16:57 UTC (2026-11-11 00:57 Asia/Shanghai). This is a separate project from the same author’s already-listed NYC cruiser. The part count and “no external models” claim are the author’s. The post says “Gemini Carbon 4”; in context it is catalogued as Gemini 4 Carbon.

### 52. An animation generated from a single reference image in JS and Python

@devteamdrew said the entire scene was made of pure code: a single reference image turned into an animation, with no skills or frameworks, in pure JS and Python, made using Google DeepMind’s Gemini 4 Carbon.

- Source: [https://x.com/devteamdrew/status/2120200837305884813](https://x.com/devteamdrew/status/2120200837305884813)
- Author / org: @devteamdrew
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 17:04 UTC (2026-11-11 01:04 Asia/Shanghai). “No frameworks” and “pure JS + Python” are the author’s claims.

### 53. A 32-second Pixar-style coral reef short film in pure code

@Adidotdev said they built a 32-second Pixar-style short film in pure code with Gemini 4 Carbon: about 4,800 corals awakening from bleached white, 3,600 schooling fish, Snell’s Window water optics, and a full ocean breach, in Three.js and GLSL, with orchestral audio also synthesized in code.

- Source: [https://x.com/Adidotdev/status/2120208990089175300](https://x.com/Adidotdev/status/2120208990089175300)
- Author / org: @Adidotdev
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 17:36 UTC (2026-11-11 01:36 Asia/Shanghai). This is a separate project from the same author’s voxel viaduct scene. Duration and counts are the author’s claims.

### 54. A playable 3D V12 hypercar coastal racer in a single HTML file

@StatsWire said Gemini 4 Carbon built a playable 3D V12 hypercar coastal racing game in a single HTML file with Three.js, describing a 9,250 RPM V12 wail, dual-clutch shift barks, stone sea-tunnel reverb, smoky hairpin drifts, and 340 km/h viaduct overtakes at 60fps.

- Source: [https://x.com/StatsWire/status/2120212182482682232](https://x.com/StatsWire/status/2120212182482682232)
- Author / org: @StatsWire
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 17:49 UTC (2026-11-11 01:49 Asia/Shanghai). Performance and sound details are the author’s claims.

### 55. Desk Racer, a miniature kart racing game in the browser

@anuragdotdev said Gemini 4 Carbon built Desk Racer, a miniature kart racing game that runs entirely in the browser, and listed four game modes and realistic 3D physics with Rapier3D, among other features.

- Source: [https://x.com/anuragdotdev/status/2120213817573740687](https://x.com/anuragdotdev/status/2120213817573740687)
- Author / org: @anuragdotdev
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 17:55 UTC (2026-11-11 01:55 Asia/Shanghai). The mode count and physics engine are the author’s claims. The post was truncated mid-list, so unseen items are not added here.

### 56. A minion scene with Carbon splitting work to a local model

@atomicagent_io said that in Atomic Agent Fusion, Gemini 4 Carbon split the prompt into tasks and sent them to a local Qwen 3.8 27B. For a minion scene, the author reported about 5 minutes and $2.39 with this setup, versus about 16 minutes and $7.71 with Gemini alone, and said Carbon was 3× cheaper and 3× faster.

- Source: [https://x.com/atomicagent_io/status/2120227531504918833](https://x.com/atomicagent_io/status/2120227531504918833)
- Author / org: @atomicagent_io
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 18:50 UTC (2026-11-11 02:50 Asia/Shanghai). This is a hybrid workflow: Carbon split the work and a local model helped generate the scene. Timing and cost are the author’s claims. Product promo links are not the basis for inclusion.

### 57. A game written from scratch with custom WebGL2 and ray-traced shaders

@ia_met said Gemini 4 Carbon in Antigravity one-shotted this project in exactly 70 minutes (about $8 in API tokens), writing about 6,800 lines of custom WebGL2 and ray-traced shaders from scratch with no external assets, then visually debugging its own screenshots.

- Source: [https://x.com/ia_met/status/2120228626608050335](https://x.com/ia_met/status/2120228626608050335)
- Author / org: @ia_met
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 18:54 UTC (2026-11-11 02:54 Asia/Shanghai). Line count, timing, cost, and “one-shotted” are the author’s claims. The post does not include a public play URL.

### 58. An SVG of two crabs approaching a pelican on a bicycle

@HarshithLucky3 said they used Gemini 4 Carbon medium in AI Studio to generate an SVG of “two aggressive crabs approaching pelican riding a bicycle.”

- Source: [https://x.com/HarshithLucky3/status/2120236571165368720](https://x.com/HarshithLucky3/status/2120236571165368720)
- Author / org: @HarshithLucky3
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 19:26 UTC (2026-11-11 03:26 Asia/Shanghai). This is the author’s own SVG, not Google’s official Pelican Quest game.

### 59. A Canvas artwork brushed up until it felt like teamLab

@Majin_AppSheet wrote in Japanese that they asked Gemini 4 Carbon to brush up a Canvas artwork they had made before, that the result now felt almost like teamLab, and that it made them want to watch The Tunnel to Summer, the Exit of Goodbyes.

- Source: [https://x.com/Majin_AppSheet/status/2120245677439783195](https://x.com/Majin_AppSheet/status/2120245677439783195)
- Author / org: @Majin_AppSheet
- Date: 2026-11-11 (Asia/Shanghai calendar day when a timestamp was available; official blog dates follow the page)
- Notes: Original post 2026-11-10 20:02 UTC (2026-11-11 04:02 Asia/Shanghai). The teamLab comparison is the author’s impression, not a claim of involvement or endorsement by that studio.

<a id="benchmarks"></a>

## Benchmarks and ecosystem

These are official or vendor-published capability and access notes. **They are not counted in the case total.**

- Google says Carbon ranked #1 on CursorBench 4.0, Perplexity’s WANDR, and Zapier’s AutomationBench, at more than 2× lower cost per task than the next best external model ([launch post](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)).
- Cursor’s account says Carbon is available in Cursor and is the top model on CursorBench at high effort, at 60.4% ([post](https://x.com/cursor_ai/status/2120193584670580857)). Demis Hassabis reposted it.
- At announcement, Google said Carbon scored 59 and ranked #1 on Artificial Analysis Intelligence Index v5.0, and led SEC-bench Pro (88.2%), ExploitGym (54.8%), and CWE-bench (71.0%) ([announcement](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)). Some cyber scores are described as Fairwind-access results. Scoreboards move; check the original pages.
- Google and Artificial Analysis launched the Multimodal Knowledge Agent (MKA) benchmark; Google says Carbon ranked #2 at more than 6× lower average cost per task than the top model.
- WebDev Arena: the announcement says Carbon jumped +89 Elo to #4 (1768).
- Simon Willison released [llm-gemini 0.36](https://simonwillison.net/2026/Nov/10/llm-gemini/), adding `gemini-4-carbon` to the `llm` CLI.
- The official safety report and launch post also cite external tests by Gray Swan and Trajectory Labs. Those are safety evaluations, not product use cases.

<a id="contributing"></a>

## Contributing

New verifiable public cases are welcome. See [CONTRIBUTING.md](CONTRIBUTING.md). Please update `README.md`, `README.en.md`, and `cases.json` together.

## License and notice

The catalog text is released under the [MIT License](LICENSE). Third-party works, trademarks, and media remain with their owners. See [NOTICE.md](NOTICE.md).

