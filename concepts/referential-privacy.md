# Referential privacy and projections

- Status: draft concept.
- Origin: private design dialogue and recordings; generalized with AI assistance.
- Related: [privacy and projections](privacy-and-projections.md), [query RFC](../rfcs/0002-policy-aware-queries.md), [provenance](provenance-and-confidence.md).

A canonical entity can render differently by projection: full name, first name,
relationship label, role, or opaque identifier. This applies to people other
than the subject as well as to the subject. Rendering is governed by recipient,
purpose, context, and the other person's permissions; it is not a global
rename.

Aliases alone do not prevent re-identification. A relationship, uncommon event,
location, quote, or combination of innocuous facts can identify someone even
when their name is hidden. Policy therefore needs to cover entity references,
relationship edges, quotations, citations, and generated summaries together.
Source visibility, eligibility for inference, and answer disclosure are
distinct decisions. A sealed, restricted, embargoed, private, or
contributor-controlled source must not become public through an apparently
harmless graph edge or explanation.

A nominated witness is not enrolled by being named. Subject permission to
invite and contributor permission to participate, attribute, quote, and
disclose are separate. Outside observations remain attributed observations, not
objective truth. The [elicitation model](enrichment-and-elicitation.md) governs
consent to contact and ask.

A projection should be tested for identifying combinations, not only literal
names. The safe rendering may be omission or a bounded answer rather than an
alias. Reviewable exports remain safer than handing a client the underlying
corpus or Git history.
