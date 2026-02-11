# LDA-1B Project Website

Official website for the LDA-1B project: Scaling Latent Dynamics Action Model via Universal Embodied Data Ingestion

## Deployment to lda-1b.github.io

### Option 1: GitHub Organization (Recommended)

1. **Create a GitHub Organization**:
   - Go to https://github.com/organizations/new
   - Organization name: `lda-1b`
   - Create organization

2. **Create the repository**:
   - In the organization, create a new repository
   - Repository name: `lda-1b.github.io` (must be exactly this)
   - Make it public
   - Don't initialize with README

3. **Push the website**:
   ```bash
   cd /Users/catburg/lda-1b-website
   git init
   git add .
   git commit -m "Initial commit: LDA-1B project website"
   git branch -M main
   git remote add origin https://github.com/lda-1b/lda-1b.github.io.git
   git push -u origin main
   ```

4. **Access your site**:
   - Your website will be live at: `https://lda-1b.github.io`
   - No additional GitHub Pages configuration needed!

### Option 2: Personal Account with Custom Domain

If you want to use a personal account:

1. Create repository: `yourusername/lda-1b`
2. Enable GitHub Pages in Settings → Pages
3. Site will be at: `https://yourusername.github.io/lda-1b/`
4. (Optional) Set up custom domain `lda-1b.github.io` via DNS

## Local Preview

```bash
cd /Users/catburg/lda-1b-website
python3 -m http.server 8000
```

Open `http://localhost:8000` in your browser.

## File Structure

```
lda-1b-website/
├── index.html          # Main HTML file
├── style.css           # Stylesheet
├── videos/             # 30 demo videos
├── images/             # Figures from LaTeX sources
│   ├── lda_teaser.png  # Main teaser image
│   ├── demo.png        # Model architecture
│   ├── dataset.png     # EI-30k dataset
│   ├── dex_demo.png    # Experimental results
│   └── ...             # Other figures
└── README.md           # This file
```

## Next Steps

1. ✅ Images integrated from LaTeX sources
2. ✅ Academic template footer with proper attribution
3. ✅ All 30 demo videos organized
4. ⏳ Deploy to lda-1b.github.io (follow instructions above)
5. ⏳ Add institutional affiliations
6. ⏳ Update Paper/Code/Models links when available

## Credits

This page was built using the [Academic Project Page Template](https://github.com/eliahuhorwitz/Academic-project-page-template) which was adopted from the [Nerfies](https://nerfies.github.io/) project page.

This website is licensed under a [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/).
