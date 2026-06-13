# Krishna Raj Yoga — Official Website

A production-ready, fully responsive website built for **Krishna Raj Yoga**, a yoga studio with two branches in Electronic City, Bengaluru. Built solo as a freelance project — from requirements gathering to deployment and SEO strategy.

🔗 **Live Site:** [krishnarajyoga.pages.dev](https://krishnarajyoga.pages.dev)

---

## Project Overview

Krishna Raj Yoga needed a modern web presence covering two studio branches, multiple wellness programs, class schedules, and a functional contact flow — with zero monthly hosting costs and fast load times for mobile-first users in Bengaluru.

**Key constraints tackled:**
- No backend or database — fully static, no ongoing server costs
- No external router library — custom SPA routing to keep the bundle lean
- SEO-optimised for both local Bengaluru search and international yoga audiences
- Deployed on Cloudflare's global CDN for sub-second load times

---

## Engineering Highlights

### Custom Hash-Based SPA Routing
Rather than pulling in React Router, I implemented a lightweight custom hash-based routing system. This keeps the bundle size minimal while still giving full SPA behaviour — no page reloads, smooth transitions, and Cloudflare Pages `_redirects` handles deep-link refresh correctly.

### IntersectionObserver Scroll Animations
Scroll-reveal animations built with the native `IntersectionObserver` API via a custom `useScrollReveal` hook — no animation library dependency. Performant and works reliably across all modern browsers.

### Zero-Cost Third-Party Integrations
- **Contact form** via Formspree — no backend needed
- **Branch maps** via Google Maps Embed API — no API key billing
- **WhatsApp floating CTA** — direct conversion path for mobile users

### SEO Strategy
- Semantic HTML structure with proper heading hierarchy
- Meta tags and Open Graph markup for social sharing
- Local SEO targeting: "yoga studio Electronic City Bengaluru", "yoga classes near me Bengaluru"
- International SEO: structured content for aerial yoga, sound bowl healing, and prenatal yoga searches
- Cloudflare Pages CDN ensures fast TTFB globally

---

## Pages

| Page | Description |
|------|-------------|
| Home | Hero section, class highlights, testimonials, WhatsApp CTA |
| About | Studio story and instructor profiles |
| Classes | Regular, Online, Kids, Senior Citizen, Special Needs, Aerial Yoga |
| Wellness | Sound Bowl Healing, Pre/Postnatal, Meditation, PET programs |
| Branches | Schedule tables, embedded Google Maps, contact info for both locations |

---

## Tech Stack

| Category | Technology |
|----------|------------|
| Frontend | React 19, TypeScript |
| Build Tool | Vite |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Routing | Custom hash-based SPA routing |
| Animations | IntersectionObserver API (custom hook) |
| Forms | Formspree |
| Maps | Google Maps Embed API |
| Deployment | Cloudflare Pages (global CDN) |
| Version Control | Git + GitHub |

---

## Project Structure

```
src/
├── components/
│   ├── Layout/         # Navbar, WhatsAppFloat
│   └── Features/       # ClassCard
├── pages/              # Home, About, Classes, Wellness, Branches
├── data/               # Class and wellness program data
├── hooks/              # useScrollReveal (IntersectionObserver)
├── types/              # TypeScript interfaces
└── styles/             # Global CSS
public/
└── _redirects          # Cloudflare Pages SPA routing fix
```

---

## Running Locally

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

---

## Design Decisions

**Why Vite over CRA?** Faster cold starts and HMR during development; smaller production bundles.

**Why no CSS framework?** The client needed a custom visual identity — utility-first frameworks like Tailwind would have required more overriding than building fresh. Pure CSS custom properties gave full control with excellent browser support.

**Why Cloudflare Pages?** Free tier with global CDN, automatic HTTPS, and Git-based deployment. Zero DevOps overhead for a small studio client.

---

## About the Client

**Krishna Raj Yoga**
📍 Electronic City, Bengaluru (2 branches)
📞 +91 96931 68027
📸 [@krishnarajyoga](https://instagram.com/krishnarajyoga)

*Source code is private per client agreement.*
