# Workflow 19: Draft a rebuttal for weak-motivation critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-motivation-response"
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
      "justification": "The conditions record the unsolved-consequence-cost framing and the introduction supplement commitment.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_05.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point prescribes a concrete use case plus the unsolved cost instead of paraphrasing the abstract.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_05.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the scenario-consequence-cost structure and the mechanism closing the loop.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_05.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that anchors the problem's importance in a concrete use case, the unsolved cost, and a motivation-method-experiment loop.",
  "id": "wf-draft-motivation-response",
  "limitations": [
    "All scenario, consequence, cost, and mechanism tokens are XXX placeholders; the card supplies no actual case or quantified cost.",
    "The introduction supplement (我们将在引言中补充) is the example answer's promise, not an executed result.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when a reviewer questions whether the problem is worth solving. The scenario, consequence, and cost must come from the user's real application; the card's XXX tokens are placeholders. The introduction supplement is a revision commitment, not an executed edit. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-motivation-response-step1",
      "instruction": "Confirm the reviewer point concerns problem motivation (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's concrete use case, the cost of leaving the problem unsolved, and the motivation-method-experiment links and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-motivation-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the problem motivation point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-motivation-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-motivation-response-step1"
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
          "justification": "The conditions record the unsolved-consequence-cost framing and the introduction supplement commitment.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_05.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point prescribes a concrete use case plus the unsolved cost instead of paraphrasing the abstract.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_05.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the scenario-consequence-cost structure and the mechanism closing the loop.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_05.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-motivation-response-step2",
      "instruction": "Apply draft-motivation-response using the user's real facts: anchor the importance in a concrete use case plus the cost of leaving the problem unsolved and connect motivation, method, and experiments as a closed logical loop, rather than re-stating the abstract or the introduction.",
      "limitations": [
        "All scenario, consequence, cost, and mechanism tokens are XXX placeholders; the card supplies no actual case or quantified cost.",
        "The introduction supplement (我们将在引言中补充) is the example answer's promise, not an executed result.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the problem motivation reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-motivation-response-step2"
      ],
      "id": "wf-draft-motivation-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-motivation-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for weak-motivation critiques"
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
        "justification": "The conditions record the unsolved-consequence-cost framing and the introduction supplement commitment.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes a concrete use case plus the unsolved cost instead of paraphrasing the abstract.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the scenario-consequence-cost structure and the mechanism closing the loop.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-motivation-response",
    "knowledge_ids": [
      "decide-motivation-specificity-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "All scenario, consequence, cost, and mechanism tokens are XXX placeholders; the card supplies no actual case or quantified cost.",
      "The introduction supplement (我们将在引言中补充) is the example answer's promise, not an executed result.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer questions whether the problem is worth solving. The scenario, consequence, and cost must come from the user's real application; the card's XXX tokens are placeholders. The introduction supplement is a revision commitment, not an executed edit.",
    "task": "Draft a rebuttal response to a reviewer who finds the problem motivation insufficient, by anchoring the importance in a concrete use case plus the cost of leaving the problem unsolved and connecting motivation, method, and experiments as a closed logical loop, rather than re-stating the abstract or the introduction.",
    "title": "Draft a rebuttal for weak-motivation critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer finds the problem motivation insufficient, the documented rule (Tip 5) is not to re-state the abstract or the introduction in other words. Instead, anchor the importance in a concrete use case plus the cost of leaving the problem unsolved. The example adds an application scenario to the introduction: in the XXX scenario, if XXX remains unsolved, the system shows XXX consequences at XXX cost, and it explains how this paper's XXX mechanism alleviates that bottleneck so that motivation, method, and experiments form a closed logical loop.",
    "evidence": [
      {
        "justification": "The conditions record the unsolved-consequence-cost framing and the introduction supplement commitment.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes a concrete use case plus the unsolved cost instead of paraphrasing the abstract.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the scenario-consequence-cost structure and the mechanism closing the loop.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_05.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-motivation-specificity-response",
    "limitations": [
      "All scenario, consequence, cost, and mechanism tokens are XXX placeholders; the card supplies no actual case or quantified cost.",
      "The introduction supplement (我们将在引言中补充) is the example answer's promise, not an executed result."
    ],
    "title": "For weak-motivation critiques, anchor importance in a concrete use case and unsolved cost",
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

