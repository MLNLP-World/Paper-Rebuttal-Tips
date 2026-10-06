# Workflow 18: Draft a reply for a criticism that appears to rest on a misunderstanding

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-misunderstanding-correction"
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
      "justification": "The core point says not to directly tell the reviewer they are wrong and to focus on neutrally clarifying the real method.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_10.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer opens by attributing the problem to unclear expression before clarifying the method.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_10.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply to a criticism the user judges to rest on a misunderstanding of the method, by acknowledging that the writing may have been unclear and neutrally clarifying the actual method flow and what it does not depend on, without telling the reviewer they are wrong.",
  "id": "wf-draft-misunderstanding-correction",
  "limitations": [
    "The recommended answer's no-risk conclusion is restricted to 当前设置 (the current setup), not a general guarantee.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the misunderstanding condition and input completeness; it does not draft the reply or decide the method's correctness."
  ],
  "scope": "Applies only when the user judges that the criticism rests on a misunderstanding of the method; requires the user to supply the actual method flow and its dependencies. Any no-risk conclusion is restricted to the current setup, not a general guarantee.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-misunderstanding-correction-step1",
      "instruction": "Confirm that the user judges the criticism to rest on a misunderstanding of the method, and check that the user has supplied the actual method flow and its dependencies; record missing method facts rather than assuming them.",
      "limitations": [
        "This step only checks the misunderstanding condition and input completeness; it does not draft the reply or decide the method's correctness."
      ],
      "rationale": "The capability applies only when the user judges the criticism rests on a misunderstanding, so the workflow must confirm this condition and the required method facts before drafting.",
      "title": "Confirm the misunderstanding condition and the method facts",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-misunderstanding-correction",
      "confidence": "high",
      "depends_on": [
        "wf-draft-misunderstanding-correction-step1"
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
          "justification": "The core point says not to directly tell the reviewer they are wrong and to focus on neutrally clarifying the real method.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_10.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer opens by attributing the problem to unclear expression before clarifying the method.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_10.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-misunderstanding-correction-step2",
      "instruction": "Apply draft-misunderstanding-correction using the user's method facts: acknowledge the writing may have been unclear and neutrally clarify the actual method flow and what it does not depend on, without telling the reviewer they are wrong, and restrict any no-risk conclusion to the current setup.",
      "limitations": [
        "The recommended answer's no-risk conclusion is restricted to 当前设置 (the current setup), not a general guarantee.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the neutral clarification reply",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Draft a reply for a criticism that appears to rest on a misunderstanding"
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
        "justification": "The core point says not to directly tell the reviewer they are wrong and to focus on neutrally clarifying the real method.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer opens by attributing the problem to unclear expression before clarifying the method.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-misunderstanding-correction",
    "knowledge_ids": [
      "decide-misunderstanding-correction",
      "readme-disclaimer"
    ],
    "limitations": [
      "The recommended answer's no-risk conclusion is restricted to 当前设置 (the current setup), not a general guarantee.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when the user judges that the criticism rests on a misunderstanding of the method. Any no-risk conclusion is restricted to the current setup, not a general guarantee.",
    "task": "Draft a rebuttal response to a criticism that appears based on a misunderstanding of the method, by acknowledging that the writing may have been unclear and neutrally clarifying the actual method flow and what it does not depend on, without telling the reviewer they are wrong.",
    "title": "Draft a rebuttal for reviewer-misunderstanding critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer's criticism appears based on a misunderstanding of the method, the documented rule (Tip 10) is not to say the reviewer is wrong. Instead, acknowledge that the writing may have been unclear and neutrally clarify the actual method flow and what it does not depend on.",
    "evidence": [
      {
        "justification": "The core point says not to directly tell the reviewer they are wrong and to focus on neutrally clarifying the real method.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer opens by attributing the problem to unclear expression before clarifying the method.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-misunderstanding-correction",
    "limitations": [
      "The recommended answer's no-risk conclusion is restricted to 当前设置 (the current setup), not a general guarantee."
    ],
    "title": "Correct reviewer misunderstandings by acknowledging unclear writing first",
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

