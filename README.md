# Medical CV Template for GitHub Pages

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![GitHub Pages](https://img.shields.io/badge/Deploy-GitHub%20Pages-brightgreen?style=flat-square)](https://pages.github.com/)

**A professional, no-code CV website template for medical professionals, residents, and researchers.**

Built with GitHub Pages and Jekyll for free, automated hosting. No programming experience required.

---

## ✨ Features

- **Free Hosting** - GitHub Pages provides free, automated hosting
- **No Coding Required** - Edit simple Markdown files directly on GitHub
- **Professional Design** - Clean, mobile-responsive layout optimized for medical CVs
- **Multiple Formats** - Automatic PDF and Word document generation
- **Fast Setup** - Get your CV online in 5 minutes
- **Customizable** - Easy color scheme and layout adjustments
- **Research-Focused** - Sections for publications, presentations, and research experience
- **ORCID Integration** - Link your academic profile and research identity

---

## 🚀 Quick Start (5 Minutes)

### Step 1: Create Your Repository

1. Click the green **"Use this template"** button at the top of this page
2. Name your repository:
   - For a personal site: `[yourusername].github.io`
   - For a project site: `[yourname]-cv` or any name you prefer
3. Make sure the repository is set to **Public**
4. Click **"Create repository"**

### Step 2: Enable GitHub Pages

1. Go to your repository's **Settings** tab
2. Click **Pages** in the left sidebar
3. Under "Build and deployment":
   - Source: **Deploy from a branch**
   - Branch: Select **main**
   - Folder: Select **/ (root)**
4. Click **Save**
5. Wait 1-2 minutes for the site to build

Your site will be live at:
- Personal site: `https://[yourusername].github.io/`
- Project site: `https://[yourusername].github.io/[repo-name]/`

### Step 3: Customize Your Content

**Option A: Edit Directly on GitHub (Easiest)**

1. Click on **`_config.yml`** in your repository
2. Click the pencil icon (✏️) to edit
3. Replace the placeholders with your information:
   ```yaml
   author: "Your Name"
   email: your.email@example.com
   url: "https://yourusername.github.io"
   baseurl: "/your-repo-name"  # Leave empty "" if using username.github.io
   ```
4. Scroll down and click **Commit changes**

5. Click on **`cv.md`** and repeat the process:
   - Replace `[Your Full Name]` with your name
   - Update all contact information
   - Add your education, experience, publications, etc.
   - Remove sections you don't need

6. Click on **`index.md`** and customize your homepage:
   - Update your name and position
   - Modify the stats cards with your metrics
   - Add your key publications and achievements

**Option B: Edit Locally (Advanced)**

```bash
git clone https://github.com/[yourusername]/[your-repo-name].git
cd [your-repo-name]
# Edit files in your text editor
git add .
git commit -m "Customize CV content"
git push origin main
```

### Step 4: Add Your Profile Photo

1. Prepare a professional photo (400x400px minimum, square format works best)
2. In your repository, click **Add file** → **Upload files**
3. Upload your photo to the `assets/` folder, naming it `profile-photo.png` (or .jpg)
4. Commit the changes

---

## 📁 Repository Structure

```
your-cv-repo/
├── index.md                    # Homepage with highlights and stats
├── cv.md                       # Full curriculum vitae
├── README.md                   # This file - setup instructions
├── _config.yml                 # Jekyll configuration
├── LICENSE                     # MIT License
├── .gitignore                  # Files to ignore in git
├── _includes/                  # Custom Jekyll components
│   └── footer.html             # Website footer
├── assets/                     # Images, CSS, and scripts
│   ├── profile-photo.png       # Your professional photo
│   ├── style.css               # Main stylesheet
│   └── convert_cv.py           # Python script for PDF/Word conversion
├── cv-downloads/               # Downloadable CV files
│   ├── README.md               # Instructions for generating downloads
│   ├── cv.pdf                  # PDF version (generated)
│   └── cv.docx                 # Word version (generated)
├── publications/               # Research paper PDFs (optional)
│   └── your-paper.pdf
└── presentations/              # Conference posters and slides (optional)
    └── your-poster.pdf
```

---

## ✏️ Customization Guide

### Changing Colors

Edit the CSS variables in `index.md` (lines 6-13):

```css
:root {
  --primary-color: #2c5aa0;      /* Main accent color */
  --primary-dark: #1a3a5c;       /* Darker shade for hover effects */
  --light-bg: #f8f9fa;           /* Light background for cards */
  --text-dark: #1a3a5c;          /* Main text color */
}
```

### Modifying Sections

**To remove a section:**
1. Open `cv.md` or `index.md`
2. Delete the entire section including the `##` heading
3. Commit the changes

**To add a section:**
1. Copy an existing section format
2. Modify the heading and content
3. Commit the changes

### Contact Information

Update contact details in **three places**:
1. `_config.yml` - Site-wide settings
2. `cv.md` - Full CV contact section
3. `index.md` - Homepage contact section

### Stats Cards (Homepage)

Edit the stats grid in `index.md` around line 270:

```html
<div class="stat-card">
  <h3>7</h3>
  <p>Peer-Reviewed<br>Publications</p>
</div>
```

Change the number and description to match your achievements.

---

## 📄 Generating PDF and Word Downloads

### Prerequisites

Install the required tools (one-time setup):

**macOS:**
```bash
brew install pandoc
brew install --cask mactex  # or basictex for smaller install
```

**Linux:**
```bash
sudo apt install pandoc texlive-xetex texlive-fonts-recommended
```

**Windows:**
- Download Pandoc: https://pandoc.org/installing.html
- Download MiKTeX: https://miktex.org/download

### Generate Downloads

1. Clone your repository locally
2. Run the conversion script:
   ```bash
   python3 assets/convert_cv.py
   ```
3. This creates:
   - `cv-downloads/cv.pdf`
   - `cv-downloads/cv.docx`
4. Commit and push the generated files:
   ```bash
   git add cv-downloads/
   git commit -m "Update CV downloads"
   git push origin main
   ```

---

## 📂 Adding Publications and Presentations

### Adding Publication PDFs

1. Upload your PDF to the `publications/` folder
2. Link it in `cv.md`:
   ```markdown
   [[PDF](./publications/your-paper.pdf)] [[PubMed](https://pubmed.ncbi.nlm.nih.gov/PMID/)]
   ```

### Adding Presentation Materials

1. Upload your poster/slides to the `presentations/` folder
2. Link it in `cv.md`:
   ```markdown
   [🖼️ PDF](./presentations/your-poster.pdf)
   ```

---

## 🎨 Advanced Customization

### Using a Custom Domain

1. Purchase a domain (e.g., from Namecheap, Google Domains)
2. In your repository, create a file named `CNAME` containing:
   ```
   www.yourname.com
   ```
3. Configure DNS settings with your domain provider:
   - Add a CNAME record pointing to `[yourusername].github.io`
4. In repository Settings → Pages → Custom domain, enter your domain

### Changing the Theme Skin

Edit `_config.yml`:
```yaml
minima:
  skin: classic  # Options: classic, dark, auto, solarized
```

### Modifying the Stylesheet

The main styles are in `assets/style.css`. To override:
1. Edit the CSS variables at the top of the file
2. Or add custom CSS to the `<style>` tags in `index.md`

---

## 🔧 Troubleshooting

### Site Not Updating

- **Wait 1-2 minutes** - GitHub Pages takes time to rebuild
- Check Settings → Pages for deployment status
- Ensure the repository is **Public**
- Verify GitHub Pages is set to deploy from **main** branch

### Images Not Showing

- Verify file paths are correct (case-sensitive)
- Check that images are uploaded to the `assets/` folder
- Ensure image names match the references in Markdown files

### PDF Generation Fails

- Install both Pandoc AND LaTeX (both are required for PDF)
- Check error messages for missing LaTeX packages
- Try generating just Word format first: `pandoc cv.md -o cv.docx`

### Formatting Issues

- Markdown requires blank lines between sections
- Check for proper indentation (lists need 4 spaces)
- Validate YAML front matter in `_config.yml` (must start with `---`)

---

## 📚 Resources

- **Markdown Guide:** https://www.markdownguide.org/
- **GitHub Pages Documentation:** https://docs.github.com/en/pages
- **Jekyll Documentation:** https://jekyllrb.com/docs/
- **Pandoc Manual:** https://pandoc.org/MANUAL.html

---

## 🤝 Contributing

Found a bug or have a suggestion? Please [open an issue](https://github.com/anthonyomorada/am-medical-cv-template/issues) on the template repository.

---

## 📄 License

This template is available under the [MIT License](LICENSE). Feel free to use, modify, and distribute as needed.

**Note:** When using this template, please customize the footer in `_includes/footer.html` to credit yourself as the CV author. The template attribution can remain or be removed as you prefer.

---

## 💡 Tips for Medical CVs

### For Residents
- Highlight clinical rotations and procedural experience
- Include research projects and quality improvement work
- List presentations at grand rounds and conferences
- Mention leadership roles in residency committees

### For Fellows
- Emphasize specialized training and advanced procedures
- Highlight research with fellowship mentors
- Include grant applications and funding
- List society memberships relevant to your specialty

### For Faculty
- Feature your research focus and lab overview
- Include grant funding history and amounts
- List mentored students and trainees
- Highlight administrative and committee service

### For Researchers
- Lead with high-impact publications and h-index
- Include collaborative projects and consortia membership
- Feature conference presentations and invited talks
- List editorial board positions and peer review work

---

**Created by Anthony Onde Morada, MD**

*Template adapted from personal CV repository for broad medical community use.*

For questions about this template, visit: https://github.com/anthonyomorada/am-medical-cv-template

---

*Last updated: November 2025*
