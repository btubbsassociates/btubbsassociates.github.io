# Quick Start Guide

## 1️⃣ Extract and Open in VS Code

1. Extract the `btubbs-jekyll-site` folder
2. Open VS Code
3. File → Open Folder → Select `btubbs-jekyll-site`

## 2️⃣ Add Your Images

Follow the instructions in `IMAGE_SETUP.md` to copy your Wix images into the correct folders.

## 3️⃣ Install Jekyll (First Time Only)

**macOS:**
```bash
# Install Homebrew if you don't have it
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Ruby
brew install ruby

# Add Ruby to PATH (add to ~/.zshrc or ~/.bash_profile)
export PATH="/usr/local/opt/ruby/bin:$PATH"

# Install Bundler
gem install bundler
```

**Windows:**
```bash
# Install Ruby using RubyInstaller
# Download from: https://rubyinstaller.org/
# Choose Ruby+Devkit version
# Run the installer and select "Add Ruby to PATH"

# After installation, open Command Prompt and run:
gem install bundler
```

## 4️⃣ Install Dependencies

In VS Code terminal (or any terminal in the site directory):

```bash
cd btubbs-jekyll-site
bundle install
```

## 5️⃣ Run Locally

```bash
bundle exec jekyll serve
```

Open browser to: http://localhost:4000

The site will auto-reload when you make changes!

## 6️⃣ Make Changes

- Edit `.md` files to change content
- Edit `_config.yml` to change site settings
- Add blog posts to `_posts/` folder
- Customize colors in `assets/css/main.scss`

## 7️⃣ Deploy to GitHub Pages

### First Time Setup:

1. **Create GitHub account** (if you don't have one): https://github.com/join

2. **Create new repository:**
   - Go to: https://github.com/new
   - Repository name: `yourusername.github.io` (replace yourusername)
   - Make it Public
   - Don't initialize with README

3. **In VS Code terminal, run these commands:**

```bash
# Initialize git
git init

# Add all files
git add .

# Make first commit
git commit -m "Initial commit - B Tubbs & Associates website"

# Set main branch
git branch -M main

# Add your GitHub repository (replace with YOUR username)
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git push -u origin main
```

4. **Enable GitHub Pages:**
   - Go to your repository on GitHub
   - Click Settings → Pages
   - Source: Deploy from branch `main` / folder `/ (root)`
   - Click Save

5. **Wait 2-5 minutes**, then visit: `https://yourusername.github.io`

### Updating Your Site:

After making changes:

```bash
git add .
git commit -m "Description of what you changed"
git push
```

GitHub will automatically rebuild and deploy (takes 2-5 minutes).

## 8️⃣ Set Up Custom Domain (Optional)

Once the basic site is working:

1. **In GitHub repository → Settings → Pages:**
   - Custom domain: `www.btubbsassociates.com`
   - Save

2. **Update DNS at your domain registrar:**

   Add CNAME record:
   ```
   Type: CNAME
   Name: www
   Value: yourusername.github.io
   ```

3. **Wait for DNS propagation** (1-24 hours)

4. **Enable HTTPS** in GitHub Pages settings

Full DNS instructions are in README.md

## 🆘 Common Issues

**"Bundle not found"**
```bash
gem install bundler
bundle install
```

**Port 4000 already in use**
```bash
bundle exec jekyll serve --port 4001
```

**Images not showing locally**
- Check file paths are correct
- File names are case-sensitive
- Use forward slashes (/) not backslashes (\)

**Site not deploying to GitHub**
- Check GitHub Actions tab for errors
- Verify _config.yml has no syntax errors
- Make sure all files are committed and pushed

## 📚 Learn More

- Jekyll Docs: https://jekyllrb.com/docs/
- GitHub Pages: https://docs.github.com/pages
- Markdown Guide: https://www.markdownguide.org/

## ✅ Checklist

- [ ] Extracted site folder
- [ ] Opened in VS Code
- [ ] Added all images
- [ ] Installed Ruby and Bundler
- [ ] Ran `bundle install`
- [ ] Tested locally with `bundle exec jekyll serve`
- [ ] Created GitHub repository
- [ ] Pushed to GitHub
- [ ] Enabled GitHub Pages
- [ ] Site is live!

---

**Need help?** Check README.md for detailed instructions or troubleshooting.
