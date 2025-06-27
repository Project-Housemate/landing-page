# 🏠 Housemate Beta Landing Page

A beautiful, responsive landing page to collect beta testers for the Housemate app.

## 🚀 Quick Setup

### 1. GitHub Pages Hosting

1. **Push to GitHub**:
   ```bash
   git add landing-page/
   git commit -m "Add beta landing page"
   git push origin main
   ```

2. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** tab
   - Scroll down to **Pages** section
   - Under **Source**, select **Deploy from a branch**
   - Choose **main** branch and **/ (root)** folder
   - Click **Save**

3. **Access your site**:
   - Your landing page will be available at: `https://yourusername.github.io/project-housemate/landing-page/`
   - GitHub will show you the exact URL in the Pages settings

### 2. Google Form Integration

1. **Create Google Form**:
   - Go to [forms.google.com](https://forms.google.com)
   - Click **+ Blank** to create a new form
   - Title it "Housemate Beta Signup"

2. **Add these questions**:
   - **Full Name** (Short answer, Required)
   - **Email Address** (Short answer, Required)
   - **Preferred Platform** (Multiple choice, Required)
     - Options: iOS (iPhone/iPad), Android, Both iOS and Android
   - **How many housemates do you have?** (Multiple choice, Required)
     - Options: 1 housemate, 2-3 housemates, 4-5 housemates, 6+ housemates

3. **Get the form URL**:
   - Click the **Send** button (top right)
   - Click the **Link** icon (<>)
   - Copy the URL that appears

4. **Update the landing page**:
   - Open `landing-page/index.html`
   - Find the line with `YOUR_GOOGLE_FORM_URL_HERE`
   - Replace it with your Google Form URL

   ```html
   <a href="https://forms.gle/your-actual-form-id" 
      target="_blank" 
      class="submit-button">
   ```

### 3. Optional: Custom Domain

If you want a custom domain (like `beta.yourdomain.com`):

1. **Add CNAME file**:
   ```bash
   echo "beta.yourdomain.com" > landing-page/CNAME
   ```

2. **Update DNS**:
   - Add a CNAME record pointing to `yourusername.github.io`

3. **Configure in GitHub**:
   - Go to Settings > Pages
   - Add your custom domain

## 📊 View Responses

- Go to your Google Form
- Click **Responses** tab
- View all beta signups in real-time
- Export to Google Sheets for analysis

## 🎨 Customization

The landing page uses your app's exact theme:
- **Colors**: Purple gradient (`#4708bd` to `#6200ea`)
- **Font**: Archivo (matches your app)
- **Logo**: Your Housemate logo
- **Responsive**: Works on all devices

## 📁 File Structure

```
landing-page/
├── index.html          # Main landing page
├── assets/
│   └── Housemate-Logo.png  # Your app logo
├── CNAME              # Custom domain (optional)
└── README.md          # This file
```

## 🔧 Troubleshooting

**Logo not showing?**
- Make sure `assets/Housemate-Logo.png` exists
- Check the file path in `index.html`

**Form not working?**
- Verify the Google Form URL is correct
- Make sure the form is set to accept responses

**Page not loading?**
- Check GitHub Pages is enabled
- Wait a few minutes for deployment
- Try incognito/private browsing

## 📈 Next Steps

1. **Share the link** with potential beta testers
2. **Monitor signups** in Google Forms
3. **Follow up** with testers when your app is ready
4. **Update the page** as needed (just push changes to GitHub)

---

**Your landing page URL**: `https://yourusername.github.io/project-housemate/landing-page/`

Replace `yourusername` with your actual GitHub username! 