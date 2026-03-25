# Expensio 💸

A fully local, AI-powered personal expense tracker — deployable to GitHub Pages.

## 🚀 Deploy to GitHub Pages

### Step 1 — Create a GitHub repository

1. Go to [github.com/new](https://github.com/new)
2. Create a **public** repository (required for free GitHub Pages)
3. Push this project to the `main` branch

### Step 2 — Add GitHub Secrets

Go to your repo → **Settings → Secrets and variables → Actions → New repository secret**

Add each of the following secrets:

| Secret Name | Where to get it |
|---|---|
| `FIREBASE_API_KEY` | Firebase Console → Project Settings → Your apps → Web app |
| `FIREBASE_AUTH_DOMAIN` | Same as above |
| `FIREBASE_PROJECT_ID` | Same as above |
| `FIREBASE_STORAGE_BUCKET` | Same as above |
| `FIREBASE_MESSAGING_SENDER_ID` | Same as above |
| `FIREBASE_APP_ID` | Same as above |
| `RAZORPAY_KEY_ID` | Razorpay Dashboard → Settings → API Keys |

> Use `rzp_test_...` key for testing, `rzp_live_...` for production.

### Step 3 — Enable GitHub Pages

1. Go to repo → **Settings → Pages**
2. Under **Source**, select **Deploy from a branch**
3. Choose branch: `gh-pages` / `/ (root)`
4. Click **Save**

### Step 4 — Trigger a deployment

Push any change to `main`, or go to **Actions → Deploy to GitHub Pages → Run workflow**.

Your app will be live at:
```
https://<your-username>.github.io/<your-repo-name>/
```

---

## 🔧 Local Development

Open `index.html` directly in your browser. The app runs in **Demo Mode** locally (all Pro features unlocked, no login required).

To test with real Firebase auth locally, run a local server:
```bash
npx serve .
```
Then paste your Firebase config directly into the `FIREBASE_CONFIG` object at the top of the script in `index.html`.

---

## 📋 License & Plan Settings

| Setting | Value |
|---|---|
| Trial duration | 1 day |
| Pro license | Lifetime (no expiry) |
| Trial expense limit | 50 expenses |
| Pro price | ₹499 |
