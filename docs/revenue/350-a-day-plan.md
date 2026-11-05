# $350/day plan — ADRD audit engine

**Built 2026-11-05.** Works inside the 09-08 Founder Decision (ADRD is the primary engine, seed freeze until the first audit sells). This file is the sales plan for that engine. It doesn't replace `DO-THIS-NOW.md`.

---

## The math (read this first)

- $350/day × 30 days = **$10,500/month**. (Weekdays only: $7,700/month.)
- At a $750 average audit (the middle of the $495–$1,495 range), that's **14 audits a month**. Every month, from new buyers. That's hard to sustain from cold email alone.
- The version that holds up is **audits up front, then a monthly plan after**:

| Month | New audits (avg $750) | Monthly plan clients ($249/mo) | Monthly revenue | Per day |
| --- | --- | --- | --- | --- |
| 1 | 2 | 0 | $1,500 | $50 |
| 2 | 5 | 1 | $3,999 | $133 |
| 3 | 8 | 4 | $6,996 | $233 |
| 4 | 9 | 9 | $8,991 | $300 |
| 5 | 9 | 14 | $10,236 | $341 |
| 6 | 9 | 20 | $11,730 | **$391** |

*Assumptions (not verified data): 60% of audit clients add the monthly plan starting the month after their audit, and churn is zero in the first six months. The $249 price is a placeholder for you to approve.*

**Monthly plan ("ADRD Compliance Watch", $249/mo, up-sell only):** the client sends new hires and the training log once a month. You check them against §430.5025 deadlines and send a one-page "who's due in the next 30 days" list. It's the same work as the audit in smaller pieces, so it doesn't break the seed freeze. **You only offer it to people who have already bought an audit.**

**Bottom line:** you can get to $350/day in roughly 5–6 months if outreach runs every weekday. It won't happen this week. This week's target is **one paid audit**.

---

## Who buys

Florida providers covered by §430.5025 that keep personnel files with ADRD training deadlines. In priority order:

1. **Independent home health agencies and nurse registries.** Small, owner-run, and the decision-maker reads email. The list is already started: 247 pulled, 27 with emails, 18 form-only.
2. **Assisted living facilities (ALFs).** Many of them, they're surveyed often, and the administrator is reachable.
3. **Homemaker/companion agencies and adult day care.**
4. **Skip for now:** multi-site chains and SNFs. They have corporate compliance staff and long buying cycles.

**Where the list comes from:** FloridaHealthFinder.gov (AHCA) facility search by provider type. Pull ALFs and home health in 2–3 regions you can name in emails, such as Tampa Bay, Orlando, and South Florida. Goal: **300 contacts with a real email address**.

---

## The three channels, ranked

### 1. Referral partners (best close rate, asynchronous)
The send-ready emails are in `docs/adrd/FL_ADRD_Referral_Partner_Outreach.docx`. Partners are people who already serve your buyer: healthcare-licensing consultants, home care franchise networks, healthcare attorneys, and insurance brokers.
- One consultant who refers 2 agencies a month adds about $1,500/month.
- Goal: **10 partners contacted in week 1 and 3 active partners by day 45.**
- Gate: they'll ask about E&O insurance, so get the quote first (`DO-THIS-NOW` #1).
- If you offer referral fees, ask the attorney before you put it in writing. It's a healthcare-adjacent business, so confirm it's clean.

### 2. Cold email (volume, asynchronous)
The sequence is ready in `adrd-cold-outreach.md`.
- **Pace: 25–40 personalized emails per weekday**, sent from a the10wellness.com address. Not Gmail, and no mass blasts, because deliverability matters more than volume.
- Realistic results to plan around: **2–5% replies, and about 1 paid audit per 100–150 emails.** That works out to about 4–6 audits a month from cold email at this pace.
- Track every send in the "Ready to Email" tab: Sent, Replied, and Booked.

### 3. The self-check page (inbound, compounds)
`site/selfcheck.html` plus the §430.5025 guide. Once the site is live (`DO-THIS-NOW` #4), every cold email and partner email links to the 2-minute self-check. Anyone who fails it gets the $495 offer. The page also builds search traffic, which goes on working after you stop sending.

**Not recommended right now:** paid ads (B2B compliance audiences are too small to buy cheaply), Instagram for ADRD (wrong buyer), and cold calling (not how you want to sell).

---

## How a sale closes (all in writing)

1. They reply, and you send the One-Page Scope plus the Sample Findings Report. Both are in `docs/adrd/`.
2. You send a **payment link** for the fixed fee, paid up front. Stripe Payment Link or a QuickBooks invoice both work, but it has to exist before the first email goes out.
3. When payment clears, send the Client Intake & Authorization form and the secure upload instructions.
4. Deliver the findings report within 48 hours.
5. On delivery, offer the monthly plan: *"Want me to catch the next deadlines before they're missed? $249/mo."*

---

## Blockers before the first send (all yours, about 2 hours total)

| Blocker | Why it blocks | Fix |
| --- | --- | --- |
| Mailing address for the email footer | CAN-SPAM requires it in commercial email | A virtual mailbox or PO box, not your home address |
| Payment link | You can't take a yes without one | Stripe Payment Link: $495, $995, $1,495 |
| Site live on the10wellness.com | It's the email footer link and the self-check funnel | `site/DEPLOY.md`, about 1 hour |
| E&O quote | Partners will ask | 1 call (`DO-THIS-NOW` #1) |
| **Credential line check** | The cold email says "former Director of Nursing at a 120-bed SNF". Only RN, BSN is confirmed in your profile | Confirm it's accurate as written, or cut it |

---

## Daily rhythm (about 90 minutes, asynchronous)

- 30 min: send 25–40 cold emails
- 20 min: answer replies and send scopes and payment links
- 20 min: follow up with partners (2–3 a day until you have 10 contacted)
- 20 min: deliver audits once they're coming in. This grows into the main job.

## Scoreboard (check every Friday)

Emails sent · replies · scopes sent · paid audits · monthly plans · partners active · revenue this week ÷ 5
