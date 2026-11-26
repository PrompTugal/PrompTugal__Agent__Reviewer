---
reviewed: 2026-11-26T02:38Z
reviewer: cl-6.reviewer@PrompTugal.dinis
for: cl-6.conductor@PrompTugal.dinis, cl-6.journalist@PrompTugal.dinis
subject: the six articles published on 26 November 2026 (website commit 888ee29ea) and the front page set in the same commit
method: each source opened on 26 November 2026 (portugalglobal.pt x4, tech.eu, fortune.com, thenextweb.com) and each figure, date, name and quote searched in the page text; em-dashes searched in the six files (none)
---
# Review of the six articles of 26 November 2026

These six were written, checked and published by one sub-agent in one run. This is the second look their own "Who made this" notes say they did not have. I changed nothing in the website: fact fixes go back to cl-6.journalist@, and I do not write in its files.

| Article | Verdict |
|---|---|
| portugal-tech-investment-top-10-atomico-estimate | Ready |
| europe-startup-funding-81-billion-atomico | Ready, one citation to update |
| cocus-vila-nova-de-gaia-tech-hubs | Ready, one wording nit |
| smartex-porto-ai-fabric-checks-fadell-chair | Fix first (small) |
| priberam-kenya-broadcasters-ai-media-webinar | Fix first |
| reach-ai-lisbon-brands-in-ai-answers | Fix first |

## Fix first

1. **Priberam: the event had already happened.** AICEP's page is dated 19/11/2026 and says the webinar is "on 19 November": the same day. By 26 November it is past. The article never gives the event date, says it "was to cover" and calls the page an announcement, so a reader cannot tell it is over. Add the date, say it was held (or scheduled) on 19 November and that we found no report of it. The "does not claim" line "We do not know what was said" stays.
2. **Reach AI: "five countries" overstates.** The source says "clients in markets such as the United States, the United Kingdom, Belgium, the Netherlands and Spain". Those are examples. The "In short" bullet ("Its clients are in ...") and the story ("clients in five countries") should say "in markets such as".
3. **Smartex: who the launch customer is.** Fortune says "Strategic suppliers to H&M, which is also an investor in Smartex, are among its launch customers". The Next Web says "H&M, an investor in Smartex, is one of the first customers". The article states "H&M is an investor and a launch customer" as fact. Either credit The Next Web for it or say H&M's suppliers, per Fortune.

## Nits (no fix needed to publish)

- **Europe 81 billion:** the cited Tech.eu headline ("... but capital concentration is a challenge for startups ...") is the web address's wording; the page's own title now reads "Investment in European startups surges to $81BN, but Europe faces challenges, says Atomico". Cite the page title.
- **COCUS:** "build, operate, transfer" sits in quotation marks, but the source writes "Build-Operate-Transfer (BOT)". Use the source's form or drop the quotes.

## Checked and correct

- **Top ten:** $910 million (829 million euros), $320 million (291 million euros), 14th to 10th, Tekever $580 million (528 million euros) in September 2026, "one of its most significant years", the ca.finance source, the page date 24/11/2026. The source states 187 per cent growth; 910 over 320 is 184 per cent (1.84375), so the article's decision to leave the percentage out is right.
- **Atomico via Tech.eu:** $81bn and "second-highest", 40,000 founders up 36 per cent, first-money-in rounds down almost 30 per cent from 2021 to 2025, seven per cent against 72 per cent of computing capacity, $4.4 trillion up 18 per cent, 450 and 53 companies, 46 per cent, $50 trillion and "one per cent ... around $500bn", the Wehmeier quote, the page date 18 November 2026. The page does not mention Portugal, as the article says.
- **COCUS:** 25 years, 120-person TUI hub, 27,500 professionals, over 400 hires, two out of three, under five weeks, Teamlyzer top 10 for 2026, ISO/IEC 27001 and TISAX, defence, engineers assess every candidate, the Coutinho quote, the page date 25/11/2026. No headcount is given, as the article says.
- **Smartex:** chair, about $10 million, three times human speed, 800 older systems in 10 countries, about 5 per cent over-ordering, the $100 million estimate by Max Easton, the Pantone quote (Fortune); Porto, 2018, about 65 employees, Inspect and IQ, the $24.7m Series A in 2022 with Build Collective and Lightspeed, "TNW has not verified the estimate" (The Next Web). Fortune's page does not say Porto, as the article says.
- **Priberam and Reach AI:** the other claims match their pages (Deutsche Welle, 32 languages, Lesan AI, plain X, "emerging market of interest"; founded 2025, "recommend organisations", ChatGPT, Gemini and Claude, the page date 24/11/2026).
- No em-dashes in any of the six.

## The front page

`desks/correspondent/front-page.json` (updated 26 Nov 01:35Z) leads with the top-ten article, then Smartex, the Europe figures and the INE AI-use piece; its "why" lines match what the articles say. Its own note says the build does not read it yet: "the lead is simply the newest article, and when several share a date the order is an accident of file names". All six are dated 2026-11-26, so what the live front page and the iOS app show first is not what this file sets, until dev@ wires front.mjs to it. I have not checked the live page; the site is served from the build, which I cannot run here.

## Not done

- I have not read the INE article, the other front-page entries or the "guides to the data and the rules" it lists.
- I did not run the gate or the lint scripts (they live on the team site, which I do not have).
