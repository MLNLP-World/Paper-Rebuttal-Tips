# Workflow 10: Draft a rebuttal for infeasible-experiment critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-infeasible-experiment-response"
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
      "justification": "The conditions record the rebuttal-cycle constraint, the representative-experiment framing, and the potential-not-completion status.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_18.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires quantifying the full cost, adding a representative experiment, explaining its reference value, and stating the completion plan.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_18.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the GPU-hours quantification and the representative small-scale experiment.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_18.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that quantifies the full experiment's cost, adds a representative small-scale experiment, and states the completion plan.",
  "id": "wf-draft-infeasible-experiment-response",
  "limitations": [
    "A small-scale result is a preliminary reference point, not completion of the large-scale validation.",
    "GPU hours, cards, days, and the small experiment's values are placeholders; no real cost or results are supplied.",
    "The stability claim in the example answer is example phrasing, not an executed result.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when the requested experiment is infeasible within the rebuttal period. A small-scale result is a preliminary reference point, not completion of the large-scale validation, and GPU hours, cards, days, and small-experiment values are placeholders until the user supplies real numbers. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-infeasible-experiment-response-step1",
      "instruction": "Confirm the reviewer point concerns an infeasible requested experiment (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the requested experiment's concrete cost estimates and which representative small-scale version is feasible and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-infeasible-experiment-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the an infeasible requested experiment point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-infeasible-experiment-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-infeasible-experiment-response-step1"
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
          "justification": "The conditions record the rebuttal-cycle constraint, the representative-experiment framing, and the potential-not-completion status.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_18.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires quantifying the full cost, adding a representative experiment, explaining its reference value, and stating the completion plan.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_18.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the GPU-hours quantification and the representative small-scale experiment.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_18.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-infeasible-experiment-response-step2",
      "instruction": "Apply draft-infeasible-experiment-response using the user's real facts: quantify the full experiment's concrete cost, add a representative small-scale experiment that directly targets the reviewer's core question where possible, explain why the small result is still a useful reference point, and state how the larger experiment will be completed afterwards, rather than simply saying it cannot be done.",
      "limitations": [
        "A small-scale result is a preliminary reference point, not completion of the large-scale validation.",
        "GPU hours, cards, days, and the small experiment's values are placeholders; no real cost or results are supplied.",
        "The stability claim in the example answer is example phrasing, not an executed result.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the an infeasible requested experiment reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-infeasible-experiment-response-step2"
      ],
      "id": "wf-draft-infeasible-experiment-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-infeasible-experiment-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for infeasible-experiment critiques"
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
        "justification": "The conditions record the rebuttal-cycle constraint, the representative-experiment framing, and the potential-not-completion status.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires quantifying the full cost, adding a representative experiment, explaining its reference value, and stating the completion plan.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the GPU-hours quantification and the representative small-scale experiment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-infeasible-experiment-response",
    "knowledge_ids": [
      "decide-costed-representative-experiment-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "A small-scale result is a preliminary reference point, not completion of the large-scale validation.",
      "GPU hours, cards, days, and the small experiment's values are placeholders; no real cost or results are supplied.",
      "The stability claim in the example answer is example phrasing, not an executed result.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when the requested experiment is infeasible within the rebuttal period. A small-scale result is a preliminary reference point, not completion of the large-scale validation, and GPU hours, cards, days, and small-experiment values are placeholders until the user supplies real numbers.",
    "task": "Draft a rebuttal response to a reviewer who asks for an experiment that cannot be completed in the rebuttal period, by quantifying the full experiment's concrete cost, adding a representative small-scale experiment that directly targets the reviewer's core question where possible, explaining why the small result is still a useful reference point, and stating how the larger experiment will be completed afterwards, rather than simply saying it cannot be done.",
    "title": "Draft a rebuttal for infeasible-experiment critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer asks for an experiment that cannot be completed in the rebuttal period, the documented rule (Tip 18) is not to simply say it cannot be done. Quantify the full experiment's concrete cost — the example names about XXX GPU hours / XX cards running XX days — and, where possible, add a representative small-scale experiment that directly targets the reviewer's core question (XXX), explain why the small result is still a useful reference point, and state how the larger experiment will be completed afterwards. A small-scale result is preliminary potential, not completion of large-scale validation.",
    "evidence": [
      {
        "justification": "The conditions record the rebuttal-cycle constraint, the representative-experiment framing, and the potential-not-completion status.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires quantifying the full cost, adding a representative experiment, explaining its reference value, and stating the completion plan.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the GPU-hours quantification and the representative small-scale experiment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_18.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-costed-representative-experiment-response",
    "limitations": [
      "A small-scale result is a preliminary reference point, not completion of the large-scale validation.",
      "GPU hours, cards, days, and the small experiment's values are placeholders; no real cost or results are supplied.",
      "The stability claim in the example answer is example phrasing, not an executed result."
    ],
    "title": "For infeasible-experiment critiques, quantify the full cost and add a representative experiment",
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

