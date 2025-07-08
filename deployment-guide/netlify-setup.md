# Deploy Zdravo Landing Page to Netlify (Free)

The easiest way to host your Zdravo landing page for free with your custom domain.

## 🚀 Quick Deployment (5 minutes)

### Step 1: Prepare Your Files
1. Make sure you have these files in your `landing-page` folder:
   - `index.html`
   - `privacy.html`
   - `terms.html`
   - `zdravo-icon.png`

### Step 2: Deploy to Netlify
1. Go to [netlify.com](https://netlify.com)
2. Click "Sign up" (free account)
3. Once logged in, you'll see the deploy area
4. **Drag and drop** your entire `landing-page` folder onto the deploy area
5. Wait 30 seconds - your site is now live!
6. Netlify will give you a random URL like `amazing-tesla-123.netlify.app`

### Step 3: Add Your Custom Domain
1. Click on your site name in Netlify dashboard
2. Go to **Site Settings** → **Domain Management**
3. Click **Add custom domain**
4. Enter your domain (e.g., `zdravo.app`)
5. Netlify will show you DNS records to add

### Step 4: Update Your Domain's DNS
In your domain registrar (GoDaddy, Namecheap, etc.), add these records:

**For apex domain (zdravo.app):**
```
Type: A
Name: @
Value: 75.2.60.5
```

**For www subdomain:**
```
Type: CNAME
Name: www
Value: your-site-name.netlify.app
```

### Step 5: Enable HTTPS (Automatic)
- Netlify automatically provides free SSL certificates
- After DNS propagation (5-60 minutes), HTTPS will be enabled
- Your site will redirect HTTP to HTTPS automatically

## 🎉 You're Live!

Your Zdravo landing page is now:
- ✅ Hosted for free
- ✅ Using your custom domain
- ✅ Secured with HTTPS
- ✅ Globally distributed via CDN
- ✅ Mobile optimized

## 🔄 Making Updates

To update your site:
1. Make changes to your HTML files locally
2. Drag and drop the updated folder to Netlify again
3. Your site updates instantly (no downtime)

## 📊 Bonus Features (All Free)

Netlify also provides:
- **Analytics**: See visitor stats
- **Form handling**: If you add contact forms later
- **Branch previews**: Test changes before going live
- **Custom redirects**: Set up URL redirects
- **Performance optimization**: Automatic image compression

## 🆘 Troubleshooting

**Domain not working?**
- DNS changes can take up to 24 hours (usually 5-60 minutes)
- Use [whatsmydns.net](https://whatsmydns.net) to check propagation

**Site not updating?**
- Clear your browser cache (Ctrl+F5 or Cmd+Shift+R)
- Check if you uploaded the right files

**Need help?**
- Netlify has excellent documentation at [docs.netlify.com](https://docs.netlify.com)
- Their support is very responsive for free users

## 💡 Pro Tips

1. **Use Git for easier updates**: Connect your GitHub repo for automatic deployments
2. **Set up redirects**: Add a `_redirects` file for SEO-friendly URLs
3. **Monitor performance**: Use Netlify Analytics to track visitors
4. **Custom 404 page**: Create a `404.html` for better user experience

Your Zdravo landing page is now ready to help people discover the app and start making connections! 🎉