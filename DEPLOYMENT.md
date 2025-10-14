# Deployment Guide

This guide will walk you through deploying the Vector Semantic Discovery visualization to GitHub Pages.

## Prerequisites

- GitHub account
- Git installed on your computer (optional - you can use GitHub's web interface)

## Step-by-Step Deployment

### Option 1: Using Git (Recommended)

1. **Create a new repository on GitHub**
   - Go to https://github.com/new
   - Name it: `vector-teaching-tool` (or your preferred name)
   - Description: "Interactive visualization for understanding semantic search and vector embeddings"
   - Make it **Public** (required for free GitHub Pages)
   - Don't initialize with README (we have our own)
   - Click "Create repository"

2. **Initialize and push from your local machine**
   ```bash
   # Navigate to your project folder
   cd C:\Users\brian.crouch\alfa-workshop
   
   # Initialize git (if not already done)
   git init
   
   # Add only the necessary files
   git add index.html README.md LICENSE SOCIAL_MEDIA_GUIDE.md DEPLOYMENT.md
   
   # Make your first commit
   git commit -m "Initial commit: Vector Semantic Discovery visualization"
   
   # Connect to your GitHub repo (replace YOUR_USERNAME)
   git remote add origin https://github.com/YOUR_USERNAME/vector-teaching-tool.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

3. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings" tab
   - Scroll to "Pages" in the left sidebar
   - Under "Source", select "Deploy from a branch"
   - Select branch: `main`
   - Select folder: `/ (root)`
   - Click "Save"

4. **Wait a few minutes**
   - GitHub will build and deploy your site
   - Your site will be live at: `https://brianava.github.io/vector-teaching-tool/`

5. **All set!**
   - The URLs are already configured correctly in the files
   - Commit and push the change:
     ```bash
     git add index.html
     git commit -m "Update URLs with actual GitHub Pages link"
     git push
     ```

### Option 2: Using GitHub Web Interface

1. **Create a new repository on GitHub**
   - Same as above

2. **Upload files**
   - Click "uploading an existing file"
   - Drag and drop:
     - `index.html`
     - `README.md`
     - `LICENSE`
     - `SOCIAL_MEDIA_GUIDE.md`
     - `DEPLOYMENT.md`
   - Commit directly to main branch

3. **Enable GitHub Pages**
   - Same as Option 1, step 3

4. **Update URLs**
   - Edit `index.html` directly on GitHub
   - Replace the URLs in meta tags
   - Commit changes

## Verification

After deployment, verify:

1. ✅ Site loads at your GitHub Pages URL
2. ✅ Visualization is interactive (can drag the red vector)
3. ✅ Terms discover themselves when vectors align
4. ✅ Angle and similarity calculations update in real-time
5. ✅ Mobile responsive (check on your phone)

## Social Sharing Preview

To test how your link will appear when shared:

- **LinkedIn**: Use LinkedIn Post Inspector
- **Twitter**: Share it in a test tweet
- **Facebook**: Use Facebook Sharing Debugger

If images don't show up initially, the platform may need to crawl your site first.

## Custom Domain (Optional)

If you want to use a custom domain instead of github.io:

1. Buy a domain (e.g., from Namecheap, Google Domains)
2. In your repository, create a file named `CNAME`
3. Put your domain in it: `vectordiscovery.yourdomain.com`
4. Configure DNS with your domain provider:
   - Add a CNAME record pointing to `YOUR_USERNAME.github.io`
5. Wait for DNS propagation (can take 24-48 hours)

## Updating the Site

To make changes after deployment:

```bash
# Make your changes to index.html or other files

# Stage changes
git add .

# Commit with a descriptive message
git commit -m "Description of what you changed"

# Push to GitHub
git push

# Site will automatically rebuild in a few minutes
```

## Troubleshooting

### Site not showing up
- Wait 5-10 minutes after enabling GitHub Pages
- Check that repository is public
- Verify the branch and folder are set correctly

### 404 Error
- Ensure `index.html` is in the root directory
- Check file name is exactly `index.html` (case-sensitive on some systems)

### Visualization not working
- Check browser console for JavaScript errors
- Verify D3.js CDN link is loading
- Test in a different browser

### Social sharing preview not working
- URLs in meta tags must be absolute (starting with `https://`)
- Some platforms cache previews - use their debugging tools to refresh

## Security Note

This is a static site with no backend, so there are no security concerns beyond standard web best practices. The visualization runs entirely in the user's browser.

## Support

For issues with:
- **GitHub Pages**: https://docs.github.com/en/pages
- **Git**: https://git-scm.com/doc
- **The visualization itself**: Open an issue in the repository

---

*Ready to deploy? Start with Option 1 if you're comfortable with command line, or Option 2 for a simpler web-based approach.*

