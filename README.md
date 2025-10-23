# Kushal Mungee - Personal Website

A beautiful, modern, and responsive personal portfolio website built with HTML, CSS, and JavaScript.

## 🌟 Features

- **Modern Design**: Clean, aesthetic interface with beautiful gradients and smooth animations
- **Fully Responsive**: Optimized for mobile, tablet, and desktop devices
- **Smooth Animations**: Scroll-triggered animations using AOS (Animate On Scroll) library
- **Interactive Navigation**: Mobile-friendly hamburger menu with smooth transitions
- **Dark Mode**: Professional dark theme for reduced eye strain
- **Sections Included**:
  - Hero section with call-to-action buttons
  - About/Academic background
  - Timeline-based experience section
  - Interests and hobbies showcase
  - Contact section with social media links
  - Responsive footer

## 📁 Project Structure

```
Personal Website/
├── index.html      # Main HTML file
├── style.css       # Complete styling and animations
├── script.js       # JavaScript for interactivity
└── README.md       # This file
```

## 🚀 Quick Start

1. **Clone or download the repository**
   ```bash
   git clone https://github.com/kushal613/Personal-Website.git
   ```

2. **Open in browser**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     python -m http.server 8000
     # or
     python3 -m http.server 8000
     ```

3. **Access the website**
   - Local: `http://localhost:8000`
   - Or open the file directly: `file:///path/to/index.html`

## 🎨 Customization Guide

### Update Personal Information

#### 1. Hero Section
Edit `index.html` to update your name and tagline:
```html
<h1 class="hero-title">
    Hi, I'm <span class="highlight">Your Name</span>
</h1>
<p class="hero-subtitle">Your Professional Tagline</p>
```

#### 2. About Section
Update the about section content:
```html
<div class="about-text">
    <p>Your about text here...</p>
</div>
```

#### 3. Experience Timeline
Edit experience entries:
```html
<div class="timeline-item">
    <div class="timeline-content">
        <h3>Your Job Title</h3>
        <p class="timeline-date">Year - Present</p>
        <p>Your job description...</p>
    </div>
</div>
```

#### 4. Interests & Hobbies
Update your interests:
```html
<div class="interest-card">
    <i class="fas fa-YOUR-ICON"></i>
    <h3>Your Interest</h3>
    <p>Description of your interest...</p>
</div>
```

#### 5. Contact Section
Update your contact links:
```html
<a href="https://twitter.com/YOUR-HANDLE" target="_blank" class="social-link">
    <i class="fab fa-x-twitter"></i>
    <span>Twitter / X</span>
</a>
```

Replace placeholders with:
- Your Twitter/X handle
- Your GitHub username (already set to kushal613)
- Your LinkedIn profile URL
- Your email address

### Color Customization

Edit the CSS variables in `style.css`:
```css
:root {
    --primary: #6366f1;      /* Main brand color */
    --secondary: #ec4899;    /* Accent color */
    --accent: #8b5cf6;       /* Secondary accent */
    --bg: #0f172a;           /* Background */
    --text: #f1f5f9;         /* Text color */
}
```

### Font Customization

Modify the font family in `style.css`:
```css
body {
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
}
```

## 🌐 Deployment

### Option 1: GitHub Pages
1. Push code to your GitHub repository
2. Go to Settings → Pages
3. Select `main` branch as source
4. Your site will be live at `https://kushal613.github.io/Personal-Website/`

### Option 2: GoDaddy (Your Domain - kushalmungee.com)
1. Log in to GoDaddy
2. Go to Hosting
3. Upload the files via FTP or File Manager:
   - `index.html`
   - `style.css`
   - `script.js`
4. Set `index.html` as your default file
5. Your site will be live at `https://kushalmungee.com`

### Option 3: Vercel, Netlify, or Other Hosting
These platforms offer free hosting with automatic deployments from GitHub:
- **Vercel**: Connect your GitHub repo for automatic deployments
- **Netlify**: Drag and drop your files or connect GitHub
- Both support custom domains

## 🔧 Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with gradients, animations, and flexbox/grid
- **JavaScript (ES6+)**: Interactive features
- **Font Awesome**: Icon library (CDN)
- **AOS (Animate On Scroll)**: Scroll animations library (CDN)

## 📝 Features in Detail

### Navigation
- Fixed navigation bar with smooth scrolling
- Mobile hamburger menu
- Active link indicator
- Backdrop blur effect

### Hero Section
- Full-screen height with gradient background
- Animated gradient shift
- Call-to-action buttons with hover effects
- Parallax scrolling effect

### About Section
- Responsive grid layout
- Three feature cards with icons
- Hover animations

### Experience Timeline
- Alternating timeline layout
- Animated markers
- Skill tags for technologies
- Responsive single-column on mobile

### Interests Section
- Card-based grid layout
- Icon-based visual hierarchy
- Zoom-in animations on scroll

### Contact Section
- Social media link cards
- Direct email link
- Hover lift effect

## ⚡ Performance

- Lightweight: No heavy frameworks, pure HTML/CSS/JS
- Fast loading: Minimal dependencies
- Optimized animations: GPU-accelerated where possible
- Mobile optimized: Responsive and touch-friendly

## 🤝 Contributing

Feel free to fork this repository and customize it for your own use!

## 📄 License

This project is open source and available under the MIT License.

## 📞 Support

For questions or suggestions, feel free to:
- Email: your-email@example.com
- GitHub: @kushal613
- Twitter/X: @your-handle

---

**Built with ❤️ and modern web technologies**

Last updated: October 2025
