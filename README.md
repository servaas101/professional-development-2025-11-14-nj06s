# Leadership Academy Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain, update, and customize your Leadership Academy landing page. Whether you're updating text, fixing links, or adding new pages, you'll find clear, step-by-step instructions tailored specifically to this website's structure.

---

## Table of Contents

1. [Understanding the Page Structure](#understanding-the-page-structure)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Colors & Styling](#modifying-colors--styling)
4. [Fixing & Managing Links](#fixing--managing-links)
5. [Adding Privacy & Terms Pages](#adding-privacy--terms-pages)
6. [Mobile Responsiveness Tips](#mobile-responsiveness-tips)
7. [Troubleshooting Common Issues](#troubleshooting-common-issues)

---

## Understanding the Page Structure

Your landing page is organized into several key sections. Here's what each section does:

### Main Sections of Your Page

```
Header Navigation (Sticky at top)
    ↓
Hero Section (Large welcome area with main message)
    ↓
Features Section (3 core features displayed)
    ↓
Benefits Section (3 main benefits)
    ↓
CTA Section (Call-to-action with background image)
    ↓
Testimonials Section (Customer success stories)
    ↓
About Us Section (Company information)
    ↓
Final CTA Section (Last call-to-action)
    ↓
Contact Form Section
    ↓
Footer (Links and company info)
```

### File Organization

Your website consists of:
- **index.html** - The main landing page (the file you received)
- **privacy.html** - Privacy policy page (you'll create this)
- **terms.html** - Terms of service page (you'll create this)
- **blog.html** - Blog page (optional, already linked)

---

## Updating Text Content

### Finding & Editing Text

The easiest way to find and edit text is to use your text editor's search function (Ctrl+F on Windows, Cmd+F on Mac).

### 1. Updating the Header/Navigation Brand Name

**Location:** Near the top of the file, inside the `<header>` tag

**Current Code:**
```html
<span class="text-2xl font-bold tracking-tight">Leadership</span>
```

**How to Change It:**
1. Open your `index.html` file in a text editor (like Notepad, VS Code, or Sublime Text)
2. Find the line with `<span class="text-2xl font-bold tracking-tight">Leadership</span>`
3. Replace `Leadership` with your company name
4. Save the file (Ctrl+S or Cmd+S)

**Example:** If your company is "Executive Growth Academy":
```html
<span class="text-2xl font-bold tracking-tight">Executive Growth Academy</span>
```

---

### 2. Updating the Hero Section (Main Headline)

**Location:** The large text at the top of the page

**Current Code:**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold tracking-tight mb-6 leading-tight">
    Professional<br><span class="text-[#FF5A5F]">Development</span>
</h1>
```

**How to Change It:**
1. Search for `Professional<br><span class="text-[#FF5A5F]">Development</span>`
2. The `<br>` creates a line break. You can keep it or remove it
3. Replace the text while keeping the HTML tags

**Example:** For a different message:
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold tracking-tight mb-6 leading-tight">
    Transform Your<br><span class="text-[#FF5A5F]">Career Path</span>
</h1>
```

**Important:** Keep the `<span class="text-[#FF5A5F]">` and `</span>` tags around the word you want in coral red color.

---

### 3. Updating the Hero Subtitle

**Location:** Below the main headline

**Current Code:**
```html
<p class="text-xl md:text-2xl text-gray-300 mb-8 leading-relaxed font-medium">
    Transform Your Skills. Lead With Confidence.
</p>
```

**How to Change It:**
1. Search for `Transform Your Skills. Lead With Confidence.`
2. Replace it with your own tagline
3. Keep the `<p>` tags and all the `class` attributes

**Example:**
```html
<p class="text-xl md:text-2xl text-gray-300 mb-8 leading-relaxed font-medium">
    Elevate Your Team. Achieve Excellence.
</p>
```

---

### 4. Updating the Hero Description Paragraph

**Location:** Longer text below the subtitle

**Current Code:**
```html
<p class="text-lg text-gray-400 mb-12 leading-relaxed max-w-xl">
    Unlock your full potential through our comprehensive professional development programs. 
    Gain the confidence, skills, and strategic mindset needed to lead with excellence in 
    today's dynamic business environment.
</p>
```

**How to Change It:**
1. Search for `Unlock your full potential`
2. Replace the paragraph text with your own message
3. Keep all the HTML tags and class names exactly as they are

---

### 5. Updating Feature Titles and Descriptions

**Location:** The three feature cards in the "Core Features" section

**Current Feature 1 Code:**
```html
<h3 class="text-2xl font-bold mb-4">Know Yourself to Grow</h3>
<p class="text-gray-400 leading-relaxed mb-6">
    Develop profound self-awareness through scientifically-backed assessments...
</p>
```

**How to Change It:**
1. Search for `Know Yourself to Grow`
2. Replace the title with your feature title
3. Find the paragraph below it and replace that text too
4. Keep all HTML tags intact

**Important:** There are THREE features. Search for each one:
- Feature 1: `Know Yourself to Grow`
- Feature 2: `From Good to Great`
- Feature 3: `Designed Purpose`

---

### 6. Updating Benefit Titles

**Location:** The three benefit items in the "Transform Your Potential" section

**Current Code:**
```html
<h3 class="text-2xl font-bold">Accessible Growth Anytime</h3>
```

**How to Change It:**
1. Search for each benefit title:
   - `Accessible Growth Anytime`
   - `Unlock Your Potential`
   - `Expert Guidance`
2. Replace each title with your own benefit names
3. Update the description paragraph below each title

---

### 7. Updating Testimonials

**Location:** The "Success Stories" section with customer reviews

**Current Testimonial Code:**
```html
<p class="text-gray-300 mb-6 leading-relaxed text-lg">
    "This program completely transformed my approach to leadership..."
</p>
<div class="border-t border-gray-700 pt-6">
    <p class="font-bold text-lg">Sarah Chen</p>
    <p class="text-gray-400">Senior Manager, Tech Innovation</p>
</div>
```

**How to Change It:**
1. Search for the testimonial text you want to replace
2. Replace the quote text within the `<p>` tags
3. Replace the customer name (e.g., `Sarah Chen`)
4. Replace the job title (e.g., `Senior Manager, Tech Innovation`)

**Tip:** There are 4 testimonials. Update each one individually.

---

### 8. Updating the "About Us" Section

**Location:** Near the bottom, before the final CTA

**Current Code:**
```html
<h2 class="text-4xl md:text-5xl lg:text-6xl font-bold tracking-tight mb-8">
    About <span class="text-[#FF5A5F]">Leadership Academy</span>
</h2>
<div class="space-y-6 text-lg leading-relaxed">
    <p class="text-gray-300">
        Founded in 2015, Leadership Academy emerged from...
    </p>
</div>
```

**How to Change It:**
1. Update the heading with your company name
2. Replace the company history paragraphs with your own story
3. Update the statistics in the right column (50K+, 150+, etc.)

---

### 9. Updating Footer Information

**Location:** At the very bottom of the page

**Current Code:**
```html
<p class="text-gray-400 text-sm">
    &copy; 2025 Leadership Academy. All rights reserved.
</p>
```

**How to Change It:**
1. Search for `2025 Leadership Academy`
2. Update the year and company name
3. Keep the `&copy;` (this displays the © symbol)

**Contact Email in Footer:**
```html
<a href="mailto:leaddershipacademy@leaddership.co.za" class="hover:text-[#FF5A5F] transition-colors duration-300">
    leaddershipacademy@leaddership.co.za
</a>
```

Replace with your email address.

---

## Modifying Colors & Styling

### Understanding the Color System

Your page uses three main colors:

| Color | Hex Code | Usage |
|-------|----------|-------|
| Coral Red | `#FF5A5F` | Accents, buttons, hover effects |
| Yellow | `#FFD166` | Secondary accents, alternative buttons |
| Dark Gray | `#1A1A1A` | Background |

### How to Change the Coral Red Color

**Step 1:** Find all instances of the color code
- Use your editor's Find & Replace (Ctrl+H or Cmd+H)
- Search for: `#FF5A5F`
- This will show you all 30+ places this color is used

**Step 2:** Choose your new color
- Use a color picker tool like [Coolors.co](https://coolors.co) or [Color-Hex.com](https://www.color-hex.com)
- Get your color's hex code (example: `#6366F1` for indigo)

**Step 3:** Replace carefully
- **Don't use "Replace All"** - this might cause issues
- Instead, replace colors in these specific areas:
  1. Buttons (`.btn-primary`)
  2. Text accents (`accent-coral`)
  3. Hover effects
  4. Borders and backgrounds

**Example - Changing Button Color:**

**Original:**
```html
.btn-primary {
    background-color: #FF5A5F;
    color: white;
}
```

**Changed to Indigo:**
```html
.btn-primary {
    background-color: #6366F1;
    color: white;
}
```

### How to Change the Yellow Color

**Step 1:** Use Find & Replace
- Search for: `#FFD166`

**Step 2:** Choose your new secondary color
- Example: `#F59E0B` (amber)

**Step 3:** Replace in the style section

**Example:**
```html
.btn-secondary {
    background-color: #F59E0B;  /* Changed from #FFD166 */
    color: #1A1A1A;
}
```

---

### Changing Background Colors

**Dark Background:**
- Search for: `bg-gray-900`
- This is used throughout the page

**Slightly Lighter Background:**
- Search for: `bg-gray-800`

**To change these:**
1. Find the Tailwind class you want to change
2. Replace it with a different shade:
   - `bg-gray-800` (lighter)
   - `bg-gray-950` (darker)
   - Or use a completely different color like `bg-blue-900`

---

### Changing Text Colors

**Gray Text (currently used for descriptions):**
- `text-gray-400` - lighter gray
- `text-gray-300` - medium gray
- `text-gray-400` - descriptions

**To change:**
1. Search for the text color class
2. Replace with your preferred color:
   - `text-blue-400`
   - `text-green-400`
   - `text-purple-400`

---

## Fixing & Managing Links

### Understanding Link Types

Your page has two types of links:

1. **Internal Links** - Links to other pages on your site (use `#section-name`)
2. **External Links** - Links to outside websites or services (use full URL)

---

### 1. Navigation Menu Links

**Location:** In the `<header>` section at the top

**Current Code:**
```html
<a href="#features" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Features</a>
<a href="#benefits" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Benefits</a>
<a href="#testimonials" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Testimonials</a>
<a href="#about" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">About</a>
```

**How These Work:**
- `href="#features"` means "scroll to the section with id='features'"
- The `#` symbol tells the browser this is an internal link
- The section must have a matching `id` attribute

**Checking if Links Work:**
1. Open your page in a browser
2. Click each navigation link
3. It should smoothly scroll to that section
4. If it doesn't, check that the section has the correct `id`

**Example - Adding a New Navigation Link:**

If you want to add a "Contact" link:

1. Find the navigation links in the header
2. Add this line:
```html
<a href="#contact" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Contact</a>
```

3. Verify the Contact section has `id="contact"` (it already does in your code)

---

### 2. Button Links (Call-to-Action)

**Location:** Throughout the page - buttons that say "Get Started", "Start Your Journey", etc.

**Current Code:**
```html
<a href="https://leaddership.co.za/shop" class="btn-primary">
    Get Started
</a>
```

**How to Change It:**
1. Search for `https://leaddership.co.za/shop`
2. Replace with your own URL
3. Keep the `class="btn-primary"` and button text

**Important:** This link appears in multiple places:
- Header navigation
- Hero section (2 buttons)
- CTA section (2 buttons)
- Final CTA section (1 button)

**Search Results:** You should find approximately 7 instances

**Example - Changing to Your Own Shop URL:**

**Original:**
```html
<a href="https://leaddership.co.za/shop" class="btn-primary">
    Start Your Journey
</a>
```

**Changed:**
```html
<a href="https://yourwebsite.com/courses" class="btn-primary">
    Start Your Journey
</a>
```

---

### 3. "Learn More" Button

**Location:** Hero section

**Current Code:**
```html
<button class="px-8 py-4 border-2 border-[#FFD166] text-[#FFD166] font-bold text-lg rounded-lg hover:bg-[#FFD166] hover:text-[#1A1A1A] transition-all duration-300 hover:scale-105">
    Learn More
</button>
```

**Issue:** This is currently a `<button>` element, not a link

**How to Fix It (Make it Functional):**

Replace the button with a link:
```html
<a href="#features" class="px-8 py-4 border-2 border-[#FFD166] text-[#FFD166] font-bold text-lg rounded-lg hover:bg-[#FFD166] hover:text-[#1A1A1A] transition-all duration-300 hover:scale-105 inline-block text-center">
    Learn More
</a>
```

**Changes Made:**
- Changed `<button>` to `<a>` tag
- Added `href="#features"` to link to features section
- Added `inline-block` and `text-center` to maintain styling

---

### 4. "Schedule Consultation" Button

**Location:** CTA section and Final CTA section

**Current Code:**
```html
<button class="px-8 py-4 border-2 border-[#FFD166] text-[#FFD166] font-bold text-lg rounded-lg hover:bg-[#FFD166] hover:text-[#1A1A1A] transition-all duration-300 hover:scale-105">
    Schedule Consultation
</button>
```

**How to Make It Functional:**

Option 1 - Link to Contact Form:
```html
<a href="#contact" class="px-8 py-4 border-2 border-[#FFD166] text-[#FFD166] font-bold text-lg rounded-lg hover:bg-[#FFD166] hover:text-[#1A1A1A] transition-all duration-300 hover:scale-105 inline-block text-center">
    Schedule Consultation
</a>
```

Option 2 - Link to External Scheduling Tool (like Calendly):
```html
<a href="https://calendly.com/your-username" class="px-8 py-4 border-2 border-[#FFD166] text-[#FFD166] font-bold text-lg rounded-lg hover:bg-[#FFD166] hover:text-[#1A1A1A] transition-all duration-300 hover:scale-105 inline-block text-center">
    Schedule Consultation
</a>
```

---

### 5. Footer Links

**Location:** At the bottom of the page in the `<footer>` section

**Quick Links Section:**
```html
<li><a href="#features" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Features</a></li>
<li><a href="#benefits" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Benefits</a></li>
<li><a href="#testimonials" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Testimonials</a></li>
<li><a href="#about" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">About Us</a></li>
```

**These are internal links** - they should work if the sections exist.

**Resources Section:**
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Terms of Service</a></li>
<li><a href="blog.html" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Blog</a></li>
<li><a href="https://leaddership.co.za/shop" class="text-gray-400 hover:text-[#FF5A5F] transition-colors duration-300">Shop</a></li>
```

**These links point to:**
- `privacy.html` - You need to create this file
- `terms.html` - You need to create this file
- `blog.html` - You need to create this file
- `https://leaddership.co.za/shop` - External link (update with your URL)

---

### 6. Social Media Links

**Location:** Footer, in the "Connect With Us" section

**Current Code:**
```html
<a href="#" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="Facebook">
    <i class="fab fa-facebook text-white"></i>
</a>
```

**How to Update:**
1. Search for `href="#"` in the social media section
2. Replace each `#` with your actual social media URL

**Example - Adding Real Social Links:**

```html
<!-- Facebook -->
<a href="https://facebook.com/yourpage" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="Facebook">
    <i class="fab fa-facebook text-white"></i>
</a>

<!-- Twitter -->
<a href="https://twitter.com/yourhandle" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="Twitter">
    <i class="fab fa-twitter text-white"></i>
</a>

<!-- LinkedIn -->
<a href="https://linkedin.com/company/yourcompany" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="LinkedIn">
    <i class="fab fa-linkedin text-white"></i>
</a>

<!-- Instagram -->
<a href="https://instagram.com/yourhandle" class="w-10 h-10 bg-gray-800 rounded-lg flex items-center justify-center hover:bg-[#FF5A5F] transition-colors duration-300" aria-label="Instagram">
    <i class="fab fa-instagram text-white"></i>
</a>
```

---

### 7. Email Link

**Location:** Footer contact information

**Current Code:**
```html
<a href="mailto:leaddershipacademy@leaddership.co.za" class="hover:text-[#FF5A5F] transition-colors duration-300">
    leaddershipacademy@leaddership.co.za
</a>
```

**How to Change It:**
1. Search for `mailto:leaddershipacademy@leaddership.co.za`
2. Replace the email address with your own

**Example:**
```html
<a href="mailto:info@yourcompany.com" class="hover:text-[#FF5A5F] transition-colors duration-300">
    info@yourcompany.com
</a>
```

---

### Checklist: All Links to Update

Use this checklist to ensure you've updated all necessary links:

- [ ] Shop/CTA button links (appears 7 times)
- [ ] "Learn More" button (make it functional)
- [ ] "Schedule Consultation" buttons (make them functional)
- [ ] Footer Quick Links (verify they work)
- [ ] Privacy Policy link
- [ ] Terms of Service link
- [ ] Blog link
- [ ] Shop link in footer
- [ ] Social media links
- [ ] Email contact link

---

## Adding Privacy & Terms Pages

### Why You Need These Pages

Privacy Policy and Terms of Service pages are legally important and help:
- Build trust with visitors
- Comply with regulations (GDPR, CCPA, etc.)
- Protect your business
- Explain how you use user data

### Step 1: Create the Privacy Policy Page

**Step 1a - Create a New File:**
1. Open your text editor
2. Create a new blank file
3. Save it as `privacy.html` in the same folder as your `index.html`

**Step 1b - Add the Basic HTML Structure:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - Leadership Academy">
    <title>Privacy Policy | Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation (Same as index.html) -->
    <header class="sticky top-0 z-50 bg-gray-800 border-b border-gray-700">
        <nav class="max-w-7xl mx-auto px-8 md:px-16 py-6 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <div class="w-10 h-10 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center">
                    <i class="fas fa-graduation-cap text-white text-lg"></i>
                </div>
                <span class="text-2xl font-bold tracking-tight">Leadership</span>
            </div>
            <a href="index.html" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Back to Home</a>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-32 px-8 md:px-16 bg-gray-900">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-5xl md:text-6xl font-bold tracking-tight mb-12">
                Privacy <span class="text-[#FF5A5F]">Policy</span>
            </h1>
            
            <div class="prose prose-invert max-w-none space-y-8">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">1. Introduction</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Leadership Academy ("we," "us," "our," or "Company") is committed to protecting your privacy. 
                        This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you 
                        visit our website.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">2. Information We Collect</h2>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        We may collect information about you in a variety of ways. The information we may collect on the 
                        Site includes:
                    </p>
                    <ul class="list-disc list-inside text-gray-300 space-y-2 ml-4">
                        <li>Personal Data: Name, email address, phone number, and other contact information</li>
                        <li>Usage Data: Browser type, IP address, pages visited, and time spent on pages</li>
                        <li>Cookies: Small files stored on your device to enhance your browsing experience</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">3. Use of Your Information</h2>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        Having accurate information about you permits us to provide you with a smooth, efficient, and 
                        customized experience. Specifically, we may use information collected about you via the Site to:
                    </p>
                    <ul class="list-disc list-inside text-gray-300 space-y-2 ml-4">
                        <li>Generate a personal profile about you so that future visits to the Site are personalized</li>
                        <li>Increase the efficiency and operation of the Site</li>
                        <li>Monitor and analyze usage and trends to improve your experience with the Site</li>
                        <li>Notify you of updates to the Site</li>
                        <li>Offer new products, services, and/or recommendations to you</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">4. Disclosure of Your Information</h2>
                    <p class="text-gray-300 leading-relaxed">
                        We may share information we have collected about you in certain situations:
                    </p>
                    <ul class="list-disc list-inside text-gray-300 space-y-2 ml-4">
                        <li><strong>By Law or to Protect Rights:</strong> If required by law or if we believe in good faith that disclosure is necessary</li>
                        <li><strong>Third-Party Service Providers:</strong> We may share your information with vendors, consultants, and service providers</li>
                        <li><strong>Business Transfers:</strong> If we are involved in a merger, acquisition, or asset sale</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">5. Security of Your Information</h2>
                    <p class="text-gray-300 leading-relaxed">
                        We use administrative, technical, and physical security measures to help protect your personal information. 
                        While we have taken reasonable steps to secure the personal information you provide to us, please be aware 
                        that no security measures are perfect or impenetrable.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">6. Contact Us</h2>
                    <p class="text-gray-300 leading-relaxed">
                        If you have questions or comments about this Privacy Policy, please contact us at:
                    </p>
                    <p class="text-gray-300 leading-relaxed mt-4">
                        Email: <a href="mailto:leaddershipacademy@leaddership.co.za" class="text-[#FF5A5F] hover:underline">leaddershipacademy@leaddership.co.za</a>
                    </p>
                </div>

                <div class="pt-8 border-t border-gray-700 mt-12">
                    <p class="text-gray-400 text-sm">
                        Last Updated: January 2025
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer (Same as index.html) -->
    <footer class="bg-black border-t border-gray-800 py-16 px-8 md:px-16">
        <div class="max-w-7xl mx-auto">
            <div class="text-center">
                <p class="text-gray-400">
                    &copy; 2025 Leadership Academy. All rights reserved.
                </p>
            </div>
        </div>
    </footer>
</body>
</html>
```

**Step 1c - Customize the Content:**
1. Replace the email address with your own
2. Update the company name if different
3. Add any specific information about your data collection practices
4. Update the "Last Updated" date

---

### Step 2: Create the Terms of Service Page

**Step 2a - Create a New File:**
1. Open your text editor
2. Create a new blank file
3. Save it as `terms.html` in the same folder as your `index.html`

**Step 2b - Add the Basic HTML Structure:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - Leadership Academy">
    <title>Terms of Service | Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <!-- Header Navigation -->
    <header class="sticky top-0 z-50 bg-gray-800 border-b border-gray-700">
        <nav class="max-w-7xl mx-auto px-8 md:px-16 py-6 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <div class="w-10 h-10 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center">
                    <i class="fas fa-graduation-cap text-white text-lg"></i>
                </div>
                <span class="text-2xl font-bold tracking-tight">Leadership</span>
            </div>
            <a href="index.html" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Back to Home</a>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-20 md:py-32 px-8 md:px-16 bg-gray-900">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-5xl md:text-6xl font-bold tracking-tight mb-12">
                Terms of <span class="text-[#FF5A5F]">Service</span>
            </h1>
            
            <div class="prose prose-invert max-w-none space-y-8">
                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">1. Agreement to Terms</h2>
                    <p class="text-gray-300 leading-relaxed">
                        By accessing and using this website, you accept and agree to be bound by the terms and provision 
                        of this agreement. If you do not agree to abide by the above, please do not use this service.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">2. Use License</h2>
                    <p class="text-gray-300 leading-relaxed mb-4">
                        Permission is granted to temporarily download one copy of the materials (information or software) 
                        on Leadership Academy's website for personal, non-commercial transitory viewing only. This is the 
                        grant of a license, not a transfer of title, and under this license you may not:
                    </p>
                    <ul class="list-disc list-inside text-gray-300 space-y-2 ml-4">
                        <li>Modifying or copying the materials</li>
                        <li>Using the materials for any commercial purpose or for any public display</li>
                        <li>Attempting to decompile or reverse engineer any software contained on the website</li>
                        <li>Transferring the materials to another person or "mirroring" the materials on any other server</li>
                        <li>Removing any copyright or other proprietary notations from the materials</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">3. Disclaimer</h2>
                    <p class="text-gray-300 leading-relaxed">
                        The materials on Leadership Academy's website are provided on an 'as is' basis. Leadership Academy 
                        makes no warranties, expressed or implied, and hereby disclaims and negates all other warranties 
                        including, without limitation, implied warranties or conditions of merchantability, fitness for a 
                        particular purpose, or non-infringement of intellectual property or other violation of rights.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">4. Limitations</h2>
                    <p class="text-gray-300 leading-relaxed">
                        In no event shall Leadership Academy or its suppliers be liable for any damages (including, without 
                        limitation, damages for loss of data or profit, or due to business interruption) arising out of the 
                        use or inability to use the materials on Leadership Academy's website, even if Leadership Academy or 
                        an authorized representative has been notified orally or in writing of the possibility of such damage.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">5. Accuracy of Materials</h2>
                    <p class="text-gray-300 leading-relaxed">
                        The materials appearing on Leadership Academy's website could include technical, typographical, or 
                        photographic errors. Leadership Academy does not warrant that any of the materials on its website are 
                        accurate, complete, or current. Leadership Academy may make changes to the materials contained on its 
                        website at any time without notice.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">6. Links</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Leadership Academy has not reviewed all of the sites linked to its website and is not responsible for 
                        the contents of any such linked site. The inclusion of any link does not imply endorsement by Leadership 
                        Academy of the site. Use of any such linked website is at the user's own risk.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">7. Modifications</h2>
                    <p class="text-gray-300 leading-relaxed">
                        Leadership Academy may revise these terms of service for its website at any time without notice. By 
                        using this website, you are agreeing to be bound by the then current version of these terms of service.
                    </p>
                </div>

                <div>
                    <h2 class="text-3xl font-bold mb-4 text-white">8. Governing Law</h2>
                    <p class="text-gray-300 leading-relaxed">
                        These terms and conditions are governed by and construed in accordance with the laws of the jurisdiction 
                        in which Leadership Academy operates, and you irrevocably submit to the exclusive jurisdiction of the 
                        courts in that location.
                    </p>
                </div>

                <div class="pt-8 border-t border-gray-700 mt-12">
                    <p class="text-gray-400 text-sm">
                        Last Updated: January 2025
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black border-t border-gray-800 py-16 px-8 md:px-16">
        <div class="max-w-7xl mx-auto">
            <div class="text-center">
                <p class="text-gray-400">
                    &copy; 2025 Leadership Academy. All rights reserved.
                </p>
            </div>
        </div>
    </footer>
</body>
</html>
```

**Step 2c - Customize the Content:**
1. Replace the email address with your own
2. Update the company name if different
3. Add any specific terms relevant to your business
4. Update the "Last Updated" date

---

### Step 3: Verify the Links Work

**Testing:**
1. Save both `privacy.html` and `terms.html` in the same folder as `index.html`
2. Open `index.html` in your web browser
3. Scroll to the footer
4. Click on "Privacy Policy" - it should open the privacy page
5. Click on "Terms of Service" - it should open the terms page
6. Click "Back to Home" on either page - it should return to the main page

**If Links Don't Work:**
- Verify file names are exactly: `privacy.html` and `terms.html` (lowercase, no spaces)
- Verify all three files are in the same folder
- Check that the links in `index.html` haven't been changed
- Clear your browser cache (Ctrl+Shift+Delete) and refresh

---

### Step 4: Update the Blog Link

**Creating a Blog Page:**

If you want a blog section, follow the same process:

1. Create `blog.html` in the same folder
2. Use similar HTML structure to privacy.html
3. Add blog post content

**Minimum Blog Page Template:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Blog - Leadership Academy">
    <title>Blog | Leadership Academy</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-gray-900 text-white">
    <header class="sticky top-0 z-50 bg-gray-800 border-b border-gray-700">
        <nav class="max-w-7xl mx-auto px-8 md:px-16 py-6 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <div class="w-10 h-10 bg-gradient-to-br from-[#FF5A5F] to-[#FFD166] rounded-lg flex items-center justify-center">
                    <i class="fas fa-graduation-cap text-white text-lg"></i>
                </div>
                <span class="text-2xl font-bold tracking-tight">Leadership</span>
            </div>
            <a href="index.html" class="text-gray-300 hover:text-[#FF5A5F] transition-colors duration-300 font-medium">Back to Home</a>
        </nav>
    </header>

    <section class="py-20 md:py-32 px-8 md:px-16 bg-gray-900">
        <div class="max-w-4xl mx-auto">
            <h1 class="text-5xl md:text-6xl font-bold tracking-tight mb-12">
                Our <span class="text-[#FF5A5F]">Blog</span>
            </h1>
            
            <div class="bg-gray-800 rounded-lg p-8 border border-gray-700">
                <h2 class="text-2xl font-bold mb-4">Coming Soon</h2>
                <p class="text-gray-300">
                    We're working on bringing you valuable content about professional development and leadership. 
                    Check back soon!
                </p>
            </div>
        </div>
    </section>

    <footer class="bg-black border-t border-gray-800 py-16 px-8 md:px-16">
        <div class="max-w-7xl mx-auto">
            <div class="text-center">
                <p class="text-gray-400">
                    &copy; 2025 Leadership Academy. All rights reserved.
                </p>
            </div>
        </div>
    </footer>
</body>
</html>
```

---

## Mobile Responsiveness Tips

Your page uses **Tailwind CSS** for responsive design. Understanding these classes will help you maintain mobile compatibility.

### Understanding Responsive Classes

Tailwind uses prefixes to target different screen sizes:

| Prefix | Screen Size | Example |
|--------|------------|---------|
| (none) | Mobile (all screens) | `text-lg` |
| `sm:` | 640px and up | `sm:text-xl` |
| `md:` | 768px and up | `md:text-2xl` |
| `lg:` | 1024px and up | `lg:text-3xl` |
| `xl:` | 1280px and up | `xl:text-4xl` |

### Examples in Your Code

**Example 1 - Text Size:**
```html
<h1 class="text-5xl md:text-6xl lg:text-7xl font-bold">
    Professional Development
</h1>
```

**Means:**
- On mobile: 3rem (text-5xl)
- On tablets (768px+): 3.75rem (text-6xl)
- On desktops (1024px+): 4.5rem (text-7xl)

**Example 2 - Layout:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12">
    <!-- Content -->
</div>
```

**Means:**
- On mobile: 1 column
- On tablets: 2 columns
- On desktops: 3 columns

**Example 3 - Visibility:**
```html
<div class="hidden lg:block">
    <!-- This only shows on desktop -->
</div>
```

### Testing Mobile Responsiveness

**In Your Browser:**
1. Open your page
2. Press F12 (or right-click → Inspect)
3. Click the device icon (top-left of developer tools)
4. Select different devices to test:
   - iPhone 12
   - iPad
   - Desktop

**Common Mobile Issues to Check:**
- [ ] Text is readable (not too small)
- [ ] Buttons are easily clickable (at least 44px tall)
- [ ] Images scale properly
- [ ] Navigation menu works on mobile
- [ ] Forms are easy to fill on mobile
- [ ] No horizontal scrolling needed

### Making Custom Elements Responsive

**If you add new content, use these patterns:**

**For Text:**
```html
<p class="text-base md:text-lg lg:text-xl">
    Your text here
</p>
```

**For Spacing (padding/margin):**
```html
<div class="p-4 md:p-8 lg:p-16">
    <!-- p-4 on mobile, p-8 on tablet, p-16 on desktop -->
</div>
```

**For Grid Layouts:**
```html
<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-4 md:gap-8">
    <!-- 1 column on mobile, 2 on tablet, 4 on desktop -->
</div>
```

---

## Troubleshooting Common Issues

### Issue 1: Links Don't Work

**Problem:** Clicking a link doesn't navigate anywhere

**Solutions:**

1. **Internal Links (with #):**
   - Check the `href` matches an `id` on the page
   - Example: `href="#features"` must match `id="features"`
   - Make sure there are no typos

2. **External Links:**
   - Verify the URL starts with `http://` or `https://`
   - Test the URL in your browser to ensure it works
   - Check for typos in the domain name

3. **File Links (privacy.html, terms.html):**
   - Ensure files are in the same folder as index.html
   - File names must match exactly (case-sensitive on some servers)
   - Use lowercase file names

**Testing:**
```html
<!-- Before (might not work): -->
<a href="leaddership.co.za/shop">Shop</a>

<!-- After (should work): -->
<a href="https://leaddership.co.za/shop">Shop</a>
```

---

### Issue 2: Colors Don't Change

**Problem:** You tried to change a color but it didn't work

**Solutions:**

1. **Save the file:**
   - After making changes, save the file (Ctrl+S)
   - The changes won't appear until saved

2. **Clear browser cache:**
   - Press Ctrl+Shift+Delete (Windows) or Cmd+Shift+Delete (Mac)
   - Select "Cached images and files"
   - Click "Clear"
   - Refresh the page (F5 or Cmd+R)

3. **Check for typos:**
   - Hex codes must start with `#`
   - Example: `#FF5A5F` (not `FF5A5F`)
   - Color names in Tailwind must be exact: `bg-gray-900` (not `bg-gray900`)

4. **Verify you're editing the right place:**
   - Search for the color code in the `<style>` section
   - Search in the HTML for inline styles
   - Both places might need updating

---

### Issue 3: Mobile Menu Not Working

**Problem:** The hamburger menu doesn't open on mobile

**Solutions:**

1. **Check JavaScript is enabled:**
   - Your browser must have JavaScript enabled
   - Most browsers have it enabled by default

2. **Verify the menu HTML:**
   - Look for `<button class="md:hidden mobile-menu-button">`
   - Look for `<div class="mobile-menu hidden">`
   - Both must be present

3. **Test in different browser:**
   - Try Chrome, Firefox, or Safari
   - If it works in one but not another, it might be a browser issue

4. **Check console for errors:**
   - Press F12 to open developer tools
   - Click "Console" tab
   - Look for red error messages
   - Take a screenshot and share if you need help

---

### Issue 4: Text Overflows or Looks Wrong

**Problem:** Text appears cut off or overlaps other content

**Solutions:**

1. **Check responsive classes:**
   - Ensure you have `md:` and `lg:` prefixes for different screen sizes
   - Example: `text-sm md:text-base lg:text-lg`

2. **Verify padding/margin:**
   - Check that container has enough padding: `px-8 md:px-16`
   - Check that text has max-width: `max-w-2xl`

3. **Test on actual devices:**
   - Use browser developer tools to test different sizes
   - Test on actual phone if possible

4. **Check line length:**
   - Long lines of text should have `max-w-` class
   - Example: `max-w-2xl` (keeps text readable)

---

### Issue 5: Images Not Loading

**Problem:** Images show as broken or missing

**Solutions:**

1. **Check image URLs:**
   - Verify URLs start with `http://` or `https://`
   - Test the URL directly in browser
   - Example: `https://images.unsplash.com/photo-1552664730-d307ca884978?w=1200`

2. **For local images:**
   - Place images in same folder as HTML files
   - Use relative paths: `<img src="image.jpg">`
   - Not absolute paths: `<img src="/images/image.jpg">`

3. **Check file format:**
   - Supported formats: JPG, PNG, GIF, WebP
   - File names are case-sensitive on some servers

---

### Issue 6: Forms Not Submitting

**Problem:** Contact form doesn't send messages

**Solutions:**

1. **Verify Web3Forms access key:**
   - Check that `access_key` value is present:
   ```html
   <input type="hidden" name="access_key" value="3bb39263-2490-491b-89f8-213fa513edae">
   ```

2. **Check email configuration:**
   - Visit [Web3Forms.com](https://web3forms.com)
   - Sign up and get your access key
   - Replace the access key in the form

3. **Test form submission:**
   - Fill out the form with test data
   - Click submit
   - Check your email for the message
   - Check spam/junk folder if not in inbox

4. **Check console for errors:**
   - Press F12 to open developer tools
   - Click "Console"
   - Look for error messages when submitting

---

### Issue 7: Styling Looks Different in Different Browsers

**Problem:** Page looks good in Chrome but different in Firefox/Safari

**Solutions:**

1. **Use standard CSS:**
   - Avoid browser-specific prefixes when possible
   - Tailwind handles this automatically

2. **Test in multiple browsers:**
   - Chrome
   - Firefox
   - Safari
   - Edge

3. **Check for browser extensions:**
   - Disable extensions that might affect styling
   - Try in private/incognito mode

4. **Clear cache in each browser:**
   - Each browser has its own cache
   - Clear cache before testing changes

---

### Issue 8: Changes Not Appearing

**Problem:** You made changes but they don't show up

**Solutions:**

1. **Save the file:**
   - Use Ctrl+S (Windows) or Cmd+S (Mac)
   - Look for indicator that file is saved (no asterisk in title)

2. **Refresh the browser:**
   - Press F5 (Windows) or Cmd+R (Mac)
   - Or press Ctrl+Shift+R for hard refresh

3. **Clear cache:**
   - Ctrl+Shift+Delete (Windows) or Cmd+Shift+Delete (Mac)
   - Select "Cached images and files"
   - Click "Clear"

4. **Close and reopen file:**
   - Close the HTML file in your text editor
   - Open it again
   - Make sure you're editing the right file

5. **Check file location:**
   - Verify you're editing the file in the correct folder
   - Not a copy or backup file

---

### Issue 9: Buttons Don't Look Right

**Problem:** Button colors or styling is incorrect

**Solutions:**

1. **Check button class:**
   - Primary buttons: `class="btn-primary"`
   - Secondary buttons: `class="btn-secondary"`
   - Custom buttons: check all classes are present

2. **Verify button HTML:**
   - Buttons should be `<a>` or `<button>` tags
   - Links should use `<a>` tags with `href`
   - Buttons should use `<button>` tags

3. **Check Tailwind classes:**
   - All classes must be spelled exactly
   - Use hyphens not underscores: `text-gray-300` not `text_gray_300`
   - No spaces in class names

---

### Issue 10: Mobile Navigation Doesn't Close

**Problem:** Mobile menu stays open after clicking a link

**Solutions:**

1. **Check JavaScript is working:**
   - Press F12 to open developer tools
   - Click "Console"
   - No red errors should appear

2. **Verify mobile menu HTML:**
   - Look for: `<div class="mobile-menu hidden">`
   - The `hidden` class should be there
   - JavaScript adds/removes this class

3. **Test in different browser:**
   - Try different browser to isolate the issue

---

## Quick Reference: Common Tasks

### Changing Your Shop URL

**Find:**
```
https://leaddership.co.za/shop
```

**Replace with your URL:**
```
https://yourwebsite.com/courses
```

**Appears in:** Header, Hero section (2x), CTA section (2x), Final CTA, Footer (1x)

---

### Changing Your Email

**Find:**
```
leaddershipacademy@leaddership.co.za
```

**Replace with:**
```
your-email@yourcompany.com
```

**Appears in:** Footer contact info, Privacy policy page, Terms page

---

### Changing Company Name

**Find:**
```
Leadership Academy
```

**Replace with:**
```
Your Company Name
```

**Appears in:** Header, Footer, All policy pages, Meta tags

---

### Changing Primary Color (Coral Red)

**Find:**
```
#FF5A5F
```

**Replace with:**
```
#YourColorCode
```

**Appears in:** 30+ places throughout the site

---

### Changing Secondary Color (Yellow)

**Find:**
```
#FFD166
```

**Replace with:**
```
#YourColorCode
```

**Appears in:** 20+ places throughout the site

---

## Getting Help

### Resources for Learning

- **Tailwind CSS Documentation:** [tailwindcss.com/docs](https://tailwindcss.com/docs)
- **HTML Reference:** [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/HTML)
- **Color Picker:** [Coolors.co](https://coolors.co)
- **Responsive Testing:** Built into all modern browsers (F12)

### Common Questions

**Q: Can I use this on multiple websites?**
A: Yes, you can use this template for multiple projects. Just save copies with different names.

**Q: How do I add more features/sections?**
A: Copy an existing section, change the ID and content, add a navigation link to it.

**Q: Can I change fonts?**
A: Yes, modify the `<link href="https://fonts.googleapis.com/...">` line to use different Google Fonts.

**Q: How do I add animations?**
A: Tailwind has built-in animation classes. Add classes like `animate-bounce` or `animate-pulse` to elements.

**Q: Is this SEO-friendly?**
A: Yes! It includes meta tags, semantic HTML, and proper heading structure. Update meta descriptions for better SEO.

---

## Maintenance Checklist

Use this checklist monthly to keep your site in good shape:

- [ ] **Update Links:** Verify all links work (especially external ones)
- [ ] **Check Forms:** Test contact form and ensure emails arrive
- [ ] **Mobile Test:** Check site on actual mobile device
- [ ] **Browser Test:** Test in Chrome, Firefox, Safari
- [ ] **Update Content:** Refresh testimonials, statistics, or offers
- [ ] **Check Performance:** Use Google PageSpeed Insights
- [ ] **Backup Files:** Save copies of all files
- [ ] **Update Copyright Year:** Change year in footer if needed
- [ ] **Monitor Analytics:** Check which pages get most traffic
- [ ] **Test Contact Form:** Send test message to verify it works

---

## Summary

You now have a complete guide for maintaining and customizing your Leadership Academy landing page. Here's what you learned:

✅ **Text Updates:** How to find and change any text on the page
✅ **Colors:** How to customize the color scheme
✅ **Links:** How to update all navigation and CTA links
✅ **Policy Pages:** How to create and link privacy and terms pages
✅ **Mobile:** How responsive design works and how to test it
✅ **Troubleshooting:** Solutions to common problems
✅ **Reference:** Quick lookup for common tasks

**Next Steps:**
1. Make a backup copy of your files
2. Start with small changes (text, links)
3. Test thoroughly before publishing
4. Use the troubleshooting guide if issues arise
5. Refer back to this guide as needed

Good luck with your website! 🚀