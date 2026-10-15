# Continuum

> The goal is not to preserve every artifact of a life. It is to preserve enough evidence, context, reasoning, and provenance that understanding can be reconstructed.

Continuum is a framework for continuity of self across time: a portable,
provenance-aware corpus that preserves both what is understood and how that
understanding emerged.

## Three repositories

| Repository | Responsibility |
| --- | --- |
| `continuum` | Framework and specification: concepts, RFCs, conventions, and templates. |
| `continuum.me` | Miquel's actual personal corpus: evidence, dialogues, knowledge, and evolving commitments. |
| `continuum.core` | Software that will index, query, and project a corpus under its policy. |

The framework can be public independently of any personal instance. Examples
here should be synthetic or explicitly cleared for publication.

## Start here

- [RFC 0001: Continuum](rfcs/0001-continuum.md) — the model and its boundaries.
- [Documentation model](concepts/documentation-model.md) — five distinct jobs for documentation.
- [Provenance and confidence](concepts/provenance-and-confidence.md) — evidence, attribution, and uncertainty.
- [Privacy and projections](concepts/privacy-and-projections.md) — audience and disclosure boundaries.
- [Oracle and AI memory](concepts/oracle-and-memory.md) and [referential privacy](concepts/referential-privacy.md) — answers and identity rendering.
- [Enrichment](concepts/enrichment-and-elicitation.md) — transparent questioning and witness consent.
- [Professional portability](concepts/portable-attestations.md) and [Concordance](concepts/concordance.md) — authorized institutional and relationship views.
- [Annual and experience](concepts/annual-and-experience.md) and [intellectual lineage](concepts/intellectual-lineage.md) — longitudinal experience and research leads.
- Draft [RFC 0002](rfcs/0002-policy-aware-queries.md) and [RFC 0003](rfcs/0003-consentful-enrichment.md) — proposed query and collection boundaries.
- [RFC template](templates/rfc.md) and [ADR template](templates/adr.md).

## Working conventions

This is a draft specification, with no released version or conformance claim.
Keep files small, use descriptive lowercase names, and link related records.
Number RFCs and ADRs independently as `0001-descriptive-name.md`. An RFC
proposes a model or change; an ADR records a particular decision and why it was
made. Copy templates into the repository where the proposal or decision
belongs. Start proposals as `draft` and decisions as `proposed`; record who
accepted them before changing their status to `accepted`.

Add directories when they contain a useful record. Concept names do not require
matching folders, software services, or database tables.
