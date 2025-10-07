================================================================================
                         IDLE MASTER WEBSITE
                    Professional Multi-Page Website
================================================================================

ABOUT THIS PROJECT
------------------
This is a modern, responsive, multi-page website for Idle Master - a Steam 
trading card farming automation tool. The website features clean design, 
smooth animations, and mobile-responsive layout.

FILES INCLUDED
--------------
- index.html       : Home page with hero section, features, and CTAs
- about.html       : About page with mission, vision, and values
- contact.html     : Contact page with Google Form integration
- download.html    : Download page with installation guide
- style.css        : All styling and responsive design
- script.js        : JavaScript for interactivity and animations
- README.txt       : This file with setup instructions


================================================================================
                        HOW TO RUN THE WEBSITE
================================================================================

OPTION 1: Open Directly in Browser
-----------------------------------
1. Navigate to the folder containing the website files
2. Double-click on "index.html" to open it in your default browser
3. The website should load and function properly

OPTION 2: Using a Local Server (Recommended)
---------------------------------------------
For better performance and to avoid any CORS issues:

Using Python (if installed):
- Python 3.x: python -m http.server 8000
- Python 2.x: python -m SimpleHTTPServer 8000
Then open: http://localhost:8000

Using Node.js (if installed):
- Install: npm install -g http-server
- Run: http-server
Then open: http://localhost:8080

Using VS Code:
- Install "Live Server" extension
- Right-click on index.html and select "Open with Live Server"


================================================================================
                      CUSTOMIZATION GUIDE
================================================================================

CHANGING COLORS
---------------
Open style.css and modify the CSS variables at the top:

:root {
    --primary-color: #EFEFEF;      /* Light gray background */
    --secondary-color: #FFFFFF;    /* White */
    --accent-color: #D10000;       /* Red accent color */
    --text-dark: #1a1a1a;         /* Dark text */
    --text-gray: #666666;         /* Gray text */
    --text-light: #999999;        /* Light gray text */
}

Save the file and refresh your browser to see changes.


UPDATING LINKS
--------------
1. Google Form Link (Contact Page):
   - Open: contact.html
   - Find: href="https://docs.google.com/forms/d/e/1FAIpQLSf..."
   - Replace with your Google Form URL
   - Line ~56 approximately

2. GitHub Repository Link:
   - Search for: "https://github.com/subtitle-edit/Idle-Master"
   - Replace in all HTML files (index.html, about.html, contact.html, download.html)
   - Update both navigation and footer links

3. Official Website Link:
   - Search for: "https://idlemaster.net/"
   - Replace with your actual website URL in all pages

4. Download Link:
   - Open: download.html
   - Find: href="https://idlemaster.net/download/"
   - Replace with your download URL
   - Line ~111 approximately


CHANGING TEXT CONTENT
----------------------
All text content is directly in the HTML files. To change:

1. Open the relevant HTML file (index.html, about.html, etc.)
2. Find the text you want to change
3. Edit it directly in the HTML
4. Save and refresh your browser

Key sections to customize:
- Hero titles and descriptions
- Feature descriptions
- About page mission and vision
- Contact page introduction
- Download page instructions
- Footer information


MODIFYING KEYWORDS & SEO
-------------------------
1. Update page titles:
   - Find: <title>Page Title</title>
   - Change to your desired title

2. Update meta descriptions:
   - Find: <meta name="description" content="...">
   - Change the content attribute

3. Update keyword links:
   - The "idle master" keyword is linked in index.html
   - Find: class="keyword-link"
   - Modify the link text and URL as needed


CHANGING FONTS
--------------
Current font: Poppins (loaded from Google Fonts)

To change:
1. Visit https://fonts.google.com/
2. Select your desired font
3. Copy the new <link> tag
4. Replace the existing font link in the <head> section of all HTML files
5. In style.css, change: font-family: 'Poppins', ...
   to: font-family: 'YourNewFont', ...


ADDING SOCIAL MEDIA LINKS
--------------------------
Footer social links are in each HTML file:

1. Find: <div class="social-links">
2. Add new social link using this template:

<a href="YOUR_SOCIAL_URL" target="_blank" rel="noopener" aria-label="Social Platform">
    <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
        <!-- SVG icon code here -->
    </svg>
</a>

Get free SVG icons from: https://heroicons.com/ or https://feathericons.com/


MODIFYING NAVIGATION
--------------------
To add/remove navigation items:

1. Open any HTML file
2. Find: <ul class="nav-menu">
3. Add or remove <li> items following the existing pattern
4. Update the same in all HTML files to maintain consistency


RESPONSIVE BREAKPOINTS
-----------------------
The website is responsive with these breakpoints:
- Desktop: 1025px and above
- Tablet: 769px to 1024px
- Mobile: 768px and below
- Small mobile: 480px and below

To adjust, modify the @media queries in style.css


================================================================================
                      ADVANCED CUSTOMIZATION
================================================================================

ADDING NEW PAGES
----------------
1. Duplicate an existing HTML file (e.g., about.html)
2. Rename it to your new page name (e.g., blog.html)
3. Update the page title and content
4. Add a link to it in the navigation of all pages
5. Ensure the navigation and footer are consistent

ADDING ANIMATIONS
-----------------
JavaScript animations are in script.js. Current animations include:
- Scroll-triggered fade-ins
- Hover effects
- Mobile menu animations
- Parallax effects on hero section

To add more animations, use the IntersectionObserver pattern in script.js

PERFORMANCE OPTIMIZATION
------------------------
The website is already optimized with:
- Minimal CSS and JavaScript
- Smooth scroll behavior
- Lazy loading support (for future images)
- Debounced scroll events
- CSS transitions instead of JavaScript animations

BROWSER SUPPORT
---------------
Compatible with:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)


================================================================================
                      DEPLOYMENT INSTRUCTIONS
================================================================================

DEPLOYING TO WEB HOSTING
-------------------------
1. Upload all files to your web host via FTP or hosting control panel
2. Ensure index.html is in the root directory
3. All other files (CSS, JS, HTML) should be in the same directory
4. Test all links and functionality after deployment

RECOMMENDED HOSTING OPTIONS
----------------------------
- GitHub Pages (Free): https://pages.github.com/
- Netlify (Free): https://www.netlify.com/
- Vercel (Free): https://vercel.com/
- Traditional hosting: Any shared hosting service

DEPLOYING TO GITHUB PAGES
--------------------------
1. Create a new repository on GitHub
2. Upload all website files
3. Go to Settings > Pages
4. Select main branch as source
5. Your site will be live at: username.github.io/repository-name


================================================================================
                      TROUBLESHOOTING
================================================================================

Website Not Loading Properly
-----------------------------
- Check that all files are in the same directory
- Ensure file names match exactly (case-sensitive on some servers)
- Clear browser cache (Ctrl+F5 or Cmd+Shift+R)

Links Not Working
-----------------
- Verify URLs are correct and properly formatted
- Check for typos in href attributes
- Ensure external links include https://

Styling Issues
--------------
- Verify style.css is in the same folder as HTML files
- Check browser console for any errors (F12)
- Ensure CSS file link in HTML is correct

Mobile Menu Not Working
------------------------
- Verify script.js is properly linked
- Check browser console for JavaScript errors
- Ensure JavaScript is enabled in browser


================================================================================
                      SUPPORT & RESOURCES
================================================================================

For questions or issues with customization:
1. Check browser console for errors (Press F12)
2. Validate HTML: https://validator.w3.org/
3. Validate CSS: https://jigsaw.w3.org/css-validator/

Learning Resources:
- HTML/CSS Basics: https://www.w3schools.com/
- JavaScript: https://javascript.info/
- Responsive Design: https://web.dev/responsive-web-design-basics/


================================================================================
                      VERSION INFORMATION
================================================================================

Version: 1.0
Created: 2025
Design: Modern, Clean, Professional
Color Palette: #EFEFEF, #FFFFFF, #D10000
Framework: Vanilla HTML/CSS/JavaScript (No dependencies)
License: Customizable for personal or commercial use


================================================================================
                      CREDITS & ACKNOWLEDGMENTS
================================================================================

Design Inspiration: idlemaster.net
Font: Poppins (Google Fonts)
Icons: SVG inline icons
Developed with ❤️ for the Idle Master community


================================================================================
                      THANK YOU FOR USING THIS WEBSITE!
================================================================================

For more information about Idle Master:
Official Website: https://idlemaster.net/
GitHub Repository: https://github.com/subtitle-edit/Idle-Master

Enjoy your new website!
