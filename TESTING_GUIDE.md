# Testing Guide - New Pages

## Local Testing

### 1. Start Development Server
```bash
npm run dev
```

The site will be available at `http://localhost:3000` (or the port shown in terminal)

### 2. Test All Pages

#### Home Page (`/`)
- ✅ Navigation menu visible with all links
- ✅ "Home" link shows as active (blue and bold)
- ✅ Contact section displays correctly
- ✅ Company information visible
- ✅ Hero section displays

#### Products Page (`/products`)
- ✅ Navigate to Products link in menu
- ✅ All 4 product cards visible
- ✅ Product titles: VaRP TMS, Mobile POD, Fleet Monitoring, WMS
- ✅ Descriptions under each title
- ✅ "Products" link shows as active
- ✅ Hover effect on cards (shadow + lift)

#### Site References Page (`/site-references`)
- ✅ Navigate to Site References link
- ✅ 8 logo placeholder cards visible
- ✅ Cards arranged in responsive grid
- ✅ "Site References" link shows as active
- ✅ Hover effects work
- ✅ After adding logos, they display correctly

### 3. Navigation Testing

**Menu Links:**
- [ ] Home - returns to home page
- [ ] Products - opens products page
- [ ] Site References - opens site references page
- [ ] Contact - scrolls to contact section on home
- [ ] Active state highlights current page

### 4. Responsive Design Testing

**Desktop (1200px+)**
- [ ] Navigation appears horizontally
- [ ] Products grid shows multiple columns
- [ ] Logo grid displays properly

**Tablet (768px - 1199px)**
- [ ] Navigation remains visible
- [ ] Products grid adjusts to 2 columns
- [ ] Logo grid responsive

**Mobile (< 768px)**
- [ ] Navigation stacks vertically
- [ ] Products single column
- [ ] Logo cards single column
- [ ] All text readable
- [ ] No horizontal scroll

### 5. Functionality Checks

**Links:**
- [ ] Contact phone number is clickable (tel: protocol)
- [ ] Contact email is clickable (mailto: protocol)
- [ ] Facebook link opens in new tab
- [ ] All navigation links work

**Content:**
- [ ] Product titles display correctly
- [ ] Product descriptions are readable
- [ ] Company name consistent across pages
- [ ] Footer year updates automatically

### 6. Browser Testing

Test on:
- [ ] Chrome/Edge
- [ ] Firefox
- [ ] Safari
- [ ] Mobile Safari (iOS)
- [ ] Chrome Mobile (Android)

### 7. Quick Visual Checklist

**Colors & Styling:**
- [ ] Primary color (blue) used consistently
- [ ] Text contrast is good
- [ ] Borders are visible but subtle
- [ ] Hover states are clear

**Spacing:**
- [ ] No content crowding
- [ ] Margins consistent
- [ ] Padding looks balanced
- [ ] Mobile spacing appropriate

**Typography:**
- [ ] Headings are prominent
- [ ] Body text readable
- [ ] Font consistent throughout
- [ ] No text overflow issues

## Before Production

1. **Add Customer Logos**
   - [ ] Create `public/logos/` directory
   - [ ] Add 7-8 customer logo files
   - [ ] Verify all logos display correctly

2. **Update Product Descriptions** (Optional)
   - [ ] Customize product descriptions
   - [ ] Add any additional details
   - [ ] Verify accuracy

3. **Test Build Process**
   ```bash
   npm run build
   npm run preview
   ```
   - [ ] Build completes without errors
   - [ ] Preview shows all pages correctly

4. **Final Review**
   - [ ] All links work
   - [ ] All content visible
   - [ ] No console errors
   - [ ] Responsive on all devices

## Performance Testing

After building for production:

```bash
npm run build
npm run preview
```

Check:
- [ ] Page loads quickly
- [ ] No console errors
- [ ] All images load
- [ ] Responsive design works

## Common Issues & Solutions

| Issue | Solution |
|-------|----------|
| Navigation links don't work | Check file paths in hrefs |
| Logos not showing | Verify file exists in `public/logos/` |
| Styling looks broken | Clear browser cache (Ctrl+Shift+Delete) |
| Mobile layout off | Check viewport meta tag in head |
| Active link not highlighting | Verify `class="active"` on correct link |

## Success Criteria

✅ All pages load without errors
✅ Navigation works on all pages
✅ Responsive design works on mobile/tablet/desktop
✅ All links functional
✅ Product cards display correctly
✅ Logo placeholders ready for customer logos
✅ Consistent styling across all pages
✅ Footer displays correctly on all pages
✅ No broken images or missing content
✅ Build process completes successfully
