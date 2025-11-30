# Medical CV Template - Free Professional Website

[![Use This Template](https://img.shields.io/badge/Use_This_Template-2ea44f?style=for-the-badge)](https://github.com/anthonyomorada/am-medical-cv-template/generate)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)

**Create your professional CV website in 5 minutes. No coding required.**

A ready-to-use template for medical professionals (residents, fellows, faculty) to showcase their CV, publications, and research online. Built with GitHub Pages for **free hosting** with automatic updates.

📺 **[Live Demo](https://anthonyomorada.github.io/anthony-morada-cv/)** | 📖 **[Full Documentation](#-setup-guide)**

---

## ✨ What You Get

- 🌐 **Professional website** with your CV automatically published
- 📱 **Mobile-optimized** design for program directors viewing on phones
- 🆓 **Free hosting** via GitHub Pages (no server costs)
- ⚡ **Instant updates** - edit and changes go live in ~1 minute
- 📄 **Downloadable PDFs** - auto-generated from your content
- 🔍 **Search engine friendly** - appears in Google searches
- 📊 **Publication showcase** - display research with direct PDF links

---

## 🎯 Perfect For

- ✅ Residency and fellowship applications
- ✅ Academic job searches
- ✅ Faculty promotion portfolios
- ✅ Research collaboration networking
- ✅ Professional branding

---

## 🚀 5-Minute Setup

### Step 1: Create Your Repository (1 minute)

**Click the green "Use this template" button at the top of this page**, then:

1. Name your repository: `[your-username]-cv` (e.g., `jsmith-cv`)
2. Choose **Public** visibility
3. Click **Create repository from template**

### Step 2: Enable GitHub Pages (1 minute)

1. In your new repository, go to **Settings** (top menu)
2. Scroll to **Pages** section (left sidebar)
3. Under "Source", select **Deploy from a branch**
4. Choose **main** branch
5. Click **Save**

✅ **Your site is now live!** Visit: `https://[your-username].github.io/[repository-name]/`

### Step 3: Add Your Information (3 minutes)

1. Click on `cv.md` file in your repository
2. Click the **pencil icon** (✏️) to edit
3. Replace the placeholder text with your information
4. Scroll down and click **Commit changes**
5. Wait ~1 minute - your website updates automatically!

Repeat for `index.md` (homepage).

---

## 📝 What to Edit

### Essential Files (Start Here)

**`_config.yml`** - Site settings
```yaml
title: Your Name, MD
email: your.email@institution.edu
description: Brief professional description
url: "https://yourusername.github.io"
baseurl: "/repository-name"
```

**`cv.md`** - Your complete CV
- Education
- Research experience
- Publications
- Presentations
- Awards and honors

**`index.md`** - Homepage with highlights
- Professional summary
- Research impact stats
- Featured publications
- Contact information

### Optional Customization

**`assets/profile-photo.png`** - Your professional headshot (400x400px recommended)

**`assets/style.css`** - Colors and styling (change `--primary-color` for main theme)

**`_includes/footer.html`** - Custom footer text

---

## 📁 File Structure Explained

```
your-cv-repository/
├── index.md              # Homepage (edit this)
├── cv.md                 # Full CV (edit this)
├── _config.yml           # Site settings (edit this)
├── assets/
│   ├── profile-photo.png # Your photo (replace this)
│   └── style.css         # Styling
├── cv-downloads/         # PDF/Word versions
├── publications/         # Upload your paper PDFs here
└── presentations/        # Upload poster PDFs here
```

---

## 📄 Creating Downloadable PDFs

### Option 1: Use Online Converter (Easiest)
1. Copy content from your `cv.md`
2. Use [Markdown to PDF](https://www.markdowntopdf.com/)
3. Upload result to `cv-downloads/` folder

### Option 2: Use Pandoc (Advanced)
```bash
# Install Pandoc first (see main documentation)
pandoc cv.md -o cv-downloads/cv.pdf
```

---

## 🎨 Customization Guide

### Change Your Theme Color

Edit `assets/style.css`:
```css
:root {
  --primary-color: #2c5aa0;  /* Change this color code */
}
```

**Popular medical theme colors:**
- `#2c5aa0` - Professional Blue (default)
- `#1a472a` - Forest Green
- `#6a1b9a` - Royal Purple
- `#c41e3a` - Crimson Red

### Add a Publication

1. Upload PDF to `publications/` folder
2. Edit `cv.md` and add link:
```markdown
[[PDF](./publications/your-paper.pdf)]
```

### Add a Presentation

1. Upload PDF to `presentations/` folder
2. Edit `cv.md` and add link:
```markdown
[🖼️ Poster PDF](./presentations/your-poster.pdf)
```

---

## 🔧 Troubleshooting

### Site isn't showing up
- Wait 2-3 minutes after enabling Pages
- Check Settings → Pages shows "Your site is live at..."
- Ensure repository is **Public** not Private

### Images not loading
- File names are case-sensitive
- Check file path matches exactly
- Use forward slashes `/` not backslashes `\`

### Changes not appearing
- Clear your browser cache (Ctrl+Shift+R / Cmd+Shift+R)
- Wait ~1 minute for GitHub Pages to rebuild
- Check your commit went through

---

## 📚 Markdown Quick Reference

```markdown
# Heading 1
## Heading 2
### Heading 3

**Bold text**
*Italic text*

[Link text](URL)

- Bullet point
- Another point

1. Numbered list
2. Second item
```

**For more:** [Markdown Guide](https://www.markdownguide.org/basic-syntax/)

---

## 💡 Pro Tips

1. **Keep it updated** - Set a monthly reminder to update your CV
2. **Add PDF versions** - Many programs want downloadable CVs
3. **Link from LinkedIn** - Put your CV website in your LinkedIn profile
4. **Include in email signature** - Share your professional site easily
5. **Mobile-first** - Program directors often view on phones

---

## 🆘 Need Help?

- 📖 **[Full Documentation](https://github.com/anthonyomorada/anthony-morada-cv)** - See working example
- 💬 **[GitHub Discussions](https://github.com/anthonyomorada/am-medical-cv-template/discussions)** - Ask questions
- 🐛 **[Report Issues](https://github.com/anthonyomorada/am-medical-cv-template/issues)** - Found a bug?

---

## 🌟 Examples in the Wild

Using this template? [Submit your site](https://github.com/anthonyomorada/am-medical-cv-template/discussions) to be featured!

- [Anthony Morada, MD](https://anthonyomorada.github.io/anthony-morada-cv/) - General Surgery Resident

---

## 📜 License

Free to use under [MIT License](LICENSE). No attribution required (but appreciated!).

---

## 🙏 Acknowledgments

Created by [Anthony Onde Morada, MD](https://github.com/anthonyomorada) for medical professionals seeking simple, professional online presence.

**Based on:**
- GitHub Pages + Jekyll
- Minima theme
- Markdown formatting

---

**Ready to get started?** Click the **"Use this template"** button at the top! ⬆️
