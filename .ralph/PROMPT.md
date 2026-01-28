# Champs Home Service Website Build

## Project Overview
Build a professional, static website for Champs Home Service - a window cleaning company in Bend, Oregon. The site should generate quote requests and drive phone calls.

## Tech Stack
- **Framework:** Astro
- **Styling:** Tailwind CSS
- **Output:** Static HTML (no client-side JavaScript)
- **Hosting:** Netlify (deploy from GitHub)

## Design System

### Colors
| Color | Hex | Usage |
|-------|-----|-------|
| Forest Green | #1a3a2f | Primary - logo, headings, buttons, footer |
| Warm White | #fdfbf7 | Backgrounds |
| Gold | #b8860b | Accent - phone number, secondary buttons, CTAs |
| Muted Green | #5c6a62 | Nav links, body text |
| Cream Border | #e8e4dc | Borders, dividers |

### Typography
- **Font:** Inter (with system font fallback)
- **Headings:** 700 weight, tight letter-spacing
- **Body:** 400-500 weight

### Style
- Clean and polished
- Minimal and professional
- Warm but not overly friendly
- Subtle hover effects on buttons/cards

## Pages to Build

### 1. Home Page
- **Hero Section:**
  - Headline: "The Difference Is Clear."
  - Subhead: "Bend's trusted window cleaning experts"
  - CTA buttons: "Get a Free Quote" (primary), "Call Us Today" (secondary)
- **Services Overview:** 3-card grid (Residential, Commercial, Vacation Rentals)
- **Testimonials snippet** (placeholder for now)
- **CTA Section:** "Ready for Cleaner Windows?"

### 2. Services Page
- Detailed service descriptions
- Residential window cleaning
- Commercial window cleaning
- What's included in each service

### 3. About Page
- Brief company intro
- "Locally owned" messaging
- Keep simple (no team photos available)

### 4. Gallery Page
- Placeholder page for now
- Will add before/after photos later
- Simple grid layout ready for images

### 5. Contact Page
- Phone number: (541) 420-8350 (prominent, click-to-call)
- Email: isaac@champshomeservice.com
- Service area: "Bend and surrounding areas"
- Embedded Jobber quote form

### 6. Quote Request Page (optional - can be combined with Contact)
- Embedded Jobber form

## Jobber Form Embed Code
```html
<div id="c0a4b306-8234-4c61-bcda-5fa2e681c849-1485602"></div>
<link rel="stylesheet" href="https://d3ey4dbjkt2f6s.cloudfront.net/assets/external/work_request_embed.css" media="screen" />
<script src="https://d3ey4dbjkt2f6s.cloudfront.net/assets/static_link/work_request_embed_snippet.js" clienthub_id="c0a4b306-8234-4c61-bcda-5fa2e681c849-1485602" form_url="https://clienthub.getjobber.com/client_hubs/c0a4b306-8234-4c61-bcda-5fa2e681c849/public/work_request/embedded_work_request_form?form_id=1485602"></script>
```

## Global Components

### Header
- Logo: "Champs Home Service" (text for now)
- Navigation: Home, Services, About, Gallery, Contact
- Phone number in gold (click-to-call on mobile)
- Sticky on scroll (optional)

### Footer
- Business name
- Location: Bend, Oregon
- Phone number
- Copyright

## Technical Requirements
- Mobile-responsive (mobile-first approach)
- Fast load times (< 3 seconds)
- SSL via Netlify
- SEO basics (meta titles, descriptions per page)
- Google Analytics ready (add placeholder)

## File Structure
```
champs-home-service/
├── src/
│   ├── components/
│   │   ├── Header.astro
│   │   ├── Footer.astro
│   │   ├── ServiceCard.astro
│   │   └── Button.astro
│   ├── layouts/
│   │   └── BaseLayout.astro
│   └── pages/
│       ├── index.astro
│       ├── services.astro
│       ├── about.astro
│       ├── gallery.astro
│       └── contact.astro
├── public/
│   └── (images, favicon)
├── astro.config.mjs
├── tailwind.config.mjs
└── package.json
```

## Success Criteria
1. All 5 pages render correctly
2. Jobber form embeds and functions
3. Phone number is click-to-call on mobile
4. Site is mobile-responsive
5. Colors match the design system
6. `npm run build` succeeds with no errors
7. Site deploys to Netlify

## Notes
- No photos available yet - use color blocks/placeholders
- No testimonials yet - create placeholder section
- Keep it simple - can enhance later
