# CV Downloads

This folder contains downloadable versions of your CV in PDF and Word formats.

## Files

- `cv.pdf` - PDF version (generated from cv.md)
- `cv.docx` - Word document version (generated from cv.md)

## Generating CV Files

To generate or update these files:

1. Make sure you have the required tools installed:
   - Pandoc: `brew install pandoc` (macOS) or see [pandoc.org](https://pandoc.org/installing.html)
   - LaTeX (for PDF): `brew install --cask mactex` (macOS)

2. Run the conversion script:
   ```bash
   python3 assets/convert_cv.py
   ```

3. The script will automatically generate both PDF and Word versions from your `cv.md` file

## Manual Conversion

Alternatively, you can convert manually using pandoc:

```bash
# Convert to PDF
pandoc cv.md -o cv-downloads/cv.pdf --variable geometry:margin=0.75in --variable fontsize=11pt

# Convert to Word
pandoc cv.md -o cv-downloads/cv.docx
```

## Note

These files are automatically linked from your website's homepage for easy downloading by visitors.
