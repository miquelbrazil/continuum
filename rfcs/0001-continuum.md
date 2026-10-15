# RFC 0001: Continuum

> The goal is not to preserve every artifact of a life. It is to preserve enough evidence, context, reasoning, and provenance that understanding can be reconstructed.

- Status: draft
- Date: 2026-10-10
- Origin: founding design dialogue, distilled with AI assistance.
- Acceptance: pending; this draft captures the requested foundation without treating every implementation proposal as settled.

## Purpose

A Continuum is a portable, provenance-aware corpus intended to preserve enough
evidence, context, reasoning, and knowledge to reconstruct understanding across
time. It preserves the structure of reasoning as well as its conclusions.

An archive can be much larger than the curated semantic layer that makes it
useful. Preserving everything does not make everything current knowledge, and
knowledge does not automatically become doctrine.

## Conceptual model

| Concept | Job |
| --- | --- |
| Archive | Preserves evidence that may matter later, including original artifacts. |
| Corpus | Makes selected evidence deliberately legible and addressable. |
| Knowledge | Expresses what is understood by interpreting and connecting evidence. |
| Doctrine | Expresses what currently guides decisions, with explicit acceptance and scope. |
| Dialogues | Preserve how understanding emerged through questions, arguments, corrections, and reframing. |
| Ledger | Records attributed observations and contributions from others, including project work and outcomes. |
| Oracle | Synthesizes answers from authorized evidence, with sources, uncertainty, and limits. |
| Collaborators | Operate within scoped domains of the corpus and explicitly bounded permissions. |
| Policy | Determines who may see or use what, for which purposes. |
| Projections | Expose policy-filtered views for particular audiences, domains, and uses. |

These are responsibilities, not ten mandatory storage locations. A dialogue may
be archived as evidence, selected into the corpus, and inform knowledge. A
ledger observation remains attributed to its author even when it informs a
synthesis.

## Foundational requirements

1. Preserve reasons and context alongside conclusions. Link distilled records
   back to their evidence and preserve the path by which understanding emerged.
2. Distinguish a direct statement, an accepted decision, a third-party
   observation, and an AI inference. Preserve contradictions and superseded views.
3. Treat confidence as an explained assessment grounded in evidence. An eloquent
   answer or a decimal score is not evidence of accuracy.
4. Make disclosure explicit. A person may maintain one or more Continuum
   projections for different audiences and domains.
5. Keep the underlying corpus portable. A receiving employer, collaborator, or
   service receives an authorized projection, not automatic access to the corpus.
6. Separate framework, instance, and implementation. The specification must be
   useful without a particular model provider, indexing engine, or application.

The [provenance](../concepts/provenance-and-confidence.md) and
[privacy](../concepts/privacy-and-projections.md) notes develop these
requirements.

## Capture and codification

Start with one useful source. Preserve its reference and relevant context,
distill a small record, identify its evidence and uncertainty, and assign its
status and disclosure scope. Mark an AI-written distillation as such until its
subject reviews it. Link the result back to the dialogue and the dialogue
forward to the result.

A codification dialogue can ask, in sequence: What do you think? What is it
distinct from? Which examples and counterexamples test it? Where did it come
from? How does it affect decisions? Where does it stop applying? What should it
be called? What does it connect to? What is the smallest durable statement?
What kind of record is it?

The dialogue preserves how an idea was reached. The distilled record preserves
what survived the conversation. Neither substitutes for the other.

## Oracle and collaborator boundaries

An oracle answers from the available, authorized record. It should distinguish
what the subject said from what the system infers they might say, identify the
relevant time and context, cite accessible evidence, and acknowledge gaps. It
may abstain when evidence is insufficient. It does not claim to be the person.

A domain collaborator receives an appropriate projection and explicit action
permissions. Knowledge of a person's preferences does not authorize actions on
their behalf. Ledger submissions do not become accepted beliefs automatically.

## Initial scope and unresolved choices

The initial implementation is linked Markdown and Git history. The
[documentation model](../concepts/documentation-model.md) and templates support
useful records immediately.

Open questions include stable identifiers across moves and exports, machine
schemas, calibrated confidence, policy enforcement and revocation, contributor
review, and the first software interface. Model selection, embeddings,
databases, agent orchestration, automatic ingestion, and automated actions are
deferred.

This draft does not claim to reproduce a mind or establish facts about a person
beyond what the evidence supports. Its wording preserves the founding dialogue;
the private instance retains the source reference and speaker attribution.

## Related draft proposals

[Policy-aware queries](0002-policy-aware-queries.md) and [consentful
enrichment](0003-consentful-enrichment.md) develop two boundaries left open
here. Their draft status does not revise the acceptance state of this RFC.
Related concepts include [Oracle and AI
memory](../concepts/oracle-and-memory.md), [referential
privacy](../concepts/referential-privacy.md), [portable
attestations](../concepts/portable-attestations.md), and
[Concordance](../concepts/concordance.md).
