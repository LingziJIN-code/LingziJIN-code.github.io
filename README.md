# 🎓 Academic Homepage Template

<p align="center">
  <strong>A modern, zero-build, elegant academic personal homepage template for researchers, Ph.D. students, and academics.</strong>
</p>

<p align="center">
  <a href="https://laip11.github.io/academic-homepage-template/"><strong>🔗 Live Demo Preview</strong></a> •
  <a href="#key-features">Key Features</a> •
  <a href="#quick-start">Quick Start</a> •
  <a href="#customization-guide">Customization Guide</a> •
  <a href="#theme-presets">Theme Colors</a> •
  <a href="#deploy-to-github-pages">Deployment</a> •
  <a href="#license">License</a>
</p>

> 🌐 **Live Demo**: Check out the live template in action at **[laip11.github.io/academic-homepage-template](https://laip11.github.io/academic-homepage-template/)**.

---

## ✨ Key Features

- ⚡ **Zero-Build Architecture**: No Node.js, no Ruby, no Jekyll, no Hugo. Just standard modern HTML, CSS, JavaScript, and Markdown. Push to GitHub and your site is instantly live!
- 🎨 **Modern Academic Aesthetic**: 
  - Typographic pairing inspired by top research institutions: **Source Serif 4** (classic editorial headings) and **DM Sans** (clean, readable body text).
  - **Floating Dynamic Island Navigation**: Pill-shaped glassmorphic floating header (Apple / Linear style) with deterministic, bidirectional scroll-spy tracking for smooth, zero-flicker section highlighting both downward and upward.
  - **Frosted Glass Card Enclosure**: Ambient multi-stop radial gradient glow + subtle dot grid background with a frosted glass content container.
  - Subtle, publication-grade scroll-reveal animations (with built-in `prefers-reduced-motion` support for accessibility).
- 📝 **Dual-Tab Publication Showcase (Selected vs. All)**:
  - Toggle between curated highlights and your comprehensive publication record with a single click.
  - Automatically sorts papers in the "All" tab by first-author priority (`data-author-rank`) and reverse chronological order (`data-year`).
  - Supports direct deep-linking via URL hash (e.g., `#publications-all`).
- 🧩 **Comprehensive Academic Modules**:
  - **Profile Header**: Avatar, bilingual names, affiliation, research tags, personal hobbies, and social/academic badges (Google Scholar, Email, GitHub, CV, Twitter/X, etc.).
  - **About Me**: Research summary, structured multi-pillar agenda, and collaboration invitation callouts.
  - **News**: Dated timeline updates.
  - **Publications**: Paper cards with teaser figures, CCF/Conference badges, oral/spotlight badges, and flexible action buttons (Paper, Code, Project, Slides, Video).
  - **Working Papers / Preprints**: Minimalist cards for manuscripts under review.
  - **Experience & Internships**: Timeline cards with organizational logos.
  - **Academic Services**: Responsive Bento Grid tiles for conference reviewing with year badges, plus structured list for journal and workshop services.
  - **Education, Honors & Awards, and Teaching Assistantships**.
- 📱 **Fully Responsive**: Flawless reading experience across mobile devices, tablets, laptops, and ultra-wide desktop monitors.
- 🌈 **One-Click Theme Customization**: Pre-configured with 4 academic color schemes (Burgundy Crimson, Classic Academic Blue, Oxford Forest Green, Slate Tech Black).

---

## 🚀 Quick Start (in 3 Minutes)

### Option 1: Use this Template on GitHub
1. Click the green **"Use this template"** button at the top of this repository (or clone it).
2. If you want your site at `https://<your-username>.github.io`, name your new repository `<your-username>.github.io`.
3. Edit `content/profile.md` and `content/main.md` with your own information.
4. Go to **Settings > Pages** in your repo, choose **Deploy from branch: `main` / `(root)`**, and click **Save**. Done!

### Option 2: Local Preview

No installation or dependencies required. Just run Python's built-in static server:

```bash
# In the repository root directory:
python3 -m http.server 8000
```

Then visit [http://localhost:8000](http://localhost:8000) in your web browser.

> 💡 **Tip**: Because the page fetches `content/profile.md` and `content/main.md` via `fetch()`, opening `index.html` directly via `file:///` may be restricted by browser CORS security policies. Always preview using a local server (like Python, VS Code Live Server, or `npx serve`).

---

## 📁 Repository Structure

```text
academic-homepage-template/
├── index.html                   # Core layout, styling, and interactivity
├── favicon.svg                  # Vector website icon
├── LICENSE                      # MIT Open Source License
├── README.md                    # Documentation
├── content/
│   ├── profile.md              # Header section: Avatar, name, role, quick links
│   └── main.md                 # Main content: About, News, Publications, Exp, etc.
├── images/
│   ├── avatar-placeholder.svg  # Sample avatar (replace with your photo)
│   ├── paper-placeholder.svg   # Sample paper figure
│   └── org-placeholder.svg     # Sample institution / company logo
└── .github/
    └── workflows/
        └── deploy.yml          # Optional GitHub Pages automated CI workflow
```

---

## 🛠 Customization Guide

### 1. Update Profile & Header (`content/profile.md`)
Open `content/profile.md` and modify:
- **Avatar image path**: Change `src="images/avatar-placeholder.svg"` to your own photo (e.g., `images/my-avatar.jpg`).
- **Name and Role**: Update your English and Chinese (or localized) names and current degree/affiliation.
- **Research focus**: Edit your core research topics.
- **Quick Links**: Update URLs for Google Scholar, Email, GitHub, CV, Twitter, etc. All link icons are inline SVGs that scale crisply.

### 2. Update Main Content (`content/main.md`)
Open `content/main.md` to edit your academic sections:
- **About Me**: Write a personal hook, overview of research, and foundational research pillars.
- **News**: Add or remove `<li>` items with `<span class="modern-list-date">YYYY.MM</span>`.
- **Publications**:
  Each publication is encapsulated in a `.paper-card`:
  ```html
  <div class="paper-card" data-selected="true" data-author-rank="1" data-year="2026">
    <div class="paper-image-container">
      <img src="images/your-paper-figure.png" alt="Framework Figure">
    </div>
    <div class="paper-content">
      <div class="paper-title">Your Paper Title Here</div>
      <div class="paper-authors"><strong>Your Name<sup>*</sup></strong>, Co-Author One, Senior Author</div>
      <div class="paper-meta">
        <span class="conf-badge">ICML 2026</span>
        <span class="ccf-badge">CCF-A</span>
      </div>
      <div class="paper-links">
        <a href="https://arxiv.org/..." class="paper-btn paper-btn-primary" target="_blank">Paper</a>
        <a href="https://github.com/..." class="paper-btn paper-btn-secondary" target="_blank">Code</a>
      </div>
    </div>
  </div>
  ```
  - `data-selected="true"`: Marks the paper as a highlight in the default **"Selected"** tab.
  - `data-author-rank="1"`: Your authorship rank (1 for first author, 2 for second, etc.) used to rank papers in the **"All"** tab.
  - `data-year="2026"`: Year of publication for secondary sorting.

### 3. Change Webpage Title & Metadata (`index.html`)
In `index.html`:
- Update `<title>Your Name's Homepage</title>`.
- Update `<meta name="description" content="...">` and `<meta name="author" content="...">`.
- Update the navigation brand text in `<a href="#" class="nav-brand">...</a>`.

### 4. Conference Reviewer Bento Grid (`content/main.md`)
Under `#services`, showcase your conference service using responsive Bento tiles:
```html
<div class="service-grid">
  <div class="service-tile">
    <div class="tile-header">
      <span class="tile-conf-name">CVPR</span>
      <div class="tile-years">
        <span class="tile-year-pill">2026</span>
        <span class="tile-year-pill">2025</span>
      </div>
    </div>
    <div class="tile-full-name">IEEE/CVF Conference on Computer Vision and Pattern Recognition</div>
  </div>
</div>
```

---

## 🎨 Theme Presets

You can switch the entire look and feel in seconds. Open `index.html` and look for the `:root` section around line 40:

```css
:root {
  /* Preset 1: Burgundy / Crimson Red (Default) */
  --accent-color: #9d3656;
  --accent-hover: #b84368;
  --accent-bg: #fdf2f6;
  --accent-border: #f5cbd8;

  /* Preset 2: Classic Academic Blue */
  /*
  --accent-color: #1d4ed8;
  --accent-hover: #2563eb;
  --accent-bg: #eff6ff;
  --accent-border: #bfdbfe;
  */

  /* Preset 3: Oxford Forest Green */
  /*
  --accent-color: #1e6b52;
  --accent-hover: #2d8a6b;
  --accent-bg: #f0fdf4;
  --accent-border: #bbf7d0;
  */

  /* Preset 4: Modern Slate / Tech Black */
  /*
  --accent-color: #27272a;
  --accent-hover: #3f3f46;
  --accent-bg: #f4f4f5;
  --accent-border: #e4e4e7;
  */
}
```

Simply uncomment your favorite preset!

---

## 🌐 Deploy to GitHub Pages

### Method A: Deploy from Branch (Recommended & Easiest)
1. Push your repository to GitHub.
2. In your GitHub repository, click **Settings** > **Pages** (in the left sidebar).
3. Under **Build and deployment > Source**, select **Deploy from a branch**.
4. Under **Branch**, select `main` and folder `/(root)`.
5. Click **Save**. In 1–2 minutes, your academic site will be live at `https://<your-username>.github.io/`!

### Method B: GitHub Actions Workflow
This template includes `.github/workflows/deploy.yml`. In **Settings > Pages**, choose **GitHub Actions** as the source, and every commit pushed to `main` will automatically trigger a clean deployment.

---

## 💡 Tips & FAQ

- **How do I add a new section?**  
  Add an `<h1>` with `class="section-title"` and an `id` attribute (e.g. `<h1 id="talks" class="section-title">🎤 Invited Talks</h1>`) in `content/main.md`. Then add `<a href="#talks">Talks</a>` to `.nav-links` in `index.html`.
- **How do I track page views?**  
  You can integrate privacy-friendly analytics like [GoatCounter](https://www.goatcounter.com/), [Google Analytics](https://analytics.google.com/), or [Umami](https://umami.is/) by pasting your tracking script tag right before `</head>` in `index.html`.

---

## 📄 License

This template is open-sourced under the [MIT License](LICENSE). Feel free to use it for personal or academic purposes. 

If you find this template helpful, a ⭐ star on GitHub is greatly appreciated!
