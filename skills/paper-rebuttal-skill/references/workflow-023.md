# Workflow 23: Draft a rebuttal for reproducibility concerns

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-reproducibility-response"
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
      "justification": "The core point lists the information to provide now and the condition on acceptance for open-sourcing.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_28.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer enumerates the currently providable experimental details and the conference-rule condition for links.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_28.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that supplies currently available experimental details instead of only promising code later.",
  "id": "wf-draft-reproducibility-response",
  "limitations": [
    "The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when reproducibility is the reviewer's concern. The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided by the repository. Link disclosure during rebuttal is conditional on conference rules, and full code release is conditioned on acceptance. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-reproducibility-response-step1",
      "instruction": "Confirm the reviewer point concerns reproducibility (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the currently available experimental details (main hyperparameters, random seeds, training rounds, batch size, learning rate, hardware environment, data preprocessing, model selection) and the venue's disclosure rules and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-reproducibility-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the reproducibility point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-reproducibility-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-reproducibility-response-step1"
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
          "justification": "The core point lists the information to provide now and the condition on acceptance for open-sourcing.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_28.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer enumerates the currently providable experimental details and the conference-rule condition for links.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_28.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-reproducibility-response-step2",
      "instruction": "Apply draft-reproducibility-response using the user's real facts: supply currently available details such as main hyperparameters, random seeds, training rounds, batch size, learning rate, hardware environment, data preprocessing, and model selection details, rather than only promising to provide code later.",
      "limitations": [
        "The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the reproducibility reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-reproducibility-response-step2"
      ],
      "id": "wf-draft-reproducibility-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-reproducibility-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for reproducibility concerns"
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
        "justification": "The core point lists the information to provide now and the condition on acceptance for open-sourcing.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_28.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer enumerates the currently providable experimental details and the conference-rule condition for links.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_28.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-reproducibility-response",
    "knowledge_ids": [
      "decide-reproducibility-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when reproducibility is the reviewer's concern. The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided by the repository. Link disclosure during rebuttal is conditional on conference rules, and full code release is conditioned on acceptance.",
    "task": "Draft a rebuttal response to a reproducibility concern by supplying currently available details such as main hyperparameters, random seeds, training rounds, batch size, learning rate, hardware environment, data preprocessing, and model selection details, rather than only promising to provide code later.",
    "title": "Draft a rebuttal for reproducibility concerns"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "For reproducibility concerns, the documented rule (Tip 28) is not to only promise to provide code later. Authors should supply currently available information such as main hyperparameters, random seeds, training rounds, batch size, learning rate, hardware environment, data preprocessing, and model selection details, and may prepare an anonymous code repository. Link disclosure during rebuttal/supplementary material is conditional on conference rules, and full code release is conditioned on acceptance.",
    "evidence": [
      {
        "justification": "The core point lists the information to provide now and the condition on acceptance for open-sourcing.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_28.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer enumerates the currently providable experimental details and the conference-rule condition for links.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_28.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-reproducibility-response",
    "limitations": [
      "The anonymous repository and detailed settings are example states in the card; no actual URL or configuration values are provided."
    ],
    "title": "For reproducibility concerns provide currently available details instead of only promising code",
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

