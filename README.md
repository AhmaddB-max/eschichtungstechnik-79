# Friends of Friends Website
## Premium Multi-Page Website for Coffee Shop, Vinyl Bar & Restaurant

Created: 2024
Location: National City, South Bay San Diego

---

## 📁 Folder Structure

```
friendsoffriends-website/
├── index.html              # Homepage
├── about.html              # About Us page
├── menu.html               # Menu with tabbed sections
├── events.html             # Events calendar & info
├── shop.html               # Merch shop with product grid
├── visit.html              # Location, map, hours
├── contact.html            # Contact form
├── 404.html                # Custom 404 error page
└── README.md               # This file
```

---

## 🎨 Design Features

### Color Palette
- **Terracotta**: #D4745E (Primary accent)
- **Warm Olive**: #8B9556 (Secondary)
- **Deep Espresso Brown**: #3D2817 (Dark accent)
- **Soft Cream**: #F5F1E8 (Light background)
- **Sage Green**: #A8B5A0 (Tertiary)
- **Rich Black**: #1A1A1A (Dark background)

### Typography
- **Headings**: DM Serif Display (distinctive, warm serif)
- **Body**: Manrope (clean, modern sans-serif)

### Key Features
- ✅ Fully responsive (mobile-first design)
- ✅ Dark/light mode toggle (defaults to warm dark mode)
- ✅ Smooth scroll animations & reveal effects
- ✅ Parallax hero sections
- ✅ Sticky navigation with scroll effects
- ✅ Mobile hamburger menu with smooth transitions
- ✅ Grain texture overlay for warmth
- ✅ Accessible (WCAG 2.2 AA compliant structure)
- ✅ SEO-optimized with meta tags
- ✅ Open Graph tags for social sharing

---

## 📄 Page Breakdown

### 1. Homepage (`index.html`)
**Sections:**
- Full-screen parallax hero with CTAs
- Quick links to Menu / Events / Shop
- Our Story teaser
- Featured drinks & food showcase
- Upcoming events carousel
- Community / "Southbay All Day" message
- Instagram feed integration
- Location map preview & hours
- Newsletter signup

### 2. About Us (`about.html`)
**Sections:**
- Mission & values
- Founder profiles (Marco Laguna, Brandon James-Keeper, Aaron Henderson)
- South Bay roots story
- Community commitment
- Photo placeholders for interior/team shots

### 3. Menu (`menu.html`)
**Tabbed Sections:**
- Coffee & Drinks (Signature + Classic)
- Food (Smash burgers, Filipino-inspired dishes, sides)
- Beer & Wine
- Pastries & Sweets

**Interactive:** Click tabs to switch between menu categories

### 4. Events (`events.html`)
**Sections:**
- Featured recurring events:
  - "For the Record" (monthly vinyl exchange)
  - Film & Chill Nights (weekly)
  - DJ Sets & Art Showcases
- Interactive calendar with event markers
- RSVP/contact CTAs

### 5. Shop (`shop.html`)
**Features:**
- Product grid with filter buttons (All, Apparel, Vinyl, Coffee, Accessories)
- 8 sample products with dummy "Add to Cart" functionality
- Hover effects on product cards
- Ready for e-commerce integration

### 6. Visit Us (`visit.html`)
**Sections:**
- Embedded Google Map (placeholder iframe)
- Full hours breakdown
- Parking & transit info
- What to expect when visiting
- Directions CTA

### 7. Contact (`contact.html`)
**Features:**
- Contact form with validation
- Subject dropdown (General, Events, Catering, Partnership, etc.)
- Direct contact info (phone, address, hours)
- FAQ section
- Social media links

### 8. 404 Error Page (`404.html`)
**Features:**
- Friendly error message
- Animated coffee cup icon
- Quick navigation back to main pages
- Maintains brand aesthetic

---

## 🚀 Setup Instructions

### Option 1: Local Development (Recommended)
1. **Extract all files** to a folder on your computer
2. **Open `index.html`** in any modern web browser
3. Navigate between pages using the menu

### Option 2: Local Server (For Testing)
```bash
# If you have Python installed:
python -m http.server 8000

# Or with Node.js:
npx serve

# Then visit: http://localhost:8000
```

### Option 3: Deploy to Web Host
1. Upload all HTML files to your web hosting root directory
2. Configure your server to serve `index.html` as the default page
3. Set up custom 404 error page in server config:
   - Apache: Use `.htaccess` → `ErrorDocument 404 /404.html`
   - Nginx: Add to config → `error_page 404 /404.html;`

---

## 🔧 Customization Guide

### Replace Placeholder Images
All image placeholders are clearly marked with descriptions of what should be there:

**Example:**
```html
<!-- PHOTO: Buko Pandan Latte - vibrant green Filipino-inspired latte in ceramic cup with latte art -->
```

**Recommended Image Sizes:**
- Hero backgrounds: 1920x1080px
- Product photos: 800x800px
- Event photos: 1600x900px
- Founder portraits: 800x1200px
- Instagram grid: 600x600px

### Update Contact Information
Search for and replace these placeholders:
- **Phone**: (619) 796-6210
- **Address**: 127 E 8th St, National City, CA 91950
- **Instagram**: @friendsoffriends.sd
- **Email**: Add your email address in contact.html form handler

### Connect Online Ordering
Replace all instances of `href="#"` on "Order Online" buttons with your Toast ordering link.

### Integrate Instagram Feed
Replace the placeholder Instagram grid in `index.html` with:
1. Instagram API integration
2. Instagram feed widget (e.g., Juicer, SnapWidget)
3. Manual updates with real images

### Google Maps Integration
In `visit.html`, replace the iframe src with your actual Google Maps embed code:
1. Go to Google Maps
2. Search for "127 E 8th St, National City, CA 91950"
3. Click Share → Embed a map
4. Copy the iframe code
5. Replace the placeholder iframe

### Connect Contact Form
The contact form in `contact.html` currently shows an alert. To make it functional:

**Option 1 - Formspree (Easy)**
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

**Option 2 - Custom Backend**
Update the JavaScript to send data to your server endpoint

**Option 3 - Email Service**
Use services like EmailJS, SendGrid, or Mailgun

---

## 🎯 Features Ready for Integration

### Analytics
Add Google Analytics or similar by inserting tracking code in the `<head>` of each page:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
```

### E-commerce
The shop page has placeholder "Add to Cart" functionality. Integrate with:
- Shopify Buy Button
- WooCommerce
- Square Online
- Custom cart system

### Email Newsletter
The newsletter signup form is ready. Connect with:
- Mailchimp
- ConvertKit
- Constant Contact
- Email service of choice

### Event RSVP
Add event registration by connecting the Events page CTAs to:
- Eventbrite
- Google Forms
- Custom RSVP system

---

## 📱 Browser Compatibility

Tested and optimized for:
- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

**Minimum supported:**
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

---

## ♿ Accessibility Features

- Semantic HTML5 structure
- ARIA labels where appropriate
- Keyboard navigation support
- Focus states for interactive elements
- Alt text placeholders for images
- Color contrast ratios meet WCAG AA standards
- Responsive font sizing

---

## 🎨 Advanced Customization

### Change Color Scheme
Edit CSS variables in each HTML file's `<style>` section:
```css
:root {
    --color-terracotta: #D4745E;  /* Your primary color */
    --color-olive: #8B9556;       /* Your secondary color */
    /* etc. */
}
```

### Modify Fonts
Replace Google Fonts links in `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=YourFont&display=swap" rel="stylesheet">
```

Then update CSS:
```css
body { font-family: 'YourFont', sans-serif; }
h1, h2, h3 { font-family: 'YourHeadingFont', serif; }
```

### Add More Pages
1. Duplicate an existing page (e.g., `about.html`)
2. Update content
3. Add navigation links in all page headers
4. Update footer links

---

## 📞 Support & Questions

For questions about this codebase or customization help:
- Review the inline HTML comments
- Check the placeholder image descriptions
- Refer to Tailwind CSS documentation for utility classes

---

## 🎉 What's Next?

1. **Replace all placeholder images** with real photos
2. **Update Google Maps** embed with actual location
3. **Connect contact form** to email service
4. **Add real menu items** and pricing
5. **Integrate online ordering** system (Toast)
6. **Connect Instagram** feed
7. **Set up analytics** tracking
8. **Add newsletter** service
9. **Deploy to your domain**
10. **Test on all devices**

---

## 📝 Notes

- All JavaScript is vanilla (no frameworks required)
- Tailwind CSS loaded via CDN (no build step needed)
- Font Awesome icons via CDN
- Google Fonts loaded via CDN
- Dark mode preference persists in localStorage
- Mobile menu state managed in JavaScript
- Smooth scroll behavior enabled globally

---

## 🚨 Important Reminders

1. **Update all "Order Online" links** with real Toast URL
2. **Replace Instagram handle** throughout if different
3. **Update phone number** if it changes
4. **Test contact form** thoroughly before launch
5. **Optimize images** for web (compress, resize)
6. **Set up SSL certificate** when deploying to production
7. **Configure 404 page** on your server
8. **Add real product info** in shop before accepting orders

---

**Built with care for Friends of Friends**  
*Southbay All Day ☕🎵*

Version 1.0 | December 2024
