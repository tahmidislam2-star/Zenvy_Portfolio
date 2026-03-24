<img width="1902" height="957" alt="image" src="https://github.com/user-attachments/assets/84d3f2b2-df23-44c2-997e-7981dc255abb" /># 🎮 Zenvy — Indie Game Dev Portfolio

> A handmade, sketchbook-inspired single-page portfolio for indie game developer **Tahmid / Zenvy**.

**🔗 Live Demo → [zenvy-pixel-portfolio.vercel.app](https://zenvy-pixel-portfolio.vercel.app/)**

---

## ✨ Features

- 🖊️ **Sketchbook / collage aesthetic** — asymmetric card layouts, tape strips, doodle stamps
- 🌙 **Dark / light mode toggle** — all colours theme-aware, contact section always stays dark
- 🖱️ **Custom pixel cursor** — saturated red/orange/yellow so it's visible on any background
- 🗒️ **Draggable sticky notes** — two floating notes you can grab and move anywhere on screen
- ✨ **Glitch hover effect** — on the big section headings
- 🎞️ **Scroll parallax** — hero image drifts gently as you scroll
- 🔄 **Scroll reveal animations** — sections fade and slide in as they enter the viewport
- 🎨 **Pixel-art canvas fallbacks** — procedurally drawn thumbnails appear if game images are missing
- 📱 **Fully responsive** — desktop collage layout → 2-column tablet → single-column phone

---

## 📸 Preview

### Light Mode
<img width="1905" height="959" alt="showcase (1)" src="https://github.com/user-attachments/assets/892e315f-5bcb-465f-931b-76b869fde33b" />

### Dark Mode
<img width="1902" height="957" alt="Screenshot 2026-03-24 171707" src="https://github.com/user-attachments/assets/f5051468-cd5d-45b8-986b-3690c5df990e" />

### Games Section
<img width="1906" height="959" alt="showcase (2)" src="https://github.com/user-attachments/assets/6bab80ab-0075-4260-820b-b53694704e7d" />

### About Me Section
<img width="1904" height="955" alt="showcase (3)" src="https://github.com/user-attachments/assets/723a1ddc-0503-4c39-bd20-89e3fb04359d" />

---

## 🗂️ File Structure

```
your-portfolio/
│
├── index.html          ← entire site (HTML + CSS + JS, single file)
│
└── images/
    ├── hero.gif        ← animated character / art for the hero section
    ├── pfp.png         ← portrait photo used in the About section
    ├── game1.png       ← Tea Pls thumbnail
    ├── game2.png       ← Oinknight thumbnail
    ├── game3.png       ← Brakefail Taxi thumbnail
    ├── game4.png       ← Power Balance thumbnail
    └── game5.png       ← Rock, Paper, Scissors Swap thumbnail
```

> All images are optional — the site renders pixel-art canvas fallbacks automatically if any image is missing.

---

## 🚀 Getting Started

No build tools, no npm, no framework. Just open the file.

**Option A — open locally:**
```bash
# Clone the repo
git clone https://github.com/your-username/your-repo-name.git

# Open in your browser
open index.html
# or just double-click it
```

**Option B — live server (recommended for GIF support):**
```bash
# With VS Code Live Server extension
# Right-click index.html → "Open with Live Server"

# Or with Python
python -m http.server 8000
# then visit http://localhost:8000
```

---

## 🎨 Customising

### Personal info
Open `index.html` and search for these lines to update your details:

| What | Where to look |
|------|--------------|
| Name / alias | `<h1 class="hero-name">` |
| Tagline | `<p class="hero-tagline">` |
| Intro paragraph | `<p class="hero-intro">` |
| About text | `<div class="about-text">` |
| Email | `href="mailto:..."` in the contact section |
| Discord handle | Contact badges + social links |

### Adding / editing games
Each game is a `<div class="game-card">` block in the `#games` section. Copy any existing card and change the `src`, title, description, tags, and `href`.

### Colours
All theme colours are CSS variables at the top of the `<style>` block:

```css
:root {
  --bg:            #f2ede6;   /* page background   */
  --ink:           #1a1714;   /* text / borders    */
  --accent-red:    #c94040;   /* primary accent    */
  --accent-yellow: #d9a832;   /* tape / highlights */
  --accent-blue:   #3a6ea5;
  --accent-green:  #4a8c5c;
}
```

---

## 🛠️ Built With

| Tool | Purpose |
|------|---------|
| Pure HTML / CSS / JS | No frameworks, no build step |
| [Syne](https://fonts.google.com/specimen/Syne) | Display headings |
| [Caveat](https://fonts.google.com/specimen/Caveat) | Handwritten labels & tags |
| [DM Mono](https://fonts.google.com/specimen/DM+Mono) | Body / code text |
| HTML Canvas API | Pixel-art fallback thumbnails |
| CSS Grid | Asymmetric collage card layout |
| IntersectionObserver | Scroll reveal + active nav |

---

## 🎮 Games Featured

| Game | Genre | Link |
|------|-------|------|
| Tea Pls | Simulation / Chill | [itch.io](https://z-envy.itch.io/tea-plss) |
| Oinknight | 2D Platformer / Action | [itch.io](https://z-envy.itch.io/oinknight) |
| Brakefail Taxi | Simulation / Driving | [itch.io](https://z-envy.itch.io/brakefail-taxi) |
| Power Balance | Action / Wave Shooter | [itch.io](https://z-envy.itch.io/power-balance-two-worlds) |
| Rock, Paper, Scissors Swap | Arcade / Wave-fighting | [itch.io](https://z-envy.itch.io/rps-s) |

---

## 🌐 Deployment

The site is a single static HTML file — it deploys anywhere with zero config.

**Vercel (recommended):**
1. Push to GitHub
2. Import the repo at [vercel.com/new](https://vercel.com/new)
3. Leave all settings as default → click **Deploy**

**GitHub Pages:**
1. Go to repo **Settings → Pages**
2. Set source to `main` branch, `/ (root)`
3. Save — your site will be live at `https://your-username.github.io/your-repo-name`

---

## 📝 License

Feel free to use this as a base for your own portfolio. If you do, a credit or a star would be appreciated but isn't required. All game content, artwork, and personal info belong to **Tahmid / Zenvy**.

---

<p align="center">made with pixels &amp; caffeine by <strong>Zenvy</strong></p>
