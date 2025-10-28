# CEO Profile — Alexander Vance

Live demo: [https://sakshsky.com/demo/ceo/index.html](https://sakshsky.com/demo/ceo/index.html)
Repository: [https://github.com/sakshsky/ceo](https://github.com/sakshsky/ceo)

---

## Overview

A polished, dark-themed single-page **CEO/Profile** demo built using Tailwind CSS, GSAP, and a small amount of vanilla JavaScript. The design highlights a hero section, animated counters, skills, timeline, testimonials, and a contact form. It's ideal as a personal landing page or a portfolio piece for a founder/CEO.

## Key Features

* Responsive dark UI with gradient hero background and glassmorphism cards
* Tailwind CSS-based utility-first styling (via CDN)
* Smooth scroll navigation and sticky nav with scroll shadow
* Animated counters and skill bars (intersection observer)
* Testimonial carousel with auto-advance and navigation dots
* Flip-cards for leadership philosophy
* Simple particle/floating-shapes visual accents
* Light/dark mode toggle
* GSAP + ScrollTrigger scroll animations

## Tech Stack

* HTML5
* Tailwind CSS (CDN)
* Font Awesome (CDN)
* GSAP + ScrollTrigger (CDN)
* Minimal vanilla JavaScript (no framework)

## Folder structure (recommended)

```
ceo/
├─ index.html
├─ README.md
├─ assets/
│  ├─ images/
│  └─ icons/
└─ docs/
   └─ demo-notes.md
```

> The demo is currently a single `index.html` containing inline styles and scripts for ease of distribution.

## Installation / Local Development

1. Clone the repository:

```bash
git clone https://github.com/sakshsky/ceo.git
cd ceo
```

2. Open the demo locally (no build step required):

* Double-click `index.html` or
* Serve with a static server (recommended for consistent behavior):

```bash
# using Python 3
python -m http.server 8000
# visit http://localhost:8000
```

## Customization Guide

* **Text & Content**: Update the hero, about, experience, testimonials and footer content directly in `index.html`.
* **Colors & Theme**: Tailwind is used via CDN; change the `tailwind.config` object in the `<head>` to customize primary/secondary colors or font.
* **Animations**: GSAP animations are configured near the bottom of `index.html`. Tweak timing and triggers in the `gsap.fromTo` blocks.
* **Counters & Skills**: Modify `data-count` on `.stats-counter` and `data-width` on `.skill-progress` to change values.
* **Icons**: Font Awesome is used for icons. Replace class names (e.g., `fa-user-tie`) to change icons.

## Accessibility & Improvements (suggested)

* Add proper `aria-*` attributes and `label` associations for form controls.
* Replace purely decorative `<i>` icons with accessible alternatives (or add `aria-hidden="true"` and visible text for screen readers).
* Extract inline scripts and styles to separate files for maintainability.
* Add form handling (e.g., Netlify Forms, Formspree, or a simple server endpoint) to make the contact form functional.
* Optimize performance by self-hosting critical assets and switching to a Tailwind build step for production to purge unused styles.

## Deployment

The demo is already hosted at the provided URL. For GitHub Pages:

1. Push the repo to GitHub (if not already).
2. Enable GitHub Pages in repository settings and set the source to the `main` (or `gh-pages`) branch root.

## Credits

* Template and layout by Sakshsky (repository owner)
* Icons: Font Awesome
* Animations: GSAP
* Styling utilities: Tailwind CSS

## License

Add a license of your choice (e.g., MIT) — include a `LICENSE` file in the repository.

---

If you want, I can also:

* produce a compact `README.md` ready to paste into the repo root,
* create a `LICENSE` file (MIT) and example `CNAME` for the demo domain, or
* extract inline CSS/JS into separate `styles.css` / `app.js` files and update `index.html` accordingly.

Tell me which of those you want and I’ll generate them.
