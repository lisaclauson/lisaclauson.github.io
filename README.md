# 📄 Personal Portfolio Website

A clean, responsive personal portfolio site inspired by [gitfolio](https://github.com/imfunniee/gitfolio), built with plain HTML, CSS, and JavaScript — no framework or build step required.

## 📁 File Structure

```
portfolio/
├── index.html     ← Main page (all sections)
├── style.css      ← All styles
├── script.js      ← Scroll animations & nav logic
└── README.md      ← This file
```

## 🚀 Deploy to GitHub Pages (5 minutes)

1. **Create a new repository** on GitHub named exactly:
   ```
   yourusername.github.io
   ```
   Replace `yourusername` with your actual GitHub username.

2. **Push these files** to the repo root:
   ```bash
   git init
   git add .
   git commit -m "initial portfolio"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages** (if not auto-enabled):
   - Go to repo → Settings → Pages
   - Source: `Deploy from a branch` → `main` → `/ (root)`
   - Save

4. Your site will be live at: `https://yourusername.github.io` within 1–2 minutes.

## ✏️ Personalizing Your Site

### Replace Placeholder Text
Search for and replace all instances of:
| Placeholder | Replace with |
|---|---|
| `Your Name` | Your full name |
| `YN` | Your initials |
| `yourusername` | Your GitHub username |
| `yourprofile` | Your LinkedIn profile slug |
| `youremail@example.com` | Your email |
| `City, State` | Your location |

### Sections to Fill In
- **About Me** — Edit the `<p>` tags in `#about`
- **Education** — Fill in degrees, universities, GPA, years, coursework
- **Experience** — Add your job titles, companies, dates, and bullet points
- **Projects** — Add your project cards with links to GitHub / reports
- **Ansys / Zemax** — Replace the 4 sample project cards with your real Zemax projects
- **Skills** — Add/remove skill tags in each group
- **Publications** — Add your papers, conferences, and posters

### Change the Avatar
The `.hero-avatar` div currently shows your initials. To use a photo:
```html
<!-- Replace this: -->
<div class="hero-avatar">YN</div>

<!-- With this: -->
<img class="hero-avatar" src="photo.jpg" alt="Your Name" />
```
Add a `photo.jpg` to the portfolio folder and add this CSS override:
```css
.hero-avatar { object-fit: cover; }
```

### Add More Cards
**Project card:**
```html
<div class="project-card">
  <div class="project-icon">🔬</div>
  <h3 class="project-title">My Project</h3>
  <p class="project-desc">Short description of what you built and why.</p>
  <div class="tag-row">
    <span class="tag">Zemax</span>
  </div>
  <div class="project-links">
    <a href="https://github.com/..." target="_blank" class="link-btn">GitHub →</a>
  </div>
</div>
```

**Zemax card:**
```html
<div class="zemax-card">
  <div class="zemax-card-accent"></div>
  <div class="zemax-card-inner">
    <span class="zemax-type">Sequential Design</span>
    <h3>My Zemax Project</h3>
    <p>Description of the optical system designed and results achieved.</p>
    <ul class="zemax-specs">
      <li><strong>Tool:</strong> OpticStudio Sequential Mode</li>
      <li><strong>Analysis:</strong> MTF, Spot Diagram</li>
      <li><strong>Result:</strong> Your result</li>
    </ul>
    <div class="project-links">
      <a href="#" class="link-btn">View Files →</a>
    </div>
  </div>
</div>
```

## 🎨 Theme Customization

All colors are CSS variables at the top of `style.css`:
```css
:root {
  --accent: #2563eb;       /* Change this to change the main accent color */
  --zemax: #0f172a;        /* Dark background for Zemax section */
  --zemax-accent: #38bdf8; /* Zemax highlight color */
  ...
}
```

## 📱 Responsive
The site is fully responsive — it works on mobile, tablet, and desktop out of the box.

---

Built with ♥ — hosted on GitHub Pages.
