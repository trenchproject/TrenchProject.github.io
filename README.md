# TrEnCh Project — GitHub Pages site (Millennial Jekyll theme)

This is a [Jekyll](https://jekyllrb.com/) site that recreates
[trenchproject.com](https://www.trenchproject.com/) using the
[Millennial theme](https://github.com/LeNPaul/Millennial), ready to host for free
on [GitHub Pages](https://pages.github.com/). Images are referenced as **labeled
placeholders** so you can drop in your own copies (see [Adding images](#adding-images)).

---

## Quick start

### 1. Create the repository

For a project site at `https://<user>.github.io/trenchproject/`:

```bash
# from inside this folder
git init
git add .
git commit -m "Initial TrEnCh Project site on Millennial theme"
git branch -M main
git remote add origin https://github.com/<user>/trenchproject.git
git push -u origin main
```

Then in the repo: **Settings → Pages → Build and deployment → Source: Deploy from
a branch → Branch: `main` / `/ (root)`**.

> **baseurl:** If you publish to `https://<user>.github.io/trenchproject/`
> (a *project* page), open `_config.yml` and set `baseurl: "/trenchproject"`.
> If you use an **organization/user page** (`https://<user>.github.io/`) or a
> **custom domain** (e.g. `www.trenchproject.com`), leave `baseurl: ""`.

### 2. Custom domain (optional)

To keep the `www.trenchproject.com` domain, add a file named `CNAME` in the
repo root containing just:

```
www.trenchproject.com
```

then point your DNS at GitHub Pages per
[GitHub's custom-domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

---

## Running locally

You need Ruby (3.x) and Bundler.

```bash
bundle install
bundle exec jekyll serve
# open http://127.0.0.1:4000
```

The included `Gemfile` uses the `github-pages` gem so your local build matches
what GitHub Pages produces. (If you prefer a plain modern Jekyll instead, you can
replace the `github-pages` line with `gem "jekyll", "~> 4.2"`.)

---

## Site structure

```
.
├── _config.yml                 # Site settings (title, baseurl, plugins)
├── _data/settings.yml          # Menu items + social links
├── _includes/
│   ├── header.html             # Top nav (built from settings.yml menu)
│   ├── footer.html             # TrEnCh footer (text nav + social + credit)
│   ├── head.html               # <head>, fonts, SEO
│   └── img.html                # Image-placeholder helper (see below)
├── _layouts/
│   ├── default.html            # Page shell (header + content + footer)
│   ├── trench-page.html        # Wide layout used by all content pages
│   ├── page.html               # Simple page layout (from theme)
│   └── post.html               # Blog/news post layout
├── _posts/                     # News posts (Latest News)
│   └── 2020-10-16-new-visualizations-in-trench-ed.md
├── _sass/
│   └── _trench.scss            # All custom TrEnCh styling (heroes, grids, cards…)
├── assets/
│   ├── css/main.scss           # Theme stylesheet entry point
│   └── img/                    # ← put your images here
├── pages/
│   ├── the-science.html
│   ├── intro-to-biophysical-modeling.html   # redirects to /the-science
│   ├── infrared-modeling.html
│   ├── case-studies.html
│   ├── butterfly.html
│   ├── grasshopper.html
│   ├── tools.html
│   ├── about.html
│   └── latest-news.html
└── index.html                  # Home page
```

### Navigation & social links

Edit `_data/settings.yml` to change the top menu or social icons. The header and
footer are generated from this file.

---

## Adding images

Every image on the site is currently rendered as a dashed placeholder box that
shows the expected **filename**, e.g. `[IMAGE: ColiasModel2.png — Colias modeling framework]`.

1. Drop your image files into `assets/img/` using the **exact filenames** listed
   in [`IMAGE_MANIFEST.md`](IMAGE_MANIFEST.md).
2. Open `_includes/img.html` and switch the placeholder for a real `<img>` tag.
   The file already contains the one-line replacement in a comment — just
   uncomment/replace the placeholder `<div>` with:

   ```liquid
   <img src="{{ site.github.url }}/assets/img/{{ include.file }}" alt="{{ include.alt }}">
   ```

   That single change turns **all** placeholders across the site into real images
   (as long as the filenames match).

3. Hero background images (home, butterfly, grasshopper, about) are set inline in
   each page's `<section class="trench-hero" style="background-image:…">`. Add the
   referenced files (`home-hero.jpg`, `gothic2.jpg`, `Grasshopper.jpg`,
   `GrasshopperIR.jpg`) to `assets/img/`, or edit/remove the `style` attribute to
   use a plain colored gradient.

---

## Things to review / finish

- **Contact form (About page):** GitHub Pages cannot process form submissions.
  The community sign-up form's `action="#"` is a stub. Wire it to a service such
  as [Formspree](https://formspree.io/) or a Google Form.
- **Outbound tool links (Tools page):** Several "GitHub Repository" / "Dryad
  Repository" mentions on the original were plain text; add real URLs where you
  have them.
- **Latest News:** Contains the single original post (Oct 16 2020) as a stub.
  Add the full body and any further posts in `_posts/` using the
  `YYYY-MM-DD-title.md` naming convention.
- **Instagram feed:** The original embedded a live Instagram feed. GitHub Pages
  is static, so this was omitted. You can add an embed widget (e.g. SnapWidget /
  LightWidget) into the relevant pages if desired.

---

## Credits

- Theme: [Millennial](https://github.com/LeNPaul/Millennial) by Paul Le (MIT License).
- Original site content © TrEnCh Project; original design by
  [Impact Media Lab](https://www.impactmedialab.com/).
