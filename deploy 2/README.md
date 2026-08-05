# LEADFUSE Site & CRM Launch Funnel

The live funnel for the Site & CRM Launch offer. 7 pages, static, no database.

## Pages
- `/` (index.html) — P1, the VSL page. Wistia VSL + live Typeform (01KZ4T861D9T6KH7PBQK43RW4J).
- `/book` — P2A, booking. Calendar embed: go.leadfuse.co/widget/booking/UxgxhRPbXkvlvV2Vxbwy. Auto-redirects to /confirmed after a booking.
- `/not-ready` — P2B, disqualification (red scores land here).
- `/confirmed` — P3, booking confirmation (2 steps; breakout videos return later).
- `/terms-of-use`, `/privacy-policy`, `/earnings-disclaimer` — legal. ATTORNEY REVIEW BEFORE PUBLISH.

Each page is a folder with an index.html inside, so URLs have no .html. Asset links are absolute (/assets, /_ds).

## What's inside
- `assets/` — logos, favicon, Vincent's app screenshot, Slack proof screenshots.
- `_ds/` — the LEADFUSE design system (fonts, colors, components). Pages need it. Don't delete.
- `support.js`, `image-slot.js` — page runtime. Don't delete.

## Embeds (all load from their own servers, nothing to configure)
- VSL video: Wistia media 6tv1ltftf3 (on / and /confirmed)
- Qualification form: Typeform 01KZ4T861D9T6KH7PBQK43RW4J (on /)
- Calendar: LEADFUSE App booking widget UxgxhRPbXkvlvV2Vxbwy (on /book)
- Testimonial videos: Wistia (on / and /book)

## Go live (see chat for the step-by-step)
Pure static site: Railway auto-detects index.html and serves it (no package.json needed). GitHub repo -> Railway "Deploy from GitHub repo" -> set Root Directory to /deploy -> Generate Domain -> add custom subdomain + CNAME in DNS.
