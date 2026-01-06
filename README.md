# Pedro Mesquita - Senior Data Engineer Portfolio

A modern, responsive portfolio website built to showcase data engineering expertise to recruiters and hiring managers.

## 🚀 Quick Start

1. Open `index.html` in a browser to preview
2. Add `resume.pdf` to the `assets/` folder
3. Deploy to GitHub Pages

## 📁 Project Structure

```
PM_Website_2026/
├── index.html          # Main portfolio (HTML + CSS + JS)
├── README.md           # This file
└── assets/
    ├── resume.pdf      # Your resume (for download button)
    └── preview.png     # OG image for social sharing
```

## ✨ Features

- **Clean, modern design** — Dark theme with cyan/blue/purple gradient accents
- **Responsive** — Mobile, tablet, and desktop optimized
- **Project filtering** — Segmented control to filter Work/Personal projects
- **Terminal code block** — Animated Python-style hero section
- **Scroll animations** — Fade-in effects on scroll
- **Single file** — No build step, easy deployment

---

## 🛠️ How to Edit Content

### Editing Projects

In `index.html`, search for `projects-grid`. Each project is an `<article>` block:

```html
<article class="project-card fade-up" data-type="work">
    <div class="project-header">
        <div class="project-icon"><i class="fas fa-database"></i></div>
        <span class="project-label label-work">Work</span>
        <span class="project-private"><i class="fas fa-lock"></i> Private</span>
    </div>
    <h3 class="project-title">Your Project Name</h3>
    <p class="project-desc">Project description here.</p>
    <div class="project-impact"><span>Impact:</span> Your metrics here</div>
    <div class="project-tags">
        <span class="tag">Tag1</span><span class="tag">Tag2</span>
    </div>
</article>
```

**To change Work/Personal classification:**
- `data-type="work"` → Shows purple "Work" label
- `data-type="personal"` → Shows green "Personal" label

**For Work projects (no public repo):**
```html
<span class="project-label label-work">Work</span>
<span class="project-private"><i class="fas fa-lock"></i> Private</span>
```

**For Personal projects (with GitHub link):**
```html
<span class="project-label label-personal">Personal</span>
<a href="https://github.com/username/repo" target="_blank" class="project-link"><i class="fab fa-github"></i></a>
```

**To change the project icon:**
Replace the icon class inside `.project-icon`. Browse icons at [Font Awesome](https://fontawesome.com/icons).
```html
<div class="project-icon"><i class="fas fa-chart-line"></i></div>
```

### Editing Skills

Search for `skills-grid`. Each skill category is a `.skill-card`:

```html
<div class="skill-card fade-up">
    <div class="skill-header">
        <i class="fas fa-exchange-alt"></i>
        <span>Category Name</span>
    </div>
    <div class="skill-list">
        <div class="skill-item"><span class="skill-dot"></span>Skill 1</div>
        <div class="skill-item"><span class="skill-dot"></span>Skill 2</div>
        <div class="skill-item"><span class="skill-dot"></span>Skill 3</div>
        <div class="skill-item"><span class="skill-dot"></span>Skill 4</div>
    </div>
</div>
```

**To add a skill:** Copy a `<div class="skill-item">` line and change the text.

**To change category icon:** Replace the `<i class="fas fa-...">` class.

**To add a new category:** Copy an entire `.skill-card` block.

### Editing Personal Info

| What | Where to search |
|------|-----------------|
| Name/Role | `hero-title`, `hero-role` |
| Company | `hero-company` |
| Tagline | `hero-desc` |
| Metrics | `metric-value`, `metric-label` |
| Terminal code | `code-block` |
| Email | `mailto:` |
| LinkedIn | `linkedin.com/in/` |
| GitHub | `github.com/` |

---

## 🎨 Customization

### Colors
Edit CSS variables in `:root`:
```css
--accent: #06b6d4;      /* Cyan */
--gradient: linear-gradient(135deg, #06b6d4, #3b82f6, #8b5cf6);
```

### OG Image (Social Sharing Preview)
The `assets/preview.png` appears when you share your site on LinkedIn/Twitter. 
- Recommended size: 1200x630px
- Test with [metatags.io](https://metatags.io) after deploying

---

## 🌐 Deployment (GitHub Pages)

1. Create repo on GitHub
2. Upload `index.html`, `README.md`, and `assets/` folder
3. Settings → Pages → Source: `main` branch
4. Access at `https://your-username.github.io/repo-name/`

**Important:** After deploying, update the OG image URL in `index.html`:
```html
<meta property="og:image" content="https://your-username.github.io/repo-name/assets/preview.png">
```

---

## 📝 Tech Stack

- HTML5 / CSS3 / Vanilla JS
- Google Fonts (Outfit, JetBrains Mono)
- Font Awesome icons
- No frameworks or build tools

---

**Pedro Mesquita** — Senior Data Engineer @ Bosch
