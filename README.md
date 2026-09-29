# Bright Concrete LLC — Homepage

A premium, redesigned homepage for **Bright Concrete LLC**, a family-owned concrete
contractor serving Central Maryland for 10+ years. Rebuilt from the existing site at
[brightconcretellcs.com](https://www.brightconcretellcs.com/), using the company's **real
logo, brand colors, project photos, and reviews**.

Built as a fast, dependency-free static site with a full-bleed **background video hero**.

**Live site:** _(GitHub Pages — see repo Settings → Pages)_

---

## Business details
- **Company:** Bright Concrete LLC
- **Owner:** Helder (owner/operator, on-site)
- **Phone:** 240-960-1928
- **License:** MHIC #162519 — Licensed, Bonded & Insured
- **Established:** 10+ years in business
- **Rating:** 5-star, 54 verified reviews
- **Hours:** Mon–Fri 7 AM – 5 PM · Sat–Sun closed
- **Tagline:** "Concrete contractors in Maryland trusted for work that lasts decades."
- **Service area:** Central Maryland & the Chesapeake corridor — Anne Arundel, Howard,
  Prince George's, Baltimore, Carroll & Queen Anne's counties.

## Services
Stamped & decorative concrete · Driveways · Patios · Walkways, sidewalks & steps · Pool
decks · Basketball courts · Repair, leveling & resurfacing · Retaining walls · Foundations,
slabs & footings · Flooring & polished concrete · Commercial concrete.

## Tech
- Static **HTML + CSS + vanilla JS** — no build step, no framework, no dependencies.
- Google Fonts (Archivo + Inter). Everything else is local.
- Accessible: semantic landmarks, single `<h1>`, keyboard nav, visible focus,
  `prefers-reduced-motion`, descriptive alt text.
- SEO: descriptive title/meta, Open Graph, and `GeneralContractor` JSON-LD with service
  areas, opening hours, and aggregate rating.

## Structure
```
index.html            # full homepage
css/styles.css        # design system + all sections + responsive
js/main.js            # sticky/transparent header, mobile menu, scroll reveals, form shell
assets/img/           # real logo + project photos + favicon
assets/video/         # hero background video + poster
```

## Design
**Bright brand palette** from the logo: **bright green `#33C414`** and **sun yellow
`#FFE500`** on a near-black `#0E1310`. Dark, transparent header (goes solid on scroll) so
the green/yellow logo pops; Archivo + Inter typography.

## Hero video
The hero uses a full-bleed, muted, looping background video (`assets/video/hero-720.mp4`,
~0.8 MB, 720p) from Pexels (free license), with `hero-poster.jpg` as the poster/fallback;
reduced-motion users get the still frame. It plays on both mobile and desktop. The
transparent nav overlays the video (header is `position: fixed`).

---

## Notes for the client
- **Logo, photos & reviews are real** — the header/footer use the actual Bright logo
  (auto-cropped from the original), every project image is a real Bright job from the
  current site, and the testimonials are real 5-star reviews. Swap or add photos by
  dropping files into `assets/img/`.
- **Estimate form** — front-end only; it does not submit anywhere yet. Wire it to email or
  a CRM (Formspree, Netlify Forms, GHL, etc.) to start capturing leads.
- Only substantiated facts are used (10+ years, MHIC #162519, 5-star/54 reviews, owner
  Helder, service area, hours) — no invented claims.

## Deploy (GitHub Pages)
Settings → Pages → Source: `main` / root. The site publishes at the Pages URL.
Local preview: open `index.html`, or run `python3 -m http.server` in the repo root.
