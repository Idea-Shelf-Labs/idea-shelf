# Lab card format (Idea Shelf), v2

A card is a **lab card**: the claim, its evidence and the test that could reject it. The blog
post is the narrative version for general readers. A poster or social line, if any, lives
elsewhere. Don't collapse the three into one file.

Each card is one Markdown file, `cards/<id>.md`, in two layers:

1. **Data (YAML frontmatter).** The claim, status, every working figure with its evidence label
   and sources, the source register, who gains and who loses, the first test, provenance and
   licence.
2. **Reasoning (Markdown body).** The argument, 1,200–3,000 words, citing figures as `[F3]` and
   sources as `[S7]`. Numbers live in the frontmatter; the body doesn't restate tables of them.

## Frontmatter

| Field | Rule |
|---|---|
| `schema` | `idea-shelf/card@2` |
| `id` | Same as the filename; never changes once published |
| `title` | 2–6 words |
| `version` | Semver: minor for added evidence, major for a changed claim |
| `updated` | `YYYY-MM-DD` |
| `status.editorial` | `draft` · `review` · `published` · `retired` |
| `status.evidence` | `untested` · `test-specified` · `testing` · `result-in` · `rejected` |
| `claim` | One sentence a skeptic can disagree with, 25–40 words. Stated once, here only |
| `summary` | 40–90 plain words for search snippets |
| `domains`, `patterns` | Topic areas, and one or more of the 8 outcome patterns |
| `readiness`, `geography` | How far along the technology is; where the card applies |
| `why_not_yet` | The real barrier that has kept this from happening |
| `coalition`, `losers` | Who has to say yes and what each gets; who loses and how that is handled |
| `boundary`, `resilience` | Optional: where support starts and stops; the single point of failure removed |
| `rival` | The strongest alternative, and why the card still differs |
| `first_test` | Design, cost band, duration, success, `kill` (the result that rejects the card) and `kill_terms` (its key phrases, which the blog post keeps word for word) |
| `figures` | `F1`, `F2`, …: value, unit, optional range, evidence label, source ids, note |
| `sources` | `S1`, `S2`, …: type, title, publisher, date, URL |
| `post_url` | Optional: the blog post written from the card |
| `provenance` | Method, editor and approval date. A published card carries the editor's approval date |
| `license` | `CC-BY-4.0` |

### Evidence labels for figures

- `established`: consistent across credible primary sources.
- `published-contested`: published, but credible sources disagree; `low` and `high` are given.
- `working-assumption`: our own estimate, with the arithmetic in `note`.
- `not-found`: needed but unsupported. It stays listed; it is never dropped silently.

## Body

Eight sections, in this order and with these headings: `## Problem`, `## Mechanism`,
`## Proposal`, `## Why this, not the rival`, `## Who gains, who loses`, `## How we'd know`,
`## Why it might fail`, `## Open questions`.

- The claim is not restated in the body. The body opens with the problem.
- Every `[Fn]` and `[Sn]` exists in the frontmatter, and every source is cited somewhere.
- Every number that matters to the conclusion is a figure.
- No slogans, poster lines, bold-italic ledes or stacked restatements of the claim. Cards have
  no images; images belong in the blog post.

## Status and tests

`published` means reviewed and released by the editor, not endorsed or proven. A card is marked
`rejected` (evidence) only when something fails a test the card itself defined in `first_test`
or `## Why it might fail`; a low rating is not a failed test.

## Writing from a card

The blog post uses the card as its only source of facts: every number in the post is one of
the card's figures, and the post links back to the card.
