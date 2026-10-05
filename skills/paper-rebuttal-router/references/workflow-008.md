# Workflow 8: Draft a rebuttal for comparison-fairness critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-fairness-details-response"
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
      "justification": "The conditions record the configuration-table commitment and the identical/default/extra-budget distinction.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_15.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires specifying data splits, training rounds, models, seeds, hyperparameter search, and compute budget.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_15.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the shared-settings enumeration and the per-method hyperparameter policy.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_15.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that specifies what is actually shared across compared methods and how the rest is controlled.",
  "id": "wf-draft-fairness-details-response",
  "limitations": [
    "The configuration table is a revision commitment in the card, not a supplied artifact.",
    "The example states the shared-settings claim but supplies no actual configuration values.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when the fairness of the comparison is questioned. The configuration table distinguishing fully identical settings, per-method defaults, and extra compute budget is a revision commitment, not a supplied artifact, and the card supplies no actual configuration values. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-fairness-details-response-step1",
      "instruction": "Confirm the reviewer point concerns comparison fairness (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect what is actually shared across the compared methods in the user's setup and how the rest is controlled and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-fairness-details-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the comparison fairness point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-fairness-details-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-fairness-details-response-step1"
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
          "justification": "The conditions record the configuration-table commitment and the identical/default/extra-budget distinction.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_15.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires specifying data splits, training rounds, models, seeds, hyperparameter search, and compute budget.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_15.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the shared-settings enumeration and the per-method hyperparameter policy.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_15.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-fairness-details-response-step2",
      "instruction": "Apply draft-fairness-details-response using the user's real facts: specify what is actually shared across methods (data splits, training rounds, model backbone, evaluation metrics, random seeds) and how the rest is controlled (the original papers' recommended settings or validation-set tuning for method-specific hyperparameters, and any extra compute budget), rather than asserting that all experimental settings are reasonable.",
      "limitations": [
        "The configuration table is a revision commitment in the card, not a supplied artifact.",
        "The example states the shared-settings claim but supplies no actual configuration values.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the comparison fairness reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-fairness-details-response-step2"
      ],
      "id": "wf-draft-fairness-details-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-fairness-details-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for comparison-fairness critiques"
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
        "justification": "The conditions record the configuration-table commitment and the identical/default/extra-budget distinction.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires specifying data splits, training rounds, models, seeds, hyperparameter search, and compute budget.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the shared-settings enumeration and the per-method hyperparameter policy.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-fairness-details-response",
    "knowledge_ids": [
      "decide-fairness-details-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "The configuration table is a revision commitment in the card, not a supplied artifact.",
      "The example states the shared-settings claim but supplies no actual configuration values.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when the fairness of the comparison is questioned. The configuration table distinguishing fully identical settings, per-method defaults, and extra compute budget is a revision commitment, not a supplied artifact, and the card supplies no actual configuration values.",
    "task": "Draft a rebuttal response to a reviewer who questions the fairness of a comparison, by specifying what is actually shared across methods (data splits, training rounds, model backbone, evaluation metrics, random seeds) and how the rest is controlled (the original papers' recommended settings or validation-set tuning for method-specific hyperparameters, and any extra compute budget), rather than asserting that all experimental settings are reasonable.",
    "title": "Draft a rebuttal for comparison-fairness critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When the fairness of a comparison is questioned, the documented rule (Tip 15) is not to assert that all experimental settings are reasonable. Specify what is actually shared and how the rest is controlled: the example keeps identical data splits, training rounds, model backbone, evaluation metrics, and random seeds across all methods; for method-specific hyperparameters it uses the original paper's recommended settings or tunes on the validation set; and the revision will add an experiment configuration table distinguishing fully identical settings, per-method default configurations, and any extra compute budget with how it is controlled.",
    "evidence": [
      {
        "justification": "The conditions record the configuration-table commitment and the identical/default/extra-budget distinction.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires specifying data splits, training rounds, models, seeds, hyperparameter search, and compute budget.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the shared-settings enumeration and the per-method hyperparameter policy.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_15.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-fairness-details-response",
    "limitations": [
      "The configuration table is a revision commitment in the card, not a supplied artifact.",
      "The example states the shared-settings claim but supplies no actual configuration values."
    ],
    "title": "For fairness critiques, specify data splits, rounds, models, seeds, tuning, and budget",
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

