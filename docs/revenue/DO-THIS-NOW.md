# Do This Now — September edition

**Rebuilt 2026-09-06.** Supersedes the 2026-08-15 version (still readable in git history). Same rule as before: every item is either ready to execute or a named decision — no building.

> **What changed since August:** a venture that isn't in the field guide was born, validated, and fully tooled — **TwelveTen Compliance Education**, the Florida ADRD personnel-file audit ($495–$1,495 fixed fee, statute verified, AHCA citing under tag CZ875). Its toolkit lives in `docs/adrd/` and its website in `site/`. It is the active expression of what the field guide calls SurveyReady step 1 ("sell the audit/service manually") plus the facility lane of venture 2. Meanwhile, the three Marellstone follow-ups flagged "overdue" on 08-15 were never sent and are now three weeks cold.

---

## FOUNDER DECISION — 2026-09-08 (canonical, supersedes all other priority lists in this repo)

Declared by Danielle after reviewing this document and the Business Autopilot inbox audit:

1. **Holiday Elf kit** — already in production and about to list on Etsy. Owned by the founder directly; not tracked here. Elf *expansion* (Memory Volume, Family Traditions, holiday bundles) waits for real conversion data from the listing — no building on top of it yet.
2. **The ADRD compliance audit (TwelveTen Compliance) is the primary revenue engine.** Rationale in the founder's words: the nurse work is more money per sale. The ranked list below is its critical path.
3. **LNC** rides behind the shared attorney/E&O errand (#1 below) and the routing calls; it is the secondary engine, not a parallel primary.
4. **Marellstone is paused** unless the founder explicitly reactivates it.
5. **Seed freeze**: no new ideas get build time until the first ADRD audit is sold.

Any Claude session working in this repo: treat this block as the tiebreaker. Do not write a competing priority list; propose changes to this one.

---

## Ranked by leverage

| # | Action | Blocker | Time | What it unlocks |
| --- | --- | --- | --- | --- |
| 1 | **One attorney meeting + one E&O insurance quote** | Founder scheduling | 2 calls | Delivery for **two ventures at once** — the same items (engagement terms, E&O, secure transfer) gate LNC delivery and ADRD go-live |
| 2 | Send the **Leesfield email** | None — published address, approved text, unsent since **07-22** | 5 min | First LNC outreach actually in market |
| 3 | **List the 7 finished PDFs on Etsy** | None — after the Elf listing is live | 2 hrs | Passive trickle; zero risk |
| 4 | **ADRD go-live**: deploy `site/` to a free host (Cloudflare Pages/Netlify/Vercel) and point the already-owned `the10wellness.com` at it via GoDaddy DNS (see `site/DEPLOY.md` — domain purchase is stale, resolved 09-16, nothing to buy) | Pick a host + update GoDaddy DNS | ~1 hr | The self-check funnel, SEO, and a legal email footer |
| 5 | **ADRD referral-partner outreach** (`docs/adrd/FL_ADRD_Referral_Partner_Outreach.docx`): 4 ready-to-send emails (attorneys, consultants, franchise networks, brokers) — now has its missing attachments, `FL_ADRD_One_Page_Scope.docx` and `FL_ADRD_Sample_Findings_Report.docx` (illustrative, added 09-19). The doc's own sequencing: consultants first, then attorneys, brokers, franchise networks last | The E&O quote in #1 — every partner will ask "what insurance do you carry" | ~1 hr to send | Referral pipeline that compounds, per the doc's own reasoning better than cold email |
| 6 | **ADRD cold outreach**: post the group/LinkedIn content, pull the AHCA licensure + HCAF lists, start the cold email sequence | #4 first (footer needs the address); lower priority than #5 per the referral doc itself | ongoing | Secondary paid-audit pipeline, once the referral channel is running |
| 7 | **LNC contact routing**: 7 receptionist calls (numbers + script in the 08-15 version, git history) | None | 45 min | 9 of 10 approved LNC emails get a send route |
| 8 | **Mail the Remote Online Notary (RON) registration**: Online Notary Public information form, signed, + course completion certificate + $10 check to Florida Dept. of State + RON provider already selected on the form. Confirm the $25,000 bond/E&O upgrade is in place first (standard commission's $7,500 bond isn't enough for RON) | None — commission held, RON course already done, provider chosen; just needs mailing | 15 min | Finishes a side-rail income source (session fees, no calls/driving) at $10 marginal cost. Does **not** break the seed freeze — it's closing out a venture already paid for and completed, not starting a new one |
| 9 | ~~Marellstone: decide — activate or pause~~ | **Decided 09-08: paused** | — | Reactivation is a founder call, not a drift back. |

## The quarter's one strategic decision

**Made — see the Founder Decision block above.** ADRD is the primary engine; LNC secondary; Marellstone paused; Elf ships and waits for conversions before expansion.

## Where things live

- `docs/adrd/` — audit tracker (Excel, formula-verified), client intake, findings report template, referral outreach (parked until 3 audits done)
- `site/` — the TwelveTen Compliance website: landing page, §430.5025 requirements guide, 2-minute self-check
- `docs/twelveten-strategic-field-guide.md` — the master strategy book
- `.claude/skills/performance-review/` — manager review skill; still needs the real competency framework pasted into its reference files
