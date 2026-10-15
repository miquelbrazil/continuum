# Documentation model

The five distinctions from the founding dialogue:

> Inventory tells you what you own.
>
> Service maps tell you how it works.
>
> ADRs tell you why it works that way.
>
> Runbooks tell you what to do when it doesn't.
>
> Change history tells you what changed.

| Record | Useful contents |
| --- | --- |
| Inventory | What exists, its role, owner, location or reference, and when it was verified. |
| Service map | End-to-end relationships, flows, dependencies, and important boundaries. |
| ADR | Decision context, alternatives, choice, consequences, and acceptance. |
| Runbook | Trigger, prerequisites, steps, expected results, recovery, and last validation. |
| Change history | Dated material changes, reasons, outcomes, and affected records. |

Link these records instead of repeating their contents. An ADR explains a choice;
the service map describes the resulting system; the runbook describes how to
operate or recover it. Configuration notes can live beside the relevant map or
runbook. Git tracks edits; change history explains meaningful changes in the world,
which may occur at a different time from the documentation edit.

> Document reasons wherever a future-you would otherwise be tempted to “clean up” something that looks strange.

These operational records sit alongside principles, perspectives, working
theories, ontologies, and dialogues. A perspective can inform many ADRs; a
dialogue can explain how a perspective emerged. Everything need not become an ADR.

Preserve the reason, not merely the configuration. Record verification dates and
unknowns rather than making old configuration notes look current. Store credential
references only, never passwords, tokens, recovery codes, or private keys.
