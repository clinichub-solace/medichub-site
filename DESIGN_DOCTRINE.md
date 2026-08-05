# MedicHub Design Doctrine
*The law of the medichub.us website. Written by Namu, approved by Boss. 2026-08-04.*

## What MedicHub Is
**MedicHub — Unified Practice Infrastructure.** One platform where independent
clinics run everything: EHR, scheduling, billing, imaging, comms, revenue ops,
and growth. Built by clinic operators, not by a software vendor guessing.
The deeper thesis: the **Relationship Model** — software is the entry point,
a circle of services (billing support, supplies, referrals, payments) is the
moat. Gravity, not walls: *"We will never forbid anyone from getting services
elsewhere."* The product wins by being genuinely better, not by lock-in.

## Voice
- Confident, calm, direct. No hype words ("revolutionary", "game-changing", "AI-powered magic").
- Speak operator-to-operator: written by people who run clinics.
- Bilingual-ready mindset (English first; Spanish will follow — write copy that translates cleanly).
- Short sentences. Concrete claims. If a claim can't be defended in a demo, cut it.

## Visual Law
**Palette (from the brand board — do not invent colors):**
- Deep navy `#1B2C5A` (primary), darker navy `#162648` (backgrounds)
- Gold `#D4AC47` (accent — CTAs, highlights; use sparingly, it's jewelry not paint)
- Ice `#F5F7FB` / `#F7F9FD` (light surfaces, text on dark)
- Muted blue-grays `#A7B4D0`, `#8FA0C2` (secondary text, borders)

**Typography:** `Inter` (body), `Inter Display` or Inter tight-tracking (headlines).
Fallbacks: 'Segoe UI', 'Helvetica Neue', Arial, sans-serif. Load via Google Fonts
or self-host. Headlines: semibold/bold, generous letter-spacing on small caps labels.

**Style: dark navy glassmorphism** — same language as the product UI:
- Dark navy gradient backgrounds, frosted-glass cards (`backdrop-filter: blur`,
  translucent white borders at ~8-12% opacity), soft shadows
- Gold used for exactly: primary CTA, key stat highlights, small accent lines
- Generous whitespace. No clutter. Elegance = restraint.
- Subtle motion only: fade/slide on scroll, gentle hover lifts. Nothing bouncy.

**Assets:** everything in `brand/` — `medichub_logo_light.svg` (for dark bg),
`medichub_logo_dark.svg` (for light bg), icons, brand board. NEVER redraw or
recolor the logo. NEVER stretch. Clear space around logo ≥ its icon width.

## Site Structure (v1 — single elegant landing, expandable)
1. **Hero** — logo, one-line promise, subline, gold CTA ("Request a demo"), product visual
2. **The Problem** — independent clinics juggle 6+ disconnected systems
3. **The Platform** — module grid: Clinical, Scheduling, Billing & Revenue, Imaging, Comms, Growth
4. **The Relationship Model** — why MedicHub is a partner, not a vendor
5. **Built by operators** — credibility, the origin story (a real clinic, real workflows)
6. **CTA + footer** — demo request, contact, © MedicHub, medichub.us

## Engineering Law
- Static site: semantic HTML + modern CSS + minimal vanilla JS. **No frameworks** for v1.
- Single repo: `~/Projects/medichub-site`. Entry: `index.html`. Assets under `brand/` and `assets/`.
- Mobile-first responsive. Lighthouse ≥ 90 across the board. Fast: no bloat, optimized images.
- Accessible: contrast AA (test gold-on-navy for text sizes), alt text, focus states.
- SEO basics: title, meta description, OG tags (og:image from brand board), favicon (`medichub_app_icon`).
- No trackers/analytics in v1. No forms that send data anywhere yet — CTA can be `mailto:` for now.
- The word "ClinicHub" must never appear. The product is **MedicHub**. Domain: **medichub.us**.

## Future (design for it, don't build it yet)
- `app.medichub.us` will host the product — the site's "Sign in" link will point there
- Spanish toggle; per-specialty *Hub pages (the umbrella grows)
