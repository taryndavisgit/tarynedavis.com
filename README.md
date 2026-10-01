# tarynedavis.com

Plain HTML and CSS. No build step.

## Before you publish
1. In `index.html`, replace both `YOUR-EMAIL@tarynedavis.com` with your real address (search the file for `YOUR-EMAIL`).
2. Read through the copy and adjust anything you'd phrase differently.

## Publish with GitHub Pages (free)
1. Create a new public repository on GitHub, for example `tarynedavis.com`.
2. Upload every file in this folder to the repository root (including `CNAME`).
3. In the repository, go to **Settings > Pages**. Under **Build and deployment**, set Source to **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
4. Under **Custom domain**, confirm `tarynedavis.com` is filled in (the CNAME file does this).

## Point your GoDaddy domain at GitHub
In GoDaddy, open **My Products > tarynedavis.com > DNS**, then:
1. Delete any existing **A** record for `@` (often a GoDaddy "parked" record).
2. Add four **A** records, Name `@`, one for each value:
   185.199.108.153, 185.199.109.153, 185.199.110.153, 185.199.111.153
3. Add or edit a **CNAME** record: Name `www`, Value `YOUR-GITHUB-USERNAME.github.io`
4. Leave your email-related records (MX, TXT for email) alone.

DNS can take up to a day to update. Once the site loads, go back to **Settings > Pages** and check **Enforce HTTPS**.

## Making changes later
Edit `index.html` or `styles.css` on GitHub and commit. The site updates within a minute or two.
