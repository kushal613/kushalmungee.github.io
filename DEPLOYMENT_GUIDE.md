# Deployment Guide for kushalmungee.com

Complete guide to deploy your personal website to your GoDaddy domain.

## 🌐 Option 1: GoDaddy (Recommended for Your Domain)

### Prerequisites
- GoDaddy account with kushalmungee.com domain
- FTP client (FileZilla is free: https://filezilla-project.org/)
- Or use GoDaddy's File Manager

### Method 1A: Using GoDaddy File Manager (Easiest)

1. **Log into GoDaddy**
   - Go to https://www.godaddy.com
   - Click your profile icon → "Manage My Products"
   - Find your hosting account

2. **Access File Manager**
   - Click "Hosting" → "Manage"
   - In the left sidebar, click "File Manager"
   - Navigate to the `public_html` folder

3. **Upload Your Files**
   - Upload these files to `public_html`:
     - `index.html`
     - `style.css`
     - `script.js`
   - Create a folder named `assets` if you add images later

4. **Set Default File** (if needed)
   - Right-click `index.html`
   - Set as "Default File" or "Index File"

5. **Access Your Website**
   - Open https://kushalmungee.com in your browser
   - Your site should load immediately!

### Method 1B: Using FTP (More Control)

1. **Get FTP Credentials**
   - Log into GoDaddy
   - Go to Hosting → Manage
   - Under "FTP Details", note your:
     - Server/Host: `ftp.kushalmungee.com` (or similar)
     - Username
     - Password

2. **Install FileZilla**
   - Download from: https://filezilla-project.org/download.php
   - Install and open

3. **Connect to Your Server**
   - File → Site Manager
   - Click "New Site"
   - Protocol: FTP
   - Host: `ftp.kushalmungee.com`
   - Username: (from GoDaddy)
   - Password: (from GoDaddy)
   - Click "Connect"

4. **Upload Files**
   - Local Files (left): Navigate to your website folder
   - Remote Files (right): Navigate to `public_html`
   - Drag and drop or right-click → Upload:
     - `index.html`
     - `style.css`
     - `script.js`

5. **Verify Upload**
   - Open https://kushalmungee.com
   - Your website should be live!

## 🚀 Option 2: GitHub Pages + Custom Domain

### Step 1: Push Code to GitHub

```bash
cd /Users/kushalmungee/Desktop/Personal\ Website
git remote set-url origin https://github.com/kushal613/Personal-Website.git
git branch -M main
git push -u origin main
```

### Step 2: Enable GitHub Pages

1. Go to https://github.com/kushal613/Personal-Website
2. Click "Settings"
3. Scroll to "GitHub Pages"
4. Under "Build and deployment":
   - Source: Deploy from a branch
   - Branch: select `main`
   - Folder: `/root` (or `/ (root)`)
5. Click "Save"

### Step 3: Connect Custom Domain

1. In the same Settings → Pages section
2. Under "Custom domain"
3. Enter: `kushalmungee.com`
4. Click "Save"

### Step 4: Update DNS on GoDaddy

1. Log into GoDaddy
2. Go to your domain → DNS
3. Edit the records to point to GitHub:
   - Type: `A`
   - Points to: `185.199.108.153` (or latest GitHub IP)
   - Or let GoDaddy auto-configure

Your site will be live at https://kushalmungee.com in 5-30 minutes!

## ⚡ Option 3: Netlify (Automatic Deployments)

### Easiest Deployment with Automatic Updates

1. **Create Netlify Account**
   - Go to https://netlify.com
   - Sign up with GitHub

2. **Connect Repository**
   - Click "Add new site"
   - Select "Import an existing project"
   - Authorize GitHub
   - Select: `kushal613/Personal-Website`

3. **Configure Build Settings**
   - Build command: (leave empty)
   - Publish directory: `.` (root)
   - Click "Deploy site"

4. **Add Custom Domain**
   - Site settings → Domain management
   - Click "Add custom domain"
   - Enter: `kushalmungee.com`
   - Follow DNS configuration steps

5. **Automatic Deployments**
   - Every time you push to GitHub, Netlify automatically updates your site!

## ✅ Testing Your Website

After deployment, verify everything works:

### Desktop Testing
- [ ] Open https://kushalmungee.com
- [ ] Test all navigation links
- [ ] Click "Get in Touch" and "Learn More" buttons
- [ ] Verify smooth scrolling
- [ ] Test all social media links

### Mobile Testing
- [ ] Open on mobile device or browser devtools
- [ ] Click hamburger menu
- [ ] Test all touch interactions
- [ ] Verify text is readable
- [ ] Check that buttons are clickable

### Browser Compatibility
- [ ] Chrome/Edge
- [ ] Firefox
- [ ] Safari
- [ ] Mobile Safari (iOS)
- [ ] Chrome Mobile (Android)

## 📝 Making Updates

### Small Changes (via GitHub)

1. Edit files locally
2. Commit and push to GitHub:
   ```bash
   git add .
   git commit -m "Update your content"
   git push
   ```
3. Changes deploy automatically (GitHub Pages or Netlify)

### Direct GoDaddy Updates

1. Log into GoDaddy File Manager
2. Edit files directly or re-upload
3. Changes are live immediately

## 🔒 SSL Certificate (HTTPS)

**Good news:** All methods above include free SSL certificates!
- GoDaddy: Auto-enabled for all hosting
- GitHub Pages: Automatic HTTPS
- Netlify: Automatic free Let's Encrypt certificate

Your site should show a green padlock in the browser address bar.

## 🎯 Domain Setup Troubleshooting

### Site not loading?
1. Wait 5-30 minutes for DNS propagation
2. Clear browser cache (Ctrl+Shift+Delete)
3. Try a different browser
4. Check DNS settings are correctly configured

### Files not showing?
1. Verify files uploaded to `public_html` (not a subfolder)
2. Check file names are exactly: `index.html`, `style.css`, `script.js`
3. Ensure `index.html` is set as the default file
4. Check file permissions (should be readable)

### SSL/HTTPS issues?
1. Wait for certificate to generate (5-30 minutes)
2. Force refresh: Ctrl+Shift+R (or Cmd+Shift+R on Mac)
3. Check certificate in browser address bar

## 📞 Support

- **GoDaddy Support**: https://www.godaddy.com/help
- **GitHub Pages Help**: https://docs.github.com/en/pages
- **Netlify Help**: https://docs.netlify.com/

## 🎉 Celebration!

Once your site is live:
- Share it on LinkedIn: https://www.linkedin.com
- Share on Twitter/X
- Share in your GitHub bio
- Add it to your resume

Congratulations on launching your personal website! 🚀

---

**Pro Tip:** Test locally first by opening `index.html` directly in your browser before deployment!
