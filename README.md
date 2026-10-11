# Notion 黑白手绘工作室

第一版：**v1.0.0** · 2026-10-11。

用于干净克制的黑白内容配图、独立人物与物件、小装饰，以及原创手绘 Logo 概念。人物随内容变化，没有固定主角。

## 使用

将 `skills/notion-handdrawn-studio` 文件夹放入个人 Codex skills 目录，再在对话中调用：

> 使用 $notion-handdrawn-studio，为我的内容创作一张干净克制的黑白手绘配图。

[Skill 主文件](skills/notion-handdrawn-studio/SKILL.md) 包含默认值与工作方式。Skill 附带 12 张精选官网参考、来源记录与画风分析，按用途读取。

## 第一版验证

- 4 张真实生成：正文配图、独立人物、小装饰、Logo 概念。
- 4 项规则走查：仅规划、仅提示词、默认值覆盖、编辑范围。
- 4 项新主题待用户参与验证。
- 文件结构、参考哈希、透明背景和 Logo 小尺寸已经检查。
- Astra 完成视觉复核；已有样例构思在切换模型前完成。生成工具为内置 image_gen，底层图像模型未披露。

用户审美验证仍待进行。人物衣褶与手部细节稍多，Logo 的“生长”意味强于“思考”；保存这些观察作为后续版本的依据。

[样例总览](evaluations/v1.0.0/previews/self-test-board.jpg) · [自评](evaluations/v1.0.0/self-review.json) · [验证集](evaluations/v1.0.0/cases.json) · [完整提示词](evaluations/v1.0.0/prompts.txt)

下载仓库后，用浏览器打开 `evaluations/v1.0.0/index.html` 查看完整验证页并填写反馈。GitHub 上的 HTML 文件显示源代码，图片与 Markdown 可直接预览。

## 回溯

`VERSION` 记录当前版本；`CHANGELOG.md` 记录变更。本地 Git 标签 `v1.0.0` 已固定第一版，之后每次改动保留提交与对应验证记录。远端提交已经保存本版，可通过提交历史准确回溯并下载。远端 `v1.0.0` 标签尚未创建：当前 GitHub 连接不提供标签创建能力，浏览器连接多次超时；本地标签与 `VERSION` 文件已保留版本号。

## 参考素材

官网图像仅作为画风研究参考，保留来源与原始字节。没有核实每张图的作者或再分发授权；这些原图不作为本项目原创资产，也没有替第三方素材授予许可。本版本未添加开源许可证。
