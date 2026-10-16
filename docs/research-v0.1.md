# The Idea Extraction Problem

Version 0.1 | 17 October 2026  
Status: Exploratory research proposal; no experiments completed.

## Idea

**H1 — Technical hypothesis:** A system could identify product proposals in authorized AI conversation data, group related proposals, and preserve their provenance well enough to produce useful candidate product intelligence.

**H2 — Deployment hypothesis:** Some AI platform may use conversation-derived proposals in product decisions beyond responding to the originating user. This release does not establish whether, where, or how that occurs.

**H3 — Governance hypothesis:** Explicit, opt-in provenance and contribution mechanisms could improve transparency and perceived fairness. Their benefits, costs, and privacy consequences require evaluation.

The research question is: if value arises from many users articulating needs and solutions, what evidence can establish their contribution, and which forms of acknowledgment or compensation would be justified?

Here, an **idea** means a stated unmet need, proposed feature, workflow, or technical approach. This operational definition makes no claim of originality or legal protection. **Extraction** means converting such content into structured records; **aggregation** means combining related records; **commercial use** means using the resulting information in a business decision. These steps must be investigated separately.

## Rationale

### Published facts and reported findings

**F1:** Sentence-BERT describes sentence embeddings suitable for semantic comparison [S1]. This is support for one component of a possible system.

**F2:** BERTopic describes document embeddings, clustering, and topic representation [S2]. Topic discovery is not the same as identifying an original invention.

**D1:** Carlini and colleagues report recovering training text from GPT-2 [S3]. This is a reported result about memorization and training-data extraction, not evidence of a product team mining private conversations for ideas.

These sources were inspected at the abstract and bibliographic-record level for this release. Their experiments have not been independently reproduced by this project. See [source scope](sources.md).

### Proposed mechanism — an inference, not an observed workflow

A candidate pipeline would accept authorized records, identify candidate needs and proposals, retain supporting text spans, group related records, and present summaries for human review. Each summary would retain links to its inputs and uncertainty labels.

The inference is that combining known text-processing components warrants an experiment. It does not establish adequate accuracy, commercial utility, or deployment.

### Unverified assumptions

**A1:** A consented dataset would contain enough substantive proposals to make aggregation useful.

**A2:** The selected models would preserve important implementation differences instead of collapsing distinct proposals into generic topics.

**A3:** Recurrence in conversations would provide useful demand information. Conversation frequency may instead reflect repeated users, bots, selection effects, or transient interest.

**A4:** Organizations would find the output economically useful. No cost-benefit measurement or willingness-to-pay study has been performed here.

None of these assumptions is a finding.

### Mechanisms that must remain distinct

| Mechanism | Research distinction |
| --- | --- |
| Model training | Updating model parameters from data |
| Inference and retention | Processing a request or storing records; neither alone establishes later product use |
| Feedback analytics | Summarizing reactions, errors, or needs |
| Proposal extraction | Producing structured candidate ideas from text |
| Product decision use | A documented connection between information and a business decision |
| Unauthorized appropriation | A separate allegation requiring evidence and context-specific legal analysis |

This release makes no assessment of current provider policies or legal entitlement. Ownership, consent, processing permission, and rights to compensation are separate questions for later jurisdiction-specific research.

## Evidence Gap

The project has no authenticated internal workflow records, access logs, product-decision records, or independently corroborated case establishing the proposed covert mechanism at OpenAI or another named provider. It has no completed benchmark and no demonstrated commercial value.

A dated conversation can support chronology if its provenance is reliable. It does not alone establish originality, access by decision-makers, causal influence, copying, or entitlement. An output resembling a user's proposal may reflect common requirements, public sources, independent development, ordinary feedback channels, or chance resemblance.

Evidence should be accumulated for each link:

| Question | Potentially useful evidence | What it would still not establish |
| --- | --- | --- |
| Can the pipeline work? | Reproducible evaluation on authorized data | Deployment by a provider |
| Is a process deployed? | Authenticated documentation with relevant scope and dates | Use of a particular user's proposal |
| Did a proposal reach a decision? | Corroborated provenance and decision records | Unauthorized use or financial harm |
| Was use permitted? | Applicable agreements, settings, facts, and qualified legal analysis | A universal answer across products or jurisdictions |
| Did contributors create measurable value? | A credible comparison with a baseline or counterfactual | An automatic compensation formula |

A provider policy would document what a provider states, not independently verify implementation. Silence in a policy would not prove covert activity. Absence of evidence in this limited review would not prove that a mechanism never exists.

## Conclusion

**Supported:** Relevant text-analysis methods have been published.

**Inferred:** A bounded, consent-based feasibility experiment is a reasonable next step.

**Unresolved:** End-to-end reliability, practical value, provider deployment, attribution in individual cases, and any entitlement to compensation.

The appropriate v0.1 conclusion is an open research agenda, not an accusation. Findings that weaken the hypotheses must be published alongside supportive findings. Technical success would support capability only; technical failure would limit the tested configuration, not every possible implementation.

## Call for Collaboration

We invite researchers and practitioners to:

1. Critique the operational definitions and proposed evaluation.
2. Reproduce or challenge extraction and clustering results once data and code exist.
3. Submit dated, public primary documents with precise scope and claim mappings.
4. Develop privacy-preserving provenance and opt-in participation designs.
5. Examine value attribution, governance trade-offs, and jurisdiction-specific legal questions.
6. Identify alternative explanations and negative results.

Use the [claim register](claim-register.md), [methodology](methodology.md), and [contribution guidance](../CONTRIBUTING.md). Do not submit private third-party conversations or confidential material. This project requests lawful research using synthetic, public, or explicitly authorized material.

The aim is to discover what can be established, including where the original hypothesis is wrong.
