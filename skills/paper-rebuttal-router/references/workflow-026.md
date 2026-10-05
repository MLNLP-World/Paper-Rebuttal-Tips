# Workflow 26: Review a supplied rebuttal draft against the documented pitfalls

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "assess-supplied-response-for-documented-pitfalls"
  ],
  "confidence": "high",
  "evidence": [
    {
      "justification": "The principle banner states the formula verbatim.",
      "kind": "documentation",
      "locator": "README.md:L26-L29",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The table labels 反面回答 as 容易踩坑的回复方式, establishing these negative answers as pitfalls.",
      "kind": "documentation",
      "locator": "README.md:L44-L47",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The table labels 反面回答 as 容易踩坑的回复方式.",
      "kind": "documentation",
      "locator": "README.md:L44-L47",
      "path": "README.md",
      "support_type": "explicit"
    },
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
      "justification": "Tip 1's visual reading metadata explicitly records same-model checking and no independent review.",
      "kind": "image",
      "locator": "visual_reading.check_status and visual_reading.independent_review",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 1's condition note states the ablation result is an example claim with no experimental values in the image.",
      "kind": "image",
      "locator": "visual_reading.conditions_and_limits",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 1's negative answer asserts innovation and component necessity without evidence.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_01.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 3's note states the SOTA claim belongs to the negative answer and cannot be used as recommended evidence.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 3's negative answer leans on first-application and SOTA claims.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_03.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 4's negative answer blames the reviewer for not noticing listed contributions.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_04.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 6's negative answer treats experimental performance as sufficient proof of validity.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_06.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 10's negative answer directly tells the reviewer they misunderstood.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_10.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 11's negative answer dismisses the review or questions the reviewer's competence.",
      "kind": "image",
      "locator": "visual_reading.negative_answer",
      "path": "pics/tips/tip_11.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_25.svg",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
      "kind": "image",
      "locator": "visual_reading.example_roles",
      "path": "pics/tips/tip_26.svg",
      "support_type": "explicit"
    }
  ],
  "goal": "Assess a rebuttal draft the user supplies against the repository's documented pitfalls and overall Respect + Evidence + Clarity principle, and report the gaps without rewriting the paper or the reply.",
  "id": "wf-review-supplied-reply-for-documented-pitfalls",
  "limitations": [
    "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
    "The placeholder values and example claims embedded in the card texts are illustrative role-play rather than verified facts or measured results. For example, Tip 1's claim that removing A/B/C each decreases performance and that the full model performs best is an example ablation claim with no experimental values in the image, and Tip 3's claim of SOTA performance appears inside the negative answer and therefore cannot serve as recommended evidence.",
    "The synthesis is scoped to the three cited negative answers; claims in other cards may differ in wording.",
    "The synthesis is scoped to the three cited negative answers; other cards were not exhaustively checked for similar blame patterns.",
    "The tip SVG contents are supplied as manual Builder image acquisitions with a same-model check only: the visual readings carry check_status 'same_model_checked' and independent_review false, the raw SVG XML was not text-parsed, and no independent visual review was performed. As a result, exact wording and pixel-region claims in the card transcriptions are not independently corroborated.",
    "The two cited placeholders are representative; the same illustrative-status concern generalizes to the other cards only through their similar placeholder annotations.",
    "This concerns the supplied transcription evidence generally; it does not by itself invalidate any specific reading.",
    "This is a documentation claim and does not establish that any particular tip card instantiates the principle.",
    "This records the repository's own stated caveat, not an independent verification of tip quality.",
    "This step only checks whether the requested draft material is present; it does not analyze or review the draft."
  ],
  "scope": "Applies to drafts the user supplies for assessment. The workflow reports gaps and does not automatically rewrite the paper or the reply; the pitfall synthesis is scoped to the cited negative answers, the listed placeholders are representative rather than an exhaustive enumeration across all 28 cards, and the transcriptions the pitfalls derive from carry a same-model check without independent visual review. Requires the user to supply the rebuttal draft; without a draft, no review is completed.",
  "steps": [
    {
      "confidence": "high",
      "depends_on": [],
      "id": "wf-review-supplied-reply-for-documented-pitfalls-step1",
      "instruction": "Confirm the user has supplied the rebuttal draft to be assessed; if no draft is supplied, record the draft as 未提供 and stop without claiming the review was completed.",
      "limitations": [
        "This step only checks whether the requested draft material is present; it does not analyze or review the draft."
      ],
      "rationale": "The assessment capability requires a user-supplied draft, so the workflow must verify the required input before calling it.",
      "title": "Confirm the rebuttal draft is supplied and record missing material",
      "type": "ORCHESTRATION_STEP"
    },
    {
      "capability_id": "assess-supplied-response-for-documented-pitfalls",
      "confidence": "high",
      "depends_on": [
        "wf-review-supplied-reply-for-documented-pitfalls-step1"
      ],
      "evidence": [
        {
          "justification": "The principle banner states the formula verbatim.",
          "kind": "documentation",
          "locator": "README.md:L26-L29",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The table labels 反面回答 as 容易踩坑的回复方式, establishing these negative answers as pitfalls.",
          "kind": "documentation",
          "locator": "README.md:L44-L47",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The table labels 反面回答 as 容易踩坑的回复方式.",
          "kind": "documentation",
          "locator": "README.md:L44-L47",
          "path": "README.md",
          "support_type": "explicit"
        },
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
          "justification": "Tip 1's visual reading metadata explicitly records same-model checking and no independent review.",
          "kind": "image",
          "locator": "visual_reading.check_status and visual_reading.independent_review",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 1's condition note states the ablation result is an example claim with no experimental values in the image.",
          "kind": "image",
          "locator": "visual_reading.conditions_and_limits",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 1's negative answer asserts innovation and component necessity without evidence.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_01.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 3's note states the SOTA claim belongs to the negative answer and cannot be used as recommended evidence.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 3's negative answer leans on first-application and SOTA claims.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_03.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 4's negative answer blames the reviewer for not noticing listed contributions.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_04.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 6's negative answer treats experimental performance as sufficient proof of validity.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_06.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 10's negative answer directly tells the reviewer they misunderstood.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_10.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 11's negative answer dismisses the review or questions the reviewer's competence.",
          "kind": "image",
          "locator": "visual_reading.negative_answer",
          "path": "pics/tips/tip_11.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_25.svg",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
          "kind": "image",
          "locator": "visual_reading.example_roles",
          "path": "pics/tips/tip_26.svg",
          "support_type": "explicit"
        }
      ],
      "id": "wf-review-supplied-reply-for-documented-pitfalls-step2",
      "instruction": "Apply assess-supplied-response-for-documented-pitfalls to the user-supplied rebuttal draft: report gaps for assertions of novelty or effectiveness without concrete evidence, reviewer-blaming or adversarial responses, example or placeholder claims presented as verified results, and departures from the Respect + Evidence + Clarity principle. Do not rewrite the paper or the reply.",
      "limitations": [
        "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
        "The placeholder values and example claims embedded in the card texts are illustrative role-play rather than verified facts or measured results. For example, Tip 1's claim that removing A/B/C each decreases performance and that the full model performs best is an example ablation claim with no experimental values in the image, and Tip 3's claim of SOTA performance appears inside the negative answer and therefore cannot serve as recommended evidence.",
        "The synthesis is scoped to the three cited negative answers; claims in other cards may differ in wording.",
        "The synthesis is scoped to the three cited negative answers; other cards were not exhaustively checked for similar blame patterns.",
        "The tip SVG contents are supplied as manual Builder image acquisitions with a same-model check only: the visual readings carry check_status 'same_model_checked' and independent_review false, the raw SVG XML was not text-parsed, and no independent visual review was performed. As a result, exact wording and pixel-region claims in the card transcriptions are not independently corroborated.",
        "The two cited placeholders are representative; the same illustrative-status concern generalizes to the other cards only through their similar placeholder annotations.",
        "This concerns the supplied transcription evidence generally; it does not by itself invalidate any specific reading.",
        "This is a documentation claim and does not establish that any particular tip card instantiates the principle.",
        "This records the repository's own stated caveat, not an independent verification of tip quality."
      ],
      "title": "Assess the supplied rebuttal draft against the documented pitfalls",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Review a supplied rebuttal draft against the documented pitfalls"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "high",
    "evidence": [
      {
        "justification": "The principle banner states the formula verbatim.",
        "kind": "documentation",
        "locator": "README.md:L26-L29",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The table labels 反面回答 as 容易踩坑的回复方式, establishing these negative answers as pitfalls.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The table labels 反面回答 as 容易踩坑的回复方式.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      },
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
        "justification": "Tip 1's visual reading metadata explicitly records same-model checking and no independent review.",
        "kind": "image",
        "locator": "visual_reading.check_status and visual_reading.independent_review",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's condition note states the ablation result is an example claim with no experimental values in the image.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's negative answer asserts innovation and component necessity without evidence.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's note states the SOTA claim belongs to the negative answer and cannot be used as recommended evidence.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's negative answer leans on first-application and SOTA claims.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 4's negative answer blames the reviewer for not noticing listed contributions.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 6's negative answer treats experimental performance as sufficient proof of validity.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 10's negative answer directly tells the reviewer they misunderstood.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 11's negative answer dismisses the review or questions the reviewer's competence.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      }
    ],
    "id": "assess-supplied-response-for-documented-pitfalls",
    "knowledge_ids": [
      "failure-claims-without-evidence",
      "failure-reviewer-blaming",
      "limitation-builder-transcription-no-independent-review",
      "limitation-placeholder-claims",
      "placeholder-token-convention",
      "principle-respect-evidence-clarity",
      "readme-disclaimer"
    ],
    "limitations": [
      "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards.",
      "The placeholder values and example claims embedded in the card texts are illustrative role-play rather than verified facts or measured results. For example, Tip 1's claim that removing A/B/C each decreases performance and that the full model performs best is an example ablation claim with no experimental values in the image, and Tip 3's claim of SOTA performance appears inside the negative answer and therefore cannot serve as recommended evidence.",
      "The synthesis is scoped to the three cited negative answers; claims in other cards may differ in wording.",
      "The synthesis is scoped to the three cited negative answers; other cards were not exhaustively checked for similar blame patterns.",
      "The tip SVG contents are supplied as manual Builder image acquisitions with a same-model check only: the visual readings carry check_status 'same_model_checked' and independent_review false, the raw SVG XML was not text-parsed, and no independent visual review was performed. As a result, exact wording and pixel-region claims in the card transcriptions are not independently corroborated.",
      "The two cited placeholders are representative; the same illustrative-status concern generalizes to the other cards only through their similar placeholder annotations.",
      "This concerns the supplied transcription evidence generally; it does not by itself invalidate any specific reading.",
      "This is a documentation claim and does not establish that any particular tip card instantiates the principle.",
      "This records the repository's own stated caveat, not an independent verification of tip quality."
    ],
    "scope": "Applies to drafts the user supplies for assessment; the capability reports gaps, it does not automatically rewrite the paper or the reply. The pitfall synthesis is scoped to the cited negative answers, the listed placeholders are representative rather than an exhaustive enumeration across all 28 cards, and the transcriptions the pitfalls derive from carry a same-model check without independent visual review. GPT-4 and Gemini-Pro are the source card's named example judge models, not verified objective judges.",
    "task": "Review a supplied rebuttal draft against the repository's documented pitfalls and overall principle, and report the gaps: assertions of novelty or effectiveness without concrete evidence, reviewer-blaming or adversarial responses, example or placeholder claims presented as verified results, and departures from the Respect + Evidence + Clarity principle.",
    "title": "Assess a supplied rebuttal draft against the documented pitfalls"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "Several negative answers exemplify the documented failure of asserting novelty or effectiveness without giving concrete supporting evidence: Tip 1's negative answer asserts innovation and that each component is necessary without support; Tip 3's negative answer claims first application plus SOTA performance as the main justification; and Tip 6's negative answer argues the method is valid merely because it performed well in experiments.",
    "evidence": [
      {
        "justification": "The table labels 反面回答 as 容易踩坑的回复方式.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 1's negative answer asserts innovation and component necessity without evidence.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's negative answer leans on first-application and SOTA claims.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 6's negative answer treats experimental performance as sufficient proof of validity.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_06.svg",
        "support_type": "explicit"
      }
    ],
    "id": "failure-claims-without-evidence",
    "limitations": [
      "The synthesis is scoped to the three cited negative answers; claims in other cards may differ in wording."
    ],
    "title": "Asserting novelty or effectiveness without concrete evidence is a documented pitfall",
    "type": "FAILURE_MODE"
  },
  {
    "confidence": "high",
    "content": "Several negative answers exemplify a documented failure of blaming or confronting the reviewer instead of addressing substance: Tip 4's negative answer attributes missing contributions to the reviewer not reading them (可能是审稿人没有注意到); Tip 10's negative answer directly says the reviewer misunderstood (您可能误解了我们的方法); and Tip 11's negative answer dismisses the review as too vague or attacks the reviewer's professionalism and judgment.",
    "evidence": [
      {
        "justification": "The table labels 反面回答 as 容易踩坑的回复方式, establishing these negative answers as pitfalls.",
        "kind": "documentation",
        "locator": "README.md:L44-L47",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 4's negative answer blames the reviewer for not noticing listed contributions.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_04.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 10's negative answer directly tells the reviewer they misunderstood.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_10.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 11's negative answer dismisses the review or questions the reviewer's competence.",
        "kind": "image",
        "locator": "visual_reading.negative_answer",
        "path": "pics/tips/tip_11.svg",
        "support_type": "explicit"
      }
    ],
    "id": "failure-reviewer-blaming",
    "limitations": [
      "The synthesis is scoped to the three cited negative answers; other cards were not exhaustively checked for similar blame patterns."
    ],
    "title": "Blame and adversarial responses toward the reviewer are documented pitfalls",
    "type": "FAILURE_MODE"
  },
  {
    "confidence": "high",
    "content": "The tip SVG contents are supplied as manual Builder image acquisitions with a same-model check only: the visual readings carry check_status 'same_model_checked' and independent_review false, the raw SVG XML was not text-parsed, and no independent visual review was performed. As a result, exact wording and pixel-region claims in the card transcriptions are not independently corroborated.",
    "evidence": [
      {
        "justification": "Tip 1's visual reading metadata explicitly records same-model checking and no independent review.",
        "kind": "image",
        "locator": "visual_reading.check_status and visual_reading.independent_review",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-builder-transcription-no-independent-review",
    "limitations": [
      "This concerns the supplied transcription evidence generally; it does not by itself invalidate any specific reading."
    ],
    "title": "Tip SVG content derives from same-model Builder readings without independent review",
    "type": "LIMITATION"
  },
  {
    "confidence": "high",
    "content": "The placeholder values and example claims embedded in the card texts are illustrative role-play rather than verified facts or measured results. For example, Tip 1's claim that removing A/B/C each decreases performance and that the full model performs best is an example ablation claim with no experimental values in the image, and Tip 3's claim of SOTA performance appears inside the negative answer and therefore cannot serve as recommended evidence.",
    "evidence": [
      {
        "justification": "Tip 1's condition note states the ablation result is an example claim with no experimental values in the image.",
        "kind": "image",
        "locator": "visual_reading.conditions_and_limits",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's note states the SOTA claim belongs to the negative answer and cannot be used as recommended evidence.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-placeholder-claims",
    "limitations": [
      "The two cited placeholders are representative; the same illustrative-status concern generalizes to the other cards only through their similar placeholder annotations."
    ],
    "title": "Placeholder values and example claims are illustrative, not verified results",
    "type": "LIMITATION"
  },
  {
    "confidence": "high",
    "content": "Across the inspected tip card visual readings, example rebuttal prose uses placeholder tokens such as XXX, X, A/B/C, N, 表 X, and XX% as illustrative fill-ins for method components, datasets, metrics, hyperparameters, and measured results rather than real values. Examples include Tip 1's component placeholders (A/B/C, XXX), Tip 3's innovation placeholder (XXX), and Tip 25's human-evaluation placeholders (N 名标注者, XXX 个样本, κ = XXX). GPT-4 and Gemini-Pro are not placeholder tokens of this kind: the Tip 26 visual reading records them as the source card's named example judge models, and the claims attached to them (客观裁判, 显著优于) are the source example's wording, not verified tool capability or an independent check.",
    "evidence": [
      {
        "justification": "Tip 1's example_roles records A/B/C and XXX as placeholders.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_01.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 3's example_roles records XXX as a placeholder for the innovation/unsolved problem.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_03.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 25's example_roles records N and XXX as placeholders, not measured values.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_25.svg",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 26's example_roles records GPT-4 and Gemini-Pro as the source card's named example judge models and the attached claims as source-example wording.",
        "kind": "image",
        "locator": "visual_reading.example_roles",
        "path": "pics/tips/tip_26.svg",
        "support_type": "explicit"
      }
    ],
    "id": "placeholder-token-convention",
    "limitations": [
      "Scope is the three cited placeholder readings plus the Tip 26 named-judge clarification and the general regularity observed in the supplied readings; occurrences were not exhaustively enumerated across all 28 cards."
    ],
    "title": "Tip card examples routinely use placeholder tokens instead of concrete values",
    "type": "CONVENTION"
  },
  {
    "confidence": "high",
    "content": "The README states the repository's overall principle as 'Good rebuttal = Respect + Evidence + Clarity', with the Chinese gloss 尊重审稿人 · 给出证据 · 澄清贡献.",
    "evidence": [
      {
        "justification": "The principle banner states the formula verbatim.",
        "kind": "documentation",
        "locator": "README.md:L26-L29",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "principle-respect-evidence-clarity",
    "limitations": [
      "This is a documentation claim and does not establish that any particular tip card instantiates the principle."
    ],
    "title": "Overall rebuttal principle is Respect + Evidence + Clarity",
    "type": "FACT"
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

