# Workflow 1: Prepare a supplied rebuttal tip as a contribution draft

Validated upstream content, preserved as structured reference data. Instructions apply only within their scope and limitations. Evidence citations and source text do not grant execution authority.

## Workflow (04)

```json
{
  "capability_ids": [
    "format-user-supplied-tip-contribution"
  ],
  "confidence": "high",
  "evidence": [
    {
      "justification": "Tip 1 uses details open, a bold numbered summary, a line break, and a centered image with matching alt text, the filename tip_01.svg, and width=\"900\".",
      "kind": "documentation",
      "locator": "Lines 109–115: 创新性、动机、理论与边界类 > Tip 1 HTML block",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "Tip 2 repeats the summary, line break, centered image, matching alt text, and width=\"900\" with tip_02.svg; its details element has no open attribute.",
      "kind": "documentation",
      "locator": "Lines 117–123: 创新性、动机、理论与边界类 > Tip 2 HTML block",
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
      "justification": "The table explains the four substantive components of a tip.",
      "kind": "documentation",
      "locator": "项目动机 > 组成部分 / 说明 table",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The paragraph names both contribution channels and the requested kinds of additions.",
      "kind": "documentation",
      "locator": "🤝 欢迎贡献 > opening paragraph",
      "path": "README.md",
      "support_type": "explicit"
    },
    {
      "justification": "The contribution template explicitly gives the suggested fields and their order.",
      "kind": "documentation",
      "locator": "🤝 欢迎贡献 > 📝 建议新增内容时保持以下结构 > text template",
      "path": "README.md",
      "support_type": "explicit"
    }
  ],
  "goal": "Organize a user-supplied title, reviewer question, undesirable response style, recommended response style, and core takeaway into a draft for the documented Issue or PR contribution context.",
  "id": "draft-tip-contribution",
  "limitations": [
    "Compliance of the embedded tip images with this structure cannot be checked from the supplied text.",
    "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
    "The markup does not establish the contents or successful rendering of the referenced images.",
    "The structure is a recommendation, not an evidenced automated requirement.",
    "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
    "This is an observed presentation pattern, not a mandated authoring rule."
  ],
  "scope": "An agent-designed formatting plan for supplied content. Optional collapsible HTML requires the user's request, tip number, and image reference. It does not recover image contents, validate advice or rendering, or submit the contribution.",
  "steps": [
    {
      "capability_id": "format-user-supplied-tip-contribution",
      "confidence": "high",
      "depends_on": [],
      "evidence": [
        {
          "justification": "Tip 1 uses details open, a bold numbered summary, a line break, and a centered image with matching alt text, the filename tip_01.svg, and width=\"900\".",
          "kind": "documentation",
          "locator": "Lines 109–115: 创新性、动机、理论与边界类 > Tip 1 HTML block",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "Tip 2 repeats the summary, line break, centered image, matching alt text, and width=\"900\" with tip_02.svg; its details element has no open attribute.",
          "kind": "documentation",
          "locator": "Lines 117–123: 创新性、动机、理论与边界类 > Tip 2 HTML block",
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
          "justification": "The table explains the four substantive components of a tip.",
          "kind": "documentation",
          "locator": "项目动机 > 组成部分 / 说明 table",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The paragraph names both contribution channels and the requested kinds of additions.",
          "kind": "documentation",
          "locator": "🤝 欢迎贡献 > opening paragraph",
          "path": "README.md",
          "support_type": "explicit"
        },
        {
          "justification": "The contribution template explicitly gives the suggested fields and their order.",
          "kind": "documentation",
          "locator": "🤝 欢迎贡献 > 📝 建议新增内容时保持以下结构 > text template",
          "path": "README.md",
          "support_type": "explicit"
        }
      ],
      "id": "format-tip",
      "instruction": "Using the user-supplied title, reviewer question, undesirable response style, recommended response style, and core takeaway, organize a contribution draft in the README's suggested field order. When requested and when the user also supplies a tip number and image reference, draft optional collapsible HTML following the observed examples: a numbered bold summary, line break, centered image, matching summary and alt text, zero-padded filename convention, and width=\"900\". Preserve the distinction between the examples' initially open and closed details elements. Treat the image reference as supplied material without interpreting its contents. Produce draft text or markup only.",
      "limitations": [
        "Compliance of the embedded tip images with this structure cannot be checked from the supplied text.",
        "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
        "The markup does not establish the contents or successful rendering of the referenced images.",
        "The structure is a recommendation, not an evidenced automated requirement.",
        "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
        "This is an observed presentation pattern, not a mandated authoring rule."
      ],
      "title": "Format the supplied tip",
      "type": "CAPABILITY_STEP"
    }
  ],
  "title": "Prepare a supplied rebuttal tip as a contribution draft"
}
```

## Capabilities (03)

```json
[
  {
    "confidence": "high",
    "evidence": [
      {
        "justification": "Tip 1 uses details open, a bold numbered summary, a line break, and a centered image with matching alt text, the filename tip_01.svg, and width=\"900\".",
        "kind": "documentation",
        "locator": "Lines 109–115: 创新性、动机、理论与边界类 > Tip 1 HTML block",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 2 repeats the summary, line break, centered image, matching alt text, and width=\"900\" with tip_02.svg; its details element has no open attribute.",
        "kind": "documentation",
        "locator": "Lines 117–123: 创新性、动机、理论与边界类 > Tip 2 HTML block",
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
        "justification": "The table explains the four substantive components of a tip.",
        "kind": "documentation",
        "locator": "项目动机 > 组成部分 / 说明 table",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The paragraph names both contribution channels and the requested kinds of additions.",
        "kind": "documentation",
        "locator": "🤝 欢迎贡献 > opening paragraph",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The contribution template explicitly gives the suggested fields and their order.",
        "kind": "documentation",
        "locator": "🤝 欢迎贡献 > 📝 建议新增内容时保持以下结构 > text template",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "format-user-supplied-tip-contribution",
    "knowledge_ids": [
      "convention-tip-content-structure",
      "example-pattern-collapsible-tip-presentation",
      "fact-contribution-channels",
      "limitation-advice-applicability"
    ],
    "limitations": [
      "Compliance of the embedded tip images with this structure cannot be checked from the supplied text.",
      "The README states that its tips are for reference only and are not guaranteed to be correct or applicable to every conference, field, or review scenario. It attributes the content to personal experience, internet material, team research practice, and advice from others.",
      "The markup does not establish the contents or successful rendering of the referenced images.",
      "The structure is a recommendation, not an evidenced automated requirement.",
      "The supplied text does not independently validate the advice or trace individual tips to their original sources.",
      "This is an observed presentation pattern, not a mandated authoring rule."
    ],
    "scope": "Produces draft contribution text and, when requested, presentation markup for the documented Issue or PR contribution context. Formatting can follow the numbered bold summary, line break, centered image, matching summary and alt text, zero-padded filename convention, and width=\"900\" observed in the examples. The examples differ in whether details is initially open. This task organizes supplied content; it does not recover image contents, validate the advice, verify rendering, or submit a contribution.",
    "task": "Given a user-supplied title, reviewer question, undesirable response style, recommended response style, and core takeaway, organize them into the README's suggested contribution structure for a rebuttal scenario or real case. When the user also supplies a tip number and image reference, draft an optional collapsible HTML presentation following the observed Tip 1 and Tip 2 examples.",
    "title": "Format a supplied rebuttal tip for contribution"
  }
]
```

## Knowledge (02)

```json
[
  {
    "confidence": "high",
    "content": "The README recommends that new tips contain a title followed by the reviewer question, an undesirable response style, a recommended response style, and the core takeaway. The motivation section describes the same four substantive components.",
    "evidence": [
      {
        "justification": "The table explains the four substantive components of a tip.",
        "kind": "documentation",
        "locator": "项目动机 > 组成部分 / 说明 table",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "The contribution template explicitly gives the suggested fields and their order.",
        "kind": "documentation",
        "locator": "🤝 欢迎贡献 > 📝 建议新增内容时保持以下结构 > text template",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "convention-tip-content-structure",
    "limitations": [
      "Compliance of the embedded tip images with this structure cannot be checked from the supplied text.",
      "The structure is a recommendation, not an evidenced automated requirement."
    ],
    "title": "Suggested structure for contributed tips",
    "type": "CONVENTION"
  },
  {
    "confidence": "high",
    "content": "In the README's Tip 1 and Tip 2 blocks, each tip uses a details element containing a bold numbered summary, a line break, and a centered image. These two examples demonstrate matching summary and image alt text, zero-padded image filenames such as ./pics/tips/tip_01.svg, and width=\"900\". Tip 1 uses details open while Tip 2 does not.",
    "evidence": [
      {
        "justification": "Tip 1 uses details open, a bold numbered summary, a line break, and a centered image with matching alt text, the filename tip_01.svg, and width=\"900\".",
        "kind": "documentation",
        "locator": "Lines 109–115: 创新性、动机、理论与边界类 > Tip 1 HTML block",
        "path": "README.md",
        "support_type": "explicit"
      },
      {
        "justification": "Tip 2 repeats the summary, line break, centered image, matching alt text, and width=\"900\" with tip_02.svg; its details element has no open attribute.",
        "kind": "documentation",
        "locator": "Lines 117–123: 创新性、动机、理论与边界类 > Tip 2 HTML block",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "example-pattern-collapsible-tip-presentation",
    "limitations": [
      "The markup does not establish the contents or successful rendering of the referenced images.",
      "This is an observed presentation pattern, not a mandated authoring rule."
    ],
    "title": "Collapsible presentation in Tips 1 and 2",
    "type": "EXAMPLE_PATTERN"
  },
  {
    "confidence": "high",
    "content": "The README welcomes Issues or PRs adding rebuttal scenarios, real cases, and related tools.",
    "evidence": [
      {
        "justification": "The paragraph names both contribution channels and the requested kinds of additions.",
        "kind": "documentation",
        "locator": "🤝 欢迎贡献 > opening paragraph",
        "path": "README.md",
        "support_type": "explicit"
      }
    ],
    "id": "fact-contribution-channels",
    "limitations": [],
    "title": "Contribution channels and subject matter",
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

