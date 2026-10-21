# Master prompt — paste this to start a new session on this repo

**Purpose:** this is a portable briefing for a fresh Claude Code session (or a teammate) working in `thelittlethingscollection-website`. Paste the block below as your first message. Updated 2026-10-21.

---

## Paste-ready block

```
You're working in TheLittleThingsCollectionCo/thelittlethingscollection-website, branch
claude/new-session-cpqico. The user is Danielle Hammerstone, RN, BSN — she runs several
ventures out of this one repo. Before anything else:

1. Run `git fetch origin claude/new-session-cpqico` and compare it to your local HEAD with
   `git merge-base --is-ancestor`. Multiple Claude sessions have worked this same branch in
   parallel without pulling each other's changes first, which has already caused one real
   divergence (two lineages of commits, resolved 2026-10-21 in commit 441bba3). If local and
   remote have both moved independently, merge — never force-push over either side. Read
   `docs/MASTER-PROMPT.md` (this file) and `docs/revenue/DO-THIS-NOW.md` for current state
   before doing anything else.

2. docs/revenue/DO-THIS-NOW.md is the canonical, founder-declared priority list. It supersedes
   any other priority list in this repo, including anything written here. The 2026-09-08
   Founder Decision block in it is the tiebreaker: ADRD compliance audits are the primary
   revenue engine, LNC is secondary, Marellstone is paused, and there's a seed freeze — no new
   venture gets build time until the first ADRD audit sells. Don't propose a competing
   priority list; propose edits to that one.

3. You do not have: Etsy publishing access, Instagram/Meta Business Suite login, the ability
   to contact insurance brokers or get quotes, or access to Danielle's GoDaddy/hosting
   accounts. You do have: read/write access to claude.ai artifacts she owns (check via the
   Artifact tool's `read` action before assuming), and full read/write on this repo.

4. Several claude.ai artifacts tied to her businesses had fabricated content from an earlier
   session (fake revenue figures, a "best seller" badge with no basis, a wrong Etsy shop link,
   a math bug in the ADRD self-check calculator). Most are fixed as of 2026-10-09 — see the
   "Session log" below for which ones and what's still open.
```

---

## Business portfolio

- **TwelveTen Compliance Education / TwelveTen Wellness** — Florida ADRD personnel-file compliance audits for home health agencies (Fla. Stat. §430.5025). **Primary revenue engine** per founder decision. Pricing: $495 (≤25 workers) / $895 (26–75) / $1,495 (76–150). Toolkit in `docs/adrd/`, website in `site/`.
- **The Little Things Collection** — consumer digital products (pregnancy/baby/family photo-idea vaults, Holiday Elf kit), sold on Etsy. Instagram: `@littlethingscollectionco`.
- **LNC (Legal Nurse Consulting)** — secondary engine, rides behind the same attorney/E&O errand as ADRD.
- **Marellstone & Co.** — paused as of 2026-09-08. Do not reactivate without an explicit founder call.
- **RON (Remote Online Notary)** — a near-complete side-rail; just needs a form mailed (see DO-THIS-NOW #8). Already paid for and completed — finishing it does **not** violate the seed freeze.

## Session log (what's been built, in order)

1. **Instagram growth plan** for `@littlethingscollectionco` — `docs/revenue/instagram-growth-plan.md`. Profile setup, 30-day content calendar, DM automation (switched to free Meta-native tooling instead of a paid ManyChat subscription).
2. **Pinterest traffic plan** — `docs/revenue/pinterest-growth-plan.md`. Companion to the IG plan; repurposes the same content instead of creating a second content workload.
3. **Etsy listing copy** for Survey Survival Kit and Bump Stories — ready, in `docs/revenue/etsy-listings.md`. Five more listings (DON OS, Newborn Vault, 3 mini-vaults) are blocked on Danielle opening the source PDFs herself — don't fabricate their contents.
4. **Day-one execution checklist** — `docs/revenue/day-one-checklist.md`. The zero-content-creation subset of the above, sequenced.
5. **ADRD referral-outreach unblock** — `docs/adrd/FL_ADRD_One_Page_Scope.docx` and `FL_ADRD_Sample_Findings_Report.docx` (illustrative/fictional, clearly banner-marked). These were the two missing prerequisites named by `docs/adrd/FL_ADRD_Referral_Partner_Outreach.docx`'s own 4 ready-to-send emails.
6. **E&O insurance research** — not contacted anyone (that needs Danielle directly: identity, business details). Gave her 3 real, verified options (CM&F Group, Proliability, NSO) with what to have ready.
7. **Fixed a live calculator defect** in the ADRD self-check tool — present in both `site/selfcheck.html` (not yet deployed) and a separately-shared claude.ai artifact (was independently reachable). First pass capped values at roster size; a regression check correctly found that still wasn't real validation (it silently substituted values). Second pass replaced it with actual input validation — blocks all output on invalid/incomplete input, preserves exactly what the user typed, shows field-specific correction messages. Verified against every case in both the original bug report and the regression report before publishing either copy.
8. **Corrected two claude.ai storefront preview artifacts** (TwelveTen Wellness "Professional Storefront" and The Little Things Collection "Consumer Storefront") — removed a fake "Best seller" badge, unverified prices, two products with no verified files, and a footer link to the wrong Etsy shop (`littlethingsheirloom.etsy.com`, a different brand). Applied the already-prepared replacement copy rather than inventing new copy.
9. **Resolved a branch divergence** (2026-10-21) — two parallel sessions had each pushed commits without pulling the other's first. Merged cleanly (commit `441bba3`); nothing was lost. RON mailing item and a real 98-provider HCAF prospect list (public directory data, no personal contacts, per Danielle's own stated constraint) are now unified with the rest of the session's work.

## Still open — needs Danielle directly, not Claude

- DON Operating System PDF contents (for its Etsy listing) — needs her to open the file.
- Actually publishing anything to Etsy — no connector access exists.
- Requesting the E&O quote — needs her identity/business details directly.
- ADRD site go-live — needs her to pick a free host (Cloudflare Pages/Netlify/Vercel) and update GoDaddy DNS for `the10wellness.com`.
- Shopify deactivation (requested 2026-10-09) — completion unconfirmed; affects whether the consumer storefront and "Money In Money Missed" dashboard can assume it's off.
- Two claude.ai artifacts are sign-in blocked — only she can supply an export or make them accessible.
- Three more artifacts have prepared-but-unapplied replacement copy (Founder OS Playbook, Social Launch Pack, Stripe App Verdict) — lower-stakes reference docs, not yet done, offered but not confirmed.
- The 116-page Elf revision and the PointClickCare V2 PDF are prepared but unverified — don't push either live without her opening and confirming them.

## Standing rules specific to this engagement

- `DO-THIS-NOW.md` is the tiebreaker on priority. A new idea gets captured and queued, not silently prioritized over it, unless Danielle explicitly overrides.
- Never fabricate product contents, financial figures, or "sample" data without clearly marking it as illustrative/fictional.
- Verify claims (regression reports, "this is broken" assertions) by reproducing them before fixing — don't take a report's word for it, and don't claim a fix works without re-verifying against the original failing case.
- This repo spans multiple real businesses with real compliance/privacy stakes (healthcare personnel data, PHI-adjacent content). Treat accuracy and credibility protection as load-bearing, not optional polish.
