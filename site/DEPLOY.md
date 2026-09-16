# TwelveTen Compliance Education — how to put this live

Status as of 2026-09-16: **files are deploy-ready.** Domain placeholders are resolved and the
mailing-address gate is handled. Nothing here needs to be bought or written before you can publish.

Target domain: **www.the10wellness.com**

---

## 1. Domain — already owned, nothing to buy

**Target: `www.the10wellness.com`** (GoDaddy). Chosen because it reads as TwelveTen Wellness,
matches the LLC name that signs the engagement letters, and the DNS is reachable today.

Verified domain portfolio as of 2026-09-16 (confirmed from registrar dashboards, not WHOIS):

| Domain | Registrar | Access | Notes |
|---|---|---|---|
| `the10wellness.com` | GoDaddy | Accessible | **Target for this site.** Exp 2027-03-28 — confirm auto-renew is ON |
| `marellstone.com` | GoDaddy | Accessible | Marellstone & Co. — do not use for compliance content |
| `thelittlethingscollection.com` | Namecheap | Accessible | Consumer brand. Active, auto-renew ON, exp 2027-06-28. Google Workspace + `hello@` already working. No site on it |
| `twelvetenwellness.com` | Squarespace | **LOCKED OUT** | Registered under an inaccessible email. Paid through 2028-10-30, so not urgent |
| `twelvetenwellnesscloudnetcorp.com` | Squarespace | **LOCKED OUT** | Expires 2026-10-16 |

Not owned, available if a dedicated compliance domain is ever wanted: `twelvetencompliance.com`,
`twelve10compliance.com`, `twelvetendesign.com` (~$12/yr each).
Owned by others, do not pursue: `twelve10.com` (parked for sale), `twelveten.com` (Cloudflare).

Changing the domain later is one find-and-replace across `site/`:
`www.the10wellness.com` -> the new domain. It appears in `index.html`, `selfcheck.html`,
`florida-adrd-training-requirements.html`, `sitemap.xml`, `robots.txt`.

### Squarespace lockout — deliberately deferred

`twelvetenwellness.com` is the best brand match but is registered under an email that can no longer
be accessed. It is paid through **October 2028**, so nothing is at risk this year and recovery is
not on the critical path. When there is capacity: use Squarespace's domain account recovery with
proof of payment (card last four, registration date 2025-10-30), then transfer the domain out to
GoDaddy or Namecheap so it sits in an account that is actually controlled.

## 2. Host it free

Pick one. All have free tiers that cover this site.

- **Cloudflare Pages** — best fit here. Connect the repo, set the build output directory to `site`,
  no build command. Then add `www.the10wellness.com` as a custom domain.
- **Netlify** — drag the `site/` folder onto app.netlify.com/drop. Then
  Site settings -> Domain management -> add the subdomain.
- **Vercel** — same idea; set the root directory to `site`.

Then in **GoDaddy DNS** for `the10wellness.com`, point it at the host:
- a `CNAME` for host `www` -> the target the host provides, and
- the host's apex/root record (GoDaddy supports forwarding, or use the `A`/`ALIAS` value the host gives you)

The host shows the exact values after you add the custom domain.

## 3. Mailing address — NOT required to publish

**A physical postal address is a CAN-SPAM requirement for commercial email, not for a web page.**
The site is legal to publish today with no address on it.

All three pages now carry a commented-out `MAILING ADDRESS GATE` block in the footer instead of a
visible placeholder. Nothing renders, so there is no broken-looking text on the live page.

**Do not put a home address here.** It would be public, indexed, and scraped into data-broker
databases. Use a virtual mailbox or a USPS PO Box.

Before the **first email campaign** that links to this site, replace the comment block in all three
footers with the real line:

```html
<p>TwelveTen Compliance Education · [VIRTUAL MAILBOX OR PO BOX ADDRESS]</p>
```

Rough costs when there's room for it: USPS PO Box ~$25-40 per six months; virtual mailbox
(Anytime Mailbox, PostScan, iPostal1) ~$10-15/month and gives a street-format address, which some
agency clients prefer over a PO box.

## 4. Contact email

Every page currently points at `twelvetenwellness@gmail.com` (in `index.html` structured data plus
the mailto links across all three pages). It works, so this is not a blocker.

Note: a working `hello@` already exists on Google Workspace, but it is attached to
`thelittlethingscollection.com` — the consumer brand — so it is the wrong address for
agency-facing compliance work. If a branded address is wanted here, set up email on
`the10wellness.com` at GoDaddy rather than reusing the Little Things mailbox.

## 5. Wire up measurement — both free, do after it's live

- **Google Search Console** (search.google.com/search-console) — verify the domain, submit
  `sitemap.xml`. In ~2-4 weeks the Performance tab shows the exact queries people typed to find you.
  This is the real "what are agencies searching" data.
- **Google Analytics 4** (analytics.google.com) — create a property, paste the snippet before
  `</head>` on all three pages.

---

## What's in this folder

| File | Purpose |
|---|---|
| `index.html` | Service / landing page |
| `florida-adrd-training-requirements.html` | SEO guide page — the ranking play |
| `selfcheck.html` | Interactive ADRD file self-check (converted from the Claude artifact) |
| `robots.txt`, `sitemap.xml` | Search engine plumbing |

## Resolved 2026-09-16

- `www.twelveten.example` placeholder replaced in all 5 files, now pointing at `www.the10wellness.com`
- `[MAILING ADDRESS]` visible placeholder replaced with a commented gate in all 3 pages
- `sitemap.xml` `lastmod` bumped to 2026-09-16
- Stale "buy a domain" step removed — the domain was already owned
