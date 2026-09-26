# Workflow 2: Review a rebuttal draft against supplied reviewer concerns

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "review-rebuttal-framing-and-concern-categories"
  ],
  "confidence": "high",
  "evidence": [
    {
      "justification": "The introduction directly states the audience and the project's framing of rebuttal writing.",
      "kind": "documentation",
      "locator": "Opening subtitle, 'Good rebuttal = Respect + Evidence + Clarity', and 项目动机",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The tip summary directly states this strategy.",
      "kind": "documentation",
      "locator": "写作澄清、相关工作与沟通策略类 > Tip 12 summary",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The disclaimer directly states these applicability restrictions and the content's reported origins.",
      "kind": "documentation",
      "locator": "项目动机 > ⚠️ 免责声明 > first and second paragraphs",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The disclaimer identifies variable conference conditions and explicitly defers to official conference instructions.",
      "kind": "documentation",
      "locator": "项目动机 > ⚠️ 免责声明 > first paragraph",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The table explicitly associates the three topic categories with these tip ranges.",
      "kind": "documentation",
      "locator": "📚 Rebuttal Tips introductory category table",
      "path": "README.md",
      "support_type": "explicit"
    }
  ],
  "goal": "Provide qualitative feedback on a user-supplied AI or large-model research conference rebuttal draft and reviewer concerns, identifying relevant documented concern categories and decisions requiring official conference instructions.",
  "id": "review-supplied-rebuttal",
  "limitations": [
    "No particular conference's official rules are supplied.",
    "Only the title is available; the detailed strategy, examples, and qualifications in the referenced image are uninspected.",
    "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
    "The README's conference-rule and applicability caveats still apply.",
    "The category table and tip titles are inspected; the embedded tip image contents are not supplied.",
    "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
    "This describes the guide's stated approach, not demonstrated effectiveness or permission to add experiments at any particular conference."
  ],
  "scope": "An agent-designed review plan bounded to the guide's stated framing, three topic categories, and Tip 12's title-level preference for direct action over promises alone. Conference-specific instructions may be used only when supplied by the user. The plan does not retrieve rules, supply omitted tip details, execute experiments, or establish effectiveness.",
  "steps": [
    {
      "capability_id": "review-rebuttal-framing-and-concern-categories",
      "confidence": "high",
      "depends_on": [],
      "evidence": [
        {
          "justification": "The introduction directly states the audience and the project's framing of rebuttal writing.",
          "kind": "documentation",
          "locator": "Opening subtitle, 'Good rebuttal = Respect + Evidence + Clarity', and 项目动机",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The tip summary directly states this strategy.",
          "kind": "documentation",
          "locator": "写作澄清、相关工作与沟通策略类 > Tip 12 summary",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The disclaimer directly states these applicability restrictions and the content's reported origins.",
          "kind": "documentation",
          "locator": "项目动机 > ⚠️ 免责声明 > first and second paragraphs",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The disclaimer identifies variable conference conditions and explicitly defers to official conference instructions.",
          "kind": "documentation",
          "locator": "项目动机 > ⚠️ 免责声明 > first paragraph",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The table explicitly associates the three topic categories with these tip ranges.",
          "kind": "documentation",
          "locator": "📚 Rebuttal Tips introductory category table",
          "path": "README.md",
          "support_type": "explicit"
        }
      ],
      "id": "review-framing",
      "instruction": "Using the user-supplied reviewer concerns and rebuttal draft for AI or large-model research, identify relevant documented topic groups and provide qualitative feedback on respect, evidence, clarity, and the title-level preference for direct action over promises alone. Identify decisions about word limits, new experiments, external links, and other rebuttal rules that depend on official conference instructions. Use those instructions only if supplied by the user; otherwise leave conference-specific permissions unresolved. Keep feedback within the stated framing, category information, and available title-level strategy without reconstructing omitted image contents or claiming the advice is effective.",
      "limitations": [
        "No particular conference's official rules are supplied.",
        "Only the title is available; the detailed strategy, examples, and qualifications in the referenced image are uninspected.",
        "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
        "The README's conference-rule and applicability caveats still apply.",
        "The category table and tip titles are inspected; the embedded tip image contents are not supplied.",
        "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
        "This describes the guide's stated approach, not demonstrated effectiveness or permission to add experiments at any particular conference."
      ],
      "title": "Review framing and categorize concerns",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Review a rebuttal draft against supplied reviewer concerns"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "high",
    "evidence": [
      {
        "justification": "The introduction directly states the audience and the project's framing of rebuttal writing.",
        "kind": "documentation",
        "locator": "Opening subtitle, 'Good rebuttal = Respect + Evidence + Clarity', and 项目动机",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The tip summary directly states this strategy.",
        "kind": "documentation",
        "locator": "写作澄清、相关工作与沟通策略类 > Tip 12 summary",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The disclaimer directly states these applicability restrictions and the content's reported origins.",
        "kind": "documentation",
        "locator": "项目动机 > ⚠️ 免责声明 > first and second paragraphs",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The disclaimer identifies variable conference conditions and explicitly defers to official conference instructions.",
        "kind": "documentation",
        "locator": "项目动机 > ⚠️ 免责声明 > first paragraph",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The table explicitly associates the three topic categories with these tip ranges.",
        "kind": "documentation",
        "locator": "📚 Rebuttal Tips introductory category table",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "review-rebuttal-framing-and-concern-categories",
    "knowledge_ids": [
      "decision-rule-conference-instructions",
      "fact-action-over-promises-tip",
      "fact-rebuttal-guide-scope",
      "fact-tip-topic-grouping",
      "limitation-advice-applicability"
    ],
    "limitations": [
      "No particular conference's official rules are supplied.",
      "Only the title is available; the detailed strategy, examples, and qualifications in the referenced image are uninspected.",
      "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
      "The README's conference-rule and applicability caveats still apply.",
      "The category table and tip titles are inspected; the embedded tip image contents are not supplied.",
      "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
      "This describes the guide's stated approach, not demonstrated effectiveness or permission to add experiments at any particular conference."
    ],
    "scope": "Applies to conference rebuttal writing for artificial intelligence and large-model research. The result is an agent's review using the guide's stated framing, three topic categories, and Tip 12's title-level strategy. It does not provide the omitted tips' detailed responses, establish effectiveness, or determine conference-specific permissions without supplied official instructions.",
    "task": "Given user-supplied reviewer concerns and a rebuttal draft, identify relevant documented topic groups and provide qualitative feedback on respect, evidence, clarity, and the title-level preference for direct action over promises alone. Identify decisions about word limits, new experiments, external links, and other rebuttal rules that require the conference's official instructions; use those instructions only if supplied by the user.",
    "title": "Review rebuttal framing and identify relevant concern categories"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "When determining rebuttal rules, word limits, whether new experiments are permitted, or whether external links are allowed, the README directs readers to the conference's official instructions because these conditions can differ across conferences.",
    "evidence": [
      {
        "justification": "The disclaimer identifies variable conference conditions and explicitly defers to official conference instructions.",
        "kind": "documentation",
        "locator": "项目动机 > ⚠️ 免责声明 > first paragraph",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "decision-rule-conference-instructions",
    "limitations": [
      "No particular conference's official rules are supplied."
    ],
    "title": "Use conference rules to determine permitted rebuttal content",
    "type": "DECISION_RULE"
  },
  {
    "confidence": "high",
    "content": "The title of Tip 12 presents a general rebuttal strategy of trying to act directly rather than only making promises.",
    "evidence": [
      {
        "justification": "The tip summary directly states this strategy.",
        "kind": "documentation",
        "locator": "写作澄清、相关工作与沟通策略类 > Tip 12 summary",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "fact-action-over-promises-tip",
    "limitations": [
      "Only the title is available; the detailed strategy, examples, and qualifications in the referenced image are uninspected.",
      "The README's conference-rule and applicability caveats still apply."
    ],
    "title": "Tip 12 favors action over promises alone",
    "type": "FACT"
  },
  {
    "confidence": "high",
    "content": "The README presents the project as a conference rebuttal writing guide for artificial intelligence and large-model research. It frames rebuttals around respect, evidence, and clarity, with the aim of reorganizing evidence, clarifying misunderstandings, and supplementing experiments within limited space.",
    "evidence": [
      {
        "justification": "The introduction directly states the audience and the project's framing of rebuttal writing.",
        "kind": "documentation",
        "locator": "Opening subtitle, 'Good rebuttal = Respect + Evidence + Clarity', and 项目动机",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "fact-rebuttal-guide-scope",
    "limitations": [
      "This describes the guide's stated approach, not demonstrated effectiveness or permission to add experiments at any particular conference."
    ],
    "title": "Guide scope and framing",
    "type": "FACT"
  },
  {
    "confidence": "high",
    "content": "The README groups Tips 1–7 under novelty, motivation, theory, and boundaries; Tips 8–12 under writing clarification, related work, and communication; and Tips 13–28 under experiments and evaluation evidence.",
    "evidence": [
      {
        "justification": "The table explicitly associates the three topic categories with these tip ranges.",
        "kind": "documentation",
        "locator": "📚 Rebuttal Tips introductory category table",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "fact-tip-topic-grouping",
    "limitations": [
      "The category table and tip titles are inspected; the embedded tip image contents are not supplied."
    ],
    "title": "Three topic groups organize the tips",
    "type": "FACT"
  },
  {
    "confidence": "high",
    "content": "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
    "evidence": [
      {
        "justification": "The disclaimer directly states these applicability restrictions and the content's reported origins.",
        "kind": "documentation",
        "locator": "项目动机 > ⚠️ 免责声明 > first and second paragraphs",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "limitation-advice-applicability",
    "limitations": [
      "The supplied text does not independently validate the advice or trace individual tips to their original sources."
    ],
    "title": "Advice carries no correctness or universal applicability guarantee",
    "type": "LIMITATION"
  }
]
```

