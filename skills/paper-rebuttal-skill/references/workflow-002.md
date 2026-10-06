# Workflow 2: Draft a rebuttal reply for a missing-ablation critique

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-ablation-evidence-response"
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
      "justification": "The conditions record the example-status of the 补充了 and 初步结果显示 phrasing.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_16.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires naming what is removed or replaced, the affected metric, and real results or a concrete supplement plan.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_16.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the M1/M2/M3 removal/replacement plan with metric placeholders.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_16.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply to a reviewer who asks for ablation evidence by naming what is removed or replaced and the metric each change affects, and by giving real results or a concrete supplement plan, rather than answering that every module is necessary without showing it.",
  "id": "wf-draft-ablation-evidence-reply",
  "limitations": [
    "M1/M2/M3 and XXX are example component and metric placeholders, not the user's modules or measured values.",
    "The preliminary-results phrasing is example status; a plan must not be reported as a completed experiment.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the comment type and input completeness; it does not draft the reply and must not substitute example placeholders for the user's facts."
  ],
  "scope": "Applies when a reviewer requests ablation evidence. Requires the user to supply their actual modules and measured values; M1/M2/M3 and XXX are example placeholders, and the example's 补充了/初步结果显示 phrasing is example status, so a plan must not be reported as a completed experiment.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-ablation-evidence-reply-step1",
      "instruction": "Confirm the reviewer comment requests ablation evidence and check whether the user has supplied their actual module names, metric values, and any completed results; record missing facts rather than substituting the card's M1/M2/M3 and XXX placeholders.",
      "limitations": [
        "This step only checks the comment type and input completeness; it does not draft the reply and must not substitute example placeholders for the user's facts."
      ],
      "rationale": "The ablation drafting capability requires the user's real modules and metrics, and its scope restricts it to ablation-evidence critiques, so these must be verified first.",
      "title": "Confirm the critique requests ablation evidence and record the user's module and metric facts",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-ablation-evidence-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-ablation-evidence-reply-step1"
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
          "justification": "The conditions record the example-status of the 补充了 and 初步结果显示 phrasing.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_16.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires naming what is removed or replaced, the affected metric, and real results or a concrete supplement plan.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_16.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the M1/M2/M3 removal/replacement plan with metric placeholders.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_16.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-ablation-evidence-reply-step2",
      "instruction": "Apply draft-ablation-evidence-response using the user's real modules and metrics: name what is removed or replaced and the metric each change affects, and give real results or a concrete supplement plan. Keep any supplement as a plan, not a completed experiment.",
      "limitations": [
        "M1/M2/M3 and XXX are example component and metric placeholders, not the user's modules or measured values.",
        "The preliminary-results phrasing is example status; a plan must not be reported as a completed experiment.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the ablation-evidence reply",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Draft a rebuttal reply for a missing-ablation critique"
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
        "justification": "The conditions record the example-status of the 补充了 and 初步结果显示 phrasing.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires naming what is removed or replaced, the affected metric, and real results or a concrete supplement plan.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the M1/M2/M3 removal/replacement plan with metric placeholders.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-ablation-evidence-response",
    "knowledge_ids": [
      "decide-ablation-evidence-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "M1/M2/M3 and XXX are example component and metric placeholders, not the user's modules or measured values.",
      "The preliminary-results phrasing is example status; a plan must not be reported as a completed experiment.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer requests ablation evidence. The M1/M2/M3 removal/replacement plan and the XXX metric are example placeholders, not the user's modules or measured values, and the example's '补充了'/'初步结果显示' phrasing is example experiment status, so a plan must not be reported as a completed experiment.",
    "task": "Draft a rebuttal response to a reviewer who asks for ablation evidence by naming what is removed or replaced and the metric each change affects, and by giving real results or a concrete supplement plan, rather than answering that every module is necessary without showing it.",
    "title": "Draft a rebuttal for missing-ablation critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer asks for ablation evidence, the documented rule (Tip 16) is not to answer that every module is necessary without showing it. State what is removed, what is replaced, and which metric is affected, and give real results or a concrete supplement plan. The example ablates three components: remove M1 to verify its effect on XXX; replace M2 with a simple strategy to verify the necessity of the design choice; remove M3 to analyze its contribution to stability/efficiency/generalization. The reading records the example's 补充了 and 初步结果显示 phrasing as example experiment status, so a plan must not be reported as a completed experiment.",
    "evidence": [
      {
        "justification": "The conditions record the example-status of the 补充了 and 初步结果显示 phrasing.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires naming what is removed or replaced, the affected metric, and real results or a concrete supplement plan.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the M1/M2/M3 removal/replacement plan with metric placeholders.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_16.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-ablation-evidence-response",
    "limitations": [
      "M1/M2/M3 and XXX are example component and metric placeholders, not the user's modules or measured values.",
      "The preliminary-results phrasing is example status; a plan must not be reported as a completed experiment."
    ],
    "title": "For missing-ablation critiques, name what is removed or replaced and the metric it affects",
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

