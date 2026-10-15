# Oracle and AI memory provider

- Status: draft concept, not an accepted interface.
- Origin: private design dialogue and recordings; generalized with AI assistance. Source locators remain in the personal instance.
- Related: [RFC 0001](../rfcs/0001-continuum.md), [query RFC](../rfcs/0002-policy-aware-queries.md), [provenance](provenance-and-confidence.md), [privacy](privacy-and-projections.md).

An Oracle answers questions from a time- and purpose-bounded projection of a
person's Continuum. A public “ask this person” page, a private assistant, and
an external AI consuming memory are different clients of the same evidence and
policy model. A canonical Continuum can reduce the stale, incompatible
representations held by separate services, but no service receives the whole
corpus by default.

## Answer contract

An answer **about** a person reports what the authorized record supports. An
answer **as** that person simulates or represents their voice and needs
explicit, narrower authorization. It must remain distinguishable from a live
statement by the person. Each substantive claim should be marked **direct**,
**synthesized**, **inferred**, or **unknown**, with relevant time, confidence
basis, contradiction, and source trace where disclosure permits. A model's
fluent output is not evidence. When authorized evidence is thin, qualify or
abstain.

“Trace this answer” should show the chain from permitted sources through
interpretation to claim. It cannot expose a hidden source, its existence, or a
private fact through explanation. A source may be eligible to inform private
reasoning yet not revealable as evidence; that separation never grants
permission to leak its content into a broader answer. Output itself needs a
disclosure decision.

An external AI should request context for a stated task and receive a limited
projection with scope, expiry, and use restrictions. It may ask the subject to
clarify uncertainty, but a response does not silently become enduring doctrine.
Memory access does not grant permission to take actions on the person's behalf.
“The system can know more than it is allowed to explain” describes a policy
constraint, not a license for unreviewed private inference.

Open questions include a portable query contract, how source-safe explanations
work, revocation and cache handling, answer-as authorization, and how client
systems represent uncertainty without stripping it away.
