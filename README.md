# Bryan Jay U. Amero — Portfolio & Résumé

A single-page portfolio and résumé site. Visitors can browse work by category, open
any piece full-size, and read/print the résumé.

## Files in this folder

- `index.html` — the entire site (HTML, CSS, and JavaScript in one file).
- `works.json` — your published projects, i.e. what visitors see. Replace the starter entries with your own.
- `.nojekyll` — tells GitHub Pages to serve the files as-is.

Upload **all three** to your repository.

---

## Put it on GitHub and go live — easiest way (no tools to install)

1. Sign in at [github.com](https://github.com) and click **New repository**.
   - Name it `your-username.github.io` to get a clean address like `https://your-username.github.io/`
   - …or name it anything (e.g. `portfolio`) for `https://your-username.github.io/portfolio/`
   - Set it to **Public** (free GitHub Pages only works on public repos), then **Create repository**.
2. On the repo page, click **Add file → Upload files**. Drag in `index.html`, `works.json`, and `.nojekyll`. Scroll down and **Commit changes**.
3. Go to **Settings** (top tab) → **Pages** (left menu, under "Code and automation").
4. Under **Build and deployment**: Source = **Deploy from a branch**; Branch = **main**, folder = **/ (root)**. Click **Save**.
5. Wait about a minute, then refresh. Your live link appears at the top of the Pages screen — click **Visit site**.

> First publish can take up to ~10 minutes. Later changes usually appear within a minute or two.

---

## Or with Git (command line)

From the folder that contains these files:

```bash
git init
git add .
git commit -m "Add portfolio site"
git branch -M main
git remote add origin https://github.com/your-username/your-repo.git
git push -u origin main
```

Then do step 3–5 above to turn on Pages.

---

## Adding or updating your work after launch

Pick whichever is easier:

**A) Use the site, then export.** On the live page click **+ Add work**, add and arrange
your pieces, then click **Export catalog**. It downloads a fresh `works.json`. Replace the
old `works.json` in your repo with this one (Add file → Upload files, or commit it with Git).

**B) Edit `works.json` by hand.** Each entry looks like:

```json
{
  "title": "Summer Sale poster",
  "category": "Social Media",
  "desc": "A short line about the project.",
  "image": "images/summer-sale.jpg"
}
```

`image` can be:
- a full URL (e.g. an image you host somewhere), or
- a path to an image you also commit to the repo (e.g. put it in an `images/` folder and use `"images/summer-sale.jpg"`), or
- `null` for a colored placeholder tile.

> Tip: if you're checking changes in the **same browser** you used before, open a private/incognito
> window. The site remembers your last view locally, so a normal window may show the old version.

---

## Using your own domain (kagie.website)

In **Settings → Pages → Custom domain**, enter `kagie.website` and Save, then point your
domain's DNS at GitHub Pages. The exact DNS records depend on your registrar — ask and I'll
give you the precise ones.
