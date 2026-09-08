# TwelveTen site — how to put this live

## 1. Buy a domain (~$12/yr)
Namecheap, Cloudflare, or Google-adjacent registrars all work.
Pick something like twelvetencompliance.com. Once chosen, do a
find-and-replace across all files: `www.twelveten.example` -> your real domain.

## 2. Host it free
Easiest paths, pick one:
- **Netlify**: drag this whole folder onto app.netlify.com/drop. Done.
  Then Settings -> Domain management -> add your domain.
- **Cloudflare Pages** or **Vercel**: same idea, free tier is plenty.
- **GitHub Pages**: push this folder to a repo, enable Pages.

## 3. Before ANY email campaign links here
- Replace [MAILING ADDRESS] in both footers with your real PO box / virtual mailbox.
- The email links point at twelvetenwellness@gmail.com. Consider
  hello@yourdomain.com once the domain exists (registrars offer cheap forwarding).

## 4. Wire up measurement (both free)
- **Google Search Console** (search.google.com/search-console):
  verify the domain, submit sitemap.xml. In ~2-4 weeks the Performance
  tab shows the EXACT queries people typed to find you, impressions,
  and clicks. This is the real "what are people searching" data.
- **Google Analytics 4** (analytics.google.com): create a property,
  paste its snippet into both pages just before </head>. Shows what
  visitors do once they arrive.

## 5. The self-check
The interactive self-check currently lives as a Claude artifact. Two options:
- Link to it from the site (works today), or
- Ask Claude to convert it into a selfcheck.html page in this folder
  so it lives on your own domain (better for SEO + analytics).

## What's here
- index.html                              — service/landing page
- florida-adrd-training-requirements.html — the SEO guide page (the ranking play)
- robots.txt, sitemap.xml                 — search engine plumbing
