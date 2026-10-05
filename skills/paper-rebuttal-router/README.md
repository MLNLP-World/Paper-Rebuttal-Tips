# Paper Rebuttal Router

`paper-rebuttal-router` 是基于 [Paper-Rebuttal-Tips](../../README.md) 构建的学术 rebuttal Skill。

它把仓库中的 rebuttal 经验整理为一组可复用的 Workflow，并根据用户当前的任务和 reviewer point 自动选择合适的处理路径。用户不需要了解内部 Workflow 的名称，只需要提供论文、reviewer comments、已有回复或相关实验信息。

它可以用于：

- 分析 reviewer comments；
- 检查已有 rebuttal response；
- 起草 response material；
- 处理缺实验、证据不足或时间受限的 reviewer request；
- 整理新的 rebuttal 经验。

---

## 快速开始

### Claude Code

首先 clone 本仓库：

```bash
git clone https://github.com/MLNLP-World/Paper-Rebuttal-Tips.git
cd Paper-Rebuttal-Tips
```

创建 Claude Code 的个人 Skill 目录：

```bash
mkdir -p ~/.claude/skills
```

安装整个 Skill：

```bash
cp -a skills/paper-rebuttal-router ~/.claude/skills/
```

需要复制整个 `paper-rebuttal-router` 目录，而不是只复制 `SKILL.md`，因为 Skill 还会读取 `references/` 中的 router 和 Workflow 文件。

安装完成后重新启动 Claude Code。若 Claude Code 已经在运行，也可以执行：

```text
/paper-rebuttal-router
```

---

## 使用方式

不需要手动指定 Workflow。直接提供材料并说明希望完成的任务即可。

### 1. 分析 reviewer comments

```text
分析这些 reviewer comments，并指出每个 reviewer point 需要我们真正回答的问题。
```

### 2. 回答一个 reviewer weakness

```text
请阅读附带的论文，并帮助我回应下面这条 reviewer weakness。

Weakness:
[粘贴 reviewer 原文]

请只使用论文中已有的证据进行分析和回应。
```

### 3. 回答指定的多个 weaknesses

```text
请阅读附带的论文，并使用 paper-rebuttal-router
帮助我回答 Summary of Weaknesses 中的第 1 条和第 3 条。

Weakness 1:
[粘贴 Weakness 1]

Weakness 3:
[粘贴 Weakness 3]

请分别处理两个 reviewer point，并根据论文中的已有证据准备回应材料。
```

### 4. 检查已有 rebuttal

```text
下面是 reviewer comment 和我当前的回复。

请检查这份回复的问题，包括是否正面回答 reviewer、证据是否充分，
但不要直接重写。
```

### 5. 处理暂时无法完成的实验

```text
Reviewer 要求补充下面这个实验，但我们无法在 rebuttal deadline 前完成。

请基于当前已有的论文证据和实验结果规划回应。
```

---

## 为什么这样组织

Paper-Rebuttal-Tips 中包含 28 条 rebuttal tips。

我们没有把它们分别做成 28 个独立 Skill，因为实际 reviewer comment 往往同时包含多个问题，而且不同 tips 之间也存在可以复用或组合的策略。

因此，构建过程中先整理原始 README 和 tip cards 中的知识，再形成 26 个 Workflow，并由一个 router 负责选择。

当前版本对应：

- 38 个 knowledge items；
- 25 个 reusable capabilities；
- 26 个 Workflows。

这些中间结构主要用于构建和追溯，使用者不需要手动操作它们。

例如，一条 reviewer comment 可能同时质疑：

> comparison fairness、ablation 和 generalization

Skill 会先将它拆成几个 reviewer points，再分别选择适合的 Workflow，最后汇总结果。

---

## 覆盖场景

当前 Workflow 覆盖了常见的 rebuttal 场景，包括：

- novelty 与 related work；
- contribution、motivation、theory 和 limitations；
- reviewer misunderstanding；
- vague / low-quality review；
- baseline coverage；
- comparison fairness；
- ablation；
- small performance gain 与 accuracy-efficiency trade-off；
- computational overhead；
- missing / infeasible experiments；
- dataset scale；
- generalization；
- statistical reliability；
- data leakage；
- hyperparameter sensitivity；
- metric choice；
- intermediate result evaluation；
- longitudinal evidence；
- reproducibility；
- existing rebuttal response review。

另外还包含一条独立的 Workflow，用于把新的 rebuttal 经验整理成结构化 tip contribution。

---

## 仓库结构

```text
paper-rebuttal-router/
├── README.md
├── SKILL.md
├── provenance.json
└── references/
    ├── router.md
    ├── source-materials.json
    ├── traceability.json
    └── workflow-001.md ... workflow-026.md
```

其中：

- `README.md`：安装和使用说明；
- `SKILL.md`：Skill 的入口与行为规则；
- `references/router.md`：Workflow selection 逻辑；
- `references/workflow-*.md`：具体 rebuttal 策略；
- `source-materials.json`、`traceability.json`：记录 Workflow 与源材料之间的关系；
- `provenance.json`：记录构建来源和 build identity。

---

## Validation

最终打包版本完成了一次真实客户端行为评测：

- 14 / 14 个 formal responses 均可评分；
- 172 / 174 项 binary checks 通过；
- 0 / 14 个 critical behavior failures。

评测主要检查：

- reviewer point 的拆分与处理；
- Workflow selection；
- evidence use；
- analysis / review / drafting 的任务边界；
- Workflow execution。
