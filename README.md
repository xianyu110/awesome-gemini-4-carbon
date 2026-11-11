# Awesome Gemini 4 Carbon

> 社区整理的 [Gemini 4 Carbon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/) 公开使用案例清单。本仓库不是 Google 或 Google DeepMind 的官方项目，也不代表其背书。

[简体中文](README.md) | [English](README.en.md)

当前收录 **59** 条已核验案例（截至 2026-11-11，Asia/Shanghai）。Carbon 于 2026-10-28 面向部分网络安全防御者宣布，2026-11-10 向付费开发者、企业与 Google AI Ultra 用户更广泛开放，公开、可核验的一手案例仍在增加。本清单宁缺毋滥：每条都有实际打开过的来源链接，不编造名称、数字或网址。

## 这是什么模型

按 Google 的定位，**Gemini 4 Carbon** 是其在网络安全与长周期智能体工作上最强的模型，面向复杂多步编码与调试、开放式科学研究、以及高密度的企业知识工作。同系列的 **Gemini 4 Argon** 仍被官方称为大多数软件工程和知识工作的日常首选。本清单只收录来源明确写明是 Carbon 完成的工作；仅属于 Argon 的案例不列入。

产品形态包括：付费 Gemini API / [Google AI Studio](https://aistudio.google.com/prompts/new_chat?model=gemini-4-carbon)、Gemini for business、Android Studio、Google Antigravity（含预览中的 `/swarm`）、Gemini 应用与搜索中的 AI Mode（Google AI Ultra）、以及面向防御者的 [Fairwind Program](https://deepmind.google/fairwind-program/)（Carbon for cyber）。模型 ID 为 `gemini-4-carbon`。

入门价（官方，至 2026-11-30）：每百万输入 token 2 美元、每百万输出 token 10 美元；2026-12-01 起为 4 / 20 美元。隐性缓存输入按官方定价页有折扣。Carbon 不在免费档。

## 官方链接

| 资源 | 说明 |
| --- | --- |
| [Carbon is now available](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/) | 2026-11-10 上市博文，多数官方演示与合作案例的一手来源 |
| [Introducing Gemini 4 Carbon](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/) | 2026-10-28 宣布博文（Fairwind 先发） |
| [Carbon and /swarm in Antigravity](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/) | `/swarm` 预览与内部试用 |
| [开发者简述](https://blog.google/innovation-and-ai/technology/developers-tools/gemini-4-carbon-developers/) | 面向开发者的短公告 |
| [Developer Guide](https://aistudio.google.com/learn/gemini-4-carbon-developer-guide) / [What's new](https://aistudio.google.com/docs/whats-new-gemini-4-carbon) | API、思考强度、长解码与迁移 |
| [定价](https://aistudio.google.com/docs/pricing) | 官方价目 |
| [Model card](https://storage.googleapis.com/deepmind-media/Model-Cards/Gemini-4-Carbon-Model-Card.pdf) / [模型卡页](https://deepmind.google/models/model-cards/gemini-4-carbon/) | 官方模型卡 |
| [Safety and Security Report](https://storage.googleapis.com/deepmind-media/gemini/gemini_4_carbon_safety_report.pdf) | 官方安全与安保报告 PDF |
| [AlphaProof Code](https://deepmind.google/blog/introducing-alphaproof-code/) · [论文](https://deepmind.google/documents/36/Formal_Verification_of_Signal_4.pdf) · [开源产物](https://google-deepmind.github.io/code-verification) | Signal 形式化验证 |
| [Fairwind Program](https://deepmind.google/fairwind-program/) | 网络安全防御者申请通道 |

可在浏览器里打开的官方演示（可能需要 Google 账号）：

- [Pelican Quest](https://aistudio.google.com/apps/bundled/pelican-campus-quest)
- [Merchandise Store 重做](https://aistudio.google.com/apps/bundled/gemini-supply)
- [Koerner Hall 古钢琴](https://aistudio.google.com/apps/bundled/koerner-hall)

## 收录范围

- 共 **59** 条。分类：官方演示 8、网络安全 6、科学研究 3、软件工程 4、知识工作/评测 2、社区作品 36。
- 一条案例对应一个可区分的项目、演示或公开结果，不把能力 bullet 复述成多条。
- 网络安全条目只写公开结论（发现了什么、如何修复是公开表述），不收录利用步骤、PoC、payload 或复现流程。
- 基准榜（CursorBench、WANDR、AutomationBench、SEC-bench Pro 等）写在下文「基准与生态」，不计入案例条数，以免把排行榜成绩当成项目。
- 结构化数据见 [`cases.json`](cases.json)。

## 目录

- [官方演示与创意工程](#official-demo)（8）
- [网络安全与形式化验证](#cybersecurity)（6）
- [科学研究](#science)（3）
- [软件工程（多为内部实践）](#engineering)（4）
- [知识工作与金融评测](#knowledge-work)（2）
- [社区作品](#community)（36）
- [基准与生态](#benchmarks)
- [如何贡献](#contributing)

<a id="official-demo"></a>

## 官方演示与创意工程

### 1. 埃菲尔铁塔 1887–1889 建造过程交互展览

Google 称，Antigravity 的 /swarm 把一条提示交给一组 Gemini 4 Carbon agent，把历史照片和工程图纸做成交互式 Three.js 三维展览，呈现埃菲尔铁塔 1887–1889 年的建造过程。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：官方上市博文中的独立演示。未提供单独试玩链接。

### 2. 用 7 份规划 PDF 重建 Platform 37 办公楼

官方称，一组 Carbon 多智能体只用 7 份公开的市议会规划 PDF（抽出 206 张工程图）和一条提示，在 /swarm 里经过 10 轮通宵循环，做成约 90.6 万三角面的交互式 Three.js 重建。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：数字（7 份 PDF、206 张图、906K 三角面、10 轮通宵循环）均来自同一篇官方博文。未提供单独试玩链接。

### 3. 针织纺织力学论文的多尺度纤维可视化

官方称 Carbon 在 Antigravity 里根据一篇学术论文做成交互式多尺度纺织可视化：虚拟纤维有限元框架、交互三维纱线网格、110 根纤维的极坐标跟踪，以及动态应力—应变曲线；提示很少。Google 官方账号另发帖说明其依据是 2026 年针织纺织力学研究，并跟踪张力下的 110 根纤维。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：补充来源：https://x.com/Google/status/2120279087314837642 （2026-11-11 06:15 Asia/Shanghai）。

### 4. Pelican Quest：鹈鹕骑 GBike 逛山景城园区

官方用 /swarm 协调子智能体：根据 Omni 与 Nano Banana 参考在 Blender 里建模，再用 Three.js 与 WebGL 着色器做成浏览器开放世界游戏，并配上程序化 Web Audio 音效和 Lyria 配乐。可在 Google AI Studio 试玩。Sundar Pichai 补充说 builder 与 critic 子智能体在 Blender 和 Three.js 之间循环，并检查自己的渲染结果。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Sundar Pichai
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://aistudio.google.com/apps/bundled/pelican-campus-quest 。补充：https://x.com/Google/status/2120260356413051147 、https://x.com/sundarpichai/status/2120198811297694192 。OrcaRouter 拆解文指出试玩页可能需要 Google 登录。

### 5. 两轮提示重做 Google Merchandise Store

官方称 Carbon 在 Antigravity 里凭借更好的前端品味与动效，用两轮提示重想象 Google Merchandise Store：提出五种艺术方向，并用 Nano Banana 2.1 生成全新商品图。官方博文同时给出试玩链接和 Gemini 前端设计 skill。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://aistudio.google.com/apps/bundled/gemini-supply 。商品图由 Nano Banana 2.1 生成，协调与站点构建由 Carbon 完成。

### 6. 从 Omni 视频参考到 Atlantis 水下电影场景

官方称从 Gemini Omni 在 Antigravity 里生成的视频参考出发，流水线先在 Blender 里做程序化遗迹、体积焦散光和水模拟，再把整个环境转到 Three.js，供浏览器实时渲染多镜头电影级水下Atlantis场景。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：视频参考来自 Gemini Omni；场景建模与转到 Three.js 的工作在官方叙述中由 Carbon 完成。未提供单独试玩链接。

### 7. 可演奏的约 1780 年 Stein-Schule 古钢琴与 Koerner Hall

官方称 Carbon 用多智能体循环，依据 CAD 图纸和 X 光片重建可演奏的约 1780 年 Stein-Schule 古钢琴（61 键擒纵机构物理），并放入多伦多皇家音乐学院 Koerner Hall 的三维模型，带座位相关的空间声学。可在 AI Studio 试玩。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://aistudio.google.com/apps/bundled/koerner-hall 。

### 8. 逆向 1994 年 Theme Park 并移植到网页

Demis Hassabis 在 Carbon 开放当天发帖：Carbon 逆向了他参与制作的 1994 年 Theme Park 原版二进制，加入一个 DeepMind 主题游乐设施，并一次性把游戏移植到网页；他形容「看着有点不可思议」。The Verge 引用了同一表述。公告未附公开试玩链接。

- 来源：[https://x.com/demishassabis/status/2120210297948696997](https://x.com/demishassabis/status/2120210297948696997)
- 作者/机构：Demis Hassabis
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖时间为 2026-11-10 17:41 UTC，即 2026-11-11 01:41 Asia/Shanghai。补充报道：https://www.theverge.com/ai-artificial-intelligence/1031117/demis-hassabis-used-ai-to-reverse-engineer-his-own-game-and-port-it-to-the-web 。原作与 Peter Molyneux / Bullfrog 有关，以 Hassabis 自述为准。

<a id="cybersecurity"></a>

## 网络安全与形式化验证

### 9. Project Fortify：扫描与分诊内部评测

官方称 Project Fortify 是覆盖扫描、分诊和修复的自主系统。在 Google 内部评测上，Carbon 扫描召回率为 100%，分诊精确率为 95%。只记录公开指标，不展开利用细节。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：内部基准，数字来自 Google 自述。与下文开源仓库测试是同一节里的另一项结果。

### 10. 开源仓库测试中发现此前未检出的逻辑缺陷

官方称在开源代码仓库测试中，Carbon 相对 Argon 已经很高的召回率又有超过 25% 的相对提升，并检出此前未发现的真实逻辑缺陷。Google 表示会把这些能力用到自身系统与更广泛的开源生态。只记录公开结论。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：「超过 25% 相对提升」是相对 Argon 召回率的官方表述，不是独立复现结果。

### 11. CVR：证明两个开源缺陷可被利用并推动修复

官方称 Google Cloud Vulnerability Research 团队用 Carbon 证明某流行开源软件中的两个缺陷实际上可被利用，严重程度可与近期 PHP2Shell 相比。团队用 Carbon 构建概念验证后，维护者将问题重分类为严重并迅速发布补丁。细节将在负责任披露完成后公布。此处只记录公开结论，不收录利用步骤或 PoC。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google Cloud Vulnerability Research
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：软件名称、CVE 与技术细节官方尚未公开。

### 12. Wiz Scan for Good：两家大型 SaaS 中发现 0-day

官方称 Wiz 在 Scan for Good 中用 Carbon 评估公共数字基础设施。扫描两家大型 SaaS 提供商时，模型在不到两小时内发现 0-day，把通常需要数周的研究压缩到一个下午。Wiz 与受影响机构合作完成修复，官方称这有助于降低对成千上万家公司的潜在影响。只记录公开结论，不收录利用细节。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Wiz（经 Google 转述）
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：截至收录时未找到 Wiz 就这两起 Carbon 发现发布的独立技术博客。更早的 Scan for Good 文章写的是 Gemini 3.8 Flash Cyber / Argon，不能当作本条来源。

### 13. AlphaProof Code：在机器码层验证 Signal 协议实现

DeepMind 介绍 AlphaProof Code：人机协作先把安全目标写成 Lean 规范（官方博文写明 Carbon 与其他模型一起参与；论文写明规范起草使用了 Carbon 和 Claude Opus 5.5），随后由 Carbon 驱动的证明智能体生成约 650 万行经 Lean 内核检查的证明，覆盖 PQXDH 与 Triple Ratchet 的前向保密、认证、失陷后安全和握手保密等，并下到未修改的 libsignal 参考实现编译出的 AArch64 机器码。五名研究者约四周完成，官方称同类工作过去往往需要专家团队数年。为检验规范强度，团队把两个已修复的历史缺陷重新引入隔离构建，并证明有缺陷版本不满足符号安全定理。产物已开源。

- 来源：[https://deepmind.google/blog/introducing-alphaproof-code/](https://deepmind.google/blog/introducing-alphaproof-code/)
- 作者/机构：Google DeepMind（Swarat Chaudhuri、Pushmeet Kohli 等）
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：技术论文：https://deepmind.google/documents/36/Formal_Verification_of_Signal_4.pdf （约 650 万行证明、约 2.6 万行可信规范与 AArch64 语义）。开源站点：https://google-deepmind.github.io/code-verification 。Sundar Pichai 帖：https://x.com/sundarpichai/status/2120207062655549933 。论文也写明结果针对的是其 libsignal-cli 构建，而非 Signal 自家应用；部分分析排除旁路等。不收录任何利用步骤。

### 14. Chrome 团队：高质量补丁生成明显优于另一实验室模型

10 月 28 日宣布博文称，Chrome 团队反馈 Carbon 在生成高质量补丁时的表现，比另一实验室的大型前沿模型好 10 倍以上。只记录这一公开对比结论，没有公开具体漏洞清单或补丁内容。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)
- 作者/机构：Google（转述 Chrome 团队）
- 日期：2026-10-28（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：对照模型未点名。属于团队内部使用反馈，不是公开复现实验。

<a id="science"></a>

## 科学研究

### 15. Axiom Bio：发现此前未找到的毒性机制

官方称对药物毒性研究公司 Axiom Bio 而言，Carbon 目前是转化科学表现领先的模型，发现了他们此前没有找到的新型毒性机制。Axiom 正把生产环境的科学分析与智能体迁移到 Carbon 和 Argon，以支持更安全的药物研发。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Axiom Bio（经 Google 转述）
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：截至收录时未找到 Axiom Bio 就 Carbon 结果发布的独立技术文章。迁移对象同时包括 Carbon 与 Argon。

### 16. 酶分析开发：从实验记录中诊断湿实验伪影

官方称 Google 研究者只提供实验记录本和原始数据，Carbon 不仅做常规分析，还找出难以解释的数据异常，并据此诊断细微湿实验伪影（例如深孔中自动混合不完全），从而提高可重复性。此外还改进了色谱峰解卷积方法，并发现研究仪器中的微量样品残留，加快新分析方法开发。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google 研究者
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：同一研究工作流中的多项发现，按官方段落收录为一条，不拆成多条凑数。

### 17. 为低同源蛋白家族检索远程同源序列

官方称结构预测模型常因标准库中匹配太少而在病毒、微生物和真核等研究不足的蛋白上吃力。研究者用多智能体配置让 Carbon 在拍碱基级未注释序列库、环境与病毒序列目录以及三维结构库中自主发现远程同源。例如在 CASP17 盲测集的 7 个低同源蛋白家族上，Carbon 平均把检索到的同源数量提高约 40 倍，且无需重训结构模型。官方同时说明更广泛的评测仍在进行。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Google 研究者
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：40 倍为官方对这 7 个家族的平均值；文中写明更广泛基准仍在进行。

<a id="engineering"></a>

## 软件工程（多为内部实践）

### 18. Google 内部：用 /swarm 做多包迁移

Antigravity 团队写道，在五周内部试用中，Google 工程师用 swarm 处理棘手的多包迁移。这是官方点名的一类真实内部工程任务，没有公开仓库或迁移清单。

- 来源：[https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- 作者/机构：The Antigravity Team
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：与下文根因调查、架构重设计同出一篇博文的三类不同任务，分开收录。官方也提醒并行多智能体会更快消耗配额。

### 19. Google 内部：跨子系统根因调查

同一篇 Antigravity 博文称，内部工程师在五周试用中用 swarm 做跨子系统的根因调查。没有公开案例编号或代码。

- 来源：[https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- 作者/机构：The Antigravity Team
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：官方概括性描述，不是可复现的外部项目。

### 20. Google 内部：复杂架构重设计

同一篇博文还提到内部 swarm 被用于复杂的架构重设计。Carbon 被定位为协调、架构和审计等高推理角色，更快的模型做并行改文件。

- 来源：[https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/](https://antigravity.google/blog/gemini-4-carbon-in-google-antigravity/)
- 作者/机构：The Antigravity Team
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：官方概括性描述。上市博文也把多包迁移、跨子系统根因和架构重设计列为 Carbon 擅长的多智能体工程任务。

### 21. 内部团队让 Carbon 连续数日做底层排障与补丁

10 月 28 日宣布博文称，内部团队看到 Carbon 能连续运行数日、在死胡同中坚持下去，处理跨大型代码库和底层系统的复杂多步工程任务，例如定位并修补细微缺陷。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)
- 作者/机构：Google / Google DeepMind
- 日期：2026-10-28（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：没有公开具体仓库或缺陷编号，属内部使用观察。

<a id="knowledge-work"></a>

## 知识工作与金融评测

### 22. Hebbia 端到端金融智能体评测中追平最佳模型

官方称在预发布评测中，Carbon 在 Hebbia 的端到端金融智能体评测上达到所测最佳模型的表现。这是面向深度金融研究的外部评测结果，不是公开的客户交付案例。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Hebbia（经 Google 转述）
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：分数与对照模型名单未在该博文中列出。

### 23. 在 Balyasny 通用金融智能基准中位列 23 套配置之首

官方称 Carbon 在 Balyasny Asset Management 的 General Financial Intelligence 基准中，在 23 套前沿模型配置里排在最前；该基准覆盖法律专业能力、智能体工具使用与执行、编码与数据工程，以及感知与上下文理解。

- 来源：[https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)
- 作者/机构：Balyasny Asset Management（经 Google 转述）
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：具体分项分数未在该博文中列出。

<a id="community"></a>

## 社区作品

### 24. 纯 CUDA/C++ 生成 5.2 万株野花草地

GlitterPixely 自称用 Carbon、不靠游戏引擎或三维库，从零用 CUDA 和 C++ 做了一片草地：约 5.2 万片草叶和野花，并在 C++ 里合成风声，使音频跟随同一阵风。Google 官方账号转发并引用了这些细节。

- 来源：[https://x.com/GlitterPixely/status/2120264316092022895](https://x.com/GlitterPixely/status/2120264316092022895)
- 作者/机构：@GlitterPixely
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 21:16 UTC（2026-11-11 05:16 Asia/Shanghai）。Google 转发：https://x.com/Google/status/2120324708826550328 。数字与实现细节为作者自述。

### 25. TIDEFORGE：WebGPU 实时模拟逾百万粒子

kimmonismus 发帖说，为 TIDEFORGE 要求一百万粒子；实际跑起来是 1,048,576 个，运动由 WebGPU compute 计算，切换流场模式会改变同一套实时模拟。他写「这个站点的全部代码来自 Carbon，没有追加提示」。Google 官方账号转发。

- 来源：[https://x.com/kimmonismus/status/2120186202271945137](https://x.com/kimmonismus/status/2120186202271945137)
- 作者/机构：@kimmonismus
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:05 UTC（2026-11-11 00:05 Asia/Shanghai）。Google 转发：https://x.com/Google/status/2120324710307131464 。

### 26. 彩色玻璃 Jenga：可敲击发声也可打碎

AI_Andrew 发布可玩的彩色玻璃 Jenga：点击积木会发声，也可在沙盒里砸碎。他提供了试玩页 vitrail.andrewvoirol.com。Google 转发时概括为：用 Carbon 模拟塔如何在光线中闪光、被敲击时发声，以及倒塌时碎成玻璃片。

- 来源：[https://x.com/AI_Andrew/status/2120243379388760176](https://x.com/AI_Andrew/status/2120243379388760176)
- 作者/机构：@AI_Andrew
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://vitrail.andrewvoirol.com 。原帖 2026-11-10 19:53 UTC。Google 转发：https://x.com/Google/status/2120324716238086357 。

### 27. 从公开数据集做出 14 个带三维可视化的垂直应用

giyu_codes 称获得 Google 早期测试权限，让 Carbon 在公开数据中寻找服务不足的高价值行业，并做成完整垂直平台。目标是测试混乱的多源数据对齐与 3D WebGL 物理。他表示 14 个应用都成功发布为托管应用，并用已有 4 个应用作架构参考。Google 转发了总览。

- 来源：[https://x.com/giyu_codes/status/2120201582319190381](https://x.com/giyu_codes/status/2120201582319190381)
- 作者/机构：@giyu_codes
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：14 个应用按官方转发与作者主题帖收录为一条，不拆成 14 条。原帖 2026-11-10 17:07 UTC。Google 转发：https://x.com/Google/status/2120324719086088676 。

### 28. 从一张参考图做出可交互的 19 世纪巴黎光学实验室

thebuggeddev 称 Carbon 仅凭一张参考图做出交互式 19 世纪风格巴黎物理实验室 Analyse Spectrale (Mod. M1-2-15)，包含 92 个黄铜、铜和硼硅酸盐零件、实时 Beer-Lambert Rankine 涡流、轴向爆炸视图，以及带 60 FPS SVG 瓦特指示器和示意图盘的档案风 Bento 界面。他写 UI 设计也由模型自行完成，没有另给设计参考。Google 转发。

- 来源：[https://x.com/thebuggeddev/status/2120201759305998343](https://x.com/thebuggeddev/status/2120201759305998343)
- 作者/机构：@thebuggeddev
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:07 UTC。Google 转发：https://x.com/Google/status/2120324721816539520 。零件数量与物理效果为作者自述。

### 29. Three.js 生物机械发条心脏

sunset_evm 发帖称 Gemini 4 Carbon 在 Antigravity 的 /swarm 中做了一个 Three.js 生物机械发条心脏，并提醒打开声音观看。

- 来源：[https://x.com/sunset_evm/status/2120308090180714970](https://x.com/sunset_evm/status/2120308090180714970)
- 作者/机构：@sunset_evm
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-11 00:10 UTC（2026-11-11 08:10 Asia/Shanghai）。作者自述，未见独立试玩页。

### 30. FreeCAD + Blender 做成可拆解的双涡轮 V8 引擎

ai_for_success 先在主题帖里展示「1,600 HP Twin-Turbo V8」：可揭开罩盖、拉转、看活塞点火和排气歧管发红，并有实时 V8 声音。次日补充说这是用 Carbon 在 Antigravity 里结合 FreeCAD 与 Blender 完成，整个过程和演示视频大约花了 6–7 小时。

- 来源：[https://x.com/ai_for_success/status/2120317619588972867](https://x.com/ai_for_success/status/2120317619588972867)
- 作者/机构：@ai_for_success
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：细节帖：https://x.com/ai_for_success/status/2120187068634837203 。功率、耗时为作者自述。

### 31. Antigravity 中的 F1 赛车，以及 Unreal/Blender MCP

athrix_codes 称获得 Carbon 早期权限，用 Antigravity、Unreal Engine MCP 和 Blender MCP 做了 F1 赛车游戏，并写这两个 MCP 也是 Carbon 做的。他还对比 Argon，认为 UI/UX、设计品味、代码质量和三维资产等有明显提升。

- 来源：[https://x.com/athrix_codes/status/2120193545344786446](https://x.com/athrix_codes/status/2120193545344786446)
- 作者/机构：@athrix_codes
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:35 UTC。游戏与两个 MCP 由同一作者在同一帖中说明，收录为一条。对比评价为作者观感。

### 32. 把 12 部交响曲做成空间化三维音乐可视化

soumyadesign 称这是他在 Antigravity 里用 Carbon 做的第一批作品之一：用三维空间表示 12 部著名交响曲的乐谱，技术栈是 WebGL、Three.js、Gaussian Splats 和薄膜渐变，每部交响曲都是独立作品。提供了可访问的试玩站。

- 来源：[https://x.com/soumyadesign/status/2120200838899712246](https://x.com/soumyadesign/status/2120200838899712246)
- 作者/机构：@soumyadesign
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://music-visualiser.ai.studio/ （从作者帖中的短链解析得到，收录时 HTTP 200）。原帖 2026-11-10 17:04 UTC。

### 33. 根据历史平面图重建被毁的考文垂大教堂

Leslie Nooteboom 发帖称 Carbon 从零重建被炸毁的考文垂大教堂，扫描历史平面图和照片，生成电影感走查视频。

- 来源：[https://x.com/LeslieNooteboom/status/2120204269173563872](https://x.com/LeslieNooteboom/status/2120204269173563872)
- 作者/机构：@LeslieNooteboom
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:17 UTC。作者自述，影片在原帖中。

### 34. 可交互体素角色工作室 Sailor

cgm_ai 发帖称 Carbon 做了可交互体素女孩：行走循环、鼠标注视、表情、三种法术和实时剖切，以 HTML + WebGL2 在浏览器运行，并给出试玩地址。

- 来源：[https://x.com/cgm_ai/status/2120327608433102929](https://x.com/cgm_ai/status/2120327608433102929)
- 作者/机构：@cgm_ai
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：试玩：https://tdgl.codes/games/sailor-voxel-studio/ 。原帖 2026-11-11 01:27 UTC（2026-11-11 09:27 Asia/Shanghai）。

### 35. 一条提示重做 Atari 2600 的 Pitfall

Glenn Gabe 称作为 Gemini 应用早期测试的一部分使用 Carbon，用一条提示重做了他喜欢的 Atari 2600 游戏 Pitfall，几分钟就完成并且「完全能玩」。

- 来源：[https://x.com/glenngabe/status/2120195911175254316](https://x.com/glenngabe/status/2120195911175254316)
- 作者/机构：@glenngabe（Glenn Gabe）
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:44 UTC。作者自述，未见单独试玩链接。

### 36. 单文件 Three.js 纽约巡游

StatsWire 发帖称 Carbon 用单个 HTML 文件做成交互式三维纽约巡游，基于 Three.js，没有外部三维模型或音频资源；并注明视频灵感来自 @Saboo_Shubham_。

- 来源：[https://x.com/StatsWire/status/2120344850071540152](https://x.com/StatsWire/status/2120344850071540152)
- 作者/机构：@StatsWire
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-11 02:36 UTC（2026-11-11 10:36 Asia/Shanghai）。实现细节为发帖者自述。

### 37. 《近日点》：鹈鹕倒挂穿越日食前的竖环

kayshen_xu 给 Carbon 做鹈鹕测试：让它骑车冲进海上竖直圆环，倒挂着从日食前穿过去，作品名《近日点》。他用 Python SDK 直接调 API 出代码，全程不用 Agent 接口；模型输出被截断后，他补齐交互，把 Three.js 和程序化模型打进可离线打开的 HTML。他还建议在环顶暂停、放大检查两脚是否踩在踏板上。

- 来源：[https://x.com/kayshen_xu/status/2120151206270267864](https://x.com/kayshen_xu/status/2120151206270267864)
- 作者/机构：@kayshen_xu
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 13:46 UTC（2026-11-10 21:46 Asia/Shanghai）。作者明确写了自己补了被截断后的交互。

### 38. Ethan Mollick：把视频片段在 Three.js 里复现

沃顿商学院的 Ethan Mollick 称获得 Carbon 早期权限，认为它比 Argon 更好，并展示一个有趣演示：把一段视频交给 Carbon，由它在 Three.js 中复现。

- 来源：[https://x.com/emollick/status/2120198832202125322](https://x.com/emollick/status/2120198832202125322)
- 作者/机构：@emollick（Ethan Mollick）
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:56 UTC。评价为作者观感；演示本身有原帖视频。

### 39. Simon Willison：低/中/高思考档的鹈鹕骑车测试

Simon Willison 在 llm-gemini 0.36 发布说明中，用 Carbon 的 low、medium、high 三档思考强度跑了自己长期使用的「鹈鹕骑自行车」测试，并公布了 high 档结果图。他指出近来 Gemini 的鹈鹕已经一直不错。

- 来源：[https://simonwillison.net/2026/Nov/10/llm-gemini/](https://simonwillison.net/2026/Nov/10/llm-gemini/)
- 作者/机构：Simon Willison
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：文章时间 2026-11-10 20:09（页面未标时区；按文中发布日收录）。这是独立复现，不是 Google 的 Pelican Quest 游戏。

### 40. Yonkers 机甲在纽约三区踩街（OpenStreetMap）

同一篇文章里，Willison 在 Google Antigravity 中使用他前一天对 Claude Fable 5.2 用过的提示：做一个 Three.js 动画，让 Yonkers 像大型机甲一样站起，并在曼哈顿、皇后区和布鲁克林踩街，使用 OpenStreetMap 数据。他得到 HTML 结果，又提示「打成无外部依赖的独立 HTML」，并录了屏。

- 来源：[https://simonwillison.net/2026/Nov/10/llm-gemini/](https://simonwillison.net/2026/Nov/10/llm-gemini/)
- 作者/机构：Simon Willison
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：与鹈鹕 SVG 测试是同一篇文章中的另一项独立实验。

### 41. 用 Carbon 指挥 DeepSeek harness 设计工作流

一位中文用户发帖称本周只剩 3% token，于是用 Carbon 指挥 DeepSeek harness（Deepseek v41 flash）干活，并说 Carbon 很好地设计了一个工作流，让 DeepSeek 高速执行。

- 来源：[https://x.com/StateInterOffic/status/2120237344309841998](https://x.com/StateInterOffic/status/2120237344309841998)
- 作者/机构：@StateInterOffic
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 19:29 UTC。作者自述的工作流搭配，没有公开仓库。

### 42. 单 HTML 文件里 1128 万体素的高架列车与飞艇场景

@Adidotdev 发帖展示一个独立 HTML 文件：约 11,286,682 个体素、60fps，含移动的高架列车、空中飞艇和 3 种实时光照模式。作者写明这是 Gemini 4 Carbon 的作品，并称当时它曾以 “gemini-4-argon” 做影子路由。

- 来源：[https://x.com/Adidotdev/status/2120158160074002823](https://x.com/Adidotdev/status/2120158160074002823)
- 作者/机构：@Adidotdev
- 日期：2026-11-10（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 14:14 UTC（2026-11-10 22:14 Asia/Shanghai）。体素数与 60fps 为作者自述。作者在公开后将早期权限阶段的模型认定为 Carbon；本条按作者现署名收录，不另把第三方 Argon/Arena 目录里的同款视频算作独立案例。

### 43. 一枪做成的 Three.js 奔驰斑马

@AI_Screening 发帖称这是 Gemini 4 Carbon 的输出，并说 Carbon 又快又便宜，一枪做成这只 Three.js 奔驰斑马。

- 来源：[https://x.com/AI_Screening/status/2120185448727462301](https://x.com/AI_Screening/status/2120185448727462301)
- 作者/机构：@AI_Screening
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:02 UTC（2026-11-11 00:02 Asia/Shanghai）。「一枪做成」为作者自述。

### 44. 纯代码生成的整支音乐视频

@kickingkeys 称用 Gemini 4 Carbon、只靠代码做了一整支音乐视频，并说已有约两周早期权限。帖中表示下面还有更多例子和代码。

- 来源：[https://x.com/kickingkeys/status/2120185497637024013](https://x.com/kickingkeys/status/2120185497637024013)
- 作者/机构：@kickingkeys
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:03 UTC（2026-11-11 00:03 Asia/Shanghai）。本条只收录该帖所展示的这一支音乐视频，不把「更多例子」拆成未经核验的多条。

### 45. Pooperman：Flappy Bird 风格的 Three.js 平台游戏

@SimonasLTU1 把提示「做一个叫 pooperman 的游戏，本质是 Flappy Bird，点击时角色会排便，要 Three.js 图形，但偏平台游戏风格」交给 Gemini 4 Carbon，称花了 14 分钟做成。

- 来源：[https://x.com/SimonasLTU1/status/2120186826451288182](https://x.com/SimonasLTU1/status/2120186826451288182)
- 作者/机构：@SimonasLTU1
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:08 UTC（2026-11-11 00:08 Asia/Shanghai）。游戏名与规则来自作者公开的提示原文。耗时为作者自述。

### 46. 不用现成素材做出的三维篮球场

@LexnLin 称拥有 Gemini 4 Carbon 早期权限，用它做了这座三维篮球场，并写明没有使用现成的三维素材。作者还认为 Carbon 在三维、网站和动态图形等需要审美判断的方面比 Argon 有进步。

- 来源：[https://x.com/LexnLin/status/2120186998707163533](https://x.com/LexnLin/status/2120186998707163533)
- 作者/机构：@LexnLin
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:09 UTC（2026-11-11 00:09 Asia/Shanghai）。对比 Argon 的观感是作者个人评价。

### 47. Adiyogi Divya Darshanam 三维演示

@ai_for_success 称拥有早期权限，一直用 Carbon 做编程和三维，并展示其做出的作品中的第一个：Adiyogi Divya Darshanam。

- 来源：[https://x.com/ai_for_success/status/2120187064184664162](https://x.com/ai_for_success/status/2120187064184664162)
- 作者/机构：@ai_for_success
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:09 UTC（2026-11-11 00:09 Asia/Shanghai）。与已收录的双涡轮 V8 引擎是同一作者的另一件作品。本条只收录帖中点名并展示的第一件 Adiyogi 演示，不把未单独给出来源的其余作品自动拆条。

### 48. 单 HTML 文件、纯代码生成的动画

@itsPaulAi 发帖称 Google 已发布 Gemini 4 Carbon，并展示下方视频：该模型用纯代码、在单个 HTML 文件里产出这段动画。作者称已使用数日。

- 来源：[https://x.com/itsPaulAi/status/2120188198592663935](https://x.com/itsPaulAi/status/2120188198592663935)
- 作者/机构：@itsPaulAi
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:13 UTC（2026-11-11 00:13 Asia/Shanghai）。原帖有视频；未写出动画的具体主题名称，故标题按作者自己的描述收录。

### 49. 自写 CUDA C++ 特效引擎做出的三维场景

@fofrAI 在 Carbon 上市当日发帖称它很强，并展示 Carbon 为他写的自定义 CUDA C++ 特效引擎所生成的三维场景。

- 来源：[https://x.com/fofrAI/status/2120188535152222407](https://x.com/fofrAI/status/2120188535152222407)
- 作者/机构：@fofrAI
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:15 UTC（2026-11-11 00:15 Asia/Shanghai）。与已收录的 GlitterPixely CUDA 草地是不同作者、不同作品。

### 50. 一颗星星、一镜到底表演动画 15 原则

@CodeByPoonam 发帖称由 Gemini 4 Carbon 做成：一颗星星在一个连续镜头、零剪辑中表演 15 条动画原则。

- 来源：[https://x.com/CodeByPoonam/status/2120192694622580794](https://x.com/CodeByPoonam/status/2120192694622580794)
- 作者/机构：@CodeByPoonam
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:31 UTC（2026-11-11 00:31 Asia/Shanghai）。「零剪辑」「15 原则」为作者自述。

### 51. 纯程序化 Three.js 的 56 件大天象仪自动机械

@StatsWire 发帖称 Gemini Carbon 4 从零用纯程序化 Three.js、不靠外部三维模型，做成一套 56 件的 Grand Celestial Planétarium Automaton。

- 来源：[https://x.com/StatsWire/status/2120199271588737356](https://x.com/StatsWire/status/2120199271588737356)
- 作者/机构：@StatsWire
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 16:57 UTC（2026-11-11 00:57 Asia/Shanghai）。与已收录的纽约巡游是同一作者的另一件作品。件数与「无外部模型」为作者自述。作者把模型写作 Gemini Carbon 4，结合上下文按 Gemini 4 Carbon 收录。

### 52. 从一张参考图做成纯代码动画

@devteamdrew 发帖称整段场景都是纯代码，把一张参考图做成动画，没有使用技能包或框架，是纯 JS + Python，由 Google DeepMind 的 Gemini 4 Carbon 制作。

- 来源：[https://x.com/devteamdrew/status/2120200837305884813](https://x.com/devteamdrew/status/2120200837305884813)
- 作者/机构：@devteamdrew
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:04 UTC（2026-11-11 01:04 Asia/Shanghai）。「无框架」「纯 JS + Python」为作者自述。

### 53. 纯代码制作的 32 秒珊瑚礁短片

@Adidotdev 称用 Gemini 4 Carbon、纯代码做了一部约 32 秒、偏皮克斯风格的短片：约 4,800 片珊瑚从白化中苏醒、约 3,600 条群游的鱼、斯涅尔窗水光学和完整破水镜头，用 Three.js 与 GLSL 实现，管弦乐也在代码里合成。

- 来源：[https://x.com/Adidotdev/status/2120208990089175300](https://x.com/Adidotdev/status/2120208990089175300)
- 作者/机构：@Adidotdev
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:36 UTC（2026-11-11 01:36 Asia/Shanghai）。与高架列车体素场景为同一作者的另一件作品。时长与数量为作者自述。

### 54. 单文件 Three.js 可玩的 V12 超跑海岸赛

@StatsWire 发帖称 Gemini 4 Carbon 用单个 HTML 文件和 Three.js 做成可玩的三维 V12 超跑海岸赛，并描述了 9,250 RPM 的 V12 声浪、双离合换挡、海边隧道混响、飘移和约 340 km/h 高架超车，称 60fps。

- 来源：[https://x.com/StatsWire/status/2120212182482682232](https://x.com/StatsWire/status/2120212182482682232)
- 作者/机构：@StatsWire
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:49 UTC（2026-11-11 01:49 Asia/Shanghai）。性能与声音细节为作者自述。

### 55. Desk Racer：浏览器里的迷你卡丁车赛

@anuragdotdev 发帖称 Gemini 4 Carbon 做出了 Desk Racer，一款完全在浏览器里运行的迷你卡丁车游戏，并列举：4 种游戏模式、用 Rapier3D 的三维物理等。

- 来源：[https://x.com/anuragdotdev/status/2120213817573740687](https://x.com/anuragdotdev/status/2120213817573740687)
- 作者/机构：@anuragdotdev
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 17:55 UTC（2026-11-11 01:55 Asia/Shanghai）。模式数量与物理引擎为作者自述；原帖在列举处被截断，本条不补充未见的条目。

### 56. Carbon 拆任务、本地模型执行的小黄人场景

@atomicagent_io 称在 Atomic Agent Fusion 里让 Gemini 4 Carbon 把提示拆成任务，交给本地 Qwen 3.8 27B 执行。作者给出小黄人场景的耗时和花费：这套编排约 5 分钟、2.39 美元，单用 Gemini 约 16 分钟、7.71 美元，并称 Carbon 更便宜、更快。

- 来源：[https://x.com/atomicagent_io/status/2120227531504918833](https://x.com/atomicagent_io/status/2120227531504918833)
- 作者/机构：@atomicagent_io
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 18:50 UTC（2026-11-11 02:50 Asia/Shanghai）。这是 Carbon 做任务拆分、本地模型参与生成的混合流程，不是 Carbon 单独完成全部画面。耗时与费用为作者自述。产品推广链接不作为收录依据。

### 57. 从零写的 WebGL2 与光线追踪着色器游戏

@ia_met 称在 Antigravity 里使用 Gemini 4 Carbon，一枪做成这个项目，花了正好 70 分钟（约 8 美元 API 费用），从零写了约 6,800 行自定义 WebGL2 与光线追踪着色器、没有外部素材，并对其截图做了视觉调试。

- 来源：[https://x.com/ia_met/status/2120228626608050335](https://x.com/ia_met/status/2120228626608050335)
- 作者/机构：@ia_met
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 18:54 UTC（2026-11-11 02:54 Asia/Shanghai）。行数、耗时、费用和「一枪」为作者自述。原帖未给出可公开试玩的独立网址。

### 58. 两只螃蟹靠近骑车鹈鹕的 SVG 动画

@HarshithLucky3 称在 Google AI Studio 使用 Gemini 4 Carbon medium，生成「两只好斗的螃蟹靠近骑着自行车的鹈鹕」的 SVG。

- 来源：[https://x.com/HarshithLucky3/status/2120236571165368720](https://x.com/HarshithLucky3/status/2120236571165368720)
- 作者/机构：@HarshithLucky3
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 19:26 UTC（2026-11-11 03:26 Asia/Shanghai）。这是作者自己生成的 SVG，不是 Google 官方的 Pelican Quest 游戏。

### 59. 把旧 Canvas 艺术作品打磨到接近 teamLab 风格

@Majin_AppSheet 用日文发帖称，请 Gemini 4 Carbon 打磨自己以前做的 Canvas 艺术作品，完成后觉得已经接近 teamLab 的感觉，并因此想再看《夏へのトンネル、さよならの出口》。

- 来源：[https://x.com/Majin_AppSheet/status/2120245677439783195](https://x.com/Majin_AppSheet/status/2120245677439783195)
- 作者/机构：@Majin_AppSheet
- 日期：2026-11-11（能确定时区的已换算到 Asia/Shanghai 的日历日；官方博文按页面标注日）
- 收录说明：原帖 2026-11-10 20:02 UTC（2026-11-11 04:02 Asia/Shanghai）。teamLab 是作者的观感比喻，不是该机构参与或背书。

<a id="benchmarks"></a>

## 基准与生态

以下是官方或厂商公布的能力与接入信息，便于对照，**不计入上方案例条数**。

- 官方称 Carbon 在 CursorBench 4.0、Perplexity WANDR、Zapier AutomationBench 上排名第一，且每任务成本不到下一外部模型的一半（[上市博文](https://blog.google/innovation-and-ai/models-and-research/gemini-models/gemini-4-carbon-now-available/)）。
- Cursor 官方账号称 Carbon 已在 Cursor 中可用，高努力档在 CursorBench 上为 60.4%、当时榜首（[帖](https://x.com/cursor_ai/status/2120193584670580857)，2026-11-11 00:35 Asia/Shanghai）。Demis Hassabis 转发了该帖。
- 宣布时官方称 Artificial Analysis Intelligence Index v5.0 为 59、当时第 1；并给出 SEC-bench Pro 88.2%、ExploitGym 54.8%、CWE-bench 71.0% 等网络安全基准（[宣布博文](https://blog.google/innovation-and-ai/models-and-research/gemini-models/introducing-gemini-4-carbon/)）。部分网络基准被标明通过 Fairwind 访问。分数会随榜单版本变动，请以原页为准。
- 官方与 Artificial Analysis 合作推出 Multimodal Knowledge Agent（MKA）基准，称 Carbon 排第 2，平均每任务成本不到第一名的 1/6。
- WebDev Arena：宣布博文称 Carbon 比 Argon 高 89 Elo，当时第 4（1768）。
- Simon Willison 发布 [llm-gemini 0.36](https://simonwillison.net/2026/Nov/10/llm-gemini/)，为 `llm` CLI 增加 `gemini-4-carbon`。
- 安全评测方面，官方安全报告与上市博文还提到 Gray Swan、Trajectory Labs 等外部测试；这是安全评估，不是产品使用案例。

<a id="contributing"></a>

## 如何贡献

欢迎补充可核验的公开案例，请先阅读 [CONTRIBUTING.md](CONTRIBUTING.md)。提交时请同时更新 `README.md`、`README.en.md` 和 `cases.json`。

## 许可与声明

清单文字以 [MIT License](LICENSE) 发布。第三方作品、商标和媒体仍归原权利人。详见 [NOTICE.md](NOTICE.md)。

