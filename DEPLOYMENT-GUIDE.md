# BKK Transit — Deployment Guide
## GitHub Pages + bkktransit.co.th

---

## FILES IN THIS PACKAGE

| File | Purpose |
|------|---------|
| `index.html` | The main BKK Transit app |
| `manifest.json` | Makes the app installable on phone home screens |
| `sw.js` | Service worker — enables offline mode |
| `CNAME` | Tells GitHub Pages to use bkktransit.co.th |

---

## STEP 1 — Create a GitHub Account (5 minutes)

1. Go to **github.com**
2. Click **Sign up**
3. Choose a username — ideally `bkktransit` or your name
4. Verify your email address

---

## STEP 2 — Create the Repository (2 minutes)

1. Once logged in, click the **+** icon (top right) → **New repository**
2. Repository name: `bkktransit.co.th`
3. Set to **Public**
4. Tick **Add a README file**
5. Click **Create repository**

---

## STEP 3 — Upload Your Files (3 minutes)

1. In your new repository, click **Add file** → **Upload files**
2. Upload all 4 files at once:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `CNAME`
3. In the commit message box, type: `Launch BKK Transit v2.0`
4. Click **Commit changes**

---

## STEP 4 — Enable GitHub Pages (2 minutes)

1. In your repository, click **Settings** (top menu)
2. Click **Pages** in the left sidebar
3. Under **Source**, select **Deploy from a branch**
4. Branch: select **main**, folder: **/ (root)**
5. Click **Save**

Your app will be live at `yourusername.github.io/bkktransit.co.th` within ~60 seconds.

---

## STEP 5 — Register bkktransit.co.th (15 minutes)

.co.th domains require a Thai business or person.

**Option A — Register directly:**
1. Go to **thnic.co.th** (Thailand NIC — official .co.th registrar)
2. Search for `bkktransit`
3. Cost: ~฿1,200–2,500/year
4. You'll need a Thai ID or company registration

**Option B — Use a registrar:**
- Namecheap or GoDaddy can register .co.th
- Slightly higher cost (~฿1,500–3,000/year) but easier process

---

## STEP 6 — Connect Domain to GitHub Pages (10 minutes)

In your domain registrar's DNS settings, add these records:

| Type  | Name | Value                  |
|-------|------|------------------------|
| A     | @    | 185.199.108.153        |
| A     | @    | 185.199.109.153        |
| A     | @    | 185.199.110.153        |
| A     | @    | 185.199.111.153        |
| CNAME | www  | yourusername.github.io |

Then in GitHub → Settings → Pages:
1. Under **Custom domain**, type `bkktransit.co.th`
2. Click **Save**
3. Tick **Enforce HTTPS** (wait ~15 minutes for SSL certificate)

---

## STEP 7 — Install on Your Phone

Once live at bkktransit.co.th:

**iPhone (Safari):** Open the URL → tap Share → **Add to Home Screen** → Add

**Android (Chrome):** Open the URL → tap menu (⋮) → **Install App** or **Add to Home Screen**

The app appears with the 🚆 icon, full screen, no browser chrome.

---

## UPDATING THE APP

1. Go to your GitHub repository
2. Click on the file you want to update
3. Click the pencil ✏️ icon to edit, OR click **Add file → Upload files** to replace it
4. Commit the change
5. GitHub Pages rebuilds automatically in ~60 seconds

---

## SUPPORT

If you get stuck, share:
- Which step you're on
- What you see on screen
- Any error messages

🚆🐝
