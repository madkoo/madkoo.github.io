# Madis Koosaar - Personal Profile Site

A simple, elegant static profile site showcasing Madis Koosaar's professional background, skills, and connections.

## 🌐 Live Site

Visit the live site at: [https://madkoo.github.io](https://madkoo.github.io)

## 📋 Overview

This is a single-page static website built with pure HTML and CSS. It features:

- **Clean Design**: Modern, minimal aesthetic with focus on readability
- **Responsive Layout**: Mobile-first design that works on all devices
- **Accessibility**: WCAG compliant with proper semantic HTML and focus states
- **Easy Theming**: CSS variables for quick color and typography changes
- **Dark Mode Support**: Automatic dark mode based on user preferences

## 📁 Site Structure

```
madkoo.github.io/
├── index.html          # Main HTML file with content
├── styles.css          # All styling and responsive design
├── assets/             # Directory for images and icons
│   └── README.md       # Instructions for assets
└── README.md           # This file
```

## 🔄 Syncing Content from Personal README

The content in this site is based on the personal README at [github.com/madkoo/madkoo](https://github.com/madkoo/madkoo). To update the content:

### Manual Update Process

1. **Visit the source README**
   ```bash
   # View the latest content at:
   https://github.com/madkoo/madkoo/blob/main/README.md
   ```

2. **Identify sections to update**
   - Introduction and tagline
   - About Me section
   - Tech Stack
   - Certifications
   - Contact links

3. **Edit index.html**
   - Open `index.html` in your text editor
   - Locate the corresponding section (look for HTML comments like `<!-- About Section -->`)
   - Update the text content within the appropriate HTML tags
   - Keep the HTML structure intact, only change the text

4. **Common sections to update:**

   **Header/Introduction:**
   ```html
   <h1 class="header__title">👋 Hi, I'm Madis Koosaar</h1>
   <p class="header__tagline">Your tagline here...</p>
   ```

   **About section:**
   ```html
   <section class="about">
       <h2 class="section__title">🚀 About Me</h2>
       <p class="about__text">Update your intro here...</p>
       <ul class="about__list">
           <li>Update specialization points...</li>
       </ul>
   </section>
   ```

   **Tech Stack:**
   ```html
   <div class="tech-stack__item">
       <h3>Category Name</h3>
       <p>Technologies list</p>
   </div>
   ```

   **Links:**
   ```html
   <a href="YOUR_URL" class="link-card" target="_blank">
       <span class="link-card__icon">🐙</span>
       <span class="link-card__text">Link Text</span>
   </a>
   ```

5. **Test your changes**
   - Open `index.html` in a web browser
   - Check on mobile and desktop views
   - Verify all links work correctly

6. **Commit and push**
   ```bash
   git add index.html
   git commit -m "Update profile content from personal README"
   git push origin main
   ```

### Automated Update (Optional Future Enhancement)

For more frequent updates, consider setting up a GitHub Action that:
1. Fetches content from your personal README
2. Parses the markdown
3. Updates specific sections in index.html
4. Creates a pull request with changes

## 🎨 Customizing the Design

### Changing Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --color-primary: #0969da;           /* Main brand color */
    --color-text: #1f2328;              /* Main text color */
    --color-background: #ffffff;         /* Background color */
    /* ... other variables */
}
```

### Changing Typography

Update font variables:

```css
:root {
    --font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', ...;
    --font-size-base: 16px;
    --font-size-large: 1.25rem;
    /* ... other font variables */
}
```

### Modifying Layout

Adjust spacing variables:

```css
:root {
    --spacing-xs: 0.5rem;
    --spacing-sm: 1rem;
    --spacing-md: 1.5rem;
    --spacing-lg: 2rem;
    --spacing-xl: 3rem;
}
```

## 📱 Responsive Design

The site uses a mobile-first approach with breakpoints at:
- **Mobile**: < 480px
- **Tablet**: < 768px
- **Desktop**: > 768px

All layouts automatically adjust using CSS Grid and Flexbox.

## ♿ Accessibility Features

- Semantic HTML5 structure
- ARIA labels where appropriate
- Keyboard navigation support
- Focus indicators for interactive elements
- Sufficient color contrast ratios
- Responsive text sizing
- Support for reduced motion preferences

## 🚀 Deployment

This site is automatically deployed to GitHub Pages from the `main` branch.

### GitHub Pages Configuration

1. Go to repository Settings → Pages
2. Source: Deploy from branch `main`
3. Folder: `/ (root)`
4. Save

Changes pushed to main are live within minutes.

## 🛠️ Development

### Local Development

Simply open `index.html` in your browser. No build process required!

For live reload during development, you can use:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx http-server

# Then visit http://localhost:8000
```

## 📝 Content Guidelines

When updating content:

1. **Keep it concise**: The site should be scannable
2. **Update links regularly**: Ensure all external links work
3. **Maintain consistency**: Match the tone of the personal README
4. **Test responsiveness**: Check on mobile after changes
5. **Verify accessibility**: Use browser dev tools to check accessibility

## 🤝 Contributing

This is a personal site, but suggestions are welcome:

1. Open an issue for discussion
2. Fork the repository
3. Make your changes
4. Submit a pull request

## 📄 License

© 2026 Madis Koosaar. All rights reserved.

## 📞 Questions?

For questions or suggestions, reach out via:
- GitHub: [@madkoo](https://github.com/madkoo)
- LinkedIn: [Madis Koosaar](https://www.linkedin.com/in/madiskoosaar/)
