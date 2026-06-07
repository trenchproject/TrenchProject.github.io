# TrEnCh Project — GitHub Pages site (Millennial Jekyll theme)


### 2. Custom domain (optional)

To keep the `www.trenchproject.com` domain, add a file named `CNAME` in the
repo root containing just:

```
www.trenchproject.com
```

then point your DNS at GitHub Pages per
[GitHub's custom-domain docs](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).

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

3. Hero background images (home, butterfly, grasshopper, about) are set inline in
   each page's `<section class="trench-hero" style="background-image:…">`. Add the
   referenced files (`home-hero.jpg`, `gothic2.jpg`, `Grasshopper.jpg`,
   `GrasshopperIR.jpg`) to `assets/img/`, or edit/remove the `style` attribute to
   use a plain colored gradient.

---

## Things to review / finish

- **Outbound tool links (Tools page):** Several "GitHub Repository" / "Dryad
  Repository" mentions on the original were plain text; add real URLs where you
  have them.

- **Instagram feed:** The original embedded a live Instagram feed. GitHub Pages
  is static, so this was omitted. You can add an embed widget (e.g. SnapWidget /
  LightWidget) into the relevant pages if desired.

---

## Credits

- Theme: [Millennial](https://github.com/LeNPaul/Millennial) by Paul Le (MIT License).
- Original site content © TrEnCh Project; original design by
  [Impact Media Lab](https://www.impactmedialab.com/).
