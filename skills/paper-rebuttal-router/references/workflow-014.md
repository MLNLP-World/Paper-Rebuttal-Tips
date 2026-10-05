# Workflow 14: Draft a rebuttal for dynamic-capability doubts

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-longitudinal-evidence-response"
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
      "justification": "The conditions record an absent status for the 下表 referenced by the recommended answer.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_26.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The conditions record an absent status for the referenced 新增表格 and learning curve.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_27.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The conditions record the example settings and that the referenced new table and learning curve are absent.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_27.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point prescribes a longitudinal time-series experiment with real trend data as the strongest response.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_27.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the 100-task, every-20-task longitudinal experiment and the XX%-to-XX% trend.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_27.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that proposes a longitudinal time-series experiment with real trend data, keeping the main experiment offline for a fair zero-shot comparison when the user's setup matches.",
  "id": "wf-draft-longitudinal-evidence-response",
  "limitations": [
    "100 tasks and the every-20-task evaluation are example settings; XX% start and end rates are placeholders, not executed results.",
    "Absence is recorded against the supplied Builder visual readings; the referenced objects were not independently checked outside this bundle.",
    "The recommended answers in Tip 26 and Tip 27 reference supporting tables or curves that are not present in the supplied materials. Tip 26 says 具体数据见下表 (with the visual reading recording that the referenced table is not actually present), and Tip 27 references an 新增表格 and a learning curve (with the visual reading recording that both are absent).",
    "The referenced new table and learning curve are absent from the supplied material (see limitation-missing-tables-curves).",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when dynamic capability is the reviewer's concern. The 100-task stream and every-20-task evaluation are example settings, not recommended values, and the start/end percentages are placeholders, not executed results. The referenced table and learning curve are absent from the supplied materials. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-longitudinal-evidence-response-step1",
      "instruction": "Confirm the reviewer point concerns dynamic or continuous capability (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual evaluation setup, whether it matches the offline main experiment with a zero-shot fair comparison, and any real trend data and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-longitudinal-evidence-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the dynamic or continuous capability point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-longitudinal-evidence-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-longitudinal-evidence-response-step1"
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
          "justification": "The conditions record an absent status for the 下表 referenced by the recommended answer.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_26.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The conditions record an absent status for the referenced 新增表格 and learning curve.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_27.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The conditions record the example settings and that the referenced new table and learning curve are absent.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_27.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point prescribes a longitudinal time-series experiment with real trend data as the strongest response.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_27.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the 100-task, every-20-task longitudinal experiment and the XX%-to-XX% trend.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_27.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-longitudinal-evidence-response-step2",
      "instruction": "Apply draft-longitudinal-evidence-response using the user's real facts: propose a longitudinal time-series experiment with real trend data while keeping the main experiment offline for a fair zero-shot comparison when the user's setup matches, rather than answering that the system is theoretically dynamic.",
      "limitations": [
        "100 tasks and the every-20-task evaluation are example settings; XX% start and end rates are placeholders, not executed results.",
        "Absence is recorded against the supplied Builder visual readings; the referenced objects were not independently checked outside this bundle.",
        "The recommended answers in Tip 26 and Tip 27 reference supporting tables or curves that are not present in the supplied materials. Tip 26 says 具体数据见下表 (with the visual reading recording that the referenced table is not actually present), and Tip 27 references an 新增表格 and a learning curve (with the visual reading recording that both are absent).",
        "The referenced new table and learning curve are absent from the supplied material (see limitation-missing-tables-curves).",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the dynamic or continuous capability reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-longitudinal-evidence-response-step2"
      ],
      "id": "wf-draft-longitudinal-evidence-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-longitudinal-evidence-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for dynamic-capability doubts"
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
        "justification": "The conditions record an absent status for the 下表 referenced by the recommended answer.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The conditions record an absent status for the referenced 新增表格 and learning curve.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The conditions record the example settings and that the referenced new table and learning curve are absent.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes a longitudinal time-series experiment with real trend data as the strongest response.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the 100-task, every-20-task longitudinal experiment and the XX%-to-XX% trend.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-longitudinal-evidence-response",
    "knowledge_ids": [
      "decide-longitudinal-evidence-response",
      "limitation-missing-tables-curves",
      "readme-disclaimer"
    ],
    "limitations": [
      "100 tasks and the every-20-task evaluation are example settings; XX% start and end rates are placeholders, not executed results.",
      "Absence is recorded against the supplied Builder visual readings; the referenced objects were not independently checked outside this bundle.",
      "The recommended answers in Tip 26 and Tip 27 reference supporting tables or curves that are not present in the supplied materials. Tip 26 says 具体数据见下表 (with the visual reading recording that the referenced table is not actually present), and Tip 27 references an 新增表格 and a learning curve (with the visual reading recording that both are absent).",
      "The referenced new table and learning curve are absent from the supplied material (see limitation-missing-tables-curves).",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when dynamic capability is the reviewer's concern. The 100-task stream and every-20-task evaluation are example settings, not recommended values, and the start/end percentages are placeholders, not executed results. The referenced table and learning curve are absent from the supplied materials.",
    "task": "Draft a rebuttal response to a reviewer who doubts the system's dynamic or continuous capability, by proposing a longitudinal time-series experiment with real trend data while keeping the main experiment offline for a fair zero-shot comparison, rather than answering that the system is theoretically dynamic.",
    "title": "Draft a rebuttal for dynamic-capability doubts"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When reviewers doubt the system's dynamic/continuous capability, the documented rule (Tip 27) is not to answer that the system is theoretically dynamic while the evaluation fixed parameters for fairness. The strongest response is a longitudinal time-series experiment with real trend data. The example keeps the main experiment offline for a fair zero-shot comparison, then adds a longitudinal experiment: the system processes 100 tasks continuously and is evaluated every 20 tasks, and the average success rate rises steadily from XX% to XX%, with the learning curve added to the appendix. The referenced new table and learning curve are not actually present in the image.",
    "evidence": [
      {
        "justification": "The conditions record the example settings and that the referenced new table and learning curve are absent.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes a longitudinal time-series experiment with real trend data as the strongest response.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the 100-task, every-20-task longitudinal experiment and the XX%-to-XX% trend.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-longitudinal-evidence-response",
    "limitations": [
      "100 tasks and the every-20-task evaluation are example settings; XX% start and end rates are placeholders, not executed results.",
      "The referenced new table and learning curve are absent from the supplied material (see limitation-missing-tables-curves)."
    ],
    "title": "For dynamic-capability doubts, add a longitudinal time-series experiment with real trends",
    "type": "DECISION_RULE"
  },
  {
    "confidence": "high",
    "content": "The recommended answers in Tip 26 and Tip 27 reference supporting tables or curves that are not present in the supplied materials. Tip 26 says 具体数据见下表 (with the visual reading recording that the referenced table is not actually present), and Tip 27 references an 新增表格 and a learning curve (with the visual reading recording that both are absent).",
    "evidence": [
      {
        "justification": "The conditions record an absent status for the 下表 referenced by the recommended answer.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The conditions record an absent status for the referenced 新增表格 and learning curve.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_27.svg",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-missing-tables-curves",
    "limitations": [
      "Absence is recorded against the supplied Builder visual readings; the referenced objects were not independently checked outside this bundle."
    ],
    "title": "Referenced tables and curves in Tips 26 and 27 are absent from the supplied material",
    "type": "LIMITATION"
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

