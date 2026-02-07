# Image Placement Instructions

After extracting this Jekyll site, you need to add your images from Wix.

## Step-by-Step:

1. **Create a folder to organize your Wix images:**
   - Create a folder called `wix-images` on your desktop
   - Copy all downloaded images there
   - Rename them according to the list below

2. **Copy images to the Jekyll site:**
   
   Copy each renamed image to its destination:

### Hero Section
- Source: `44a8b5374d1c4364a684efdb64db7728.jpg` (Touchscreen computer)
- Rename to: `hero-background.jpg`
- Destination: `assets/images/hero-background.jpg`

### Professional Photo
- Source: `tubbs_cropped.jpg` or `304379_b1c26c33d7804604827531b2c7d99962~mv2.jpg`
- Rename to: `bill-tubbs-photo.jpg`
- Destination: `assets/images/bill-tubbs-photo.jpg`

### Services Images (go in `assets/images/services/`)

1. **Data Analytics:**
   - Source: `9441146dbd3b4a31a35f513916b26942.jpg` (Analyzing data)
   - Rename to: `data-analytics.jpg`
   - Destination: `assets/images/services/data-analytics.jpg`

2. **Process Control:**
   - Source: `95d9be60e88844eaa92ed30f871d5bae.jpg` (Business meeting)
   - Rename to: `process-control.jpg`
   - Destination: `assets/images/services/process-control.jpg`

3. **Energy Management:**
   - Source: `304379_3b764f62be2148db9b29483bb3614dbc~mv2.jpg` or `iStock-1138642441.jpg`
   - Rename to: `energy-management.jpg`
   - Destination: `assets/images/services/energy-management.jpg`

4. **Production Optimization:**
   - Source: `11062b_20c42921c1444677960ec127624a88d3~mv2.jpeg` (Control room)
   - OR use a replacement image (this was the non-downloadable one)
   - Rename to: `production-optimization.jpg`
   - Destination: `assets/images/services/production-optimization.jpg`
   - **Alternative:** Search Unsplash for "industrial control room" if needed

5. **Management Control:**
   - Source: `da9d83ef63014589acac69d0c0f44f45.jpg` (Graphs)
   - Rename to: `management-control.jpg`
   - Destination: `assets/images/services/management-control.jpg`

### Testimonials Icons (go in `assets/images/testimonials/`)

1. **Oil & Gas Icon:**
   - Source: `304379_794073d63624471bb5b752f0b10b07d5~mv2.gif`
   - Rename to: `icon-oil-gas.gif`
   - Destination: `assets/images/testimonials/icon-oil-gas.gif`

2. **Mine Icon:**
   - Source: `304379_46aeed33b8a14a7db6e72b4f43c9cea5~mv2.gif`
   - Rename to: `icon-mine.gif`
   - Destination: `assets/images/testimonials/icon-mine.gif`

### Social Icons (go in `assets/images/icons/`)

1. **LinkedIn:**
   - Source: `7528824071724d12a3e6c31eee0b40d4.png`
   - Rename to: `linkedin.png`
   - Destination: `assets/images/icons/linkedin.png`

## Quick Commands (macOS/Linux):

If you want to automate the copying, open Terminal in your wix-images folder and run:

```bash
# From your wix-images folder, assuming Jekyll site is at ~/btubbs-jekyll-site

cp hero-background.jpg ~/btubbs-jekyll-site/assets/images/
cp bill-tubbs-photo.jpg ~/btubbs-jekyll-site/assets/images/
cp data-analytics.jpg ~/btubbs-jekyll-site/assets/images/services/
cp process-control.jpg ~/btubbs-jekyll-site/assets/images/services/
cp energy-management.jpg ~/btubbs-jekyll-site/assets/images/services/
cp production-optimization.jpg ~/btubbs-jekyll-site/assets/images/services/
cp management-control.jpg ~/btubbs-jekyll-site/assets/images/services/
cp icon-oil-gas.gif ~/btubbs-jekyll-site/assets/images/testimonials/
cp icon-mine.gif ~/btubbs-jekyll-site/assets/images/testimonials/
cp linkedin.png ~/btubbs-jekyll-site/assets/images/icons/
```

## Verification:

After copying, verify you have these files:

```
assets/images/
├── hero-background.jpg
├── bill-tubbs-photo.jpg
├── services/
│   ├── data-analytics.jpg
│   ├── process-control.jpg
│   ├── energy-management.jpg
│   ├── production-optimization.jpg
│   └── management-control.jpg
├── testimonials/
│   ├── icon-oil-gas.gif
│   └── icon-mine.gif
└── icons/
    └── linkedin.png
```

## Image Optimization (Optional but Recommended):

Before deployment, optimize images for web:

1. **Using ImageOptim (macOS):**
   - Download from: https://imageoptim.com/
   - Drag all images into ImageOptim
   - It will compress without quality loss

2. **Using TinyPNG (Web-based):**
   - Go to: https://tinypng.com/
   - Upload images (max 20 at a time)
   - Download compressed versions

Target sizes:
- Hero image: < 500KB
- Service images: < 200KB each
- Icons: < 50KB each

## Missing Image?

If you couldn't download the control room image (`Pump in power plant.jpg`):

**Option 1 - Use a free alternative:**
- Visit: https://unsplash.com/s/photos/industrial-control-room
- Download a high-quality image
- Rename to: `production-optimization.jpg`

**Option 2 - Use another of your images:**
- Pick another relevant industrial/operations image
- Use it as a replacement

**Option 3 - Skip it temporarily:**
- The site will work without it (image will show as broken)
- Add it later when you find a suitable replacement
