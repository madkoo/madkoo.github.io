# Madis Koosaar - Personal Profile Site

A simple, elegant static profile site showcasing my professional background, technical expertise, and contact information.

🌐 **Live Site**: [https://madkoo.github.io](https://madkoo.github.io)

## Overview

This is a single-page static website built with clean HTML and CSS, designed to be:
- **Minimal and elegant**: Focus on content without unnecessary clutter
- **Responsive**: Mobile-first design that works on all devices
- **Accessible**: WCAG compliant with semantic HTML and proper contrast
- **Themeable**: Easy to customize colors and typography via CSS variables

## Features

- ✅ Professional introduction and background
- ✅ Tech stack highlights
- ✅ Key certifications display
- ✅ Links to LinkedIn, GitHub, and blog
- ✅ Contact section
- ✅ Dark mode support (automatically adapts to system preferences)
- ✅ Print-friendly styles

## Project Structure

```
madkoo.github.io/
├── index.html          # Main HTML file with content
├── styles.css          # All styling with CSS variables
├── assets/             # Images, icons, and other static files
│   └── README.md       # Guide for adding assets
└── README.md           # This file
```

## Updating Content from Personal README

The content in this site is based on the personal README at [github.com/madkoo/madkoo](https://github.com/madkoo/madkoo). To sync or update content:

### Manual Update Process

1. **Review the source README**:
   ```bash
   # Visit or fetch the content
   curl https://raw.githubusercontent.com/madkoo/madkoo/main/README.md
   ```

2. **Update index.html sections**:
   - **Introduction**: Update the `<header class="hero">` section
   - **About Me**: Update the `<section class="about">` section
   - **Tech Stack**: Update the `<section class="tech-stack">` section
   - **Certifications**: Update the `<section class="certifications">` section
   - **Links**: Update URLs in the `<section class="links">` section

3. **Keep these sections in sync**:
   - Professional title and tagline
   - Current company and role
   - Specializations list
   - Tech stack categories
   - Key certifications
   - Social media links

### Quick Update Checklist

When updating from the personal README:

- [ ] Copy the professional tagline from the README blockquote
- [ ] Update company name and role if changed
- [ ] Sync the specializations list (icons and descriptions)
- [ ] Update tech stack categories and technologies
- [ ] Add/remove certifications as needed
- [ ] Verify all social media and external links are current
- [ ] Test the site locally before committing

### Key Content Mappings

| Personal README Section | index.html Element | Notes |
|------------------------|-------------------|-------|
| Main heading | `.hero h1` | Keep the emoji |
| Blockquote | `.tagline` | The professional summary |
| About Me | `.about` | Company, role, specializations |
| Tech Stack | `.tech-stack` | Technologies by category |
| Certifications | `.certifications` | Key certifications only |
| Connect section | `.links` | LinkedIn, GitHub URLs |

## Customization

### Changing Colors

Edit CSS variables in `styles.css`:

```css
:root {
    --color-primary: #2563eb;      /* Main brand color */
    --color-secondary: #10b981;    /* Secondary actions */
    --color-accent: #8b5cf6;       /* Accent elements */
    /* ... more variables */
}
```

### Changing Typography

Update font variables in `styles.css`:

```css
:root {
    --font-primary: -apple-system, BlinkMacSystemFont, ...;
    --text-base: 1rem;
    --text-lg: 1.125rem;
    /* ... more font settings */
}
```

### Adding a Profile Photo

1. Add your photo to the `assets/` directory
2. Update `index.html` in the hero section:

```html
<header class="hero">
    <img src="assets/profile-photo.jpg" alt="Madis Koosaar" class="profile-photo">
    <h1>👋 Hi, I'm Madis Koosaar</h1>
    <!-- ... rest of content -->
</header>
```

3. Add styling in `styles.css`:

```css
.profile-photo {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    margin: 0 auto var(--space-lg);
    display: block;
    box-shadow: 0 4px 12px var(--color-shadow);
}
```

## Local Development

### Testing Locally

1. **Simple HTTP Server (Python)**:
   ```bash
   python3 -m http.server 8000
   ```
   Open http://localhost:8000 in your browser

2. **Using Node.js**:
   ```bash
   npx http-server -p 8000
   ```

3. **Or just open the file**:
   Open `index.html` directly in your browser (some features like fonts may not load properly)

### Testing Responsiveness

- Use browser DevTools to test different screen sizes
- Test on actual mobile devices when possible
- Verify touch targets are at least 44x44px

### Accessibility Testing

- Use browser DevTools Lighthouse audit
- Test keyboard navigation (Tab, Enter, etc.)
- Verify color contrast ratios meet WCAG AA standards
- Test with a screen reader if possible

## Deployment

This site is automatically deployed via GitHub Pages when you push to the main branch.

### Manual Deployment Steps

1. Commit your changes:
   ```bash
   git add index.html styles.css
   git commit -m "Update profile content"
   ```

2. Push to GitHub:
   ```bash
   git push origin main
   ```

3. Wait a few minutes for GitHub Pages to rebuild

4. Visit https://madkoo.github.io to see your changes

### GitHub Pages Settings

Ensure GitHub Pages is enabled in repository settings:
- Settings → Pages → Source: Deploy from branch → main → root

## Browser Support

This site works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Performance

- No JavaScript dependencies
- Minimal CSS (≈10KB)
- Fast load times (<1s)
- Optimized for Core Web Vitals

## License

This is a personal website. Feel free to use this as a template for your own profile site.

## Maintenance Notes

- **Last major update**: 2026-02-05
- **Content sync with [madkoo/madkoo README](https://github.com/madkoo/madkoo)**: Initial creation
- **Next review**: Update when professional role or certifications change

---

Built with ❤️ and clean code by Madis Koosaar
