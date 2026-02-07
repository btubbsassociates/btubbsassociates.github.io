# Fixing Footer and Colors

## The Problems

1. **Footer showing raw YAML data** - The default Minima theme doesn't properly format custom author fields
2. **No colors visible** - The CSS file needs to be named `style.scss` not `main.scss`

## The Fixes

### Step 1: Create _includes folder

In your `btubbsassociates` folder, create the following structure:

```
btubbsassociates/
├── _includes/
│   ├── footer.html
│   └── head.html
```

Copy the files I provided into this folder.

### Step 2: Fix CSS filename

Rename your CSS file:

```bash
cd ~/btubbsassociates
mv assets/css/main.scss assets/css/style.scss
```

OR delete the old one and use the new one I provided:
```bash
rm assets/css/main.scss
# Then copy the style.scss file I provided to assets/css/
```

### Step 3: Stop and restart Jekyll

```bash
# Stop Jekyll (Ctrl+C if it's running)

# Restart it
bundle exec jekyll serve
```

## Quick Copy-Paste Method

If you downloaded the fix files, run these commands in Terminal:

```bash
# Navigate to your site folder
cd ~/btubbsassociates

# Create _includes directory if it doesn't exist
mkdir -p _includes

# Copy the footer.html
cp ~/Downloads/_includes/footer.html _includes/

# Copy the head.html  
cp ~/Downloads/_includes/head.html _includes/

# Rename or replace the CSS file
mv assets/css/main.scss assets/css/main.scss.backup
cp ~/Downloads/btubbs-css-fix/css/style.scss assets/css/

# Restart Jekyll
bundle exec jekyll serve
```

## What Changed

### Footer (footer.html)
- Properly formats contact information
- Shows location, email, phone, LinkedIn link
- Uses proper HTML structure
- Your brand colors applied

### Head (head.html)
- Ensures CSS loads correctly
- Points to the correct stylesheet path

### CSS (style.scss)
- Renamed from main.scss to style.scss (required by Minima theme)
- All your brand colors are now active
- Hero section has colored overlay
- Service cards have colored borders
- Links use your blue-gray colors
- Footer uses your dark brand color

## After Applying Fixes

You should now see:

✅ **Footer properly formatted** with:
- Your company name
- Contact info in a clean list
- Links styled in your brand colors

✅ **Colors throughout** the site:
- Dark blue-gray headers
- Medium blue-gray links
- Colored borders on cards
- Branded footer with dark background
- Hero section with colored overlay

## Verify It Worked

Visit http://localhost:4000 and check:

1. Scroll to footer - should show clean contact info, not raw YAML
2. Look at service cards - should have blue-gray borders
3. Hover over links - should change to lighter blue-gray
4. Check hero section - should have dark overlay
5. Footer background should be dark blue-gray

## If Colors Still Don't Show

Try this:

```bash
# Clear Jekyll cache
rm -rf _site .jekyll-cache

# Restart
bundle exec jekyll serve
```

Sometimes Jekyll caches the old CSS and needs a fresh start.

## File Locations Summary

Make sure you have these files:

```
btubbsassociates/
├── _includes/
│   ├── footer.html      ← NEW: Custom footer
│   └── head.html        ← NEW: Custom head
├── assets/
│   └── css/
│       └── style.scss   ← RENAMED: Was main.scss
```

The `_includes` folder overrides Minima's default templates, so your custom footer and CSS will be used instead.
