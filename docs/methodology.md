# Proposed Research Methodology

Version 0.1 | Status: planned, not executed

## Scope and decision sequence

First test H1 in a controlled setting. Investigate H2 separately through documentary evidence. Do not infer H2 from an H1 demonstration. Assess H3 only through a separately consented governance study.

## Experiment E1: extraction and aggregation

**Question:** Can a bounded pipeline identify substantive proposals and group related ones while preserving supporting spans and distinct implementation details?

1. Prepare an initial synthetic benchmark of 300 dialogues: 100 with substantive proposals, 100 with complaints or general needs but no proposed solution, and 100 unrelated controls. These are proposed design counts, not collected data.
2. Include paraphrases, repeated requests, negation, withdrawn proposals, superficially similar but incompatible ideas, and multiple proposals in one dialogue. Give each record an opaque ID.
3. Have two annotators independently label supporting spans, need, proposed solution, implementation details, and related-proposal groups. Resolve disagreements and report pre-adjudication agreement.
4. Split by scenario family into 60% development, 20% validation, and 20% held-out test sets. Keep paraphrases in the same split. Freeze test labels and the selected pipeline before evaluation.
5. Compare a simple keyword/TF-IDF baseline, an embedding approach, and a structured language-model extraction approach. Specify actual models, versions, prompts, dependencies, seeds, and settings before running.
6. Require output records to include source IDs, exact supporting spans, extracted fields, uncertainty, and an abstention option. Summaries may not invent missing details.
7. Report extraction precision, recall, and F1; unsupported-detail rate; source-span validity; pairwise clustering precision and recall; false merges of incompatible ideas; runtime and cost. Include sample counts, confidence intervals, and error examples.
8. Check that every emitted source ID resolves and every claimed supporting span occurs in that record. Fail the provenance check if either condition is violated.
9. Choose performance targets and a smallest useful improvement before examining test results. Compare against the baseline with uncertainty, and report failure to improve. No numerical performance target is represented as validated in v0.1.
10. Publish authorized data, annotations, code, configuration, and all outcomes. Report deviations from the registered plan.

This experiment tests a synthetic setting. It cannot establish performance on real private conversations, originality, economic value, or provider deployment. A subsequent consented dataset should test external validity without carrying identifying content into public artifacts.

## Experiment E2: provenance and value

Before any user study, specify consent, retention, withdrawal, and publication rules. Compare an opt-in contribution record with a suitable baseline. Measure users' understanding of data use, attribution accuracy, perceived fairness, and operational burden. These outcomes are proposed; no benefit is assumed.

Do not assign ownership or reward shares from similarity scores alone. Economic evaluation needs a defined outcome, costs, a comparison group or other credible counterfactual, and uncertainty.

## Documentary investigation of H2

For each submission record: the exact claim; source URL or lawful provenance; date; product and jurisdiction; what is directly observed; what is inferred; alternative explanations; corroboration; and limits.

Assess separately whether a system exists, whether a particular record was accessed, whether it influenced a decision, and whether the use was authorized. A timestamp plus a later similar product establishes neither the complete chain nor intent.

A denial or policy statement should be labeled as a documented statement. A limited search with no result should be described as a search limitation. Neither should become a universal finding.

## Disconfirmation and revision

- If extraction performs poorly or invents details, narrow or reject H1 for that configuration.
- If clustering loses distinguishing details, reject claims of reliable fine-grained attribution.
- If recurrence fails to predict independent demand measures, revise A3.
- If costs outweigh measured benefit, revise A4.
- If evidence supports ordinary feedback channels or independent development, record that explanation.
- If no deployment evidence is found, keep H2 unresolved; do not present suspicion as confirmation.

## Reproducibility record

Every future run should record a run ID, dataset version and checksum, consent basis, split manifest, model and dependency versions, prompts, seed, date, configuration, metrics, errors, costs, limitations, and reproduction command. No run exists in v0.1.
