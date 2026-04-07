# Millcreek Church Utah — Website

A full multi-page church website built in the style of bellevue.org, adapted for **Millcreek Church Utah** (Southern Baptist Convention).

## Live Site
Once deployed, your site will be live at:
`https://YOUR-USERNAME.github.io/millcreek-church/`

## File Structure
```
millcreek-church/
├── index.html              ← Home page
├── .nojekyll               ← Required for GitHub Pages
├── README.md               ← This file
├── css/
│   └── style.css           ← Shared stylesheet (used by all pages)
└── pages/
    ├── jesus.html
    ├── vision.html
    ├── beliefs.html
    ├── pastor.html
    ├── new.html
    ├── next-steps.html
    ├── worship.html
    ├── groups.html
    ├── midweek.html
    ├── serve.html
    ├── ministries.html
    ├── adults.html
    ├── men.html
    ├── women.html
    ├── young-adults.html
    ├── next-gen.html
    ├── kids.html
    ├── special-needs.html
    ├── counseling.html
    ├── discipleship.html
    ├── missions.html
    ├── music.html
    ├── pastoral.html
    ├── prayer.html
    ├── recreation.html
    ├── media.html
    ├── events.html
    ├── resources.html
    ├── give.html
    ├── campus.html
    └── contact.html
```

## How to Deploy

### Step 1 — Create a new GitHub repository
1. Go to [github.com/new](https://github.com/new)
2. Name it: `millcreek-church`
3. Set to **Public**
4. Do NOT check "Add a README" (we already have one)
5. Click **Create repository**

### Step 2 — Upload the files
**Option A — Upload via GitHub website (easiest):**
1. In your new repo, click **Add file → Upload files**
2. Drag and drop the entire contents of this folder
3. Make sure to include the `css/` folder and `pages/` folder
4. Write commit message: `Initial site upload`
5. Click **Commit changes**

**Option B — Using Git (command line):**
```bash
git init
git add .
git commit -m "Initial Millcreek Church website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/millcreek-church.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages
1. In your repo, go to **Settings** (top menu)
2. Click **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Choose **main** branch and **/ (root)** folder
5. Click **Save**
6. Wait 2–5 minutes

### Step 4 — Your site is live!
Visit: `https://YOUR-USERNAME.github.io/millcreek-church/`

## After Deployment — What to Update

### 1. Replace photo placeholders
Search for `📷` in any HTML file — those are photo placeholder sections.
Replace with real photos by changing the `background-image` URL or `<img src="">` tag.

### 2. Set up Stripe for online giving
In `pages/give.html`, find these lines and replace with your real Stripe Payment Links:
```javascript
'One-Time': 'https://buy.stripe.com/REPLACE_ONETIME'
'Weekly':   'https://buy.stripe.com/REPLACE_WEEKLY'
'Monthly':  'https://buy.stripe.com/REPLACE_MONTHLY'
```
Get your links at: stripe.com → Dashboard → Payment Links → New Link

### 3. Add sermon videos
In `pages/media.html`, replace the video placeholder div with a YouTube embed:
```html
<iframe width="100%" height="400"
  src="https://www.youtube.com/embed/YOUR-VIDEO-ID"
  frameborder="0" allowfullscreen></iframe>
```

### 4. Update contact email
Replace `church@millcreekchurchutah.com` with your real church email.

### 5. Custom domain (optional)
If you have a domain like `millcreekchurchutah.com`:
1. Go to repo **Settings → Pages → Custom domain**
2. Type your domain and save
3. At your domain registrar, add these DNS A records:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```

## Millcreek Church Info
- **Address:** 1515 E 4500 S, Millcreek, UT 84124
- **Phone:** (801) 278-5683
- **Facebook:** facebook.com/pages/Millcreek-Baptist-Church/105877852786914
- **Affiliation:** Southern Baptist Convention
