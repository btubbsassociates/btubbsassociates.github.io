# B Tubbs & Associates Consulting Website

Professional consulting website built with Jekyll and deployed on GitHub Pages.

- **Live site:** https://btubbsassociates.com
- **Repository:** https://github.com/btubbsassociates/btubbsassociates.github.io

## 🚀 Quick Start

### Prerequisites

- Ruby 3.3.6 (see `.ruby-version`)
- Bundler gem
- Git

### Local Development

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Run locally:**
   ```bash
   bundle exec jekyll serve
   ```

3. **View in browser:**
   Open http://localhost:4000

4. **Make changes:**
   - Edit content in `.md` files
   - Customize styles in `assets/css/style.scss`
   - Add blog posts in `_posts/` folder
   - The site will auto-reload when you save changes (except `_config.yml`, which needs a server restart)

## 📁 Project Structure

```
btubbsassociates/
├── _config.yml              # Site configuration
├── _includes/               # Reusable page fragments
│   ├── head.html
│   └── footer.html
├── _layouts/                # Custom layouts
│   └── home.html
├── _posts/                  # Blog posts
│   ├── 2023-03-01-welcome.md
│   ├── 2023-03-01-article-short-interval-control.md
│   ├── 2023-03-19-article-choke-model.md
│   ├── 2023-04-22-article-loss-accounting.md
│   ├── 2023-07-09-article-short-interval-control-for-management.md
│   └── 2024-06-16-3-2-1-reporting-control-the-whole-by-controlling-the-parts.md
├── assets/
│   ├── css/
│   │   └── style.scss       # Custom styles
│   └── images/
│       ├── hero-background.jpg
│       ├── bill-tubbs-photo.jpg
│       ├── blog/            # Blog post images and diagrams
│       ├── services/
│       ├── testimonials/
│       └── icons/
├── index.md                 # Home page
├── services.md              # Services page
├── testimonials.md          # Testimonials page
├── blog.md                  # Blog page
├── contact.md               # Contact page
├── CNAME                    # Custom domain for GitHub Pages
├── Gemfile                  # Ruby dependencies
├── Gemfile.lock
├── BRAND_COLORS.md          # Brand colour reference
├── IMAGE_SETUP.md           # Image setup guide
├── QUICKSTART.md            # Quick start guide
├── README.md                # This file
├── dev_guides/              # Development notes (git-ignored)
└── media/                   # Original source images (git-ignored)
```

`README.md`, the other guide files, `dev_guides/` and `media/` are excluded from the site build in `_config.yml`.

## 📝 Content Management

### Editing Pages

All main pages are Markdown files (`.md`). Edit them with any text editor:

- `index.md` - Home page content
- `services.md` - Services descriptions
- `testimonials.md` - Client testimonials
- `contact.md` - Contact information
- `blog.md` - Blog listing page

### Adding Blog Posts

Create new files in `_posts/` folder with this naming format:
```
YYYY-MM-DD-title-of-post.md
```

Posts are published at `/post/<title>` (e.g. `_posts/2023-03-19-article-choke-model.md` → `/post/article-choke-model`), matching the old Wix URLs. Link between posts using these paths.

Example post format:
```markdown
---
layout: post
title: "Your Post Title"
date: 2024-06-16 16:20:00 -0700
categories: operations-management
---

Your content here...

![Descriptive alt text for the image.](/assets/images/blog/your-image.png)
```

`layout: post` and `author: "Bill Tubbs"` are applied by default (see `defaults` in `_config.yml`), so they can be omitted.

Put post images in `assets/images/blog/` using descriptive, hyphenated file names, and give every image alt text.

### Updating Site Information

Edit `_config.yml` to update:
- Site title, description and tagline
- Contact details (email, phone, location, LinkedIn URL) — these appear in the footer
- Navigation menu (`header_pages`)
- Other site-wide settings

## 🎨 Customization

### Colors

Brand colours are defined as CSS variables at the top of `assets/css/style.scss` (see also `BRAND_COLORS.md`):
```css
:root {
  --brand-primary: #262f33;      /* Dark blue-gray (darkest) */
  --brand-secondary: #617b82;    /* Medium blue-gray */
  --brand-accent: #637b83;       /* Light blue-gray */
  --brand-dark: #233237;         /* Very dark blue-gray */
  --brand-light: #66797f;        /* Lighter blue-gray */
}
```

### Layout

- The site uses the `minima` theme, with overrides in `_layouts/` and `_includes/`
- Edit `header_pages` in `_config.yml` to change the navigation menu

## 🌐 Deployment

The site is already deployed on GitHub Pages from the `main` branch of this repository, and the domain https://btubbsassociates.com (set in the `CNAME` file) points to it. No further setup is needed — pushing to `main` publishes changes.

### Updating the Site

```bash
# 1. Make your changes to files
# 2. Test locally
bundle exec jekyll serve

# 3. Commit and push
git add .
git commit -m "Description of changes"
git push

# GitHub Pages will automatically rebuild and deploy (takes 2-5 minutes)
```

## 🛠️ Troubleshooting

### Site not building?
- Check GitHub Actions tab in your repository for build errors
- Verify `_config.yml` syntax (YAML is whitespace-sensitive)
- Make sure all required gems are in Gemfile

### Images not showing?
- Check file paths match exactly (case-sensitive)
- Verify images are in `assets/images/` directory
- Check image file extensions (.jpg vs .jpeg)

### Custom domain not working?
- Verify DNS records are correct
- Check GitHub Pages settings show "DNS check successful"

## 📞 Support

For questions or issues:
- Edit files in VS Code and test locally first
- Check Jekyll documentation: https://jekyllrb.com/docs/
- Check GitHub Pages docs: https://docs.github.com/pages

## 📄 License

© 2023–2026 B Tubbs & Associates Consulting
