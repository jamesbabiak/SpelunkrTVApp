# Spelunkr TV — App Support Website (GitHub Pages)

This is a **ready-to-upload static website** for Spelunkr TV app support and privacy. No coding, custom domain, or build tools are required. It contains **no scripts, tracking pixels, advertising, or web forms**.

## What to upload

Upload these files and folders **at the repository root** (not inside an extra folder):

- `index.html` — home / support landing page
- `support.html` — help and contact
- `privacy.html` — privacy policy
- `styles.css` — retro theme
- `assets/` — Spelunkr S artwork and favicon
- `.nojekyll` — keeps this as a plain static site

`README.md` and `TVOS_PRIVACY_TEXT.txt` are development/helper files. You may include them in the GitHub repository; they do not affect the website.

## Publish using only the GitHub website

1. Sign into https://github.com and click **+** → **New repository**.
2. Repository name: `spelunkr-tv-support` (recommended, but any name works).
3. Set visibility to **Public** (free GitHub Pages works with public repositories).
4. Do **not** initialize with a README; click **Create repository**.
5. On the empty repo page, select **uploading an existing file** (or **Add file → Upload files**).
6. Open this extracted ZIP in Finder. Drag **the files and `assets` folder inside it**, *not the enclosing site folder*, into the GitHub upload area. Be sure `index.html` and `assets/` appear in the root.
7. Click **Commit changes**.
8. In the repository, go to **Settings → Pages**.
9. Under **Build and deployment**, set **Source** to `Deploy from a branch`.
10. Choose branch `main` and folder `/(root)`, then **Save**.
11. After GitHub publishes it, the Pages settings screen shows the live website URL. Open that URL and click **Support** and **Privacy** to verify both pages work. Deployment may take a few minutes.

> GitHub Pages URL usually looks like: `https://YOUR-GITHUB-USERNAME.github.io/spelunkr-tv-support/`.
> This is **an example pattern**, not your actual URL; use the address shown by GitHub in Settings → Pages.

## Where to enter links in App Store Connect

After the site is actually live, use:

- **Support URL (both platforms):** `YOUR-LIVE-PAGES-URL/support.html`
- **Privacy Policy URL (iOS):** `YOUR-LIVE-PAGES-URL/privacy.html`
- **Apple TV Privacy Policy text (tvOS):** copy the full contents of `TVOS_PRIVACY_TEXT.txt` into App Store Connect's tvOS privacy text field.
- **Marketing URL (optional):** `YOUR-LIVE-PAGES-URL/` or leave it empty.

If GitHub provides a URL ending in `/`, add `support.html` or `privacy.html` immediately after that slash.

### Notes

- Website contact email is **support@routed.com**.
- The site credits the **original Spelunkr creator** and the **Internet Archive**; it does not personally name the independent app developer.
- This package does not modify any app source files or targets.
- Review the privacy text if you later add analytics, accounts, crash reporting SDKs, advertising, or new third-party services.
- The site uses relative links so it works from project-based GitHub Pages URLs without requiring you to edit any HTML.
- If your account already owns a repository named `spelunkr-tv-support`, choose another repository name; the pages still work unchanged.
