# B Tubbs & Associates Consulting Website

Professional consulting website built with Jekyll and deployed on GitHub Pages.

## 🚀 Quick Start

### Prerequisites

- Ruby 2.7 or higher
- Bundler gem
- Git

### Local Development

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Add your images:**
   - Copy your downloaded Wix images to the appropriate folders:
     - `assets/images/hero-background.jpg` - Hero background image
     - `assets/images/bill-tubbs-photo.jpg` - Your professional photo
     - `assets/images/services/` - Service page images (5 images)
     - `assets/images/testimonials/` - Testimonial icons (2 .gif files)
     - `assets/images/icons/linkedin.png` - LinkedIn icon

3. **Run locally:**
   ```bash
   bundle exec jekyll serve
   ```

4. **View in browser:**
   Open http://localhost:4000

5. **Make changes:**
   - Edit content in `.md` files
   - Customize styles in `assets/css/main.scss`
   - Add blog posts in `_posts/` folder
   - The site will auto-reload when you save changes

## 📁 Project Structure

```
btubbs-jekyll-site/
├── _config.yml              # Site configuration
├── _layouts/                # Custom layouts
│   └── home.html
├── _posts/                  # Blog posts
│   └── 2024-01-15-welcome.md
├── assets/
│   ├── css/
│   │   └── main.scss        # Custom styles
│   └── images/              # Your images go here
│       ├── hero-background.jpg
│       ├── bill-tubbs-photo.jpg
│       ├── services/
│       ├── testimonials/
│       └── icons/
├── index.md                 # Home page
├── services.md              # Services page
├── testimonials.md          # Testimonials page
├── blog.md                  # Blog page
├── contact.md               # Contact page
├── Gemfile                  # Ruby dependencies
└── README.md                # This file
```

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

Example post format:
```markdown
---
layout: post
title: "Your Post Title"
date: 2024-01-15 10:00:00 -0800
categories: operations optimization
---

Your content here...
```

### Updating Site Information

Edit `_config.yml` to update:
- Site title and description
- Your contact information
- LinkedIn URL
- Other site-wide settings

## 🎨 Customization

### Colors

Edit `assets/css/main.scss` to change colors:
```css
:root {
  --primary-color: #2c5aa0;      /* Main brand color */
  --secondary-color: #4a90e2;    /* Accent color */
  --dark-gray: #333333;          /* Text color */
}
```

### Layout

- Modify `_layouts/` files to change page structure
- Edit `_config.yml` for navigation menu changes

## 🌐 Deploying to GitHub Pages

### Option 1: GitHub.com Repository (Recommended)

1. **Create a new repository on GitHub:**
   - Go to https://github.com/new
   - Name it: `yourusername.github.io` (replace with your GitHub username)
   - Make it public
   - Don't initialize with README (we already have one)

2. **Initialize Git and push:**
   ```bash
   cd btubbs-jekyll-site
   git init
   git add .
   git commit -m "Initial commit - B Tubbs & Associates website"
   git branch -M main
   git remote add origin https://github.com/yourusername/yourusername.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click "Settings" → "Pages"
   - Under "Source", select "Deploy from a branch"
   - Select branch: `main` and folder: `/ (root)`
   - Click "Save"

4. **Wait for deployment:**
   - GitHub will build your site (takes 2-5 minutes)
   - Your site will be live at: `https://yourusername.github.io`

### Option 2: Custom Domain (www.btubbsassociates.com)

1. **Complete steps 1-4 above first**

2. **Configure custom domain on GitHub:**
   - In repository settings → Pages
   - Under "Custom domain", enter: `www.btubbsassociates.com`
   - Click "Save"
   - Enable "Enforce HTTPS" (wait a few minutes after saving domain)

3. **Update DNS with your domain registrar:**

   Add these DNS records:

   **For www.btubbsassociates.com:**
   ```
   Type: CNAME
   Name: www
   Value: yourusername.github.io
   ```

   **For btubbsassociates.com (apex domain):**
   ```
   Type: A
   Name: @
   Value: 185.199.108.153
   
   Type: A
   Name: @
   Value: 185.199.109.153
   
   Type: A
   Name: @
   Value: 185.199.110.153
   
   Type: A
   Name: @
   Value: 185.199.111.153
   ```

4. **Wait for DNS propagation:**
   - Can take 1-48 hours (usually within a few hours)
   - Test at: https://www.whatsmydns.net

5. **Add CNAME file:**
   Create a file named `CNAME` in the root directory:
   ```
   www.btubbsassociates.com
   ```
   Then commit and push:
   ```bash
   echo "www.btubbsassociates.com" > CNAME
   git add CNAME
   git commit -m "Add custom domain"
   git push
   ```

## 🔄 Updating Your Site

After initial deployment, to make changes:

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

## 📋 Image Setup Checklist

After downloading images from Wix, rename and place them as follows:

- [ ] `assets/images/hero-background.jpg` - Touchscreen computer image
- [ ] `assets/images/bill-tubbs-photo.jpg` - Your professional photo
- [ ] `assets/images/services/data-analytics.jpg` - Analyzing data image
- [ ] `assets/images/services/process-control.jpg` - Business meeting image
- [ ] `assets/images/services/energy-management.jpg` - Industrial facility image
- [ ] `assets/images/services/production-optimization.jpg` - Control room image (or use replacement)
- [ ] `assets/images/services/management-control.jpg` - Graphs image
- [ ] `assets/images/testimonials/icon-oil-gas.gif` - Oil & gas facility icon
- [ ] `assets/images/testimonials/icon-mine.gif` - Mine icon
- [ ] `assets/images/icons/linkedin.png` - LinkedIn icon (or use Font Awesome)

**Note:** For the control room image you couldn't download, consider:
- Using a free stock image from Unsplash/Pexels
- Using another relevant image from your collection
- Reaching out to the stock provider

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
- Wait for DNS propagation (can take up to 48 hours)
- Check GitHub Pages settings show "DNS check successful"

## 💰 Cost Comparison

**Previous (Wix):**
- ~$192-420/year

**Current (GitHub Pages):**
- Hosting: $0/year
- Domain: ~$12-15/year (if you own it)
- **Total savings: ~$180-405/year**

## 📞 Support

For questions or issues:
- Edit files in VS Code and test locally first
- Check Jekyll documentation: https://jekyllrb.com/docs/
- Check GitHub Pages docs: https://docs.github.com/pages

## ✅ Pre-Launch Checklist

Before going live:

- [ ] All images added and optimized
- [ ] Contact information updated in `_config.yml`
- [ ] Test all pages locally
- [ ] Test all links work
- [ ] Review on mobile (use browser dev tools)
- [ ] Add more blog posts (optional)
- [ ] Set up custom domain DNS
- [ ] Enable HTTPS on GitHub Pages
- [ ] Test site after deployment

## 📄 License

© 2023 B Tubbs & Associates Consulting
