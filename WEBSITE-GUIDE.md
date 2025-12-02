# Soil Genesis Website - User Guide

## Overview

Your new website is a single-page, fully responsive HTML file that combines:
- Clean, professional design with earthy, organic aesthetic
- Information about your acoustic soil restoration technology
- Product showcase for Genesis Column AI
- Clear call-to-action for investors and partners
- Mobile-friendly layout

## Quick Start

1. **View the website**: Simply open `soil-genesis-website.html` in any web browser
2. **Deploy online**: Upload the file to any web hosting service (see deployment options below)
3. **Customize**: Edit the HTML file with any text editor

## Easy Customization

### Adding Your Logo

Replace line 267 in the HTML:
```html
<!-- Current: -->
<div class="logo">Soil <span>Genesis</span></div>

<!-- Replace with: -->
<div class="logo"><img src="your-logo.png" alt="Soil Genesis" style="height: 40px;"></div>
```

### Adding Product Images

Replace the placeholder in the product section (around line 457):
```html
<!-- Current placeholder: -->
<div class="product-placeholder">
    Genesis<br>Column AI
</div>

<!-- Replace with: -->
<img src="genesis-column.jpg" alt="Genesis Column AI" style="max-width: 100%; border-radius: 8px;">
```

### Updating Contact Information

Find and replace email addresses (lines 697, 698):
```html
<!-- Current placeholders: -->
<a href="mailto:info@soilgenesis.dao" class="btn btn-white">Request Investment Materials</a>
<a href="mailto:partnerships@soilgenesis.dao" class="btn btn-secondary">Explore Partnership</a>

<!-- Update to your actual emails: -->
<a href="mailto:todd@soilgenesis.com" class="btn btn-white">Request Investment Materials</a>
<a href="mailto:partnerships@soilgenesis.com" class="btn btn-secondary">Explore Partnership</a>
```

### Changing Colors

All colors are defined at the top of the CSS (lines 12-21). Modify these CSS variables:
```css
:root {
    --soil-dark: #2c1810;        /* Dark brown */
    --soil-medium: #5c3d2e;      /* Medium brown */
    --growth-green: #4a7c59;     /* Primary green */
    --vibrant-green: #6b9e78;    /* Accent green */
    /* ... etc */
}
```

### Adding New Sections

To add a new section, copy this template before the CTA section:
```html
<section id="new-section">
    <div class="container">
        <div class="section-header">
            <h2>Your Section Title</h2>
            <p>Your section description</p>
        </div>
        
        <!-- Your content here -->
        
    </div>
</section>
```

Don't forget to add a navigation link:
```html
<li><a href="#new-section">New Section</a></li>
```

## Deployment Options

### Option 1: GitHub Pages (Free, Easy)
1. Create a GitHub account if you don't have one
2. Create a new repository named "soil-genesis-website"
3. Upload `soil-genesis-website.html`
4. Rename it to `index.html`
5. Go to Settings → Pages → Enable GitHub Pages
6. Your site will be live at `https://yourusername.github.io/soil-genesis-website`

### Option 2: Netlify (Free, Professional)
1. Create account at netlify.com
2. Drag and drop your HTML file
3. Get instant deployment with custom domain support
4. Free SSL certificate included

### Option 3: Traditional Web Hosting
1. Purchase hosting from providers like:
   - Bluehost (~$3/month)
   - HostGator (~$3/month)
   - SiteGround (~$4/month)
2. Upload via FTP or hosting control panel
3. Rename to `index.html` for homepage

### Option 4: Vercel (Free, Fast)
1. Create account at vercel.com
2. Import project or drag/drop file
3. Automatic deployment with global CDN
4. Free custom domain support

## Advanced Customization

### Adding Analytics

Add before the closing `</body>` tag:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=YOUR-GA-ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'YOUR-GA-ID');
</script>
```

### Adding a Contact Form

Replace the email buttons with a form service like:
- **Formspree** (formspree.io) - Easy, free tier available
- **Google Forms** - Free, familiar
- **Netlify Forms** - Built into Netlify hosting

Example with Formspree:
```html
<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
    <input type="email" name="email" placeholder="Your email" required>
    <textarea name="message" placeholder="Your message" required></textarea>
    <button type="submit" class="btn btn-primary">Send</button>
</form>
```

### Custom Domain

Most hosting services allow custom domains:
1. Purchase domain (recommended: namecheap.com, google domains)
2. Point DNS to your hosting provider
3. Common domains: soilgenesis.com, soilgenesis.io, soilgenesisdao.com

## Content Updates

### Scientific Data
Update statistics in the Science section (lines 360-380) with your latest research results.

### Product Specifications
Modify the specs list (lines 480-505) as your product evolves.

### Impact Numbers
Update the Impact section (lines 556-575) with real deployment data.

## SEO Optimization

Add these meta tags in the `<head>` section for better search engine visibility:

```html
<meta name="description" content="Soil Genesis DAO - Revolutionary acoustic soil restoration technology using AI and mechanotransduction">
<meta name="keywords" content="soil restoration, acoustic agriculture, mycorrhizal fungi, regenerative farming">
<meta property="og:title" content="Soil Genesis DAO | Acoustic Soil Restoration">
<meta property="og:description" content="Regenerating Earth's living soil through acoustic innovation">
<meta property="og:image" content="https://yoursite.com/preview-image.jpg">
<meta property="og:url" content="https://yoursite.com">
<meta name="twitter:card" content="summary_large_image">
```

## File Structure for Growth

If your site grows, consider splitting into separate files:

```
/
├── index.html          (main page)
├── styles.css          (move CSS here)
├── script.js           (move JavaScript here)
├── images/
│   ├── logo.png
│   ├── product.jpg
│   └── hero-bg.jpg
└── pages/
    ├── about.html
    └── technology.html
```

## Browser Compatibility

This website works on:
- ✅ Chrome (all versions from 2020+)
- ✅ Firefox (all versions from 2020+)
- ✅ Safari (all versions from 2020+)
- ✅ Edge (all versions from 2020+)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

## Performance Tips

1. **Optimize images**: Compress images before uploading (use tinypng.com)
2. **Use WebP format**: Better compression than JPG/PNG
3. **Lazy loading**: Add `loading="lazy"` to image tags
4. **Minify**: Use online tools to minify HTML/CSS for faster loading

## Support & Resources

### Editing Tools
- **VSCode**: Free, powerful code editor (code.visualstudio.com)
- **Sublime Text**: Fast, lightweight editor
- **CodePen**: Online playground for testing changes

### Learning Resources
- **MDN Web Docs**: Comprehensive HTML/CSS reference
- **W3Schools**: Beginner-friendly tutorials
- **CSS-Tricks**: Advanced techniques and guides

### Design Resources
- **Google Fonts**: Free fonts (currently using Crimson Pro + Work Sans)
- **Coolors**: Color palette generator
- **Unsplash**: Free high-quality images

## Backup & Version Control

### Simple Backup
Save dated copies: `soil-genesis-website-2025-11-30.html`

### Professional Version Control (Optional)
Use Git for tracking changes:
```bash
git init
git add soil-genesis-website.html
git commit -m "Initial website"
```

## Next Steps

1. ✅ Review content for accuracy
2. ✅ Add your actual contact information
3. ✅ Upload logo and product images
4. ✅ Choose a deployment method
5. ✅ Test on mobile devices
6. ✅ Share with stakeholders for feedback
7. ✅ Set up analytics
8. ✅ Register custom domain (optional)

## Questions?

The website is designed to be simple and self-contained. Everything you need to customize it is in the single HTML file. Start with small changes and build confidence!

---

**Created for Soil Genesis DAO LLC**  
November 30, 2025
