# AI Spark · 写作工作流演示 vault

> 这是 **AI Spark 第四节课**（劳伦斯主讲）的演示 vault ——用课上讲的那套最小工作流，从想法一路跑到定稿 + 封面提示词的完整产物。

## 它是怎么来的

把 [`deploy-prompt.md`](https://github.com/lawrencewzen/write-workflow/blob/main/course/2025-04-25/assets/deploy-prompt.md) 粘贴给 Claudian 部署，就会自动生成 `AGENTS.md`、`articles/`、`idea/`、`memory/` 这套结构。然后照着讲义的流程跑一遍：

```
想法 → 补充要点 → 导入工作流（AI 扩写）→ 改 working.md → 定稿
                                                          ↓
                                          final.md + cover-prompt.md
                                          memory/我的改稿习惯.md（自动学习）
```

## 目录说明

```
.
├── AGENTS.md                                 ← 给 AI 看的规则手册（部署时自动生成）
├── idea/
│   └── 抓住 AI 时代的红利.md                  ← 最初的想法 + 补充要点
├── articles/抓住 AI 时代的红利/
│   ├── draft/
│   │   ├── source.md                         ← AI 扩写出的初稿（不要改）
│   │   └── working.md                        ← 学员改过的工作稿
│   └── final/
│       ├── final.md                          ← 正式稿（可直接发公众号）
│       └── cover-prompt.md                   ← 定稿时一起生成的封面提示词
└── memory/
    └── 我的改稿习惯.md                        ← AI 从 diff(source, working) 自动学的偏好
```

## 对着看什么

- 打开 `articles/抓住 AI 时代的红利/draft/source.md` 和 `working.md` 对比，看学员改了哪些地方
- 打开 `memory/我的改稿习惯.md`，看 AI 从 diff 里提炼出的 6 条写作偏好
- 打开 `articles/抓住 AI 时代的红利/final/cover-prompt.md`，把里面的英文或中文 prompt 复制到 Midjourney / 即梦 / 可灵，就能生成配套封面图

## 想自己跑一遍？

去 [`write-workflow`](https://github.com/lawrencewzen/write-workflow) 仓库下的 `course/2025-04-25/` 目录，里面有讲义、教程和那段一键部署提示词。
