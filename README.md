# 真实素材短视频脚本 · 使用说明

把已经有的经历、转录稿和方法变成能直接讲、直接演示的内容。适合有素材但不会组织、稿子像作文、镜头前背不下来，或需要不露脸表达的人。

## 怎么用

调用 `$lany-short-video-script-skill`，附原始素材、给谁看、希望观众得到什么。平台、时长、是否露脸有要求再补充。没有具体经历也可写知识解释，但不会替你编“我做成了”。

得到：表达锚点、完整口播稿，必要时附提词骨架、镜头表和事实核实项。不需要先填复杂问卷。

## 完整示例（以下经历为演示而虚构）

输入：

> $lany-short-video-script-skill 给刚接小项目的设计师写一条约45秒口播。我第一次接海报项目，只问客户喜欢什么颜色，做完才知道他需要印成店门口的立牌。我重新问了摆放位置、尺寸、顾客离多远看，把小字减少了。没有销售数据，不要写成交提升。不露脸，录屏即可。

可能得到的锚点：接设计任务先确认使用场景，再谈颜色。

示例稿：

> 接海报项目，先别急着问客户喜欢什么颜色。
>
> 我第一次接单就这么问。做完才知道，他要的不是手机里看的图，而是摆在店门口的立牌。屏幕上能看清的小字，放到那个场景里就不合适了。
>
> 后来我重新问：摆在哪里，多大尺寸，顾客站多远看。再按这些条件删掉小字。
>
> 这只能说明设计更贴近使用场景，还不能说销量变好了。
>
> 下次接需求，先把这三个问题发给客户。颜色可以后面聊。

镜头：显示模拟需求表→展示屏幕和立牌用途差异→逐项显示三个问题。不展示真实客户信息。时长为估计，录制前按本人语速试听。

## 什么时候换技能

想研究别人的视频为什么有效，用 `lany-content-remix-skill`；想根据发布数据决定下一轮改什么，用 `lany-content-experiment-skill`。本技能只负责表达成品，不承诺爆款、涨粉或收入。

依据见 [来源与提炼说明](references/sources.md)。

## 2026 年星球增补

新增标题—开头—正文的承诺核对。调用例：`$lany-short-video-script-skill 这是我的标题与口播稿，检查标题吸引的人和正文帮助的人是否一致，只修承诺断裂，不增加效果数字。`

[增补来源与适用边界](references/zsxq-2026.md)。原有小报童方法与说明保留。

## 独立仓库与安装

仓库：[lany-short-video-script-skill](https://github.com/LanyXiaosheng/lany-short-video-script-skill)。本仓库根目录即技能目录，包含 `SKILL.md`、本说明及 `references/`。

确认目标目录不存在后，可在未设置 `CODEX_HOME` 的默认环境下安装：

```bash
mkdir -p ~/.codex/skills
git clone https://github.com/LanyXiaosheng/lany-short-video-script-skill.git ~/.codex/skills/lany-short-video-script-skill
```

已设置 `CODEX_HOME` 时，将目标改为该目录下的 `skills/lany-short-video-script-skill`。已有同名技能时先比较或备份，不覆盖。客户端发现技能后，使用 `$lany-short-video-script-skill` 调用。

初次拆分的提交历史继续保留；当前工作版本已纳入2026年知识星球增强方法。
