# SDA Lab Website

Space Domain Awareness Lab @ Embry-Riddle Aeronautical University  
Built with plain HTML, CSS, and JavaScript — no frameworks needed.

---

## File Structure

```
sda-lab/
├── index.html              ← Homepage
├── css/
│   └── style.css           ← All styles
├── js/
│   └── main.js             ← Starfield + nav + animations
├── images/                 ← Put your photos here
└── pages/
    ├── research.html
    ├── people.html
    ├── publications.html
    ├── news.html
    └── join.html
```

---

## How to Deploy on GitHub Pages (Step by Step)

### Step 1 — Create a GitHub account
Go to https://github.com and sign up for a free account.

### Step 2 — Create a new repository
1. Click the **+** button (top right) → "New repository"
2. Name it exactly: `yourusername.github.io`  
   (Replace "yourusername" with your actual GitHub username)
3. Set it to **Public**
4. Click "Create repository"

### Step 3 — Upload your files
1. On the repository page, click **"uploading an existing file"**
2. Drag and drop the entire `sda-lab` folder contents (all files and folders)
3. Write a commit message like "Initial website upload"
4. Click **"Commit changes"**

### Step 4 — Enable GitHub Pages
1. Go to your repository → **Settings** tab
2. Scroll to **Pages** in the left sidebar
3. Under "Source", select **"Deploy from a branch"**
4. Branch: **main**, Folder: **/ (root)**
5. Click **Save**

### Step 5 — Your site is live!
After ~2 minutes, your site will be live at:  
`https://yourusername.github.io`

---

## Customizing Your Content

### Change "[Your Name]" throughout the site
Search for `[Your Name]`, `[Your Full Name]`, `youremail@erau.edu`, `[Department]`, `[Institution]` across all HTML files and replace with your real information.

### Add your headshot
1. Put your photo in the `images/` folder (e.g., `images/headshot.jpg`)
2. In `pages/people.html`, find the PI photo section and change:
   ```html
   <div class="team-photo">👩‍🔬</div>
   ```
   to:
   ```html
   <div class="team-photo"><img src="../images/headshot.jpg" alt="Dr. Your Name"/></div>
   ```

### Add a publication
In `pages/publications.html`, copy this block and fill it in:
```html
<div class="pub-item">
  <div class="pub-year">2024</div>
  <div>
    <div class="pub-title">Your Paper Title</div>
    <div class="pub-authors">Author A., <strong>Your Name</strong></div>
    <div class="pub-journal">Journal Name</div>
    <a href="https://doi.org/..." class="pub-doi">doi: 10.xxxx/xxxxxx</a>
  </div>
</div>
```

### Add a news item
In `pages/news.html`, copy a `news-full-card` block and edit the month, year, type, title, and description. Type classes: `type-launch`, `type-paper`, `type-award`, `type-hiring`.

### Update stats on homepage
In `index.html`, find the `stats-inner` div and update the numbers to reflect your lab's real metrics.

### Add a custom domain (optional)
If you buy a domain (e.g., `sdalab.com` from Namecheap):
1. In your GitHub repo, go to Settings → Pages
2. Under "Custom domain", type your domain name and click Save
3. At your domain registrar, add a CNAME record pointing to `yourusername.github.io`
4. Wait up to 24 hours for DNS to propagate

---

## Colors (if you want to adjust)

Edit `css/style.css` at the top — the `:root` block:

```css
--accent:   #4f9cf9;   /* orbital blue — links, highlights */
--accent2:  #f9a84f;   /* ERAU gold — secondary highlights */
--bg:       #080c14;   /* page background */
```

---

## Need Help?

If you get stuck, search for the specific file and text in GitHub's web editor (pencil icon on any file). Every edit can be made directly in the browser — no coding tools needed for updates.
