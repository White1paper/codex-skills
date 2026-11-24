# Codex Skills

这个仓库存放可在 Codex 中使用的技能。目前提供 [Word 统一排版](skills/word-formatting-standard/SKILL.md)，用于生成或修订 Word 文档时统一排版，并标出附件原文、局部修改和新增内容。

## Word 统一排版

- 中文正文用宋体，数字和英文字母用 Times New Roman。正文为小四（12 磅），采用 1.5 倍行距、两端对齐和首行缩进 2 字符。
- 生成或改写内容时，附件原文用黑色 `#000000`，保留原意的局部修改用黄色 `#FFFF00`，重写、实质性修改和新增内容用红色 `#FF0000`。
- 同一句或同一段包含不同类别时，分别设置对应文字的字体颜色。当次任务指定格式或要求无标色稿时，以当次要求为准。

## 安装

1. 在 GitHub 仓库页面选择 **Code → Download ZIP**，下载并解压。
2. 将 `skills/word-formatting-standard` 整个目录复制到用户级技能目录 `~/.agents/skills/`。在 Windows PowerShell 中，该目录是 `$HOME\.agents\skills\`。如目录不存在，先创建它。只在一个项目使用时，可将同一目录放在项目的 `.agents/skills/` 下。
3. 在 Codex 输入 `$word-formatting-standard`，或在技能选择器中选择 **Word 统一排版**。如果没有看到新技能，重启 Codex。

在 Windows 上生成 Word 文件时，使用本机 Microsoft Word 或 WPS。技能原文提到的 `word-wps-documents` 是配套的本地 Word/WPS 工作流程，可按自己的环境配置。

## 使用示例

> 请使用 `$word-formatting-standard`，根据上传的会议纪要和研究报告撰写一份项目进展说明，交付 Word 文件。沿用的原文用黑色，保留原意的局部修改用黄色，重写或新增内容用红色。

## 文件

- [`SKILL.md`](skills/word-formatting-standard/SKILL.md) 包含完整的排版、标色和交付核验规则。
- [`agents/openai.yaml`](skills/word-formatting-standard/agents/openai.yaml) 包含技能显示名称、默认提示和自动调用设置。

技能目录和调用方式见 [OpenAI 技能文档](https://learn.chatgpt.com/docs/build-skills)。
