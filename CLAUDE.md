# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Jekyll static site for the "Risk IT in Fire Dept." NSF-funded research project (risk-it.github.io). Uses the Minima theme with extensive custom styling. Deployed via GitHub Pages.

## Build & Development Commands

```bash
bundle install              # Install Ruby dependencies
bundle exec jekyll serve    # Local dev server (http://localhost:4000)
bundle exec jekyll build    # Build to _site/
docker-compose up           # Alternative: Docker-based dev server
```

## Architecture

- **Theme**: Minima with custom SCSS overrides in `assets/main.scss`
- **Font**: Inter (Google Fonts)
- **Pages**: `_pages/` directory, linked via `_config.yml` header_pages
- **Assets**: Images in `assets/imgs/`, logos in `assets/imgs/logo/`
- **Custom components**: `_includes/footer.html`, `_includes/module.html`

## Key Pages

- `_pages/frontpage.md` — Homepage (layout: default, no title shown)
- `_pages/about.md` — Detailed project description
- `_pages/partners.md` — Fire department partner cards (2x2 grid)
- `_pages/authors.md` — Team member cards
- `_pages/cscw2025workshop.md` — Workshop page (commented out of nav)

## Work History

### 2026-03-28: Site Redesign & Content Updates
- **Visual redesign**: Replaced default Minima styling with custom design using Inter font, red accent color (#c0392b), card-based layouts, and clean typography
- **Homepage**: Hero section with NSF project title, approach diagram with SVG icons (Understand -> Co-Design -> Evaluate), concise project overview. Removed "Home" from nav and page title
- **About page** (new): Detailed project description focused on Fire-based EMS, risk work definition, data-intensive challenges, and three research phases
- **Partners page**: Added 4 fire department partner cards in 2x2 grid -- Fairfax County Fire & Rescue, Columbus Division of Fire (Ohio), Fort Worth Fire Department, LA County Fire Department. Removed academic partners section (universities shown on Home/About instead)
- **Team page**: Converted to card grid layout with photos and role badges. Added Hiba Siraj (GMU) and Ruchita Mandhre (ASU). Reordered: Katie Pine, Yunan Chen, Myeong Lee, Mauricio Mejia, Melissa Mazmanian, Rachel Warren, Hiba Siraj, Ruchita Mandhre. Updated titles (Katie -> Associate Professor, Yunan -> Professor, Rachel/Ruchita -> Ph.D. Candidate)
- **Logos**: Updated GMU logo to 2024 version. Downloaded consistent horizontal wordmark logos for UCI, ASU. Downloaded fire department seals/emblems. Adjusted sizes for visual consistency across pages (NSF, ASU, GMU, UCI order)
- **Footer**: Removed site footer
- **Site title**: Changed to "Risk IT in Fire Dept."
- **Dependencies**: Updated Gemfile.lock to resolve vulnerabilities
