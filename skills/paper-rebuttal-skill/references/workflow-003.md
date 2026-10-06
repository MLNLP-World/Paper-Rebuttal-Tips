# Workflow 3: Draft a rebuttal for missing-baseline critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-baseline-coverage-response"
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
      "justification": "The core point prescribes baseline-coverage explanation and adds experiments or representativeness justification instead of resource excuses.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_13.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that explains the compared baselines' coverage and adds comparison experiments or a representativeness justification instead of citing time and resource limits.",
  "id": "wf-draft-baseline-coverage-response",
  "limitations": [
    "The core point retains a fallback branch (无法完整补充) that does not promise an actual full additional comparison.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when a reviewer questions baseline coverage. The fallback branch does not promise an actual full additional comparison when it cannot be completed. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-draft-baseline-coverage-response-step1",
      "instruction": "Confirm the reviewer point concerns baseline coverage (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the baselines the user already compared and the rationale for their representativeness, or a plan for additional comparison experiments and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-baseline-coverage-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the baseline coverage point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-baseline-coverage-response",
      "confidence": "high",
      "depends_on": [
        "wf-draft-baseline-coverage-response-step1"
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
          "justification": "The core point prescribes baseline-coverage explanation and adds experiments or representativeness justification instead of resource excuses.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_13.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-baseline-coverage-response-step2",
      "instruction": "Apply draft-baseline-coverage-response using the user's real facts: explain the coverage of the baselines already compared and either add executable comparison experiments or justify, with algorithmic or logical analysis, why the existing baselines are representative, without using time and resource limits as the main excuse.",
      "limitations": [
        "The core point retains a fallback branch (无法完整补充) that does not promise an actual full additional comparison.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the baseline coverage reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "high",
      "depends_on": [
        "wf-draft-baseline-coverage-response-step2"
      ],
      "id": "wf-draft-baseline-coverage-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-baseline-coverage-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for missing-baseline critiques"
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
        "justification": "The core point prescribes baseline-coverage explanation and adds experiments or representativeness justification instead of resource excuses.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_13.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-baseline-coverage-response",
    "knowledge_ids": [
      "decide-strong-baseline-response",
      "readme-disclaimer"
    ],
    "limitations": [
      "The core point retains a fallback branch (无法完整补充) that does not promise an actual full additional comparison.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer questions baseline coverage. The fallback branch does not promise an actual full additional comparison when it cannot be completed.",
    "task": "Draft a rebuttal response to a reviewer who criticizes the absence of the latest or strongest baselines, by explaining the coverage of baselines already compared and either adding executable comparison experiments or justifying why the existing baselines are representative, ideally with algorithmic or logical analysis, rather than using time and resource limits as the main excuse.",
    "title": "Draft a rebuttal for missing-baseline critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When criticized for not comparing to the latest or strongest baselines, the documented rule (Tip 13) is not to use time and resource limits as the main excuse. Explain the coverage of baselines already compared, and either add executable comparison experiments or explain why the existing baselines are representative, ideally with some algorithmic/logical analysis.",
    "evidence": [
      {
        "justification": "The core point prescribes baseline-coverage explanation and adds experiments or representativeness justification instead of resource excuses.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_13.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-strong-baseline-response",
    "limitations": [
      "The core point retains a fallback branch (无法完整补充) that does not promise an actual full additional comparison."
    ],
    "title": "For missing strong baselines explain coverage and add experiments or justify representativeness",
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

