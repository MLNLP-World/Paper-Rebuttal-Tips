# Workflow 24: Draft a rebuttal for small-improvement critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-small-gain-response"
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
      "justification": "The conditions record the cost/stability/generalization alternatives and the revision commitments.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_14.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires interpreting small gains with task difficulty, stability, cost, robustness, and statistical significance.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_14.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the three-point gain interpretation and the significance/variance revision commitment.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_14.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that interprets the small gain with task difficulty, stability, cost, and robustness instead of resting on a single metric.",
  "id": "wf-draft-small-gain-response",
  "limitations": [
    "Statistical significance cannot be inferred from the example wording; it is a revision commitment in the card.",
    "The card gives no concrete gain, variance, or significance values.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when the improvement size is the reviewer's concern. Statistical significance and variance results are revision commitments, not inferred results, and the card supplies no concrete gain, variance, or significance values. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-small-gain-response-step1",
      "instruction": "Confirm the reviewer point concerns the size of the improvement (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual gain and the task-difficulty, stability, cost, and robustness facts around it and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-small-gain-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the the size of the improvement point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-small-gain-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-small-gain-response-step1"
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
          "justification": "The conditions record the cost/stability/generalization alternatives and the revision commitments.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_14.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires interpreting small gains with task difficulty, stability, cost, robustness, and statistical significance.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_14.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the three-point gain interpretation and the significance/variance revision commitment.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_14.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-small-gain-response-step2",
      "instruction": "Apply draft-small-gain-response using the user's real facts: interpret the gain with task difficulty, stability, cost, and robustness so the contribution does not rest on a single metric, rather than insisting only that the method still beats the baseline.",
      "limitations": [
        "Statistical significance cannot be inferred from the example wording; it is a revision commitment in the card.",
        "The card gives no concrete gain, variance, or significance values.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the the size of the improvement reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-small-gain-response-step2"
      ],
      "id": "wf-draft-small-gain-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-small-gain-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for small-improvement critiques"
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
        "justification": "The conditions record the cost/stability/generalization alternatives and the revision commitments.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires interpreting small gains with task difficulty, stability, cost, robustness, and statistical significance.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the three-point gain interpretation and the significance/variance revision commitment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-small-gain-response",
    "knowledge_ids": [
      "decide-small-gain-context-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "Statistical significance cannot be inferred from the example wording; it is a revision commitment in the card.",
      "The card gives no concrete gain, variance, or significance values.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when the improvement size is the reviewer's concern. Statistical significance and variance results are revision commitments, not inferred results, and the card supplies no concrete gain, variance, or significance values.",
    "task": "Draft a rebuttal response to a reviewer who notes the improvement is small, by interpreting the gain with task difficulty, stability, cost, and robustness so the contribution does not rest on a single metric, rather than insisting only that the method still beats the baseline.",
    "title": "Draft a rebuttal for small-improvement critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When reviewers note that the improvement is small, the documented rule (Tip 14) is not to insist only that the method still beats the baseline. Interpret the gain with task difficulty, stability, cost, robustness, and statistical significance. The example makes three points: a XXX gain over the strongest baseline on the main metric; a larger gain in more difficult settings (e.g., XXX); and simultaneously lower compute cost, better stability, or stronger generalization, so the contribution does not rest on a single metric; the revision will add statistical significance, variance results, and per-scenario performance-difference explanations.",
    "evidence": [
      {
        "justification": "The conditions record the cost/stability/generalization alternatives and the revision commitments.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires interpreting small gains with task difficulty, stability, cost, robustness, and statistical significance.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the three-point gain interpretation and the significance/variance revision commitment.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_14.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-small-gain-context-response",
    "limitations": [
      "Statistical significance cannot be inferred from the example wording; it is a revision commitment in the card.",
      "The card gives no concrete gain, variance, or significance values."
    ],
    "title": "For small-gain critiques, explain gains with task difficulty, cost, stability, and significance",
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

