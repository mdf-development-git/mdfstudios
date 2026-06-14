# MDF Studios - Professional Gaming Studio Website

## 🎮 Overview

A modern, professional website for MDF Studios featuring stunning animations, gallery management, and secure integration with Patreon for modpack downloads.

## ✨ Features Included

### Visual & Animation
- **GTA 6 Style Splash Screen**: Stunning intro animation with glitch effects
- **Logo Animation**: Glowing neon effect with dynamic text-shadow
- **Smooth Scroll Navigation**: Sticky navbar with smooth transitions
- **Responsive Design**: Works on all devices (mobile, tablet, desktop)
- **Modern Dark Theme**: Sleek black and neon green color scheme

### Gallery Management
- **Bidirectional Image Scroll**: Two rows of screenshots scrolling in opposite directions
- **Infinite Scroll Effect**: Seamless looping gallery
- **Hover Effects**: Interactive image overlays with titles
- **Easy Image Integration**: Simple functions to add/manage screenshots
- **Placeholder Support**: Pre-configured with placeholder images

### Modpack Distribution
- **Patreon Integration**: Direct links for downloads
- **Feature Showcase**: Highlight key modpack features
- **Version Tracking**: Display current version and update dates

### Security
- **XSS Protection**: Input sanitization on contact forms
- **No External Dependencies**: Uses vanilla JavaScript
- **HTTPS Ready**: Can be deployed with SSL certificates

## 🚀 Quick Start

### 1. Update Patreon Link
Edit `index.html` and find this line:
```html
<a href="https://www.patreon.com" target="_blank">
```
Replace with your actual Patreon link.

### 2. Add Screenshots
Use the `addScreenshot()` function in your browser console:
```javascript
addScreenshot('https://your-image-url.jpg', 'Screenshot Title');
```

Or edit the gallery images in the script section:
```javascript
const galleryImages = [
    { url: 'your-image-url.jpg', title: 'Your Title' },
    // ... more images
];
```

### 3. Customize Colors
Edit these CSS variables at the top of the `<style>` tag:
```css
:root {
    --primary-color: #00ff00;      /* Main accent color */
    --secondary-color: #1a1a1a;    /* Dark background */
    --accent-color: #ff6600;       /* Secondary accent */
    --text-color: #ffffff;         /* Text color */
}
```

### 4. Update Social Links
Find the contact section and update:
```html
<a href="https://discord.gg/YOUR_SERVER" class="social-icon">Discord</a>
<a href="https://twitter.com/YOUR_HANDLE" class="social-icon">Twitter</a>
<a href="https://youtube.com/@YOUR_CHANNEL" class="social-icon">YouTube</a>
```

## 📁 File Structure

```
index.html          # Complete HTML file with embedded CSS and JavaScript
README.md          # This file
```

## 🌐 Deployment

### GitHub Pages
1. Go to repository Settings → Pages
2. Select `main` branch as source
3. Your site will be live at `https://mdf-development-git.github.io/mdfstudios`

### Custom Domain
1. Add CNAME file with your domain
2. Configure DNS with your domain provider
3. Enable HTTPS in GitHub Pages settings

### Traditional Hosting
1. Upload `index.html` to your web server
2. Ensure HTTPS is enabled
3. Set proper file permissions

## 🎨 Customization

### Change Primary Color
```css
--primary-color: #00ff00;  /* Change this value */
```

### Modify Splash Screen Duration
Find this line in the script:
```javascript
setTimeout(() => {
    splashScreen.classList.add('hidden');
}, 3500);  // Change 3500 (milliseconds)
```

### Update Stats
Find the About section and change:
```html
<h3>50+</h3>      <!-- Change number -->
<p>Curated Mods</p>  <!-- Change label -->
```

## 🔐 Security

The website includes:
- ✅ XSS Protection via input sanitization
- ✅ Secure external links with `noopener` attributes
- ✅ No sensitive data storage
- ✅ HTTPS ready
- ✅ No external JavaScript dependencies

## 📱 Browser Support

- ✅ Chrome/Edge (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Mobile browsers
- ⚠️ IE11 (not recommended)

## 🛠️ API Functions Available

### Add Screenshot Programmatically
```javascript
addScreenshot('image-url.jpg', 'Screenshot Title');
```

### Show Notification
```javascript
showNotification('Your message here', 'success');  // or 'info'
```

### Sanitize Input
```javascript
const clean = sanitizeInput(userInput);
```

## 📊 Future Enhancements (Optional)

### Recommended
- [ ] Admin dashboard for managing content
- [ ] Backend database for screenshots
- [ ] Email notifications
- [ ] Download statistics tracking
- [ ] User authentication

### Not Recommended
- User comments system (moderation burden)
- Real-time chat (use Discord instead)
- Complex e-commerce (use Patreon)
- Community forum (use Discord)

## 🐛 Troubleshooting

### Splash Screen Not Showing
- Check if JavaScript is enabled
- Open browser console (F12) for errors
- Verify CSS is loading

### Gallery Not Scrolling
- Check if images are loading properly
- Verify animation CSS is applied
- Check for JavaScript errors in console

### Form Not Working
- Open browser console and submit form
- Check for JavaScript errors
- Note: Form needs backend integration to actually send emails

## 📞 Support

For issues:
1. Check browser console for errors (Press F12)
2. Review the code comments in the HTML file
3. Verify all URLs are correct and accessible
4. Contact MDF Studios support

## 📝 Notes

- The entire website is contained in one HTML file for simplicity
- CSS is embedded in the `<style>` tag
- JavaScript is embedded in the `<script>` tag
- All animations are GPU-accelerated for smooth performance
- The gallery uses placeholder images - replace with your actual screenshots

---

**Built with ❤️ for the gaming community**

Copyright © 2026 MDF Studios. All rights reserved.