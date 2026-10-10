# Awesome Humanizer Skills

[English](README.md)

开源的 **去 AI 味 / humanizer skill**:让 AI 写的文字、代码和界面读起来像人做的,检测 AI 腔,让 agent 守住写作风格。中英文都有。共 230 个仓库,每个都由 [Agent Skills Hub](https://agentskillshub.top?utm_source=github&utm_medium=awesome-list) 读过 README 并做了安全评级。

带类型筛选的在线页面:**[https://agentskillshub.top/best/anti-slop/](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list)** · 每 8 小时刷新

## 到底装哪个

我们实跑了其中 26 个(23 个出了结果),结论如下。[完整实测结果](#tested)在下面。

- 🥇 **英文文本: [sloptrim](https://github.com/seyedehsanhadi/sloptrim)**  
  实测里读起来最像人写的改写（4.5/5），事实全保留。和其他工具一样，它改的是措辞，不是结构。
- 🥈 **中文文本: [Humanizer-zh](https://github.com/op7418/Humanizer-zh)**  
  3.0/5，事实全保留，和另外三个中文工具并列；其中用的人最多。中文类没有得分更高的。
- 🥉 **只检查不改写: [humanizer-skill](https://github.com/Aboudjem/humanizer-skill)**  
  唯一认真查结构的检测器：报出的 38 处里有 8 处是讲明的道理、整齐的结尾这类结构问题。

**别用:** AI-Text-Humanizer-App (在句首硬加连接词，越改越像 AI（1/5）).

没有一个工具改掉结构上的 AI 味：40 份改写里，讲明的道理 26/26 留着，整齐的结尾 28/28 留着。删道理、留结尾、把泛指换成具体名字，得自己动手。

*排名规则：改写类按改写稿读起来像人写的程度（1–5 分）排；检测类按报出多少结构问题排。*

## 这些 skill 能做什么

<table>
<tr>
<td align="center" valign="top" width="33%"><b>✍️ 文字去 AI 味</b><br><sub>58 个仓库</sub><br><br><a href="https://github.com/ilyautov/humanizer-it"><img src="assets/previews/ilyautov__humanizer-it.jpg" width="260" alt="ilyautov/humanizer-it"></a><br><sub>把 AI 写的文章、帖子、邮件改得像人写的。</sub><br><a href="#type-writing"><b>查看列表 →</b></a></td>
<td align="center" valign="top" width="33%"><b>🔍 AI 味检测</b><br><sub>80 个仓库</sub><br><br><sub>找出并给 AI 写作痕迹打分。</sub><br><a href="#type-detector"><b>查看列表 →</b></a></td>
<td align="center" valign="top" width="33%"><b>🀄 中文去 AI 味</b><br><sub>36 个仓库</sub><br><br><sub>专门给中文去 AI 味。</sub><br><a href="#type-chinese"><b>查看列表 →</b></a></td>
</tr>
<tr>
<td align="center" valign="top" width="33%"><b>🧹 代码去 AI 味</b><br><sub>5 个仓库</sub><br><br><sub>清理代码和注释里的 AI 痕迹。</sub><br><a href="#type-code"><b>查看列表 →</b></a></td>
<td align="center" valign="top" width="33%"><b>🎨 设计去 AI 味</b><br><sub>31 个仓库</sub><br><br><a href="https://github.com/changemaner/design-taste-frontend"><img src="assets/previews/changemaner__design-taste-frontend.jpg" width="260" alt="changemaner/design-taste-frontend"></a><br><sub>让 AI 做的界面摆脱千篇一律的 AI 感。</sub><br><a href="#type-design"><b>查看列表 →</b></a></td>
<td align="center" valign="top" width="33%"><b>📏 写作规则</b><br><sub>20 个仓库</sub><br><br><sub>agent 遵守的写作规范和禁用词表。</sub><br><a href="#type-rules"><b>查看列表 →</b></a></td>
</tr>
</table>

## 目录

- [🧪 端到端实测](#tested)
- [✍️ 文字去 AI 味](#type-writing) (58)
- [🔍 AI 味检测](#type-detector) (80)
- [🀄 中文去 AI 味](#type-chinese) (36)
- [🧹 代码去 AI 味](#type-code) (5)
- [🎨 设计去 AI 味](#type-design) (31)
- [📏 写作规则](#type-rules) (20)

## 什么样的仓库能上榜

1. 它让 AI 的产出读起来像人做的,或者检测、去除文字、代码、设计里的 AI 痕迹。通用写作助手、语法检查器不算。
2. 它是能安装或运行的软件,不是链接合集或空仓库。
3. 它有 README。没有 README 就没法评级。
4. 50 星及以上只看是否切题;50 星以下还要过 README 质量线(展示效果、一条命令上手、说清产出、文档完整),并且至少 5 星。

这些问题由决策模型逐个读 README 回答,不是人工挑选。卡在线上的仓库可能判到任一边,归错了请提 issue。

<a id="tested"></a>
## 🧪 端到端实测

2026-10-07 我们实跑了其中 26 个,跑成 23 个:每个在用完即删的沙箱里改写同样的三份文本(英文文章、中文文章、短篇小说),由 Claude Code (Claude Opus 5.5) 调用,gpt-6-astra 按 StoryScope 的结构特征评审([COLM 2026](https://arxiv.org/abs/2604.03136))。按像人写的程度排序。

**发现:** 没有一个把结构上的 AI 味改掉。40 份改写里,讲明的道理 26/26 留着,整齐的结尾 28/28 留着,单线论证 40/40 没动;21 个改写类里 19 个只改了措辞。没有一份改丢事实。

| # | Skill | ★ | 像人写 | 改到哪层 | 去掉的 AI 结构 | 事实 | 检测报出 | |
|---|---|---|---|---|---|---|---|---|
| 1 | [sloptrim](https://github.com/seyedehsanhadi/sloptrim) | 212 | 4.5/5 | 措辞 | 0 | 全保留 | 6 (0) | [证据](https://agentskillshub.top/best-runs/slop/seyedehsanhadi__sloptrim.html) |
| 2 | [slop-guard](https://github.com/eric-tramel/slop-guard) | 163 | 4.0/5 | 措辞 | 0 | 全保留 | 5 (2) | [证据](https://agentskillshub.top/best-runs/slop/eric-tramel__slop-guard.html) |
| 3 | [anti-slop](https://github.com/miqdadbadjuber/anti-slop) | 4,501 | 4.0/5 | 措辞 | 1 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/miqdadbadjuber__anti-slop.html) |
| 4 | [humanizer-stack](https://github.com/NulightJens/humanizer-stack) | 318 | 3.5/5 | 结构 | 1 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/NulightJens__humanizer-stack.html) |
| 5 | [academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer) | 1,781 | 3.5/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/AIScientists-Dev__academic-humanizer.html) |
| 6 | [no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules) | 694 | 3.5/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/realrossmanngroup__no_ai_slop_writing_rules.html) |
| 7 | [humanizer-skill](https://github.com/Aboudjem/humanizer-skill) | 264 | 3.3/5 | 措辞 | 1 | 全保留 | 38 (8) | [证据](https://agentskillshub.top/best-runs/slop/Aboudjem__humanizer-skill.html) |
| 8 | [humanizer](https://github.com/blader/humanizer) | 54,072 | 3.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/blader__humanizer.html) |
| 9 | [sepia](https://github.com/Nanako0129/sepia) | 2,970 | 3.0/5 | 结构 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/Nanako0129__sepia.html) |
| 10 | [humanize](https://github.com/harshaneel/humanize) | 515 | 3.0/5 | 措辞 | 1 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/harshaneel__humanize.html) |
| 11 | [unslop](https://github.com/MohamedAbdallah-14/unslop) | 153 | 3.0/5 | 措辞 | 1 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/MohamedAbdallah-14__unslop.html) |
| 12 | [Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 18,940 | 3.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/op7418__Humanizer-zh.html) |
| 13 | [speak-human-tw](https://github.com/Raymondhou0917/speak-human-tw) | 1,027 | 3.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/Raymondhou0917__speak-human-tw.html) |
| 14 | [De-AI-Prompt-Enhancer-Writer-Booster-SKILL](https://github.com/OUBIGFA/De-AI-Prompt-Enhancer-Writer-Booster-SKILL) | 848 | 3.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/OUBIGFA__De-AI-Prompt-Enhancer-Writer-Booster-SKILL.html) |
| 15 | [qu-ai-wei](https://github.com/LifelongLazyLearner/qu-ai-wei) | 622 | 3.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/LifelongLazyLearner__qu-ai-wei.html) |
| 16 | [stop-slop](https://github.com/hardikpandya/stop-slop) | 17,755 | 3.0/5 | 措辞 | 1 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/hardikpandya__stop-slop.html) |
| 17 | [StealthHumanizer](https://github.com/rudra496/StealthHumanizer) | 156 | 2.3/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/rudra496__StealthHumanizer.html) |
| 18 | [patina](https://github.com/devswha/patina) | 363 | 2.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/devswha__patina.html) |
| 19 | [lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone) | 2,303 | 2.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/larashero3-dotcom__lieflat-less-ai-tone.html) |
| 20 | [shuorenhua](https://github.com/MrGeDiao/shuorenhua) | 1,980 | 2.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/MrGeDiao__shuorenhua.html) |
| 21 | [AI-Text-Humanizer-App](https://github.com/DadaNanjesha/AI-Text-Humanizer-App) | 435 | 1.0/5 | 措辞 | 0 | 全保留 | - | [证据](https://agentskillshub.top/best-runs/slop/DadaNanjesha__AI-Text-Humanizer-App.html) |
| 22 | [vale-ai-tells](https://github.com/tbhb/vale-ai-tells) | 115 | - | 只检测 | - | - | 22 (2) | [证据](https://agentskillshub.top/best-runs/slop/tbhb__vale-ai-tells.html) |
| 23 | [avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | 4,864 | - | 只检测 | - | - | 7 (0) | [证据](https://agentskillshub.top/best-runs/slop/conorbronsdon__avoid-ai-writing.html) |

**未能实测:** humanize-text (除 LLM key 外还要 Niutrans 翻译 key，且只输出英文。); AIWriteX (桌面应用，从热点生成新文章发公众号，不能改写给定的文件。); attention-span (改的是 Claude 自己的回话方式，而且只能由人手动敲命令启动。)

[全部结果、提示词和脚本](https://github.com/zhuyansen/agent-skills-hub/blob/main/ops/slop-runs/RESULTS.md) · [https://agentskillshub.top/best/anti-slop/#test-results](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#test-results)

<a id="type-writing"></a>
## ✍️ 文字去 AI 味

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-writing)

<table><tr>
<td align="center" valign="top"><a href="https://github.com/sgaofen/humanizer-local-model"><img src="assets/previews/sgaofen__humanizer-local-model.jpg" width="260" alt="sgaofen/humanizer-local-model"></a><br><sub><a href="https://github.com/sgaofen/humanizer-local-model">sgaofen/humanizer-local-model</a></sub></td>
</tr></table>

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [blader/humanizer](https://github.com/blader/humanizer) | 55.1k | 消除文本中 AI 生成痕迹的 agent skill | [SAFE](https://agentskillshub.top/skill/blader/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [lynote-ai/humanize-text](https://github.com/lynote-ai/humanize-text) | 3.2k | 开源文本人性化流水线，公开每个中间步骤。先以1.3温度进行两次LLM改写，再通过不同NMT引擎完成两次转换。提供四种可阅读、修改并本地运行的方法。 | [SAFE](https://agentskillshub.top/skill/lynote-ai/humanize-text/?utm_source=github&utm_medium=awesome-list) |
| [Nanako0129/sepia](https://github.com/Nanako0129/sepia) | 3.1k | De-AI 写作 skill：Agent Skills 兼容 agent，修复小说叙事架构，匹配专业文体规则，基于 StoryScope。 | [SAFE](https://agentskillshub.top/skill/Nanako0129/sepia/?utm_source=github&utm_medium=awesome-list) |
| [iniwap/AIWriteX](https://github.com/iniwap/AIWriteX) | 2.1k | AIWriteX：微信公众号AI工具，支持热搜舆情聚合、趋势分析、选题、文章采集、生成排版发布、配图及多平台发布；支持多账号、短视频文案、手机控制和小说连载 | [SAFE](https://agentskillshub.top/skill/iniwap/AIWriteX/?utm_source=github&utm_medium=awesome-list) |
| [harshaneel/humanize](https://github.com/harshaneel/humanize) | 523 | 静态AI文本人性化工具：两项有研究依据且不依赖特定LLM的skill，使AI写作更自然易懂。含9个调节项、50+篇同行评审文献及2024—2026年检测研究。 | [SAFE](https://agentskillshub.top/skill/harshaneel/humanize/?utm_source=github&utm_medium=awesome-list) |
| [DadaNanjesha/AI-Text-Humanizer-App](https://github.com/DadaNanjesha/AI-Text-Humanizer-App) | 434 | 将 AI 生成文本转换为正式、自然且学术化的写作，规避 AI 检测。 | [SAFE](https://agentskillshub.top/skill/DadaNanjesha/AI-Text-Humanizer-App/?utm_source=github&utm_medium=awesome-list) |
| [devswha/patina](https://github.com/devswha/patina) | 366 | 支持韩/英/中/日文的 AI 写作去机器感工具 | [SAFE](https://agentskillshub.top/skill/devswha/patina/?utm_source=github&utm_medium=awesome-list) |
| [NulightJens/humanizer-stack](https://github.com/NulightJens/humanizer-stack) | 346 | 基于 StoryScope 研究的双遍流程：表层与结构处理，去除对外文本的 AI 写作痕迹，封装为 Claude Code Skills | [SAFE](https://agentskillshub.top/skill/NulightJens/humanizer-stack/?utm_source=github&utm_medium=awesome-list) |
| [rudra496/StealthHumanizer](https://github.com/rudra496/StealthHumanizer) | 161 | 开源 AI 文本改写工具，支持16+语言、35个提供商、4级改写、6种风格、9种用途、13种语气和多轮 ninja mode；无需登录，面向学生和写作者。 | [SAFE](https://agentskillshub.top/skill/rudra496/StealthHumanizer/?utm_source=github&utm_medium=awesome-list) |
| [MohamedAbdallah-14/unslop](https://github.com/MohamedAbdallah-14/unslop) | 155 | AI输出拟人，去AI腔，保代码/URL/标题；Claude Code、Cursor、Windsurf、Codex、Cline、Copilot、Gemini插件 | [SAFE](https://agentskillshub.top/skill/MohamedAbdallah-14/unslop/?utm_source=github&utm_medium=awesome-list) |
| [sergebulaev/x-skills](https://github.com/sergebulaev/x-skills) | 124 | Claude Code/Codex的X skill：写推文、串文、回复，去AI痕迹并经Publora发布；开源MIT；Creative Content Cra… | [SAFE](https://agentskillshub.top/skill/sergebulaev/x-skills/?utm_source=github&utm_medium=awesome-list) |
| [ehmo/slopkit](https://github.com/ehmo/slopkit) | 106 | AI agent 的反低质内容 skills：slopbeth 清理已发布文案，slopgent 清理对话。 | [SAFE](https://agentskillshub.top/skill/ehmo/slopkit/?utm_source=github&utm_medium=awesome-list) |
| [carlosafjr-dev/humanizer-br](https://github.com/carlosafjr-dev/humanizer-br) | 95 | 用于 Claude Code 的 skill，分析并重写文本，去除 AI 生成痕迹，使表达更自然、清晰、流畅。 | [SAFE](https://agentskillshub.top/skill/carlosafjr-dev/humanizer-br/?utm_source=github&utm_medium=awesome-list) |
| [sgaofen/humanizer-local-model](https://github.com/sgaofen/humanizer-local-model) | 94 | 本地模型，让 AI 文本更像人类并绕过 AI 检测器 | [SAFE](https://agentskillshub.top/skill/sgaofen/humanizer-local-model/?utm_source=github&utm_medium=awesome-list) |
| [ksanyok/TextHumanize](https://github.com/ksanyok/TextHumanize) | 85 | 将 AI 生成的文本转换为自然的人类风格内容；支持离线运行、25种语言和零依赖；PHANTOM™、ASH™；Python/PHP/TypeScript | [SAFE](https://agentskillshub.top/skill/ksanyok/TextHumanize/?utm_source=github&utm_medium=awesome-list) |
| [bushrabeg/turkce-humanizer](https://github.com/bushrabeg/turkce-humanizer) | 84 | 去除土耳其语文本中 AI 写作痕迹的 Claude skill，使其更自然。 | [SAFE](https://agentskillshub.top/skill/bushrabeg/turkce-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [Wenzhi-Ding/wenzhi-plugins](https://github.com/Wenzhi-Ding/wenzhi-plugins) | 75 | coding agent 行为插件：humanize 注入「说人话」规则，skill-stats 统计技能触发和来源。 | [SAFE](https://agentskillshub.top/skill/Wenzhi-Ding/wenzhi-plugins/?utm_source=github&utm_medium=awesome-list) |
| [asavvin-pixel/unslop](https://github.com/asavvin-pixel/unslop) | 74 | Claude 英文文本润色工具：调整排版、词汇和结构，适配你的文风。基于 UMD、Google DeepMind 研究及维基百科《Signs of AI wr… | [SAFE](https://agentskillshub.top/skill/asavvin-pixel/unslop/?utm_source=github&utm_medium=awesome-list) |
| [sanjaysah101/humanize-ai](https://github.com/sanjaysah101/humanize-ai) | 64 | 利用自然语言处理技术和数学模型，将 AI 生成文本转换为自然内容的系统。 | [SAFE](https://agentskillshub.top/skill/sanjaysah101/humanize-ai/?utm_source=github&utm_medium=awesome-list) |
| [zhouying20/HMGC](https://github.com/zhouying20/HMGC) | 60 | COLING'24 使机器生成内容更像人类：通过对抗攻击规避 AI 文本检测 | [SAFE](https://agentskillshub.top/skill/zhouying20/HMGC/?utm_source=github&utm_medium=awesome-list) |
| [lguz/humanize-writing-skill](https://github.com/lguz/humanize-writing-skill) | 54 | 将 AI 文本改得更像人写。三轮编辑：36+ 个禁用词、10 种结构模式、质量清单。支持 Claude、ChatGPT、Gemini、Cursor、Winds… | [SAFE](https://agentskillshub.top/skill/lguz/humanize-writing-skill/?utm_source=github&utm_medium=awesome-list) |
| [chengez/Adversarial-Paraphrasing](https://github.com/chengez/Adversarial-Paraphrasing) | 52 | [NeurIPS 2025]《对抗性改写：使 AI 生成文本人性化的通用攻击》实现 | [SAFE](https://agentskillshub.top/skill/chengez/Adversarial-Paraphrasing/?utm_source=github&utm_medium=awesome-list) |
| [ZAYUVALYA/AI-Text-Humanizer](https://github.com/ZAYUVALYA/AI-Text-Humanizer) | 51 | ZAYUVALYA - AI Humanizer 用于改写 AI 生成文本，使其更自然并降低被 AI 内容检测器识别的概率，专注于上下文感知改写。 | [SAFE](https://agentskillshub.top/skill/ZAYUVALYA/AI-Text-Humanizer/?utm_source=github&utm_medium=awesome-list) |
| [thevseprod/humanizer-ru](https://github.com/thevseprod/humanizer-ru) | 42 | 让 AI 文本更像人类：规则 + Claude Code skill，适用于俄语和英语。 | [SAFE](https://agentskillshub.top/skill/thevseprod/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [glaforge/deslopify](https://github.com/glaforge/deslopify) | 37 | 让文本更真实、自然，避免 AI 套话的 Gemini CLI skill | [SAFE](https://agentskillshub.top/skill/glaforge/deslopify/?utm_source=github&utm_medium=awesome-list) |
| [CBIhalsen/text-rewriter](https://github.com/CBIhalsen/text-rewriter) | 31 | 开源 Python 项目，通过词句处理、词性标注、同义词替换和格式优化，让 AI 文本更自然易读。 | [SAFE](https://agentskillshub.top/skill/CBIhalsen/text-rewriter/?utm_source=github&utm_medium=awesome-list) |
| [bejek/humanizer-czech](https://github.com/bejek/humanizer-czech) | 24 | 捷克语AI文本人性化工具，检测并改写27种捷克语AI写作模式，支持改写、自检、4种风格及Claude Code、ChatGPT、Gemini和其他LLM。 | [SAFE](https://agentskillshub.top/skill/bejek/humanizer-czech/?utm_source=github&utm_medium=awesome-list) |
| [amanmaqsood/prose-humanizer](https://github.com/amanmaqsood/prose-humanizer) | 21 | 通用 AI 写作 skill，将泛泛草稿改成具体、真实且风格一致的文字。 | [SAFE](https://agentskillshub.top/skill/amanmaqsood/prose-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [yyx20202020/natural-writing-skill](https://github.com/yyx20202020/natural-writing-skill) | 17 | 中英文自然写作与去AI味 skill，支持事实保护、文风校准、场景路由和可审查提示词。 | [SAFE](https://agentskillshub.top/skill/yyx20202020/natural-writing-skill/?utm_source=github&utm_medium=awesome-list) |
| [hjongc/humanizer-kr](https://github.com/hjongc/humanizer-kr) | 15 | 让带有 AI 痕迹的韩语更像人话、符合语境的 Codex·Claude Code skill | [SAFE](https://agentskillshub.top/skill/hjongc/humanizer-kr/?utm_source=github&utm_medium=awesome-list) |
| [dotoricode/korean-humanizer](https://github.com/dotoricode/korean-humanizer) | 14 | 用于去除生成文本常见 AI 痕迹的韩语人性化提示词和 skill | [SAFE](https://agentskillshub.top/skill/dotoricode/korean-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [msdanyg/humanize-pro](https://github.com/msdanyg/humanize-pro) | 13 | Claude skill：清除各类 AI 痕迹，按渠道重写文本，并从你的修改中学习语气。双重自检，严格不编造。 | [SAFE](https://agentskillshub.top/skill/msdanyg/humanize-pro/?utm_source=github&utm_medium=awesome-list) |
| [shreyas-makes/deslopify](https://github.com/shreyas-makes/deslopify) | 13 | 让 AI 写作更自然 | [SAFE](https://agentskillshub.top/skill/shreyas-makes/deslopify/?utm_source=github&utm_medium=awesome-list) |
| [odinfree/stop-slop-refined](https://github.com/odinfree/stop-slop-refined) | 12 | 用于去除文本中常见 AI 模式的公开写作 skill。 | [SAFE](https://agentskillshub.top/skill/odinfree/stop-slop-refined/?utm_source=github&utm_medium=awesome-list) |
| [machinemade-mm/humanmade-antislop](https://github.com/machinemade-mm/humanmade-antislop) | 11 | Claude Code 的反 AI 腔科学写作 skill，或：用人类口吻进行科学写作。 | [SAFE](https://agentskillshub.top/skill/machinemade-mm/humanmade-antislop/?utm_source=github&utm_medium=awesome-list) |
| [walterwritesai/walter-skills](https://github.com/walterwritesai/walter-skills) | 10 | Claude SEO skills：AI humanizer、AI detection bypass、关键词、QC、本地SEO、程序化SEO、内容改写；MIT… | [SAFE](https://agentskillshub.top/skill/walterwritesai/walter-skills/?utm_source=github&utm_medium=awesome-list) |
| [Albert-Lsk/alskai-deai-writer](https://github.com/Albert-Lsk/alskai-deai-writer) | 9 | 去除 AI 文本的生成痕迹，支持专业商务、技术科普、亲和对话、学术研究 4 种风格 | [SAFE](https://agentskillshub.top/skill/Albert-Lsk/alskai-deai-writer/?utm_source=github&utm_medium=awesome-list) |
| [LeahLiang/humanizer](https://github.com/LeahLiang/humanizer) | 9 | 降低AI率改写Skill，支持知网、维普、Turnitin等平台，中英文适用，保持准确、易读和学术规范。https://ushallpass.ai/ | [SAFE](https://agentskillshub.top/skill/LeahLiang/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [OthmanAdi/humanizer-semitic](https://github.com/OthmanAdi/humanizer-semitic) | 9 | 适用于阿拉伯语（现代标准语、埃及方言、黎凡特方言）和希伯来语的 AI 文本人性化 skill | [SAFE](https://agentskillshub.top/skill/OthmanAdi/humanizer-semitic/?utm_source=github&utm_medium=awesome-list) |
| [behzadsp/humanized-writing-skill](https://github.com/behzadsp/humanized-writing-skill) | 9 | 不依赖特定 agent 的 skill，用于撰写自然、人性化、注重 SEO 的文章和博客内容，避免机械化 AI 语言。 | [SAFE](https://agentskillshub.top/skill/behzadsp/humanized-writing-skill/?utm_source=github&utm_medium=awesome-list) |
| [dixon2004/ai-humanizer](https://github.com/dixon2004/ai-humanizer) | 9 | AI Humanizer 是一个开源工具，可改写 AI 生成的文本，使其更自然流畅。 | [SAFE](https://agentskillshub.top/skill/dixon2004/ai-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [timolabs-ai/claude-humanize-skill](https://github.com/timolabs-ai/claude-humanize-skill) | 9 | Claude Code skill (/humanize)：通过五层编辑去除内容中的 AI 写作痕迹：词汇、句式、项目符号节奏、段落结构和章节叙述。 | [SAFE](https://agentskillshub.top/skill/timolabs-ai/claude-humanize-skill/?utm_source=github&utm_medium=awesome-list) |
| [KondrashovDenis/claude-humanizer-ru-skill](https://github.com/KondrashovDenis/claude-humanizer-ru-skill) | 8 | 清理俄语文本中 AI 套话的 Claude Code skill。blader/humanizer 适配版：公文腔、直译腔、夸大意义、排版退化与审计模式。 | [SAFE](https://agentskillshub.top/skill/KondrashovDenis/claude-humanizer-ru-skill/?utm_source=github&utm_medium=awesome-list) |
| [evergreentree97/K-Humanizer](https://github.com/evergreentree97/K-Humanizer) | 8 | Agent Skill，让 LLM 撰写的韩语对韩国读者更自然，同时保留事实、数字和领域术语。 | [SAFE](https://agentskillshub.top/skill/evergreentree97/K-Humanizer/?utm_source=github&utm_medium=awesome-list) |
| [ferr079/humanizer-fr](https://github.com/ferr079/humanizer-fr) | 8 | Claude Code skill humanizer 的法语分支（blader/humanizer，MIT）——33种适合法语的AI写作模式 | [SAFE](https://agentskillshub.top/skill/ferr079/humanizer-fr/?utm_source=github&utm_medium=awesome-list) |
| [nordefors-max/claude-humanizer-svenska](https://github.com/nordefors-max/claude-humanizer-svenska) | 8 | 去除瑞典专业文本中AI写作模式的Claude skill，涵盖16类模式，适配北欧专业文风。 | [SAFE](https://agentskillshub.top/skill/nordefors-max/claude-humanizer-svenska/?utm_source=github&utm_medium=awesome-list) |
| [pielas-activy/humanizer-pl](https://github.com/pielas-activy/humanizer-pl) | 8 | 双语（PL+EN）humanizer/de-slop skill，基于 blader/humanizer，加入波兰语自然度层，测试 Bielik 是否适合审校… | [SAFE](https://agentskillshub.top/skill/pielas-activy/humanizer-pl/?utm_source=github&utm_medium=awesome-list) |
| [Floka-as/floka-marketplace](https://github.com/Floka-as/floka-marketplace) | 7 | Floka AS 的 Claude Code 工具：humanizer 去 AI 痕迹；board 顾问团；translate-to-no 英译挪威语；for… | [SAFE](https://agentskillshub.top/skill/Floka-as/floka-marketplace/?utm_source=github&utm_medium=awesome-list) |
| [aeopress/writing-skills.TW](https://github.com/aeopress/writing-skills.TW) | 7 | Claude Code 繁体中文写作skill：humanizer-tw+good-writing-zh+fable-econ/fable-explore | [SAFE](https://agentskillshub.top/skill/aeopress/writing-skills.TW/?utm_source=github&utm_medium=awesome-list) |
| [diaiq/claude-skill-humanizer](https://github.com/diaiq/claude-skill-humanizer) | 7 | 让 AI 生成文本更像人类，绕过 GPTZero、Turnitin 等 AI 检测器。由 DiaIQ 提供支持。 | [SAFE](https://agentskillshub.top/skill/diaiq/claude-skill-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [musharrafff/humanizer_v2](https://github.com/musharrafff/humanizer_v2) | 7 | 像真正的人类一样写作，避免常见的 AI 写作模式。 | [SAFE](https://agentskillshub.top/skill/musharrafff/humanizer_v2/?utm_source=github&utm_medium=awesome-list) |
| [Khushiyant/humano](https://github.com/Khushiyant/humano) | 5 | 使用 DIPPER、HMGC 和 ADAT 等技术，将 AI 生成或机器化文本变得更像人类的 Python 包。 | [SAFE](https://agentskillshub.top/skill/Khushiyant/humano/?utm_source=github&utm_medium=awesome-list) |
| [daniel-bogale/anti-ai-writing-humanizer](https://github.com/daniel-bogale/anti-ai-writing-humanizer) | 5 | 让 AI 文本更像人写：可移植的 agent skill，用于写作或改写文字，去除 AI 痕迹，支持 Claude Code、Cursor、Codex、Ope… | [SAFE](https://agentskillshub.top/skill/daniel-bogale/anti-ai-writing-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [durmazoguzhan/turkish-humanify](https://github.com/durmazoguzhan/turkish-humanify) | 5 | 面向 Claude 和 Claude Code 的土耳其语 humanizer skill，保留技术术语 | [SAFE](https://agentskillshub.top/skill/durmazoguzhan/turkish-humanify/?utm_source=github&utm_medium=awesome-list) |
| [humanizer-tools/slop-humanizer](https://github.com/humanizer-tools/slop-humanizer) | 5 | Claude skill：去除 AI 写作模式，将文本重写得更像人类，综合自 8 个文本改写仓库。 | [SAFE](https://agentskillshub.top/skill/humanizer-tools/slop-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [ilyautov/humanizer-it](https://github.com/ilyautov/humanizer-it) | 5 | 去除意大利语文本中的 AI 痕迹，开源 MIT skill for Claude：52 种模式、15 条硬性禁用项、无依赖扫描器 | [SAFE](https://agentskillshub.top/skill/ilyautov/humanizer-it/?utm_source=github&utm_medium=awesome-list) |
| [matsutouya/humanizer-ja](https://github.com/matsutouya/humanizer-ja) | 5 | 去除日文文本中 AI 生成痕迹的 Claude Code skill | [SAFE](https://agentskillshub.top/skill/matsutouya/humanizer-ja/?utm_source=github&utm_medium=awesome-list) |
| [rephrasyai/rephrasy-skills](https://github.com/rephrasyai/rephrasy-skills) | 5 | 面向 AI agent 的免费内容 skill：人性化 AI 文本，保留关键词，适用于 Claude Code、Codex、Cursor 和 ChatGPT。… | [SAFE](https://agentskillshub.top/skill/rephrasyai/rephrasy-skills/?utm_source=github&utm_medium=awesome-list) |

<a id="type-detector"></a>
## 🔍 AI 味检测

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-detector)

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) | 5.9k | 将 AI 撰写的韩文润色得像人写的 Claude skill：检测并改写翻译腔、机械排比及其他71种 AI 痕迹 | [SAFE](https://agentskillshub.top/skill/epoko77-ai/im-not-ai/?utm_source=github&utm_medium=awesome-list) |
| [dmmulroy/anti-slop](https://github.com/dmmulroy/anti-slop) | 5.4k | 用于拒绝缺乏依据的 TypeScript 和 JavaScript 写法的 Oxlint 规则 | [SAFE](https://agentskillshub.top/skill/dmmulroy/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | 4.9k | 审查并改写内容以去除 AI 写作特征的 skill，支持 Claude Code、OpenClaw、Codex 和 Hermes 等 agent。 | [SAFE](https://agentskillshub.top/skill/conorbronsdon/avoid-ai-writing/?utm_source=github&utm_medium=awesome-list) |
| [Jakeschincariol/linkedin-agent-skill](https://github.com/Jakeschincariol/linkedin-agent-skill) | 1.7k | 11个 Claude skill：管理 LinkedIn 账号，按21个开头公式发帖、评论和回复，评估资料、制定周计划，并在发布前去除AI痕迹和评分草稿。 | [SAFE](https://agentskillshub.top/skill/Jakeschincariol/linkedin-agent-skill/?utm_source=github&utm_medium=awesome-list) |
| [peakoss/anti-slop](https://github.com/peakoss/anti-slop) | 842 | 检测并自动关闭低质量和 AI 垃圾 PR 的 GitHub Action | [SAFE](https://agentskillshub.top/skill/peakoss/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [theclaymethod/unslop](https://github.com/theclaymethod/unslop) | 518 | 去除写作中 AI 痕迹的 agent skill | [SAFE](https://agentskillshub.top/skill/theclaymethod/unslop/?utm_source=github&utm_medium=awesome-list) |
| [ilyautov/humanizer-ru](https://github.com/ilyautov/humanizer-ru) | 428 | humanizer-ru：为 AI agent 编辑俄语文本，去除官样话和模板化表达，核查含义与事实。含 67 项特征、21 条禁用规则、扫描器、CLI、MC… | [SAFE](https://agentskillshub.top/skill/ilyautov/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [Aboudjem/humanizer-skill](https://github.com/Aboudjem/humanizer-skill) | 264 | 开源 AI 写作人性化处理工具和检测器，支持 55 种模式、5 种语气及 0–100 AI 痕迹评分，数据不离开本机。 | [SAFE](https://agentskillshub.top/skill/Aboudjem/humanizer-skill/?utm_source=github&utm_medium=awesome-list) |
| [talkstream/ru-text](https://github.com/talkstream/ru-text) | 259 | AI代理的俄语文本质量：清理低质内容、排版、信息风格、编辑规范、UX写作和商务通信。文本评分0–10分。 | [SAFE](https://agentskillshub.top/skill/talkstream/ru-text/?utm_source=github&utm_medium=awesome-list) |
| [lynote-ai/humanize-text-skill](https://github.com/lynote-ai/humanize-text-skill) | 242 | 在线将 AI 文本改写得更像人工撰写 | [SAFE](https://agentskillshub.top/skill/lynote-ai/humanize-text-skill/?utm_source=github&utm_medium=awesome-list) |
| [seyedehsanhadi/sloptrim](https://github.com/seyedehsanhadi/sloptrim) | 213 | 本地 AI 写作模式检测器，为 agent 保存的每个文章文件评分。仅用 Python 标准库，无网络、无模型。 | [SAFE](https://agentskillshub.top/skill/seyedehsanhadi/sloptrim/?utm_source=github&utm_medium=awesome-list) |
| [smixs/humanizer-ru](https://github.com/smixs/humanizer-ru) | 187 | Claude Code、Codex、OpenClaw、Hermes 的 skill：去除俄语文本中的37种AI生成特征，检测是否由神经网络撰写 | [SAFE](https://agentskillshub.top/skill/smixs/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) | 171 | Claude Code 与 Codex 的德语文本润色工具。修改 AI 套话，保留写作风格，并忠实检查 72 种德语模式。 | [SAFE](https://agentskillshub.top/skill/marmbiz/humanizer-de/?utm_source=github&utm_medium=awesome-list) |
| [eric-tramel/slop-guard](https://github.com/eric-tramel/slop-guard) | 164 | 通过低质内容评分遏制低质内容 | [SAFE](https://agentskillshub.top/skill/eric-tramel/slop-guard/?utm_source=github&utm_medium=awesome-list) |
| [Heyosseus/sloppy](https://github.com/Heyosseus/sloppy) | 156 | PHP AI agent债务分析：26规则、Claude Code hooks、git-diff、Rector/Pint、Pest、MCP；本地、确定性、无L… | [SAFE](https://agentskillshub.top/skill/Heyosseus/sloppy/?utm_source=github&utm_medium=awesome-list) |
| [Akimiya-z/codex-guard](https://github.com/Akimiya-z/codex-guard) | 138 | AI/Codex 生成 PR 的质量门禁：合并到 main 前拦截遗留 TODO、密钥泄露、草率提交和失败的 CI。 | [SAFE](https://agentskillshub.top/skill/Akimiya-z/codex-guard/?utm_source=github&utm_medium=awesome-list) |
| [manavmishra/ZeroSlop](https://github.com/manavmishra/ZeroSlop) | 132 | 开源 skill：发现并移除写作中的 AI 垃圾内容 | [SAFE](https://agentskillshub.top/skill/manavmishra/ZeroSlop/?utm_source=github&utm_medium=awesome-list) |
| [brandonwise/humanizer](https://github.com/brandonwise/humanizer) | 128 | 检测并去除 AI 写作痕迹、让文本更自然的 OpenClaw skill，依据 Wikipedia《Signs of AI Writing》。 | [SAFE](https://agentskillshub.top/skill/brandonwise/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [Vladimir-Human/humanizer-ru](https://github.com/Vladimir-Human/humanizer-ru) | 126 | 可验证的俄文文本聊天粘贴清理 | [SAFE](https://agentskillshub.top/skill/Vladimir-Human/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [crabin/paper-humanizer-skill](https://github.com/crabin/paper-humanizer-skill) | 123 | 中英文学术文本润色与人性化 skill，减少 AI 痕迹，保持事实准确。 | [SAFE](https://agentskillshub.top/skill/crabin/paper-humanizer-skill/?utm_source=github&utm_medium=awesome-list) |
| [tbhb/vale-ai-tells](https://github.com/tbhb/vale-ai-tells) | 116 | vale-ai-tells 是用于检查 AI 写作痕迹的 Vale 风格包。 | [SAFE](https://agentskillshub.top/skill/tbhb/vale-ai-tells/?utm_source=github&utm_medium=awesome-list) |
| [qin1473692580-ux/oh-story-claudecode](https://github.com/qin1473692580-ux/oh-story-claudecode) | 104 | 网文/小说写作 skill 包，涵盖长短篇扫榜、拆文、写作、去AI味和封面图制作 | [SAFE](https://agentskillshub.top/skill/qin1473692580-ux/oh-story-claudecode/?utm_source=github&utm_medium=awesome-list) |
| [Nopon-Knowledge/huawei-cup-modeling-skill](https://github.com/Nopon-Knowledge/huawei-cup-modeling-skill) | 99 | Codex Skill：面向华为杯的论文AI痕迹诊断、改写、图表优化、规则核验与提交审计，保留事实和引文 | [SAFE](https://agentskillshub.top/skill/Nopon-Knowledge/huawei-cup-modeling-skill/?utm_source=github&utm_medium=awesome-list) |
| [flamehaven01/AI-SLOP-Detector](https://github.com/flamehaven01/AI-SLOP-Detector) | 99 | 停止发布 AI 垃圾代码。检测 AI 生成代码中的空函数、虚假文档和夸大注释。 | [SAFE](https://agentskillshub.top/skill/flamehaven01/AI-SLOP-Detector/?utm_source=github&utm_medium=awesome-list) |
| [misbahsy/anti-ai-slop](https://github.com/misbahsy/anti-ai-slop) | 96 | 用于检查并去除 AI 垃圾内容的 agent skill，可与 Codex、Claude Code 等 AI 工具配合使用。 | [SAFE](https://agentskillshub.top/skill/misbahsy/anti-ai-slop/?utm_source=github&utm_medium=awesome-list) |
| [distil-labs/distil-ai-slop-detector](https://github.com/distil-labs/distil-ai-slop-detector) | 95 | 在浏览器本地检测 AI 生成的文本 | [SAFE](https://agentskillshub.top/skill/distil-labs/distil-ai-slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [DadaNanjesha/AI-content-detector-Humanizer](https://github.com/DadaNanjesha/AI-content-detector-Humanizer) | 91 | 检测 PDF 文档中的 AI 生成内容，并将 AI 文本改写得更自然。基于 Streamlit、spaCy 和 Hugging Face transforme… | [SAFE](https://agentskillshub.top/skill/DadaNanjesha/AI-content-detector-Humanizer/?utm_source=github&utm_medium=awesome-list) |
| [rsionnach/sloppylint](https://github.com/rsionnach/sloppylint) | 91 | Python AI 代码检测器：发现代码库中的过度设计、幻觉和死代码 | [SAFE](https://agentskillshub.top/skill/rsionnach/sloppylint/?utm_source=github&utm_medium=awesome-list) |
| [airlock-hq/airlock](https://github.com/airlock-hq/airlock) | 86 | Airlock 将每次 git push 转为无垃圾内容的 PR。 | [SAFE](https://agentskillshub.top/skill/airlock-hq/airlock/?utm_source=github&utm_medium=awesome-list) |
| [gouwsxander/slop-detector](https://github.com/gouwsxander/slop-detector) | 62 | AI 写作检测器的端到端实现 | [SAFE](https://agentskillshub.top/skill/gouwsxander/slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [AgriciDaniel/anti-slop](https://github.com/AgriciDaniel/anti-slop) | 61 | 发现并修复 AI 辅助文章、代码、文档和 agent 输出的实质缺陷。报告缺陷，不判定作者身份。用结构化测试代替模型判断，因 LLM 评审与人工低质标签的一致… | [SAFE](https://agentskillshub.top/skill/AgriciDaniel/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [Text2Go/ai-humanizer-mcp-server](https://github.com/Text2Go/ai-humanizer-mcp-server) | 61 | 帮助改进 AI 生成内容，使其更自然。具备 AI 检测和文本增强功能。 | [SAFE](https://agentskillshub.top/skill/Text2Go/ai-humanizer-mcp-server/?utm_source=github&utm_medium=awesome-list) |
| [millionco/deslop-js](https://github.com/millionco/deslop-js) | 60 | 清理 JavaScript 代码 | [SAFE](https://agentskillshub.top/skill/millionco/deslop-js/?utm_source=github&utm_medium=awesome-list) |
| [ilien-dev/quiron](https://github.com/ilien-dev/quiron) | 57 | AI humanizer skill，适用于 Claude Code、Codex 和 Cursor。去除 AI 腔和写作痕迹，并与人类基准比较改写结果。 | [SAFE](https://agentskillshub.top/skill/ilien-dev/quiron/?utm_source=github&utm_medium=awesome-list) |
| [Nimblesite/Deslop](https://github.com/Nimblesite/Deslop) | 56 | Deslop Live 在 IDE 中分析重复代码，提供内联警告、问题视图和实时查询通道。 | [SAFE](https://agentskillshub.top/skill/Nimblesite/Deslop/?utm_source=github&utm_medium=awesome-list) |
| [pablocaeg/sloptotal](https://github.com/pablocaeg/sloptotal) | 55 | 开源 AI 文本与 ChatGPT 检测器：23 个引擎，统一校准评分，数值均经测量。支持 CLI、MCP server 和 GitHub Action，可自… | [SAFE](https://agentskillshub.top/skill/pablocaeg/sloptotal/?utm_source=github&utm_medium=awesome-list) |
| [apurvrdx1/tagore](https://github.com/apurvrdx1/tagore) | 54 | 让 AI 文本更像人写。29种模式+8条规则+8维评分，支持 Claude Code、OpenCode、Copilot CLI、Codex、Gemini、Go… | [SAFE](https://agentskillshub.top/skill/apurvrdx1/tagore/?utm_source=github&utm_medium=awesome-list) |
| [stephenlzc/humanize-mba-text-skill](https://github.com/stephenlzc/humanize-mba-text-skill) | 51 | 中文MBA论文AI写作痕迹检测与去除工具 | [SAFE](https://agentskillshub.top/skill/stephenlzc/humanize-mba-text-skill/?utm_source=github&utm_medium=awesome-list) |
| [humanizerai/agent-skills](https://github.com/humanizerai/agent-skills) | 49 | HumanizerAI：用于 Claude Code 和 Codex 的 agent skill，AI 检测与文本去 AI 化 | [SAFE](https://agentskillshub.top/skill/humanizerai/agent-skills/?utm_source=github&utm_medium=awesome-list) |
| [mmartoccia/grain](https://github.com/mmartoccia/grain) | 34 | 面向 AI 辅助代码库的低质代码检查器 | [SAFE](https://agentskillshub.top/skill/mmartoccia/grain/?utm_source=github&utm_medium=awesome-list) |
| [dripips/plain-prose](https://github.com/dripips/plain-prose) | 25 | 去除英语、俄语和德语文章中 AI 写作模式的 agent skill，合并 stop-slop 和 avoid-ai-writing，加入零依赖检查器。 | [SAFE](https://agentskillshub.top/skill/dripips/plain-prose/?utm_source=github&utm_medium=awesome-list) |
| [scale-venture-partners/windbag](https://github.com/scale-venture-partners/windbag) | 25 | 反垃圾代码检查器：捕获描述变更历史而非当前约束的注释（Python/JS/TS/Terraform） | [SAFE](https://agentskillshub.top/skill/scale-venture-partners/windbag/?utm_source=github&utm_medium=awesome-list) |
| [vstorm-co/content-skills](https://github.com/vstorm-co/content-skills) | 25 | 内容工作室 skill 包，支持博客、社交媒体、幻灯片、视频和信息图；遵循品牌规范，内置反低质机制。支持 Claude Code、Codex 和 AGENTS… | [SAFE](https://agentskillshub.top/skill/vstorm-co/content-skills/?utm_source=github&utm_medium=awesome-list) |
| [drunkrhin0/antislop](https://github.com/drunkrhin0/antislop) | 24 | 用低质内容对抗低质内容，清除 AI 低质内容。 | [SAFE](https://agentskillshub.top/skill/drunkrhin0/antislop/?utm_source=github&utm_medium=awesome-list) |
| [momo2young/humanize-academic-writing](https://github.com/momo2young/humanize-academic-writing) | 24 | 面向社科学者的 Cursor skill（支持 Claude），将 AI 生成的学术文本转为自然学术写作 | [SAFE](https://agentskillshub.top/skill/momo2young/humanize-academic-writing/?utm_source=github&utm_medium=awesome-list) |
| [walidboulanouar/anti-ai-slop](https://github.com/walidboulanouar/anti-ai-slop) | 24 | 检测并移除 AI 套话词和长破折号的 CLI | [SAFE](https://agentskillshub.top/skill/walidboulanouar/anti-ai-slop/?utm_source=github&utm_medium=awesome-list) |
| [allanta8/slop-check](https://github.com/allanta8/slop-check) | 19 | 面向 X、ViewFT、LinkedIn 和长文的反低质内容审核 skill | [SAFE](https://agentskillshub.top/skill/allanta8/slop-check/?utm_source=github&utm_medium=awesome-list) |
| [badmuriss/unslop](https://github.com/badmuriss/unslop) | 19 | Strip AI writing tells at two layers: surface (Wikipedia Signs of AI writing) + narrative (StoryScope, arXiv:2604.03136). A model-agnostic LLM skill. | [SAFE](https://agentskillshub.top/skill/badmuriss/unslop/?utm_source=github&utm_medium=awesome-list) |
| [dabit3/deslop](https://github.com/dabit3/deslop) | 19 | 检测并移除分支中的 AI 生成代码模式（slop） | [SAFE](https://agentskillshub.top/skill/dabit3/deslop/?utm_source=github&utm_medium=awesome-list) |
| [noeigenstate/AI-Writing-without-AI-feel](https://github.com/noeigenstate/AI-Writing-without-AI-feel) | 19 | 去除 AI 痕迹，提炼个人写作风格，整合主流写作 skills | [SAFE](https://agentskillshub.top/skill/noeigenstate/AI-Writing-without-AI-feel/?utm_source=github&utm_medium=awesome-list) |
| [adamdunkels/deslop-text](https://github.com/adamdunkels/deslop-text) | 18 | 消除30种 AI 写作痕迹的 Claude skill | [SAFE](https://agentskillshub.top/skill/adamdunkels/deslop-text/?utm_source=github&utm_medium=awesome-list) |
| [comol/Humanizer_RU](https://github.com/comol/Humanizer_RU) | 16 | 俄语 Humanizer：面向 LLM agent 的 Agent Skill 和可读性检查器 | [SAFE](https://agentskillshub.top/skill/comol/Humanizer_RU/?utm_source=github&utm_medium=awesome-list) |
| [skew202/antislop](https://github.com/skew202/antislop) | 16 | 检测 AI 生成低质代码的多语言代码检查工具 | [SAFE](https://agentskillshub.top/skill/skew202/antislop/?utm_source=github&utm_medium=awesome-list) |
| [huangziyuan-general/dsh-novel-forge](https://github.com/huangziyuan-general/dsh-novel-forge) | 15 | DSH 小说锻炉：将AI写作通病转为代码约束：事实账本、上下文包、阶段门禁、零费用去AI味扫描、确定性审计、提案式修订。 | [SAFE](https://agentskillshub.top/skill/huangziyuan-general/dsh-novel-forge/?utm_source=github&utm_medium=awesome-list) |
| [cglabs-ai/guardian](https://github.com/cglabs-ai/guardian) | 12 | 在 AI 垃圾代码进入你的代码库前拦截它 | [SAFE](https://agentskillshub.top/skill/cglabs-ai/guardian/?utm_source=github&utm_medium=awesome-list) |
| [skyzer/deslop-the-copy](https://github.com/skyzer/deslop-the-copy) | 12 | 可移植的 agent skill，去除 AI 写作模式，同时保留作者文风。支持 Claude Code、Codex、OpenClaw、Cursor 等。 | [SAFE](https://agentskillshub.top/skill/skyzer/deslop-the-copy/?utm_source=github&utm_medium=awesome-list) |
| [styrene-lab/lipstyk](https://github.com/styrene-lab/lipstyk) | 12 | 反 AI 垃圾代码分析，检测 Rust、TS/JS、Python、HTML/CSS 中的机器生成代码模式 | [SAFE](https://agentskillshub.top/skill/styrene-lab/lipstyk/?utm_source=github&utm_medium=awesome-list) |
| [MauroPello/stop-the-slop](https://github.com/MauroPello/stop-the-slop) | 11 | 实时识别 AI 生成的 YouTube 脚本和内容农场。支持 Chrome、Firefox 的开源浏览器扩展，提供缩略图标记和句子热力图。 | [SAFE](https://agentskillshub.top/skill/MauroPello/stop-the-slop/?utm_source=github&utm_medium=awesome-list) |
| [Octember/stupify](https://github.com/Octember/stupify) | 11 | 反低质代码审查工具 | [SAFE](https://agentskillshub.top/skill/Octember/stupify/?utm_source=github&utm_medium=awesome-list) |
| [TinyFrontier/anti-slop-py](https://github.com/TinyFrontier/anti-slop-py) | 11 | 一个确定性的 Python linter，检测 AI 编程 agent 未提供依据就屏蔽类型检查器。 | [SAFE](https://agentskillshub.top/skill/TinyFrontier/anti-slop-py/?utm_source=github&utm_medium=awesome-list) |
| [beavis07/slop-detector](https://github.com/beavis07/slop-detector) | 11 | 用于检测 AI Slop 的 AI Slop | [SAFE](https://agentskillshub.top/skill/beavis07/slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [cm2435/slopcop](https://github.com/cm2435/slopcop) | 11 | 用于发现 LLM 生成反模式的快速 Python linter，使用 Rust 编写，基于 tree-sitter。 | [SAFE](https://agentskillshub.top/skill/cm2435/slopcop/?utm_source=github&utm_medium=awesome-list) |
| [0xNyk/unmachined](https://github.com/0xNyk/unmachined) | 10 | 反 AI-slop agent skill：让文本像人写的、UI 像人做的，而非生成的。确定性扫描器与按严重程度分级的特征目录。 | [SAFE](https://agentskillshub.top/skill/0xNyk/unmachined/?utm_source=github&utm_medium=awesome-list) |
| [tomerose/stop-slop](https://github.com/tomerose/stop-slop) | 10 | 写作技能：5维评分，检测41种AI写作反模式。支持 Claude Code、Claude、Cursor、Copilot 和中英文。 | [SAFE](https://agentskillshub.top/skill/tomerose/stop-slop/?utm_source=github&utm_medium=awesome-list) |
| [Aaron-Bushnell/humanizer](https://github.com/Aaron-Bushnell/humanizer) | 9 | 检测47种AI写作模式，并按5种人类语气重写文本。基于ICML 2025词元概率分布研究的Claude Code skill。 | [SAFE](https://agentskillshub.top/skill/Aaron-Bushnell/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [aplaceforallmystuff/claude-slop-detector](https://github.com/aplaceforallmystuff/claude-slop-detector) | 9 | 用于检测内容中 AI 生成写作模式（slop）的 Claude Code skill | [SAFE](https://agentskillshub.top/skill/aplaceforallmystuff/claude-slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [apoapostolov/humanizer](https://github.com/apoapostolov/humanizer) | 8 | Humanizer 是一种 AI 写作 skill，可检测并改写 AI 文本特征，保留原意、匹配受众和语气，减少夸张与冗余，使内容更自然具体。 | [SAFE](https://agentskillshub.top/skill/apoapostolov/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [bnivanov/omp-writing-skills](https://github.com/bnivanov/omp-writing-skills) | 8 | 面向 agent harness 的生产级反低质 AI 写作套件，含语气校准、写作规则、去低质编辑器和确定性 AST 检查 | [SAFE](https://agentskillshub.top/skill/bnivanov/omp-writing-skills/?utm_source=github&utm_medium=awesome-list) |
| [puneethkotha/humanizer-workbench](https://github.com/puneethkotha/humanizer-workbench) | 8 | AI humanizer：将 AI 生成文本改写为自然人类写作的 CLI 工具和 Claude Code skill。 | [SAFE](https://agentskillshub.top/skill/puneethkotha/humanizer-workbench/?utm_source=github&utm_medium=awesome-list) |
| [theserverlessdev/wsc](https://github.com/theserverlessdev/wsc) | 8 | 散文校对器和AI套话检测器：识别模糊措辞、被动语态、模棱两可表达及190多项有研究依据的AI特征。提供网页编辑器、API、MCP server、CLI和Git… | [SAFE](https://agentskillshub.top/skill/theserverlessdev/wsc/?utm_source=github&utm_medium=awesome-list) |
| [zaterka/anti-slop-python](https://github.com/zaterka/anti-slop-python) | 8 | anti-slop-python：拒绝低证据、低信号 Python 模式的 AST 规则，基于标准库 ast，无运行时依赖，含 11 条 Python 专用规… | [CAUTION](https://agentskillshub.top/skill/zaterka/anti-slop-python/?utm_source=github&utm_medium=awesome-list) |
| [Lowcountry-AI/guardrail-skills](https://github.com/Lowcountry-AI/guardrail-skills) | 7 | 三个独立的 AI 编程 agent 防护：反 AI-slop 写作清单、代码注释规范清单、多 agent 编排配方钩子 | [SAFE](https://agentskillshub.top/skill/Lowcountry-AI/guardrail-skills/?utm_source=github&utm_medium=awesome-list) |
| [NorbertBodziony/biome-anti-slop](https://github.com/NorbertBodziony/biome-anti-slop) | 7 | Biome GritQL 规则：拒绝证据不足的 TypeScript 模式 | [SAFE](https://agentskillshub.top/skill/NorbertBodziony/biome-anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [forint573/human-copywrite](https://github.com/forint573/human-copywrite) | 7 | Claude Agent Skill：让AI营销和长文案更像人写，适用于落地页、销售页、电子书、案例和创始人笔记；去除AI痕迹与流程噪音，删掉破折号，不编造事… | [SAFE](https://agentskillshub.top/skill/forint573/human-copywrite/?utm_source=github&utm_medium=awesome-list) |
| [LanNguyenSi/agent-dx](https://github.com/LanNguyenSi/agent-dx) | 6 | Monorepo workshop for agent-development tooling: orchestrator-workflow and okf-kit ship on npm; slop-detector is the AI-slop linter for PRs. | [SAFE](https://agentskillshub.top/skill/LanNguyenSi/agent-dx/?utm_source=github&utm_medium=awesome-list) |
| [godagoo/slopcheck-deslop](https://github.com/godagoo/slopcheck-deslop) | 6 | 检测并遏制 AI 编写 TypeScript 的结构劣化。Slop Check 发现问题，Deslop 工具清理。基于 SlopCodeBench（arXiv… | [SAFE](https://agentskillshub.top/skill/godagoo/slopcheck-deslop/?utm_source=github&utm_medium=awesome-list) |
| [lokicik/novel-idea-hunter](https://github.com/lokicik/novel-idea-hunter) | 6 | 面向编程 agent 的证据优先、反低质内容机会发现 skill（Claude Code + Codex） | [SAFE](https://agentskillshub.top/skill/lokicik/novel-idea-hunter/?utm_source=github&utm_medium=awesome-list) |
| [infoslack/anti-slop-py](https://github.com/infoslack/anti-slop-py) | 5 | 用于拒绝低证据 Python 模式的严格 lint 规则 | [SAFE](https://agentskillshub.top/skill/infoslack/anti-slop-py/?utm_source=github&utm_medium=awesome-list) |
| [liuxiaobai8868/ai-slop-detector](https://github.com/liuxiaobai8868/ai-slop-detector) | 5 | 多语言 AI 味检测与去 AI 化工具集（中/英/西/阿/印地） | [SAFE](https://agentskillshub.top/skill/liuxiaobai8868/ai-slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [lxgicstudios/humanize-cli](https://github.com/lxgicstudios/humanize-cli) | 5 | 检测 AI 生成文本模式并改进写作以避免检测的 CLI 工具，对内容评分、分析并使其更像人类写作。 | [SAFE](https://agentskillshub.top/skill/lxgicstudios/humanize-cli/?utm_source=github&utm_medium=awesome-list) |

<a id="type-chinese"></a>
## 🀄 中文去 AI 味

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-chinese)

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 19.2k | Humanizer 中文版：Claude Code skill，用于去除文本中的 AI 生成痕迹。 | [SAFE](https://agentskillshub.top/skill/op7418/Humanizer-zh/?utm_source=github&utm_medium=awesome-list) |
| [larashero3-dotcom/lieflat-less-ai-tone](https://github.com/larashero3-dotcom/lieflat-less-ai-tone) | 2.6k | 基于283万字语料统计的去AI味skill | [SAFE](https://agentskillshub.top/skill/larashero3-dotcom/lieflat-less-ai-tone/?utm_source=github&utm_medium=awesome-list) |
| [MrGeDiao/shuorenhua](https://github.com/MrGeDiao/shuorenhua) | 2.0k | 中文优先的去 AI 味改写 skill：保留事实，按场景改写，可直接发布，支持 Codex、Claude Code、Cursor、ChatGPT | [SAFE](https://agentskillshub.top/skill/MrGeDiao/shuorenhua/?utm_source=github&utm_medium=awesome-list) |
| [Raymondhou0917/speak-human-tw](https://github.com/Raymondhou0917/speak-human-tw) | 1.0k | 「说人话」：繁体中文去 AI 味改写 skill，识别 38 种 AI 写作痕迹，校正大陆用语和半角标点，供 Claude Code、Codex、Cursor… | [SAFE](https://agentskillshub.top/skill/Raymondhou0917/speak-human-tw/?utm_source=github&utm_medium=awesome-list) |
| [OUBIGFA/De-AI-Prompt-Enhancer-Writer-Booster-SKILL](https://github.com/OUBIGFA/De-AI-Prompt-Enhancer-Writer-Booster-SKILL) | 857 | 去AI味提示词：作家增强 SKILL | [SAFE](https://agentskillshub.top/skill/OUBIGFA/De-AI-Prompt-Enhancer-Writer-Booster-SKILL/?utm_source=github&utm_medium=awesome-list) |
| [LifelongLazyLearner/qu-ai-wei](https://github.com/LifelongLazyLearner/qu-ai-wei) | 634 | 去除简体中文 AI 写作痕迹的 Chinese humanizer skill | [SAFE](https://agentskillshub.top/skill/LifelongLazyLearner/qu-ai-wei/?utm_source=github&utm_medium=awesome-list) |
| [Liuxiangjian-ai/official-document-skill](https://github.com/Liuxiangjian-ai/official-document-skill) | 388 | 面向公文写作的 skill，基于数百篇报刊文章总结，生成规范、稳妥、具体的公文 | [SAFE](https://agentskillshub.top/skill/Liuxiangjian-ai/official-document-skill/?utm_source=github&utm_medium=awesome-list) |
| [redbaronyyyyy-eng/humanizer-zh-academic](https://github.com/redbaronyyyyy-eng/humanizer-zh-academic) | 308 | 降低中文学术写作 AIGC 检测率的 Claude Code Skill | [SAFE](https://agentskillshub.top/skill/redbaronyyyyy-eng/humanizer-zh-academic/?utm_source=github&utm_medium=awesome-list) |
| [Hyacehila/humanizer-zh-next](https://github.com/Hyacehila/humanizer-zh-next) | 178 | 去除中文文本 AI 写作痕迹的 skill，基于 blader/humanizer 和 op7418/humanizer-zh | [SAFE](https://agentskillshub.top/skill/Hyacehila/humanizer-zh-next/?utm_source=github&utm_medium=awesome-list) |
| [ai-zixun/humanizer-zh](https://github.com/ai-zixun/humanizer-zh) | 178 | humanizer-zh 是兼容 Codex、Claude Code 和 OpenClaw 的中文去 AI 味 skill，用于重写、润色和审阅长文本。 | [SAFE](https://agentskillshub.top/skill/ai-zixun/humanizer-zh/?utm_source=github&utm_medium=awesome-list) |
| [VincentOld/stop-slop-zh](https://github.com/VincentOld/stop-slop-zh) | 93 | 消除中文 AI 写作痕迹的 Claude Skill：拆解排比、去名词化、将抽象主语换成具体细节。灵感来自 hardikpandya/stop-slop。 | [SAFE](https://agentskillshub.top/skill/VincentOld/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [mengke-wang/zh-humanizer-literary](https://github.com/mengke-wang/zh-humanizer-literary) | 86 | 增强 Codex Skill 的中文去 AI 味与文采，让草稿更像人写。 | [SAFE](https://agentskillshub.top/skill/mengke-wang/zh-humanizer-literary/?utm_source=github&utm_medium=awesome-list) |
| [baibanbao/qu-ai-wei](https://github.com/baibanbao/qu-ai-wei) | 67 | 中文写作的 AI 痕迹清理 skill，合并三家规则并裁决七处矛盾，用于清理中文草稿中的 AI 痕迹。 | [SAFE](https://agentskillshub.top/skill/baibanbao/qu-ai-wei/?utm_source=github&utm_medium=awesome-list) |
| [cangtianhuang/humanizer-academic-zh](https://github.com/cangtianhuang/humanizer-academic-zh) | 63 | Humanizer 中文学术版，Claude Code Skills/System Prompt，中文学术论文去AI痕迹提示词 | [SAFE](https://agentskillshub.top/skill/cangtianhuang/humanizer-academic-zh/?utm_source=github&utm_medium=awesome-list) |
| [allenloves/de-ai-tone](https://github.com/allenloves/de-ai-tone) | 62 | 去 AI 味：繁體中文寫作與翻譯的風格規範（Claude Code skill） | [SAFE](https://agentskillshub.top/skill/allenloves/de-ai-tone/?utm_source=github&utm_medium=awesome-list) |
| [pencil20388-eng/stop-slop-zh](https://github.com/pencil20388-eng/stop-slop-zh) | 52 | 消除中文写作中的 AI 腔：禁用词、标点规则、结构约束与四层质检。支持 Claude Code、Cursor、Codex CLI。 | [SAFE](https://agentskillshub.top/skill/pencil20388-eng/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [Smith-2758/Humanizer-zh-academic](https://github.com/Smith-2758/Humanizer-zh-academic) | 26 | 大学生学术写作去AI味与反检测提示词指南，将机器腔调改为朴实严谨的学生笔触。 | [SAFE](https://agentskillshub.top/skill/Smith-2758/Humanizer-zh-academic/?utm_source=github&utm_medium=awesome-list) |
| [swaylq/humanize-chinese](https://github.com/swaylq/humanize-chinese) | 25 | 中文 AI 文本去痕迹与 Claude/SynthID 水印检查：六段式改写，清理零宽字符和同形字；仅测量 SynthID 残留，不声称可删除。纯 Pytho… | [SAFE](https://agentskillshub.top/skill/swaylq/humanize-chinese/?utm_source=github&utm_medium=awesome-list) |
| [mattwang1230/legal-paper-framework-humanizer-zh](https://github.com/mattwang1230/legal-paper-framework-humanizer-zh) | 24 | 基于《法学》期刊目录语料的中文法学写作 skill，减少论文框架的 AI 味 | [SAFE](https://agentskillshub.top/skill/mattwang1230/legal-paper-framework-humanizer-zh/?utm_source=github&utm_medium=awesome-list) |
| [0xtresser/cn-humanizer](https://github.com/0xtresser/cn-humanizer) | 16 | 减少 AI 生成内容的 AI 味的 Agent Skill，适用于内容生成和英文翻译。 | [SAFE](https://agentskillshub.top/skill/0xtresser/cn-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [yelban/humanizer.TW](https://github.com/yelban/humanizer.TW) | 15 | 去除文本中 AI 生成痕迹的 Claude Code skill | [SAFE](https://agentskillshub.top/skill/yelban/humanizer.TW/?utm_source=github&utm_medium=awesome-list) |
| [leeguooooo/stop-slop-zh](https://github.com/leeguooooo/stop-slop-zh) | 11 | 消除中文 AI 写作痕迹的 Claude Skill：拆解排比、去名词化、具体化抽象主语。 | [SAFE](https://agentskillshub.top/skill/leeguooooo/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [deedeekong07-alt/fiction-humanizer-zh](https://github.com/deedeekong07-alt/fiction-humanizer-zh) | 10 | 中文小说去AI化写作 skill，用于AI辅助小说创作 | [SAFE](https://agentskillshub.top/skill/deedeekong07-alt/fiction-humanizer-zh/?utm_source=github&utm_medium=awesome-list) |
| [evelynyaxueke/anti-ai-writing-kit-zh](https://github.com/evelynyaxueke/anti-ai-writing-kit-zh) | 9 | 可定制、可维护的中文去 AI 味写作系统，支持写作、编辑、改写、润色和审稿。 | [SAFE](https://agentskillshub.top/skill/evelynyaxueke/anti-ai-writing-kit-zh/?utm_source=github&utm_medium=awesome-list) |
| [fanjack510-ctrl/chinese-webnovel-editor](https://github.com/fanjack510-ctrl/chinese-webnovel-editor) | 8 | 中文网络小说逐镜头去AI味审查与精修 skill | [SAFE](https://agentskillshub.top/skill/fanjack510-ctrl/chinese-webnovel-editor/?utm_source=github&utm_medium=awesome-list) |
| [fqy9242/TextAIGCreducer](https://github.com/fqy9242/TextAIGCreducer) | 8 | 基于 AI 降低文本、论文和段落的 AI 痕迹 | [SAFE](https://agentskillshub.top/skill/fqy9242/TextAIGCreducer/?utm_source=github&utm_medium=awesome-list) |
| [nagameTW/formosa-humanizer](https://github.com/nagameTW/formosa-humanizer) | 8 | blader/humanizer 的繁中版，讓 AI 生成的中文內容看起來更像人寫的。含中國用語偵測和中文標點規則等 49 種模式，支援 Claude Code、Codex 等 Agent | [SAFE](https://agentskillshub.top/skill/nagameTW/formosa-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [tentenco/shuorenhua-zh-tw](https://github.com/tentenco/shuorenhua-zh-tw) | 8 | 繁中（台湾）AI腔清理skill：去AI腔、中港用语和简繁错字，教育部标点，七种文体。Claude Code、Codex、Cursor、ChatGPT。 | [SAFE](https://agentskillshub.top/skill/tentenco/shuorenhua-zh-tw/?utm_source=github&utm_medium=awesome-list) |
| [RobinZorro86/humanizer-zh-plus](https://github.com/RobinZorro86/humanizer-zh-plus) | 7 | 中文文本去AI味工具，含34种Pattern（29种原版+5种中文特有），适用于中文写作场景。 | [SAFE](https://agentskillshub.top/skill/RobinZorro86/humanizer-zh-plus/?utm_source=github&utm_medium=awesome-list) |
| [Zeng-xiangkai/humanizer-document-zh](https://github.com/Zeng-xiangkai/humanizer-document-zh) | 7 | Claude Code Skill，识别并移除 LLM 生成论文的典型痕迹，基于 Wikipedia“Signs of AI writing”等来源，总结28… | [SAFE](https://agentskillshub.top/skill/Zeng-xiangkai/humanizer-document-zh/?utm_source=github&utm_medium=awesome-list) |
| [M1kasaYU/paper-expression-editor-skill](https://github.com/M1kasaYU/paper-expression-editor-skill) | 5 | 中文论文与开题报告去AI化表达评阅和改写工具，适用于 Codex | [SAFE](https://agentskillshub.top/skill/M1kasaYU/paper-expression-editor-skill/?utm_source=github&utm_medium=awesome-list) |
| [NocodeMrLi/mr-li-writer-skill](https://github.com/NocodeMrLi/mr-li-writer-skill) | 5 | Mr.Li Writer 是一种去除 AI 腔调的中文长文写作 skill：评估选题价值，寻找独特角度，设计开头和标题，并完成可发布的稿件。 | [SAFE](https://agentskillshub.top/skill/NocodeMrLi/mr-li-writer-skill/?utm_source=github&utm_medium=awesome-list) |
| [dbhosbu-dotcom/renwei](https://github.com/dbhosbu-dotcom/renwei) | 5 | 人味 Renwei——书稿级中文去AI味工具，含51条规则，提供无Token lint CLI，兼容 AGENTS.md。 | [SAFE](https://agentskillshub.top/skill/dbhosbu-dotcom/renwei/?utm_source=github&utm_medium=awesome-list) |
| [evoworkAI/xiaoci-skill](https://github.com/evoworkAI/xiaoci-skill) | 5 | 消磁：中文去 AI 味 skill，用密度门限和反向清单替代特征清单 | [SAFE](https://agentskillshub.top/skill/evoworkAI/xiaoci-skill/?utm_source=github&utm_medium=awesome-list) |
| [wdkang123/stop-slop-zh](https://github.com/wdkang123/stop-slop-zh) | 5 | 减少中文 LLM 写作中可预测的 AI 行文模式，同时保持事实和作者风格的 skill。 | [SAFE](https://agentskillshub.top/skill/wdkang123/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [win4r/jev-humanize-writing](https://github.com/win4r/jev-humanize-writing) | 5 | Jev 辅助自然写作编辑：保留事实、归因与作者语气 | [SAFE](https://agentskillshub.top/skill/win4r/jev-humanize-writing/?utm_source=github&utm_medium=awesome-list) |

<a id="type-code"></a>
## 🧹 代码去 AI 味

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-code)

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [peteromallet/desloppify](https://github.com/peteromallet/desloppify) | 3.2k | 用于将粗糙代码改进为工程化且美观代码的 Agent。 | [SAFE](https://agentskillshub.top/skill/peteromallet/desloppify/?utm_source=github&utm_medium=awesome-list) |
| [MrZoyo/deslop-GPT](https://github.com/MrZoyo/deslop-GPT) | 137 | 以删除为先的 Agent skill：移除测试膨胀、验证表演和推测性后备方案，同时保持行为不变。 | [SAFE](https://agentskillshub.top/skill/MrZoyo/deslop-GPT/?utm_source=github&utm_medium=awesome-list) |
| [LeonardNJU/code-humanizer](https://github.com/LeonardNJU/code-humanizer) | 70 | 代码清理 agent skill：移除 AI 生成代码赘余，经测试验证且保持行为不变。 | [SAFE](https://agentskillshub.top/skill/LeonardNJU/code-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [iCodeCraft/anti-slop](https://github.com/iCodeCraft/anti-slop) | 27 | 可直接接入的 skill，避免 AI coding agents 产出低质代码：kill-slop、security-review、PR hygiene | [SAFE](https://agentskillshub.top/skill/iCodeCraft/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [agent-sh/deslop](https://github.com/agent-sh/deslop) | 7 | 清理 AI 生成的冗余内容，尽量少改动并保持行为不变 | [SAFE](https://agentskillshub.top/skill/agent-sh/deslop/?utm_source=github&utm_medium=awesome-list) |

<a id="type-design"></a>
## 🎨 设计去 AI 味

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-design)

<table><tr>
<td align="center" valign="top"><a href="https://github.com/sva-admin/sv-academy-prom-design"><img src="assets/previews/sva-admin__sv-academy-prom-design.jpg" width="260" alt="sva-admin/sv-academy-prom-design"></a><br><sub><a href="https://github.com/sva-admin/sv-academy-prom-design">sva-admin/sv-academy-prom-design</a></sub></td>
</tr></table>

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 94.0k | Taste-Skill：让 AI 具备审美，避免生成无聊、千篇一律的内容 | [SAFE](https://agentskillshub.top/skill/Leonxlnx/taste-skill/?utm_source=github&utm_medium=awesome-list) |
| [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 29.8k | 适用于 Claude Code、Cursor 和 Codex 的反 AI 垃圾设计 skill。 | [SAFE](https://agentskillshub.top/skill/Nutlope/hallmark/?utm_source=github&utm_medium=awesome-list) |
| [yetone/kill-ai-slop](https://github.com/yetone/kill-ai-slop) | 1.3k | AI 生成产品的视觉与文案特征指南，以及扫描项目并清除它们的 Agent Skill。https://killaislop.com | [SAFE](https://agentskillshub.top/skill/yetone/kill-ai-slop/?utm_source=github&utm_medium=awesome-list) |
| [agiwhitelist/auteur](https://github.com/agiwhitelist/auteur) | 1.0k | Claude Code skill 以电影制作方式指导网站，涵盖提交清单、生成资源、构建和每次发布前执行的 anti-slop linter。 | [SAFE](https://agentskillshub.top/skill/agiwhitelist/auteur/?utm_source=github&utm_medium=awesome-list) |
| [Yu-369/VibeCurb](https://github.com/Yu-369/VibeCurb) | 980 | VibeCurb：为 AI 工作流注入审美，避免 agent 生成乏味的 AI 垃圾内容 | [SAFE](https://agentskillshub.top/skill/Yu-369/VibeCurb/?utm_source=github&utm_medium=awesome-list) |
| [joeseesun/qiaomu-design](https://github.com/joeseesun/qiaomu-design) | 577 | Claude Code设计顾问：反通用UI、风格试衣间、58个真实网站设计系统库 | [SAFE](https://agentskillshub.top/skill/joeseesun/qiaomu-design/?utm_source=github&utm_medium=awesome-list) |
| [codeswithroh/tastemaker](https://github.com/codeswithroh/tastemaker) | 444 | Claude Code skill，基于真实参考图和开发者持久化审美档案生成 UI，避免通用 AI 默认风格。 | [SAFE](https://agentskillshub.top/skill/codeswithroh/tastemaker/?utm_source=github&utm_medium=awesome-list) |
| [educlopez/ui-craft](https://github.com/educlopez/ui-craft) | 375 | 面向 AI 编程 agent 的设计工程系统——以精工级质量交付 UI。安装为 agent skill。 | [SAFE](https://agentskillshub.top/skill/educlopez/ui-craft/?utm_source=github&utm_medium=awesome-list) |
| [tasteskill/tasteskill](https://github.com/tasteskill/tasteskill) | 240 | 面向 AI Agent 的反低质前端框架 | [SAFE](https://agentskillshub.top/skill/tasteskill/tasteskill/?utm_source=github&utm_medium=awesome-list) |
| [mblode/agent-skills](https://github.com/mblode/agent-skills) | 144 | 没人会故意发布 AI 垃圾内容。这些 skill 确保你不会。 | [SAFE](https://agentskillshub.top/skill/mblode/agent-skills/?utm_source=github&utm_medium=awesome-list) |
| [funboy322/avoid-ai-design](https://github.com/funboy322/avoid-ai-design) | 100 | 审查并重写 AI 生成的前端，去除紫色渐变、奶油+陶土色和单色默认样式。附零依赖扫描器，是 avoid-ai-writing 的设计对应工具。 | [SAFE](https://agentskillshub.top/skill/funboy322/avoid-ai-design/?utm_source=github&utm_medium=awesome-list) |
| [Gesso-Build/skills](https://github.com/Gesso-Build/skills) | 91 | HTML/CSS 确定性设计审查：73 条专业设计师的生产级反粗糙规则，含精确检测器、幂等自动修复、反粗糙 skill 和 /gesso-critique 命… | [SAFE](https://agentskillshub.top/skill/Gesso-Build/skills/?utm_source=github&utm_medium=awesome-list) |
| [Laith0003/ux-skill](https://github.com/Laith0003/ux-skill) | 80 | Claude Code、Cursor、Windsurf 设计引擎：确定性反 AI-slop 检查器（152 条规则）；离线运行，不调用 LLM，MIT。 | [SAFE](https://agentskillshub.top/skill/Laith0003/ux-skill/?utm_source=github&utm_medium=awesome-list) |
| [h3nryprod01/design-taste](https://github.com/h3nryprod01/design-taste) | 70 | Claude Code / Cowork 的前端设计规范，涵盖字体、配色、动效、组件与反套路。 | [SAFE](https://agentskillshub.top/skill/h3nryprod01/design-taste/?utm_source=github&utm_medium=awesome-list) |
| [Mutakisa/game-slop-purge](https://github.com/Mutakisa/game-slop-purge) | 69 | 游戏 UI 清理 Agent Skill 2026：移除杂乱，保留趣味 | [SAFE](https://agentskillshub.top/skill/Mutakisa/game-slop-purge/?utm_source=github&utm_medium=awesome-list) |
| [phazurlabs/sumi](https://github.com/phazurlabs/sumi) | 54 | Sumi——Claude Code 的 UX/UI 设计知识库：43 个 skill、168 份参考、37 个命令，反低质设计并提供可审计引用链。使用 /su… | [SAFE](https://agentskillshub.top/skill/phazurlabs/sumi/?utm_source=github&utm_medium=awesome-list) |
| [stevembarclay/pencilplaybook](https://github.com/stevembarclay/pencilplaybook) | 50 | PencilPlaybook 是 Pencil.dev + Claude Code 的 UI Taste-Skill，结合感知心理学与资深设计约束，减少雷同… | [SAFE](https://agentskillshub.top/skill/stevembarclay/pencilplaybook/?utm_source=github&utm_medium=awesome-list) |
| [nghiahsgs/skills-slides](https://github.com/nghiahsgs/skills-slides) | 35 | 5万多个独特 HTML 演示设计。零依赖。拒绝 AI 垃圾风。Claude Code skill。 | [SAFE](https://agentskillshub.top/skill/nghiahsgs/skills-slides/?utm_source=github&utm_medium=awesome-list) |
| [sva-admin/sv-academy-prom-design](https://github.com/sva-admin/sv-academy-prom-design) | 29 | Claude Code、Cowork 和 Cursor 的设计风格。Prom 是泰语“准备好”的意思。免费学习：loop.sv-academy.org | [SAFE](https://agentskillshub.top/skill/sva-admin/sv-academy-prom-design/?utm_source=github&utm_medium=awesome-list) |
| [2389-research/landing-page-design](https://github.com/2389-research/landing-page-design) | 21 | 用 Vibe Discovery 流程和反 AI 套话原则创建视觉独特的落地页 | [SAFE](https://agentskillshub.top/skill/2389-research/landing-page-design/?utm_source=github&utm_medium=awesome-list) |
| [nickture/skills](https://github.com/nickture/skills) | 20 | Two Agent Skills that help an AI agent make an interface clear, consistent, easy to use and scalable, and Russian text clear and correct (English ver… | [SAFE](https://agentskillshub.top/skill/nickture/skills/?utm_source=github&utm_medium=awesome-list) |
| [Ferousco-dev/anti-slop-design](https://github.com/Ferousco-dev/anti-slop-design) | 14 | Claude Agent Skill，避免生成千篇一律的 AI 设计。 | [SAFE](https://agentskillshub.top/skill/Ferousco-dev/anti-slop-design/?utm_source=github&utm_medium=awesome-list) |
| [kmaida/deslop-skills](https://github.com/kmaida/deslop-skills) | 10 | 用于去除或避免 AI agent 生成的前端 UI 设计和文字内容中的低质内容的 skills。 | [SAFE](https://agentskillshub.top/skill/kmaida/deslop-skills/?utm_source=github&utm_medium=awesome-list) |
| [Hayatelin/taste-skill-zh-CN](https://github.com/Hayatelin/taste-skill-zh-CN) | 8 | Taste Skill 简体中文版——面向 AI agent 的反低质前端设计 skill | [SAFE](https://agentskillshub.top/skill/Hayatelin/taste-skill-zh-CN/?utm_source=github&utm_medium=awesome-list) |
| [kesslerio/ultimate-frontend-design-openclaw-skill](https://github.com/kesslerio/ultimate-frontend-design-openclaw-skill) | 8 | 使用 React、Tailwind、shadcn/ui 创建静态网站，无需设计稿。避免 AI 套路化设计，采用移动优先模式和单文件打包。 | [SAFE](https://agentskillshub.top/skill/kesslerio/ultimate-frontend-design-openclaw-skill/?utm_source=github&utm_medium=awesome-list) |
| [saidkaban/evalmedia](https://github.com/saidkaban/evalmedia) | 7 | 停止 AI 垃圾内容 | [SAFE](https://agentskillshub.top/skill/saidkaban/evalmedia/?utm_source=github&utm_medium=awesome-list) |
| [changemaner/design-taste-frontend](https://github.com/changemaner/design-taste-frontend) | 5 | 反低质前端设计 skill（通用前端设计+deck 模式），含30个真实品牌素材库、清单驱动的风格选择和质量检查关卡 | [SAFE](https://agentskillshub.top/skill/changemaner/design-taste-frontend/?utm_source=github&utm_medium=awesome-list) |
| [jferracini/anti-slop-os](https://github.com/jferracini/anti-slop-os) | 5 | anti-slop-os：运行在 AI agent 内的 Creative Director，检查生成的 UI，识别“AI 风格”。 | [SAFE](https://agentskillshub.top/skill/jferracini/anti-slop-os/?utm_source=github&utm_medium=awesome-list) |
| [local-over/Anti-Slop-UI](https://github.com/local-over/Anti-Slop-UI) | 5 | Anti-Slop UI：50层UI架构，约束AI编码助手构建规范界面，避免生成通用布局 | [SAFE](https://agentskillshub.top/skill/local-over/Anti-Slop-UI/?utm_source=github&utm_medium=awesome-list) |
| [mah-claude/anti-slop-website-prompts](https://github.com/mah-claude/anti-slop-website-prompts) | 5 | Meez（meez.design）的15个艺术指导网站构建提示词和反低质设计SKILL.md，适用于Lovable、Bolt、v0、Cursor和Claude… | [SAFE](https://agentskillshub.top/skill/mah-claude/anti-slop-website-prompts/?utm_source=github&utm_medium=awesome-list) |
| [rohunvora/anti-slop-library](https://github.com/rohunvora/anti-slop-library) | 5 | 防止 AI 生成低质氛围编程代码的 UI 参考库 | [SAFE](https://agentskillshub.top/skill/rohunvora/anti-slop-library/?utm_source=github&utm_medium=awesome-list) |

<a id="type-rules"></a>
## 📏 写作规则

[在在线页面打开这一类,按星数排序 →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-rules)

| 仓库 | 星数 | 做什么 | 安全评级 |
|---|---:|---|---|
| [hardikpandya/stop-slop](https://github.com/hardikpandya/stop-slop) | 17.9k | 去除文章中 AI 痕迹的 skill 文件 | [SAFE](https://agentskillshub.top/skill/hardikpandya/stop-slop/?utm_source=github&utm_medium=awesome-list) |
| [miqdadbadjuber/anti-slop](https://github.com/miqdadbadjuber/anti-slop) | 5.4k | AI 编程 agent 筛除通用 AI 生成的 UI 设计、文本和代码的规则。 | [SAFE](https://agentskillshub.top/skill/miqdadbadjuber/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer) | 1.9k | 去除论文和NSF/NIH基金申请中的AI写作痕迹，保持学术文风，让论断有据。适用于 Claude Code、Codex 和 MorphMind 的 skill | [SAFE](https://agentskillshub.top/skill/AIScientists-Dev/academic-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [alexgreensh/attention-span](https://github.com/alexgreensh/attention-span) | 1.4k | 让你的 agent 说人话。为 Claude Code、Codex 等提供 ADHD 友好的输出风格，关注内容而非 token。 | [SAFE](https://agentskillshub.top/skill/alexgreensh/attention-span/?utm_source=github&utm_medium=awesome-list) |
| [realrossmanngroup/no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules) | 696 | Claude Code 参考：用 Louis Rossmann 的口吻写作，避免 AI 垃圾。可移植的 CLAUDE.md 和 skills。 | [SAFE](https://agentskillshub.top/skill/realrossmanngroup/no_ai_slop_writing_rules/?utm_source=github&utm_medium=awesome-list) |
| [jalaalrd/anti-ai-slop-writing](https://github.com/jalaalrd/anti-ai-slop-writing) | 519 | 消除可检测 AI 模式的 AI 写作 skill，支持 Claude Code、Codex、Cursor、Gemini CLI 等 agent。 | [SAFE](https://agentskillshub.top/skill/jalaalrd/anti-ai-slop-writing/?utm_source=github&utm_medium=awesome-list) |
| [iKora128/stop-ai-slop-jp](https://github.com/iKora128/stop-ai-slop-jp) | 470 | 去除日语文章 AI 痕迹的 Claude skill | [SAFE](https://agentskillshub.top/skill/iKora128/stop-ai-slop-jp/?utm_source=github&utm_medium=awesome-list) |
| [stephenturner/skill-deslop](https://github.com/stephenturner/skill-deslop) | 409 | 去除科学写作中的 AI 痕迹 | [SAFE](https://agentskillshub.top/skill/stephenturner/skill-deslop/?utm_source=github&utm_medium=awesome-list) |
| [matsuikentaro1/humanizer_academic](https://github.com/matsuikentaro1/humanizer_academic) | 276 | 用于去除学术医学论文中 AI 生成痕迹的 Claude Code skill，使其更自然、专业。 | [SAFE](https://agentskillshub.top/skill/matsuikentaro1/humanizer_academic/?utm_source=github&utm_medium=awesome-list) |
| [gonta223/humanizer-ja](https://github.com/gonta223/humanizer-ja) | 152 | 将AI味日语改写成人类文章的Claude Code skill，含20种模式检查清单和改写指南。 | [SAFE](https://agentskillshub.top/skill/gonta223/humanizer-ja/?utm_source=github&utm_medium=awesome-list) |
| [adenaufal/anti-slop-writing](https://github.com/adenaufal/anti-slop-writing) | 146 | 让 AI 不再写得像 AI，消除常见 LLM 风格特征；适用于 Claude Code、Gemini CLI、Codex CLI、Copilot、Cursor… | [SAFE](https://agentskillshub.top/skill/adenaufal/anti-slop-writing/?utm_source=github&utm_medium=awesome-list) |
| [proffitteoy/Mathematician-Humanizer](https://github.com/proffitteoy/Mathematician-Humanizer) | 30 | 基于文体计量与参考文风分析的 AI 写作技能，让数学文字更清晰自然 | [SAFE](https://agentskillshub.top/skill/proffitteoy/Mathematician-Humanizer/?utm_source=github&utm_medium=awesome-list) |
| [adewale/anti-slop-writing](https://github.com/adewale/anti-slop-writing) | 18 | 用于编辑文稿，使其读起来不像通用 LLM 输出的 Agent Skill | [SAFE](https://agentskillshub.top/skill/adewale/anti-slop-writing/?utm_source=github&utm_medium=awesome-list) |
| [haidrrrry/humanize-ai-writing](https://github.com/haidrrrry/humanize-ai-writing) | 16 | 反 AI 套话 system prompt 和 skill，让 ChatGPT、Claude、Gemini、Grok、Kimi 写得像人，禁用常见 AI 话术。 | [SAFE](https://agentskillshub.top/skill/haidrrrry/humanize-ai-writing/?utm_source=github&utm_medium=awesome-list) |
| [jiutianxvanyin/humanizer-formal](https://github.com/jiutianxvanyin/humanizer-formal) | 11 | 降低商务和学术文本的 AI 生成感，适用于中英文。 | [SAFE](https://agentskillshub.top/skill/jiutianxvanyin/humanizer-formal/?utm_source=github&utm_medium=awesome-list) |
| [impactcrew/dont-be-a-sloperator](https://github.com/impactcrew/dont-be-a-sloperator) | 10 | 别做 sloperator。十条基于原则而非禁词的规则，让 AI 不再像 AI。附 /work skill，要求输出前思考。支持 Claude Code、Ch… | [SAFE](https://agentskillshub.top/skill/impactcrew/dont-be-a-sloperator/?utm_source=github&utm_medium=awesome-list) |
| [AMishradev/outbound-writing](https://github.com/AMishradev/outbound-writing) | 6 | 去除冷邮件中 AI 痕迹的 Claude Code skill，面向技术人员的创业公司外联反套话工具 | [SAFE](https://agentskillshub.top/skill/AMishradev/outbound-writing/?utm_source=github&utm_medium=awesome-list) |
| [Dexxter182/humanizer-hu](https://github.com/Dexxter182/humanizer-hu) | 5 | 匈牙利语写作 skill：让 agent 输出不像 AI，含26个示例、文档级决策和无 LLM lint，支持 Claude Code、Codex、Curso… | [SAFE](https://agentskillshub.top/skill/Dexxter182/humanizer-hu/?utm_source=github&utm_medium=awesome-list) |
| [barbodshafiee0012-hash/student-exam-skill](https://github.com/barbodshafiee0012-hash/student-exam-skill) | 5 | 一个 Claude skill，像大学生一样回答考试问题，简洁自然，参考伊朗大学教材，只给答案。 | [SAFE](https://agentskillshub.top/skill/barbodshafiee0012-hash/student-exam-skill/?utm_source=github&utm_medium=awesome-list) |
| [nakashimatakaya/deslop-ja](https://github.com/nakashimatakaya/deslop-ja) | 5 | 用于发现并修正 AI 生成日语风格的 Claude Code / Codex / claude.ai skill，支持临床研究论文模式。 | [SAFE](https://agentskillshub.top/skill/nakashimatakaya/deslop-ja/?utm_source=github&utm_medium=awesome-list) |

**安全评级**是 Agent Skills Hub 对仓库 README 和安装步骤的评级。*待评级*表示目录还没评到它。

预览图是各项目 README 里图片的缩小副本,只收录采用宽松许可证的项目,版权归原作者所有。来源和许可证见 [assets/previews/NOTICE.md](assets/previews/NOTICE.md)。如需移除请提 issue。

## 相关合集

- [zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills), [zhuyansen/awesome-codex-ppt-skills](https://github.com/zhuyansen/awesome-codex-ppt-skills) —— 同样做法的合集。

## 推荐仓库

提一个 issue 附上 GitHub 链接。它会走和每个条目一样的评审;决定上不上榜的是上面的规则,不是星数。

---

机器可读版本:[`data/skills.json`](data/skills.json)。生成于 2026-10-09。
