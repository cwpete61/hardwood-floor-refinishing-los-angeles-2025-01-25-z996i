# Tykoon Wood Floors Landing Page - Maintenance Guide

This guide will help you maintain and customize the Tykoon Wood Floors landing page. Whether you're new to web development or just getting started, follow these instructions to make updates while preserving the page's functionality and design.

## Table of Contents
1. [Updating Text and Styling](#updating-text-and-styling)
2. [Managing Links](#managing-links)
3. [Adding Privacy and Terms Pages](#adding-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Styling

### Header Section
The header contains the company name and navigation menu. To update:

```html
<!-- Company Name -->
<span class="text-2xl font-bold text-blue-600">Tykoon Wood Floors</span>
```
- Replace "Tykoon Wood Floors" with your company name
- Keep the classes unchanged to maintain styling

### Hero Section
Located at the top of the page with the main heading and call-to-action buttons:

```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Hardwood Floor Refinishing Los Angeles
</h1>
```
- Update the heading text while keeping the classes
- The `md:` and `lg:` prefixes control responsive text sizes
- Don't remove these prefixes as they ensure proper display on different devices

### Tailwind CSS Class Guide
Common classes used throughout:
- `text-{size}`: Controls text size (xl, 2xl, 3xl, etc.)
- `font-{weight}`: Controls text boldness (normal, medium, semibold, bold)
- `text-{color}-{shade}`: Sets text color (blue-600, gray-900, etc.)
- `bg-{color}-{shade}`: Sets background color
- `p-{number}`: Sets padding (p-4, p-8, etc.)
- `m-{number}`: Sets margin
- `rounded-{size}`: Controls corner roundness

## Managing Links

### Navigation Menu Links
Current navigation links are:
```html
<div class="hidden md:flex space-x-8">
    <a href="#services" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Services</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600 transition-colors duration-300">Contact</a>
</div>
```

To update links:
1. Locate the `href` attribute
2. Replace the value with your new link
3. For internal page sections, use `#section-name`
4. For external links, use the full URL: `https://example.com`

### Call-to-Action Buttons
The "Get a Free Quote" button needs updating:
```html
<a href="https://Form.com" class="inline-flex items-center justify-center px-8 py-4 text-lg font-semibold text-white bg-blue-600 rounded-lg hover:bg-blue-700 transition-colors duration-300 transform hover:scale-105">
```
Replace `https://Form.com` with your actual form URL

## Adding Privacy and Terms Pages

### Step 1: Create New Pages
1. Create two new files in your project folder:
   - `privacy.html`
   - `terms.html`

### Step 2: Update Footer Links
Locate these lines in the footer:
```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
</ul>
```

Replace the `#` with proper file paths:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Links**
   - Check for typos in URLs
   - Ensure file names match exactly
   - Verify file locations in your project folder

2. **Styling Problems**
   - Don't remove Tailwind CSS classes unless you're sure about the impact
   - Keep the `md:` and `lg:` prefixes for responsive design
   - Test on different screen sizes after making changes

3. **Layout Issues**
   - Maintain the container structure:
     ```html
     <div class="container mx-auto px-4 sm:px-6 lg:px-8">
     ```
   - Don't remove responsive classes
   - Keep the grid system intact in multi-column layouts

### Need Help?
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Double-check your changes against the original code
- Test all links after making updates
- View the page in different browsers to ensure compatibility

Remember to always make a backup of your files before making significant changes!