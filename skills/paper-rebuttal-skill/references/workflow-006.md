# Workflow 6: Draft a rebuttal for data-scale critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-data-scale-response"
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
      "justification": "The conditions record the example status of the added statistics and dataset-B experiment and the remaining larger-scale validation need.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_19.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires explaining the dataset choice and stating whether experiments are added or conclusions narrowed.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_19.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the prior-work dataset justification and the data-statistics plus dataset-B supplement.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_19.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that explains the dataset choice and either adds experiments and statistics or narrows the conclusions with a scale limitation.",
  "id": "wf-draft-data-scale-response",
  "limitations": [
    "Dataset B and the XXX scenario tokens remain unnamed; no real dataset facts are supplied.",
    "The added statistics and dataset-B experiment are example states in the card.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when dataset size or scale is the reviewer's concern. Dataset names and scenario coverage come from the user's real data (Dataset B and XXX are placeholders), and added statistics and experiments are example states in the card, not completed work. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-data-scale-response-step1",
      "instruction": "Confirm the reviewer point concerns data scale (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's dataset choice and its rationale, plus any added experiments, statistics, or scale limitations and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-data-scale-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the data scale point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-data-scale-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-data-scale-response-step1"
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
          "justification": "The conditions record the example status of the added statistics and dataset-B experiment and the remaining larger-scale validation need.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_19.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires explaining the dataset choice and stating whether experiments are added or conclusions narrowed.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_19.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the prior-work dataset justification and the data-statistics plus dataset-B supplement.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_19.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-data-scale-response-step2",
      "instruction": "Apply draft-data-scale-response using the user's real facts: explain why the dataset was chosen (such as prior-work alignment and fair comparison) and either add experiments and statistics or narrow the conclusions with a limitations note that larger-scale validation is still needed, rather than claiming the existing results already prove effectiveness.",
      "limitations": [
        "Dataset B and the XXX scenario tokens remain unnamed; no real dataset facts are supplied.",
        "The added statistics and dataset-B experiment are example states in the card.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the data scale reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-data-scale-response-step2"
      ],
      "id": "wf-draft-data-scale-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-data-scale-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for data-scale critiques"
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
        "justification": "The conditions record the example status of the added statistics and dataset-B experiment and the remaining larger-scale validation need.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires explaining the dataset choice and stating whether experiments are added or conclusions narrowed.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the prior-work dataset justification and the data-statistics plus dataset-B supplement.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-data-scale-response",
    "knowledge_ids": [
      "decide-data-scale-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "Dataset B and the XXX scenario tokens remain unnamed; no real dataset facts are supplied.",
      "The added statistics and dataset-B experiment are example states in the card.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when dataset size or scale is the reviewer's concern. Dataset names and scenario coverage come from the user's real data (Dataset B and XXX are placeholders), and added statistics and experiments are example states in the card, not completed work.",
    "task": "Draft a rebuttal response to a reviewer who questions the data scale, by explaining why the dataset was chosen (such as prior-work alignment and fair comparison) and either adding experiments and statistics or narrowing the conclusions with a limitations note that larger-scale validation is still needed, rather than claiming the existing results already prove effectiveness.",
    "title": "Draft a rebuttal for data-scale critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When reviewers question the data scale, the documented rule (Tip 19) is not to claim the existing results already prove effectiveness. Explain why the dataset was chosen — the example follows prior work in selecting a classical dataset that covers XXX scenarios and enables fair comparison with existing methods — and either add experiments (the example adds data statistics and a dataset-B experiment) or narrow the conclusions, stating in the limitations that the conclusion still needs validation on larger-scale data.",
    "evidence": [
      {
        "justification": "The conditions record the example status of the added statistics and dataset-B experiment and the remaining larger-scale validation need.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires explaining the dataset choice and stating whether experiments are added or conclusions narrowed.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the prior-work dataset justification and the data-statistics plus dataset-B supplement.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_19.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-data-scale-response",
    "limitations": [
      "Dataset B and the XXX scenario tokens remain unnamed; no real dataset facts are supplied.",
      "The added statistics and dataset-B experiment are example states in the card."
    ],
    "title": "For small-dataset critiques, justify dataset choice and add experiments or narrow conclusions",
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

