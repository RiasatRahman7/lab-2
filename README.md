# Riasat Rahman — Personal Portfolio Website

> **Cybersecurity & Network Security Specialist | Adjunct Instructor | Academic Researcher**  
> Pacific States University · California, USA

[![GitHub Pages](https://img.shields.io/badge/Deployed_on-GitHub_Pages-blue?logo=github)](https://pages.github.com/)

---

## 🚀 Live Demo

Once deployed: `https://<your-username>.github.io/riasat-portfolio/`

---

## 📁 Project Structure

```
riasat-portfolio/
├── index.html              # Main single-page portfolio
├── assets/
│   ├── css/
│   │   └── style.css       # All styles (responsive, dark theme)
│   └── js/
│       └── main.js         # Interactions, canvas, animations
└── README.md               # This file
```

---

## 🌐 Deploying to GitHub Pages

### Method 1: GitHub GUI (Easiest)

1. Create a new GitHub repository named `riasat-portfolio`
2. Upload all project files to the repository root
3. Go to **Settings → Pages**
4. Under **Source**, select `Deploy from a branch`
5. Choose branch: `main`, folder: `/ (root)`
6. Click **Save**
7. Your site will be live at `https://<your-username>.github.io/riasat-portfolio/`

### Method 2: Git CLI

```bash
# Initialize and push
git init
git add .
git commit -m "Initial portfolio deployment"
git branch -M main
git remote add origin https://github.com/<your-username>/riasat-portfolio.git
git push -u origin main

# Enable GitHub Pages via Settings → Pages (as above)
```

### Method 3: Custom Domain (Optional)

1. Add a `CNAME` file to the project root with your domain:
   ```
   www.riasatrahman.com
   ```
2. Configure DNS A records to point to GitHub Pages IPs:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

---

## 🛠 Customization Guide

### Updating Personal Information

Edit `index.html` and find/replace:
- Email: `riasat.rahman@psu.edu`
- LinkedIn URL: `linkedin.com/in/riasatrahman`
- Google Scholar: Update the link in the Research section

### Adding a Real Profile Photo

Replace the initials placeholder in `index.html`:
```html
<!-- Find this block -->
<div class="photo-placeholder">
  <div class="photo-initials">RR</div>
  ...
</div>

<!-- Replace with -->
<img src="assets/images/profile.jpg" alt="Riasat Rahman" class="profile-photo" />
```
Add to `style.css`:
```css
.profile-photo {
  width: 260px; height: 260px;
  border-radius: 50%;
  object-fit: cover;
  border: 2px solid var(--border-glow);
}
```

### Adding Award Images (Picture 2 & 3)

Replace placeholder blocks in the Awards section:
```html
<!-- Replace award-img-placeholder div with: -->
<img src="assets/images/award1.jpg" alt="IEEE Excellence Award 2023" />
```

### Adding Publications / Projects

Publications follow this pattern in `index.html`:
```html
<div class="pub-item reveal">
  <span class="pub-year mono">2025</span>
  <div class="pub-body">
    <h4>Your Paper Title Here</h4>
    <p class="pub-meta">Journal Name · Volume, Issue</p>
    <div class="pub-tags"><span class="pub-tag">Tag</span></div>
  </div>
  <a href="link-to-pdf.pdf" class="pub-link mono">PDF ↗</a>
</div>
```

### Connecting the Contact Form

The form is pre-styled but needs a backend. Options:

**Option A — Formspree (free, no backend needed):**
```html
<form class="contact-form" action="https://formspree.io/f/YOUR_ID" method="POST">
```

**Option B — Netlify Forms:**
Add `data-netlify="true"` to the form tag (requires Netlify hosting).

---

## 🎨 Design System

| Token | Value | Usage |
|-------|-------|-------|
| `--accent` | `#63b3ed` | Primary blue, links, highlights |
| `--accent2` | `#38bdf8` | Sky blue, gradients |
| `--accent3` | `#a78bfa` | Purple, hero gradient |
| `--bg-dark` | `#080c14` | Main background |
| `--bg-card` | `#0d1422` | Card backgrounds |
| `--font-display` | Syne | Headlines, nav |
| `--font-body` | DM Sans | Body text |
| `--font-mono` | JetBrains Mono | Code, labels, tags |

---

## ✅ Features

- ✅ Fully responsive (mobile, tablet, desktop)
- ✅ Animated particle network canvas (hero)
- ✅ Scroll-triggered reveal animations
- ✅ Animated skill progress bars
- ✅ Research tab switcher (Journals / Conferences)
- ✅ Mobile hamburger navigation
- ✅ SEO meta tags (OpenGraph, description, keywords)
- ✅ Sticky navbar with active section highlighting
- ✅ Smooth scroll navigation
- ✅ Contact form with success state
- ✅ Awards gallery with hover effects
- ✅ GitHub Pages ready (zero dependencies)

---

## 📄 License

MIT License — Free to use and modify for personal portfolio use.

---

*Built for Riasat Rahman · Pacific States University · 2025*
