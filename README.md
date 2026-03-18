<div align="center">

<br/>

# 🎙️ TechWave — Podcast Landing Page

**A sleek, dark-themed podcast website built with HTML, Tailwind CSS & custom CSS**

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Complete-brightgreen)]()

<br/>

> *A production-quality podcast landing page — dark aesthetic, glassmorphism cards, responsive navbar, featured episodes, host profile, and multi-platform footer links.*

<br/>

</div>

---

## 🌟 What is This?

**TechWave** is a fully responsive podcast website landing page for a fictional tech podcast. Built for **Programming Hero (Batch-13, Assignment 02)**, it demonstrates real-world front-end layout skills — multi-section page structure, custom CSS with Tailwind utility classes, glassmorphism UI, responsive mobile navigation, and a carefully crafted dark visual identity.

---

## ✨ Features at a Glance

| Feature | Description |
|---|---|
| 🌑 **Dark Theme** | Deep space aesthetic with purple/cyan/pink accents |
| 🪟 **Glassmorphism Cards** | Frosted-glass feature cards with custom CSS |
| 📐 **Bento Grid Layout** | Asymmetric CSS Grid for the "Why Choose" section |
| 📱 **Responsive Navbar** | Hamburger menu with smooth expand/collapse on mobile |
| 🎧 **Episodes Section** | Hoverable episode cards with play button overlays |
| 📊 **Stats Dashboard** | Animated stat counters — 150K+ listeners, 200+ episodes |
| 🎤 **Host Profile** | Bio section with social media icon links |
| 🔗 **Platform Footer** | Spotify, Apple Podcasts, YouTube, Twitter links |

---

## 🖥️ Page Structure

```
┌──────────────────────────────────────────────────────────┐
│  🎙️  TechWave         About  Episodes  Host  [Subscribe] │  ← Navbar
├──────────────────────────────────────────────────────────┤
│                                                          │
│              🎙  [ pulsing mic icon ]                    │  ← Hero Banner
│                     TechWave                             │
│       "Your daily dose of tech insights..."              │
│    [Listen on Spotify]   [Subscribe]                     │
├──────────────────────────────────────────────────────────┤
│  About    150K+ Listeners  200+ Episodes  4.9★  50+ Experts │ ← Stats
├──────────────────────────────────────────────────────────┤
│  Why Choose TechWave                                     │
│  ┌──────────────────────┬──────────────┐                 │
│  │ 🎧 Premium Audio     │ 📱 Mobile    │  ← Bento Grid  │
│  │    (tall card)       ├──────────────┤                 │
│  │                      │ 🌍 Community │                 │
│  ├──────────────────────┼──────────────┤                 │
│  │ 🎤 Exclusive         │ 📚 Resources │                 │
│  └──────────────────────┴──────────────┘                 │
├──────────────────────────────────────────────────────────┤
│  Featured Episodes  [ 3 hoverable cards with overlays ]  │
├──────────────────────────────────────────────────────────┤
│  Host: Alex Kumar  [ bio + social icons ]                │
├──────────────────────────────────────────────────────────┤
│  © TechWave  Spotify · Apple · YouTube · Twitter         │  ← Footer
└──────────────────────────────────────────────────────────┘
```

---

## 🎨 Design Highlights

### Glassmorphism Feature Cards
```css
.glass-card {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 1.25rem;
}
```

### Asymmetric Bento Grid
```css
/* 5 cards in a 2-column grid with varying row spans */
.features-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: repeat(3, auto);
  gap: 1.5rem;
}

.card-premium-audio        { grid-row: 1 / 3; }   /* spans 2 rows */
.card-exclusive-interviews { grid-row: 3; }
```

### Gradient CTA Button
```css
.gradient-btn {
  background: linear-gradient(135deg, #ec4899, #8b5cf6, #06b6d4);
  transition: opacity 0.2s ease;
}
.gradient-btn:hover { opacity: 0.88; }
```

### Mobile Hamburger Menu
```js
hamburger.addEventListener('click', () => {
  mobileMenu.style.maxHeight =
    mobileMenu.style.maxHeight === '0px' || !mobileMenu.style.maxHeight
      ? '300px'
      : '0px';
});
```

---

## 📁 Project Structure

```
TechWave/
│
├── index.html          ← Full page: navbar, hero, about, episodes, host, footer
│
└── styles/
    ├── style.css       ← Custom styles: glass cards, grid, animations, dark theme
    ├── microphone.png  ← Hero & features icon
    ├── headphone.png   ← Premium audio feature icon
    ├── device.png      ← Mobile friendly feature icon
    ├── location.png    ← Global community feature icon
    ├── resource.png    ← Rich resources feature icon
    ├── host.png        ← Alex Kumar host photo
    ├── group.png       ← Remote work episode thumbnail
    ├── linkedin.png    ← Social icon
    ├── x.png           ← Social icon
    ├── instagram.png   ← Social icon
    ├── youtube.png     ← Social icon
    ├── spotify.png     ← Footer platform icon
    ├── apple-podcast.png
    ├── youtube-podcast.png
    └── twitter.png
```

---

## 🚀 Getting Started

No build step. No install. Just open.

**Option 1 — Direct open:**
```bash
git clone https://github.com/Safin313-stack/Assingment-B13-A02-TechWave.git
open index.html
```

**Option 2 — Live Server (VS Code):**
1. Install [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer)
2. Right-click `index.html` → **Open with Live Server** ✅

---

## 🎨 Tech Stack

```
Frontend Only — No Build Tools Required
────────────────────────────────────────
  HTML5        →  Full page semantic structure
  Tailwind CSS →  Utility-first layout & spacing (CDN)
  CSS3         →  Custom glassmorphism, grid, animations
  JavaScript   →  Hamburger menu toggle only
  Unsplash     →  Episode thumbnail images
```

---

## 🎙️ Sections Overview

**Navbar** — Fixed top bar with logo, nav links, subscribe CTA, and a mobile-responsive hamburger toggle.

**Hero Banner** — Centred layout with animated pulsing mic icon, tagline, and dual CTA buttons (Spotify + Subscribe).

**About** — Podcast description with a 4-column stat grid: 150K+ listeners, 200+ episodes, 4.9★ rating, 50+ experts.

**Why Choose TechWave** — Asymmetric 2×3 bento grid of 5 glassmorphism cards covering audio quality, mobile experience, global community, exclusive interviews, and resources.

**Featured Episodes** — 3-column card grid with hover overlay effects and a play button on each episode thumbnail.

**Host** — Side-by-side bio section for Alex Kumar with social media links.

**Footer** — Podcast platform links (Spotify, Apple, YouTube, Twitter) and copyright.

---

## 👤 Developer

<div align="center">

**Saharia Hassan Safin**

[![GitHub](https://img.shields.io/badge/GitHub-Safin313--stack-181717?style=flat&logo=github)](https://github.com/Safin313-stack)

*Designing dark-mode interfaces one glass card at a time 🎙️*

</div>

---

## 📜 License

```
MIT License — Free to use, modify, and distribute.
© 2025 Saharia Hassan Safin
```

---

<div align="center">

⭐ **If this helped you, drop a star — it means a lot!**

</div>
