# Workflow 17: Draft a rebuttal for missing-experiment critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-missing-experiment-response"
  ],
  "confidence": "medium",
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
      "justification": "The core point states not to just say 我们会补充 and, when time allows, to give key results with setup, numbers and conclusions.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_12.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 12 demonstrates acknowledgement, a difficulty-stratified supplement, a trend claim, and deferral to the revision.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_12.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 21's core point lists multiple random seeds, standard deviation, and, optionally, confidence intervals or significance tests as stability evidence.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_21.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 21 demonstrates acknowledgement, a multi-seed mean/std supplement, a stability-trend claim, and deferral of annotations.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_21.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 25 demonstrates acknowledgement, a human-evaluation supplement with protocol/agreement placeholders, a trend claim, and deferral.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_25.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that gives the added experiment's key results when time allows, or the documented supplement-and-defer shape, instead of a bare promise.",
  "id": "wf-draft-missing-experiment-response",
  "limitations": [
    "All numeric fields in the three cited examples are placeholders and do not establish any executed experiment; the shape is scoped to these three examples.",
    "The applicability is conditioned on 如果时间允许; the sample recommended answer itself still contains an ellipsis (结果显示……) rather than concrete figures.",
    "The optional statistical evidence (confidence intervals or significance tests) is listed without prescribing any specific unnamed test or fabricated values.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when a reviewer asks for an experiment or analysis not yet present. Giving new results is conditioned on time allowing; the sample answer's ellipsis is example status, and a promise or plan must not be reported as a completed experiment. The reusable shape covers the three cited supplementary-experiment cards (difficulty-stratified analysis, at-least-XXX-random-seeds mean/standard-deviation reporting, small-scale human evaluation); confidence intervals or significance tests are optional stability evidence, listed without prescribing any specific unnamed test, and all numeric fields are placeholders. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "medium",
      "depends_on": [],
      "id": "wf-draft-missing-experiment-response-step1",
      "instruction": "Confirm the reviewer point concerns a missing key experiment or analysis (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect which experiment or analysis the point names, the user's actual results if they exist, and the current status and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-missing-experiment-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the a missing key experiment or analysis point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-missing-experiment-response",
      "confidence": "medium",
      "depends_on": [
        "wf-draft-missing-experiment-response-step1"
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
          "justification": "The core point states not to just say 我们会补充 and, when time allows, to give key results with setup, numbers and conclusions.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_12.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 12 demonstrates acknowledgement, a difficulty-stratified supplement, a trend claim, and deferral to the revision.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_12.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 21's core point lists multiple random seeds, standard deviation, and, optionally, confidence intervals or significance tests as stability evidence.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_21.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 21 demonstrates acknowledgement, a multi-seed mean/std supplement, a stability-trend claim, and deferral of annotations.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_21.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 25 demonstrates acknowledgement, a human-evaluation supplement with protocol/agreement placeholders, a trend claim, and deferral.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_25.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-missing-experiment-response-step2",
      "instruction": "Apply draft-missing-experiment-response using the user's real facts: give the added experiment or analysis's key results (setup, core numbers, conclusions) when time allows; otherwise use the documented supplementary-experiment shape of acknowledging the concern, describing the supplementary analysis, stating the supporting trend, and deferring full details to the revision, rather than replying with a bare promise to add it later.",
      "limitations": [
        "All numeric fields in the three cited examples are placeholders and do not establish any executed experiment; the shape is scoped to these three examples.",
        "The applicability is conditioned on 如果时间允许; the sample recommended answer itself still contains an ellipsis (结果显示……) rather than concrete figures.",
        "The optional statistical evidence (confidence intervals or significance tests) is listed without prescribing any specific unnamed test or fabricated values.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the a missing key experiment or analysis reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "medium",
      "depends_on": [
        "wf-draft-missing-experiment-response-step2"
      ],
      "id": "wf-draft-missing-experiment-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-missing-experiment-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for missing-experiment critiques"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "medium",
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
        "justification": "The core point states not to just say 我们会补充 and, when time allows, to give key results with setup, numbers and conclusions.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_12.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 12 demonstrates acknowledgement, a difficulty-stratified supplement, a trend claim, and deferral to the revision.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_12.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 21's core point lists multiple random seeds, standard deviation, and, optionally, confidence intervals or significance tests as stability evidence.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_21.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 21 demonstrates acknowledgement, a multi-seed mean/std supplement, a stability-trend claim, and deferral of annotations.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_21.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25 demonstrates acknowledgement, a human-evaluation supplement with protocol/agreement placeholders, a trend claim, and deferral.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-missing-experiment-response",
    "knowledge_ids": [
      "decide-act-over-promise",
      "example-supplementary-experiment-shape",
      "readme-disclaimer"
    ],
    "limitations": [
      "All numeric fields in the three cited examples are placeholders and do not establish any executed experiment; the shape is scoped to these three examples.",
      "The applicability is conditioned on 如果时间允许; the sample recommended answer itself still contains an ellipsis (结果显示……) rather than concrete figures.",
      "The optional statistical evidence (confidence intervals or significance tests) is listed without prescribing any specific unnamed test or fabricated values.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer asks for an experiment or analysis not yet present. Giving new results is conditioned on time allowing; the sample answer's ellipsis is example status, and a promise or plan must not be reported as a completed experiment. The reusable shape covers the three cited supplementary-experiment cards (difficulty-stratified analysis, at-least-XXX-random-seeds mean/standard-deviation reporting, small-scale human evaluation); confidence intervals or significance tests are optional stability evidence, listed without prescribing any specific unnamed test, and all numeric fields are placeholders.",
    "task": "Draft a rebuttal response to a reviewer who points out that a key experiment or analysis is missing, by giving the added experiment or analysis's key results (setup, core numbers, conclusions) when time allows, using the documented supplementary-experiment shape of acknowledging the concern, describing the supplementary analysis, stating the supporting trend, and deferring full details to the revision, rather than replying with a bare promise to add it later.",
    "title": "Draft a rebuttal for missing-experiment critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When a reviewer points out that a key experiment or analysis is missing, the documented general strategy (Tip 12) is not to reply with a bare promise to add it in the revision. If time allows, the rebuttal should directly give the added experiment or analysis's key results, including experimental setup, core numbers, and conclusions.",
    "evidence": [
      {
        "justification": "The core point states not to just say 我们会补充 and, when time allows, to give key results with setup, numbers and conclusions.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_12.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-act-over-promise",
    "limitations": [
      "The applicability is conditioned on 如果时间允许; the sample recommended answer itself still contains an ellipsis (结果显示……) rather than concrete figures."
    ],
    "title": "If time allows, provide new experimental results rather than only promising them",
    "type": "DECISION_RULE"
  },
  {
    "confidence": "medium",
    "content": "Three recommended answers that involve supplementary experiments share a reusable shape: acknowledge the concern's importance, describe a supplementary analysis with placeholders for setup and result, state the supporting trend, and defer full details to the revision. Tip 12 adds a sample-difficulty-stratified analysis and claims greater gains on harder samples, deferring the full result to the revision. Tip 21 adds at least XXX random seeds with mean and standard deviation, claims a stable advantage over baseline, and defers standard-deviation annotation and discussion to the tables/text; its core point additionally lists confidence intervals or significance tests as optional stability evidence. Tip 25 adds a small-scale human evaluation with N annotators, XXX samples, dimensions, and κ/Krippendorff's α placeholders, claims agreement with automatic metrics, and defers setup, protocol, and analysis to the final version. Tip 12 is grouped in the README's communication category (写作澄清、相关工作与沟通策略类) rather than the experiment category, and this synthesis does not change the README's category grouping.",
    "evidence": [
      {
        "justification": "Tip 12 demonstrates acknowledgement, a difficulty-stratified supplement, a trend claim, and deferral to the revision.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_12.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 21's core point lists multiple random seeds, standard deviation, and, optionally, confidence intervals or significance tests as stability evidence.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_21.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 21 demonstrates acknowledgement, a multi-seed mean/std supplement, a stability-trend claim, and deferral of annotations.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_21.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25 demonstrates acknowledgement, a human-evaluation supplement with protocol/agreement placeholders, a trend claim, and deferral.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      }
    ],
    "id": "example-supplementary-experiment-shape",
    "limitations": [
      "All numeric fields in the three cited examples are placeholders and do not establish any executed experiment; the shape is scoped to these three examples.",
      "The optional statistical evidence (confidence intervals or significance tests) is listed without prescribing any specific unnamed test or fabricated values."
    ],
    "title": "涉及补充实验的三个推荐回答",
    "type": "EXAMPLE_PATTERN"
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

