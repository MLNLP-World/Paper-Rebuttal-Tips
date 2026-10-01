# Workflow 7: Draft a rebuttal for design-necessity and hyperparameter-sensitivity critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-design-necessity-and-hyperparameter-response"
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
      "justification": "Tip 1's negative answer provides the pitfall side of the pair.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 1's recommended answer supplies the contrasting strategy for the same question.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 23's core point requires explaining the test range, the result trend, and the reasonableness of the final value rather than reporting only the best result.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_23.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 23's negative answer reports only the best-result rationale.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_23.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 23's recommended answer supplies the sensitivity-analysis contrast for the same k=40 question.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_23.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The unresolved note flags the II-shaped mark as a noncritical layout item with no source explanation.",
      "kind": "image",
      "locator": "visual_reading.unresolved",
      "path": "pics/tips/tip_23.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply for the matching scenario: design motivation plus per-component reasoning for a complexity critique, or tested range, trend, and trade-off for a hyperparameter-sensitivity critique.",
  "id": "wf-draft-design-necessity-and-hyperparameter-response",
  "limitations": [
    "Scope is the two cited cards; this contrastive shape was verified against these examples rather than all 28 cards.",
    "The mark is visually confirmed but unexplained; its meaning cannot be recovered from the supplied material.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied.",
    "Tip 23 contains an II-shaped two-stroke mark below the recommended-answer sample label whose meaning the original image does not explain. The Builder visual reading records it as an unresolved layout item and states it should not be treated as another answer or a numeric conclusion."
  ],
  "scope": "Applies to the two cited card scenarios (method complexity and hyperparameter sensitivity); each scenario keeps its own recommended strategy and must not be substituted by the ablation task. k=40 in the hyperparameter example is an example value, not a recommended setting, and the card supplies no concrete range values. The unexplained II-shaped mark in Tip 23 is recorded as unresolved and must not be read as another answer or a numeric conclusion. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "medium",
      "depends_on": [],
      "id": "wf-draft-design-necessity-and-hyperparameter-response-step1",
      "instruction": "Confirm the reviewer point concerns method complexity or hyperparameter sensitivity (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect which of the two scenarios the point matches, and for it the design motivation with per-component reasoning, or the tested hyperparameter range, result trend, and final-value trade-off and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-design-necessity-and-hyperparameter-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the method complexity or hyperparameter sensitivity point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-design-necessity-and-hyperparameter-response",
      "confidence": "medium",
      "depends_on": [
        "wf-draft-design-necessity-and-hyperparameter-response-step1"
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
          "justification": "Tip 1's negative answer provides the pitfall side of the pair.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 1's recommended answer supplies the contrasting strategy for the same question.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 23's core point requires explaining the test range, the result trend, and the reasonableness of the final value rather than reporting only the best result.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_23.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 23's negative answer reports only the best-result rationale.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_23.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 23's recommended answer supplies the sensitivity-analysis contrast for the same k=40 question.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_23.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The unresolved note flags the II-shaped mark as a noncritical layout item with no source explanation.",
          "kind": "image",
          "locator": "visual_reading.unresolved",
          "path": "pics/tips/tip_23.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-design-necessity-and-hyperparameter-response-step2",
      "instruction": "Apply draft-design-necessity-and-hyperparameter-response using the user's real facts: answer the matching scenario only: for a method-too-complex critique, supply design motivation plus per-component ablation reasoning instead of bare novelty and universal component necessity; for a hyperparameter-sensitivity critique, report the tested range, the result trend, and the justification of the final value through its performance/efficiency trade-off instead of reporting only the best result.",
      "limitations": [
        "Scope is the two cited cards; this contrastive shape was verified against these examples rather than all 28 cards.",
        "The mark is visually confirmed but unexplained; its meaning cannot be recovered from the supplied material.",
        "This records the repository's own stated caveat, not an independent verification of tip quality.",
        "Tip 23 contains an II-shaped two-stroke mark below the recommended-answer sample label whose meaning the original image does not explain. The Builder visual reading records it as an unresolved layout item and states it should not be treated as another answer or a numeric conclusion."
      ],
      "title": "Draft the method complexity or hyperparameter sensitivity reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "medium",
      "depends_on": [
        "wf-draft-design-necessity-and-hyperparameter-response-step2"
      ],
      "id": "wf-draft-design-necessity-and-hyperparameter-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-design-necessity-and-hyperparameter-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for design-necessity and hyperparameter-sensitivity critiques"
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
        "justification": "Tip 1's negative answer provides the pitfall side of the pair.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's recommended answer supplies the contrasting strategy for the same question.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's core point requires explaining the test range, the result trend, and the reasonableness of the final value rather than reporting only the best result.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's negative answer reports only the best-result rationale.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's recommended answer supplies the sensitivity-analysis contrast for the same k=40 question.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The unresolved note flags the II-shaped mark as a noncritical layout item with no source explanation.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-design-necessity-and-hyperparameter-response",
    "knowledge_ids": [
      "example-contrastive-pair",
      "limitation-tip23-unexplained-glyph",
      "readme-disclaimer"
    ],
    "limitations": [
      "Scope is the two cited cards; this contrastive shape was verified against these examples rather than all 28 cards.",
      "The mark is visually confirmed but unexplained; its meaning cannot be recovered from the supplied material.",
      "This records the repository's own stated caveat, not an independent verification of tip quality.",
      "Tip 23 contains an II-shaped two-stroke mark below the recommended-answer sample label whose meaning the original image does not explain. The Builder visual reading records it as an unresolved layout item and states it should not be treated as another answer or a numeric conclusion."
    ],
    "scope": "Applies to the two cited card scenarios (method complexity and hyperparameter sensitivity); each scenario keeps its own recommended strategy and must not be substituted by the ablation task. k=40 in the hyperparameter example is an example value, not a recommended setting, and the card supplies no concrete range values. The unexplained II-shaped mark in Tip 23 is recorded as unresolved and must not be read as another answer or a numeric conclusion.",
    "task": "Draft a rebuttal response in either of two distinct scenarios the cards cover as contrastive pairs: (1) a method-too-complex critique, by supplying design motivation plus per-component ablation reasoning instead of bare novelty and universal component necessity; or (2) a hyperparameter-sensitivity critique, by reporting the tested range, the result trend, and the justification of the final value through its performance/efficiency trade-off instead of reporting only the best result.",
    "title": "Draft a rebuttal for design-necessity and hyperparameter-sensitivity critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "medium",
    "content": "The tip cards pair, for the same reviewer question, a negative answer and a recommended answer, creating a contrastive do/don't shape. In Tip 1 (method too complex) the negative answer asserts bare novelty and universal component necessity while the recommended answer supplies design motivation plus per-component ablation reasoning. In Tip 23 (hyperparameter sensitivity) the negative answer reports only the best result (k=40) while the recommended answer reports a k sensitivity analysis and explains the performance/efficiency trade-off behind the default value; the core point further requires stating the test range and the result trend and justifying the final value, and the card does not supply concrete k range values.",
    "evidence": [
      {
        "justification": "Tip 1's negative answer provides the pitfall side of the pair.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's recommended answer supplies the contrasting strategy for the same question.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's core point requires explaining the test range, the result trend, and the reasonableness of the final value rather than reporting only the best result.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's negative answer reports only the best-result rationale.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 23's recommended answer supplies the sensitivity-analysis contrast for the same k=40 question.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      }
    ],
    "id": "example-contrastive-pair",
    "limitations": [
      "Scope is the two cited cards; this contrastive shape was verified against these examples rather than all 28 cards."
    ],
    "title": "Cards pair a negative answer with a recommended answer for contrastive drafting",
    "type": "EXAMPLE_PATTERN"
  },
  {
    "confidence": "high",
    "content": "Tip 23 contains an II-shaped two-stroke mark below the recommended-answer sample label whose meaning the original image does not explain. The Builder visual reading records it as an unresolved layout item and states it should not be treated as another answer or a numeric conclusion.",
    "evidence": [
      {
        "justification": "The unresolved note flags the II-shaped mark as a noncritical layout item with no source explanation.",
        "kind": "image",
        "locator": "visual_reading.unresolved",
        "path": "pics/tips/tip_23.svg",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-tip23-unexplained-glyph",
    "limitations": [
      "The mark is visually confirmed but unexplained; its meaning cannot be recovered from the supplied material."
    ],
    "title": "Tip 23 contains an unexplained II-shaped mark",
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

