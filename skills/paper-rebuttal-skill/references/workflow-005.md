# Workflow 5: Draft a rebuttal for unclear-contribution critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-contribution-focus-response"
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
      "justification": "The conditions record the revision commitment and the background-as-contribution prohibition.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_04.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point prescribes concrete, verifiable contributions tied to method and experiments instead of blaming the reviewer.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_04.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the three-point rewrite and the no-background-as-contribution rule.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_04.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that acknowledges the focus problem and rewrites the contribution points to be concrete, verifiable, and tied to the method and experiments.",
  "id": "wf-draft-contribution-focus-response",
  "limitations": [
    "The three-point enumeration is an example outline; the actual contribution points come from the user's paper.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied.",
    "XXX is a placeholder; the card supplies no concrete contribution content."
  ],
  "scope": "Applies when the reviewer's critique is that the contribution statement is unclear or that concrete contributions are hard to identify, not when the author merely claims the contributions were already listed. The three-point problem/method/experiment enumeration is an example outline; the actual contribution points come from the user's paper, and background statements must not be written up as contributions. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-contribution-focus-response-step1",
      "instruction": "Confirm the reviewer point concerns the contribution statement (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual contribution points and how each ties to the method and the experiments and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-contribution-focus-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the the contribution statement point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-contribution-focus-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-contribution-focus-response-step1"
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
          "justification": "The conditions record the revision commitment and the background-as-contribution prohibition.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_04.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point prescribes concrete, verifiable contributions tied to method and experiments instead of blaming the reviewer.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_04.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the three-point rewrite and the no-background-as-contribution rule.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_04.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-contribution-focus-response-step2",
      "instruction": "Apply draft-contribution-focus-response using the user's real facts: acknowledge the focus problem and rewrite the contribution points so each is concrete, verifiable, and directly tied to the method and experiments, without blaming the reviewer for not noticing them.",
      "limitations": [
        "The three-point enumeration is an example outline; the actual contribution points come from the user's paper.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "XXX is a placeholder; the card supplies no concrete contribution content."
      ],
      "title": "Draft the the contribution statement reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-contribution-focus-response-step2"
      ],
      "id": "wf-draft-contribution-focus-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-contribution-focus-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for unclear-contribution critiques"
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
        "justification": "The conditions record the revision commitment and the background-as-contribution prohibition.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes concrete, verifiable contributions tied to method and experiments instead of blaming the reviewer.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the three-point rewrite and the no-background-as-contribution rule.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-contribution-focus-response",
    "knowledge_ids": [
      "decide-contribution-focus-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "The three-point enumeration is an example outline; the actual contribution points come from the user's paper.",
      "This records the repository's own stated caveat, not an independent verification of tip quality.",
      "XXX is a placeholder; the card supplies no concrete contribution content."
    ],
    "scope": "Applies when the reviewer's critique is that the contribution statement is unclear or that concrete contributions are hard to identify, not when the author merely claims the contributions were already listed. The three-point problem/method/experiment enumeration is an example outline; the actual contribution points come from the user's paper, and background statements must not be written up as contributions.",
    "task": "Draft a rebuttal response to a reviewer who finds the contribution statement unclear or cannot identify concrete contributions, by acknowledging the focus problem and rewriting the contribution points so each is concrete, verifiable, and directly tied to the method and experiments, without blaming the reviewer for not noticing them.",
    "title": "Draft a rebuttal for unclear-contribution critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer finds the listed contributions unconvincing, the documented rule (Tip 4) is not to blame the reviewer for not noticing them. Instead, acknowledge the focus problem and rewrite the contribution points so each corresponds to the core innovation and is concrete, verifiable, and directly tied to the method and experiments. The example revision enumerates: 一、提出 XXX 问题设定; 二、设计 XXX 方法; 三、构建 XXX 实验或分析, and explicitly avoids writing background statements up as contributions.",
    "evidence": [
      {
        "justification": "The conditions record the revision commitment and the background-as-contribution prohibition.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes concrete, verifiable contributions tied to method and experiments instead of blaming the reviewer.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the three-point rewrite and the no-background-as-contribution rule.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-contribution-focus-response",
    "limitations": [
      "The three-point enumeration is an example outline; the actual contribution points come from the user's paper.",
      "XXX is a placeholder; the card supplies no concrete contribution content."
    ],
    "title": "For 'contributions already listed' critiques, rewrite contributions as specific verifiable claims",
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

