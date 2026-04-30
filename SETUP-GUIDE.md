# How to publish this course online
## GitHub + Netlify — step by step

This guide assumes no prior experience with GitHub or Netlify.
Total time: approximately 20 minutes.

---

## Part 1 — Create a GitHub account (skip if you have one)

1. Go to **github.com**
2. Click **Sign up**
3. Choose a username (this appears in your URL, e.g. `github.com/yourname`)
4. Enter your email and create a password
5. Verify your email when GitHub sends you a confirmation

---

## Part 2 — Create the repository

A repository is a folder on GitHub that stores your files.

1. Log into GitHub
2. Click the **+** icon in the top-right corner → **New repository**
3. Fill in:
   - **Repository name:** `linux-course` (or any name you prefer)
   - **Description:** "Six-month Linux seminar for ages 15–18"
   - **Visibility:** Public ✓ (required for free Netlify hosting)
   - Leave everything else at default
4. Click **Create repository**

You now have an empty repository.

---

## Part 3 — Upload your files

You need to upload all 13 HTML files plus the README.

**Option A — Upload via the GitHub website (no technical knowledge required):**

1. In your new repository, click **Add file** → **Upload files**
2. Drag all 13 HTML files into the upload area:
   - `index.html`
   - `phase1-teacher-manual.html`
   - `phase1-handouts.html`
   - `phase2-teacher-manual.html`
   - `phase2-handouts.html`
   - `phase3-teacher-manual.html`
   - `phase3-handouts.html`
   - `phase4-teacher-manual.html`
   - `phase4-handouts.html`
   - `phase5-teacher-manual.html`
   - `phase5-handouts.html`
   - `phase6-teacher-manual.html`
   - `phase6-handouts.html`
3. Also upload `README.md`
4. At the bottom, in **Commit changes**, write a message like: `Add all course materials`
5. Click **Commit changes**

All files are now in GitHub. You can verify by clicking on the repository name and seeing the file list.

**Option B — Upload via terminal (if you have git installed):**

```bash
# Clone your empty repository
git clone https://github.com/YOURUSERNAME/linux-course.git
cd linux-course

# Copy all HTML files and README into this folder
# Then:
git add .
git commit -m "Add all course materials"
git push origin main
```

---

## Part 4 — Deploy with Netlify

1. Go to **netlify.com**
2. Click **Sign up** → choose **Sign up with GitHub** (easier — links your accounts)
3. Authorize Netlify to access your GitHub account
4. Click **Add new site** → **Import an existing project**
5. Click **Deploy with GitHub**
6. Select your `linux-course` repository from the list
7. On the configuration screen:
   - **Branch to deploy:** main
   - **Build command:** leave empty
   - **Publish directory:** leave empty (or type `/`)
8. Click **Deploy site**

Netlify will deploy your site in about 30 seconds.

---

## Part 5 — Your site is live

After deployment, Netlify gives you a URL like:
`https://random-name-12345.netlify.app`

You can change this to something more readable:
1. In Netlify dashboard, click **Site configuration** → **Change site name**
2. Type something like `linux-course-campiling`
3. Your URL becomes: `https://linux-course-campiling.netlify.app`

Share this URL with anyone who needs access to the materials.

---

## Part 6 — Updating files later

When you update a file (for example, you improve a handout after teaching a phase), the process is:

1. Go to your GitHub repository
2. Click on the file you want to update
3. Click the **pencil icon** (Edit) or upload a new version
4. Commit the change

**Netlify automatically redeploys within 1–2 minutes.** No action needed on Netlify — it watches the GitHub repository and updates the site whenever you push changes.

---

## Optional — custom domain

If you want to use `course.campiling.com` instead of a `.netlify.app` URL:

1. In Netlify: **Site configuration** → **Domain management** → **Add custom domain**
2. Enter `course.campiling.com`
3. Netlify will ask you to add a DNS record in Cloudflare
4. In Cloudflare: go to your campiling.com domain → DNS → Add record
   - Type: CNAME
   - Name: course
   - Target: your-site-name.netlify.app
5. Wait a few minutes for DNS to propagate

You already have Cloudflare managing campiling.com, so this is straightforward.

---

## Summary of what you have after this

| What | Where |
|---|---|
| Source files | GitHub — `github.com/YOURUSERNAME/linux-course` |
| Live website | Netlify — `https://your-site-name.netlify.app` |
| Auto-update | Any push to GitHub → site updates in ~1 minute |
| Cost | Free (both GitHub public repos and Netlify free tier) |

---

*Total files to upload: 13 HTML files + 1 README = 14 files.*
