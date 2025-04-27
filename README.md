# Landing Page Maintenance Guide

This guide will help you maintain and customize the Hoogwerker Huren landing page. Follow these detailed instructions to make common updates while preserving the page's functionality and design.

## 1. Updating Text and Tailwind CSS Classes

### Main Content Sections

#### Header Navigation
```html
<nav class="container mx-auto px-4 sm:px-6 lg:px-8 py-4">
    <div class="flex-shrink-0">
        <a href="/" class="text-2xl font-bold text-blue-600">Hoogwerker Huren</a>
    </div>
```
To update the company name:
1. Locate the `<a>` tag within the `flex-shrink-0` div
2. Replace "Hoogwerker Huren" with your desired text
3. Keep the existing classes to maintain styling

#### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 mb-6">
    Hoogwerker Huren Harderwijk
    <span class="block text-blue-600 mt-2">Tijdelijk 10% Korting!</span>
</h1>
```
To modify the main headline:
1. Change the text within the `<h1>` tag
2. Maintain the nested `<span>` for the promotional text
3. Keep the responsive text classes (`text-4xl md:text-5xl lg:text-6xl`)

### Tailwind CSS Class Guide

Key classes explained:
- `container mx-auto`: Centers content with automatic margins
- `px-4 sm:px-6 lg:px-8`: Responsive padding (increases at different breakpoints)
- `text-4xl md:text-5xl lg:text-6xl`: Responsive text sizing
- `bg-white/95`: White background with 95% opacity

To modify styles:
1. Find the element you want to change
2. Reference the [Tailwind CSS documentation](https://tailwindcss.com/docs)
3. Replace existing classes while maintaining responsive prefixes (`sm:`, `md:`, `lg:`)

Example modification:
```html
<!-- Original -->
<div class="bg-white p-8 rounded-xl shadow-lg">

<!-- Modified with different colors -->
<div class="bg-gray-50 p-8 rounded-xl shadow-lg">
```

## 2. Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-blue-600">Kenmerken</a>
    <a href="#benefits" class="text-gray-600 hover:text-blue-600">Voordelen</a>
    <a href="#faq" class="text-gray-600 hover:text-blue-600">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-blue-600">Contact</a>
</div>
```

To update navigation links:
1. Identify the section ID you want to link to
2. Update the `href` attribute with the corresponding ID
3. Example: `<a href="#new-section">New Section</a>`

### Call-to-Action Links
Current CTA button:
```html
<a href="https://hansschuiling.nl" class="inline-flex items-center justify-center px-8 py-4">
    Direct Huren
</a>
```

To update external links:
1. Replace `https://hansschuiling.nl` with your desired URL
2. Ensure the URL includes `https://` for secure connections
3. Test the link after updating

## 3. Linking Privacy and Terms Pages

### Adding Footer Links
Locate the footer section:
```html
<footer class="bg-gray-900 text-white py-16">
    <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
```

Add privacy and terms links:
```html
<div class="border-t border-gray-800 mt-12 pt-8 text-center text-gray-400">
    <p>&copy; 2024 Hoogwerker Huren Harderwijk. Alle rechten voorbehouden.</p>
    <!-- Add these lines below the copyright notice -->
    <div class="mt-4 space-x-4">
        <a href="/privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a>
        <a href="/terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a>
    </div>
</div>
```

## Troubleshooting Tips

1. **Broken Layouts**
   - Check for missing closing tags
   - Verify all container divs are properly nested
   - Ensure responsive classes are correctly prefixed

2. **Missing Styles**
   - Confirm Tailwind CDN is properly loaded
   - Check for typos in class names
   - Verify class combinations are valid

3. **Non-Working Links**
   - Ensure IDs match exactly (case-sensitive)
   - Verify file paths for internal pages
   - Test external URLs in a new tab

## Best Practices

1. Always backup the file before making changes
2. Test changes on multiple screen sizes
3. Validate links after updating
4. Maintain consistent spacing and indentation
5. Keep the responsive design intact by preserving breakpoint classes

Need further assistance? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).