# Sarah Drain — Academic Website (GitHub Pages Ready)

A standalone, 6-page academic website based on the structure of the provided Mustahsin Aziz website, redesigned with midnight-navy backgrounds and blue accents. Sarah's professional information is taken from her **October 2026 CV**. The site runs with plain HTML, CSS, and JavaScript: **no Jekyll theme, Node.js, dependencies, package installation, or build step required.**

## Website pages

- `index.html` — Home, profile, highlights
- `portfolio.html` — Research, job market paper, publications, working papers, UrbanEye
- `contact.html` — Teaching (filename retained from original site)
- `about.html` — Background, experience, photo gallery
- `blogs.html` — Outreach / activities (filename retained from original site)
- `cv.html` — Embedded/downloadable PDF CV

## Change the photos (REPLACE THESE EXACT FILES)

All picture files are placeholder artwork, not personal photographs. When you have final images, name them **exactly** as below and put them inside `images/`, replacing the existing JPEGs:

| File | Where shown | Image suggestion |
| --- | --- | --- |
| `images/profile.jpg` | Circular portrait, homepage | Square headshot, at least 600×600 pixels |
| `images/hero.jpg` | Large background of homepage | Wide 16:9 landscape or campus image, ideally 1600×900+ |
| `images/gallery-01.jpg` to `images/gallery-06.jpg` | Six tiles on About page | Photos from research, travel, campus or professional activities; 4:3 ideal |

The About page photo captions currently say "Photo # · Replace ...". Edit those `<figcaption>` lines in `about.html` to real captions when pictures are added. Update the `<img alt="...">` descriptions as well. You can remove the gallery intro placeholder sentence in `about.html` after replacement.

Photos should be web optimized (for example 100–400 KB for portraits/gallery and 200–600 KB for the cover) so the site loads quickly. **Do not reuse Mustahsin's photographs without permission.**

## Update the CV

Replace `documents/Sarah_Drain_CV.pdf` with a newer PDF of the **same filename**. No HTML changes are necessary.

## How to change content and theme

- Name/email: search `Sarah Drain` / `sarah.drain@mail.wvu.edu` in the six `.html` files. The email address and profile fields come from the attached CV.
- Publications: edit `portfolio.html`; only the peer-reviewed publication has a live DOI link. Unpublished papers intentionally have descriptions instead of fake PDF links.
- Add social profiles: add actual, confirmed URL links to `index.html` or the footer in the HTML pages. None were supplied, so none have been invented.
- Colors: edit variables at the top of `assets/styles.css`. Key variables: `--bg`, `--surface`, `--accent`, `--accent2`, `--text`, `--muted`.
- Navigation labels/links: update `header()` output directly in **each** `.html` file; currently the site is fully static and intentionally has no templating dependency.
- To make a new page, copy an existing `.html` file, edit the title, main content, and navigation as appropriate.

## Preview the site on your computer (before GitHub)

1. Unzip the file.
2. Open the `SarahDrain_Academic_Website` folder.
3. Double-click `index.html`. It will open in your web browser.
4. Follow the website's navigation links. The CV PDF and all image placeholders are included.

If images or layout do not refresh after editing, press `Ctrl + Shift + R` in your browser.

## Publish as a personal GitHub Pages website

**Important: GitHub does NOT publish the .zip itself. You need to unzip it and upload the files INSIDE the website folder.**

1. Sign in to https://github.com as the person who should own the website.
2. Click the `+` menu (top right) and choose **New repository** (or visit https://github.com/new).
3. Enter `<username>.github.io` for the repository name, replacing `<username>` with that GitHub account's exact username (lowercase). Example: username `sarahdrain` → repository name `sarahdrain.github.io`.
4. Choose **Public**; click **Create repository**. The site repository can start empty.
5. On the new repository's **Code** tab, choose **Add file → Upload files**. If that menu is not visible in an empty repository, use its **uploading an existing file** link.
6. On your computer, open the **extracted** website folder. Select **all files and folders inside it** (`index.html`, `cv.html`, `portfolio.html`, `about.html`, `contact.html`, `blogs.html`, `assets`, `images`, `documents`, etc.). Drag those items into GitHub's upload area. Do **not** upload just the outer folder and do **not** upload the ZIP. `index.html` must be at the repository top level, not nested under another folder.
7. Once uploads finish, scroll down. Enter a commit message like `Add Sarah Drain website` and click **Commit changes** / **Propose changes** (wording may vary).
8. In your repository, select **Settings → Pages** from the left sidebar (under Code and automation).
9. Under **Build and deployment → Source**, choose **Deploy from a branch**. Under **Branch**, select `main` and `/(root)`, then **Save**.
10. Once GitHub publishes it, use **Settings → Pages → Visit site** or open `https://<username>.github.io/`. Initial publication may take a few minutes (GitHub documents up to about 10 minutes).
11. Test Home, Research, Teaching, About, Outreach, and CV links. If you see a 404 error, verify that the repo is named `username.github.io`, Pages uses `main` + `/(root)`, and `index.html` is at the repository root.

If the owner already has a repository called `<username>.github.io`, **use the existing repository** instead. Upload this site's files to that repository, removing obsolete files as appropriate, rather than creating a second personal-site repository. Be careful: replacing files changes the currently published site.

### Updating the live site later

Open the repository on GitHub, select **Add file → Upload files**, add modified files, and commit the change. For a single text edit, select the HTML file, click the pencil **Edit** icon, make changes, and **Commit changes**. GitHub Pages republishes the changes automatically.

### Known caveats

- This site is public once published. The CV PDF and listed email address are publicly accessible. Decide if you wish to omit contact details from the public CV.
- The uploaded CV says **October 2026** and an expected **May 2027** Ph.D. completion. Review these details as they evolve.
- Paper PDF links were **not** invented. Add public papers yourself once available.
- The About-page personal photographs are placeholders. No personally specific non-CV information, such as hobbies, was invented.
- File `contact.html` is intentionally the Teaching page, consistent with the original site's existing filenames. `blogs.html` is intentionally Outreach.

GitHub documentation:
https://docs.github.com/en/pages/quickstart
https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
