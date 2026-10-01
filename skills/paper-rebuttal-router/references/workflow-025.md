# Workflow 25: Organize contributed tip material into the four-part card structure

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "organize-tip-card-contribution"
  ],
  "confidence": "high",
  "evidence": [
    {
      "justification": "The four-part table defines the four body parts and their descriptions.",
      "kind": "documentation",
      "locator": "README.md:L44-L47",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The 欢迎贡献 section states the Issue/PR path and the four-part template in this order.",
      "kind": "documentation",
      "locator": "README.md:L449-L462",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The disclaimer block contains the reference-only caveat, the venue-difference warning, and the content-source statement.",
      "kind": "documentation",
      "locator": "README.md:L52-L58",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "L56 states that when venues differ in rebuttal rules, word limits, new-experiment allowance, and external-link allowance, the conference's official instructions take priority (请以会议官方说明为准).",
      "kind": "documentation",
      "locator": "README.md:L56",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The category overview table lists the three groups and their tip ranges.",
      "kind": "documentation",
      "locator": "README.md:L64-L95",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_25.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_26.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Organize user-provided tip material into the repository's documented card structure — a tip title plus four parts (the typical reviewer question or doubt, the pitfall reply style, the recommended reply strategy, and the key takeaway) — and assign the card to one of the three README categories, following the documented contribution path without submitting it.",
  "id": "wf-organize-tip-card-contribution",
  "limitations": [
    "Category membership is taken from the README index; category assignments were not cross-checked against every card's image text.",
    "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
    "The documented path is limited to the text template and submission channel; the README does not describe further validation or review stages.",
    "The structure is stated in the README; the tip SVGs themselves are supplied as Builder visual readings without independent visual review.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only gathers and checks tip material and intent; it does not organize the card and does not submit an Issue or PR."
  ],
  "scope": "Applies to organizing tip material for contribution, not to drafting replies to a user's reviewers. The contribution path is limited to the text template and submission channel (Issue or PR); the workflow does not submit issues or pull requests, and the four-part structure must not be forced onto a real rebuttal reply.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-organize-tip-card-contribution-step1",
      "instruction": "Gather the tip material the user provides and confirm they intend contribution organization (not rebuttal drafting); record any missing parts and the user's preferred or derived README category, without submitting anything.",
      "limitations": [
        "This step only gathers and checks tip material and intent; it does not organize the card and does not submit an Issue or PR."
      ],
      "rationale": "The contribution capability organizes user-provided material and does not submit; the workflow must collect the material and distinguish this intent from rebuttal drafting before applying it.",
      "title": "Gather the user's tip material and contribution intent",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "organize-tip-card-contribution",
      "confidence": "high",
      "depends_on": [
        "wf-organize-tip-card-contribution-step1"
      ],
      "evidence": [
        {
          "justification": "The four-part table defines the four body parts and their descriptions.",
          "kind": "documentation",
          "locator": "README.md:L44-L47",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The 欢迎贡献 section states the Issue/PR path and the four-part template in this order.",
          "kind": "documentation",
          "locator": "README.md:L449-L462",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The disclaimer block contains the reference-only caveat, the venue-difference warning, and the content-source statement.",
          "kind": "documentation",
          "locator": "README.md:L52-L58",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "L56 states that when venues differ in rebuttal rules, word limits, new-experiment allowance, and external-link allowance, the conference's official instructions take priority (请以会议官方说明为准).",
          "kind": "documentation",
          "locator": "README.md:L56",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The category overview table lists the three groups and their tip ranges.",
          "kind": "documentation",
          "locator": "README.md:L64-L95",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_25.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_26.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-organize-tip-card-contribution-step2",
      "instruction": "Apply organize-tip-card-contribution to the user-provided tip material: produce a card with a tip title and the four parts (typical reviewer question or doubt, pitfall reply style, recommended reply strategy, key takeaway), assign it to one of the three README categories, and explain the Issue/PR contribution path without submitting it.",
      "limitations": [
        "Category membership is taken from the README index; category assignments were not cross-checked against every card's image text.",
        "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
        "The documented path is limited to the text template and submission channel; the README does not describe further validation or review stages.",
        "The structure is stated in the README; the tip SVGs themselves are supplied as Builder visual readings without independent visual review.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Organize the tip material into the four-part card and assign a category",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Organize contributed tip material into the four-part card structure"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "high",
    "evidence": [
      {
        "justification": "The four-part table defines the four body parts and their descriptions.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The 欢迎贡献 section states the Issue/PR path and the four-part template in this order.",
        "kind": "documentation",
        "locator": "README.md:L449-L462",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The disclaimer block contains the reference-only caveat, the venue-difference warning, and the content-source statement.",
        "kind": "documentation",
        "locator": "README.md:L52-L58",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "L56 states that when venues differ in rebuttal rules, word limits, new-experiment allowance, and external-link allowance, the conference's official instructions take priority (请以会议官方说明为准).",
        "kind": "documentation",
        "locator": "README.md:L56",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The category overview table lists the three groups and their tip ranges.",
        "kind": "documentation",
        "locator": "README.md:L64-L95",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      }
    ],
    "id": "organize-tip-card-contribution",
    "knowledge_ids": [
      "contribution-procedure",
      "four-part-card-structure",
      "placeholder-token-convention",
      "readme-disclaimer",
      "three-category-grouping"
    ],
    "limitations": [
      "Category membership is taken from the README index; category assignments were not cross-checked against every card's image text.",
      "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
      "The documented path is limited to the text template and submission channel; the README does not describe further validation or review stages.",
      "The structure is stated in the README; the tip SVGs themselves are supplied as Builder visual readings without independent visual review.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies to organizing tip material for contribution, not to drafting replies to a user's reviewers: rebuttal replies are not required to include the pitfall-reply column. The contribution path is limited to the text template and submission channel (Issue or PR); the capability does not submit issues or pull requests. Example prose may use placeholder tokens (XXX, A/B/C, 表 X, XX%) as illustrative fill-ins rather than real values. Category membership comes from the README index, and the four-part structure is stated in the README.",
    "task": "Organize user-provided tip material into the repository's documented card structure — a tip title plus four parts: the typical reviewer question or doubt, the pitfall reply style, the recommended reply strategy, and the key takeaway — and assign the card to one of the three README categories (innovation/motivation/theory/boundaries, writing/related-work/communication, or experiments/evaluation evidence), following the documented contribution path without submitting it.",
    "title": "Organize contributed tip material into the four-part card structure"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "The README documents that new rebuttal content is contributed via Issue or PR, and that when adding new content it should keep a four-part structure in order: first the <Tip 标题>, then 审稿人问题, then 反面回答样式, then 推荐回答样式, then 核心点.",
    "evidence": [
      {
        "justification": "The 欢迎贡献 section states the Issue/PR path and the four-part template in this order.",
        "kind": "documentation",
        "locator": "README.md:L449-L462",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "contribution-procedure",
    "limitations": [
      "The documented path is limited to the text template and submission channel; the README does not describe further validation or review stages."
    ],
    "title": "Documented contribution path via Issue or PR with a four-part template",
    "type": "PROCEDURE"
  },
  {
    "confidence": "high",
    "content": "The README documents that each rebuttal scenario is summarized into four parts: 审稿人问题 (typical reviewer question or doubt), 反面回答 (a pitfall reply style), 推荐回答 (a more effective reply strategy), and 核心点 (key takeaway).",
    "evidence": [
      {
        "justification": "The four-part table defines the four body parts and their descriptions.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "four-part-card-structure",
    "limitations": [
      "The structure is stated in the README; the tip SVGs themselves are supplied as Builder visual readings without independent visual review."
    ],
    "title": "The README documents a four-part structure for each tip scenario",
    "type": "FACT"
  },
  {
    "confidence": "high",
    "content": "Across the inspected tip card visual readings, example rebuttal prose uses placeholder tokens such as XXX, X, A/B/C, N, 表 X, and XX% as illustrative fill-ins for method components, datasets, metrics, hyperparameters, and measured results rather than real values. Examples include Tip 1's component placeholders (A/B/C, XXX), Tip 3's innovation placeholder (XXX), and Tip 25's human-evaluation placeholders (N 名标注者, XXX 个样本, κ = XXX). GPT-4 and Gemini-Pro are not placeholder tokens of this kind: the Tip 26 visual reading records them as the source card's named example judge models, and the claims attached to them (客观裁判, 显著优于) are the source example's wording, not verified tool capability or an independent check.",
    "evidence": [
      {
        "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      }
    ],
    "id": "placeholder-token-convention",
    "limitations": [
      "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards."
    ],
    "title": "Tip card examples routinely use placeholder tokens instead of concrete values",
    "type": "CONVENTION"
  },
  {
    "confidence": "high",
    "content": "The README's 免责声明 block states that all listed techniques are for reference only, do not guarantee correctness, and need not apply to all conferences, fields, or review scenarios. It warns that venues differ in rebuttal rules such as word limits, whether new experiments are allowed, and whether external links are allowed, and that the conference's official instructions take priority where such differences exist (请以会议官方说明为准). It also states that content derives from personal experience, internet data, team research practice, and experienced colleagues.",
    "evidence": [
      {
        "justification": "The disclaimer block contains the reference-only caveat, the venue-difference warning, and the content-source statement.",
        "kind": "documentation",
        "locator": "README.md:L52-L58",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "L56 states that when venues differ in rebuttal rules, word limits, new-experiment allowance, and external-link allowance, the conference's official instructions take priority (请以会议官方说明为准).",
        "kind": "documentation",
        "locator": "README.md:L56",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "readme-disclaimer",
    "limitations": [
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "title": "The README includes a broad disclaimer about tip applicability",
    "type": "FACT"
  },
  {
    "confidence": "high",
    "content": "The README groups the 28 tips into three categories: 创新性、动机、理论与边界类 (Tips 1-7), 写作澄清、相关工作与沟通策略类 (Tips 8-12), and 实验与评测证据类 (Tips 13-28).",
    "evidence": [
      {
        "justification": "The category overview table lists the three groups and their tip ranges.",
        "kind": "documentation",
        "locator": "README.md:L64-L95",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "three-category-grouping",
    "limitations": [
      "Category membership is taken from the README index; category assignments were not cross-checked against every card's image text."
    ],
    "title": "The 28 tips are grouped into three README categories",
    "type": "FACT"
  }
]
```

