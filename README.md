# tim-ending

把影视飓风 Tim 在视频结尾说的“涩话”，整理成一个可以反复调用的写作 Skill。

一篇文章写完，想在最后多留一点东西，就可以把正文交给它，让它帮你写一段 Tim 式的“涩话”结尾。

这里说的“涩话”，是那种从眼前的一件小事讲起，慢慢讲到人与人、人与时间的关系，最后又落回生活的收尾。看完以后，让人愿意停一会儿，再想想自己。

这份 Skill 根据 Tim 的公开文案、原片信息和创作者访谈，提炼了其中的叙事方法。它会先读你的正文，找到最值得回扣的真实细节，再把情绪接起来，保留你自己的说话习惯。

## 让 AI 帮你安装

把下面这段话复制给支持联网和本地 Skill 安装的 AI 助手，例如 Codex：

```text
请帮我下载并安装 tim-ending 这个 Skill。

仓库地址：https://github.com/xiaoniaoyou0325/tim-ending
技能目录：skills/tim-ending
直接地址：https://github.com/xiaoniaoyou0325/tim-ending/tree/main/skills/tim-ending

请把 skills/tim-ending 整个目录安装到当前工具支持的个人技能目录，保留里面的 SKILL.md、agents/ 和 references/。
安装完成后，确认技能名称为 tim-ending，并告诉我怎样调用。
```

安装时使用 `skills/tim-ending` 这一份完整目录即可。它包含写作指令、工具配置、方法、样例和研究依据。

## 安装后怎么用

提供文章正文，再告诉 AI：

```text
请使用 $tim-ending，为下面这篇文章写一个 Tim 式的“涩话”结尾。
保留我的口吻，从正文里的真实细节出发，先给一版。

正文：
（粘贴你的文章）
```

也可以提供最后几段和希望回扣的真实故事。如果最后一句互动已经确定，就把那句话一并给它。

可以继续调整要求，例如“收得更轻一点”“情绪可以再往上走一点”“保留最后这句互动”。技能提供写法，每篇文章仍需要自己的材料。

## 这些文件和文件夹是干嘛的

仓库目前同时提供根目录版和 `skills/tim-ending` 独立目录版，二者承载同一套结尾写作方法。**安装推荐使用 `skills/tim-ending`；浏览时可以直接阅读根目录文件。**

```text
tim-ending/
├── README.md                     给使用者看的介绍和安装说明
├── SKILL.md                      给 AI 读取的技能入口
├── agents/
│   └── openai.yaml               支持该配置的工具使用的显示与调用信息
├── references/
│   ├── craft.md                  写法与自检方法
│   ├── examples.md               原创样例和反例
│   └── research.md               Tim 结尾的研究来源
└── skills/
    └── tim-ending/               推荐安装这一整个目录
        ├── SKILL.md
        ├── agents/
        │   └── openai.yaml
        └── references/
            ├── craft.md
            ├── examples.md
            └── research.md
```

| 文件或目录 | 用途 |
| --- | --- |
| [README.md](README.md) | 当前这份说明，方便使用者了解技能、复制安装指令和查看用法。 |
| [SKILL.md](SKILL.md) | AI 的工作说明，定义什么时候使用技能、怎么读材料、怎么写结尾，以及交稿前检查什么。 |
| [agents/](agents/) | 保存工具适配配置。`openai.yaml` 提供技能显示名称、简介、默认调用提示词等信息。 |
| [references/](references/) | 保存写作参考，供 AI 按任务需要读取。`craft.md` 讲方法与自检，`examples.md` 给样例与反例，`research.md` 记录研究依据。 |
| [skills/tim-ending/](skills/tim-ending/) | 这套技能的独立安装目录。需要下载安装时，把这一整个目录交给 AI。 |

## 它适合什么内容

- 公众号文章、视频口播、纪实故事的收尾。
- 技术、工具、创作和生活观察中，希望落回人的感受的段落。
- 已经写好结尾，希望改得自然、有余味的稿子。

它会根据正文判断情绪该走多远。普通操作教程，也可以停在一个清楚的判断或下一步动作。

## 手动下载

1. [下载仓库 ZIP](https://github.com/xiaoniaoyou0325/tim-ending/archive/refs/heads/main.zip)，或者点击仓库页面的 **Code → Download ZIP**。
2. 解压后找到 `skills/tim-ending`，保留整个文件夹。
3. 按所用工具的要求安装，再提供正文调用。

在 Codex 中，个人技能可放到 `~/.agents/skills/tim-ending/`；项目专用技能可放到项目的 `.agents/skills/tim-ending/`。安装后确认该目录里能直接看到 `SKILL.md`。其他工具按各自支持的安装方式使用。[Codex 官方技能目录说明](https://learn.chatgpt.com/docs/customization/overview#skills)

## 进一步了解

- [写法与检查](skills/tim-ending/references/craft.md)：怎样从材料走向感受，怎样决定停笔。
- [样例与反例](skills/tim-ending/references/examples.md)：包含 AI 音乐文章结尾和不同情绪尺度的练习。
- [研究依据](skills/tim-ending/references/research.md)：公开来源、研究范围与取样边界。

由「火星来信 Marswan」整理。本项目非影视飓风官方出品；示范结尾均为原创整理文本，非 Tim 原话。

当前版本：1.0.1。
