# Workflow 20: Draft a rebuttal for novelty and related-work critiques

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "draft-novelty-and-related-work-response"
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
      "justification": "Tip 2's recommended answer enumerates three labeled difference dimensions.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_02.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The core point prescribes emphasizing the core innovation, synergy mechanism, deep coupling, and contribution to the field.",
      "kind": "image",
      "locator": "visual_reading.core_point",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The reading places the SOTA claim inside the negative answer, so it cannot serve as recommended evidence.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "The recommended answer demonstrates the XXX innovation plus the A-with-B synergy mechanism.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 8's recommended answer enumerates per-work focus and assumes a contrast between C's assumption and this paper.",
      "kind": "image",
      "locator": "visual_reading.recommended_answer",
      "path": "pics/tips/tip_08.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Draft a reply that presents the core innovation and its synergy mechanism with labeled dimensions of difference from prior work instead of bare novelty claims.",
  "id": "wf-draft-novelty-and-related-work-response",
  "limitations": [
    "Module A/B and XXX are placeholder tokens; no measured performance values are supplied.",
    "The shared-shape generalization is a bounded synthesis from the two cited examples, which use placeholder tokens (XXX) rather than real papers.",
    "The synergy phrasing is the card's example answer for the card's example scenario; the specific mechanism must come from the user's own paper.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts.",
    "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
  ],
  "scope": "Applies when a reviewer questions novelty or the relation to prior work. The core innovation, synergy mechanism, and module roles are filled from the user's own paper (the card's XXX and A/B placeholders are not real components), and labeled dimensions such as motivation, implementation, and effect, or per-related-work focus plus the closest work's differing assumption, are a structure the user fills with real differences. Adding the comparison to the revision remains a revision commitment, not a completed edit. The documented pitfall of asserting novelty or effectiveness without concrete evidence is the pattern this task must avoid. The workflow drafts this point's reply only: other reviewer points are handled by their own workflows, and an analysis-only request without a drafting request uses the analysis workflow instead.",
  "steps": [
    {
      "confidence": "medium",
      "depends_on": [],
      "id": "wf-draft-novelty-and-related-work-response-step1",
      "instruction": "Confirm the reviewer point concerns novelty or the relation to prior work (a topic match rather than a generic negative review) and that the user asked to draft a reply for this point (an analysis-only request without a drafting request uses the analysis workflow); collect the user's actual core innovation, its synergy mechanism, and the real differences from the closest prior work and record which are present and which are missing; check whether the strategy's conditions hold for the user's actual setup (condition-applicable) rather than assuming they do; do not substitute the card's example values for the user's facts.",
      "limitations": [
        "This step only checks the point's topic, the user's drafting request, and input completeness; it does not draft the reply and does not substitute example placeholders for the user's facts."
      ],
      "rationale": "The draft-novelty-and-related-work-response strategy needs the user's real material and applies only when the point matches its topic and its conditions hold for the user's setup; checking this first keeps the drafting step grounded instead of assuming the card's examples.",
      "title": "Confirm the novelty or the relation to prior work point, the drafting request, and the required material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "draft-novelty-and-related-work-response",
      "confidence": "medium",
      "depends_on": [
        "wf-draft-novelty-and-related-work-response-step1"
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
          "justification": "Tip 2's recommended answer enumerates three labeled difference dimensions.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_02.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The core point prescribes emphasizing the core innovation, synergy mechanism, deep coupling, and contribution to the field.",
          "kind": "image",
          "locator": "visual_reading.core_point",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The reading places the SOTA claim inside the negative answer, so it cannot serve as recommended evidence.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "The recommended answer demonstrates the XXX innovation plus the A-with-B synergy mechanism.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 8's recommended answer enumerates per-work focus and assumes a contrast between C's assumption and this paper.",
          "kind": "image",
          "locator": "visual_reading.recommended_answer",
          "path": "pics/tips/tip_08.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-draft-novelty-and-related-work-response-step2",
      "instruction": "Apply draft-novelty-and-related-work-response using the user's real facts: present the core innovation and its synergy mechanism and structure the difference from prior work as labeled dimensions, rather than asserting bare novelty, a first application, or a SOTA slogan.",
      "limitations": [
        "Module A/B and XXX are placeholder tokens; no measured performance values are supplied.",
        "The shared-shape generalization is a bounded synthesis from the two cited examples, which use placeholder tokens (XXX) rather than real papers.",
        "The synergy phrasing is the card's example answer for the card's example scenario; the specific mechanism must come from the user's own paper.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Draft the novelty or the relation to prior work reply",
      "type": "CAPABILITY_STEP"
    },
    {
      "confidence": "medium",
      "depends_on": [
        "wf-draft-novelty-and-related-work-response-step2"
      ],
      "id": "wf-draft-novelty-and-related-work-response-step3",
      "instruction": "Organize this reviewer point's result as: reviewer point; existing response or missing; selected strategy (draft-novelty-and-related-work-response); applicability reason; feedback or requested draft; missing evidence; unresolved items. Present the capability's limitations with the result. Missing material limits only this point's steps and does not block other reviewer points, which continue through their own workflows.",
      "limitations": [
        "This step only organizes this reviewer point's result; it does not cover other reviewer points, does not claim completed experiments, and does not claim a draft review was performed when no draft was supplied."
      ],
      "rationale": "The per-point result structure lets the user see what was applied, why it applies, what was produced, and what stays unresolved, without merging reviewer points or inventing missing material.",
      "title": "Organize this reviewer point's result",
      "type": "ORCHESTRATION_STEP"
    }
  ],
  "title": "Draft a rebuttal for novelty and related-work critiques"
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
        "justification": "Tip 2's recommended answer enumerates three labeled difference dimensions.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_02.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The core point prescribes emphasizing the core innovation, synergy mechanism, deep coupling, and contribution to the field.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The reading places the SOTA claim inside the negative answer, so it cannot serve as recommended evidence.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the XXX innovation plus the A-with-B synergy mechanism.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 8's recommended answer enumerates per-work focus and assumes a contrast between C's assumption and this paper.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_08.svg",
        "support_type": "explicit"
      }
    ],
    "id": "draft-novelty-and-related-work-response",
    "knowledge_ids": [
      "decide-combination-critique-response",
      "example-dimension-contrast",
      "readme-disclaimer"
    ],
    "limitations": [
      "Module A/B and XXX are placeholder tokens; no measured performance values are supplied.",
      "The shared-shape generalization is a bounded synthesis from the two cited examples, which use placeholder tokens (XXX) rather than real papers.",
      "The synergy phrasing is the card's example answer for the card's example scenario; the specific mechanism must come from the user's own paper.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies when a reviewer questions novelty or the relation to prior work. The core innovation, synergy mechanism, and module roles are filled from the user's own paper (the card's XXX and A/B placeholders are not real components), and labeled dimensions such as motivation, implementation, and effect, or per-related-work focus plus the closest work's differing assumption, are a structure the user fills with real differences. Adding the comparison to the revision remains a revision commitment, not a completed edit. The documented pitfall of asserting novelty or effectiveness without concrete evidence is the pattern this task must avoid.",
    "task": "Draft a rebuttal response to a reviewer who challenges the work's novelty, dismisses it as a combination of existing techniques, or questions its relation to prior work, by presenting the core innovation and its synergy mechanism and by structuring the difference from prior work as labeled dimensions, rather than asserting bare novelty, a first application, or a SOTA slogan.",
    "title": "Draft a rebuttal for novelty and related-work critiques"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When reviewers dismiss the work as merely combining existing techniques, the documented rule (Tip 3) is not to answer with first application plus a SOTA slogan. Instead, positively respond by emphasizing the core innovation, the synergy mechanism, the deep coupling between modules, and the contribution to the field. The recommended answer names the core innovation (XXX) and presents basic modules such as retrieval and summarization as serving that innovation rather than engineering assembly: module A combined with B solves XXX that traditional methods handle poorly, and this deep coupling brings the performance gain. The SOTA-performance slogan appears only in the negative answer.",
    "evidence": [
      {
        "justification": "The core point prescribes emphasizing the core innovation, synergy mechanism, deep coupling, and contribution to the field.",
        "kind": "image",
        "locator": "visual_reading.core_point",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The reading places the SOTA claim inside the negative answer, so it cannot serve as recommended evidence.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "The recommended answer demonstrates the XXX innovation plus the A-with-B synergy mechanism.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      }
    ],
    "id": "decide-combination-critique-response",
    "limitations": [
      "Module A/B and XXX are placeholder tokens; no measured performance values are supplied.",
      "The synergy phrasing is the card's example answer for the card's example scenario; the specific mechanism must come from the user's own paper."
    ],
    "title": "For combination-of-existing-techniques critiques, answer with the core innovation and the synergy mechanism",
    "type": "DECISION_RULE"
  },
  {
    "confidence": "medium",
    "content": "For novelty or related-work challenges, the recommended answers in Tip 2 and Tip 8 structure the difference from prior work as explicitly labeled dimensions rather than as a bare assertion of difference: Tip 2 enumerates 动机不同, 实现方式不同, and 作用不同 between this paper and method A; Tip 8 enumerates what related works A, B, and C each focus on, identifies C as closest, and contrasts C's core assumption with this paper's focus. Both close by promising to add the comparison in the revision.",
    "evidence": [
      {
        "justification": "Tip 2's recommended answer enumerates three labeled difference dimensions.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_02.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 8's recommended answer enumerates per-work focus and assumes a contrast between C's assumption and this paper.",
        "kind": "image",
        "locator": "visual_reading.recommended_answer",
        "path": "pics/tips/tip_08.svg",
        "support_type": "explicit"
      }
    ],
    "id": "example-dimension-contrast",
    "limitations": [
      "The shared-shape generalization is a bounded synthesis from the two cited examples, which use placeholder tokens (XXX) rather than real papers."
    ],
    "title": "Novelty and related-work responses structure differences as labeled dimensions",
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

