# LEADFUSE Site & CRM Launch Funnel

The live funnel for the Site & CRM Launch offer. 7 pages, static, no database.

## Pages
- `/` (index.html) — P1, the VSL page. Wistia VSL + live Typeform (01KZ4T861D9T6KH7PBQK43RW4J).
- `/book.html` — P2A, booking. Calendar embed: go.leadfuse.co/widget/booking/UxgxhRPbXkvlvV2Vxbwy. Auto-redirects to /confirmed.html after a booking.
- `/book-red.html` — P2B, disqualification (red scores land here).
- `/confirmed.html` — P3, booking confirmation (2 steps; breakout videos return later).
- `/terms-of-use.html`, `/privacy-policy.html`, `/earnings-disclaimer.html` — legal. ATTORNEY REVIEW BEFORE PUBLISH.

## What's inside
- `assets/` — logos, favicon, Vincent's app screenshot, Slack proof screenshots.
- `_ds/` — the LEADFUSE design system (fonts, colors, components). Pages need it. Don't delete.
- `support.js`, `image-slot.js` — page runtime. Don't delete.
- `package.json` — tells Railway how to serve the site.

## Embeds (all load from their own servers, nothing to configure)
- VSL video: Wistia media 6tv1ltftf3 (on / and /confirmed.html)
- Qualification form: Typeform 01KZ4T861D9T6KH7PBQK43RW4J (on /)
- Calendar: LEADFUSE App booking widget UxgxhRPbXkvlvV2Vxbwy (on /book.html)
- Testimonial videos: Wistia (on / and /book.html)

## Go live (see chat for the step-by-step)
GitHub repo -> Railway "Deploy from GitHub repo" -> Generate Domain -> add custom subdomain + CNAME in DNS.
