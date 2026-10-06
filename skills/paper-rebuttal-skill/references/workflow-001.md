# Workflow 1: Respond to vague or unlocatable reviewer points

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
  "goal": "Split out the reviewer points that are themselves vague, low-quality, or whose concrete concern cannot be located, and produce for exactly those points the extracted concerns, clarification requests, and per-point results — reviewer point, existing response or missing, selected strategy (draft-vague-review-response), applicability reason, feedback or requested draft, missing evidence, unresolved items — without processing any clearly locatable point and without claiming to cover them.",
  "id": "wf-analyze-reviewer-comments",
  "limitations": [
    "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step applies the capability only to the points identified as vague, low-quality, or unlocatable; clearly locatable points are processed by their own domain workflows, not here.",
    "This step only identifies and records which points are vague or unlocatable; it does not process clearly locatable points, does not draft replies, does not review a draft that was not supplied, and does not substitute example placeholders for the user's facts.",
    "This step organizes only the vague or unlocatable points this workflow processed; it does not select workflows or strategies for clearly locatable points, does not claim a general all-comment analysis, and missing material limits only the point that needs it."
  ],
  "scope": "Applies only when reviewer comments contain points that are themselves vague, low-quality, or whose concrete concern cannot be located; when a group of comments mixes such points with clearly locatable points, this workflow processes only the vague or unlocatable ones. This workflow is not a general analysis entry for all reviewer comments: it responds only to the vague or unlocatable points through draft-vague-review-response, clearly locatable points are excluded from its processing scope and are left to the Skill Router for domain-workflow selection, and this workflow does not match or select domain workflows for any point. When the user supplies no reply draft, no draft review is performed or claimed.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-analyze-reviewer-comments-step1",
      "instruction": "Split the supplied reviewer comments into individual reviewer points and record which of them are themselves vague, low-quality, or whose concrete concern cannot be located; clearly locatable points are explicitly excluded from this workflow's processing scope and are left to the Skill Router for domain-workflow selection; for each vague or unlocatable point record the user's existing response if any (otherwise record it as missing) and which material is missing without assuming it; if no reply draft was supplied, record that no draft review is possible. This workflow does not claim to cover all reviewer points.",
      "limitations": [
        "This step only identifies and records which points are vague or unlocatable; it does not process clearly locatable points, does not draft replies, does not review a draft that was not supplied, and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The referenced capability applies only to vague, low-quality, or unlocatable points, so this step must delimit exactly those points and exclude the rest; clearly locatable points are handled by their domain workflows selected by the Skill Router, not here.",
      "title": "Identify the vague or unlocatable reviewer points and exclude the locatable ones",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-vague-review-response",
      "confidence": "high",
      "depends_on": [
        "wf-analyze-reviewer-comments-step1"
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
      "id": "wf-analyze-reviewer-comments-step2",
      "instruction": "Apply draft-vague-review-response only to the points identified as vague, low-quality, or unlocatable, within its documented scope: extract and respond item-by-item to every identifiable concern of those points, politely request more specific feedback for the concerns that cannot be located, and, when explaining to the AC, state only facts and evidence without evaluating the reviewer personally; clearly locatable points are not processed in this workflow — their domain workflows are selected by the Skill Router.",
      "limitations": [
        "The AC escalation is conditional (如需向 AC 说明), not presented as required in every case.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "This step applies the capability only to the points identified as vague, low-quality, or unlocatable; clearly locatable points are processed by their own domain workflows, not here."
      ],
      "title": "Respond to the vague or unlocatable points",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-analyze-reviewer-comments-step2"
      ],
      "id": "wf-analyze-reviewer-comments-step3",
      "instruction": "Organize only the points this workflow actually processed as: reviewer point; existing response or missing; selected strategy (draft-vague-review-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Do not match, select, or list strategies for clearly locatable points — general multi-point splitting, topic classification, applicability judgment, and workflow selection are the Skill Router's responsibility, not this workflow's. Missing material limits only the point that needs it. This workflow does not claim to have completed a general analysis of all reviewer comments.",
      "limitations": [
        "This step organizes only the vague or unlocatable points this workflow processed; it does not select workflows or strategies for clearly locatable points, does not claim a general all-comment analysis, and missing material limits only the point that needs it."
      ],
      "rationale": "Per-point organization for the processed points keeps the result traceable; the Router aggregates this workflow's per-point results with the domain workflows' per-point results, which this workflow does not claim to do.",
      "title": "Organize the vague or unlocatable points' results",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Respond to vague or unlocatable reviewer points"
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

