<div align="center">

# 🏋️‍♂️ GYM-PLUS

### *Train Harder. Live Stronger.*

A sleek, fully responsive one-page fitness website — built with **pure HTML & CSS**, no JavaScript required.

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![FontAwesome](https://img.shields.io/badge/Font%20Awesome-528DD7?style=for-the-badge&logo=fontawesome&logoColor=white)
![Responsive](https://img.shields.io/badge/Responsive-Yes-success?style=for-the-badge)

![Status](https://img.shields.io/badge/status-in%20progress-yellow?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

</div>

---

## 🔥 About The Project

**Gym-Plus** is a modern, single-page fitness & gym website. It walks a visitor through everything they need — services, classes, trainers, real member results, a gallery, and a contact/booking form — in one smooth scroll.

> Notable technical detail: the mobile nav menu **and** the light/dark accent-color toggle are both built with the pure-CSS `<input type="checkbox">` + `:checked` trick — no JavaScript file is used anywhere in the project.

---

## 🧭 Sections (in actual page order)

| # | Section (`id`) | What's inside |
|---|-----------------|----------------|
| 01 | `#Home` | Sticky navbar (logo, links, burger menu, theme switch) + hero with headline and CTA |
| 02 | `#Services` | 5 service cards (Strength, Cardio Fitness, Personal Training, Nutrition Plans, Locker Room) |
| 03 | `#FeedBack` | Stats row (412+ transformations, 4.9 rating, 97% goal-hit rate) + 3 "plate" testimonial cards |
| 04 | `#Classes` | 6 class cards (Strength Training, Bodybuilding, Cardio Blast, Functional Training, Personal Coaching, Boxing Fitness) |
| 05 | `#Trainers` | 4 trainer cards with animated star ratings, specialty tags & social icons |
| 06 | `#Gallery` | 7-image mosaic grid (CSS Grid, spanning cells) |
| 07 | `#Contact_us` | Membership signup form (name, phone, email, plan) + embedded Google Map |
| — | `footer` | Copyright + credit line |

---

## 🎨 Design System

**Colors** (defined as CSS custom properties inside `main`, in `global.css`):

| Variable | Value | Used for |
|---|---|---|
| `--primary-color` | `#f5f5f5` | Light backgrounds / form panel |
| `--text-color` | `#e0dddd` | Body text on dark surfaces |
| `--ink` | `#3b2e34` | Headings / dark UI text (feedback section, footer) |
| `--muted` | `#6e6e6e` | Secondary/caption text |
| `--red` | `#e31e1e` | Primary accent (borders, buttons, highlights) |
| `--red-dark` | `#a81212` | Accent gradient / hover depth |
| `--red-border` | `rgba(227,30,30,.45)` | Soft borders & glows |
| `--line` | `#e7e2dc` | Dividers |

**🌗 Built-in theme switch:** toggling the `#themeColor` checkbox in the navbar swaps `--red` / `--red-dark` / `--red-border` to a **blue** variant across the entire site — done purely with the CSS selector `#themeColor:checked + main { ... }`.

**🔤 Typography** *(self-hosted via `@font-face` in `fonts.css`, not a Google Fonts CDN link)*:

| Role | Font |
|------|------|
| Headings (`h1`–`h6`) | `Sora` |
| Body text | `Roboto` |

**🧩 Icons:** [Font Awesome](https://fontawesome.com/) (loaded locally from `css/all.min.css`)

---

## 📱 Fully Responsive

Handled through a dedicated stylesheet (`index.responsive.css`) with **6 breakpoints**, from full desktop down to small mobile:

`> 1600px` → `1400–1600px` → `1300–1400px` → `990–1300px` → `765–990px` → `573–765px` → `368–573px` → `< 368px`

Each breakpoint individually adjusts the navbar, service grid, class cards, trainer cards, gallery grid, feedback grid, and the contact form/map layout.

---

## 🗂️ Actual Project Structure

```
Gym-Plus/
│
├── index.html
│
├── css/
│   ├── all.min.css          → Font Awesome
│   ├── fonts.css           → Self-hosted Roboto & Sora @font-face rules
│   ├── animations.css       → @keyframes (light, rail-scroll, ...)
│   ├── global.css           → Root variables, typography, buttons, shared UI
│   ├── index.css            → Section-by-section styles (header, services, classes,
│   │                           trainers, gallery, feedback, contact, footer)
│   └── index.responsive.css → All media queries (responsive breakpoints)
│
├── images/
│   ├── logo.svg
│   ├── favicon.svg
│   ├── header.png
│   ├── counters_bg.png
│   ├── serviceImgs/         → dumbbell.gif, cardio.gif, personal.gif, tasks.gif, door.gif
│   ├── classes/              → class1.png ... class6.png
│   ├── trainers/              → trainer1.png ... trainer4.png
│   └── gallery/               → images_1.png ... images_7.png
│
└── README.md
```

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/your-username/gym-plus.git

# 2. Move into the project folder
cd gym-plus

# 3. Open index.html in your browser
# (or use the VS Code "Live Server" extension for auto-reload)
```

No build tools, no `npm install`, no JavaScript. Just open `index.html`. ⚡

---

## 🛠️ Built With

- **HTML5** — Semantic sections with anchor-linked navigation
- **CSS3** — Flexbox, Grid, custom properties (`:root` / scoped variables), `@keyframes`, `backdrop-filter`, checkbox-driven interactivity
- **Font Awesome** — Star ratings, social icons, arrows
- **Self-hosted Web Fonts** — Sora (headings) & Roboto (body)

---

## ✅ Known Issues / TODO

- [ ] The embedded Google Map in `#Contact_us` currently points to **Canada** — update the `iframe` `src` with the real gym location's coordinates.
- [ ] Replace placeholder `href="#"` / empty social links (`<a href="">`) in the trainer cards with real profile URLs.
- [ ] Replace `REPLACE-WITH-YOUR-DOMAIN.com` placeholders in the `<head>` meta tags (canonical, `og:url`, `og:image`, `twitter:image`) once the site is deployed.
- [ ] Add real screenshots to this README once the visual design is finalized.

---

## 📬 Contact

**Project by:** SemiCode Team
📧 your-email@example.com
🔗 [LinkedIn](#) · [GitHub](#) · [Portfolio](#)

---

<div align="center">

### 💥 Train. Transform. Repeat. 💥

</div>