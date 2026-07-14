# ReBind GitHub Pages

This is the project page for **ReBind: Multi-Reference Video Editing via Structured Instructions with Explicit Reference Relationships** (CVPR 2026).

## 🌐 Live Demo

Visit the project page at: `https://your-username.github.io/rebind`

## 📁 Structure

```
rebind-github-page/
├── index.html              # Main page
├── static/
│   ├── css/               # Stylesheets (Bulma framework)
│   ├── js/                # JavaScript files
│   ├── images/            # Images (teaser, method, results, etc.)
│   └── videos/            # Demo videos
└── README.md              # This file
```

## 🚀 Setup Instructions

### Option 1: GitHub Pages (Recommended)

1. Create a new repository named `rebind` (or any name you prefer)
2. Copy all files from `rebind-github-page/` to the repository root
3. Push to GitHub:
   ```bash
   git add .
   git commit -m "Add project page"
   git push origin main
   ```
4. Enable GitHub Pages:
   - Go to repository Settings → Pages
   - Source: Deploy from a branch
   - Branch: `main` / `root`
   - Save
5. Your site will be live at `https://your-username.github.io/rebind`

### Option 2: Local Preview

```bash
# Using Python's built-in HTTP server
cd rebind-github-page
python3 -m http.server 8000

# Visit http://localhost:8000 in your browser
```

## 📝 Content to Add

Before publishing, you need to add the following content:

### 1. Images (place in `static/images/`)
- `teaser.png` - Main teaser figure showing the key idea
- `method.png` - Method overview diagram
- `instruction_comparison.png` - Comparison between basic and dense instructions
- `results_intelligentbench.png` - Quantitative results table for IntelligentVBench
- `results_univbench.png` - Quantitative results table for UniVBench
- `ablation.png` - Ablation study results
- `rebind-logo.png` - Project logo (favicon)

### 2. Videos (place in `static/videos/`)
- `demo1.mp4` - Multi-reference character replacement example
- `demo2.mp4` - Object and style editing example
- `demo3.mp4` - Background and lighting example
- `demo4.mp4` - Complex multi-entity editing example

### 3. Update Links in `index.html`
- Line 70: Update arXiv link once paper is published
- Line 79: Update GitHub repository link
- Line 88: Update HuggingFace model link
- Line 53-56: Update author information (remove "Anonymous")
- Line 61: Update institution
- Line 358: Update BibTeX citation

## 🎨 Customization

### Colors
The main accent color is `#FF6B6B` (red). To change:
- Search for `#FF6B6B` in `index.html` and replace with your preferred color

### Fonts
The page uses Google Sans and Noto Sans. To change:
- Update the `<link>` tag in the `<head>` section

### Layout
The page uses Bulma CSS framework. Refer to [Bulma documentation](https://bulma.io/documentation/) for customization.

## 📊 Adding More Results

To add more video examples:

```html
<div class="column is-half">
  <video controls autoplay loop muted style="width: 100%; border-radius: 10px;">
    <source src="static/videos/your_video.mp4" type="video/mp4">
  </video>
  <p class="has-text-centered" style="margin-top: 10px;"><i>Your description</i></p>
</div>
```

## 🐛 Troubleshooting

### Videos not playing
- Ensure videos are in MP4 format (H.264 codec)
- Check file paths are correct
- Try reducing video file sizes (GitHub Pages has 100MB file limit)

### Images not showing
- Verify image paths match the directory structure
- Check image formats (PNG, JPG, WebP are supported)
- Ensure images are optimized for web (< 1MB per image)

### GitHub Pages not updating
- Wait 5-10 minutes after pushing changes
- Clear browser cache
- Check GitHub Actions tab for build status

## 📄 License

This project page template is adapted from [Nerfies](https://github.com/nerfies/nerfies.github.io).

## 🙏 Acknowledgments

- Design inspired by [DreamVideo-Omni](https://dreamvideo-omni.github.io)
- Built with [Bulma CSS framework](https://bulma.io)
