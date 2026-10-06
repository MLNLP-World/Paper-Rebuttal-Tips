# Workflow 15: Draft a rebuttal for missing-theory critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-mechanism-and-theory-response"
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
      "justification": "The conditions record the assumption and failure-boundary framing.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_06.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires explaining the mechanism, assumptions, and boundary, with a full theorem not mandatory.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_06.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the intuition-under-assumption chain and the three-part analytic supplement.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_06.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that explains the mechanism, its assumptions, and its failure boundary instead of claiming validity from experimental performance.",
  "id": "wf-draft-mechanism-and-theory-response",
  "limitations": [
    "Experimental performance cannot substitute for a mechanism explanation.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied.",
    "XXX and M1/M2 are placeholder labels, not measurements or named components."
  ],
  "scope": "Applies when a reviewer asks for theory or mechanism justification. The intuition-under-assumption chain and the analytic statement covering the core assumptions, the relation between key steps and the objective/representation space, and the failure boundary are filled from the user's own method; M1/M2 and XXX are placeholders. Experimental performance cannot substitute for the mechanism explanation. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-mechanism-and-theory-response-step1",
      "instruction": "Confirm the reviewer point concerns theory or mechanism justification (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's method mechanism, its assumptions, and the boundary where it may fail and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-mechanism-and-theory-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the theory or mechanism justification point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-mechanism-and-theory-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-mechanism-and-theory-response-step1"
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
          "justification": "The conditions record the assumption and failure-boundary framing.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_06.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires explaining the mechanism, assumptions, and boundary, with a full theorem not mandatory.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_06.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the intuition-under-assumption chain and the three-part analytic supplement.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_06.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-mechanism-and-theory-response-step2",
      "instruction": "Apply draft-mechanism-and-theory-response using the user's real facts: explain the mechanism, its assumptions, and the boundary where the method may fail, with a complete theorem explicitly not mandatory, rather than claiming validity merely from experimental performance.",
      "limitations": [
        "Experimental performance cannot substitute for a mechanism explanation.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "XXX and M1/M2 are placeholder labels, not measurements or named components."
      ],
      "title": "Draft the theory or mechanism justification reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-mechanism-and-theory-response-step2"
      ],
      "id": "wf-draft-mechanism-and-theory-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-mechanism-and-theory-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for missing-theory critiques"
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
        "justification": "The conditions record the assumption and failure-boundary framing.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires explaining the mechanism, assumptions, and boundary, with a full theorem not mandatory.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the intuition-under-assumption chain and the three-part analytic supplement.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-mechanism-and-theory-response",
    "knowledge_ids": [
      "decide-mechanism-explanation-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "Experimental performance cannot substitute for a mechanism explanation.",
      "This records the repository's own stated caveat, not an independent verification of tip quality.",
      "XXX and M1/M2 are placeholder labels, not measurements or named components."
    ],
    "scope": "Applies when a reviewer asks for theory or mechanism justification. The intuition-under-assumption chain and the analytic statement covering the core assumptions, the relation between key steps and the objective/representation space, and the failure boundary are filled from the user's own method; M1/M2 and XXX are placeholders. Experimental performance cannot substitute for the mechanism explanation.",
    "task": "Draft a rebuttal response to a reviewer who asks for theoretical justification, by explaining the mechanism, its assumptions, and the boundary where the method may fail, with a complete theorem explicitly not mandatory, rather than claiming validity merely from experimental performance.",
    "title": "Draft a rebuttal for missing-theory critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer asks for theoretical justification, the documented rule (Tip 6) is not to claim validity merely from good experimental performance. A complete theorem is not mandatory, but the mechanism, assumptions, and boundaries must be explained. The example answer states the core intuition (XXX): under the XXX assumption, M1 causes XXX, which enables M2 to XXX; and the revision will add an analytic statement covering the core assumptions, the relation between the key steps and the objective function/representation space, and the boundary where the method may fail.",
    "evidence": [
      {
        "justification": "The conditions record the assumption and failure-boundary framing.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires explaining the mechanism, assumptions, and boundary, with a full theorem not mandatory.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the intuition-under-assumption chain and the three-part analytic supplement.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-mechanism-explanation-response",
    "limitations": [
      "Experimental performance cannot substitute for a mechanism explanation.",
      "XXX and M1/M2 are placeholder labels, not measurements or named components."
    ],
    "title": "For missing-theory critiques, explain the mechanism, assumptions, and failure boundary",
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

