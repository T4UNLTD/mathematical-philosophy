# Mathematical Philosophy Through Vaporwave

A GitHub Pages blog exploring mathematical philosophy through vaporwave aesthetics, powered by Jekyll and KaTeX.

## Description

Exploring zero, division, time_0, and simultaneity through the lens of sacred geometry and digital mysticism. This blog uses the "Philosopher-Synthesizer" framework, combining monist ontology, mathematical formalism, phenomenology, and programming metaphors.

## Features

- ✨ **Vaporwave Aesthetics** - Neon pink, cyan, and purple with dark backgrounds
- 🧮 **KaTeX Integration** - Beautiful mathematical notation rendering
- 📱 **Responsive Design** - Works on all devices
- 🎨 **Custom Styling** - VT323 monospace font with glow effects
- ⚡ **Jekyll Powered** - Fast, static site generation

## Setup Instructions

### Prerequisites

1. A GitHub account
2. Git installed on your local machine
3. (Optional) Ruby and Bundler for local development

### Quick Start (GitHub Pages)

1. **Clone or create your repository:**
   ```bash
   git clone https://github.com/your-username/mathematical-philosophy.git
   cd mathematical-philosophy
   ```

2. **Push to GitHub:**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository settings on GitHub
   - Navigate to **Pages** (under "Code and automation")
   - Under **Source**, select "Deploy from a branch"
   - Select **main** branch and **/(root)** directory
   - Click **Save**

4. **Your site is live!**
   - Wait 1-2 minutes for deployment
   - Access at: `https://your-username.github.io/mathematical-philosophy/`

### Local Development (Optional)

If you want to preview changes locally:

1. **Install dependencies:**
   ```bash
   gem install jekyll bundler
   ```

2. **Install theme gems:**
   ```bash
   bundle install
   ```

3. **Start local server:**
   ```bash
   bundle exec jekyll serve
   ```

4. **Visit locally:**
   - Open your browser to `http://localhost:4000`

## Creating Blog Posts

1. Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`

2. Add front matter at the top:
   ```yaml
   ---
   layout: default
   title: Your Post Title
   date: 2026-02-07
   ---
   ```

3. Write your content using Markdown
   - Use `$$...$$` for block math
   - Use `$...$` for inline math
   - KaTeX will auto-render both

### Example Post

```markdown
---
layout: default
title: The Nature of Zero
date: 2026-02-07
---

# The Nature of Zero

Zero is not nothing—it is infinite potential.

Consider the fundamental equation:

$$ \lim_{x \to 0} \frac{1}{x} = \infty $$

This reveals that as we approach zero, we approach the infinite.
```

## Directory Structure

```
mathematical-philosophy/
├── _config.yml              # Jekyll configuration
├── _layouts/
│   └── default.html         # Main layout with KaTeX
├── _includes/
│   ├── head.html            # Head elements
│   ├── footer.html          # Footer content
│   └── navigation.html      # Site navigation
├── _posts/                  # Blog posts (YYYY-MM-DD-title.md)
├── _drafts/                 # Draft posts
├── assets/
│   ├── css/
│   │   └── custom.css       # Vaporwave styling
│   └── images/              # Static images
├── about.md                 # About page
├── index.md                 # Homepage
└── README.md                # This file
```

## Math Notation

This blog uses KaTeX for beautiful mathematical rendering:

### Inline Math
Use single dollar signs: `$E = mc^2$`

Result: $E = mc^2$

### Block Math
Use double dollar signs:
```
$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$
```

Result:
$$
\int_{-\infty}^{\infty} e^{-x^2} dx = \sqrt{\pi}
$$

## Customization

### Colors (in `assets/css/custom.css`)

Edit the CSS variables to customize the color scheme:
```css
:root {
    --neon-pink: #ff6eb8;
    --neon-cyan: #00f0ff;
    --neon-purple: #bc13fe;
    --dark-bg: #0a0a0f;
    /* ... */
}
```

### Site Configuration (in `_config.yml`)

Edit site metadata:
```yaml
title: "Your Site Title"
description: "Your site description"
author: "Your Name"
```

## Deployment

### Automatic Deployment

GitHub Pages automatically builds and deploys when you push to the main branch.

### Custom Domain

To use a custom domain:

1. Create a `CNAME` file in the root directory
2. Add your domain: `yourdomain.com`
3. Configure DNS settings with your domain provider

## Troubleshooting

### Math not rendering?
- Check that KaTeX CDN links are accessible
- Verify math delimiters: `$$...$$` or `$...$`
- Check browser console for errors

### Site not building?
- Verify `_config.yml` syntax (no trailing spaces)
- Check front matter in Markdown files (YAML must be valid)
- Review GitHub Actions logs for build errors

### Styling issues?
- Clear browser cache
- Verify `custom.css` path in `<head>`
- Check for CSS syntax errors

## Resources

- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [KaTeX Documentation](https://katex.org/docs/)
- [GitHub Pages Guide](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)

## License

This project is open source and available under the MIT License.

## Author

**Chris** - *Mathematical Philosophy Through Vaporwave*

---

Built with ❤️, Jekyll, KaTeX, and vaporwave aesthetics.
