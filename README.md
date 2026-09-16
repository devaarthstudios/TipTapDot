# Devaarth Studios site (TipTapDot)

A small static website for the game: home, support, privacy policy, terms and contact.
No build step, no dependencies, plain HTML and one CSS file. It works on GitHub Pages
as is.

## Files

| File | Purpose |
|---|---|
| `index.html` | Landing page with features and a Google Play button |
| `support.html` | How to play, FAQ and troubleshooting |
| `privacy.html` | **Privacy policy** (this is the URL Play Console asks for) |
| `terms.html` | Terms of use |
| `contact.html` | Contact details and what to include in a bug report |
| `404.html` | Friendly not found page |
| `style.css` | Shared dark theme matching the game |
| `icon.png` | Game icon, also used as the favicon |
| `.nojekyll` | Tells GitHub Pages to serve the files exactly as they are |

The contact email used across the site is `devyansh.du@gmail.com`.

## Host it on GitHub Pages

1. Create a new **public** repository, for example `tiptapdot`.
2. Upload every file from this folder to the repository root. Keep `index.html` at the
   root so it becomes the home page.
3. Open the repository, go to **Settings**, then **Pages**.
4. Under **Build and deployment** set Source to **Deploy from a branch**, pick branch
   **main** and folder **/ (root)**, then Save.
5. Wait one or two minutes. Your site will be live at:

   `https://YOUR_GITHUB_USERNAME.github.io/tiptapdot/`

   and the privacy policy will be at:

   `https://YOUR_GITHUB_USERNAME.github.io/tiptapdot/privacy.html`

6. Open both links in a private browser window to confirm they load without a login.

## What to paste into Play Console

- App content, Privacy policy: the `privacy.html` URL above.
- Store listing, Contact details: `devyansh.du@gmail.com` (or a website field pointing
  at the home page).
- The store listing description can link to `support.html` if you want.

## Notes

- All internal links are relative, so the site works at any URL, including a custom
  domain later. To use a custom domain, add a `CNAME` file containing the domain and
  point the DNS record at GitHub Pages.
- Keep the site online for as long as the app is on the store. A dead privacy policy
  URL can get a listing flagged.
- If you ever add ads, analytics or online leaderboards, update `privacy.html` before
  shipping that version.
