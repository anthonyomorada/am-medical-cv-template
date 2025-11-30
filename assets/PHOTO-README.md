# Profile Photo Instructions

## Adding Your Profile Photo

Your professional headshot should be placed in this folder and named `profile-photo.png` (or `profile-photo.jpg`).

### Requirements

- **Format:** PNG or JPG
- **Size:** Minimum 400x400 pixels
- **Aspect Ratio:** Square format works best (1:1 ratio)
- **File Size:** Keep under 500KB if possible
- **Quality:** Professional, high-resolution headshot

### How to Add Your Photo

**Option 1: GitHub Web Interface (Easiest)**
1. Go to your repository on GitHub
2. Navigate to the `assets/` folder
3. Click **Add file** → **Upload files**
4. Upload your photo and name it `profile-photo.png`
5. Delete this `PHOTO-README.md` file (it's just a placeholder)
6. Commit the changes

**Option 2: Local Git (Advanced)**
```bash
# Copy your photo to the assets folder
cp /path/to/your/photo.jpg assets/profile-photo.png

# Stage and commit
git add assets/profile-photo.png
git commit -m "Add profile photo"
git push origin main
```

### Photo Tips

- Use a professional headshot with good lighting
- Plain or neutral background works best
- Dress professionally (white coat, business attire)
- Smile naturally
- Crop to focus on your face and shoulders
- Avoid selfies or casual photos

### Temporary Placeholder

Until you add your own photo, the template references `profile-photo.png`. You may see a broken image icon on your site. This will be fixed once you upload your actual photo.

### File Name Reference

The photo is referenced in:
- `index.md` line ~216: `<img src="assets/profile-photo.png" ...>`

If you use a different filename (e.g., `headshot.jpg`), update this line accordingly.
