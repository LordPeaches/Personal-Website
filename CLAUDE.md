# CLAUDE.md — Personal Website (Alex Hughes)

## Project Overview

Static HTML/CSS/JS personal portfolio website for Alex Hughes, a mechanical/hardware engineer based in Austin, Texas. Hosted on Cloudflare Pages at [AlexDHughes.com](https://www.AlexDHughes.com).

## Repository Structure

```
/
├── public/                  # All website files (deployed root)
│   ├── index.html           # Main portfolio page
│   ├── assets/              # CSS, JS, images, vendor libs
│   │   ├── css/style.css    # Primary custom stylesheet
│   │   ├── img/             # Images (profile, hero, project photos)
│   │   ├── js/main.js       # Custom JS
│   │   └── vendor/          # Bootstrap, AOS, Swiper, Boxicons, etc.
│   ├── favicon_package_v0.16/  # Favicon set
│   ├── robots.txt
│   └── *.html               # Individual project detail pages (one per portfolio item)
├── Resume - Alex Hughes - 2 Pages.docx
├── .gitignore
└── CLAUDE.md
```

## Portfolio Project Pages

Each file in `public/` (besides `index.html`) is a standalone project detail page:

| File | Project |
|------|---------|
| `Firefly Aerospace.html` | Firefly Aerospace — Miranda engine design |
| `BeltPrinter.html` | Belt Printer project |
| `Candles.html` | Candles project |
| `FRC1895.html` | FRC Team 1895 |
| `FRC612.html` | FRC Team 612 |
| `FRC6800.html` | FRC Team 6800 |
| `HypernovaSolar.html` | Hypernova Solar |
| `MasonEntrepreneurshipClub.html` | Mason Entrepreneurship Club |
| `StealthBot.html` | StealthBot |
| `ZorseCode.html` | ZorseCode |

## Tech Stack

- **Framework**: Plain HTML/CSS/JS (no build step)
- **CSS/UI**: Bootstrap 5, Bootstrap Icons, Boxicons, AOS (scroll animations), Swiper (carousels), GLightbox
- **Fonts**: Space Grotesk, JetBrains Mono (Google Fonts)
- **Analytics**: Google Analytics (G-ZEEYVT5GZX)
- **Hosting**: Cloudflare Pages
- **Template base**: BootstrapMade Portfolio v3.0.0, heavily customized

## Development Notes

- **No build process** — edit HTML/CSS/JS files directly; changes are live on push.
- All pages share the same vendor assets via relative paths from `public/`.
- Project detail pages follow the same header/nav/footer structure as `index.html`.
- The `.gitignore` is configured for Firebase but hosting has moved to Cloudflare Pages.

## Key Contact / Identity Info

- **Name**: Alexander Hughes
- **Email**: AlexHughesNOVA@gmail.com
- **LinkedIn**: AlexHughesNOVA
- **Location**: Austin, Texas
- **Background**: Mechanical/hardware engineer, 3+ years aerospace propulsion at Firefly Aerospace (Miranda 230,000 lbf main engine program)
- **Education**: B.S. Bioengineering

## Common Tasks

- **Update content**: Edit the relevant section in `public/index.html` (About, Skills, Resume, Portfolio, Contact sections are clearly commented).
- **Add a portfolio project**: Create a new `public/ProjectName.html` modeled after an existing project page, then add a card to the `#portfolio` section in `index.html`.
- **Update styles**: Edit `public/assets/css/style.css`.
- **Deploy**: Push to `main` — Cloudflare Pages deploys automatically from the `public/` directory.
