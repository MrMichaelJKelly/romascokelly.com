# Converting romascokelly.com to GitHub Pages

## Step 1: Create a GitHub Repository

1. Go to https://github.com/new
2. Repository name: `romascokelly.com`
3. Set to **Public** (required for free GitHub Pages)
4. Check "Add a README file"
5. Click "Create repository"

## Step 2: Enable GitHub Pages

1. In your repository, go to **Settings** → **Pages**
2. Under "Source", select **Deploy from a branch**
3. Select **main** branch and **/ (root)** folder
4. Click **Save**

## Step 3: Upload the Website Files

I've created all the HTML files you need. You can either:

**Option A: Upload via GitHub Web Interface**
1. Click "Add file" → "Upload files"
2. Drag and drop all the HTML files I've created
3. Commit the files

**Option B: Use Git (if you're comfortable with command line)**
```bash
git clone https://github.com/MrMichaelJKelly/romascokelly.com.git
cd romascokelly.com
# Copy all the HTML files into this directory
git add .
git commit -m "Initial GitHub Pages site"
git push
```

## Step 4: Configure Custom Domain (Optional)

To use your romascokelly.com domain:

1. In your repository, go to **Settings** → **Pages**
2. Under "Custom domain", enter `www.romascokelly.com`
3. Click **Save**
4. This will create a `CNAME` file in your repo

5. Update your DNS settings at TigerTech (or wherever you manage DNS):
   - Add a CNAME record: `www` → `mrmichaeljkelly.github.io`
   - Or set A records for the apex domain to GitHub's IPs:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

## Step 5: Wait and Verify

- GitHub Pages deploys in 1-5 minutes
- Your site will be at: `https://mrmichaeljkelly.github.io/romascokelly.com/`
- Once DNS propagates (up to 48 hours), it'll work at `romascokelly.com`

## Files to Upload

See the artifacts I've created:
1. `index.html` - Home page
2. `directions.html` - Directions page
3. `france.html` - France overview page
4. `why-grenoble.html` - Why Grenoble page
5. `diary.html` - France diary index
6. `style.css` - Stylesheet for all pages

## Downloading Images

You'll need to save these images from your current site:
- Header image: `https://www.romascokelly.com/wp-content/uploads/2017/03/cropped-cropped-Christmas-08-2008-12-25-022-Large-Web-view.jpg`
- Panorama: `https://www.romascokelly.com/wp-content/uploads/2017/03/Panorama.jpg`
- Grenoble image: `https://www.thediscoveriesof.com/wp-content/uploads/2017/09/Grenoble-shutterstock_161553770.jpg.webp`

Create an `images` folder in your repo and upload these images there, then the HTML files will reference them correctly.

## Cost Savings

GitHub Pages: **$0/year** 🎉
TigerTech: $185/year

**Annual savings: $185**