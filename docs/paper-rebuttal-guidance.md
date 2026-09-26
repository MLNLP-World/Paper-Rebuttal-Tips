# paper-rebuttal-guidance（S0 初版）

[Skill 入口](../skills/paper-rebuttal-guidance/SKILL.md)提供两种可分别使用的辅助流程：

1. 整理用户提供的 tip 标题、审稿人问题、反面回答样式、推荐回答样式和核心点，形成投稿草稿；按需整理 HTML，不代为提交。
2. 根据用户提供的审稿意见和 rebuttal 草稿，在有限已读知识范围内提供定性反馈，指出需要会议官方说明才能判断的问题。

这是供维护者审核的有限范围初版。六文件包由 Repo2Skill 生成，经既有静态审查和首轮评测后原样保留；包内“候选／待评测”文字记录冻结时状态，最新评测结论见下文。

## 在 Codex 中使用

成功加载记录使用 Codex CLI 0.155.1：将本仓库 `skills/paper-rebuttal-guidance/` 整个六文件目录复制到任务项目的 `.agents/skills/paper-rebuttal-guidance/`，保留 `references/` 和 `provenance.json`，再从该项目启动新会话。本仓库的 `skills/` 是包的存放位置；仅合入这里不代表客户端会自动加载。项目发现目录及显式调用方式也见 [Codex 官方 Skill 文档](https://learn.chatgpt.com/docs/build-skills#where-codex-loads-local-skills)。

按任务选择一种提示，并附上实际材料：

```text
$paper-rebuttal-guidance
请把以下 tip 内容整理为贡献草稿：
标题：…
审稿人问题：…
反面回答样式：…
推荐回答样式：…
核心点：…
```

```text
$paper-rebuttal-guidance
请在已读材料范围内，对以下 rebuttal 提供定性反馈：
审稿意见：…
rebuttal 草稿：…
会议官方说明（如有）：…
```

第二种用途仍缺有效 Skill 配对评测证据。未提供会议说明时，字数、新实验和外链权限等保持未决；不能将计划实验写成结果，也不能据 tip 标题补写未读图片内容。

## 已有评测与缺口

首轮评测于 2026-09-26 使用 Codex CLI 0.155.1，配置为 `gpt-6-astra` / `medium`；以下摘要依据 2026-09-27 的最终独立评审。共 21 次会话，无重跑：3 次加载诊断和 18 个主对照。主对照中 14 个可评分、4 个受阻；“可评分”不等于全部通过。

| 条件 | 可评分主对照 |
| --- | --- |
| A：基础条件 | 5/6 |
| B：提供固定 commit 原始文本 | 6/6 |
| C：提供 Skill | 3/6 |

Skill 的有效案例仅为 T1/T4/T5（tip 整理、缺失材料处理、未读图片边界）；T2/T3/T6 的 Skill 会话受阻。核心 rebuttal 审阅 T3 仅 B 可评分，尚缺有效 Skill 配对证据。每案例每组仅一次会话且配对不完整，已有比较仅支持局部观察，不证明稳定提升、普遍优于原材料或完整领域覆盖。

Codex 显式调用和隐式选择均有成功读取完整 `SKILL.md` 的工具证据；发现名称或模型自述不算加载证据。Claude Code 客户端加载：**NOT RUN**。这些结论来自已有记录，本次贡献没有重跑模型或补样。

## 来源与范围限制

证据固定于本仓库 commit [`4fe2b488c1ebc83eba9c91fbd2fc2eb51abeba4c`](https://github.com/MLNLP-World/Paper-Rebuttal-Tips/tree/4fe2b488c1ebc83eba9c91fbd2fc2eb51abeba4c)，未因本次贡献重新抽取。[Provenance](../skills/paper-rebuttal-guidance/provenance.json) 保留来源、构建输入与文件哈希；[追溯记录](../skills/paper-rebuttal-guidance/references/traceability.json)连接流程与固定版本证据。

- 抽取仅覆盖已提供的 README 和 `.gitignore` 文本；包内证据材料仅收录被引用的 README。repo map 为 dry-run，无语义推断，空白部分不代表仓库没有相关知识。
- 动机 PNG 和全部 28 个 tip SVG 未读取或解释；图片中的问题、回答和核心点未被抽取。外链资源、工具、课程及其当前状态未检查。
- rebuttal 反馈限于指南定位、三个主题分类和 Tip 12 的标题级策略；不补全其他 tip 细节，不执行实验，不保证建议有效，也不替代会议规则。
- 原指南的来源与适用性声明继续适用。来源归属、许可和再分发安排仍待维护者核对；本初版不表示作者背书。
