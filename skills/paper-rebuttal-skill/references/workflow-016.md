# Workflow 16: Draft a rebuttal for metric-choice critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-metric-response"
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
      "justification": "The conditions record the example-status of the added experiment and the consistent conclusion.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_24.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires keeping the fair-comparison metric, adding the suggested metric, verifying consistency, and explaining each metric's focus.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_24.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the A/B/C fair-comparison rationale and the added-metric experiment.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_24.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that keeps the fair-comparison metric, adds the reviewer-suggested metric, and explains what each measures.",
  "id": "wf-draft-metric-response",
  "limitations": [
    "A, B, C baseline names and the XXX metric tokens are placeholders; no real metric results are supplied.",
    "The added-metric advantage claim in the example is example phrasing, not an executed experiment.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when the metric choice is the reviewer's concern. Baseline names and metric tokens are placeholders, and the added-metric advantage is example phrasing, not an executed experiment. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-metric-response-step1",
      "instruction": "Confirm the reviewer point concerns the metric choice (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the original metric, the reviewer-suggested metric, and what each measures in the user's task and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-metric-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the the metric choice point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-metric-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-metric-response-step1"
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
          "justification": "The conditions record the example-status of the added experiment and the consistent conclusion.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_24.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires keeping the fair-comparison metric, adding the suggested metric, verifying consistency, and explaining each metric's focus.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_24.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the A/B/C fair-comparison rationale and the added-metric experiment.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_24.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-metric-response-step2",
      "instruction": "Apply draft-metric-response using the user's real facts: explain that the original metric keeps fair comparison with existing baselines, add the reviewer-suggested metric that measures the task property more directly, verify whether the conclusion still holds, and explain what each metric measures, rather than answering only that the metric is standard in the field.",
      "limitations": [
        "A, B, C baseline names and the XXX metric tokens are placeholders; no real metric results are supplied.",
        "The added-metric advantage claim in the example is example phrasing, not an executed experiment.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the the metric choice reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-metric-response-step2"
      ],
      "id": "wf-draft-metric-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-metric-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for metric-choice critiques"
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
        "justification": "The conditions record the example-status of the added experiment and the consistent conclusion.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires keeping the fair-comparison metric, adding the suggested metric, verifying consistency, and explaining each metric's focus.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the A/B/C fair-comparison rationale and the added-metric experiment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-metric-response",
    "knowledge_ids": [
      "decide-metric-justification-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "A, B, C baseline names and the XXX metric tokens are placeholders; no real metric results are supplied.",
      "The added-metric advantage claim in the example is example phrasing, not an executed experiment.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when the metric choice is the reviewer's concern. Baseline names and metric tokens are placeholders, and the added-metric advantage is example phrasing, not an executed experiment.",
    "task": "Draft a rebuttal response to a reviewer who questions the chosen metric, by explaining that the original metric keeps fair comparison with existing baselines, adding the reviewer-suggested metric that measures the task property more directly, verifying whether the conclusion still holds, and explaining what each metric measures, rather than answering only that the metric is standard in the field.",
    "title": "Draft a rebuttal for metric-choice critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer questions the chosen metric, the documented rule (Tip 24) is not to answer only that the metric is standard in the field. First explain that the original metric keeps fair comparison with existing baselines (the example names A, B, C); then add the reviewer-suggested metric that measures the task property (XXX) more directly and report its results (表 X); verify whether the conclusion still holds; and explain what each metric measures so no single favorable metric carries the conclusion.",
    "evidence": [
      {
        "justification": "The conditions record the example-status of the added experiment and the consistent conclusion.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires keeping the fair-comparison metric, adding the suggested metric, verifying consistency, and explaining each metric's focus.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the A/B/C fair-comparison rationale and the added-metric experiment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_24.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-metric-justification-response",
    "limitations": [
      "A, B, C baseline names and the XXX metric tokens are placeholders; no real metric results are supplied.",
      "The added-metric advantage claim in the example is example phrasing, not an executed experiment."
    ],
    "title": "For metric-choice critiques, keep the comparable metric and add the suggested one with results",
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

