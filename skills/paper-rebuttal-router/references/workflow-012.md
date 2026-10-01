# Workflow 12: Draft a rebuttal for data-leakage concerns

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-leakage-check-response"
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
      "justification": "The conditions record the example-status of the no-leakage finding and the absence of a concrete deduplication algorithm.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_22.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires describing the check-and-exclude process instead of a bare denial.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_22.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the prior-settings adoption and the train/validation/test overlap check.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_22.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that describes the user's actual overlap check and exclusion procedure instead of a bare no-leakage denial.",
  "id": "wf-draft-leakage-check-response",
  "limitations": [
    "No concrete deduplication algorithm or check-procedure detail is supplied.",
    "The no-leakage finding is the example answer's claim and cannot establish that any user's data is leakage-free.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when data leakage is the reviewer's concern. The card gives no concrete deduplication algorithm, so the check description must come from the user's actual procedure, and the no-leakage finding in the example cannot establish that any user's data is leakage-free. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-leakage-check-response-step1",
      "instruction": "Confirm the reviewer point concerns data leakage (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual overlap check and exclusion procedure and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-leakage-check-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the data leakage point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-leakage-check-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-leakage-check-response-step1"
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
          "justification": "The conditions record the example-status of the no-leakage finding and the absence of a concrete deduplication algorithm.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_22.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires describing the check-and-exclude process instead of a bare denial.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_22.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the prior-settings adoption and the train/validation/test overlap check.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_22.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-leakage-check-response-step2",
      "instruction": "Apply draft-leakage-check-response using the user's real facts: describe how overlap was checked and excluded (such as following prior experimental settings and checking train/validation/test overlap) so the reviewer can be convinced, rather than answering merely that no leakage exists.",
      "limitations": [
        "No concrete deduplication algorithm or check-procedure detail is supplied.",
        "The no-leakage finding is the example answer's claim and cannot establish that any user's data is leakage-free.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the data leakage reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-leakage-check-response-step2"
      ],
      "id": "wf-draft-leakage-check-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-leakage-check-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for data-leakage concerns"
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
        "justification": "The conditions record the example-status of the no-leakage finding and the absence of a concrete deduplication algorithm.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires describing the check-and-exclude process instead of a bare denial.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the prior-settings adoption and the train/validation/test overlap check.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-leakage-check-response",
    "knowledge_ids": [
      "decide-leakage-check-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "No concrete deduplication algorithm or check-procedure detail is supplied.",
      "The no-leakage finding is the example answer's claim and cannot establish that any user's data is leakage-free.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when data leakage is the reviewer's concern. The card gives no concrete deduplication algorithm, so the check description must come from the user's actual procedure, and the no-leakage finding in the example cannot establish that any user's data is leakage-free.",
    "task": "Draft a rebuttal response to a reviewer who suspects data leakage, by describing how overlap was checked and excluded (such as following prior experimental settings and checking train/validation/test overlap) so the reviewer can be convinced, rather than answering merely that no leakage exists.",
    "title": "Draft a rebuttal for data-leakage concerns"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer suspects data leakage, the documented rule (Tip 22) is not to answer merely that no leakage exists. Take the concern seriously and describe how it was checked and excluded so the reviewer can be convinced. The example adopted the dataset following prior experimental settings, further checked the overlap between training, validation, and test sets and found no leakage, and will add the discussion to the next version. The card does not give a concrete deduplication algorithm.",
    "evidence": [
      {
        "justification": "The conditions record the example-status of the no-leakage finding and the absence of a concrete deduplication algorithm.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires describing the check-and-exclude process instead of a bare denial.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the prior-settings adoption and the train/validation/test overlap check.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_22.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-leakage-check-response",
    "limitations": [
      "No concrete deduplication algorithm or check-procedure detail is supplied.",
      "The no-leakage finding is the example answer's claim and cannot establish that any user's data is leakage-free."
    ],
    "title": "For data-leakage concerns, describe how overlap was checked and excluded",
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

