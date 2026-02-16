# Image Assets Structure

This directory contains all image assets for the Adeng-Adeng website.

## Directory Structure

```
images/
├── hero/              # Hero section images (1920x1080px minimum)
├── turtles/           # Turtle and marine life images (800x600px)
├── snorkeling/        # Snorkeling activity images (800x600px)
├── horse-tours/       # Cidomo and horse images (800x600px)
├── beach-bar/         # Beach bar and restaurant images (800x600px)
├── bungalows/         # Accommodation images (800x600px)
├── diving/            # Underwater/diving images (800x600px)
├── culture/           # Local culture images (800x600px)
├── food/              # Food and cuisine images (800x600px)
└── logo/              # Logo files (SVG preferred, PNG fallback)
```

## Image Requirements

### Dimensions
- **Hero images:** 1920x1080px minimum (16:9 ratio)
- **Card images:** 800x600px (4:3 ratio)
- **Gallery images:** 800x800px (1:1 ratio)
- **Logo:** SVG preferred, PNG fallback (multiple sizes)

### Format
- **Primary:** WebP format for optimal performance
- **Fallback:** JPG format for compatibility
- Use `<picture>` element with both formats

### Naming Convention
- `turtles-*.jpg` / `turtles-*.webp` → Turtle images
- `snorkeling-*.jpg` / `snorkeling-*.webp` → Snorkeling images
- `horse-tours-*.jpg` / `horse-tours-*.webp` → Cidomo images
- `beach-bar-*.jpg` / `beach-bar-*.webp` → Beach bar images
- `bungalows-*.jpg` / `bungalows-*.webp` → Bungalow images
- `diving-*.jpg` / `diving-*.webp` → Diving images
- `food-*.jpg` / `food-*.webp` → Food images
- `culture-*.jpg` / `culture-*.webp` → Culture images
- `adeng-adeng-logo.svg` / `adeng-adeng-logo.png` → Logo files

### Optimization
- All images should be optimized for web
- Use compression tools (e.g., ImageOptim, TinyPNG)
- Maintain quality while reducing file size
- Lazy loading enabled via `loading="lazy"` attribute

### Image Filter
All images (except logos) have a consistent filter applied via CSS:
- `brightness(1.02) contrast(1.05) saturate(1.1)`
- Hover: `brightness(1.08) contrast(1.05) saturate(1.15)`

## Required Images

### Hero Section
- `hero-main.jpg` / `hero-main.webp` (1920x1080px)

### Logo
- `adeng-adeng-logo.svg` (preferred)
- `adeng-adeng-logo.png` (fallback)
- `favicon-32x32.png`
- `favicon-16x16.png`
- `apple-touch-icon.png`

### Sections
Each section should have at least 2-3 images:
- Turtles: 3+ images
- Snorkeling: 3+ images
- Beach bar: 4+ images
- Bungalows: 2+ images
- Diving: 2+ images
- Culture: 3+ images
- Food: 2+ images
- Horse tours: 2+ images

### Gallery
- Mix of images from all categories
- Minimum 8 images for gallery grid

## Usage in HTML

```html
<picture>
    <source srcset="images/turtles/turtles-1.webp" type="image/webp">
    <img src="images/turtles/turtles-1.jpg" alt="Description" loading="lazy" decoding="async">
</picture>
```

## Notes
- All images should have descriptive alt text
- Use WebP format for better performance
- Always provide JPG fallback
- Enable lazy loading for images below the fold
- Optimize images before uploading
