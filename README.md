# Wide Awake Solar

**Empowering People. Transforming Energy.**

Official website for Wide Awake Solar — Ireland's solar panel installation company offering custom solar systems, battery storage, EV charging and infrared heating with SEAI grants handled in full.

🌐 [wideawakesolar.ie](https://wideawakesolar.ie)

---

## About the Site

Single-page HTML website, fully self-contained in one `index.html` file. No build tools, no dependencies, no framework — just drop it on a server and it works.

### Sections
- Hero
- Manifesto
- Stats
- About
- How It Works
- AI Bill Analyser
- 3D Solar Simulator
- Performance
- Services
- Pricing
- Testimonials
- FAQ
- Contact

---

## Features

- **3D Solar Simulator** — Three.js powered rooftop simulator with full solar physics, SEAI grant calculator (€1,800 + €300 EV), and real-time energy output modelling
- **Mobile 2D Simulator** — Canvas-based touch simulator on mobile (≤768px) replacing Three.js for performance
- **AI Bill Analyser** — Anthropic API powered tool that reads your electricity bill and calculates solar savings
- **Scroll animations** — 40 animated elements, `prefers-reduced-motion` respected
- **SEO ready** — Meta tags, Open Graph, Twitter Cards, structured data
- **Fully responsive** — Mobile-first design with custom mobile nav drawer
- **No external dependencies at runtime** — Three.js and Chart.js loaded via CDN with `defer`

---

## Tech Stack

| Layer | Detail |
|---|---|
| HTML/CSS/JS | Vanilla, single file |
| 3D | Three.js r128 |
| Charts | Chart.js 4.4.1 |
| Fonts | Fraunces, Plus Jakarta Sans, DM Mono (Google Fonts) |
| AI | Anthropic Claude API |
| Images | WebP (base64 embedded) |

---

## Deployment

This is a static single-page site. Deploy anywhere that serves HTML:

- **Netlify** — drag and drop `index.html` or connect this repo for auto-deploy
- **Cloudflare Pages** — connect repo, no build command needed
- **Vercel** — connect repo, framework = Other
- **Traditional hosting** — upload `index.html` to public root via FTP/SFTP

No build step required.

---

## Future Development

When moving to a multi-page structure:
- Extract base64 images to `/images/` folder
- Connect nav links between pages
- Add real form backend (Netlify Forms, Formspree, or custom)
- Replace placeholder Google Analytics ID
- Add real photography

---

## Brand

| | |
|---|---|
| Primary | `#1B9BD4` (Sky Blue) |
| Accent | `#F5A623` (Sun Yellow) |
| Green | `#2EAA4A` (Leaf) |
| Dark | `#1565C0` (Panel Blue) |

Fonts: **Fraunces** (display) · **Plus Jakarta Sans** (body) · **DM Mono** (labels)

---

Built by [SolarIreland](https://solarireland.ie)

---

## Pre-Launch Checklist

The following items need to be completed before going live:

### ✅ Done
- Favicon set to pill logo
- All images converted to WebP (83% size saving)
- Accessibility: aria-labels added to all form inputs and simulator controls
- SEO: meta tags, Open Graph, canonical URL, H1, viewport all set
- Scripts: Three.js and Chart.js deferred

### 🔲 Needs Dev / You
- **OG image** — upload a real 1200×630px image to `/og-image.jpg` on the server and update the meta tag. This is what shows when the link is shared on WhatsApp, LinkedIn etc.
- **Contact form** — form has no backend. Connect to Netlify Forms (free, one line of code if hosting on Netlify) or Formspree (free tier, works anywhere)
- **Google Analytics** — create a GA4 property at analytics.google.com, get your `G-XXXXXXXXXX` ID and replace the placeholder in the `<head>`
- **Images folder** — when deploying to a server, extract base64 images to an `/images/` folder and update `src` paths for better caching and performance
- **Real photography** — site currently uses placeholder/stock imagery. Replace with real Wide Awake Solar project photos

