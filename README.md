# Landing Page Maintenance Guide
## El Mejor Vendedor Website

This guide provides detailed instructions for maintaining and customizing the El Mejor Vendedor landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the main navigation and logo. To update:

1. **Logo Text:**
```html
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">
    El Mejor Vendedor  <!-- Change this text to update the logo -->
</a>
```

2. **Navigation Menu Items:**
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Update menu text here -->
    <a href="#benefits">Benefits</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
Located at the top of the page:
```html
<h1 class="text-4xl md:text-6xl lg:text-7xl font-extrabold mb-8">
    Hola mundo.  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-300 mb-12">
    Un saludo para todos los humanos  <!-- Subheadline -->
</p>
```

### Tailwind CSS Classes Explained
- `text-4xl`: Sets font size (increases with md: and lg: prefixes)
- `mb-8`: Adds margin bottom spacing
- `font-extrabold`: Controls font weight
- `text-gray-300`: Sets text color

To modify styles:
1. Find the element you want to change
2. Locate its class attribute
3. Add or replace Tailwind classes
4. Maintain responsive prefixes (md:, lg:) for different screen sizes

## Managing Links

### Navigation Links
Current internal links in the navigation:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#contact">Contact</a>
```

To update:
1. Replace the `#` with your new link destination
2. For external links, use complete URLs
3. For internal pages, use relative paths

Example:
```html
<a href="https://yoursite.com/features">Features</a>
<a href="/benefits.html">Benefits</a>
```

### Call-to-Action Buttons
Located in hero and contact sections:
```html
<a href="https://elmejorvendedor.com" class="inline-block bg-gradient-to-r from-purple-600 to-pink-600...">
    Start Selling Now  <!-- Update button text here -->
</a>
```

### Email Links
Update email addresses in contact section and footer:
```html
<a href="mailto:hola@elmejorvendedor.com">
    hola@elmejorvendedor.com
</a>
```

## Adding Privacy and Terms Pages

### Current Footer Links Structure
```html
<div>
    <h4 class="font-semibold mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To link privacy and terms pages:

1. Create new HTML files:
   - `privacy.html`
   - `terms.html`

2. Update the footer links:
```html
<li><a href="/privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="/terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

3. Maintain consistent styling by copying these classes:
   - `text-gray-400`: Default text color
   - `hover:text-white`: Hover state color
   - `transition-colors duration-300`: Smooth color transition

## Troubleshooting

### Common Issues and Solutions

1. **Broken Internal Links**
   - Ensure hash links (#features, #benefits) match section IDs
   - Check file paths for relative links
   - Verify file names are exact matches (case-sensitive)

2. **Responsive Design Issues**
   - Keep responsive prefixes (md:, lg:) when updating classes
   - Test on multiple screen sizes
   - Don't remove the viewport meta tag in head

3. **Styling Problems**
   - Verify Tailwind CSS CDN link is working
   - Check for typos in class names
   - Maintain existing class structure for consistency

### Need Help?
- Check the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Validate HTML at [W3C Validator](https://validator.w3.org/)
- Test responsive design using browser developer tools

Remember to always backup your files before making changes and test thoroughly across different devices and browsers.