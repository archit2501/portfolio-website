# 🚀 Portfolio Website Deployment Guide

This guide will help you deploy Archit Jain's portfolio website online using various platforms.

## 🌐 Quick Deploy Options

### Option 1: Netlify (Recommended) ⭐
**Best for: Easy deployment with working contact forms**

1. **Fork/Clone the repository** to your GitHub account
2. **Go to [Netlify](https://netlify.com)** and sign in with GitHub
3. **Click "Add new site" → "Import an existing project"**
4. **Select your repository** and configure:
   - Build command: `echo "Static site"`
   - Publish directory: `.` (root)
5. **Deploy!** Your site will be live instantly
6. **Contact form works automatically** - no configuration needed!

**Your site will be available at:** `https://[random-name].netlify.app`

To customize the domain:
- Go to Site settings → Domain management
- Add your custom domain

### Option 2: Vercel ⚡
**Best for: Fast deployment and great performance**

1. **Fork/Clone the repository** to your GitHub account
2. **Go to [Vercel](https://vercel.com)** and sign in with GitHub
3. **Click "Add New" → "Project"**
4. **Import your repository**
5. **Deploy!** No configuration needed

**Your site will be available at:** `https://[project-name].vercel.app`

*Note: For contact forms on Vercel, you'll need to set up Formspree (see Contact Form Setup below)*

### Option 3: GitHub Pages 📚
**Best for: Free hosting directly from GitHub**

1. **Fork the repository** to your GitHub account
2. **Go to repository Settings → Pages**
3. **Select source:** Deploy from a branch
4. **Choose branch:** `main` and folder `/ (root)`
5. **Save** - your site will be available at: `https://[username].github.io/portfolio-website`

*Note: For contact forms on GitHub Pages, you'll need to set up Formspree (see Contact Form Setup below)*

## 📧 Contact Form Setup

### For Netlify (Automatic)
✅ **Already configured!** The contact form will work automatically with Netlify Forms.

### For Vercel/GitHub Pages (Manual Setup Required)

1. **Go to [Formspree](https://formspree.io)** and create a free account
2. **Create a new form** and get your form ID
3. **Update the contact form** in `index.html`:

Replace line 338:
```html
<form class="contact-form" id="contact-form" name="contact" method="POST" data-netlify="true" netlify-honeypot="bot-field">
```

With:
```html
<form class="contact-form" id="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

4. **Replace `YOUR_FORM_ID`** with your actual Formspree form ID

## 🛠️ Customization Before Deployment

### Update Personal Information
1. **Replace profile photo:** Upload your photo as `profile-photo.jpg`
2. **Update contact details** in `index.html`:
   - Email: `architjain2501@gmail.com`
   - Phone: `+91 8595875456`
   - Social media links

### Customize Content
1. **Projects:** Update project descriptions and GitHub links
2. **Skills:** Modify the skills sections to match your expertise
3. **About section:** Personalize your story and background

## 🎯 Domain Setup (Optional)

### Custom Domain with Netlify
1. Buy a domain from any registrar
2. In Netlify: Site settings → Domain management → Add custom domain
3. Update your domain's DNS settings as instructed

### Custom Domain with Vercel
1. In Vercel: Project Settings → Domains → Add
2. Follow the DNS configuration instructions

### Custom Domain with GitHub Pages
1. In repository: Settings → Pages → Custom domain
2. Add a `CNAME` file with your domain name
3. Configure DNS with your registrar

## 🚀 Deployment Status

Once deployed, your portfolio will be available 24/7 online with:
- ✅ Responsive design for all devices
- ✅ Fast loading times
- ✅ Working contact form
- ✅ Professional appearance
- ✅ SEO optimization

## 📱 Testing Your Deployment

After deployment, test:
1. **Navigation:** All menu items work
2. **Responsive design:** Test on mobile/tablet
3. **Contact form:** Send a test message
4. **External links:** GitHub, LinkedIn, etc.
5. **Loading speed:** Should load quickly

## 🔧 Troubleshooting

### Contact Form Not Working
- **Netlify:** Form should work automatically
- **Other platforms:** Set up Formspree as described above

### Site Not Loading
- Check deployment logs in your platform
- Ensure all files are uploaded correctly
- Verify domain DNS settings

### Images Not Showing
- Ensure `profile-photo.jpg` is in the repository
- Check file names and paths are correct

## 📞 Need Help?

If you encounter any issues:
1. Check the platform's documentation
2. Review deployment logs
3. Ensure all files are committed to your repository

**Your portfolio is now ready to impress clients and showcase your skills! 🌟**