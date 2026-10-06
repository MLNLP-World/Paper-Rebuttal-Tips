# Router (compiler-authored orchestration)

Compiler-authored orchestration by the repo2skill compiler. The source repository supplies the rebuttal strategies and contribution tips; the routing rules, intent classes, topic tags, and route table are navigation metadata authored by the compiler from the accepted workflow and capability task semantics — not behavior described in the source repository and not author domain knowledge. No numeric scores, priority algorithms, or confidence thresholds are used. Each route's Reference points at that workflow's validated record, which carries its full scope, steps, and limitations.

## Pipeline

user intent -&gt; reviewer point -&gt; topic relevance -&gt; applicability -&gt; user evidence / results / plan availability -&gt; select zero, one, or multiple workflows from the route table below -&gt; execute the selected workflow\(s\) -&gt; aggregate per-point results

## Intent classes

- reviewer-comment-analysis — Analyze the reviewer comments: split into reviewer points, classify topics, judge applicability, and list candidate workflows and missing evidence; no drafting.
- existing-reply-review — Review a user-supplied existing rebuttal draft against the documented pitfalls.
- drafting — Draft rebuttal reply text, only on the user's explicit drafting request.
- tip-organization — Organize a user-supplied tip contribution into the documented four-part card structure.

## Execution rules

- Analysis only: Split, classify, judge applicability, and list candidate workflows and missing evidence; do not draft replies, do not claim a review of a draft that was not supplied, and do not execute draft workflows without a drafting request.
- Existing-reply review: Only claim a reply was reviewed when the user actually supplied it; use wf-review-supplied-reply-for-documented-pitfalls; may point out which drafting workflows could improve the reply, but must not rewrite the reply automatically.
- Drafting: Execute draft workflows only when the user explicitly asks to draft a reply.
- Tip organization: A tip contribution request enters wf-organize-tip-card-contribution directly; do not route it through rebuttal topic selection first.
- Partial failure: Missing material marks that reviewer point's missing evidence and limits only that point's workflow\(s\); other independent points continue; one missing experiment never stops the whole request.

## Output protocol

Per reviewer point: reviewer point; existing reply or not supplied; selected Workflow\(s\); applicability reason; concrete analysis / feedback; requested draft \(only when the user asked to draft\); missing evidence; unresolved items

## Route table

### 1. wf-analyze-reviewer-comments

- Intent class: reviewer-comment-analysis
- Role: analysis
- Topic tags: vague points, low-quality points, unlocatable points
- Trigger description: at least one reviewer point is itself vague, low-quality, or its concrete concern cannot be located
- Applicability conditions: Applies only when reviewer comments contain points that are themselves vague, low-quality, or whose concrete concern cannot be located; when a group of comments mixes such points with clearly locatable points, this workflow processes only the vague or unlocatable ones.
- Linked capabilities: draft-vague-review-response
- Local limitations: Processes only the vague or unlocatable points through draft-vague-review-response; clearly locatable points are left to the Router's domain-workflow selection; never claims a general all-comment analysis.
- Reference: [workflow 1](workflow-001.md)

### 2. wf-draft-ablation-evidence-reply

- Intent class: drafting
- Role: draft
- Topic tags: ablation evidence
- Trigger description: the reviewer comment requests ablation evidence
- Applicability conditions: Applies when a reviewer requests ablation evidence.
- Linked capabilities: draft-ablation-evidence-response
- Local limitations: Requires the user's actual modules and measured values; M1/M2/M3 and XXX are example placeholders, never substituted for the user's facts.
- Reference: [workflow 2](workflow-002.md)

### 3. wf-draft-baseline-coverage-response

- Intent class: drafting
- Role: draft
- Topic tags: baseline coverage
- Trigger description: the reviewer point questions baseline coverage
- Applicability conditions: Applies when a reviewer questions baseline coverage.
- Linked capabilities: draft-baseline-coverage-response
- Local limitations: The fallback branch does not promise an actual full additional comparison when it cannot be completed in the rebuttal period; needs the user's real baseline details.
- Reference: [workflow 3](workflow-003.md)

### 4. wf-draft-concrete-revision-plan

- Intent class: drafting
- Role: draft
- Topic tags: unclear writing, revision plan
- Trigger description: the critique targets unclear writing or presentation
- Applicability conditions: Applies when the critique targets unclear writing or presentation.
- Linked capabilities: draft-concrete-revision-plan
- Local limitations: Section and symbol names are filled from the user's paper; the plan is a commitment, not a completed revision.
- Reference: [workflow 4](workflow-004.md)

### 5. wf-draft-contribution-focus-response

- Intent class: drafting
- Role: draft
- Topic tags: unclear contribution
- Trigger description: the critique says the contribution statement is unclear or concrete contributions are hard to identify
- Applicability conditions: Applies when the reviewer's critique is that the contribution statement is unclear or that concrete contributions are hard to identify, not when the author merely claims the contributions were already listed.
- Linked capabilities: draft-contribution-focus-response
- Local limitations: Needs the user's actual contribution structure; not a general writing-advice workflow.
- Reference: [workflow 5](workflow-005.md)

### 6. wf-draft-data-scale-response

- Intent class: drafting
- Role: draft
- Topic tags: data scale
- Trigger description: dataset size or scale is the reviewer point's concern
- Applicability conditions: Applies when dataset size or scale is the reviewer's concern.
- Linked capabilities: draft-data-scale-response
- Local limitations: Dataset names and scenario coverage come from the user's real data; example names are placeholders.
- Reference: [workflow 6](workflow-006.md)

### 7. wf-draft-design-necessity-and-hyperparameter-response

- Intent class: drafting
- Role: draft
- Topic tags: design necessity, hyperparameter sensitivity
- Trigger description: the point concerns method complexity or hyperparameter sensitivity \(the two cited card scenarios\)
- Applicability conditions: Applies to the two cited card scenarios \(method complexity and hyperparameter sensitivity\); each scenario keeps its own recommended strategy and must not be substituted by the ablation task.
- Linked capabilities: draft-design-necessity-and-hyperparameter-response
- Local limitations: Each of the two cited scenarios keeps its own recommended strategy; they must not be conflated.
- Reference: [workflow 7](workflow-007.md)

### 8. wf-draft-fairness-details-response

- Intent class: drafting
- Role: draft
- Topic tags: comparison fairness
- Trigger description: the fairness of the comparison is questioned
- Applicability conditions: Applies when the fairness of the comparison is questioned.
- Linked capabilities: draft-fairness-details-response
- Local limitations: The configuration table \(identical settings, per-method defaults, extra settings\) must be filled with the user's actual comparison configuration.
- Reference: [workflow 8](workflow-008.md)

### 9. wf-draft-generalization-response

- Intent class: drafting
- Role: draft
- Topic tags: generalization
- Trigger description: generalization is the reviewer point's concern
- Applicability conditions: Applies when generalization is the reviewer's concern.
- Linked capabilities: draft-generalization-response
- Local limitations: Current coverage supports only preliminary validation and must not be reported as a verified generalization result.
- Reference: [workflow 9](workflow-009.md)

### 10. wf-draft-infeasible-experiment-response

- Intent class: drafting
- Role: draft
- Topic tags: infeasible experiment
- Trigger description: the requested experiment is infeasible within the rebuttal period
- Applicability conditions: Applies when the requested experiment is infeasible within the rebuttal period.
- Linked capabilities: draft-infeasible-experiment-response
- Local limitations: A small-scale result is a preliminary reference point, not a claim that the requested experiment was completed.
- Reference: [workflow 10](workflow-010.md)

### 11. wf-draft-intermediate-quality-response

- Intent class: drafting
- Role: draft
- Topic tags: intermediate output quality
- Trigger description: the quality of intermediate outputs is the reviewer point's concern
- Applicability conditions: Applies when the quality of intermediate outputs is the reviewer's concern.
- Linked capabilities: draft-intermediate-quality-response
- Local limitations: GPT-4 and Gemini-Pro are the source card's named example judges, not prescribed tools; the user's actual evaluation setup decides.
- Reference: [workflow 11](workflow-011.md)

### 12. wf-draft-leakage-check-response

- Intent class: drafting
- Role: draft
- Topic tags: data leakage
- Trigger description: data leakage is the reviewer point's concern
- Applicability conditions: Applies when data leakage is the reviewer's concern.
- Linked capabilities: draft-leakage-check-response
- Local limitations: The card gives no concrete deduplication algorithm; the check description must come from the user's actual pipeline.
- Reference: [workflow 12](workflow-012.md)

### 13. wf-draft-limitations-response

- Intent class: drafting
- Role: draft
- Topic tags: limitations discussion
- Trigger description: the reviewer asks for limitations or a weakness discussion
- Applicability conditions: Applies when a reviewer asks for limitations or a weakness discussion.
- Linked capabilities: draft-limitations-response
- Local limitations: The named limitations are the card's examples and do not apply to every method; use the user's real limitations.
- Reference: [workflow 13](workflow-013.md)

### 14. wf-draft-longitudinal-evidence-response

- Intent class: drafting
- Role: draft
- Topic tags: dynamic capability, longitudinal evidence
- Trigger description: dynamic capability is the reviewer point's concern
- Applicability conditions: Applies when dynamic capability is the reviewer's concern.
- Linked capabilities: draft-longitudinal-evidence-response
- Local limitations: Offline longitudinal zero-shot runs apply only when the user's offline setup matches the card's framing; the 100-task stream and every-20-task evaluation are example settings, not recommended values.
- Reference: [workflow 14](workflow-014.md)

### 15. wf-draft-mechanism-and-theory-response

- Intent class: drafting
- Role: draft
- Topic tags: theory, mechanism
- Trigger description: the reviewer asks for theory or mechanism justification
- Applicability conditions: Applies when a reviewer asks for theory or mechanism justification.
- Linked capabilities: draft-mechanism-and-theory-response
- Local limitations: The intuition chain and analytic statement are filled from the user's own method analysis, not invented theory.
- Reference: [workflow 15](workflow-015.md)

### 16. wf-draft-metric-response

- Intent class: drafting
- Role: draft
- Topic tags: metric choice
- Trigger description: the metric choice is the reviewer point's concern
- Applicability conditions: Applies when the metric choice is the reviewer's concern.
- Linked capabilities: draft-metric-response
- Local limitations: Baseline names and metric tokens are placeholders; the added-metric advantage is example text until the user supplies their results.
- Reference: [workflow 16](workflow-016.md)

### 17. wf-draft-missing-experiment-response

- Intent class: drafting
- Role: draft
- Topic tags: missing experiment
- Trigger description: the reviewer asks for an experiment or analysis not yet present
- Applicability conditions: Applies when a reviewer asks for an experiment or analysis not yet present.
- Linked capabilities: draft-missing-experiment-response
- Local limitations: Giving new results is conditioned on time allowing; the sample answer's elements are the card's examples, not the user's results; missing material limits only this point.
- Reference: [workflow 17](workflow-017.md)

### 18. wf-draft-misunderstanding-correction

- Intent class: drafting
- Role: draft
- Topic tags: misunderstanding
- Trigger description: the user judges that the criticism rests on a misunderstanding of the method
- Applicability conditions: Applies only when the user judges that the criticism rests on a misunderstanding of the method; requires the user to supply the actual method flow and its dependencies.
- Linked capabilities: draft-misunderstanding-correction
- Local limitations: Applies only on the user's own judgment of a misunderstanding; requires the user's actual method flow and dependencies; any no-risk conclusion stays within the cited bounds.
- Reference: [workflow 18](workflow-018.md)

### 19. wf-draft-motivation-response

- Intent class: drafting
- Role: draft
- Topic tags: motivation
- Trigger description: the reviewer questions whether the problem is worth solving
- Applicability conditions: Applies when a reviewer questions whether the problem is worth solving.
- Linked capabilities: draft-motivation-response
- Local limitations: Scenario, consequence, and cost must come from the user's real application.
- Reference: [workflow 19](workflow-019.md)

### 20. wf-draft-novelty-and-related-work-response

- Intent class: drafting
- Role: draft
- Topic tags: novelty, related work
- Trigger description: the reviewer questions novelty or the relation to prior work
- Applicability conditions: Applies when a reviewer questions novelty or the relation to prior work.
- Linked capabilities: draft-novelty-and-related-work-response
- Local limitations: Core innovation, synergy mechanism, and module roles are filled from the user's paper; the workflow does not verify novelty itself.
- Reference: [workflow 20](workflow-020.md)

### 21. wf-draft-overhead-response

- Intent class: drafting
- Role: draft
- Topic tags: computational overhead
- Trigger description: overhead or cost is the reviewer point's concern
- Applicability conditions: Applies when overhead or cost is the reviewer's concern.
- Linked capabilities: draft-overhead-response
- Local limitations: Cost source, complexity, and percentages are filled from the user's own measurements; the card's example numbers are placeholders.
- Reference: [workflow 21](workflow-021.md)

### 22. wf-draft-reply-for-vague-review

- Intent class: drafting
- Role: draft
- Topic tags: vague review
- Trigger description: the review's concerns are partly or wholly too general to locate
- Applicability conditions: Applies to reviews whose concerns are partly or wholly too general to locate; the AC escalation is conditional, not required in every case.
- Linked capabilities: draft-vague-review-response
- Local limitations: AC escalation is conditional, not required in every case; requires the user's review text.
- Reference: [workflow 22](workflow-022.md)

### 23. wf-draft-reproducibility-response

- Intent class: drafting
- Role: draft
- Topic tags: reproducibility
- Trigger description: reproducibility is the reviewer point's concern
- Applicability conditions: Applies when reproducibility is the reviewer's concern.
- Linked capabilities: draft-reproducibility-response
- Local limitations: The anonymous repository and detailed settings are example states in the card; no actual URL or settings are fabricated — only the user's real release state is used.
- Reference: [workflow 23](workflow-023.md)

### 24. wf-draft-small-gain-response

- Intent class: drafting
- Role: draft
- Topic tags: small improvement
- Trigger description: the improvement size is the reviewer point's concern
- Applicability conditions: Applies when the improvement size is the reviewer's concern.
- Linked capabilities: draft-small-gain-response
- Local limitations: Statistical significance and variance results are revision commitments, not inferred results; the card supplies no concrete gain, variance, or significance numbers to quote as the user's.
- Reference: [workflow 24](workflow-024.md)

### 25. wf-organize-tip-card-contribution

- Intent class: tip-organization
- Role: tip
- Topic tags: tip contribution
- Trigger description: the user supplies tip material to organize into the documented card structure
- Applicability conditions: Applies to organizing tip material for contribution, not to drafting replies to a user's reviewers.
- Linked capabilities: organize-tip-card-contribution
- Local limitations: Four-part card organization only; not a rebuttal strategy; the contribution path is limited to the text template and submission channel \(Issue or PR\) — no automatic submission.
- Reference: [workflow 25](workflow-025.md)

### 26. wf-review-supplied-reply-for-documented-pitfalls

- Intent class: existing-reply-review
- Role: review
- Topic tags: supplied draft review
- Trigger description: the user supplies a rebuttal draft and reviewer concerns for review
- Applicability conditions: Applies to drafts the user supplies for assessment.
- Linked capabilities: assess-supplied-response-for-documented-pitfalls
- Local limitations: Reports gaps only; does not automatically rewrite the reply; the pitfall synthesis is scoped to the cited negative answers.
- Reference: [workflow 26](workflow-026.md)

