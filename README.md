# Solution PPT Workflow

一个用于制作**客户解决方案 PPT**和**产品介绍 PPT**的 Codex Skill。它帮助你从资料核对、目录与逐页分镜开始，再制作蓝图、真实产品场景和原型，最后逐页验收与全稿检查。具体工作规则见 [SKILL.md](SKILL.md)。

## 安装

在 Codex 中提出：

> 使用 `$skill-installer`，从 `https://github.com/VicoZhou/solution-ppt-workflow` 的仓库根目录安装 Skill，名称为 `solution-ppt-workflow`。

也可以将本仓库放到用户技能目录 `~/.codex/skills/solution-ppt-workflow/`，并确认 `SKILL.md` 位于该目录根部。Windows 对应路径通常是 `C:\Users\<用户名>\.codex\skills\solution-ppt-workflow\`。已安装的用户无需重复安装。

## 最快的使用方式

在新的 Codex 对话中明确写出 **`$solution-ppt-workflow`**。技能也可能在请求匹配时自动启用，但显式调用更容易保证按此工作流执行。参见 [OpenAI Docs 的技能调用说明](https://developers.openai.com/blog/eval-skills)。

### 从零制作客户方案

```text
使用 $solution-ppt-workflow，为【客户名称】制作【项目/产品】解决方案 PPT。
目标听众：【客户高管/业务负责人/IT团队】；这次演示希望达成：【目标】。
我会提供现有 PPT、会议纪要、业务表格和系统页面。
请先核对事实、待确认问题和一期/后续边界，再给我目录与逐页分镜；在我确认前不要编辑 PPT。
确认后在【在线 PPT 地址或指定文件】中制作，按【一页一验收/整章验收】推进。
```

### 制作产品介绍

```text
使用 $solution-ppt-workflow，为【产品名称】制作面向【目标行业/客户】的产品介绍 PPT。
请先核对真实已实现功能，把标准业务范围与差异化体验分开讲；AI 能力需说明输入、业务上下文、人工确认和结果回写。
参考资料：【产品地址/代码目录/现有 PPT/品牌模板】。
先交付目录、逐页分镜和 2–3 张不同类型的风格样张，确认后再批量制作。
```

### 审查或修改现有 PPT

```text
使用 $solution-ppt-workflow 审查【PPT 文件或在线地址】。
先只检查内容逻辑、重复页、事实依据、AI 能力表述和分期口径，不要修改。
给出按页的修改清单；我确认后再按【逐页/整章】编辑，并同步核对备注、页码与页尾。
```

## 开始前最好提供什么

- 演示对象、目的、预期页数或时长；
- 现有 PPT、品牌模板、会议纪要、业务表格及可使用的案例数据；
- 实际产品页面、截图或演示环境；
- 哪些能力已上线、哪些只是规划，以及不能公开的内容；
- 希望在线编辑还是处理文件，以及逐页或整章验收。

资料不齐也可以开始：Skill 会优先询问影响叙事和承诺范围的关键问题，不会把 PPT 讨论变成完整 PRD 访谈。它提供的是**制作方法**，不会自动拥有你的客户资料、账号或编辑权限。

## 仓库内容

- [SKILL.md](SKILL.md)：核心工作流与制作关口；
- [AI 原生产品介绍方法](references/ai-native-product-intro.md)：AI 闭环、标准产品与差异化场景的讲述方式；
- [分镜与验收工作表](references/production-checklists.md)：证据、逐页分镜和全稿质检；
- [视觉资产指南](references/visual-assets.md)：真实截图、生成原型与 PPT 原生元素的取舍。

公开仓库仅包含通用方法，不包含客户项目的私有案例、PPT 或截图。
