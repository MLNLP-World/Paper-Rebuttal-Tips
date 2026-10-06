# Workflow 21: Draft a rebuttal for computational-overhead critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-overhead-response"
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
      "justification": "The conditions note instructs preserving both wordings as scenario-dependent rather than a universal guarantee.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_17.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point requires concrete complexity, time, memory, and amortization analysis instead of a vague answer.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_17.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the cost source, complexity, stage controllability, parallelization, and amortization argument.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_17.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The unresolved note flags the noncritical source-meaning ambiguity between the two stage wordings.",
      "kind": "image",
      "locator": "visual_reading.unresolved",
      "path": "pics/tips/tip_17.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The unresolved note records the stage-wording ambiguity that must be preserved.",
      "kind": "image",
      "locator": "visual_reading.unresolved",
      "path": "pics/tips/tip_17.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that gives a concrete cost analysis from the user's own measurements instead of a vague gain-is-worth-it answer.",
  "id": "wf-draft-overhead-response",
  "limitations": [
    "All cost, complexity, and time tokens are placeholders; the card supplies no measured values.",
    "The stage wording has an unresolved source-meaning ambiguity (see limitation-tip17-stage-wording).",
    "The wordings themselves were read clearly by the Builder; only their applicable-scenario relationship is unresolved.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied.",
    "Tip 17's recommended answer first says the method adds about XXX% time at the training/inference stage, then says the overhead is introduced only at training/preprocessing/offline-construction and does not affect online inference. The Builder visual reading records this as an unresolved source-meaning ambiguity because the original card does not reconcile the two statements, so no universal stage guarantee should be read from the example."
  ],
  "scope": "Applies when overhead or cost is the reviewer's concern. The cost source, complexity, and percentages are filled from the user's own measurements (the card's tokens are placeholders). The source card's stage wording is ambiguous between training/inference overhead and offline-only construction that does not affect online inference; no universal stage guarantee should be read from the example, and the user's actual stage placement must come from their own method. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-overhead-response-step1",
      "instruction": "Confirm the reviewer point concerns computational overhead (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's own cost measurements (complexity, time, memory, amortization) and where the cost is introduced and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-overhead-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the computational overhead point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-overhead-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-overhead-response-step1"
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
          "justification": "The conditions note instructs preserving both wordings as scenario-dependent rather than a universal guarantee.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_17.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point requires concrete complexity, time, memory, and amortization analysis instead of a vague answer.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_17.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the cost source, complexity, stage controllability, parallelization, and amortization argument.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_17.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The unresolved note flags the noncritical source-meaning ambiguity between the two stage wordings.",
          "kind": "image",
          "locator": "visual_reading.unresolved",
          "path": "pics/tips/tip_17.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The unresolved note records the stage-wording ambiguity that must be preserved.",
          "kind": "image",
          "locator": "visual_reading.unresolved",
          "path": "pics/tips/tip_17.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-overhead-response-step2",
      "instruction": "Apply draft-overhead-response using the user's real facts: give a concrete analysis such as complexity, time, memory, and amortization, including where the cost is introduced and how it is controlled, rather than answering vaguely that the gain is worth it.",
      "limitations": [
        "All cost, complexity, and time tokens are placeholders; the card supplies no measured values.",
        "The stage wording has an unresolved source-meaning ambiguity (see limitation-tip17-stage-wording).",
        "The wordings themselves were read clearly by the Builder; only their applicable-scenario relationship is unresolved.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "Tip 17's recommended answer first says the method adds about XXX% time at the training/inference stage, then says the overhead is introduced only at training/preprocessing/offline-construction and does not affect online inference. The Builder visual reading records this as an unresolved source-meaning ambiguity because the original card does not reconcile the two statements, so no universal stage guarantee should be read from the example."
      ],
      "title": "Draft the computational overhead reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-overhead-response-step2"
      ],
      "id": "wf-draft-overhead-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-overhead-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for computational-overhead critiques"
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
        "justification": "The conditions note instructs preserving both wordings as scenario-dependent rather than a universal guarantee.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point requires concrete complexity, time, memory, and amortization analysis instead of a vague answer.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the cost source, complexity, stage controllability, parallelization, and amortization argument.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The unresolved note flags the noncritical source-meaning ambiguity between the two stage wordings.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The unresolved note records the stage-wording ambiguity that must be preserved.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-overhead-response",
    "knowledge_ids": [
      "decide-cost-detail-response",
      "limitation-tip17-stage-wording",
      "readme-disclaimer"
    ],
    "limitations": [
      "All cost, complexity, and time tokens are placeholders; the card supplies no measured values.",
      "The stage wording has an unresolved source-meaning ambiguity (see limitation-tip17-stage-wording).",
      "The wordings themselves were read clearly by the Builder; only their applicable-scenario relationship is unresolved.",
      "This records the repository's own stated caveat, not an independent verification of tip quality.",
      "Tip 17's recommended answer first says the method adds about XXX% time at the training/inference stage, then says the overhead is introduced only at training/preprocessing/offline-construction and does not affect online inference. The Builder visual reading records this as an unresolved source-meaning ambiguity because the original card does not reconcile the two statements, so no universal stage guarantee should be read from the example."
    ],
    "scope": "Applies when overhead or cost is the reviewer's concern. The cost source, complexity, and percentages are filled from the user's own measurements (the card's tokens are placeholders). The source card's stage wording is ambiguous between training/inference overhead and offline-only construction that does not affect online inference; no universal stage guarantee should be read from the example, and the user's actual stage placement must come from their own method.",
    "task": "Draft a rebuttal response to a reviewer who questions computational overhead, by giving a concrete analysis such as complexity, time, memory, and amortization, including where the cost is introduced and how it is controlled, rather than answering vaguely that the gain is worth it.",
    "title": "Draft a rebuttal for computational-overhead critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When reviewers question computational overhead, the documented rule (Tip 17) is not to answer vaguely that the gain is worth it. Give a concrete analysis such as complexity, time, memory, and amortization. The example answer: the extra cost comes from XXX with complexity XXX, adding about XXX% time at the training/inference stage versus baseline for a XXX gain; the cost is controllable because it is introduced only at the training/preprocessing/offline-construction stage and does not affect online inference; the relevant steps can be parallelized; at large scale the cost is small relative to model training; and a multi-stage workflow has a one-time-investment, long-term-reuse property because the upfront construction cost is amortized in later inference. The reading records an unresolved ambiguity between the training/inference phrasing and the offline-only phrasing, so no universal stage guarantee should be read from the example.",
    "evidence": [
      {
        "justification": "The core point requires concrete complexity, time, memory, and amortization analysis instead of a vague answer.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the cost source, complexity, stage controllability, parallelization, and amortization argument.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The unresolved note records the stage-wording ambiguity that must be preserved.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-cost-detail-response",
    "limitations": [
      "All cost, complexity, and time tokens are placeholders; the card supplies no measured values.",
      "The stage wording has an unresolved source-meaning ambiguity (see limitation-tip17-stage-wording)."
    ],
    "title": "For overhead critiques, give concrete complexity/time/memory and amortization analysis",
    "type": "DECISION_RULE"
  },
  {
    "confidence": "high",
    "content": "Tip 17's recommended answer first says the method adds about XXX% time at the training/inference stage, then says the overhead is introduced only at training/preprocessing/offline-construction and does not affect online inference. The Builder visual reading records this as an unresolved source-meaning ambiguity because the original card does not reconcile the two statements, so no universal stage guarantee should be read from the example.",
    "evidence": [
      {
        "justification": "The conditions note instructs preserving both wordings as scenario-dependent rather than a universal guarantee.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The unresolved note flags the noncritical source-meaning ambiguity between the two stage wordings.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_17.svg",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-tip17-stage-wording",
    "limitations": [
      "The wordings themselves were read clearly by the Builder; only their applicable-scenario relationship is unresolved."
    ],
    "title": "Tip 17 has an unresolved training/inference vs offline-only stage ambiguity",
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

