# Workflow 9: Draft a rebuttal for generalization critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-generalization-response"
  ],
  "confidence": "high",
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
    },
    {
      "justification": "The conditions record that the current coverage is only 初步验证 and that the failure-boundary discussion is a revision commitment.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_20.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires cross-dataset, cross-model, cross-task, or failure-case analysis instead of a bare representativeness claim.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_20.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the extra dataset/model supplement and the cross-setting analysis commitment.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_20.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that proposes cross-dataset, cross-model, cross-task, or failure-case analysis instead of a one-sentence representativeness claim.",
  "id": "wf-draft-generalization-response",
  "limitations": [
    "Preliminary validation must not be reported as established generalization.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied.",
    "XXX and XX are placeholder scenario and architecture tokens; no real coverage facts are supplied."
  ],
  "scope": "Applies when generalization is the reviewer's concern. Current coverage in the example supports only preliminary validation, which must not be reported as established generalization; the extra dataset/model and scenario tokens are placeholders until the user supplies real coverage facts. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-generalization-response-step1",
      "instruction": "Confirm the reviewer point concerns generalization (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual dataset, model, and task coverage plus any failure-case facts and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-generalization-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the generalization point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-generalization-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-generalization-response-step1"
      ],
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
        },
        {
          "justification": "The conditions record that the current coverage is only 初步验证 and that the failure-boundary discussion is a revision commitment.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_20.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires cross-dataset, cross-model, cross-task, or failure-case analysis instead of a bare representativeness claim.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_20.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the extra dataset/model supplement and the cross-setting analysis commitment.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_20.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-generalization-response-step2",
      "instruction": "Apply draft-generalization-response using the user's real facts: propose cross-dataset, cross-model, cross-task, or failure-case analysis and discuss applicable scenarios and possible failure boundaries, rather than answering with one sentence that the current datasets and models are representative.",
      "limitations": [
        "Preliminary validation must not be reported as established generalization.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "XXX and XX are placeholder scenario and architecture tokens; no real coverage facts are supplied."
      ],
      "title": "Draft the generalization reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-generalization-response-step2"
      ],
      "id": "wf-draft-generalization-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-generalization-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for generalization critiques"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "high",
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
      },
      {
        "justification": "The conditions record that the current coverage is only 初步验证 and that the failure-boundary discussion is a revision commitment.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires cross-dataset, cross-model, cross-task, or failure-case analysis instead of a bare representativeness claim.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the extra dataset/model supplement and the cross-setting analysis commitment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-generalization-response",
    "knowledge_ids": [
      "decide-generalization-evidence-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "Preliminary validation must not be reported as established generalization.",
      "This records the repository's own stated caveat, not an independent verification of tip quality.",
      "XXX and XX are placeholder scenario and architecture tokens; no real coverage facts are supplied."
    ],
    "scope": "Applies when generalization is the reviewer's concern. Current coverage in the example supports only preliminary validation, which must not be reported as established generalization; the extra dataset/model and scenario tokens are placeholders until the user supplies real coverage facts.",
    "task": "Draft a rebuttal response to a reviewer who doubts generalization, by proposing cross-dataset, cross-model, cross-task, or failure-case analysis and discussing applicable scenarios and possible failure boundaries, rather than answering with one sentence that the current datasets and models are representative.",
    "title": "Draft a rebuttal for generalization critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When generalization is doubted, the documented rule (Tip 20) is not to answer with one sentence that the current datasets and models are representative. The current coverage in the example supports only 初步验证 (preliminary validation). Better: add cross-dataset, cross-model, cross-task, or failure-case analysis. The example adds results on an extra dataset/model (XXX) together with cross-dataset, cross-model, or cross-task analysis, and the revision will discuss the applicable scenarios and possible failure boundaries. Preliminary validation must not be reported as established generalization.",
    "evidence": [
      {
        "justification": "The conditions record that the current coverage is only 初步验证 and that the failure-boundary discussion is a revision commitment.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires cross-dataset, cross-model, cross-task, or failure-case analysis instead of a bare representativeness claim.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the extra dataset/model supplement and the cross-setting analysis commitment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_20.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-generalization-evidence-response",
    "limitations": [
      "Preliminary validation must not be reported as established generalization.",
      "XXX and XX are placeholder scenario and architecture tokens; no real coverage facts are supplied."
    ],
    "title": "For generalization critiques, add cross-dataset/model/task or failure-case evidence",
    "type": "DECISION_RULE"
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
  }
]
```

