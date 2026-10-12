# 个人论文写作技能（zh-humanities-paper）

这是一个 Claude 技能，用来按作者的个人标准写作、修改、整理和评审中文人文社科论文，主要面向新闻传播学、媒介理论、戏剧与影视学（含纪录片）。

## 内容来源

- 四组 AI 协作记录的分析：
  - 一篇媒介理论期刊论文的多轮修改；
  - 一份博士研究计划与文献综述的写作过程；
  - 一次文献综述的修改过程；
  - 一篇“理论+创作”型硕士毕业论文的选题与写作准备。
- 五篇范文的写法拆解。只提炼结构和手法，不收录原文。

## 文件结构

```
.claude/skills/zh-humanities-paper/
├── SKILL.md                         核心标准：五条反复强调的要求、任务类型判断、理想论文、
│                                    结构、概念、措辞、引文、标题、协作纪律、交付前自检
├── references/
│   ├── exemplar-moves.md            五篇范文的骨架和 16 个论证动作，以及不宜照搬之处
│   ├── sentence-craft.md            短评词典（“幼稚”“杂糅”等各指什么）、被否决的表达、AI 痕迹清单、改稿习惯
│   ├── concept-naming.md            概念规范性检查、界定写法、命名四项检验、推敲记录
│   ├── citation.md                  引文底线、四种表述的标注、格式、核查流程
│   ├── genre-templates.md           期刊理论论文、经验研究、文献综述、研究计划、摘要、题目的结构
│   ├── degree-thesis.md             学位论文的选题、选题汇报、题目范式、章节递进、“理论+创作”型写法
│   └── collaboration-lessons.md     以往协作中的 22 条失误与教训，以及被接受的修改格式
└── evals/evals.json                 3 个测试用例（不打包进技能）
dist/zh-humanities-paper.skill       打包好的技能文件，可直接上传安装
```

## 使用方法

- **Claude Code**：
  - 在本仓库中使用时，技能会自动加载；
  - 想在所有项目中使用，把 `.claude/skills/zh-humanities-paper/` 复制到 `~/.claude/skills/`。
- **claude.ai**：在设置的技能（Skills）页面上传 `dist/zh-humanities-paper.skill`。
- 平时不需要特别指明。只要让 Claude 写论文、改段落、拟题目、整理综述、核查引文，技能就会被调用。也可以直接说“用我的论文写作技能”。

## 后续完善

以后有新的对话记录或改稿，可以继续补充：
- 新的被否决的说法，加进 `references/sentence-craft.md`；
- 新的失误，加进 `references/collaboration-lessons.md`；
- 新的范文，加进 `references/exemplar-moves.md`。
