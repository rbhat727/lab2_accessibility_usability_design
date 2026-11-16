# AUDIT

Name:

## Baseline (home.html before any changes)

| Check | Result |
|---|---|
| Lighthouse accessibility score | 84 |
| Lighthouse failed audits | 0 |
| WAVE errors | 1 |
| WAVE contrast errors | 6 |
| WAVE alerts | 9 |
| HTML validator errors | 5 |
| Keyboard test (notes) | Tab, Shift + Tab and Space work, Enter seems to do the same thing as Space |
| 200% zoom and 320px test (notes) | When not full screen, there is missing content and sideways scrolling needed. |

Contrast pairs checked:

| Text color | Background color | Ratio | Pass or fail (4.5:1 normal, 3:1 large) |
|---|---|---|---|
|Light blue| White| 1.31:1|Fail |
| Black|White |18.12:1 |Pass |
| Light grey|White | 1.75:1|Fail |

## Problems found on home.html (at least 8)

| # | What I saw (evidence) | Tool or test that showed it | POUR principle | WCAG idea | Severity | Planned fix |
|---|---|---|---|---|---|---|
| 1 |Language missing |WAVE test |robust |Language |Medium | Specify language|
| 2 |Duplicate hours |HTML test | Robust|Info and Relationships| Medium| Remove one of the hours|
| 3 |No li element in scope but a li end tag seen. | HTML|robust |Info and relationships |Medium | |
| 4 | Two contrast failures| contrast test|perceivable |Contrast |medium | change the colours|
| 5 |Missing text and sideways scrolling |zoom test |operable |Reflow |high | increase minimum fixed width|
| 6 |h5 follows h3, skipping one heading level |HTML |Robust |Info and relationships |Medium | |
| 7 |Center element is obsolete, use CSS instead |HTML |Robust |Info and relationships |Medium | |
| 8 |Stray end tag ul |HTML |Robust |Info and relationships |Medium | |

## ARIA notes (Part 2, step 13)

For each ARIA attribute you kept or added, explain why a native HTML element could not do the job. If you use none, say so.

## Usability review of services.html

Task scenarios:

- Task A: Estimate the cost for a large dog for boarding and grooming.
- Task B: Find out if a stay from December 24, 2026 to December 26, 2026 is possible.
- Task C: You added Training by mistake. Remove only Training.

Findings (at least 6, at least 5 different heuristics):

| # | Task | Evidence (what happened) | Heuristic | Severity | Change to test |
|---|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

Design checklist for this page:

- Who is using this?
- What is the primary action?
- What competes with it?

## Retest of services.html

| Task | Before (result) | After (result) |
|---|---|---|
| A | | |
| B | | |
| C | | |

## Verification of book.html

| Check | Result |
|---|---|
| HTML validator errors | |
| Lighthouse accessibility score | |
| Keyboard test (notes) | |
| DevTools check of the status message container (what attribute did you see?) | |

## After (home.html final)

| Check | Before | After |
|---|---|---|
| Lighthouse accessibility score | | |
| WAVE errors | | |
| WAVE contrast errors | | |
| HTML validator errors | | |
| Keyboard test | | |
| 200% zoom and 320px test | | |

## Before shipping checklist (all three pages)

- [ ] Keyboard access works everywhere. Proof:
- [ ] Focus is always visible. Proof:
- [ ] Contrast passes. Proof:
- [ ] Layout works on small screens. Proof:
- [ ] Feedback is meaningful (errors and success). Proof:

## One thing I had to check by hand that the tools did not catch

