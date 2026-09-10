# Holiday Elf — Listing Images and Restyle Decision (2026-09-08)

Canonical product: Product Factory item 12825906007. All files referenced here are attached to that item.

## What exists
- Five customer PDFs (v3.3, 108 pages, plain cream text layout).
- Five listing images from 09-04 (v1) plus the 09-08 set: hero v2 and four new slots (assets 3232514015, 3232514173, 3232514226, 3232514267, 3232514308). Read-back hashes verified.
- v3.7 hardcover (64 pages) and reset-notes (16 pages) in the founder-approved illustrated "heirloom Christmas" look. The hardcover embeds 10 scene illustrations at 1254 px.

## Founder feedback 09-08
"Not aesthetically pleasing, looks like a form, not a fun Christmas thing."

## Diagnosis
The listing images are honest pictures of plain pages. The cause is the customer PDFs, which were never restyled when v3.7 was approved. The fix is upstream: rebuild the five digital PDFs in the v3.7 look, then regenerate listing images from the new pages.

## Restyle proof of direction
Three sample story pages (Day 1, 12, 24) and one hero mockup were built using only the approved hardcover scene art plus the existing story text. No new artwork was generated. Samples are marked "direction only" and are not deliverables.

## Recommended build (v3.8 digital)
1. Story + letters PDF: full-bleed scene per day drawn from the 10 approved scenes, parchment card sized to content.
2. Parent setup cards and Command Center: parchment card on a soft warm background, no full-bleed art (these are working documents).
3. Child missions: illustrated header band, plenty of white space for drawing.
4. Low-ink props: unchanged.
5. Add a "low-ink story" variant so the illustrated file does not cost a parent a full cartridge.
Then regenerate all nine listing images from the real pages and re-QA.

## Adult / parents party edition
Captured as Idea Inbox item 13001181395, QUEUED behind the family kit. Not a Cards Against Humanity clone: original name, original card design, PG-13 base with optional expansion, and a separate shop placement because of brand fit and Etsy mature-content rules. A milder "Parents' After-Hours" bonus deck inside the family kit is the brand-safe way to test the idea first.

## Update 2026-09-09 — v3.8 restyle delivered
Founder rejected the heirloom/parchment samples ("not eye-catching, reads like a form") and asked for the fun, trendy look that sells in the category, plus a parent deck.

Built and attached to Product Factory item 12825906007:
- Five customer PDFs rebuilt in the "Candy Cane Pop" system (stripe borders, red/green/white/mint/gold, Fredoka + Pacifico, elf cut-out character, day badges, 24-spark progress strip). Text is the exact v3.3 content; automated check confirmed zero body blocks dropped.
- New bonus file: The Parents' After-Hours Deck, 36 PG cards (elf excuses, parent dares, confessions).
- Ten listing images, one per Etsy slot, built from the real new pages.
- Listing copy draft v2 in `holiday-elf-listing-draft-v2.md`.

Rejected directions kept for the record: v1/v2 plain-page images (09-04, 09-08) and the 09-08 heirloom samples.
Idea Inbox item 13001181395 (adult edition) updated: brand-safe bonus deck built; standalone adult SKU stays queued.

## Update 2026-09-10 — v4 "Groovy Little Sparks" full rebuild

Founder feedback on v3.8: "better but still not 100%... don't make it so 'AI' looking fun fonts... do research and see what people are doing and the vibe."

### Research (not a guess)
Searched current Etsy/design-trend coverage rather than picking a look. Finding: the documented 2026 Etsy aesthetic is "Play Haus" — dopamine-bright maximalism combined with a 70s groovy revival, an explicit rejection of safe rounded minimalism, with bold retro typography as the primary visual tool. Fredoka, Baloo, and Chewy (used in v3.8) are named as the generic AI/Canva-template tell buyers are moving away from.

### New system: Groovy Little Sparks
- Palette: muted retro (cranberry, pine, mustard, rust, cream) instead of stop-sign candy-cane red/green.
- Type: Righteous (70s disco-lettering retro-futuristic display) for headlines, Caveat (genuine handwritten script) for elf-note accents, Poppins for body.
- Shapes: sunburst medallion day badges, scalloped wavy card borders, wavy ribbon dividers, halftone dot texture, elf photo as a round die-cut sticker instead of a flat cutout.
- Approved from a 2-page preview (hero + one story day) before the full 24-day rebuild, to avoid a third blind full-cost iteration.

### Build
All five customer PDFs and the parent deck rebuilt in the new system from the same source text as v3.8 (same automated content-routing check, zero dropped blocks). One rendering bug found in QA — a background color band left a gap behind two-line titles on 6 of 10 listing images, clipping letter tops — fixed before upload.

New assets: 6 PDFs (114 pages) + 10 listing images (2000×2000), all attached to Product Factory item 12825906007, SHA-256 verified against a Monday read-back. Supersedes v3.8 (2026-09-09) and the original v1/v2 sets.

### Still open
Founder sign-off on v4 look-and-feel, then Executive Reviewer QA, then Router publish package at $18.
