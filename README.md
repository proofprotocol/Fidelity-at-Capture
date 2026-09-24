# PP-SPEC-023: Structural Independence and the Fidelity-at-Capture Requirement

**Status:** Published
**Author:** Craig Ellrod
**Date:** Sept 17, 2026
**License:** CC BY-ND 4.0

## Cite as

Ellrod, C. (2026). PP-SPEC-023: Structural Independence and the Fidelity-at-Capture Requirement.
Proof Economy Standards Alliance (PESA). https://doi.org/10.5281/zenodo.22821379

## Summary

Every corroboration model in this industry, including our own five-tier model (Activated, Committed, Witnessed, Analyzed, Sealed), answers the question: once evidence is captured, does it stay intact. None of them answer a different question: was the evidence faithful to begin with, or did the party being evaluated shape what got captured. This spec names that gap and defines the axis that closes it.

## The Gap

Consistency-of-data and fidelity-at-capture are not the same property. A tamper-evident record can be perfectly consistent with itself and still be worthless as proof, if the party who benefits from a favorable result also controls what gets fed into the record in the first place.

Cryptographic integrity proves a record wasn't altered after the fact. It says nothing about who generated the record, under what incentive, or with what access to shape the input. A hash chain on a self-generated log is still a self-generated log.

This is the Self-Attestation Oxymoron: a proof of efficacy cannot originate from the entity whose efficacy is in question. Not because the entity is dishonest. Because the structure of self-attestation makes independence unverifiable regardless of intent.

## Definitions

**Structural Independence.** The evidence-capturing party has no outcome-contingent financial relationship, no operational control ceded to, and no reporting relationship with the party whose performance is being measured, and the assessed party has no ability to alter the execution environment before or during capture. Payment for the act of assessment does not itself violate independence. Payment contingent on a favorable result does. A relationship in which continued revenue depends on producing favorable results for the same party does, whether or not any single fee is formally contingent. Selling remediation, consulting, or defense products to the same party whose product is being assessed does, regardless of fee structure, because it creates a return-engagement incentive that functions the same as a contingent fee.

**Cryptographic Integrity.** The evidence, once captured, cannot be altered without detection. This is necessary and not sufficient.

**Fidelity-at-Capture.** The evidence faithfully represents what the executor actually did, established through structural independence at the moment of capture, not through tamper-evidence after the fact.

**Consistency-of-Data.** The evidence remains internally consistent and unaltered from the point of capture forward. This is what most existing tier models, including four-tier axis models used elsewhere in this space, actually measure.

## Note on Payment

Structural independence is not the absence of payment. No assessor works for free, and a standard that required zero compensation would be unworkable by construction. What independence requires is that compensation not be tied, directly or through incentive structure, to producing a result favorable to the assessed party. This mirrors long-standing auditor independence practice: contingent fees are prohibited, non-audit consulting relationships with an audit client are restricted, and mandatory rotation prevents financial dependence on a single client's repeat business from accumulating. The same logic applies here. A flat fee for the act of assessment, paid regardless of outcome, from a party with no ongoing remediation or consulting relationship to the assessor, satisfies structural independence. A fee structure where the assessor's ongoing revenue depends on the assessed party being satisfied with the result does not, regardless of what the invoice says.

## Relation to the Five-Tier Model

Activated, Committed, Witnessed, Analyzed, and Sealed describe what happens to evidence once it exists. They do not describe whether the evidence was faithful at the moment it was generated. Fidelity-at-capture is a precondition to Witnessed and Sealed carrying any evidentiary weight. A Sealed record built on a self-attested capture is a well-preserved unreliable record.

## Distinguishing Note

AgentSight (arXiv:2508.02736, Zheng et al., Aug 2025) correlates an AI agent's stated intent with its system-level actions using eBPF, run as a daemon on the same host and under the same operator as the agent it observes. It solves signal correlation. It does not address origination independence, because its trust model assumes the operator running the observability daemon is trustworthy. That assumption is exactly what fidelity-at-capture refuses to make. The two are complementary, not competing: correlation tells you what happened, structural independence tells you whether you can believe who is telling you.

## Provenance

This document is timestamped and anchored via Zenodo, DOI https://doi.org/10.5281/zenodo.22821380, as of the publication date above.
