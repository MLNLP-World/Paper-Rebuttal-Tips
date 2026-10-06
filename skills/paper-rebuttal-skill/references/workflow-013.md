# Workflow 13: Draft a rebuttal for limitation critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-limitations-response"
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
      "justification": "The conditions record the three named limitations and the RL-paradigm future plan.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_07.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point prescribes concrete limitations such as capability thresholds, negative transfer, and no-benefit effects instead of generic compute excuses.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_07.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the base-model-dependence, negative-transfer, and cognitive-ceiling limitations.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_07.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that names concrete limitations true of the user's method and keeps future-work plans explicitly as plans.",
  "id": "wf-draft-limitations-response",
  "limitations": [
    "Literature placeholders X and Y are unnamed; no real citations are supplied.",
    "The RL-style future plan is a plan, not a verified result.",
    "The named limitations are the card's examples and do not apply to every method.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when a reviewer asks for limitations or a weakness discussion. The named limitations are the card's examples and do not apply to every method; the user supplies the limitations true of their own method. The RL-style future plan and the literature citations are plans and unnamed placeholders (X, Y), not verified results or real citations. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-limitations-response-step1",
      "instruction": "Confirm the reviewer point concerns limitations (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the limitations true of the user's method and the future-work plans and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-limitations-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the limitations point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-limitations-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-limitations-response-step1"
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
          "justification": "The conditions record the three named limitations and the RL-paradigm future plan.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_07.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point prescribes concrete limitations such as capability thresholds, negative transfer, and no-benefit effects instead of generic compute excuses.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_07.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the base-model-dependence, negative-transfer, and cognitive-ceiling limitations.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_07.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-limitations-response-step2",
      "instruction": "Apply draft-limitations-response using the user's real facts: name concrete limitations true of the user's method (such as capability thresholds, negative transfer, or no-benefit effects) and keep future-work plans explicitly as plans, rather than answering with generic compute excuses.",
      "limitations": [
        "Literature placeholders X and Y are unnamed; no real citations are supplied.",
        "The RL-style future plan is a plan, not a verified result.",
        "The named limitations are the card's examples and do not apply to every method.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the limitations reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-limitations-response-step2"
      ],
      "id": "wf-draft-limitations-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-limitations-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for limitation critiques"
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
        "justification": "The conditions record the three named limitations and the RL-paradigm future plan.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes concrete limitations such as capability thresholds, negative transfer, and no-benefit effects instead of generic compute excuses.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the base-model-dependence, negative-transfer, and cognitive-ceiling limitations.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-limitations-response",
    "knowledge_ids": [
      "decide-specific-limitations-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "Literature placeholders X and Y are unnamed; no real citations are supplied.",
      "The RL-style future plan is a plan, not a verified result.",
      "The named limitations are the card's examples and do not apply to every method.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer asks for limitations or a weakness discussion. The named limitations are the card's examples and do not apply to every method; the user supplies the limitations true of their own method. The RL-style future plan and the literature citations are plans and unnamed placeholders (X, Y), not verified results or real citations.",
    "task": "Draft a rebuttal response to a reviewer who asks about limitations, by naming concrete limitations such as capability thresholds, negative transfer, and no-benefit effects, and keeping future-work plans explicitly as plans, rather than answering with generic compute excuses.",
    "title": "Draft a rebuttal for limitation critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When asked about limitations, the documented rule (Tip 7) is not to answer generically with insufficient compute and future optimization. Instead, name concrete limitations such as capability thresholds, negative transfer, and no-benefit effects. The example revision adds a limitations section: the method depends on the base model's initial capability, and adding overly complex extra modules to a weak model may interfere with its original behavior (negative transfer); non-parametric extraction is limited by the model's cognitive ceiling; and future work will explore reinforcement-learning-style paradigms (citing recent literature X, Y).",
    "evidence": [
      {
        "justification": "The conditions record the three named limitations and the RL-paradigm future plan.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes concrete limitations such as capability thresholds, negative transfer, and no-benefit effects instead of generic compute excuses.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the base-model-dependence, negative-transfer, and cognitive-ceiling limitations.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_07.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-specific-limitations-response",
    "limitations": [
      "Literature placeholders X and Y are unnamed; no real citations are supplied.",
      "The RL-style future plan is a plan, not a verified result.",
      "The named limitations are the card's examples and do not apply to every method."
    ],
    "title": "For limitation critiques, name concrete limitations instead of generic compute excuses",
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

