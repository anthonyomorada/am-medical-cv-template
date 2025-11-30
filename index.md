---
layout: default
---

<style>
:root {
  --primary-color: #2c5aa0;
  --primary-dark: #1a3a5c;
  --light-bg: #f8f9fa;
  --text-dark: #1a3a5c;
  --link-color: var(--primary-color);
  --link-visited: var(--primary-dark);
}

body {
  font-size: 16px;
  line-height: 1.6;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  color: var(--text-dark);
}

a {
  color: var(--link-color);
  text-decoration: none;
}

a:visited {
  color: var(--link-visited);
}

a:hover {
  text-decoration: underline;
}

/* Tighter paragraph and heading spacing */
p {
  margin: 0.7em 0;
}

h2 {
  margin-top: 1.1em;
  margin-bottom: 0.7em;
  border-bottom: none;
  padding-bottom: 0;
}

h1 {
  border-bottom: none;
  padding-bottom: 0;
}

hr {
  margin: 1em 0;
}

.hero-tagline {
  font-size: 1.2em;
  color: var(--text-dark);
  margin-bottom: 14px;
}

.stat-card p {
  margin: 10px 0 0 0;
  font-size: 0.95em;
  color: var(--text-dark);
}

.featured-item .meta {
  color: var(--text-dark);
  font-size: 0.9em;
  margin: 10px 0;
}

.contact-badges {
  display: flex;
  gap: 8px;
  justify-content: center;
  flex-wrap: wrap;
  margin: 0px 0px;
}

.hero-section {
  text-align: center;
  padding: 18px 0 10px;
  margin-bottom: 8px;
}

.hero-section h1 {
  font-size: 2.5em;
  margin-bottom: 10px;
  color: var(--text-dark);
}

/* Stats grid - tighter spacing */
.stats-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 16px;
  margin: 20px 0;
}

.stat-card {
  text-align: center;
  padding: 16px;
  background: var(--light-bg);
  border-radius: 8px;
  border-left: 4px solid var(--primary-color);
}

.stat-card h3 {
  font-size: 2.5em;
  margin: 0;
  color: var(--primary-color);
}

.nav-cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  gap: 16px;
  margin: 18px 0;
}

.nav-card {
  display: block;
  padding: 10px 16px;
  background: var(--primary-color);
  color: white;
  text-align: center;
  text-decoration: none;
  border-radius: 8px;
  font-weight: bold;
  font-size: 1.1em;
  min-height: 48px;
  transition: background 0.3s ease;
}

.nav-card:visited {
  color: white;
}

.nav-card:hover {
  background: var(--primary-dark);
  color: white;
}

.featured-section {
  margin: 30px 0;
}

.featured-item {
  margin: 20px 0;
  padding: 20px;
  border-left: 4px solid var(--primary-color);
  background: var(--light-bg);
}

.featured-item h3 {
  margin-top: 0;
  color: var(--primary-color);
}

.featured-item .description {
  margin: 15px 0;
  line-height: 1.6;
}

.awards-list {
  display: grid;
  gap: 15px;
  margin: 20px 0;
}

.award-item {
  padding: 15px 20px;
  background: var(--light-bg);
  border-radius: 6px;
  border-left: 4px solid var(--primary-color);
}

.award-item strong {
  color: var(--primary-color);
}

/* Mobile responsive */
@media (max-width: 768px) {
  body {
    font-size: 15px;
  }

  .hero-section {
    padding: 16px 0 12px;
    margin-bottom: 12px;
  }

  .hero-section h1 {
    font-size: 1.8em;
  }

  .stats-grid {
    grid-template-columns: repeat(2, 1fr);
    margin: 18px 0;
  }

  .nav-cards {
    grid-template-columns: 1fr;
    margin: 18px 0;
  }

  .featured-section {
    margin: 20px 0;
  }
}
</style>

<div class="hero-section">
  <img src="assets/profile-photo.png" alt="[Your Name] - Professional headshot" style="max-width: 200px; border-radius: 50%; margin: 0 auto 20px; display: block;">
  <h1>[Your Full Name], MD</h1>
  <p class="hero-tagline">[Your Position] | [Your Specialty/Research Focus]</p>
  <p>[Your Institution/Program Name]<br>
  [Previous Institution (Optional)] | [Other Affiliations (Optional)]</p>

  <div class="contact-badges">
    <a href="https://orcid.org/0000-0000-0000-0000" target="_blank">
      <img src="https://img.shields.io/badge/ORCID-0000--0000--0000--0000-green?style=flat-square&logo=orcid" alt="ORCID">
    </a>
    <a href="https://linkedin.com/in/yourlinkedin" target="_blank">
      <img src="https://img.shields.io/badge/LinkedIn-yourlinkedin-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn">
    </a>
   <a href="https://github.com/yourgithub" target="_blank">
      <img src="https://img.shields.io/badge/GitHub-yourgithub-black?style=flat-square&logo=github" alt="GitHub">
    </a>
  </div>
</div>

---

## 📄 Quick Navigation

<div class="nav-cards">
  <a href="cv.html" class="nav-card">
    📋 View Full CV
  </a>
  <a href="cv-downloads/cv.pdf" class="nav-card" download>
    📥 Download PDF
  </a>
  <a href="cv-downloads/cv.docx" class="nav-card" download>
    📝 Download Word
  </a>
</div>

<p style="text-align: center; color: var(--text-dark); font-size: 0.9em; margin-top: 10px;">
  <em>Last Updated: [Month Year]</em><br>
  <a href="cv.html">View Full CV</a> • <a href="cv-downloads/">Download CV Files</a>
</p>

---

## 📬 Contact

**Institutional Email:** [institutional.email@institution.edu](mailto:institutional.email@institution.edu)
**Personal Email:** [your.email@example.com](mailto:your.email@example.com)
**Phone:** +1 (XXX) XXX-XXXX
**ORCID:** [0000-0000-0000-0000](https://orcid.org/0000-0000-0000-0000) • **LinkedIn:** [yourlinkedin](https://linkedin.com/in/yourlinkedin) • **GitHub:** [yourgithub](https://github.com/yourgithub)

---

## 📊 [Your Field] Impact at a Glance

<div class="stats-grid">
  <div class="stat-card">
    <h3>[#]</h3>
    <p>[Metric Description]<br>[Sub-description]</p>
  </div>
  <div class="stat-card">
    <h3>[#]</h3>
    <p>[Metric Description]<br>[Sub-description]</p>
  </div>
  <div class="stat-card">
    <h3>[#]</h3>
    <p>[Metric Description]<br>[Sub-description]</p>
  </div>
  <div class="stat-card">
    <h3>[#]</h3>
    <p>[Metric Description]<br>[Sub-description]</p>
  </div>
</div>

---

## 🎯 Research Focus

**[Area 1] • [Area 2] • [Area 3]**

[2-3 sentences describing your overall research focus and experience. Highlight key projects, areas of expertise, or methodologies you use. Connect your past work to your current interests and future goals.]

**Key Areas:**
- [Specific research area or methodology]
- [Specific research area or methodology]
- [Specific research area or methodology]
- [Specific research area or methodology]

---

## 🔬 Selected Publications

1. **[Your Initials]**, [Co-authors]. [Article title]. *[Journal Name]*. [Year];[Volume]([Issue]):[Pages]. PMID: [PMID]. [[PDF](publications/your-paper.pdf)] [[PubMed](https://pubmed.ncbi.nlm.nih.gov/PMID/)]

2. **[Your Initials]**, [Co-authors]. [Article title]. *[Journal Name]*. [Year];[Volume]([Issue]):[Pages]. [[Preprint](https://doi.org/DOI)]

3. [Co-author], **[Your Initials]**, [Co-authors]. [Article title]. *[Journal Name]*. [Year];[Volume]([Issue]):[Pages]. PMID: [PMID]. [[PubMed](https://pubmed.ncbi.nlm.nih.gov/PMID/)]

**[→ View all publications in full CV](cv.html#publications)**

---

## 💼 [Research/Clinical] Experience Highlights

### **[Institution Name]** ([Start Year]-[End Year])
**[Position Title]** • [Department/Program Name]

- [Key responsibility or achievement with specific details]
- [Key responsibility or achievement with specific details]
- [Key responsibility or achievement with specific details]
- [Key responsibility or achievement with specific details]

### **[Institution Name]** ([Start Year]-[End Year])
**[Position Title]** • [Department/Program Name]

- [Key responsibility or achievement with specific details]
- [Key responsibility or achievement with specific details]
- [Key responsibility or achievement with specific details]

**[→ View Full Experience Timeline in CV](cv.html#research-experience)**

---

## 🏆 Selected Recognition

<div class="awards-list">
  <div class="award-item">
    <strong>[Award Name or Achievement]</strong><br>
    [Awarding Organization or Context] ([Year])
  </div>
  <div class="award-item">
    <strong>[Award Name or Achievement]</strong><br>
    [Awarding Organization or Context] ([Year])
  </div>
  <div class="award-item">
    <strong>[Award Name or Achievement]</strong><br>
    [Awarding Organization or Context] ([Year])
  </div>
  <div class="award-item">
    <strong>[Award Name or Achievement]</strong><br>
    [Awarding Organization or Context] ([Year])
  </div>
</div>

---

## 🎓 Professional Memberships

- **[Professional Organization Name]** ([Abbreviation])
- **[Professional Organization Name]** ([Abbreviation])
- **[Professional Organization Name]**
- **[Professional Organization Name]**
