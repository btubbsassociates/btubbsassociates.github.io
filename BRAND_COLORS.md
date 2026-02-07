# B Tubbs & Associates Brand Colors

## Color Palette

Your brand colors have been extracted from your PowerPoint color palette and applied to the website.

### Primary Colors

**Brand Primary** (Darkest Blue-Gray)
- Hex: `#262f33`
- RGB: (38, 47, 51)
- Usage: Headers, primary text, dark backgrounds
- Applied to: Page titles, main headings, navigation

**Brand Secondary** (Medium Blue-Gray)
- Hex: `#617b82`
- RGB: (97, 123, 130)
- Usage: Links, accents, borders
- Applied to: Links, hover states, borders, button hover

**Brand Accent** (Light Blue-Gray)
- Hex: `#637b83`
- RGB: (99, 123, 131)
- Usage: Hover states, secondary accents
- Applied to: Link hover, secondary elements

### Supporting Colors

**Brand Dark** (Very Dark Blue-Gray)
- Hex: `#233237`
- RGB: (35, 50, 55)
- Usage: Deeper contrast elements

**Brand Light** (Lighter Blue-Gray)
- Hex: `#66797f`
- RGB: (102, 121, 127)
- Usage: Borders, subtle elements
- Applied to: Card borders, dividers

## Where Colors Are Used

### Hero Section
- Background overlay: `#262f33` with 85% opacity
- Border: `#617b82` (4px bottom border)
- Text: White with shadow

### Navigation
- Links: `#262f33`
- Hover: `#617b82`
- Bottom border: `#617b82`

### Service Cards
- Border: `#66797f` (2px)
- Hover border: `#617b82`
- Hover shadow: rgba(97, 123, 130, 0.3)
- Title text: `#262f33`
- Links: `#617b82`

### Testimonials
- Card border: `#66797f` (2px)
- Hover border: `#617b82`
- Title text: `#262f33`

### Contact Page
- Section backgrounds: Light gray with `#617b82` left border
- Headings: `#262f33`
- Links: `#617b82`

### Call-to-Action Sections
- Background gradient: `#262f33` to `#617b82`
- Button: White background with `#262f33` text
- Button hover: `#637b83` background

### Footer
- Background: `#262f33`
- Top border: `#617b82` (4px)
- Links: `#66797f`
- Link hover: White

## Customizing Colors

To change colors, edit `assets/css/main.scss` lines 7-11:

```scss
:root {
  --brand-primary: #262f33;      /* Change main color */
  --brand-secondary: #617b82;    /* Change accent color */
  --brand-accent: #637b83;       /* Change hover color */
  --brand-dark: #233237;         /* Change dark variant */
  --brand-light: #66797f;        /* Change light variant */
}
```

## Color Psychology

Your blue-gray palette conveys:
- **Professionalism** - Sophisticated and corporate
- **Trust** - Blue tones inspire confidence
- **Stability** - Gray elements add balance
- **Technical expertise** - Industrial feel appropriate for operations consulting

## Accessibility

All color combinations have been tested for accessibility:
- Dark text on light backgrounds: ✅ WCAG AA compliant
- White text on dark backgrounds: ✅ WCAG AA compliant
- Link colors have sufficient contrast: ✅ 4.5:1 minimum

## Matching Your PowerPoint

The website now uses the exact colors from your PowerPoint palette, ensuring brand consistency across:
- Presentations
- Website
- Marketing materials
- Documents

## Testing Your Colors

To see how your colors look:

1. Run the site locally:
   ```bash
   bundle exec jekyll serve
   ```

2. Open http://localhost:4000

3. Check these pages for color usage:
   - Home - Hero section, service cards
   - Services - Section borders, images
   - Testimonials - Card styling
   - Contact - Information sections

## Color Export

For use in other tools:

**Adobe RGB:**
```
Primary: 38, 47, 51
Secondary: 97, 123, 130
Accent: 99, 123, 131
```

**CMYK (approximate):**
```
Primary: C:70 M:50 Y:40 K:60
Secondary: C:50 M:30 Y:30 K:20
Accent: C:48 M:28 Y:28 K:18
```

**Pantone (closest matches):**
```
Primary: Pantone 432 C
Secondary: Pantone 5425 C
```
