# Awesome Humanizer Skills

[中文](README.zh-CN.md)

Open-source **humanizer and anti-slop skills**: make AI-written text, code and UI read like a person made it, detect AI tells, and keep agents to a house style. English and Chinese. 108 repos, each one read and security-graded by [Agent Skills Hub](https://agentskillshub.top?utm_source=github&utm_medium=awesome-list).

Live page with filters: **[https://agentskillshub.top/best/anti-slop/](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list)** · refreshed every 8 hours

## What these skills do

<table>
<tr>
<td align="center" valign="top" width="33%"><b>✍️ Writing humanizers</b><br><sub>25 repos</sub><br><br><sub>Rewrite AI prose so it reads human.</sub><br><a href="#type-writing"><b>View the list →</b></a></td>
<td align="center" valign="top" width="33%"><b>🔍 Slop detectors</b><br><sub>37 repos</sub><br><br><sub>Find and score AI writing patterns.</sub><br><a href="#type-detector"><b>View the list →</b></a></td>
<td align="center" valign="top" width="33%"><b>🀄 Chinese text</b><br><sub>17 repos</sub><br><br><sub>Take the AI flavour out of Chinese writing.</sub><br><a href="#type-chinese"><b>View the list →</b></a></td>
</tr>
<tr>
<td align="center" valign="top" width="33%"><b>🧹 Code cleanup</b><br><sub>2 repos</sub><br><br><sub>Clean AI patterns out of code and comments.</sub><br><a href="#type-code"><b>View the list →</b></a></td>
<td align="center" valign="top" width="33%"><b>🎨 UI & design taste</b><br><sub>16 repos</sub><br><br><sub>Steer AI-made UI away from the generic AI look.</sub><br><a href="#type-design"><b>View the list →</b></a></td>
<td align="center" valign="top" width="33%"><b>📏 Style rules</b><br><sub>11 repos</sub><br><br><sub>Style guides and word lists agents follow.</sub><br><a href="#type-rules"><b>View the list →</b></a></td>
</tr>
</table>

## Contents

- [✍️ Writing humanizers](#type-writing) (25)
- [🔍 Slop detectors](#type-detector) (37)
- [🀄 Chinese text](#type-chinese) (17)
- [🧹 Code cleanup](#type-code) (2)
- [🎨 UI & design taste](#type-design) (16)
- [📏 Style rules](#type-rules) (11)

## How a repo gets on the list

1. It makes AI-made output read as if a person made it, or detects or removes AI patterns in text, code or design. A general writing assistant or grammar checker does not count.
2. It is software someone can install or run, not a list of links or a placeholder.
3. It has a README. Without one it cannot be graded.
4. At 50 stars or more it is listed on topic alone. Under 50 it must also clear a README quality bar (shows it working, one-command start, a concrete outcome, complete docs), and have 5 stars.

The questions are answered by a decision model reading each README, not by hand. A repo near a cut-off can land on either side; open an issue if one is misfiled.

<a id="type-writing"></a>
## ✍️ Writing humanizers

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-writing)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [blader/humanizer](https://github.com/blader/humanizer) | 53.7k | Agent skill that removes signs of AI-generated writing from text | [SAFE](https://agentskillshub.top/skill/blader/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [lynote-ai/humanize-text](https://github.com/lynote-ai/humanize-text) | 3.2k | Open-source text humanization pipeline with every intermediate step published. Two LLM rewrites at temp 1.3, then two hops across different NMT engin… | [SAFE](https://agentskillshub.top/skill/lynote-ai/humanize-text/?utm_source=github&utm_medium=awesome-list) |
| [Nanako0129/sepia](https://github.com/Nanako0129/sepia) | 2.9k | De-AI writing skill for any Agent Skills-compatible agent (77+ via the Skills CLI), with native plugins for Claude Code, Codex, Grok Build, and Antig… | [SAFE](https://agentskillshub.top/skill/Nanako0129/sepia/?utm_source=github&utm_medium=awesome-list) |
| [iniwap/AIWriteX](https://github.com/iniwap/AIWriteX) | 2.0k | AIWriteX - 微信公众号全自动AI工具：全网热搜舆情聚合+趋势分析+爆款选题+文章采集+一键生成排版发布 \| AI自动配图 \| 去AI味、过朱雀检测 \| 支持小红书/百家号/头条等多平台 \| 洗稿润色支持多账号 \| 专家赛道 \| 小绿书贴图 \| 短视频文案 \| 手机控制 \… | [SAFE](https://agentskillshub.top/skill/iniwap/AIWriteX/?utm_source=github&utm_medium=awesome-list) |
| [harshaneel/humanize](https://github.com/harshaneel/humanize) | 512 | Best static AI text humanizer. Two research-grounded LLM-agnostic skills that make AI writing sound human and relatable. Nine levers, 50+ peer-review… | [SAFE](https://agentskillshub.top/skill/harshaneel/humanize/?utm_source=github&utm_medium=awesome-list) |
| [devswha/patina](https://github.com/devswha/patina) | 362 | AI-writing humanizer for KO/EN/ZH/JA | [SAFE](https://agentskillshub.top/skill/devswha/patina/?utm_source=github&utm_medium=awesome-list) |
| [NulightJens/humanizer-stack](https://github.com/NulightJens/humanizer-stack) | 315 | Two-pass pipeline for removing AI writing tells from outward-facing text: a surface pass plus a structural pass grounded in the StoryScope study. Pac… | [SAFE](https://agentskillshub.top/skill/NulightJens/humanizer-stack/?utm_source=github&utm_medium=awesome-list) |
| [MohamedAbdallah-14/unslop](https://github.com/MohamedAbdallah-14/unslop) | 152 | Make AI output sound human. Strips AI-isms (sycophancy, stock vocab, hedging stacks, em-dash pileups), preserves code/URLs/headings. Plugin for Claud… | [SAFE](https://agentskillshub.top/skill/MohamedAbdallah-14/unslop/?utm_source=github&utm_medium=awesome-list) |
| [rudra496/StealthHumanizer](https://github.com/rudra496/StealthHumanizer) | 150 | 🔓 Free open-source AI text humanizer — bypass GPTZero, Turnitin & AI detectors with 16+ Languages support. 35 providers, 4 rewrite levels, 6 Writing… | [SAFE](https://agentskillshub.top/skill/rudra496/StealthHumanizer/?utm_source=github&utm_medium=awesome-list) |
| [sergebulaev/x-skills](https://github.com/sergebulaev/x-skills) | 115 | X (Twitter) marketing skills for Claude Code and Codex: write tweets, threads, and replies in your voice, strip AI tells, and publish via Publora. Op… | [SAFE](https://agentskillshub.top/skill/sergebulaev/x-skills/?utm_source=github&utm_medium=awesome-list) |
| [bushrabeg/turkce-humanizer](https://github.com/bushrabeg/turkce-humanizer) | 81 | Türkçe metinlerden yapay zekâ yazım imzalarını temizleyen Claude skill'i. YZ üretimi Türkçe'yi doğal, insan-sesli Türkçe'ye dönüştürür. \| A Claude s… | [SAFE](https://agentskillshub.top/skill/bushrabeg/turkce-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [thevseprod/humanizer-ru](https://github.com/thevseprod/humanizer-ru) | 42 | Make AI text sound human - rules + a Claude Code skill, built for Russian, works for English too. | [SAFE](https://agentskillshub.top/skill/thevseprod/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [dotoricode/korean-humanizer](https://github.com/dotoricode/korean-humanizer) | 14 | Korean humanizer prompt and skill for removing the usual AI smell from generated writing. | [SAFE](https://agentskillshub.top/skill/dotoricode/korean-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [msdanyg/humanize-pro](https://github.com/msdanyg/humanize-pro) | 13 | Claude skill that goes past word-list humanizers: strips the full catalog of AI tells, refits the text to its channel (LinkedIn, X, cold email, Slack… | [SAFE](https://agentskillshub.top/skill/msdanyg/humanize-pro/?utm_source=github&utm_medium=awesome-list) |
| [machinemade-mm/humanmade-antislop](https://github.com/machinemade-mm/humanmade-antislop) | 11 | Anti-AI slop scientific writing skill for Claude Code. Or: Scientific writing with a human voice. | [SAFE](https://agentskillshub.top/skill/machinemade-mm/humanmade-antislop/?utm_source=github&utm_medium=awesome-list) |
| [walterwritesai/walter-skills](https://github.com/walterwritesai/walter-skills) | 11 | Free Claude skills for SEO content: AI humanizer, AI detection bypass, keyword preservation, agency QC, local SEO, programmatic SEO, content repurpos… | [SAFE](https://agentskillshub.top/skill/walterwritesai/walter-skills/?utm_source=github&utm_medium=awesome-list) |
| [timolabs-ai/claude-humanize-skill](https://github.com/timolabs-ai/claude-humanize-skill) | 9 | Claude Code skill (/humanize). Strips AI writing patterns from content via five editorial layers: vocabulary, sentence shape, bullet rhythm, paragrap… | [SAFE](https://agentskillshub.top/skill/timolabs-ai/claude-humanize-skill/?utm_source=github&utm_medium=awesome-list) |
| [KondrashovDenis/claude-humanizer-ru-skill](https://github.com/KondrashovDenis/claude-humanizer-ru-skill) | 8 | Claude Code skill для чистки русских текстов от AI-штампов. Адаптация blader/humanizer: канцелярит, кальки, раздутая значимость + типографическая дег… | [SAFE](https://agentskillshub.top/skill/KondrashovDenis/claude-humanizer-ru-skill/?utm_source=github&utm_medium=awesome-list) |
| [aeopress/writing-skills.TW](https://github.com/aeopress/writing-skills.TW) | 7 | 繁體中文寫作 skill 工具鏈 for Claude Code：humanizer-tw（去 AI 味）+ good-writing-zh（節奏打磨：PG／余光中／王鼎鈞 + 技術文件保守模式）+ fable-econ／fable-explore（Amanda Askell 寓言式概念學習） | [SAFE](https://agentskillshub.top/skill/aeopress/writing-skills.TW/?utm_source=github&utm_medium=awesome-list) |
| [ferr079/humanizer-fr](https://github.com/ferr079/humanizer-fr) | 7 | Fork français du skill Claude Code « humanizer » (blader/humanizer, MIT) — 33 motifs d'écriture IA adaptés au français | [SAFE](https://agentskillshub.top/skill/ferr079/humanizer-fr/?utm_source=github&utm_medium=awesome-list) |
| [daniel-bogale/anti-ai-writing-humanizer](https://github.com/daniel-bogale/anti-ai-writing-humanizer) | 5 | Humanize AI-written text — a portable agent skill that writes or rewrites prose to remove AI tells. Works in Claude Code, Cursor, Codex, OpenClaw. | [SAFE](https://agentskillshub.top/skill/daniel-bogale/anti-ai-writing-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [durmazoguzhan/turkish-humanify](https://github.com/durmazoguzhan/turkish-humanify) | 5 | Turkish humanizer skill for Claude and Claude Code. Rewrites AI-sounding Turkish into Turkish a person would have written: native sentence architectu… | [SAFE](https://agentskillshub.top/skill/durmazoguzhan/turkish-humanify/?utm_source=github&utm_medium=awesome-list) |
| [humanizer-tools/slop-humanizer](https://github.com/humanizer-tools/slop-humanizer) | 5 | A Claude skill that strips AI writing patterns and rewrites text to sound human. Synthesized from 8 humanizer repos. | [SAFE](https://agentskillshub.top/skill/humanizer-tools/slop-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [matsutouya/humanizer-ja](https://github.com/matsutouya/humanizer-ja) | 5 | Claude Code skill that removes signs of AI-generated writing from Japanese text | [SAFE](https://agentskillshub.top/skill/matsutouya/humanizer-ja/?utm_source=github&utm_medium=awesome-list) |
| [rephrasyai/rephrasy-skills](https://github.com/rephrasyai/rephrasy-skills) | 5 | Free content skills for AI agents. Humanize AI text, keep your keywords intact, ship agency-quality drafts. Free, MIT, works across Claude Code, Code… | [SAFE](https://agentskillshub.top/skill/rephrasyai/rephrasy-skills/?utm_source=github&utm_medium=awesome-list) |

<a id="type-detector"></a>
## 🔍 Slop detectors

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-detector)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [epoko77-ai/im-not-ai](https://github.com/epoko77-ai/im-not-ai) | 5.8k | AI가 쓴 한글을 사람 글처럼 윤문하는 Claude 스킬 — Korean AI-text humanizer: detects and rewrites translationese, mechanical parallelism, and 71 other AI tells | [SAFE](https://agentskillshub.top/skill/epoko77-ai/im-not-ai/?utm_source=github&utm_medium=awesome-list) |
| [dmmulroy/anti-slop](https://github.com/dmmulroy/anti-slop) | 5.1k | Opinionated Oxlint rules for rejecting low-evidence TypeScript and JavaScript patterns | [SAFE](https://agentskillshub.top/skill/dmmulroy/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [conorbronsdon/avoid-ai-writing](https://github.com/conorbronsdon/avoid-ai-writing) | 4.8k | Skill that audits and rewrites content to remove AI writing patterns. Use it with your favorite agents including Claude Code, OpenClaw, Codex, and He… | [SAFE](https://agentskillshub.top/skill/conorbronsdon/avoid-ai-writing/?utm_source=github&utm_medium=awesome-list) |
| [Jakeschincariol/linkedin-agent-skill](https://github.com/Jakeschincariol/linkedin-agent-skill) | 1.1k | Eleven free Claude skills that run a LinkedIn account: posts off 21 hook formulas, comments, replies, profile score, weekly plan, and a humanizer tha… | [SAFE](https://agentskillshub.top/skill/Jakeschincariol/linkedin-agent-skill/?utm_source=github&utm_medium=awesome-list) |
| [theclaymethod/unslop](https://github.com/theclaymethod/unslop) | 498 | An agent skill to de-AI your writing | [SAFE](https://agentskillshub.top/skill/theclaymethod/unslop/?utm_source=github&utm_medium=awesome-list) |
| [ilyautov/humanizer-ru](https://github.com/ilyautov/humanizer-ru) | 406 | humanizer-ru: редактура русского текста для AI-агентов. Убирает канцелярит и шаблонные обороты, сверяет смысл и факты. 67 признаков, 21 жёсткий запре… | [SAFE](https://agentskillshub.top/skill/ilyautov/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [Aboudjem/humanizer-skill](https://github.com/Aboudjem/humanizer-skill) | 263 | Free, open-source AI writing humanizer and detector. 55 patterns, 5 voices, a 0-100 AI-tell score, and nothing leaves your machine. | [SAFE](https://agentskillshub.top/skill/Aboudjem/humanizer-skill/?utm_source=github&utm_medium=awesome-list) |
| [talkstream/ru-text](https://github.com/talkstream/ru-text) | 245 | Russian text quality for AI agents — neuroslop cleanup, typography, information style, editorial standards, UX writing, business correspondence. Scor… | [SAFE](https://agentskillshub.top/skill/talkstream/ru-text/?utm_source=github&utm_medium=awesome-list) |
| [seyedehsanhadi/sloptrim](https://github.com/seyedehsanhadi/sloptrim) | 211 | A local detector for AI-writing patterns. Scores every prose file your agent saves. Python standard library only, no network, no model. | [SAFE](https://agentskillshub.top/skill/seyedehsanhadi/sloptrim/?utm_source=github&utm_medium=awesome-list) |
| [smixs/humanizer-ru](https://github.com/smixs/humanizer-ru) | 185 | Skill для AI-агентов (Claude Code, Codex, OpenClaw, Hermes): убирает 37 признаков AI-генерации из русского текста и проверяет, писала ли его нейросет… | [SAFE](https://agentskillshub.top/skill/smixs/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [marmbiz/humanizer-de](https://github.com/marmbiz/humanizer-de) | 169 | Deutscher Text-Humanizer für Claude Code & Codex. Redigiert KI-Floskeln, schützt deine Schreibstimme und prüft 72 deutsche Muster quellentreu. | [SAFE](https://agentskillshub.top/skill/marmbiz/humanizer-de/?utm_source=github&utm_medium=awesome-list) |
| [eric-tramel/slop-guard](https://github.com/eric-tramel/slop-guard) | 164 | Slop Scoring to Stop Slop | [SAFE](https://agentskillshub.top/skill/eric-tramel/slop-guard/?utm_source=github&utm_medium=awesome-list) |
| [Heyosseus/sloppy](https://github.com/Heyosseus/sloppy) | 145 | Static analysis for the debt AI agents leave in PHP: 26 rules, Claude Code hooks, git-diff review, a Rector and Pint fix pass, Pest expectations, CI… | [SAFE](https://agentskillshub.top/skill/Heyosseus/sloppy/?utm_source=github&utm_medium=awesome-list) |
| [Akimiya-z/codex-guard](https://github.com/Akimiya-z/codex-guard) | 138 | Quality gate for AI/Codex-generated pull requests: blocks TODO leftovers, leaked secrets, sloppy commits and red CI before they reach main. | [SAFE](https://agentskillshub.top/skill/Akimiya-z/codex-guard/?utm_source=github&utm_medium=awesome-list) |
| [manavmishra/ZeroSlop](https://github.com/manavmishra/ZeroSlop) | 130 | Open-source Agent Skill that finds and removes AI slop from your writing | [SAFE](https://agentskillshub.top/skill/manavmishra/ZeroSlop/?utm_source=github&utm_medium=awesome-list) |
| [Vladimir-Human/humanizer-ru](https://github.com/Vladimir-Human/humanizer-ru) | 126 | Проверяемая гигиена вставки из чата для русского текста | [SAFE](https://agentskillshub.top/skill/Vladimir-Human/humanizer-ru/?utm_source=github&utm_medium=awesome-list) |
| [tbhb/vale-ai-tells](https://github.com/tbhb/vale-ai-tells) | 115 | In today's rapidly evolving landscape, vale-ai-tells is a comprehensive, cutting-edge Vale style package that empowers writers to seamlessly delve in… | [SAFE](https://agentskillshub.top/skill/tbhb/vale-ai-tells/?utm_source=github&utm_medium=awesome-list) |
| [Nopon-Knowledge/huawei-cup-modeling-skill](https://github.com/Nopon-Knowledge/huawei-cup-modeling-skill) | 99 | 论文去 AI 味 · AI 痕迹检测 · 学术润色｜面向华为杯中国研究生数学建模竞赛的 Codex Skill，支持逐句诊断、去模板化改写、图表优化、规则核验与提交审计，保留研究事实与引文。 | [SAFE](https://agentskillshub.top/skill/Nopon-Knowledge/huawei-cup-modeling-skill/?utm_source=github&utm_medium=awesome-list) |
| [misbahsy/anti-ai-slop](https://github.com/misbahsy/anti-ai-slop) | 95 | An agent skill with multiple gates to check and to remove any AI slop. Use it with codex/claude code or any of your favorite AI tools. | [SAFE](https://agentskillshub.top/skill/misbahsy/anti-ai-slop/?utm_source=github&utm_medium=awesome-list) |
| [airlock-hq/airlock](https://github.com/airlock-hq/airlock) | 86 | All slop must die. Airlock is where every git push turns into a slop-free PR. | [SAFE](https://agentskillshub.top/skill/airlock-hq/airlock/?utm_source=github&utm_medium=awesome-list) |
| [apurvrdx1/tagore](https://github.com/apurvrdx1/tagore) | 54 | Make AI-generated prose sound human. 29-pattern catalog + 8-rule operating system + 8-dimension scoring rubric. Works with Claude Code, OpenCode, Cop… | [SAFE](https://agentskillshub.top/skill/apurvrdx1/tagore/?utm_source=github&utm_medium=awesome-list) |
| [ilien-dev/quiron](https://github.com/ilien-dev/quiron) | 53 | AI humanizer skill for Claude Code, Codex and Cursor. Removes AI slop and the signs of AI writing, then measures the rewrite against human baselines. | [SAFE](https://agentskillshub.top/skill/ilien-dev/quiron/?utm_source=github&utm_medium=awesome-list) |
| [humanizerai/agent-skills](https://github.com/humanizerai/agent-skills) | 49 | HumanizerAI Agent Skills for Claude Code and Codex - AI detection and text humanization | [SAFE](https://agentskillshub.top/skill/humanizerai/agent-skills/?utm_source=github&utm_medium=awesome-list) |
| [pablocaeg/sloptotal](https://github.com/pablocaeg/sloptotal) | 48 | Open-source AI text detector and ChatGPT detector: 23 engines, one calibrated score, every number measured. CLI, MCP server and GitHub Action. Self-h… | [SAFE](https://agentskillshub.top/skill/pablocaeg/sloptotal/?utm_source=github&utm_medium=awesome-list) |
| [dripips/plain-prose](https://github.com/dripips/plain-prose) | 25 | Agent skill that removes AI writing patterns from English, Russian and German prose. Merges stop-slop and avoid-ai-writing, adds a zero-dependency ch… | [SAFE](https://agentskillshub.top/skill/dripips/plain-prose/?utm_source=github&utm_medium=awesome-list) |
| [vstorm-co/content-skills](https://github.com/vstorm-co/content-skills) | 24 | Content studio skill pack for coding agents — blog, social, slides, video, infographics — all brand-aware with built-in anti-slop. Works with Claude… | [SAFE](https://agentskillshub.top/skill/vstorm-co/content-skills/?utm_source=github&utm_medium=awesome-list) |
| [allanta8/slop-check](https://github.com/allanta8/slop-check) | 19 | Anti-slop content audit skill for X, ViewFT, LinkedIn, and long-form posts. | [SAFE](https://agentskillshub.top/skill/allanta8/slop-check/?utm_source=github&utm_medium=awesome-list) |
| [skyzer/deslop-the-copy](https://github.com/skyzer/deslop-the-copy) | 12 | Portable Agent Skill that removes AI writing patterns while preserving the writer voice. Works with Claude Code, Codex, OpenClaw, Cursor, and more. | [SAFE](https://agentskillshub.top/skill/skyzer/deslop-the-copy/?utm_source=github&utm_medium=awesome-list) |
| [0xNyk/unmachined](https://github.com/0xNyk/unmachined) | 10 | Anti-AI-slop agent skill: makes text read written and UI look made, not generated. Deterministic scanners + severity-tiered tell catalogs. | [SAFE](https://agentskillshub.top/skill/0xNyk/unmachined/?utm_source=github&utm_medium=awesome-list) |
| [tomerose/stop-slop](https://github.com/tomerose/stop-slop) | 10 | 去AI味写作技能 — 5维评分体系，检测41种AI反模式。让 Claude/Cursor/Copilot 写出人话。Claude Code Skill，支持中英文。 | [SAFE](https://agentskillshub.top/skill/tomerose/stop-slop/?utm_source=github&utm_medium=awesome-list) |
| [aplaceforallmystuff/claude-slop-detector](https://github.com/aplaceforallmystuff/claude-slop-detector) | 9 | Claude Code skill for detecting AI-generated writing patterns (slop) in content | [SAFE](https://agentskillshub.top/skill/aplaceforallmystuff/claude-slop-detector/?utm_source=github&utm_medium=awesome-list) |
| [Aaron-Bushnell/humanizer](https://github.com/Aaron-Bushnell/humanizer) | 8 | Detect 47 AI writing patterns and rewrite text in 5 human voice profiles. A Claude Code skill backed by ICML 2025 research on token-probability distr… | [SAFE](https://agentskillshub.top/skill/Aaron-Bushnell/humanizer/?utm_source=github&utm_medium=awesome-list) |
| [puneethkotha/humanizer-workbench](https://github.com/puneethkotha/humanizer-workbench) | 8 | AI humanizer: CLI tool and Claude Code skill for rewriting AI-generated text into natural human writing. | [SAFE](https://agentskillshub.top/skill/puneethkotha/humanizer-workbench/?utm_source=github&utm_medium=awesome-list) |
| [theserverlessdev/wsc](https://github.com/theserverlessdev/wsc) | 8 | Prose linter + AI-slop detector: weasel words, passive voice, hedging, and 190+ research-cited AI tells. Web editor, API, MCP server, CLI, GitHub Act… | [SAFE](https://agentskillshub.top/skill/theserverlessdev/wsc/?utm_source=github&utm_medium=awesome-list) |
| [forint573/human-copywrite](https://github.com/forint573/human-copywrite) | 7 | A Claude Agent Skill that humanizes AI-written marketing and long-form copy: landing pages, sales pages, e-books, case studies, founder notes. Remove… | [SAFE](https://agentskillshub.top/skill/forint573/human-copywrite/?utm_source=github&utm_medium=awesome-list) |
| [LanNguyenSi/agent-dx](https://github.com/LanNguyenSi/agent-dx) | 6 | Monorepo workshop for agent-development tooling: orchestrator-workflow and okf-kit ship on npm; slop-detector is the AI-slop linter for PRs. | [SAFE](https://agentskillshub.top/skill/LanNguyenSi/agent-dx/?utm_source=github&utm_medium=awesome-list) |
| [lokicik/novel-idea-hunter](https://github.com/lokicik/novel-idea-hunter) | 6 | Evidence-first, anti-slop opportunity discovery skill for coding agents (Claude Code + Codex) | [SAFE](https://agentskillshub.top/skill/lokicik/novel-idea-hunter/?utm_source=github&utm_medium=awesome-list) |

<a id="type-chinese"></a>
## 🀄 Chinese text

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-chinese)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [op7418/Humanizer-zh](https://github.com/op7418/Humanizer-zh) | 18.9k | Humanizer 的汉化版本，Claude Code Skills，旨在消除文本中 AI 生成的痕迹。 | [SAFE](https://agentskillshub.top/skill/op7418/Humanizer-zh/?utm_source=github&utm_medium=awesome-list) |
| [MrGeDiao/shuorenhua](https://github.com/MrGeDiao/shuorenhua) | 2.0k | 说人话｜中文优先的去 AI 味改写 skill：保事实、分场景、改完可直接发。Chinese-first rewrite skill for Codex / Claude Code / Cursor / ChatGPT — removes AI tone, preserves facts. | [SAFE](https://agentskillshub.top/skill/MrGeDiao/shuorenhua/?utm_source=github&utm_medium=awesome-list) |
| [Raymondhou0917/speak-human-tw](https://github.com/Raymondhou0917/speak-human-tw) | 1.0k | 「說人話」：繁體中文的去 AI 味改寫 skill。抓 38 種 AI 寫作痕跡，順手校正中國用語與半形標點，給 Claude Code / Codex / Cursor 用。 | [SAFE](https://agentskillshub.top/skill/Raymondhou0917/speak-human-tw/?utm_source=github&utm_medium=awesome-list) |
| [LifelongLazyLearner/qu-ai-wei](https://github.com/LifelongLazyLearner/qu-ai-wei) | 621 | 去 AI 味：去除简体中文 AI 写作痕迹 / Chinese humanizer skill | [SAFE](https://agentskillshub.top/skill/LifelongLazyLearner/qu-ai-wei/?utm_source=github&utm_medium=awesome-list) |
| [Hyacehila/humanizer-zh-next](https://github.com/Hyacehila/humanizer-zh-next) | 163 | 去除中文文本中 AI 写作痕迹的 Agent Skill（基于 blader/humanizer 与 op7418/humanizer-zh） | [SAFE](https://agentskillshub.top/skill/Hyacehila/humanizer-zh-next/?utm_source=github&utm_medium=awesome-list) |
| [mengke-wang/zh-humanizer-literary](https://github.com/mengke-wang/zh-humanizer-literary) | 86 | 中文去 AI 味与文采增强 Codex Skill，汲取 Mengke / 好事风格，让中文草稿更像人写。 | [SAFE](https://agentskillshub.top/skill/mengke-wang/zh-humanizer-literary/?utm_source=github&utm_medium=awesome-list) |
| [baibanbao/qu-ai-wei](https://github.com/baibanbao/qu-ai-wei) | 64 | 去 AI 味：中文写作的 AI 痕迹清理 skill。合并三家规则（含语料实测），并裁决它们互相矛盾的七处。A Claude skill for stripping AI tells from Chinese drafts. | [SAFE](https://agentskillshub.top/skill/baibanbao/qu-ai-wei/?utm_source=github&utm_medium=awesome-list) |
| [allenloves/de-ai-tone](https://github.com/allenloves/de-ai-tone) | 63 | 去 AI 味：繁體中文寫作與翻譯的風格規範（Claude Code skill） | [SAFE](https://agentskillshub.top/skill/allenloves/de-ai-tone/?utm_source=github&utm_medium=awesome-list) |
| [cangtianhuang/humanizer-academic-zh](https://github.com/cangtianhuang/humanizer-academic-zh) | 62 | Humanizer 中文学术版本，Claude Code Skills/ System Prompt，轻量级中文学术论文去 AI 痕迹提示词——运行迅速，节约 token，开箱即用！ | [SAFE](https://agentskillshub.top/skill/cangtianhuang/humanizer-academic-zh/?utm_source=github&utm_medium=awesome-list) |
| [pencil20388-eng/stop-slop-zh](https://github.com/pencil20388-eng/stop-slop-zh) | 49 | 🚫 Stop AI slop in Chinese writing. 干掉中文 AI 味 — banned words, punctuation rules, structure constraints & 4-layer QA. Works with Claude Code, Cursor, C… | [SAFE](https://agentskillshub.top/skill/pencil20388-eng/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [swaylq/humanize-chinese](https://github.com/swaylq/humanize-chinese) | 24 | 中文 AI 文本去痕迹 + Claude 水印检查 — 六段式改写；零宽字符、同形字清干净，SynthID 采样水印只量残留、不声称能删。纯 Python 本地跑，零 LLM 零 API Key。Chinese AI-text humanizer & Claude / SynthID waterm… | [SAFE](https://agentskillshub.top/skill/swaylq/humanize-chinese/?utm_source=github&utm_medium=awesome-list) |
| [leeguooooo/stop-slop-zh](https://github.com/leeguooooo/stop-slop-zh) | 11 | 消除中文 AI 写作痕迹的 Claude Skill：拆排比三件套、去名词化、换抽象主语为具体细节。灵感来自 hardikpandya/stop-slop。 | [SAFE](https://agentskillshub.top/skill/leeguooooo/stop-slop-zh/?utm_source=github&utm_medium=awesome-list) |
| [nagameTW/formosa-humanizer](https://github.com/nagameTW/formosa-humanizer) | 8 | blader/humanizer 的繁中版，讓 AI 生成的中文內容看起來更像人寫的。含中國用語偵測和中文標點規則等 49 種模式，支援 Claude Code、Codex 等 Agent | [SAFE](https://agentskillshub.top/skill/nagameTW/formosa-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [Zeng-xiangkai/humanizer-document-zh](https://github.com/Zeng-xiangkai/humanizer-document-zh) | 7 | 一个 Claude Code Skill，用于识别并移除 LLM 生成论文的典型痕迹。基于知乎高赞回答（最高 757 赞）、Wikipedia "Signs of AI writing" 等来源，总结了 **28 种常见 AI 写作模式**，配合四层自检体系，系统性地去除"AI 味"。 | [SAFE](https://agentskillshub.top/skill/Zeng-xiangkai/humanizer-document-zh/?utm_source=github&utm_medium=awesome-list) |
| [M1kasaYU/paper-expression-editor-skill](https://github.com/M1kasaYU/paper-expression-editor-skill) | 5 | 论文去AI化表述（论文去AI味、学术论文润色）：面向中文论文与开题报告的表达评阅和去模板化改写 \| Chinese academic writing editor for Codex | [SAFE](https://agentskillshub.top/skill/M1kasaYU/paper-expression-editor-skill/?utm_source=github&utm_medium=awesome-list) |
| [evoworkAI/xiaoci-skill](https://github.com/evoworkAI/xiaoci-skill) | 5 | 消磁 · 中文去 AI 味 skill：用密度门限和反向清单，替代流行的 AI 味特征清单 | [SAFE](https://agentskillshub.top/skill/evoworkAI/xiaoci-skill/?utm_source=github&utm_medium=awesome-list) |
| [win4r/jev-humanize-writing](https://github.com/win4r/jev-humanize-writing) | 5 | Jev 辅助去 AI 味写作：保留事实、归因与作者语气 \| Natural prose editing with Jev-assisted fidelity review | [SAFE](https://agentskillshub.top/skill/win4r/jev-humanize-writing/?utm_source=github&utm_medium=awesome-list) |

<a id="type-code"></a>
## 🧹 Code cleanup

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-code)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [MrZoyo/deslop-GPT](https://github.com/MrZoyo/deslop-GPT) | 136 | Deletion-first Agent Skill for removing test bloat, verification theater, and speculative fallbacks while preserving behavior. | [SAFE](https://agentskillshub.top/skill/MrZoyo/deslop-GPT/?utm_source=github&utm_medium=awesome-list) |
| [LeonardNJU/code-humanizer](https://github.com/LeonardNJU/code-humanizer) | 68 | humanizer, but for code — an agent skill that removes AI-generated code slop: duplicated helpers, try-import fallbacks, broad excepts, speculative ab… | [SAFE](https://agentskillshub.top/skill/LeonardNJU/code-humanizer/?utm_source=github&utm_medium=awesome-list) |

<a id="type-design"></a>
## 🎨 UI & design taste

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-design)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [Leonxlnx/taste-skill](https://github.com/Leonxlnx/taste-skill) | 92.3k | Taste-Skill - gives your AI good taste. stops the AI from generating boring, generic slop | [SAFE](https://agentskillshub.top/skill/Leonxlnx/taste-skill/?utm_source=github&utm_medium=awesome-list) |
| [Nutlope/hallmark](https://github.com/Nutlope/hallmark) | 29.5k | Anti-AI-slop design skill for Claude Code, Cursor, and Codex. | [SAFE](https://agentskillshub.top/skill/Nutlope/hallmark/?utm_source=github&utm_medium=awesome-list) |
| [yetone/kill-ai-slop](https://github.com/yetone/kill-ai-slop) | 1.3k | A field guide to the visual & copy tics of AI-generated products — and an Agent Skill that scans your project and strips them out. https://killaislop… | [SAFE](https://agentskillshub.top/skill/yetone/kill-ai-slop/?utm_source=github&utm_medium=awesome-list) |
| [agiwhitelist/auteur](https://github.com/agiwhitelist/auteur) | 1.0k | The Claude Code skill that directs a website like a film. Commit-sheet, generated assets, build, and an executable anti-slop linter that gates every… | [SAFE](https://agentskillshub.top/skill/agiwhitelist/auteur/?utm_source=github&utm_medium=awesome-list) |
| [joeseesun/qiaomu-design](https://github.com/joeseesun/qiaomu-design) | 572 | 偏执型设计顾问：反 AI 味设计 + 风格试衣间 + 58 站设计系统库的 Claude Code Skill \| Opinionated design advisor for Claude Code: anti-generic UI, style fitting room, 58 real-s… | [SAFE](https://agentskillshub.top/skill/joeseesun/qiaomu-design/?utm_source=github&utm_medium=awesome-list) |
| [codeswithroh/tastemaker](https://github.com/codeswithroh/tastemaker) | 431 | A Claude Code skill that grounds AI-generated UI in real reference images and a persistent per-developer taste profile, instead of generic AI-slop de… | [SAFE](https://agentskillshub.top/skill/codeswithroh/tastemaker/?utm_source=github&utm_medium=awesome-list) |
| [educlopez/ui-craft](https://github.com/educlopez/ui-craft) | 366 | Design engineering system for AI coding agents — ship UI with craft-level quality. Install as an agent skill. | [SAFE](https://agentskillshub.top/skill/educlopez/ui-craft/?utm_source=github&utm_medium=awesome-list) |
| [mblode/agent-skills](https://github.com/mblode/agent-skills) | 141 | Nobody ships AI slop on purpose. These skills make sure you don’t. | [SAFE](https://agentskillshub.top/skill/mblode/agent-skills/?utm_source=github&utm_medium=awesome-list) |
| [funboy322/avoid-ai-design](https://github.com/funboy322/avoid-ai-design) | 91 | Audits AI-generated frontend and rewrites it so it stops looking AI-made: purple-gradient slop and the "tasteful" defaults (cream + terracotta, mono… | [SAFE](https://agentskillshub.top/skill/funboy322/avoid-ai-design/?utm_source=github&utm_medium=awesome-list) |
| [Laith0003/ux-skill](https://github.com/Laith0003/ux-skill) | 79 | Design intelligence engine for AI coding tools (Claude Code, Cursor, Windsurf). Deterministic anti-AI-slop linter with 152 rules, 160 brand specs, a… | [SAFE](https://agentskillshub.top/skill/Laith0003/ux-skill/?utm_source=github&utm_medium=awesome-list) |
| [h3nryprod01/design-taste](https://github.com/h3nryprod01/design-taste) | 63 | Elite frontend design taste for Claude Code / Cowork — a merged synthesis of emilkowalski/skill, pbakaus/impeccable, and leonxlnx/taste-skill. Typogr… | [SAFE](https://agentskillshub.top/skill/h3nryprod01/design-taste/?utm_source=github&utm_medium=awesome-list) |
| [phazurlabs/sumi](https://github.com/phazurlabs/sumi) | 50 | Sumi — UX/UI design intelligence for Claude Code: 43 skills, 168 references, 37 commands, an anti-slop engine, and an auditable citation trail. Start… | [SAFE](https://agentskillshub.top/skill/phazurlabs/sumi/?utm_source=github&utm_medium=awesome-list) |
| [stevembarclay/pencilplaybook](https://github.com/stevembarclay/pencilplaybook) | 50 | PencilPlaybook is the UI Skills / Taste-Skill for Pencil.dev + Claude Code — a design playbook that gives Claude real perceptual psychology and senio… | [SAFE](https://agentskillshub.top/skill/stevembarclay/pencilplaybook/?utm_source=github&utm_medium=awesome-list) |
| [simonlin1212/SDesign](https://github.com/simonlin1212/SDesign) | 38 | 去 AI 味设计系统库 · 6 美学家族 × 64 套设计系统 · 复制一段提示词粘给任意 AI 就出片不飘 · 含在线预览站 \| Anti-slop design systems for any AI — 64 curated design systems across 6 aesthetic… | [SAFE](https://agentskillshub.top/skill/simonlin1212/SDesign/?utm_source=github&utm_medium=awesome-list) |
| [nghiahsgs/skills-slides](https://github.com/nghiahsgs/skills-slides) | 35 | 50,000+ unique HTML presentation designs. Zero dependencies. Anti-AI-slop. A Claude Code skill. | [SAFE](https://agentskillshub.top/skill/nghiahsgs/skills-slides/?utm_source=github&utm_medium=awesome-list) |
| [Ferousco-dev/anti-slop-design](https://github.com/Ferousco-dev/anti-slop-design) | 14 | Claude Agent Skill that eliminates generic AI-generated design. Stop your AI shipping the same purple-gradient, Inter-font, three-feature-card websit… | [SAFE](https://agentskillshub.top/skill/Ferousco-dev/anti-slop-design/?utm_source=github&utm_medium=awesome-list) |

<a id="type-rules"></a>
## 📏 Style rules

[Open this type on the live page, sorted by stars →](https://agentskillshub.top/best/anti-slop/?utm_source=github&utm_medium=awesome-list#type-rules)

| Repo | Stars | What it does | Security |
|---|---:|---|---|
| [miqdadbadjuber/anti-slop](https://github.com/miqdadbadjuber/anti-slop) | 4.4k | Rules for an AI coding agent to filter out generic AI-generated UI designs, text, and code. | [SAFE](https://agentskillshub.top/skill/miqdadbadjuber/anti-slop/?utm_source=github&utm_medium=awesome-list) |
| [AIScientists-Dev/academic-humanizer](https://github.com/AIScientists-Dev/academic-humanizer) | 1.8k | Strip AI-writing tells from papers and grant proposals (NSF/NIH), while keeping scholarly voice and tying claims to evidence. A skill for Claude Code… | [SAFE](https://agentskillshub.top/skill/AIScientists-Dev/academic-humanizer/?utm_source=github&utm_medium=awesome-list) |
| [alexgreensh/attention-span](https://github.com/alexgreensh/attention-span) | 1.2k | Make your agents talk human. ADHD-friendly output styles for Claude Code, Codex, and others. So you can pay attention, not tokens. | [SAFE](https://agentskillshub.top/skill/alexgreensh/attention-span/?utm_source=github&utm_medium=awesome-list) |
| [realrossmanngroup/no_ai_slop_writing_rules](https://github.com/realrossmanngroup/no_ai_slop_writing_rules) | 694 | Claude Code reference: write in Louis Rossmann's voice, never like AI slop. Portable CLAUDE.md plus skills. | [SAFE](https://agentskillshub.top/skill/realrossmanngroup/no_ai_slop_writing_rules/?utm_source=github&utm_medium=awesome-list) |
| [jalaalrd/anti-ai-slop-writing](https://github.com/jalaalrd/anti-ai-slop-writing) | 494 | AI writing skill that eliminates detectable AI patterns. Works with Claude Code, Codex, Cursor, Gemini CLI, and 8+ other agents. | [SAFE](https://agentskillshub.top/skill/jalaalrd/anti-ai-slop-writing/?utm_source=github&utm_medium=awesome-list) |
| [matsuikentaro1/humanizer_academic](https://github.com/matsuikentaro1/humanizer_academic) | 271 | A Claude Code skill that removes signs of AI-generated writing from academic medical papers, making them sound more natural and professionally writte… | [SAFE](https://agentskillshub.top/skill/matsuikentaro1/humanizer_academic/?utm_source=github&utm_medium=awesome-list) |
| [adenaufal/anti-slop-writing](https://github.com/adenaufal/anti-slop-writing) | 143 | Stop your AI from writing like AI. A universal system prompt eliminating every known LLM style tell — works with Claude Code, Gemini CLI, Codex CLI,… | [SAFE](https://agentskillshub.top/skill/adenaufal/anti-slop-writing/?utm_source=github&utm_medium=awesome-list) |
| [haidrrrry/humanize-ai-writing](https://github.com/haidrrrry/humanize-ai-writing) | 16 | Free anti-AI-slop system prompt & skill that makes ChatGPT, Claude, Gemini, Grok & Kimi write like a human. Bans AI tells (delve, tapestry, 'not just… | [SAFE](https://agentskillshub.top/skill/haidrrrry/humanize-ai-writing/?utm_source=github&utm_medium=awesome-list) |
| [impactcrew/dont-be-a-sloperator](https://github.com/impactcrew/dont-be-a-sloperator) | 10 | Don't be a sloperator. Ten rules that stop AI from writing and behaving like naked AI. Principle-based, not vocabulary bans. Includes a bonus /work s… | [SAFE](https://agentskillshub.top/skill/impactcrew/dont-be-a-sloperator/?utm_source=github&utm_medium=awesome-list) |
| [AMishradev/outbound-writing](https://github.com/AMishradev/outbound-writing) | 5 | A Claude Code skill that strips AI tells out of cold email. Anti-slop engine for startup outbound to technical people. | [SAFE](https://agentskillshub.top/skill/AMishradev/outbound-writing/?utm_source=github&utm_medium=awesome-list) |
| [Dexxter182/humanizer-hu](https://github.com/Dexxter182/humanizer-hu) | 5 | Magyar írásstílus-skill agenteknek: a kimenet ne hangozzon AI-nak. Írás közben ad szabályokat, nem a kész szöveget javítja utólag. Csak azt állítja,… | [SAFE](https://agentskillshub.top/skill/Dexxter182/humanizer-hu/?utm_source=github&utm_medium=awesome-list) |

**Security** is the grade of the repo's README and install steps on Agent Skills Hub. *pending* means the catalog has not graded it yet.

Preview images are reduced copies of pictures from each project's own README, included only for projects under a permissive license. Sources and licenses: [assets/previews/NOTICE.md](assets/previews/NOTICE.md). Open an issue to have one removed.

## Related collections

- [zhuyansen/awesome-claude-video-skills](https://github.com/zhuyansen/awesome-claude-video-skills), [zhuyansen/awesome-codex-ppt-skills](https://github.com/zhuyansen/awesome-codex-ppt-skills) — lists built the same way.

## Add a repo

Open an issue with the GitHub URL. It goes through the same review as every entry; the rules above decide, stars do not.

---

Machine-readable copy: [`data/skills.json`](data/skills.json). Generated 2026-10-04.
