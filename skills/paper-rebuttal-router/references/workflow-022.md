# Workflow 22: Analyze a vague or generic negative review and draft a reply

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-vague-review-response"
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
      "justification": "The core point prescribes item-by-item response, polite clarification requests, and fact-only AC communication.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_11.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the polite clarification request and conditional AC explanation.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_11.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "For a review whose concerns are partly or wholly too general to locate, extract and respond item-by-item to every identifiable concern, politely request more specific feedback for concerns that cannot be located, and, when explaining to the AC, state only facts and evidence without evaluating the reviewer personally.",
  "id": "wf-draft-reply-for-vague-review",
  "limitations": [
    "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only organizes the review text and records material presence; it does not draft the reply or analyze review content."
  ],
  "scope": "Applies to reviews whose concerns are partly or wholly too general to locate; the AC escalation is conditional, not required in every case. Requires the user to supply the review text and the paper facts referenced in the reply; the workflow does not evaluate the reviewer personally and does not fabricate numbers or completed statuses.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-reply-for-vague-review-step1",
      "instruction": "Split the supplied review into identifiable concerns, position each concern relative to the user's paper, and record which required material (review text, paper facts, existing draft) is present or missing; mark missing reply material as 未提供/未找到 rather than assuming it.",
      "limitations": [
        "This step only organizes the review text and records material presence; it does not draft the reply or analyze review content."
      ],
      "rationale": "The drafting capability needs the review's individual concerns located and its required inputs checked before it can produce an item-by-item reply.",
      "title": "Split the review into identifiable concerns and record missing material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-vague-review-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-reply-for-vague-review-step1"
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
          "justification": "The core point prescribes item-by-item response, polite clarification requests, and fact-only AC communication.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_11.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the polite clarification request and conditional AC explanation.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_11.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-reply-for-vague-review-step2",
      "instruction": "Apply draft-vague-review-response to the located concerns: respond item-by-item to each identifiable concern, politely request more specific feedback for concerns that cannot be located, and, only if explaining to the AC, state only facts and evidence without evaluating the reviewer personally. Do not fabricate numbers or completed statuses.",
      "limitations": [
        "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the item-by-item reply for the vague review",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Analyze a vague or generic negative review and draft a reply"
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
        "justification": "The core point prescribes item-by-item response, polite clarification requests, and fact-only AC communication.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the polite clarification request and conditional AC explanation.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-vague-review-response",
    "knowledge_ids": [
      "decide-vague-review-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies to reviews whose concerns are partly or wholly too general to locate. The AC escalation is conditional, not required in every case.",
    "task": "Draft a rebuttal response to a generic, low-quality negative review by extracting and responding item-by-item to every identifiable concern, politely requesting more specific feedback for concerns that cannot be located, and, when explaining to the AC, stating only facts and evidence without evaluating the reviewer personally.",
    "title": "Draft a rebuttal for vague negative reviews"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "For generic, low-quality negative reviews, the documented rule (Tip 11) is: extract and respond item-by-item to every identifiable concern; for overly general concerns that cannot be located, politely request more specific feedback; and when explaining to the AC, state only facts and evidence without evaluating the reviewer personally.",
    "evidence": [
      {
        "justification": "The core point prescribes item-by-item response, polite clarification requests, and fact-only AC communication.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the polite clarification request and conditional AC explanation.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-vague-review-response",
    "limitations": [
      "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case."
    ],
    "title": "For vague negative reviews respond to identifiable issues and request specifics politely",
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

