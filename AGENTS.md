# AGENTS.md — Khaled Mamdooh Portfolio

This is a **vanilla static website** (HTML + CSS + JS). No build tools, no package manager, no dev server.

## Commands
- **Preview**: Open `index.html` in a browser directly (double-click or `start index.html`)
- No lint, test, typecheck, or build commands exist

## Architecture
- `index.html` — single-page portfolio with sections: Home, About, Skills, Services, Work, Contact
- `style.css` — all styles (~700 lines); responsive via `@media (max-width: 1040px)`
- `script.js` — vanilla JS for: sticky header, mobile hamburger menu, scroll-to-top button, scroll-based reveal animations
- `images/` — static assets (background, photos, app screenshots, menu icons)

## Conventions
- Section IDs match nav anchors: `#main`, `#about`, `#skills`, `#services`, `#work`, `#contact`
- Scroll reveal uses `.reveal` class + `.active` toggled by JS on scroll
- JavaScript uses `classList.toggle` pattern; no framework or libraries
- CSS uses Poppins font from Google Fonts, Font Awesome 5.15.2 for icons
- Image paths are relative (`images/...`) — keep them in `images/`
- No backend; the contact form is static (no submit handler)
