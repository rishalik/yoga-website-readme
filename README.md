# Krishna Raj Yoga — Official Website

A fully responsive, production-ready website built for **Krishna Raj Yoga**, a yoga studio based in Electronic City, Bengaluru. The site covers two studio branches, online classes, wellness programs, class schedules, branch maps, and a contact form.

🔗 **Live:** [krishnarajyoga.pages.dev](https://krishnarajyoga.pages.dev) <!-- update with your actual URL -->

---

## Features

- Multi-page SPA with custom hash-based routing (no external router library)
- Responsive design — mobile, tablet, and desktop
- Animated scroll-reveal using IntersectionObserver API
- Interactive branch tabs with embedded Google Maps (no API key required)
- Contact form powered by Formspree
- WhatsApp floating CTA button
- Sticky navbar with transparent-to-solid scroll transition
- Full-screen mobile navigation drawer with social links
- Deployed on Cloudflare Pages with global CDN

## Pages

| Page | Description |
|---|---|
| Home | Hero section, class highlights, testimonials, contact |
| About | Studio story and instructor profiles |
| Classes | Regular, Online, Kids, Senior Citizen, Special Needs, Aerial Yoga |
| Wellness | Sound Bowl Healing, Pre-Postnatal, Meditation, PET programs |
| Branches | Schedule tables, Google Maps, and contact info for both studio locations |

## Tech Stack

| Category | Technology |
|---|---|
| Frontend | React 19, TypeScript |
| Build Tool | Vite |
| Styling | CSS3 (custom properties, grid, flexbox) |
| Routing | Custom hash-based SPA routing |
| Forms | Formspree |
| Maps | Google Maps Embed API |
| Deployment | Cloudflare Pages |
| Version Control | Git + GitHub |

## Getting Started

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

## Project Structure

```
src/
├── components/
│   ├── Layout/         # Navbar, WhatsAppFloat
│   └── Features/       # ClassCard
├── pages/              # Home, About, Classes, Wellness, Branches
├── data/               # Class and wellness program data
├── hooks/              # useScrollReveal
├── types/              # TypeScript interfaces
└── styles/             # Global CSS
public/
└── _redirects          # Cloudflare Pages SPA routing
```

## Contact

**Krishna Raj Yoga**  
📞 +91 96931 68027  
📍 Electronic City, Bengaluru  
📸 [@krishnarajyoga](https://instagram.com/krishnarajyoga)
