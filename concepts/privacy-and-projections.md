# Privacy and projections

> A person may maintain one or more Continuum projections for different audiences and domains.

A projection is a policy-filtered view with a defined recipient, purpose,
domain, and disclosure boundary. It may be a reviewed export today and a
mediated query interface later. The underlying corpus remains distinct from
what is shared.

## Working policy

Default to private when permission is absent or ambiguous. Labels such as
public, professional, team, trusted, and private describe possible audiences;
they do not form an automatic hierarchy of access. Permission for one employer
does not imply permission for another. Domain relevance alone does not grant
access.

A projection should state:

- Who may receive it and for what purpose.
- Which records, fields, domains, and dates are included or excluded.
- Which uses and actions are permitted, including onward sharing.
- Which evidence and confidence requirements apply.
- Who authorized it, when it was generated, and any expiry or review date.

Filter evidence before retrieval and synthesis. Apply the same boundary to
quotations, citations, filenames, metadata, generated answers, caches, and
logs. A citation or confidence explanation must not reveal a restricted source
or its existence. If authorized evidence is insufficient, give a bounded answer
or abstain.

Derived material remains at least as restricted as its inputs unless an
explicit disclosure review authorizes a redacted version. Third-party ledger
observations retain attribution and their own sharing restrictions; possession
of a record does not establish a right to share it.

## Practical boundaries

Markdown policy is a declared intention, not enforcement. GitHub visibility,
filesystem permissions, and future software controls must implement the
intended boundary. A private repository can still contain material unsuitable
for all of its collaborators.

Export only reviewed content into a fresh projection artifact. Sharing a Git
repository can also expose its history, including removed material. An exported
copy cannot be reliably recalled; revocation can govern future access but does
not erase copies already received.

Secrets do not belong in any of the repositories or projections. Keep
credentials in a secret store and record only an appropriate reference. Ignore
rules are an accidental-addition guard, not a security boundary or a secret
scanner.

## Additional boundaries

[Referential privacy](referential-privacy.md) covers aliases, relationships,
and identifying combinations of facts. Policy should distinguish eligibility
for inference, source visibility, and answer disclosure; a restricted source
cannot be laundered into a wider projection. The [query
RFC](../rfcs/0002-policy-aware-queries.md) proposes how to enforce these
boundaries before retrieval and again at output.
