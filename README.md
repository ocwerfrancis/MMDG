# Mary Mother of Divine Grace (MMDG) — Shrine Website

A multi-page website for the Mary Mother of Divine Grace Shrine, built with plain HTML, CSS, and vanilla JavaScript (no frameworks or build tools required). Deployed on Cloudflare Workers: https://mmdg.ocwerfrancis.workers.dev/

## Project Structure

```
MMDG/
├── index.html          # Homepage — hero slideshow, Mass Programs, Marian Apparitions, Rosary Meditations, footer
├── about.html           # About the Parish — history and Christian communities
├── devotions.html       # Devotions — Rosary/Novena, Adoration, First Saturday, Prayer Intentions
├── donate.html           # Projects & Donation — account details and project funding table
├── rector.html            # Rector page — header, hero section (in progress)
├── style.css               # Single shared stylesheet for all pages
└── images/                  # Site images (hero photos, slideshow images, apparition/devotion photos, etc.)
```

## Pages

- **Home (`index.html`)** — Fixed navy header with hamburger menu on mobile, full-screen image slideshow hero with office hours and a "Mass Programs" call-to-action, a Mass schedule table (Sunday/Weekly/Thursday programs), a hover-animated "Marian Apparitions" card grid, a tabbed "Rosary Meditations" section (Joyful/Sorrowful/Glorious/Luminous), and the site footer.
- **About (`about.html`)** — Shrine history and parish structure, presented in a two-image + text card layout on a cream background.
- **Devotions (`devotions.html`)** — Card grid of ongoing shrine devotions, each with an image, title, and description.
- **Donate (`donate.html`)** — Bank/Momo account details plus a table of current shrine projects and funding amounts, alongside a shrine photo.
- **Rector (`rector.html`)** — Header and hero section added; content still in progress.

## Design System

- **Colors:** Navy `#003262` (header, footers, buttons), Cream `#FFFFF0` (page background), white cards with soft navy-tinted shadows.
- **Fonts:** Montserrat (body/UI text), Roboto Slab (headings), imported via Google Fonts.
- **Components reused across pages:** fixed header/nav with mobile hamburger menu, `.donate`-style two-column card layout (About/Donate), card grids (Devotions/Apparitions), and a shared footer with contact info and quick links.

## Key Interactive Features

- **Hero slideshow** — auto-rotating background images on the homepage, implemented with CSS opacity transitions and a small JS interval loop.
- **Mobile navigation** — hamburger icon toggles a slide-in menu via a hidden checkbox (`#menu-toggler`) and the CSS `:checked` selector — no JS required.
- **Marian Apparitions hover cards** — captions expand and fade in on hover, collapse when the mouse leaves.
- **Rosary mystery tabs** — JavaScript toggles an `active` class to switch between the four mystery sets without reloading the page.

## Notes for Future Work

Pending real data from stakeholders — the following are known placeholders/issues to revisit once that information is available:

- **Footer contact info** — office address, phone number, and email in the site footer are still placeholders.
- **Footer "Important Links"** — currently only lists Home and About Us; needs Devotions, Programs, Rector, and Donate added to match the main nav.
- **Marian Apparitions section** — the Medjugorje card is currently using the Guadalupe image file by mistake; needs its own image.
- **Donate page** — bank account, Momo merchant code, and project funding amounts are placeholders pending the shrine's actual figures.
- **Rector page (`rector.html`)** — header and hero are in place; body content still to be written.
- **About/Devotions** — some text and images are still placeholder content pending real shrine photography and confirmed copy.
