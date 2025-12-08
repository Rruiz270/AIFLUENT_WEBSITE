# AIFLUENT Website

A modern, responsive website for AIFLUENT - Infrastructure for High-Performance Education Companies, built following Apple's design standards.

## 🚀 Features

- **Modern Design**: Clean, professional design inspired by Apple's design principles
- **Responsive**: Fully responsive design that works on all devices
- **Fast Loading**: Optimized for performance with minimal dependencies
- **SEO Friendly**: Semantic HTML structure for better search engine visibility
- **Accessibility**: Built with accessibility best practices in mind

## 📁 Project Structure

```
aifluent-website/
├── index.html              # Homepage
├── solutions.html           # Solutions page
├── assets/
│   ├── css/
│   │   └── style.css       # Main stylesheet
│   ├── js/
│   │   └── script.js       # JavaScript functionality
│   └── images/             # Image assets (to be added)
└── README.md               # This file
```

## 🎨 Brand Colors

The website uses AIFLUENT's brand colors as defined in the design:

- **Primary Blue**: #1A3C5A (Deep Learning Blue)
- **Secondary Blue**: #546A76 (Slate Grey) 
- **Accent Gold**: #B89B5E (Knowledge Gold)
- **Cream**: #F4F0E3 (Background cream)
- **White**: #FFFFFF

## 🖼️ Image Requirements

To complete the website, you'll need to add the following images to the `assets/images/` directory:

### Brand Assets
- `aifluent-logo.svg` - Main AIFLUENT logo (vector format preferred)
- `aifluent-logo.png` - PNG version of the logo for fallback

### Homepage Images
- `education-infrastructure.jpg` (1200x800px) - Hero section image showing educational technology/infrastructure
  - *Suggested: Modern classroom with technology, digital learning platforms, or connected educational systems*
- `fragmented-systems.jpg` (1000x600px) - Problem section illustration
  - *Suggested: Split-screen showing fragmented vs. unified systems, or disconnected vs. connected workflow*

### Solution Icons
- `lms-icon.svg` (64x64px) - Learning Management System icon
- `sales-icon.svg` (64x64px) - Sales funnel/CRM icon  
- `payments-icon.svg` (64x64px) - Payment/financial icon
- `ai-icon.svg` (64x64px) - AI/analytics icon

### How It Works Images
- `diagnose-step.jpg` (400x300px) - Shows analysis/diagnosis process
  - *Suggested: Business meeting, data analysis, system mapping*
- `design-build-step.jpg` (400x300px) - Shows development/building process
  - *Suggested: Software development, system architecture, technical planning*
- `operate-optimize-step.jpg` (400x300px) - Shows optimization/monitoring
  - *Suggested: Dashboard monitoring, performance analytics, continuous improvement*

### Partner Logos
- `mindset-logo.png` - Mindset company logo
- `burlington-logo.png` - Burlington English logo

### About Section
- `team-collaboration.jpg` (800x600px) - Team working together
  - *Suggested: Diverse team collaborating, educational professionals, technology experts*

### Solutions Page Images
- `lms-dashboard.jpg` (800x600px) - Learning management system interface
- `sales-funnel.jpg` (800x600px) - Sales process or CRM dashboard
- `payment-dashboard.jpg` (800x600px) - Financial/payment system interface
- `ai-analytics.jpg` (800x600px) - AI analytics dashboard with charts and data

## 🚀 Getting Started

1. **Clone or download** the project files to your web server
2. **Add images** to the `assets/images/` directory (see Image Requirements above)
3. **Open** `index.html` in your web browser or deploy to your web server

### Local Development

For local development, you can simply open the HTML files in your browser. For a better development experience with live reload:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js (if http-server is installed)
npx http-server

# Using PHP (if installed)
php -S localhost:8000
```

Then visit `http://localhost:8000` in your browser.

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🎯 Content Structure

### Homepage (`index.html`)
- **Hero Section**: Main value proposition and CTAs
- **Problem Statement**: Why infrastructure matters for education companies
- **Solution Pillars**: Four main service areas
- **How It Works**: 3-step process
- **Partners**: Trusted brands (Mindset, Burlington English)
- **About**: Company background
- **Contact**: Call-to-action for engagement

### Solutions Page (`solutions.html`)
- **Detailed Solutions**: In-depth look at each pillar
- **Implementation Process**: 5-step implementation approach
- **Technology Stack**: Platforms and tools used
- **Call-to-Action**: Consultation scheduling

## ✨ Key Features

### Design Elements
- **Apple-inspired**: Clean typography, generous white space, subtle shadows
- **Smooth Animations**: Fade-in effects and hover transitions
- **Mobile-First**: Responsive grid system and mobile navigation
- **Performance**: Optimized CSS and minimal JavaScript

### Interactive Elements
- Smooth scrolling navigation
- Mobile hamburger menu
- Hover effects on cards and buttons
- Intersection observer for scroll animations

### SEO & Accessibility
- Semantic HTML5 structure
- Alt text for images (when added)
- Proper heading hierarchy
- Focus management for keyboard navigation

## 🔧 Customization

### Colors
Brand colors are defined as CSS custom properties in `:root` for easy customization.

### Typography
Uses system fonts with SF Pro Display as the primary choice, falling back to system defaults.

### Layout
Built with CSS Grid and Flexbox for modern, flexible layouts.

## 📞 Contact Information

Update the contact information in both HTML files:
- Email: `contact@aifluent.com`
- Update links and contact forms as needed

## 🚀 Deployment

This is a static website that can be deployed to any web hosting service:

- **GitHub Pages**
- **Netlify**
- **Vercel**
- **Traditional web hosting**
- **AWS S3 + CloudFront**

Simply upload the files to your hosting provider and ensure the images are properly added to the `assets/images/` directory.

## 📝 Next Steps

1. **Add Images**: Source and optimize the required images
2. **Content Review**: Review and adjust copy as needed
3. **Contact Form**: Implement backend for contact form processing
4. **Analytics**: Add Google Analytics or similar tracking
5. **SEO**: Add meta descriptions and optimize for search engines
6. **Performance**: Optimize images and implement lazy loading if needed

---

Built with ❤️ for AIFLUENT - Infrastructure for fluent growth in education.