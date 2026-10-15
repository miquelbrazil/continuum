# RFC 0002: Policy-aware queries and AI memory

- Status: draft
- Date: 2026-10-15
- Author(s): Codex, distilling private design dialogue; review and acceptance pending.
- Visibility and intended audience: general framework proposal; synthetic examples only.
- Sources and related records: [Oracle and memory](../concepts/oracle-and-memory.md), [referential privacy](../concepts/referential-privacy.md), [provenance](../concepts/provenance-and-confidence.md).
- Supersedes / superseded by: none

## Purpose and context

A Continuum may answer directly or supply context to outside AI systems. A
corpus-wide search followed by redaction can let restricted evidence influence
the result or leak through citations, aliases, confidence explanations, and
caches. The framework needs a query boundary before an implementation is
chosen.

## Proposal

A query states requester, audience, purpose, domain, time scope, requested
answer mode (`about` or explicitly authorized `as`), and permitted uses. Policy
selects eligible records and fields before retrieval. A second disclosure check
governs the answer, entity rendering, source trace, and any durable cache. An
answer carries claim-level status (`direct`, `synthesized`, `inferred`,
`unknown`), confidence basis, time, and authorized citations or an explanation
that cannot name restricted evidence. Lack of permission or adequate evidence
yields a bounded answer or abstention. Memory consumers receive a projection,
not the canonical corpus.

Treat source visibility, use in inference, and output disclosure as separate
policy dimensions. An inference may not launder an undisclosable private fact
into a broader projection. Action authority is not implied by memory access.

## Evidence and confidence

The design motivation comes from private dialogue and recordings; this RFC
contains no personal source excerpts. It is a proposed boundary, not evidence
that any implementation exists or that confidence is calibrated.

## Privacy and projections

Apply policy to retrieval, graph edges, names and aliases, quotes, citations,
filenames, logs, and caches. Test re-identification from fact combinations.
Revocation controls future access but cannot erase copies already exported.

## Alternatives and consequences

A static, reviewed export is simpler and may be the first safe POC. A mediated
query service adds flexibility and enforcement burden. Redact-after-retrieval
is insufficient as a general policy boundary because excluded sources can
affect synthesis before redaction.

## Scope and open questions

No schema, API, model, or policy language is selected. Open: source-safe
explanations, answer-as authorization, expiry, client-side cache constraints,
contributor controls, and verification of projections.

## Validation

With synthetic records, a requester can get a dated direct answer from
permitted evidence; a hidden witness record neither changes nor leaks into the
answer. A permitted private query may use that record only within its stated
purpose. Alias rendering does not expose a person through a unique relationship
or event. An external AI cannot take an action merely because it received
context.
