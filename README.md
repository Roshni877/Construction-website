# Lux Construction — Scrollytelling Website
## Setup Guide for Roshni

---

### 📁 Folder Structure
```
Construction_Website_Roshni/
├── index.html                    ← The entire website (single file)
├── public/
│   └── assets/
│       └── sequence/
│           ├── frame_000000.jpeg
│           ├── frame_000001.jpeg
│           ├── ...
│           └── frame_000239.jpeg  ← 240 frames total
└── README.md
```

---

### 🎬 Step 1 — Extract Video Frames

1. Go to **https://www.frametoolkit.com/tools/frame-extractor**
2. Upload your video (the one you shared: `can_u_make_it_more_better.mp4`)
3. Set frame count to **240**
4. Download all frames
5. Rename them as: `frame_000000.jpeg`, `frame_000001.jpeg` ... `frame_000239.jpeg`
6. Place all 240 images in: `public/assets/sequence/`

---

### 🌐 Step 2 — View the Website Locally (How to Run)

> ⚡ **Quick Run (Single Command):**
> ```bash
> npx http-server "d:/Construction_Website_Roshni" -o index.html
> ```
> *Or inside the project directory:*
> ```bash
> npx http-server -o index.html
> ```

---

**Other Options:**

- **Option A — Python local server**
  ```bash
  cd Construction_Website_Roshni
  python -m http.server 8080
  # Open http://localhost:8080
  ```

- **Option B — VS Code Live Server**
  1. Open the `Construction_Website_Roshni` folder in VS Code
  2. Install the "Live Server" extension
  3. Right-click `index.html` → "Open with Live Server"

> ⚠️ **Do NOT just double-click index.html** — browsers block local image loading via `file://`. Use a local server.

---

### 🚀 Step 3 — Deploy to Netlify (Free)

1. Go to **https://app.netlify.com/drop**
2. Drag and drop the entire `Construction_Website_Roshni` folder
3. Your site goes live instantly with a URL!

---

### 🎨 What's Built

| Section | Details |
|---|---|
| **Navbar** | Fixed glass nav, italic Cormorant Garamond logo, dark glass style |
| **Scrollytelling Hero** | 8000px scroll, 4 text phases, 240 canvas frames, GSAP ScrollTrigger |
| **Selected Work** | Villa Sereno + Glass House, grid layout, hover zoom |
| **Philosophy** | 3 pillars, dark background, scroll reveals |
| **Services** | 6 services, grid, hover glow |
| **Testimonials** | 3 cards, glass morphism, 5-star ratings, architectural grid bg |
| **Contact** | Enquiry form, studio details |
| **Footer** | Logo, copyright, socials |

### 🔤 Typography
- **Cormorant Garamond** — Display headings, logo
- **Cormorant SC** — Small caps labels, testimonial names
- **Bodoni Moda** — Body text
- **Syncopate** — Utility labels, nav links

---

### 💡 Customisation Tips

- Change company name: search `lux construction` in `index.html`
- Change gold accent colour: edit `--gold: #c9a86c` in `:root`
- Change frame count: edit `TOTAL_FRAMES = 240`
- Change frame path: edit `FRAME_PATH = 'public/assets/sequence/'`
- Add real project photos: replace the Unsplash URLs in the Work section

---

*Built with GSAP ScrollTrigger + Canvas API + Google Fonts. No frameworks needed.*
