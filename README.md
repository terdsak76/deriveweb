# Company Landing Page - Astro Framework

A beautiful, responsive landing page built with Astro framework.

## Features

- ✅ Company name and logo
- ✅ Company address
- ✅ Phone number (clickable to call)
- ✅ Facebook page link
- ✅ Contact person email
- ✅ Responsive design
- ✅ Modern gradient background
- ✅ Smooth animations

## Setup Instructions

### 1. Install Dependencies

```bash
cd my-company-site
npm install
```

### 2. Run Development Server

```bash
npm run dev
```

The site will be available at `http://localhost:4321`

### 3. Build for Production

```bash
npm run build
```

The built site will be in the `dist/` folder.

### 4. Preview Production Build

```bash
npm run preview
```

## Customization

### Update Company Information

Edit the `companyInfo` object in `src/pages/index.astro`:

```javascript
const companyInfo = {
  name: "Your Company Name",
  address: "123 Business Street, City, State 12345, Country",
  phone: "+1 (555) 123-4567",
  facebookPage: "https://facebook.com/yourcompany",
  contactEmail: "contact@yourcompany.com",
  contactPerson: "John Doe"
};
```

### Replace the Logo

Replace `public/logo.svg` with your own logo file. Supported formats:
- SVG (recommended)
- PNG
- JPG

If using PNG/JPG, update the logo reference in `index.astro`:

```html
<img src="/logo.png" alt="Company Logo" class="logo">
```

### Change Colors

The site uses a purple gradient background. To change colors, edit the CSS in `src/pages/index.astro`:

```css
/* Background gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Header gradient */
background: linear-gradient(135deg, #2563eb 0%, #1d4ed8 100%);
```

## File Structure

```
my-company-site/
├── public/
│   └── logo.svg           # Company logo
├── src/
│   └── pages/
│       └── index.astro    # Main landing page
├── astro.config.mjs       # Astro configuration
├── package.json           # Dependencies
└── tsconfig.json          # TypeScript config
```

## Deployment

### Deploy to Netlify

1. Push your code to GitHub
2. Connect your repository to Netlify
3. Build command: `npm run build`
4. Publish directory: `dist`

### Deploy to Vercel

1. Push your code to GitHub
2. Import your repository in Vercel
3. Vercel will automatically detect Astro

### Deploy to GitHub Pages

```bash
npm run build
# Upload the dist/ folder to your web server
```

## Technologies Used

- **Astro** - Modern static site framework
- **HTML5** - Semantic markup
- **CSS3** - Modern styling with gradients and animations
- **JavaScript** - Minimal client-side interactivity

## Browser Support

- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers

## License

MIT License - Feel free to use this for your company!
