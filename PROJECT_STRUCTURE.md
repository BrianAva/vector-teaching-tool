# Project Structure

This document outlines the file structure and purpose of each file in the Vector Semantic Discovery repository.

## File Structure

```
vector-semantic-discovery/
│
├── index.html                  # Main visualization (standalone, no dependencies)
├── README.md                   # Project overview and documentation
├── LICENSE                     # MIT License
├── DEPLOYMENT.md              # Step-by-step deployment guide
├── SOCIAL_MEDIA_GUIDE.md      # LinkedIn/Twitter post templates
├── PROJECT_STRUCTURE.md       # This file
└── .gitignore                 # Git ignore rules
```

## File Descriptions

### index.html
**The star of the show.** A self-contained, interactive visualization built with D3.js.

**Key features:**
- No build process needed
- No external dependencies beyond D3.js CDN
- Runs entirely in the browser
- Mobile responsive
- Includes all meta tags for social sharing

**Tech stack:**
- HTML5
- CSS3 (embedded)
- JavaScript (vanilla + D3.js v7)
- D3.js for interactive graphics

**Semantic elements:**
- Actual tax/compliance domain embeddings
- Real-time cosine similarity calculations
- Interactive vector manipulation
- Term discovery system

### README.md
**Public-facing documentation.** This is what people see when they visit your GitHub repo.

**Includes:**
- Project description and goals
- Live demo link
- Usage instructions
- Educational value proposition
- Author attribution (Brian Crouch)
- Avalara branding

**Audience:** Developers, SEO professionals, data scientists, educators

### LICENSE
**MIT License.** Permissive open-source license.

**Key points:**
- Free to use, modify, distribute
- Requires attribution
- No warranty
- Copyright held by Brian Crouch, Avalara

### DEPLOYMENT.md
**Technical deployment guide.** Step-by-step instructions for GitHub Pages.

**Covers:**
- Two deployment methods (Git CLI and web interface)
- GitHub Pages setup
- URL configuration
- Troubleshooting
- Custom domain setup (optional)

**Audience:** Anyone deploying the visualization

### SOCIAL_MEDIA_GUIDE.md
**Marketing playbook.** Ready-to-use social media content.

**Includes:**
- 3 LinkedIn post templates
- Twitter post suggestions
- Video demo script
- Timing recommendations
- Hashtag strategy
- Engagement tips

**Audience:** Marketing, social media managers

### .gitignore
**Git configuration.** Prevents committing unnecessary files.

**Excludes:**
- OS-specific files (.DS_Store, Thumbs.db)
- Editor configs (.vscode, .idea)
- Temporary files (*.tmp, *.bak)
- Log files

## Design Principles

### 1. Simplicity
- Single HTML file for the visualization
- No build process
- No package managers
- No frameworks beyond D3.js

### 2. Accessibility
- Semantic HTML
- Clear visual hierarchy
- Responsive design
- Keyboard navigation support

### 3. Performance
- Lightweight (HTML file < 100KB)
- Loads in < 1 second on good connection
- No external API calls
- Runs entirely client-side

### 4. Shareability
- Comprehensive meta tags
- Social media optimized
- LLM-readable context
- Professional branding

## Maintenance

### When to update index.html:
- Bug fixes or improvements
- New semantic terms to discover
- Visual design updates
- Performance optimizations

### When to update README.md:
- New features added
- Usage instructions change
- Contact information updates
- Links change

### When to update SOCIAL_MEDIA_GUIDE.md:
- New social media best practices
- Platform algorithm changes
- Better post templates discovered
- Community feedback

## Technical Notes

### Browser Compatibility
- **Modern browsers:** Full support (Chrome, Firefox, Safari, Edge)
- **IE11:** Not supported (uses ES6 features)
- **Mobile:** Full support on iOS Safari and Chrome Android

### Dependencies
- D3.js v7 (loaded from CDN)
- No other external dependencies

### Performance Considerations
- All calculations done in JavaScript
- No database queries
- No server-side processing
- Scales well to 100+ semantic terms

### Future Enhancement Ideas
- [ ] Add more semantic domains (not just tax/compliance)
- [ ] Export discovered terms as CSV
- [ ] Share specific configurations via URL params
- [ ] 3D version with additional dimension
- [ ] Tutorial overlay for first-time users
- [ ] Dark mode toggle
- [ ] Animation presets

## Contributing

If others want to contribute:
1. Fork the repository
2. Create a feature branch
3. Make changes
4. Test thoroughly in multiple browsers
5. Submit a pull request with clear description

## Support

For questions or issues:
- **GitHub Issues:** For bugs or feature requests
- **LinkedIn:** Contact Brian Crouch for professional inquiries
- **Avalara:** For partnership or enterprise use cases

---

*This structure is designed to be minimal yet complete - everything you need, nothing you don't.*

