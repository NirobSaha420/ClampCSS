<div align="center">
  <h1>
    <a href="https://clamp.ascender-solutions.com">ClampCSS</a>
  </h1>
  
  <p>
    <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version">
    <img src="https://img.shields.io/badge/size-3.7KB_gzipped-purple.svg" alt="Size">
    <img src="https://img.shields.io/badge/dependencies-none-darkgreen" alt="Dependencies">
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="License">
    <img src="https://img.shields.io/badge/css-modern-ff69b4.svg" alt="CSS">
  </p>
</div>

<p align="center">
Ascend Your Vision with fluid typography, responsive utilities, and performance-optimized CSS-only framework 🔥
</p>

> **Ready to Clamp? ClampCSS is a modern, minimal, production-ready CSS framework featuring fluid typography & spacing, responsive utilities, accessibility-first design, and zero JavaScript dependencies.**  
> 4 goals : Reduce your number of breakpoints, make web a little more accessible and a hope that it will reduce some headaches comes from build process and dependencies with some rememberable, easy to override codes.

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
- [💬 Community](#-community)

## ✨ Features

| Feature | Description |
|---------|-------------|
| **Fluid Typography System** | CSS `clamp()` based responsive typography |
| **Fluid Spacing System** | CSS `clamp()` based responsive Spacing |
| **Modern CSS Reset** | Normalized base styles with accessibility focus |
| **Utility-First Approach** | Comprehensive utility classes for rapid development |
| **Performance Optimized** | Minimal CSS with smart defaults |
| **Accessibility First** | WCAG-compliant focus management and semantic structure |
| **Responsive by Design** | Mobile-first responsive utilities and components |
| **Zero JavaScript** | Pure CSS solution, no dependencies |

## 📦 Installation

### Production-Ready CDN (Recommended)
For optimal performance in production environments:

```html
<!-- DNS pre-connection for faster loading -->
<link rel="preconnect" href="https://clamp.ascender-solutions.com" crossorigin>

<!-- Preload CSS for critical rendering path -->
<link rel="preload" type="text/css" as="style" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css" fetchpriority="high"> <!-- use fetchpriority as your requirement -->

<!-- Main stylesheet -->
<link rel="stylesheet" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css">
```

### Quick Start (Simpler Alternative)
```html
<link rel="stylesheet" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css">
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
    <link rel="preconnect" href="https://clamp.ascender-solutions.com" crossorigin>
    <link rel="preload" type="text/css" as="style" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css" fetchpriority="high"> <!-- use fetchpriority as your requirement -->
    <link rel="stylesheet" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css">
    
    <!-- Your custom CSS -->
    <link rel="stylesheet" href="/path/to/styles.css">
</head>
<body>
    <!-- Your content here -->
</body>
</html>
```
### Alternative Method
Self-Hosted
Download the file from:

```html
https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css
```
Include in your project:
```html
<link rel="stylesheet" href="/css/clamp.min.css">
```
### Content Security Policy (CSP)
If you use CSP, add these directives:

```http
Content-Security-Policy: 
  style-src 'self' https://clamp.ascender-solutions.com;
  font-src 'self' https://clamp.ascender-solutions.com;
  connect-src 'self' https://clamp.ascender-solutions.com;
```
For stricter CSP:
```http
Content-Security-Policy: 
  style-src 'self' https://clamp.ascender-solutions.com;
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
    <link rel="stylesheet" href="https://clamp.ascender-solutions.com/v1.0.0/clamp.min.css">
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
Utility Classes
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
  --spacing: 0.5rem; /*16px base*/
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
- **Focus Management:** Visible focus indicators for keyboard navigation

- **Reduced Motion:** Respects prefers-reduced-motion preferences

- **Screen Reader Ready:** Semantic HTML structure

- **High Contrast:** Color palette with sufficient contrast ratios


## 🏗️ Performance
- **Minimal Footprint:** ~3.7KB gzipped

- **Efficient Selectors:** Optimized CSS specificity

- **Critical Path Optimization:** Preload and prefetch hints

- **No Render Blocking:** Non-blocking CSS loading

## 🌐 Browser Support
- Chrome
- Firefox
- Safari
- Edge
- Opera

**Note:** Uses modern CSS features like `clamp()` and CSS Custom Properties.

## 📄 License
MIT License © 2025 Nirob Chandra Saha

## 💬 Community
- Facebook Public Group: ClampCSS

- Facebook Page: Mr. Nr

- Email: nr.classic2077@gmail.com or cto@ascender-solutions.com

---

<div align="center">
Built with ❤️ by Mr. Nr (Nirob Chandra Saha)

  [Get Started](#-installation) • [View Examples](https://clamp.ascender-solutions.com/examples)
</div>

---
