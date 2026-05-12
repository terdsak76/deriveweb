# Customer Logo Setup Guide

## Quick Setup

### Step 1: Create the Logos Directory
```bash
mkdir -p public/logos
```

### Step 2: Add Your Logo Files
Place your customer logo files in `public/logos/` with these names:
- `customer1.png`
- `customer2.png`
- `customer3.png`
- `customer4.png`
- `customer5.png`
- `customer6.png`
- `customer7.png`
- `customer8.png`

### Step 3: Update Company Names (Optional)
Edit `src/pages/site-references.astro` and update the customer names:

```javascript
const customers = [
  {
    name: "ABC Logistics",
    logo: "/logos/customer1.png"
  },
  {
    name: "XYZ Distribution",
    logo: "/logos/customer2.png"
  },
  // ... and so on
];
```

## Logo File Recommendations

| Aspect | Recommendation |
|--------|-----------------|
| **Format** | PNG (recommended) or SVG |
| **Background** | Transparent (PNG) or white |
| **Dimensions** | 400×300px or similar ratio |
| **File Size** | Under 500KB per file |
| **Quality** | High resolution (300 DPI) |

## Example Files Structure
```
public/
├── hero.jpg                  (existing)
└── logos/                    (create this folder)
    ├── customer1.png         (your 1st customer logo)
    ├── customer2.png         (your 2nd customer logo)
    ├── customer3.png         (your 3rd customer logo)
    ├── customer4.png         (your 4th customer logo)
    ├── customer5.png         (your 5th customer logo)
    ├── customer6.png         (your 6th customer logo)
    ├── customer7.png         (your 7th customer logo)
    └── customer8.png         (your 8th customer logo)
```

## Logo Card Styling

The logo cards automatically:
- Scale the logo to fit the card (max 150px height)
- Maintain aspect ratio
- Center the logo both horizontally and vertically
- Show hover effects (shadow and lift animation)
- Display on a clean white background

## Browser Compatibility

The site works on:
- Chrome/Edge (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Troubleshooting

**Logo not showing?**
1. Check file path matches: `/logos/customer#.png`
2. Verify file exists in `public/logos/` directory
3. Check file extension matches (case-sensitive on Linux/Mac)
4. Ensure logo file is a valid image format

**Logo looks stretched?**
1. Ensure logo has transparent background or is a square
2. SVG files work better for logos with transparency
3. Consider using PNG files with transparent backgrounds

**Need to add more logos?**
- Duplicate a customer object in the `customers` array
- Add the new image file to `public/logos/`
- The grid will automatically adjust to fit the new items

## Adding Logos from URLs

If you prefer to serve logos from external URLs, you can modify the customers array:

```javascript
const customers = [
  {
    name: "Customer Name",
    logo: "https://example.com/path/to/logo.png"
  },
];
```

However, local files are recommended for better performance and reliability.
