# Lab card format (Idea Shelf)

Card = **lab card**. Blog = spoken prose. Poster / X = optional short line elsewhere. Do not collapse all three into one file.

## Fields

| Field | Job | Limit |
|---|---|---|
| `title` | Name | a few words |
| **Claim** (once, in body) | One sentence a skeptic can disagree with | ~25–35 words, one clause |
| **Status** (once, under the Claim) | Two axes. Editorial: `draft` or `ready`. Evidence: `untested`, `test specified`, `testing`, or `result in` | `ready` means reviewable, not endorsed or proven |
| **Serious rival:** (one line, end of §2) | Names the strongest existing alternative and why the card still differs | one line; not a second claim |
| body (§1–9) | Why, how, what breaks | paragraphs |
| Sources (optional appendix after §9) | Links and source notes | Mark the heading as an appendix (`## Appendix: Sources`). §9 stays the end of the argument |
| poster / X line | Optional chant | **never** in the card file; **never** feed to blog/essay prompts |

Quiet YAML only: `idea_id`, `title`, `status`, `tags`. **Deleted:** `one_liner`, `slogan`, and any bold+italic double lede that restates the claim.

## Body rules

- The claim appears **once**. After that: mechanism, bands, pilots, failure modes only.
- No stacked fragments, repeated thesis lines, bolded chants, or “X beats Y” as a paragraph. One short insight sentence is fine; the whole file is not a poster.
- Reject drafts where three or more sentences under twelve words restate the claim in the first screen.
- Evidence labels on working figures: **established**, **published-contested**, **working assumption**, **not found**. A figure that could not be verified is marked **not found**, not dropped silently.
- A rating that pulls a card is not a failed test. A card is marked rejected and kept only once something fails a test the card has defined (§6 First test or §9 Stress-test).

## Writing from a card

Use **sections 1–9** as source of truth. Do not imitate an old chant header. Negative example: pre-fix `phev-first` files that printed one_liner + slogan + bold + italic before §1.
