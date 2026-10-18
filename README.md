# Fairport Cross Country website

A static site for GitHub Pages. Files:

- `index.html` is the whole website
- `data.json` holds the schedule, results and logo setting (the admin panel edits this)
- `logo.png` appears after you upload a logo in the admin panel

## 1. Put it online (about 5 minutes)

1. Create a free account at github.com, then click **New repository**. Name it, for example, `fairport-xc`. Make it **Public**.
2. Click **uploading an existing file** and drag in `index.html`, `data.json` and `.nojekyll` (from this folder). Click **Commit changes**.
3. Go to **Settings > Pages**. Under **Build and deployment**, set **Source** to *Deploy from a branch*, choose branch `main` and folder `/ (root)`, then **Save**.
4. After a minute your site is at `https://YOURNAME.github.io/fairport-xc/`.

Optional custom domain: in **Settings > Pages**, enter your domain under **Custom domain** and add the DNS records GitHub shows you at your domain registrar.

## 2. Make an admin access token (this is your "password")

1. On GitHub, open **Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate new token**.
2. Set **Repository access** to *Only select repositories* and pick `fairport-xc`.
3. Under **Permissions > Repository permissions**, set **Contents** to *Read and write*.
4. Generate it and copy the token (you only see it once). Keep it private, like a password.

## 3. Update the site

1. Open your site, scroll to the footer and click the small **Admin** button.
2. Enter the repository (`yourname/fairport-xc`, usually filled in for you) and your token, then **Sign in**.
3. Add meets, results, individual race results and the logo. Each change is saved to `data.json` in your repo and goes live in about a minute.

Anyone who has the token can edit the site, so only share it with coaches you trust. You can delete the token on GitHub at any time to cut off access.

Also remember to clear the sample data (meets, results, runners) and the "sample data" notes before sharing the site widely.
