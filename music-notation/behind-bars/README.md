# Behind Bars — Elaine Gould (Faber Music, 2011)

知识库形态：**每章一份中文 Markdown 笔记 + 原页图（每页一张 JPG）**。

笔记是给人和 AI 搜索/阅读用的；原图是真相源 —— 任何笔记里描述不清或可能理解错的地方，AI 都可以回去翻原图核对。

## 仓库布局

```
behind-bars/
├── README.md                          ← 本文件（总目录 + 规范 + 进度）
├── front-matter/
│   ├── notes.md
│   └── pages/                         p_i.jpg, p_ii.jpg, ...
├── part-1-general-conventions/
│   ├── 01-ground-rules/
│   │   ├── notes.md
│   │   └── pages/                     p003.jpg, p004.jpg, ...
│   ├── 02-chords-dotted-ties/
│   │   ├── notes.md
│   │   └── pages/
│   └── ...
├── part-2-idiomatic-notation/
│   └── ...
├── part-3-layout-and-presentation/
│   └── ...
└── back-matter/
    ├── notes.md
    └── pages/                         p651.jpg, ...
```

## 命名规范（重要 —— 桌面 Claude Code 按这套定位页面）

- **章节文件夹**：`<两位章号>-<kebab-case 标题>/`，例：`06-metre/`
- **正文页图**：`p<三位 0 填充阿拉伯页码>.jpg`，**页码与书印刷页码一致**。例：第 47 页 → `p047.jpg`
- **前言罗马页图**：`p_<小写罗马数字>.jpg`，例：`p_xii.jpg`
- **笔记**：每章固定 `notes.md`
- **格式**：JPG（不要 PNG，体积差 5–10×；本书纯黑白，灰度 JPG 足够清晰）

## 扫描质量要求（"干净"标准）

为了让桌面 Claude Code 后续能准确读图：

1. **用扫描 App 不要直接拍照**：Apple 备忘录"扫描文稿" / Adobe Scan / 微软 Lens / CamScanner —— 它们会自动**裁边、纠斜、增强对比度**
2. **一页一张图**，不要拍跨页
3. **整页在框内**，不要切到内容；不要有手指、阴影、装订阴影盖住文字或谱例
4. **方向正确**（页码朝下/正读方向）
5. **页码可见** —— 这样我能验证文件名和实际页码对得上
6. **JPG 输出**，质量中高即可（单页 < 1 MB 是好结果）

## 完整章节表 + 进度

页码区间已确定，文件夹会随你扫到对应章节时建出来。

| # | 章节 | 页码 | 状态 |
|---|------|------|------|
|   | Front Matter | i–xviii | ⬜ |
|   | **Part I — General Conventions** |   |   |
| 1 | Ground Rules | 3–44 | ⬜ |
| 2 | Chords / Dotted notes / Ties | 45–74 | ⬜ |
| 3 | Accidentals & Key Signatures | 75–98 | ⬜ |
| 4 | Dynamics & Articulation | 99–122 | ⬜ |
| 5 | Grace Notes / Arpeggio / Trills / Glissandos / Vibrato | 123–148 | ⬜ |
| 6 | Metre | 149–190 | ⬜ |
| 7 | Tuplets | 191–216 | ⬜ |
| 8 | Repeat Signs | 217–242 | ⬜ |
|   | **Part II — Idiomatic Notation** |   |   |
| 9 | Woodwind & Brass | 243–268 | ⬜ |
| 10 | Percussion | 269–300 | ⬜ |
| 11 | Keyboard | 301–348 | ⬜ |
| 12 | Harp | 349–370 | ⬜ |
| 13 | Classical Guitar | 371–390 | ⬜ |
| 14 | Strings | 391–430 | ⬜ |
| 15 | Vocal Music | 431–478 | ⬜ |
|   | **Part III — Layout and Presentation** |   |   |
| 16 | Preparing Materials | 479–498 | ⬜ |
| 17 | Score Layout | 499–554 | ⬜ |
| 18 | Part Preparation | 555–588 | ⬜ |
| 19 | Electroacoustic Music | 589–606 | ⬜ |
| 20 | Freedom and Choice | 607–650 | ⬜ |
|   | Back Matter (Appendix / Further Reading / Index) | 651–end | ⬜ |

状态：⬜ 未开始 · 🟡 进行中 · ✅ 已完成

## 笔记规范（每章 `notes.md` 模板）

```markdown
# 第 N 章 · 章节标题（中文）

> 原书页码 X–Y · 原图：`./pages/`

## 概述
（这一章在讲什么，2–3 句）

## 要点

### 主题 1（对应 p.X）
- ...
- ![p.X 谱例](./pages/p0XX.jpg)

### 主题 2（对应 p.X）
- ...

## 关键术语
- 中文术语 (English term)：定义

## 交叉引用
- 见第 N 章「主题」（p.X）
```
