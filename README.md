# The Tech Agency — HTML & CSS Assignment

A responsive, multi-page static website for a fictional tech agency, built with semantic HTML5 and modern CSS (Flexbox, mobile-first). No frameworks, no JavaScript.

## Live Demo

**https://lorenzobude.github.io/HTMLCSSAssignment/**

Deployed with GitHub Pages from the `main` branch.

## Pages

| Page | File | Content |
|------|------|---------|
| Home | `index.html` | Hero with text + image, info cards, quote, CTA banner |
| About Us | `about.html` | Story, values cards, CTA |
| Services | `services.html` | Hero with `hgroup` + `figure/picture`, 9-item services grid (`ul > li`), consultation CTA |

## Features

- **Semantic HTML5:** `header`, `nav`, `main`, `section`, `hgroup`, `figure`/`picture`, `ul > li` for cards, `footer`
- **Responsive (mobile-first):** base `375px` → tablet `@media (min-width: 768px)` → desktop `@media (min-width: 1200px)`
- **CSS-only hamburger nav:** hidden `checkbox` + `label` toggle (`:checked ~ .nav-links`), hidden with `display: none` on tablet/desktop
- **Shared + per-page CSS:** `css/global.css` (fonts, nav, footer, containers) + `css/home.css`, `css/about.css`, `css/services.css`
- **Images:** WebP with JPG fallback via `<picture>`, `width`/`height` to avoid layout shift, `fetchpriority="high"` on hero, `loading="lazy"` below the fold
- **Icons:** Font Awesome 7 via CDN

## Project Structure

```
HTMLCSSAssignment/
├── index.html
├── about.html
├── services.html
├── css/
│   ├── global.css
│   ├── home.css
│   ├── about.css
│   └── services.css
├── images/
│   ├── hero-image.webp / hero-image.jpg
│   └── service-agency.jpg
└── README.md
```

## Run Locally

No build step — just open the file or serve the folder:

```bash
# option 1: open directly
start index.html

# option 2: local server (Python)
python -m http.server 5500
# then visit http://localhost:5500
```

## Tech

- HTML5
- CSS3 (Flexbox, media queries)
- Google Fonts (Roboto)
- Font Awesome icons
