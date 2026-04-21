# Cassandra Skinner - Portfolio Website

Professional portfolio website showcasing product and design strategy leadership.

## 🌐 Site Structure

- **Home** (`index.html`) - Hero section with key metrics and featured work
- **About** (`about.html`) - Leadership philosophy, career highlights, education
- **Work** (`work.html`) - Strategic case studies
- **Resume** (`resume.html`) - Full resume with download option
- **Contact** (`contact.html`) - Contact information and availability

## 🚀 Deploying to GitHub Pages (Free Hosting)

### Step 1: Create GitHub Repository

1. Go to [github.com](https://github.com) and sign in (or create an account)
2. Click the `+` icon in the top right → "New repository"
3. Name it: `your-username.github.io` (replace `your-username` with your GitHub username)
   - Example: if your username is `caskinne`, name it `caskinne.github.io`
4. Make it **Public**
5. Don't initialize with README (we already have files)
6. Click "Create repository"

### Step 2: Upload Your Website

**Option A: Using GitHub Web Interface (Easiest)**
1. On your new repository page, click "uploading an existing file"
2. Drag all files from `/Users/caskinner/Documents/cassandra-portfolio-website/` into the upload area:
   - index.html
   - about.html
   - work.html
   - resume.html
   - contact.html
   - styles.css
3. Scroll down and click "Commit changes"

**Option B: Using Git (Command Line)**
```bash
cd /Users/caskinner/Documents/cassandra-portfolio-website
git init
git add .
git commit -m "Initial portfolio website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings" tab
3. Click "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait 1-2 minutes for deployment

### Step 4: View Your Site

Your site will be live at: `https://your-username.github.io`

## 🌍 Using a Custom Domain (Optional)

If you want to use `cassandraskinner.com` instead of GitHub's URL:

1. **Buy a domain** from Namecheap, Google Domains, or GoDaddy (~$12/year)

2. **Add custom domain in GitHub:**
   - Go to Settings → Pages
   - Under "Custom domain", enter your domain (e.g., `cassandraskinner.com`)
   - Click "Save"

3. **Configure DNS at your domain registrar:**
   - Add these A records pointing to GitHub:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - Add CNAME record: `www` → `your-username.github.io`

4. Wait 24-48 hours for DNS to propagate

## ✏️ Updating Your Website

To make changes:

1. Edit the HTML files locally
2. Test by opening `index.html` in your browser
3. Upload changed files to GitHub (drag & drop on repository page, or use git push)
4. Changes will appear on your live site within 1-2 minutes

## 📝 What to Update

**Before going live, customize these:**

- [ ] Update all content to reflect your actual work
- [ ] Add real case study details in `work.html`
- [ ] Verify all links work
- [ ] Test on mobile (resize browser to check)
- [ ] Update contact information if needed

## 💡 Tips

- Keep it simple and professional
- Update regularly with new work
- Test all links before sharing
- Share the URL on LinkedIn, resume, etc.

## 🆘 Need Help?

**Common Issues:**

- **Site not showing up:** Wait 2-3 minutes after first deployment
- **Changes not appearing:** Clear browser cache (Cmd+Shift+R)
- **Custom domain not working:** Wait 24-48 hours for DNS
- **404 error:** Make sure files are in root directory, not a subfolder

---

Built with HTML, CSS, and ❤️ | Hosted free on GitHub Pages
