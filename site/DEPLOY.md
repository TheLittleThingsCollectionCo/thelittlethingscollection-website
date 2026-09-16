# TwelveTen Compliance Education — how to put this live

Status as of 2026-09-16: **files are deploy-ready.** Domain placeholders are resolved and the
mailing-address gate is handled. Nothing here needs to be bought or written before you can publish.

Target domain: **compliance.thelittlethingscollection.com**

---

## 1. Domain — already owned, nothing to buy

`thelittlethingscollection.com` is registered at Namecheap (renews 2027-06-28, $11.18/yr) and is
currently serving a Namecheap parking page. This site goes on the `compliance.` subdomain so the
consumer brand and the nurse-facing compliance brand stay separate.

Checked and confirmed unavailable/not owned as of 2026-09-16: `twelve10.com` (parked for sale,
Spaceship), `twelveten.com` (Cloudflare), `twelvetenwellness.com` (Squarespace, redirects to an
unrelated company). `the10wellness.com` sits on a GoDaddy parking page — verify in the GoDaddy
account whether it belongs to us.

If a dedicated domain is bought later (`twelvetencompliance.com` was unregistered as of
2026-09-16, ~$12/yr), the switch is one find-and-replace across `site/`:
`compliance.thelittlethingscollection.com` -> the new domain. Four files contain it:
`index.html`, `selfcheck.html`, `florida-adrd-training-requirements.html`, `sitemap.xml`,
`robots.txt`.

## 2. Host it free

Pick one. All have free tiers that cover this site.

- **Cloudflare Pages** — best fit here. Connect the repo, set the build output directory to `site`,
  no build command. Then add `compliance.thelittlethingscollection.com` as a custom domain.
- **Netlify** — drag the `site/` folder onto app.netlify.com/drop. Then
  Site settings -> Domain management -> add the subdomain.
- **Vercel** — same idea; set the root directory to `site`.

Then at Namecheap, add one DNS record pointing `compliance` at the host:
a `CNAME` for host `compliance` -> the target the host gives you. The host will show the exact value.

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
the mailto links across all three pages). It works, so this is not a blocker. Once the domain is
settled, `hello@` forwarding is cheap at the registrar and reads better to agency buyers.

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

- `www.twelveten.example` placeholder replaced in all 5 files
- `[MAILING ADDRESS]` visible placeholder replaced with a commented gate in all 3 pages
- `sitemap.xml` `lastmod` bumped to 2026-09-16
- Stale "buy a domain" step removed — the domain was already owned
