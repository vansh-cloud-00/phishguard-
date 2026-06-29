# 🛡️ PhishGuard – Phishing Awareness & Cyber Safety

A static web app for phishing awareness training, quizzes, and threat intelligence.

## 🚀 Deploy to GitHub Pages (Step-by-Step)

### 1. Create a GitHub Repository
1. Go to [github.com](https://github.com) → click **New repository**
2. Name it `phishguard` (or anything you like)
3. Set it to **Public**
4. Do **NOT** check "Add README" (you already have one)
5. Click **Create repository**

### 2. Upload the Files
**Option A – Drag & Drop (easiest):**
1. On the repository page, click **uploading an existing file**
2. Drag all files from this folder into the browser
3. Click **Commit changes**

**Option B – Git (if you have Git installed):**
```bash
cd phishguardnew
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/phishguard.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to your repository → **Settings** → **Pages** (left sidebar)
2. Under **Source**, select **Deploy from a branch**
3. Choose branch: `main`, folder: `/ (root)`
4. Click **Save**
5. Wait ~2 minutes, then your site is live at:
   `https://YOUR_USERNAME.github.io/phishguard/`

---

## 🔥 Optional: Enable Firebase

To track stats across devices (instead of just localStorage):

1. Go to [console.firebase.google.com](https://console.firebase.google.com)
2. Create a project → Add a web app → Copy the config
3. Open `js/firebase-config.js`
4. Replace the placeholder values with your real config
5. Set `FIREBASE_ENABLED = true`

Without Firebase, everything works using the browser's localStorage — no setup needed.

---

## 📁 File Structure

```
index.html          ← Home page
about.html          ← About page
learn.html          ← Learning modules
quiz.html           ← Interactive quiz
threat.html         ← Threat Intel scanner
dashboard.html      ← Your progress dashboard
detector.html       ← URL detector (links to threat.html)
css/styles.css      ← All styles
js/main.js          ← Shared utilities
js/quiz.js          ← Quiz logic
js/dashboard.js     ← Dashboard stats
js/firebase-config.js ← Optional Firebase setup
.nojekyll           ← Required for GitHub Pages
404.html            ← Custom 404 page
```
