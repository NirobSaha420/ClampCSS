<div align="center">
  <h1>
    <a href="https://clamp.ascender-solutions.com">ClampCSS</a>
  </h1>
  
  <p>
    <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version">
    <img src="https://img.shields.io/badge/size-3.7KB_gzipped-purple.svg" alt="Size">
    <img src="https://img.shields.io/badge/dependencies-none-darkgreen" alt="Dependencies">
    <img src="https://img.shields.io/jsdelivr/gh/hm/NirobSaha420/ClampCSS" alt="jsDelivr hits">
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="License">
    <img src="https://img.shields.io/badge/css-modern-ff69b4.svg" alt="CSS">
  </p>
</div>

<p align="center">
Ascend Your Vision with fluid typography, responsive utilities, and performance-optimized CSS-only framework 🔥
</p>

> **Ready to Clamp? ClampCSS is a modern, minimal, production-ready CSS framework featuring fluid typography & spacing, responsive utilities, accessibility-first design, and zero JavaScript dependencies.**  
> 3 goals : Reduce your number of breakpoints and build time with fluid utilities, make web a little more accessible and a hope that it will reduce some headaches comes from build process and dependencies with some rememberable, easy to override codes.

---

## 🌐 Website

🏃 **[clamp.ascender-solutions.com](https://clamp.ascender-solutions.com)** 

## 📋 Table of Contents

- [✨ Features](#-features)
- [📦 Installation](#-installation)
- [🚀 Quick Start](#-quick-start)
- [🎨 Core Features](#-core-features)
- [📐 Layout System](#-layout-system)
- [🔧 Customization](#-customization)
- [♿ Accessibility Features](#-accessibility-features)
- [🏗️ Performance](#️-performance)
- [🌐 Browser Support](#-browser-support)
- [📄 License](#-license)
- [❓ Frequently Asked Questions](#-frequently-asked-questions)
- [💬 Community](#-community)

## ✨ Features

| Feature | Description |
|---------|-------------|
| **Fluid Typography System** | CSS `clamp()` based responsive typography |
| **Fluid Spacing System** | CSS `clamp()` based responsive Spacing |
| **Modern CSS Reset** | Normalized base styles with accessibility focus |
| **Utility Classes** | Comprehensive utility classes for rapid development |
| **Performance Optimized** | Minimal CSS with smart defaults |
| **Accessibility First** | WCAG-compliant focus management and semantic structure |
| **Responsive by Design** | Mobile-first responsive utilities and components |
| **Zero JavaScript** | Pure CSS solution, no dependencies |

## 📦 Installation

### Production-Ready CDN (Recommended)
For optimal performance in production environments:

```html
<!-- DNS pre-connection for faster loading -->
<link rel="preconnect" href="https://cdn.jsdelivr.net" crossorigin>

<!-- Main stylesheet -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/NirobSaha420/ClampCSS@1.0.0/dist/v1.0.0/clamp.min.css" fetchpriority="high"> <!-- use fetchpriority for above-the-fold styles -->
```

### Simpler Alternative
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/NirobSaha420/ClampCSS@1.0.0/dist/v1.0.0/clamp.min.css">
```

### Complete HTML Template
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My ClampCSS Project</title>
    
    <!-- ClampCSS Optimized Installation -->
    <link rel="preconnect" href="https://cdn.jsdelivr.net" crossorigin>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/NirobSaha420/ClampCSS@1.0.0/dist/v1.0.0/clamp.min.css" fetchpriority="high">
    
    <!-- Your custom CSS -->
    <link rel="stylesheet" href="/path/to/styles.css" media="print" onload="this.media='all'">
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```
### Download & Self-Host
Download the file from:

```html
https://cdn.jsdelivr.net/gh/NirobSaha420/ClampCSS@1.0.0/dist/v1.0.0/clamp.min.css
```
Include in your project:
```html
<link rel="stylesheet" href="/css/clamp.min.css">
```
### Content Security Policy (CSP)
If you use CSP, add these directives:

```http
Content-Security-Policy: 
  style-src 'self' https://cdn.jsdelivr.net;
  font-src 'self' https://cdn.jsdelivr.net;
  connect-src 'self' https://cdn.jsdelivr.net;
```
For stricter CSP:
```http
Content-Security-Policy: 
  style-src 'self' https://cdn.jsdelivr.net;
  font-src 'self';
  default-src 'self';
  script-src 'none';  # ClampCSS has no JavaScript
```

### 🚀 Quick Start
Basic Structure
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ClampCSS Project</title>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/NirobSaha420/ClampCSS@1.0.0/dist/v1.0.0/clamp.min.css">
</head>
<body>
    <div class="container">
        <h1 class="text-3xl color-primary">Hello, ClampCSS!</h1>
        <p class="text-md mt-2">A modern CSS framework with fluid typography.</p>
        <button class="btn mt-3">Get Started</button>
    </div>
</body>
</html>
```

## 🎨 Core Features
### Utility Classes Reference
| Category | Class Pattern | Example |
|----------|---------------|---------|
| Spacing | `m-{0-4}`, `p-{0-4}` | `m-2 p-4` |
| Typography | `text-{xs, sm, md, lg, xl, 2xl, 3xl, 4xl}` | `text-2xl` |
| Colors | `color-{primary, success, warning, danger}` | `color-primary` |
| Background | `bg-{primary, success, white, black}` | `color-white`, `bg-success` |
| Flexbox | `flex`, `flex-center`, `gap-{0-4}` | `flex`, `flex-center`, `gap-2` |
| Grid | `grid`, `grid-cols-{1-12}` | `grid grid-cols-3` |
| Border Radius | `bra-{5, 10, 15, 25, 50}` | `bra-10` | 
| Shadows | `shadow-{none, sm, md, lg, xl}` | `shadow-lg` |   

Fluid Typography
```html
<h1 class="text-4xl">Fluid Heading</h1> /* 48-72px */
<p class="text-lg">Responsive paragraph text</p> /* 18-22px */
<span class="text-xs">Small fluid text</span> /*10.666-12px*/
```

Fluid Spacing
```html
<!-- Spacing, (0 - 4 values) -->
<div class="m-2 p-4">
    <!-- Margin & Padding -->
</div>
```

Responsive Grid
```html
<div class="grid grid-cols-3 gap-2">
    <div class="bg-primary p-2">Column 1</div>
    <div class="bg-success p-2">Column 2</div>
    <div class="bg-warning p-2">Column 3</div>
</div>
```
Example Usage
```html
<!-- Spacing, (0 - 4 values) -->
<div class="m-2 p-4">
    <!-- Margin & Padding -->
</div>

<!-- Font Size, (xs - 4xl values) -->
<p class="text-lg">Responsive paragraph text</p>

<!-- Colors -->
<p class="color-primary bg-white">Colored text</p>

<!-- Flexbox -->
<div class="flex flex-center gap-2">
    <div>Centered</div>
    <div>Items</div>
</div>

<!-- Border Radius, (5,10,15,25,50% values) -->
<div class="bra-10 shadow-lg p-4">Border Radius</div>
```

## 📐 Layout System
Container
```html
<div class="container">
    <!-- Content constrained to responsive max-width -->
</div>
```
Grid System
```html
<div class="grid grid-cols-1 gap-4">
    <!-- Responsive columns -->
</div>
```
Flexbox System
```html
<div class="row">
    <div class="col-12">
        <!-- Responsive column -->
    </div>
</div>
```

## 🔧 Customization
CSS Custom Properties
Override default variables in your CSS:
```css
:root {
      /* Color Palette */
  --color-white: #fff;
  --color-black: #000;
  --color-primary: #005fcc;
  --color-success: #28a745;
  --color-warning: #ffc107;
  --color-danger: #dc3545;

  /* Transitions */
  --transition: 0.3s ease;

  /* layout */
  --aspect-ratio: auto; /* Default value, change with inline css for each img tag */

  /* SPACING */
  --spacing: 0.5rem;
  --spacing-vw: 0.5vw;

  /* FLUID TYPOGRAPHY */
  --text-xs: clamp(0.666666rem, 0.64rem + 0.1333333vw, 0.75rem);  /*10.666-12px*/
  --text-sm: clamp(0.875rem, 0.84rem + 0.18vw, 1rem);  /* 14-16px */
  --text-md: clamp(1rem, 0.96rem + 0.2vw, 1.125rem);  /* 16-18px */
  --text-lg: clamp(1.125rem, 1.05rem + 0.3vw, 1.375rem);  /* 18-22px */
  --text-xl: clamp(1.25rem, 1.15rem + 0.5vw, 1.75rem);  /* 20-28px */
  --text-2xl: clamp(1.5rem, 1.3rem + 1vw, 2.25rem);  /* 24-36px */
  --text-3xl: clamp(1.875rem, 1.55rem + 1.5vw, 3rem);  /* 30-48px */
  --text-4xl: clamp(3rem, 2.6rem + 2vw, 4.5rem);  /* 48-72px */

  /* SHADOWS */
  --shadow-none:0 0 #0000;
  --shadow-sm: 0 1px 3px 0 rgb(0 0 0 / 0.07);
  --shadow-md: 0 4px 6px -1px rgb(0 0 0 / 0.1),0 2px 4px -2px rgb(0 0 0 / 0.1);
  --shadow-lg: 0 10px 15px -3px rgb(0 0 0 / 0.1),0 4px 6px -4px rgb(0 0 0 / 0.1);
  --shadow-xl: 0 20px 25px -5px rgb(0 0 0 / 0.1),0 8px 10px -6px rgb(0 0 0 / 0.1);
  --shadow-inner-sm: inset 0 1px 2px 0 rgb(0 0 0 / 0.05);
  --shadow-inner-md: inset 0 4px 6px -1px rgb(0 0 0 / 0.1), inset 0 2px 4px -2px rgb(0 0 0 / 0.1);
  --shadow-inner-lg: inset 0 10px 15px -3px rgb(0 0 0 / 0.1), inset 0 4px 6px -4px rgb(0 0 0 / 0.1);
  --shadow-inner-xl: inset 0 20px 25px -5px rgb(0 0 0 / 0.1), inset 0 8px 10px -6px rgb(0 0 0 / 0.1);
}
```

## ♿ Accessibility Features
- **Focus Management:** Uses `:focus-visible` for intelligent focus indicators that only appear during keyboard navigation

- **Reduced Motion:** Respects `prefers-reduced-motion` media query

- **Screen Reader Ready:** Semantic HTML structure

- **High Contrast:** Color palette with sufficient contrast ratios


## 🏗️ Performance
- **Minimal Footprint:** ~3.7KB gzipped

- **Efficient Selectors:** Low-specificity single-class selectors using `:where()` for complex patterns like input[type="text"]

- **Critical Path Optimization:** Preconnect and `fetchpriority="high"` hints in installation guide. `Print` loading trick for non-critical CSS.

- **No Render Blocking:** Optimized loading patterns shown in installation examples

- **Zero Runtime:** Pure CSS with no JavaScript overhead

## 🌐 Browser Support
- Chrome
- Firefox
- Safari
- Edge
- Opera

**Note:** Uses modern CSS features like `clamp()` and CSS Custom Properties. [View browser support details on caniuse.com](https://caniuse.com/css-math-functions)

## 📄 License
MIT License © 2025 Nirob Chandra Saha


## ❓ Frequently Asked Questions

### Q: Why use ClampCSS over Tailwind/Bootstrap?
A: ClampCSS is significantly smaller (~3.7KB vs. hundreds of KB), features built-in fluid typography/spacing using modern CSS, and requires no JavaScript, build process, or configuration to start.

### Q: Does it work with React/Vue/Angular?
A: Yes! It's purely CSS and completely framework-agnostic. Just include the stylesheet.

### Q: How does ClampCSS handle CSS specificity?
A: ClampCSS uses a flat specificity structure. All utility classes have single-class specificity (0,1,0), and complex selectors use `:where()` which has zero specificity. This makes overriding styles predictable and easy.

### Q: How to override styles?
A: You can override any utility class with your own CSS using higher specificity. For global theming, override the CSS Custom Properties (variables) in the `:root` selector as shown in the [Customization](#-customization) section.

### Q: Can I use it with my existing CSS?
A: Absolutely. It's designed to be non-invasive and can be used as a base layer or alongside other styles. Its reset is mild and its utility classes use a low-specificity single-class pattern.

### Q: What accessibility standards does ClampCSS follow?
A: ClampCSS follows WCAG standards. Focus management uses `:focus-visible` for keyboard users, and animations respect `prefers-reduced-motion`.


## 💬 Community
- Facebook Public Group: ClampCSS

- Facebook Profile : [Mr. Nr](https://www.facebook.com/NirobChandraSaha)

- Email: nr.classic2077@gmail.com or cto@ascender-solutions.com

---

<div align="center">
Built with ❤️ by Mr. Nr (Nirob Chandra Saha)

  [Get Started](#-installation) • [View Examples](https://clamp.ascender-solutions.com/examples)
</div>

---
