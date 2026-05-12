# DeRIVE Innovation Website - Setup Instructions

## New Pages Added

### 1. **Products Page** (`/products`)
- Displays 4 product categories with descriptions:
  - VaRP TMS and Route Optimization
  - Mobile POD
  - Fleet Monitoring/Order Tracking
  - WMS
- Fully responsive grid layout
- Integrated navigation menu

### 2. **Site References Page** (`/site-references`)
- Displays customer logos (7-8 slots available)
- Clean grid layout with hover effects
- Fully responsive design

### 3. **Updated Home Page** (`/`)
- Added navigation menu with links to all pages
- Maintains all existing functionality
- Updated header styling with navigation

## Adding Customer Logos

To add customer logos to the Site References page:

1. Create a `logos` folder in your `public` directory:
   ```
   public/
   └── logos/
       ├── customer1.png
       ├── customer2.png
       ├── customer3.png
       ├── customer4.png
       ├── customer5.png
       ├── customer6.png
       ├── customer7.png
       └── customer8.png
   ```

2. Edit `/src/pages/site-references.astro` and update the `customers` array:
   ```javascript
   const customers = [
     {
       name: "Your Company Name",
       logo: "/logos/your-logo.png"
     },
     // ... more customers
   ];
   ```

## Logo Recommendations

- **Format**: PNG or SVG (supports transparency)
- **Size**: Recommended 400x300px or similar aspect ratio
- **Quality**: High resolution for best appearance
- **Style**: Company logos work best with consistent sizing

## Navigation Structure

All pages now include a unified navigation menu:
- Home
- Products
- Site References
- Contact

## Development

The website uses **Astro** as the static site generator. All pages are built with:
- Responsive design
- Clean, professional styling
- Consistent layout and navigation
- Mobile-friendly interface

To run locally:
```bash
npm install
npm run dev
```

To build for production:
```bash
npm run build
npm run preview
```
