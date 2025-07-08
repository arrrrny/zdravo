# Deploy Zdravo Landing Page to GitHub Pages (Free)

Host your Zdravo landing page for free using GitHub Pages with your custom domain.

## 🚀 Quick Deployment (10 minutes)

### Step 1: Create GitHub Repository
1. Go to [github.com](https://github.com) and sign up/login
2. Click the **"+" icon** → **"New repository"**
3. Name it `zdravo-website` (or any name you prefer)
4. Make it **Public** (required for free GitHub Pages)
5. Check **"Add a README file"**
6. Click **"Create repository"**

### Step 2: Upload Your Files
1. In your new repository, click **"uploading an existing file"**
2. Drag and drop these files from your `landing-page` folder:
   - `index.html`
   - `privacy.html`
   - `terms.html`
   - `zdravo-icon.png`
3. Write a commit message like "Add Zdravo landing page"
4. Click **"Commit changes"**

### Step 3: Enable GitHub Pages
1. Go to your repository **Settings** tab
2. Scroll down to **"Pages"** in the left sidebar
3. Under **"Source"**, select **"Deploy from a branch"**
4. Choose **"main"** branch and **"/ (root)"** folder
5. Click **"Save"**
6. GitHub will show you the URL: `https://yourusername.github.io/zdravo-website`

### Step 4: Add Your Custom Domain
1. Still in Pages settings, scroll to **"Custom domain"**
2. Enter your domain (e.g., `zdravo.app`)
3. Click **"Save"**
4. Check **"Enforce HTTPS"** (after DNS is configured)

### Step 5: Configure Your Domain's DNS
In your domain registrar, add these DNS records:

**For apex domain (zdravo.app):**
```
Type: A
Name: @
Value: 185.199.108.153

Type: A
Name: @
Value: 185.199.109.153

Type: A
Name: @
Value: 185.199.110.153

Type: A
Name: @
Value: 185.199.111.153
```

**For www subdomain:**
```
Type: CNAME
Name: www
Value: yourusername.github.io
```

### Step 6: Verify Domain (Important!)
1. Back in GitHub Pages settings, your domain should show a green checkmark
2. If you see warnings, wait for DNS propagation (5-60 minutes)
3. Enable **"Enforce HTTPS"** once the domain is verified

## 🎉 You're Live!

Your site will be available at:
- `https://yourdomain.com`
- `https://www.yourdomain.com`

## 🔄 Making Updates

**Option 1: Web Interface (Easy)**
1. Go to your repository on GitHub
2. Click on the file you want to edit
3. Click the pencil icon to edit
4. Make changes and commit
5. Site updates automatically in 1-2 minutes

**Option 2: Git Commands (Advanced)**
```bash
git clone https://github.com/yourusername/zdravo-website.git
cd zdravo-website
# Make your changes
git add .
git commit -m "Update landing page"
git push origin main
```

## 📊 Benefits of GitHub Pages

✅ **Completely free** (even with custom domain)
✅ **Automatic SSL** certificates
✅ **Global CDN** for fast loading
✅ **Version control** - track all changes
✅ **Reliable** - 99.9% uptime
✅ **No bandwidth limits**
✅ **Custom 404 pages** supported

## 🔧 Advanced Configuration

### Custom 404 Page
Create a `404.html` file in your repository:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Page Not Found - Zdravo</title>
    <meta http-equiv="refresh" content="3;url=/">
</head>
<body>
    <h1>Oops! Page not found</h1>
    <p>Redirecting to homepage in 3 seconds...</p>
</body>
</html>
```

### Redirects with Jekyll
Create a `_config.yml` file for redirects:
```yaml
plugins:
  - jekyll-redirect-from

# Example redirect
redirect_from:
  - /old-page/
  - /another-old-page/
```

### Google Analytics
Add to your `<head>` section:
```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🆘 Troubleshooting

**"Domain is not properly configured"**
- Wait for DNS propagation (up to 24 hours)
- Check DNS with [whatsmydns.net](https://whatsmydns.net)
- Ensure all 4 A records are added correctly

**Site not updating after changes**
- Changes can take 1-10 minutes to appear
- Clear browser cache (Ctrl+F5)
- Check if commit went through

**HTTPS not working**
- Make sure domain is verified first
- DNS must be properly configured
- Can take up to 24 hours for certificate

**Build failed**
- Check repository "Actions" tab for errors
- Ensure all files are valid HTML
- No special characters in filenames

## 💡 Pro Tips

1. **Use branch protection**: Protect your main branch from accidental changes
2. **Set up monitoring**: Use GitHub's insights to track traffic
3. **Backup regularly**: GitHub is your backup, but consider local copies
4. **SEO optimization**: Add sitemap.xml and robots.txt files
5. **Performance**: Optimize images and minify CSS for faster loading

## 📈 Next Steps

Once your site is live, consider:
- Setting up Google Search Console
- Adding social media meta tags
- Creating a sitemap for SEO
- Monitoring with Google Analytics
- Setting up automated testing

Your Zdravo landing page is now hosted for free on GitHub Pages with your custom domain! 🎉