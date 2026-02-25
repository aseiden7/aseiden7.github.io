# Personal Website Guide

Welcome to your new personal website! This site features a beautiful dark theme with an image slideshow, CV page, and social media links.

## 🎨 Customization Guide

### 1. Update Your Personal Information

Edit `_config.yml` to add your information:

```yaml
title: Your Name
email: your.email@example.com
description: Your bio/tagline
url: "https://aseiden7.github.io"

social:
  twitter: your_twitter
  github: aseiden7
  linkedin: your-linkedin
  instagram: your_instagram
  email: your.email@example.com
```

**Note:** After editing `_config.yml`, restart the Jekyll server for changes to take effect.

### 2. Add Slideshow Images

Place your images in the `/assets/images/` folder:
- `slide1.jpg` - First slideshow image
- `slide2.jpg` - Second slideshow image
- `slide3.jpg` - Third slideshow image

**Tips for best results:**
- Use high-quality images (recommended: 1920x1080 or similar aspect ratio)
- Images will be cropped to fit, so center important content
- JPG or PNG formats work best

**To add more slides:**
1. Add more images to `/assets/images/`
2. Edit `index.markdown` to add more slide divs
3. Add corresponding dots in the dots-container

### 3. Update Your CV

Edit `cv.markdown` to add your:
- Education history
- Work experience
- Skills
- Projects & publications
- Awards

**To add a downloadable PDF:**
1. Place your CV PDF in `/assets/` folder
2. Update the download button link in `cv.markdown`

### 4. Customize the About Page

Edit `about.markdown` to tell your story.

### 5. Update the Homepage

Edit `index.markdown` to:
- Change the welcome message
- Add your introduction
- Customize the call-to-action buttons

## 🚀 Running Locally

```bash
cd /Users/adrianneseiden/Documents/jekyll-site/aseiden7.github.io
bundle exec jekyll serve
```

Visit: http://localhost:4000

## 📤 Publishing Changes

After making changes:

```bash
git add .
git commit -m "Update website content"
git push origin main
```

Your site will update at https://aseiden7.github.io within a few minutes.

## 🎨 Styling

Custom styles are in `/assets/css/custom.css`. You can:
- Change colors
- Adjust fonts
- Modify button styles
- Update slideshow dimensions

## 📁 File Structure

```
.
├── _config.yml          # Site configuration
├── _layouts/            # Page templates
│   ├── default.html     # Main layout with header/footer
│   ├── home.html        # Homepage layout
│   ├── page.html        # Standard page layout
│   └── post.html        # Blog post layout
├── _includes/           # Reusable components
│   └── head-custom.html # Custom head elements
├── assets/
│   ├── css/
│   │   └── custom.css   # Your custom styles
│   ├── js/
│   │   └── slideshow.js # Slideshow functionality
│   └── images/          # Your images for slideshow
├── index.markdown       # Homepage
├── about.markdown       # About page
└── cv.markdown          # CV page
```

## 🆘 Need Help?

- Jekyll documentation: https://jekyllrb.com/docs/
- GitHub Pages docs: https://docs.github.com/en/pages
- Midnight theme: https://github.com/pages-themes/midnight

## ✨ Tips

1. **Images not loading?** Make sure filenames match exactly (case-sensitive)
2. **Changes not showing?** Hard refresh: `Cmd + Shift + R`
3. **Config changes?** Restart Jekyll server
4. **Slideshow not working?** Check browser console for errors

Enjoy your new website! 🎉
