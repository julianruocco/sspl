# Student Space Programs Laboratory (SSPL) — Git Web Stack

Welcome to the official Git repository web stack for the **Student Space Programs Laboratory (SSPL)** at Penn State University!

This repository provides a modern, fast, mobile-responsive static website and documentation portal built with [MkDocs Material](https://squidfunk.github.io/mkdocs-material/). It combines the high visual impact and onboarding clarity of sites like Penn State Rocket Labs with SSPL's rich systems engineering, NASA projects, facilities, and Student Training Program (STP) curriculum.

---

## ⚡ Key Features & Stack Components

1. **Modern Static Web Architecture:**
   - Dark/Light mode theme toggle.
   - Built-in instant client-side search (lunr index).
   - Responsive tabbed navigation and deep sidebar tree.
   - Admonition callouts, code syntax highlighting, badge headers, and card grids.

2. **Automated CI/CD Deployment:**
   - `.github/workflows/deploy.yml`: Automatically builds and publishes the website to GitHub Pages on every `git push` to `main`.

3. **Complete SSPL Content Structure:**
   - **Home / Hero (`docs/index.md`):** High-impact banner, active missions, fast facts, and quick calls-to-action.
   - **About (`docs/about.md`):** Faculty direction (Dr. Sven Bilén), matrix structure, lab history, and systems engineering mindset.
   - **Projects Hub (`docs/projects/`):** Dedicated technical pages for NASA LunaRecycle (Phase 2), SMELT (Big Idea 2023), NEBP Ballooning, Flight Program / CubeSats (OSPREY 3U), and Past Projects.
   - **Student Training Program (`docs/stp.md`):** 14-week curriculum schedule, onboarding milestones, and registration guidelines led by Julian Ruocco.
   - **Facilities (`docs/facilities.md`):** Electronics prototyping, cleanrooms, machining shops, and satellite ground station setups.
   - **Team (`docs/team.md`):** Leadership roster, subsystem leads, and alumni connections.
   - **Join Us (`docs/get-involved.md` & `docs/contact.md`):** Recruitment workflow, contact list, and application forms.
   - **Sponsors & Media (`docs/sponsors.md` & `docs/media.md`):** Corporate tiers, donation links, and news press releases.

---

## ✏️ Customization Markings Guide (`[FILL IN: ...]`)

To make customization effortless, every file contains explicit, highlighted placeholders where custom or updated information can be added.

### How to Find All Fill-In Placeholders:
Search the repository for the text `FILL IN`:

```bash
# On Linux / macOS
grep -rn "FILL IN" docs/

# On Windows (PowerShell)
Select-String -Path "docs\*.md", "docs\**\*.md" -Pattern "FILL IN"
```

Common items marked with `<span class="fill-in-highlight">[FILL IN: ...]</span>` or `<!-- TODO: [FILL IN DETAILS HERE] -->`:
- Meeting dates, times, and room locations.
- Email addresses for subsystem leads.
- Links to Microsoft Forms / Qualtrics application forms.
- Links to Discord / Microsoft Teams workspaces.
- High-resolution CAD models and lab photo uploads.
- Penn State giving/donation portal links.

---

## 🚀 Local Development Setup

Follow these steps to preview and edit the site locally on your computer:

### 1. Clone the Repository
```bash
git clone https://github.com/sspl/sspl-website.git
cd sspl-website
```

### 2. Set Up Python Environment
```bash
python3 -m venv venv
source venv/bin/venv/bin/activate  # On Windows: venv\Scriptsctivate
pip install -r requirements.txt
```

### 3. Run Live Local Development Server
```bash
mkdocs serve
```
Open your web browser and navigate to `http://127.0.0.1:8000` to see live auto-reloading updates as you edit Markdown files!

### 4. Build Static HTML Files (Optional)
```bash
mkdocs build
```
The compiled, production-ready HTML/CSS site will be generated in the `site/` folder.

---

## 🌐 Deploying to GitHub Pages

1. Push this repository to your GitHub account or SSPL GitHub organization.
2. Go to **Repository Settings &rarr; Pages**.
3. Under **Build and deployment**, set Source to **GitHub Actions**.
4. Push any change to the `main` branch. The GitHub Action in `.github/workflows/deploy.yml` will automatically build and publish your website!

---

## 📄 License & Ownership

Created for the **Student Space Programs Laboratory (SSPL)** at The Pennsylvania State University. All rights reserved.
