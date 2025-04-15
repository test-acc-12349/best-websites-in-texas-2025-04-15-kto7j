# Landing Page Maintenance Guide
A comprehensive guide for maintaining and customizing the Best Websites TX landing page.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains the company name and navigation menu. To update:

1. Company Name:
```html
<!-- Find this line in the header section -->
<div class="text-2xl font-bold text-blue-600">
    Best Websites TX  <!-- Change this text -->
</div>
```

2. Navigation Menu Items:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features">Features</a>  <!-- Change menu text here -->
    <a href="#benefits">Benefits</a>
    <a href="#faq">FAQ</a>
    <a href="#contact">Contact</a>
</div>
```

### Hero Section
To modify the main headline and subheading:
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-6">
    Best Websites In Texas  <!-- Main headline -->
</h1>
<p class="text-xl md:text-2xl text-gray-600 mb-12">
    Custom Websites For Your Business  <!-- Subheading -->
</p>
```

### Understanding Tailwind Classes
Common classes explained:
- `text-4xl`: Large text size
- `md:text-5xl`: Larger text on medium screens
- `font-bold`: Bold text weight
- `mb-6`: Margin bottom spacing
- `bg-blue-600`: Blue background color
- `text-white`: White text color

To modify a style:
1. Find the element you want to change
2. Locate the class attribute
3. Modify or add Tailwind classes

Example:
```html
<!-- Original -->
<button class="bg-blue-600 text-white">

<!-- Modified to red -->
<button class="bg-red-600 text-white">
```

## Fixing Broken Links

### Navigation Menu Links
Current internal links:
```html
<a href="#features">Features</a>
<a href="#benefits">Benefits</a>
<a href="#faq">FAQ</a>
<a href="#contact">Contact</a>
```

To update:
1. For internal sections, keep the `#` followed by the section ID
2. For external links, use the full URL:
```html
<a href="https://yourwebsite.com/page">Link Text</a>
```

### Call-to-Action Buttons
Current CTA links:
```html
<!-- Hero section -->
<a href="https://sigmaseo.io" class="inline-block bg-blue-600...">
    Get Started Today
</a>

<!-- CTA section -->
<a href="https://sigmaseo.io" class="inline-block bg-white...">
    Contact Us Now
</a>
```

To update:
1. Replace `https://sigmaseo.io` with your desired URL
2. Ensure the URL includes `https://` or `http://`

## Linking Privacy and Terms Pages

### Footer Legal Links
Current placeholder links:
```html
<div>
    <h4 class="text-lg font-semibold text-white mb-4">Legal</h4>
    <ul class="space-y-2">
        <li><a href="#" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```

To add proper links:
1. Create privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

### Social Media Links
Update social media links in the footer:
```html
<div class="flex space-x-4">
    <a href="https://facebook.com/yourpage" class="text-2xl hover:text-white transition-colors duration-300">
        <i class="fab fa-facebook"></i>
    </a>
    <!-- Repeat for Twitter and LinkedIn -->
</div>
```

## Troubleshooting

Common Issues:
1. **Broken Layout**: Check if you've maintained all responsive classes (md:, lg:, etc.)
2. **Missing Icons**: Ensure Font Awesome CSS is properly linked
3. **Non-working Links**: Verify href attributes begin with `#` for internal links or `https://` for external links

Need Help?
- Double-check your changes against the original code
- Use browser inspection tools (F12) to identify CSS issues
- Ensure all HTML tags are properly closed
- Maintain the existing class structure when making changes

Remember: Always test your changes across different screen sizes using browser developer tools before publishing updates.