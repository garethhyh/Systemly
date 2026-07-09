# Systemly Website

A 3-page static website for **Systemly** — an AI assistant that routes business questions (IT, HR, Billing, Sales) to a verified answer or the right person.

Built for the C240 AI in Action final assessment, Republic Polytechnic — Team "Princess and the rest".

## Pages

| Page | File |
|---|---|
| Home | `index.html` |
| Contact Us | `contact.html` |
| Locate Us | `locate.html` |

## Structure

```
systemly-website/
├── index.html        # Home
├── contact.html       # Contact Us
├── locate.html         # Locate Us
├── css/
│   └── style.css      # Design tokens + all component styles
├── js/
│   └── script.js       # Nav toggle + scroll-reveal
└── assets/
    └── logo.png         # Systemly logo
```

No build step, no dependencies, no backend. Pure HTML/CSS/JS — just open `index.html` in a browser, or serve the folder with any static host.

## Running locally

```bash
# from inside the systemly-website folder
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploying

This is a static site, so it works as-is on GitHub Pages, Netlify, Vercel, or any static host.

**GitHub Pages:**
1. Push this repo to GitHub.
2. Go to **Settings → Pages**.
3. Under "Build and deployment", set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`.
4. Your site will be live at `https://<username>.github.io/<repo-name>/`.

## Notes

- The contact form on `contact.html` opens the visitor's email client via `mailto:` — there's no backend, so nothing is stored or sent automatically.
- The map on `locate.html` is a Google Maps embed (no API key required).
- Fonts (Space Grotesk, IBM Plex Sans, IBM Plex Mono) load from Google Fonts, so an internet connection is needed to see the intended typography.
