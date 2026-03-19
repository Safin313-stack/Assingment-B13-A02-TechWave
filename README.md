<div align="center">

<br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0f,50:1a1a3e,100:2d1b69&height=200&section=header&text=TechWave&fontSize=60&fontColor=ffffff&fontAlignY=38&desc=Your+daily+dose+of+tech+insights+and+growth&descAlignY=60&descSize=15&descColor=94a3b8" width="100%"/>

<br/>

[![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![MIT License](https://img.shields.io/badge/License-MIT-22c55e?style=flat-square)](LICENSE)
[![Deployed](https://img.shields.io/badge/Deployed-GitHub%20Pages-0ea5e9?style=flat-square&logo=github)](https://safin313-stack.github.io/Assingment-B13-A02-TechWave/)
[![PH Batch](https://img.shields.io/badge/Programming%20Hero-Batch%2013-f97316?style=flat-square)](https://web.programming-hero.com)

<br/>

<a href="https://safin313-stack.github.io/Assingment-B13-A02-TechWave/">
  <img src="https://img.shields.io/badge/-%F0%9F%8E%99%EF%B8%8F%20%20LIVE%20DEMO%20%20%E2%86%92-2d1b69?style=for-the-badge&logoColor=white" alt="Live Demo" height="42"/>
</a>

<br/>
<sub>✦ No login &nbsp;·&nbsp; No install &nbsp;·&nbsp; Opens instantly in your browser ✦</sub>

<br/><br/>

</div>

---

<div align="center">

### 🎙️ What You Get

| 🌑 Dark Theme | 🪟 Glass Cards | 📐 Bento Grid | 📱 Responsive Nav | 🎧 Episodes | 📊 Stats |
|:---:|:---:|:---:|:---:|:---:|:---:|
| Deep space aesthetic with purple and cyan accents | Frosted-glass feature cards via custom CSS | Asymmetric CSS Grid layout for feature section | Hamburger menu with smooth expand on mobile | Hoverable cards with play button overlays | 150K+ listeners · 200+ episodes · 4.9★ |

</div>

---

## 🖥️ Page Structure

```
╔══════════════════════════════════════════════════════════════╗
║  🎙️  TechWave       About · Episodes · Host   [Subscribe]   ║  ← Navbar
╠══════════════════════════════════════════════════════════════╣
║              [ pulsing mic icon — animated ring ]            ║
║                        TechWave                              ║  ← Hero
║          "Your daily dose of tech insights..."               ║
║         [ Listen on Spotify ]   [ Subscribe ]                ║
╠══════════════════════════════════════════════════════════════╣
║   150K+ Listeners · 200+ Episodes · 4.9★ · 50+ Experts      ║  ← Stats
╠══════════════════════════════════════════════════════════════╣
║  Why Choose TechWave                                         ║
║  ╔═══════════════════════╦═══════════════╗                   ║
║  ║  🎧 Premium Audio     ║  📱 Mobile    ║  ← Bento Grid    ║
║  ║     (spans 2 rows)    ╠═══════════════╣                   ║
║  ║                       ║  🌍 Community ║                   ║
║  ╠═══════════════════════╬═══════════════╣                   ║
║  ║  🎤 Exclusive         ║  📚 Resources ║                   ║
║  ╚═══════════════════════╩═══════════════╝                   ║
╠══════════════════════════════════════════════════════════════╣
║  Featured Episodes  [ 3 hoverable cards with overlays ]      ║  ← Episodes
╠══════════════════════════════════════════════════════════════╣
║  🎤 Alex Kumar  ·  Bio  ·  LinkedIn · X · Instagram · YT    ║  ← Host
╠══════════════════════════════════════════════════════════════╣
║  © TechWave  ·  Spotify · Apple · YouTube · Twitter          ║  ← Footer
╚══════════════════════════════════════════════════════════════╝
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
.features-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-rows: repeat(3, auto);
  gap: 1.5rem;
}
.card-premium-audio        { grid-row: 1 / 3; }
.card-exclusive-interviews { grid-row: 3;     }
```

### Gradient CTA Button

```css
.gradient-btn {
  background: linear-gradient(135deg, #ec4899, #8b5cf6, #06b6d4);
  transition: opacity 0.2s ease;
}
.gradient-btn:hover { opacity: 0.88; }
```

### Mobile Hamburger Toggle

```js
hamburger.addEventListener('click', () => {
  mobileMenu.style.maxHeight =
    mobileMenu.style.maxHeight === '0px' || !mobileMenu.style.maxHeight
      ? '300px' : '0px';
});
```

---

## 📁 Project Structure

```
Assingment-B13-A02-TechWave/
│
├── 📄 index.html          ← Full page · navbar · hero · sections · footer
│
└── 📂 styles/
    ├── 🎨 style.css       ← Glass cards · bento grid · dark theme · animations
    ├── 🎙️  microphone.png  ← Hero and features icon
    ├── 🎧 headphone.png   ← Premium audio icon
    ├── 📱 device.png      ← Mobile friendly icon
    ├── 📍 location.png    ← Global community icon
    ├── 📚 resource.png    ← Rich resources icon
    ├── 🧑 host.png        ← Alex Kumar host photo
    ├── 👥 group.png       ← Episode thumbnail
    └── 🔗 social icons    ← linkedin · x · instagram · youtube · spotify · apple
```

---

## 🚀 Run It Yourself

**Option 1 — Live (instant, no setup)**

> 🔗 **[https://safin313-stack.github.io/Assingment-B13-A02-TechWave/](https://safin313-stack.github.io/Assingment-B13-A02-TechWave/)**

**Option 2 — Clone and open locally**

```bash
git clone https://github.com/Safin313-stack/Assingment-B13-A02-TechWave.git
cd Assingment-B13-A02-TechWave
open index.html
```

**Option 3 — VS Code Live Server**

```
1. Install Live Server extension
2. Right-click index.html → Open with Live Server
3. Site opens at localhost:5500 ✅
```

---

## 🛠️ Tech Stack

```
┌──────────────────────────────────────────────────┐
│           Frontend · No Build Tools Required     │
├─────────────────┬────────────────────────────────┤
│  HTML5          │  Full semantic page structure  │
│  Tailwind CSS   │  Utility-first layout (CDN)    │
│  CSS3           │  Glassmorphism · grid · anims  │
│  JavaScript     │  Hamburger toggle only         │
│  Unsplash       │  Episode thumbnail images      │
└─────────────────┴────────────────────────────────┘
```

---

## 🎙️ Sections Overview

```
Navbar     → Logo · nav links · subscribe CTA · mobile hamburger toggle
Hero       → Animated pulsing mic · tagline · dual CTA buttons
About      → Podcast description + 4-column stat grid
Why Choose → 5-card asymmetric bento grid with glassmorphism
Episodes   → 3-column cards with hover overlay + play button
Host       → Alex Kumar bio + social media icon links
Footer     → Spotify · Apple Podcasts · YouTube · Twitter + copyright
```

---

<div align="center">

## 👤 Developer

<br/>

**Saharia Hassan Safin**
Front-end Developer · Programming Hero Batch 13

<br/>

[![GitHub](https://img.shields.io/badge/GitHub-Safin313--stack-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Safin313-stack)
&nbsp;
[![Live Project](https://img.shields.io/badge/Live%20Project-Visit%20Now-2d1b69?style=for-the-badge&logo=vercel&logoColor=white)](https://safin313-stack.github.io/Assingment-B13-A02-TechWave/)

<br/>

*"Designing dark-mode interfaces one glass card at a time"* 🎙️

<br/>

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:2d1b69,50:1a1a3e,100:0a0a0f&height=120&section=footer" width="100%"/>

<sub>MIT License · © 2025 Saharia Hassan Safin · ⭐ Star this repo if it helped you!</sub>

</div>
