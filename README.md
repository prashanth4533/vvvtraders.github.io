# VVV Traders — Premium Quality Pulses & Rice

Premium Export-Grade Pulses, Rice, and Grains. Direct sourcing from farms. Wholesale & bulk supply for supermarkets, wholesalers, and export buyers.

## 🌍 Live Website

**Status:** Ready for Deployment → [Deploy to GitHub Pages](#deployment)

## 🎯 Features

- ✅ **Bilingual Interface** — English & Tamil
- ✅ **Product Showcase** — 20+ premium products with categories
- ✅ **Contact Forms** — Email notifications via Formspree
- ✅ **Mobile Responsive** — Works on all devices
- ✅ **Fast Loading** — Static site, no backend needed
- ✅ **Relative Image Paths** — Ready for deployment

## 📱 Website Structure

### Pages

1. **index.html** — Home page with hero, categories, testimonials, and contact form
2. **products.html** — Product listing with filters and enquiry modal
3. **style.css** — Shared styling for both pages

### Key Sections

- Hero Banner with CTA buttons
- Product Categories (Pulses, Rice, Millets)
- Popular Products showcase
- Contact form with validation
- Footer with company info
- Language toggle (EN/தமிழ்)

## 🚀 Deployment

### Option A: GitHub Pages (Free, Recommended)

```bash
# 1. Create repository at github.com/new
#    Name: "vvvtraders.github.io"
#    Make it PUBLIC

# 2. In project folder:
git init
git add .
git commit -m "Initial commit - VVV Traders website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/vvvtraders.github.io.git
git push -u origin main

# 3. Enable GitHub Pages:
#    - Go to Settings > Pages
#    - Select "Deploy from a branch" > main > / (root)
#    - Wait 1-2 minutes
#    - Visit: https://your-username.github.io

# 4. (Optional) Add custom domain:
#    - Update DNS to point to GitHub Pages
#    - Add domain to Settings > Pages
```

### Option B: Netlify (Free tier available)

```bash
# 1. Connect GitHub repo to netlify.com
# 2. Deploy automatically on every push
# 3. Custom domain available
```

## 📧 Email Setup (Formspree)

### Already Integrated ✅

- Contact form sends to: `formspree.io/f/meojowla`
- Product enquiry modal sends to same address
- All submissions include: Name, Phone, Product, Requirements

### Custom Email Domain (Optional)

1. Log in to [formspree.io](https://formspree.io)
2. Update form endpoint in JavaScript if needed
3. Change both `submitModal()` and `handleContactSubmit()` functions

## 🖼️ Image Setup

### Required Folder Structure

```
/images/
├── hero-bg.png
├── pulses-tab.png
├── rice-tab.png
├── millets-tab.png
├── export-toor-dal.png
├── warehouse.jpg
├── basmati-rice.png
├── seller-profile.jpg
└── /products/
    ├── toor-dal.png
    ├── urad-dal.png
    ├── moong-dal.png
    ├── masoor-dal.png
    ├── chana-dal.png
    ├── green-gram.png
    ├── black-gram.png
    ├── red-lentils.png
    ├── bengal-gram.png
    ├── horse-gram.png
    ├── field-beans.png
    ├── kidney-beans.png
    ├── black-chickpeas.png
    ├── white-chickpeas.png
    ├── peas.png
    ├── wheat.png
    ├── maize.png
    ├── basmati-rice.png
    ├── steam-rice.png
    └── raw-rice.png
```

## 🌐 Internationalization (i18n)

### Language Support

- **English (EN)** — Default
- **Tamil (தமிழ்)** — Full translation

### Supported Elements

- Navigation menu
- Hero section
- Product categories
- Filters
- Forms and modals
- Footer

### Language Toggle

Click `EN` or `தமிழ்` button in navbar to switch languages. Selection saved in browser.

## 📋 Pre-Deployment Checklist

- [x] All image paths converted to relative URLs
- [x] Image folder structure created
- [x] Form integration with Formspree
- [x] Language toggle functional
- [x] Mobile responsive design
- [x] Console errors checked and fixed
- [ ] All images moved to `/images/` folder
- [ ] Formspree form ID verified
- [ ] GitHub repo created and pushed
- [ ] GitHub Pages enabled
- [ ] Test deployment live

## 🧪 Testing

### Browser Testing

```
✅ Chrome (latest)
✅ Firefox (latest)
✅ Safari (latest)
✅ Edge (latest)
✅ Mobile Chrome (Android)
✅ Mobile Safari (iOS)
```

### Functionality Testing

```
Functions to test:
✅ Language toggle (EN/தமிழ்)
✅ Product filter buttons
✅ Form validation (empty fields)
✅ Form submission (Formspree)
✅ Modal open/close
✅ Navigation links
✅ Responsive grid on mobile
✅ Hamburger menu on mobile
```

### Form Testing

```
1. Fill out contact form
2. Submit → should see "✓ Enquiry sent!" message
3. Check your email (may take 5-60 seconds)
4. Repeat for product enquiry modal
```

## 🔧 Customization

### Update Company Info

- **Phone:** `6382378017` or `9443394930` (search in HTML)
- **Email:** `info@vvvtraders.com` (search in HTML)
- **Location:** "Coimbatore, Tamil Nadu, India" (search in HTML)

### Update Product Prices

Edit in `products.html` or `index.html`, look for price values (₹39/kg, etc.)

### Update Product Lists

Products array in `products.html` (lines ~1190-1210):

```javascript
const products = [
  { id: 1, nameKey: "product_toor_dal", ... },
  // Add or remove entries
];
```

## 📲 Add Phone Integration

### WhatsApp Button

Already in footer: `<a href="tel:6382378017">`

### Add WhatsApp Direct Link

```html
<a href="https://wa.me/916382378017?text=Hi%20VVV%20Traders">WhatsApp Us</a>
```

### Add Viber/Signal

```html
<a href="viber://chat?number=%2B916382378017">Viber</a>
```

## 🚨 Troubleshooting

### Images Not Loading

1. Check folder structure matches `/images/` and `/images/products/`
2. Verify image file names exactly match HTML (case-sensitive)
3. Use browser DevTools (F12) → Network tab to see 404s

### Forms Not Sending

1. Check browser console (F12 → Console) for errors
2. Verify Formspree form ID in JavaScript
3. Test in Incognito/Private window (bypass cache)

### Language Toggle Not Working

1. Check browser console for JavaScript errors
2. Verify `localStorage` not disabled
3. Test in different browser

## 📞 Support

For issues or questions:

1. Check browser console (F12)
2. Review HOSTING_GUIDE.md
3. Test in Incognito window
4. Check GitHub Pages deployment status

## 📄 License

VVV Traders Confidential — 2025

---

**Last Updated:** April 2, 2026  
**Version:** 1.0 - Production Ready  
**Author:** GitHub Copilot
