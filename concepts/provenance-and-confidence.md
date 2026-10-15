# Provenance and confidence

Provenance records where a claim came from and how it became this record.
Confidence records how well the evidence supports a particular claim in a
particular context. Neither can be replaced by a model's self-assurance.

## Preserve epistemic differences

- A direct statement by the subject.
- Repeated behavior inferred across records.
- A decision the subject explicitly accepted.
- An old belief that has since been superseded.
- An observation written by somebody else.
- An AI inference based on weak evidence.

These categories can overlap, but they are not interchangeable. A summary of a
direct statement is still a summary; the summarizer is not the original
speaker. Agreement to explore an idea is not acceptance of every suggestion
made during it.

## Minimum useful record

Use a short metadata list or frontmatter; no machine schema is fixed yet:

- Title, record type, and status: draft, accepted, superseded, or retired.
- Author or speaker, subject where relevant, and who distilled or edited it.
- Source reference with a message, section, or other precise locator; state when
  only a summary or excerpt is available.
- Source date, capture date, and last verification date when applicable; use
  `unknown` when a date is not known.
- Evidence kind, supporting and conflicting evidence, and inference boundaries.
- Confidence assessment with its basis, limitations, and scope.
- Visibility and permitted audience/use; missing permission means private.
- Related records and supersession links when applicable.

Attribute individual claims when a document mixes speakers or evidence types.
When accepting a record, note who accepted it and when. Record changes of
belief explicitly and link both the old and new views; Git history alone does
not tell a reader which belief currently applies.

## Explain confidence before scoring it

Assess evidence strength, independent supporting sources, recency, consistency
over time, explicitness, supersession, and how much inference an answer
requires. Several copies of the same source do not count as independent
corroboration. Recency matters differently for a historical fact and a current
preference.

For now, use a qualitative assessment such as `well supported`, `tentative`, or
`unknown`, followed by an explanation. Numerical scores remain a future design
question until there is a defined method and calibration. Do not copy the
illustrative numerical score from the founding conversation as a measured
result.

Confidence in accurate quotation can be high while confidence that the
statement still describes the subject is unknown. Report that distinction,
conflicting evidence, and the limits of the available record. When evidence is
inadequate, say so rather than inventing a current belief.

## Correction as provenance

An observation, another person's interpretation of it, and the subject's
correction are separate records. Close observation can still miss context or
private meaning. Preserve the earlier interpretation and the correction with
dates and attribution; do not overwrite either or silently promote an outside
observation to truth. This applies to interpersonal dialogues as well as
imported behavioral data. See [elicitation](enrichment-and-elicitation.md).
