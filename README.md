# Landing Page Maintenance Guide
## For 101Headshots Corporate Photography Website

This guide provides detailed instructions for maintaining and customizing the 101Headshots landing page. Whether you're new to web development or need a quick reference, follow these step-by-step instructions.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the logo and navigation menu. To modify:

```html
<!-- Logo Text -->
<a href="/" class="text-2xl font-bold bg-gradient-to-r from-purple-500 to-pink-500 bg-clip-text text-transparent">101Headshots</a>
```
- To change the logo text, simply replace "101Headshots"
- The gradient colors can be modified by changing `from-purple-500` and `to-pink-500`

### Hero Section
Located at the top of the page:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold leading-tight mb-8">
    Louisburg, Kansas Corporate Headshot Photography Services
</h1>
```
- Replace the heading text while maintaining the existing classes
- Text sizes are responsive:
  - Mobile: `text-4xl`
  - Tablet: `md:text-5xl`
  - Desktop: `lg:text-6xl`

### Feature Cards
Each feature card follows this structure:

```html
<div class="bg-gray-800/50 rounded-2xl p-8 hover:bg-gray-800">
    <h3 class="text-xl font-semibold mb-4">Core Focus</h3>
    <p class="text-gray-400">Specialized expertise in corporate photography...</p>
</div>
```
To modify:
1. Locate the feature card you want to update
2. Change the heading text within the `<h3>` tags
3. Update the description within the `<p>` tags
4. Maintain existing classes for consistent styling

## Managing Links

### Navigation Menu Links
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-300 hover:text-white">Features</a>
    <a href="#benefits" class="text-gray-300 hover:text-white">Benefits</a>
    <a href="#contact" class="text-gray-300 hover:text-white">Contact</a>
</div>
```
To update:
1. Identify the link you want to change
2. Modify the `href` attribute:
   - Internal sections use `#section-name`
   - External pages use full URLs
3. Update the link text between the `<a>` tags

### Call-to-Action Buttons
```html
<a href="https://www.101headshots.com" class="inline-block px-8 py-4 bg-gradient-to-r from-purple-600 to-pink-600">
    Transform Your Brand Today
</a>
```
To modify:
1. Update the `href` with your booking URL
2. Change button text as needed
3. Maintain the existing classes for styling

## Adding Privacy and Terms Pages

### Footer Link Updates
Current footer structure:
```html
<div class="mt-4 md:mt-0">
    <a href="https://www.101headshots.com" class="text-gray-400 hover:text-white">Terms</a>
    <span class="mx-3 text-gray-600">|</span>
    <a href="https://www.101headshots.com" class="text-gray-400 hover:text-white">Privacy</a>
</div>
```

To add proper links:
1. Create new files:
   - `privacy.html`
   - `terms.html`
2. Update the href attributes:
```html
<a href="/privacy.html" class="text-gray-400 hover:text-white">Privacy</a>
<a href="/terms.html" class="text-gray-400 hover:text-white">Terms</a>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Gradients**
   - Ensure all gradient classes include both `from-` and `to-` components
   - Example: `bg-gradient-to-r from-purple-500 to-pink-500`

2. **Responsive Issues**
   - Check that responsive classes are properly ordered:
     - Base (mobile): `text-sm`
     - Tablet: `md:text-base`
     - Desktop: `lg:text-lg`

3. **Link Problems**
   - Internal links should start with `#` for same-page sections
   - External links need complete URLs starting with `https://`
   - File links should use relative paths (`/privacy.html`)

### Need Help?
If you encounter issues:
1. Verify all classes match exactly as shown in examples
2. Check for proper closing tags
3. Ensure all links have valid destinations
4. Test responsive layouts using browser dev tools

Remember to always backup your files before making changes, and test all modifications in a development environment first.