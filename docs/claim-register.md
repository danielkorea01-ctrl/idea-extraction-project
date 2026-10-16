# Claim Register

Version 0.1 | 17 October 2026

## Labels

- **Fact:** A narrowly verifiable statement supported by the cited source or a reproducible observation.
- **Documented claim:** What a source reports; not independently reproduced here.
- **Inference:** Reasoning from stated premises, with alternatives.
- **Hypothesis:** A proposition to evaluate.
- **Unverified assumption:** A premise used in planning that has not been tested.

A source's existence is a fact; the validity and generality of its reported results require separate assessment.

| ID | Statement | Label | Basis / current status | Next evidence needed |
| --- | --- | --- | --- | --- |
| F1 | Sentence-BERT describes semantic sentence embeddings | Fact about a publication | S1, abstract | Review full method before selecting an implementation |
| F2 | BERTopic describes embedding-based document clustering and topic representations | Fact about a publication | S2, abstract | Evaluate on the proposed dataset |
| D1 | GPT-2 training text was recovered in the reported experiments | Documented claim | S3, abstract; not replicated here | Full-method review and authorized replication if relevant |
| I1 | Published text-analysis components justify testing a combined proposal-analysis system | Inference | F1 and F2; integration remains untested | End-to-end benchmark |
| H1 | A pipeline can produce useful, traceable candidate proposals | Hypothesis | No project measurements | Preregistered extraction and clustering evaluation |
| H2 | Conversation-derived ideas inform product decisions at a platform | Hypothesis | No deployment evidence in this release | Authenticated, scoped workflow and decision evidence |
| H3 | Opt-in provenance improves transparency and perceived fairness | Hypothesis | No user study | Consented comparison with explicit outcome measures |
| A1 | Authorized data contains enough substantive proposals | Unverified assumption | No dataset collected | Dataset characterization |
| A2 | Models preserve important distinctions among proposals | Unverified assumption | No evaluation | False-merge and detail-retention analysis |
| A3 | Repeated requests are informative about demand | Unverified assumption | No validated demand measure | Deduplication and comparison against independent measures |
| A4 | Insights produce net commercial value | Unverified assumption | No economic study | Costs, baselines, and counterfactual evaluation |

S1-S3 are defined in [sources.md](sources.md).

## Not established

No provider-specific misconduct, copied invention, revenue attributable to user ideas, or legal liability has been established. No numerical accuracy or prevalence estimate is claimed.

## Revision rule

For every changed claim, retain its ID and record the date, evidence, old label, new label, and reason in the pull request. Mark retracted claims explicitly instead of silently removing them. Record contradictory evidence and scope limits.
