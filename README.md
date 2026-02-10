# Psychology Practice Website

A warm, professional website for a clinical psychologist, featuring smooth navigation, responsive design, and an inviting aesthetic.

## 📁 File Structure

```
your-repository-name/
├── index.html          # Main homepage with all sections
├── contact.html        # Contact form page
├── styles.css          # All styles and responsive design
├── script.js           # JavaScript for interactivity
├── images/             # Folder for your images (create this)
│   ├── hero-image.jpg  # Hero section image
│   └── profile.jpg     # About section profile photo
└── README.md           # This file
```

## 🚀 Setup Instructions

### 1. Create Your GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the **+** icon in the top-right → **New repository**
3. Name it (e.g., `psychologist-website` or `dr-[yourname]-website`)
4. Choose **Public** or **Private**
5. Don't initialize with README (you already have these files)
6. Click **Create repository**

### 2. Upload Your Files to GitHub

**Option A: Upload via GitHub Web Interface (Easiest)**

1. On your new repository page, click **uploading an existing file**
2. Drag and drop these files:
   - `index.html`
   - `contact.html`
   - `styles.css`
   - `script.js`
3. Add a commit message like "Initial website upload"
4. Click **Commit changes**

**Option B: Use Git Command Line**

```bash
# Navigate to your project folder
cd path/to/your/website-files

# Initialize git
git init

# Add all files
git add .

# Commit
git commit -m "Initial website upload"

# Add your GitHub repository as remote (replace with your URL)
git remote add origin https://github.com/your-username/your-repo-name.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 3. Add Your Images

1. In your repository, click **Add file** → **Upload files**
2. Create a folder called `images` (or upload images and specify `images/` in the filename)
3. Upload:
   - `hero-image.jpg` - A calming, professional image for the hero section
   - `profile.jpg` - Your partner's professional headshot

**Image Recommendations:**
- **Hero image**: Peaceful therapy space, nature scene, or abstract calming imagery (16:10 or 4:3 ratio)
- **Profile photo**: Professional headshot with natural lighting (3:4 or 1:1 ratio)
- **Format**: JPG or PNG
- **Size**: Optimize images to under 500KB each for fast loading

### 4. Enable GitHub Pages (Free Hosting!)

1. In your repository, go to **Settings**
2. Scroll down to **Pages** (left sidebar)
3. Under **Source**, select **main** branch
4. Click **Save**
5. Wait a few minutes - your site will be live at:
   ```
   https://your-username.github.io/your-repo-name/
   ```

## ✏️ Customization Guide

### Essential Edits (Must Do)

Open each file and replace placeholder content:

**index.html & contact.html:**
- Replace `[Name]` with the psychologist's name
- Replace `[Street Address]`, `[City, State ZIP]`, etc.
- Update contact info: phone number and email
- Update credentials, specializations, and bio text
- Update the Google Maps embed URL (see below)

**Google Maps:**
1. Go to [Google Maps](https://www.google.com/maps)
2. Search for your office address
3. Click **Share** → **Embed a map**
4. Copy the `<iframe>` code
5. Replace the iframe in `index.html` (around line 219)

### Styling Adjustments (Optional)

**Change Colors** (styles.css, lines 10-15):
```css
--primary-green: #2D5F4C;        /* Main green color */
--primary-green-light: #3A7259;  /* Lighter green for hovers */
--bg-cream: #FAF8F5;             /* Background color */
```

**Change Fonts** (index.html & contact.html, line 8):
- Current fonts: Crimson Pro (headings) + Karla (body)
- Browse [Google Fonts](https://fonts.google.com/) for alternatives
- Replace the Google Fonts link with your chosen fonts
- Update CSS variables in `styles.css` (lines 18-19)

### FAQ Content

Edit the FAQ section in `index.html` (lines 152-230):
- Add, remove, or modify questions
- Keep the same HTML structure for each FAQ item

## 🔧 Form Functionality

The contact form currently displays a success message but **doesn't actually send emails**. To make it functional:

**Option 1: Formspree (Easiest, Free)**
1. Sign up at [Formspree](https://formspree.io/)
2. Create a new form
3. Update `contact.html` line 26:
   ```html
   <form id="contactForm" action="https://formspree.io/f/YOUR-FORM-ID" method="POST">
   ```

**Option 2: Netlify Forms (If hosting on Netlify)**
1. Add `netlify` attribute to form tag
2. Deploy to Netlify instead of GitHub Pages

**Option 3: EmailJS**
1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Follow their documentation to integrate
3. Update `script.js` with EmailJS code

**Option 4: Custom Backend**
- Requires a server (Node.js, Python, PHP, etc.)
- Beyond scope of basic setup

## 📱 Testing Your Website

### Before Going Live
- ✅ Test all navigation links
- ✅ Test mobile responsiveness (use browser dev tools)
- ✅ Verify all images load correctly
- ✅ Check FAQ accordion functionality
- ✅ Test contact form (even if just shows success message)
- ✅ Proofread all content

### Browser Testing
Test in multiple browsers:
- Chrome/Edge
- Firefox
- Safari (if on Mac)
- Mobile browsers

## 🎨 Design Features

This website includes:
- **Smooth scrolling navigation** with active section highlighting
- **Responsive design** that works on all devices
- **FAQ accordion** with smooth animations
- **Embedded Google Maps** for location
- **Professional contact form** with validation
- **Warm color palette** using off-white, dark green, and charcoal
- **Modern animations** that feel calm and professional

## 🔄 Making Updates

After initial setup, to update your website:

1. Edit files locally
2. Go to your repository on GitHub
3. Click on the file you want to update
4. Click the pencil icon (Edit)
5. Make your changes
6. Scroll down and click **Commit changes**
7. Changes will appear on your live site in 1-2 minutes

## 📞 Common Issues & Solutions

**Images not showing:**
- Check file paths are correct: `images/hero-image.jpg`
- Ensure images are uploaded to the `images` folder
- Check image file names match exactly (case-sensitive)

**Google Maps not working:**
- Make sure you replaced the iframe src with your location
- Ensure iframe code is complete

**Mobile menu not working:**
- Clear browser cache
- Check that script.js is loaded correctly

**Form not submitting:**
- This is expected - see "Form Functionality" section above
- Success message will still show for testing

## 💡 Next Steps

1. **SEO**: Add meta descriptions and title tags
2. **Analytics**: Add Google Analytics to track visitors
3. **Accessibility**: Test with screen readers
4. **Performance**: Optimize images further with tools like TinyPNG
5. **Custom Domain**: Purchase and connect a custom domain (e.g., drname.com)
6. **SSL Certificate**: GitHub Pages provides this automatically

## 📝 License

This website template is provided as-is for your personal use.

## 🤝 Support

If you run into issues:
1. Check this README thoroughly
2. Search GitHub documentation
3. Ask the developer who created this template

---

**Built with care for mental health professionals** 🌿
