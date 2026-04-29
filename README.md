# Jeff Omondi — Portfolio v2

A single-file, interactive portfolio for a Data Scientist & Machine Learning Engineer. Built with vanilla HTML, CSS, and JavaScript — no build step required.

---

## Overview

This portfolio presents Jeff Omondi's skills, projects, and workflow in a dark, sci-fi aesthetic with animated WebGL backgrounds, smooth scrolling, and interactive UI elements.

**File:** `jeff_omondi_portfolio_v2.html`  
**Type:** Single-page application (SPA), self-contained HTML file  
**Theme:** Void dark (`#020204`) with cyan (`#00f0ff`), violet (`#bd00ff`), and magenta (`#ff006e`) accents

---

## Features

- **Boot sequence** — Simulated terminal startup animation on load
- **WebGL background** — Animated particle/noise canvas rendered behind all content
- **Custom cursor** — Glow cursor that expands on hover and hides on touch devices
- **Smooth scrolling** — Powered by [Lenis](https://github.com/studio-freight/lenis)
- **Scroll animations** — GSAP + ScrollTrigger reveal effects on sections
- **3D tilt cards** — Project cards with mouse-tracking perspective and radial glow
- **Skill rings** — SVG circular progress indicators animated on scroll
- **Filterable project grid** — Filter projects by category (Anomaly, NLP, CV, etc.)
- **Project modals** — Click any project card to open a detail modal (problem, dataset, tech stack, methods, results, GitHub link)
- **Tech arsenal** — Filterable tag cloud of all tools and frameworks, organized by category
- **Data pipeline** — Alternating timeline layout showing Jeff's 7-step workflow
- **Terminal easter egg** — Press `` ` `` or `~` to open a full-screen simulated terminal with live command output
- **Magnetic buttons** — Navigation and CTA buttons subtly follow the cursor
- **Film grain overlay** — SVG noise texture layered over the page for texture
- **Mobile menu** — Full-screen slide-in nav for small screens
- **Responsive** — Layouts adapt from mobile to desktop; custom cursor disabled on touch devices

---

## Sections

| Section | ID | Description |
|---|---|---|
| Hero | `#hero` | Name, title, and call-to-action buttons |
| About | `#about` | Bio, years of experience, models deployed, datasets processed |
| Skills | `#skills` | 10 core skills with animated SVG ring indicators |
| Arsenal | `#tech` | Filterable tag cloud of 60+ technologies |
| Projects | `#projects` | 6 featured projects with modal detail views |
| Pipeline | `#workflow` | 7-step data science workflow timeline |
| Contact | `#contact` | Email, LinkedIn, GitHub links |

---

## Projects

| # | Title | Domain | Key Result |
|---|---|---|---|
| 1 | Real-Time Fraud Detection | Anomaly Detection / Financial | 95% precision, 50ms latency, 10K+ TPS |
| 2 | NLP Sentiment Analysis API | NLP / Social Media | 88% accuracy, 2K+ req/min, AWS auto-scaling |
| 3 | CV Inventory System | Computer Vision / Warehouse | 92% mAP, 80% reduction in counting time |
| 4 | Customer Churn Pipeline | Classification / Telecom | 89% accuracy, automated weekly retraining |
| 5 | Sales Forecasting Engine | Time Series / Retail | 8.5% MAPE, 35% reduction in stockouts |
| 6 | Recommendation Engine | Recommendation / E-commerce | +35% CTR, +28% conversion rate |

All project GitHub links point to `https://github.com/Omondi-je/`.

---

## Tech Stack (Portfolio itself)

| Dependency | Version | Purpose |
|---|---|---|
| [Tailwind CSS](https://tailwindcss.com) | CDN | Utility-class styling |
| [GSAP](https://gsap.com) | 3.12.5 | Scroll and entrance animations |
| [ScrollTrigger](https://gsap.com/docs/v3/Plugins/ScrollTrigger/) | 3.12.5 | GSAP scroll plugin |
| [Lenis](https://github.com/studio-freight/lenis) | 1.0.29 | Smooth scroll |
| [Google Fonts](https://fonts.google.com) | — | Orbitron, Rajdhani, Space Grotesk |

No npm, no bundler. Everything is loaded via CDN.

---

## Usage

Open the file directly in any modern browser:

```bash
open jeff_omondi_portfolio_v2.html
# or just double-click the file
```

No server, build step, or dependencies to install.

---

## Customisation

All content (skills, projects, workflow steps) is defined in a single `DATA` object at the top of the `<script>` block (around line 556). To update the portfolio:

1. Edit the `DATA.skills`, `DATA.projects`, or `DATA.workflow` arrays
2. Update contact links in the `#contact` section of the HTML
3. Replace the GitHub URLs in each project entry
4. Adjust color variables in `:root` (`--cyan`, `--violet`, `--magenta`, `--void`) for a different palette

---

## Browser Support

Requires a modern browser with support for:
- CSS `backdrop-filter`
- `mix-blend-mode`
- WebGL (canvas)
- ES Modules (`type="module"`)

Tested on Chrome, Edge, and Firefox. Safari may have minor `backdrop-filter` differences.

---

## Easter Egg

Press the backtick (`` ` ``) or tilde (`~`) key anywhere on the page to open a simulated terminal showing fake shell output — `whoami`, `ls`, `docker ps`, `kubectl`, `git log`, and more.# portfolio
