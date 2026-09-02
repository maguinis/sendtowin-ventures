# SendtoWin Ventures

Static, single-page site. No build step, no dependencies. Just `index.html` plus a `vercel.json` for clean URLs.

## Push to GitHub

```
cd sendtowin-ventures-site
git init
git add .
git commit -m "Initial site"
git branch -M main
git remote add origin https://github.com/<your-username>/sendtowin-ventures.git
git push -u origin main
```

(Create the empty repo on GitHub first, without a README, so the push doesn't conflict.)

## Deploy on Vercel

1. Go to vercel.com and click "Add New" then "Project".
2. Import the `sendtowin-ventures` repo you just pushed.
3. Framework preset: choose "Other" (it's a static site, no build command needed).
4. Click Deploy.

## Connect your domain

Once deployed, in the Vercel project go to Settings then Domains, and add whichever domain you land on (for example `sendtowinventures.com`). Vercel will give you the DNS records to set at your registrar. It usually takes a few minutes to a few hours to propagate.

## Editing later

Everything (styles included) lives in `index.html`. Change the text or colors there, commit, and push. Vercel redeploys automatically on every push to `main`.
