# RFC 0003: Consentful enrichment and witness contributions

- Status: draft
- Date: 2026-10-15
- Author(s): Codex, distilling private design dialogue; review and acceptance pending.
- Visibility and intended audience: general framework proposal; synthetic examples only.
- Sources and related records: [enrichment](../concepts/enrichment-and-elicitation.md), [referential privacy](../concepts/referential-privacy.md), [provenance](../concepts/provenance-and-confidence.md).
- Supersedes / superseded by: none

## Purpose and context

A system that connects sources and asks questions can improve understanding,
but it can also infer silently, steer behavior covertly, or recruit third
parties without consent. The framework needs distinct evidence and consent
states.

## Proposal

Before collection, declare source, purpose, scope, retention, inference
eligibility, disclosure boundary, and withdrawal path. Distinguish observed
behavior, self-report, elicited response, third-party observation,
institutional claim, and AI inference. Retain the path from hypothesis to
question, clarification, distillation, confirmation, and revision. Explain why
a question is being asked. Transparent stimuli are allowed only with the
subject's informed participation; no covert fake accounts or hidden social
experiments.

Witness flow is nomination → subject-authorized invitation → witness opt-in →
attributed contribution → subject review → separately authorized disclosure.
Nomination is not enrollment. Contributor policy may restrict identity,
relationship, quotation, and onward use. Reciprocity is optional.

## Evidence and confidence

The private design record includes an earlier covert-engagement exploration and
a later transparent boundary. This RFC proposes the later boundary while
preserving the design history in the personal instance. It does not assert that
any connector or witness workflow has been implemented.

## Privacy and projections

A connected service can contain other people's data. Consent to connect it is
not consent to publish, infer without limit, or contact those people. Derived
material remains restricted until reviewed. Questions and answers may
themselves become sensitive evidence.

## Alternatives and consequences

Manual, one-source import and subject-led codification reduce integration
complexity. Autonomous enrichment could cover more data but increases
interpretive and consent risk. A separate social account that hides its purpose
fails the transparency requirement.

## Scope and open questions

No connector, consent receipt format, retention schedule, or witness invitation
channel is selected. What can be corrected or deleted after derivation, and how
does withdrawal propagate to later knowledge records?

## Validation

With synthetic sources, a hypothesis is visibly labeled, a subject can correct
it without losing the source, and a named witness receives no contact before
authorization. Declining an invitation does not enroll or repeatedly prompt the
witness. A hidden stimulus fails the workflow.
