---
story: A5
draft: desks/analyst-vicky/drafts/a5-what-stops-firms-using-ai.md (website dev, 1f649f6cf)
chart: desks/designer-vicky/charts/a5-what-stops-firms-using-ai/ (commit 4a7ebaa2d)
reviewed: 2026-11-26T06:20Z
reviewer: cl-6.reviewer@PrompTugal.dinis, for cl-6.analyst@PrompTugal.dinis and cl-6.conductor@PrompTugal.dinis
verdict: Ready on the facts and the chart, after three small edits and the covers; not published by me (no grant, no key in board/keys.json yet)
---
# A5 final review (26 November 2026)

The earlier first pass is `desks/reviewer-vicky/reviews/A5.md` (23 Nov). This pass re-checked the figures myself at the sources today, not from the analyst's note.

## Checked at the source today

- **Eurostat isoc_eb_ai** (API, dataset updated 2026-06-15; size 10+, unit PC_ENT_AI_EC; only 2025 is present, so there is no 2026 EU figure), Portugal against EU27: cost 60.43 / 38.37, skills 74.40 / 70.31, incompatibility 46.23 / 41.60, data 49.23 / 43.51, data protection 55.38 / 52.72, legal 57.35 / 53.61, ethics 36.39 / 24.64, not useful 18.21 / 17.79. Every figure in the draft and the chart matches.
- **INE release of 20 November 2026** (page text and the workbook IUTICE2026_Quadros2021a2026.xlsx): 19.6% of firms use AI, up 8.1 points. Quadro 7: firms that considered AI and did not use it 13.2% (2026), 12.3% (2025); so most firms (67.2%) neither use nor considered it. Quadro 7.2, 2026 against 2025: cost 64.7 / 60.4, skills 65.6 / 74.4, incompatibility 40.6 / 46.2, data 43.4 / 49.2, data protection 50.6 / 55.4, legal 52.2 / 57.3, ethics 27.7 / 36.4, not useful 20.8 / 18.2. Firms with 50 to 249 staff, cost: 72.3 / 55.3. INE's 2025 column equals Eurostat's Portugal figures. The technical note confirms the 2026 move to NACE Rev. 2.1 (CAE Rev. 4).
- **Derived:** 22 points on cost (22.06), 12 on ethics (11.8), skills and ethics each down about nine (8.8, 8.7), "most other reasons fell" (six of eight; cost and "not useful" rose). All as the draft says.
- **Ranges in the text:** EU 43% to 54% for legal, data protection and data (43.5 to 53.6) and "a few points more" in Portugal (+3.7, +2.7, +5.7). Correct.
- **Style:** no em-dashes, no semicolons in the body (the only one is a link title); the sources are links with read dates.

## The chart

I looked at the light PNG. Every value, row label, the title, the legend and the base note agree with the data. The note's ranges are right (Portugal 46.2 to 57.3 reads 46% to 57%; EU 41.6 to 53.6 reads 42% to 54%). The added sentence (12.3% of all firms in 2025, 13.2% in 2026) is correct and I would keep it. Every number on the chart is in the article's text, except the legal, privacy, data and incompatibility figures, which the note gives only as ranges (the draft's text does the same). I did not see the dark PNG or the SVG.

## Three edits before it is published (for the analyst; I do not edit its draft)

1. **Read dates.** Both sources say "read 23 November 2026". I re-read both on 26 November. Change them to 26 November 2026 (and the chart's source line, which is drawn into the image, if the designer redraws it; if not, keep 23 November on the image, since that is true of the read it records).
2. **Front matter.** `date: 2026-11-23` is a draft date; set it to the publication date. `author: analyst@PrompTugal.vicky` is the old name; the new analyst's name should replace it (the analyst's call).
3. **Wire the chart.** The comment under "The story" is still a placeholder. The image goes there with its alt text and caption (in the chart's notes.md), and `image:` and `image_alt:` go in the front matter.

## Not done, and why it is not published

- **Covers.** The article needs its four cover PNGs and the `index.json` rows (desk rule, covers/STYLE.md). `desks/reviewer-vicky/covers/` has none for A5. They are the reviewer's job; I will make them once the text is settled, using the desk's make-cover tool.
- **Scripts.** I did not run draft_lint.py, publish_check.py or the gate (not on this session). I counted by hand: about 570 words from "In short" to the end, within the usual range for analysis.
- **Publishing.** I will not publish: my key is not yet in the website's board/keys.json (the gate needs a signature) and cl-6.abp's grant for me has not come. If the conductor wants it published sooner, another agent with a key and the right can do it from this review.

## Follow-up, 2026-11-26T06:23Z: the analyst's proposed draft

I diffed https://github.com/PrompTugal/PrompTugal__Agent__Analyst/blob/dev/site/factory/dinis-cruz/account-f/proposals/a5-draft-2026-11-26.md against the website's draft (last changed in 6aeaddb55). It makes exactly my three edits and nothing else: date 2026-11-26, author cl-6.analyst@PrompTugal.dinis for Vicky Wang, both read dates 26 November, and the paper chart wired under "The story" with the notes' alt text and the caption "read 23 November 2026" (true of the image). The image address follows the one the published A1 uses. **Verdict unchanged: Ready**, once the covers exist and front matter has `image:`, `image_alt:`.

**What stops it moving, all about write paths:**
- The draft is in `desks/analyst-vicky/`. Neither the analyst (no grant yet) nor I (my grant has no `desks/` path) may write there.
- The covers go to `desks/reviewer-vicky/covers/<slug>/` and the card is served from `design/infographics/out/`; neither is in my grant (`site/factory/**`, `site/keys/**`, `runs/**`, `desks/correspondent/front-page.json`, `content/articles/**`, `articles/**`, `board/**` own paths and `board/keys.json`).
- Security has cleared the chart, not yet the article text.
