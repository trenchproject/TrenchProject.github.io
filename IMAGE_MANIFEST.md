# Image manifest

Every image referenced by the site, grouped by page. Place files in `assets/img/` using these **exact filenames** (or rename references in the page files to match your own filenames). Most names mirror the originals from trenchproject.com; a few were given clean slugs where the original used spaces or ambiguous names — those are flagged with a note.

After adding files, follow [README → Adding images](README.md#adding-images) to swap the placeholders for real `<img>` tags in one edit.

## Hero background images (set inline per page)

| File | Page |
|----|----|
| `home-hero.jpg` | Home hero (new slug — pick any landscape/banner image) |
| `gothic2.jpg` | Butterfly hero |
| `Grasshopper.jpg` | Grasshopper hero |
| `GrasshopperIR.jpg` | About hero |

## Home (`index.html`)

| File                  | Note                                       |
|-----------------------|--------------------------------------------|
| `butterflyscale.webp` | Colias project-highlight image (slug)      |
| `ghop.webp`           | Grasshopper project-highlight image (slug) |

## The Science (`pages/the-science.html`)

| File                      | Note                                          |
|---------------------------|-----------------------------------------------|
| `iguana.webp`             | Thermal image of basking marine iguana (slug) |
| `FLIRmusselseastar3.webp` | Intertidal sea star & mussels (slug)          |
| `ModStep1.webp`           | Step 1 diagram                                |
| ``` ModStep2.``webp ```   | Step 2 diagram                                |
| ``` ModStep3.``webp ```   | Step 3 diagram                                |
| `vizualizations.gif`      | Visualization demo                            |

## Infrared Imagery (`pages/infrared-modeling.html`)

| File               | Note                                        |
|--------------------|---------------------------------------------|
| ThermalImages.png  | "Real-time thermal conditions" image (slug) |
| ThermalImages2.png | "Thermal processes" image (slug)            |

## Butterfly (`pages/butterfly.html`)

| File | Note |
|----|----|
| `colias.webp` | Museum specimens of *Colias meadii* (slug) |
| `gothic1_gothicmtn&lab-1969.webp` | Watt RMBL photo |
| `gothic2_butterflyhunters-1974.webp` | Watt RMBL photo |
| `gothic3_1963_08-26+dad+on+mt+tilton.webp` | Watt RMBL photo (orig. had `&`) |
| `gothic4_1966_08-26+travelall_SM.webp` | Watt RMBL photo |
| `ColiasModel2.webp` | Modeling-framework diagram |
| `BIISchematic.webp` | Reaction-norm figure |
| `ColiasAbsMap.webp` | 2040 absorptivity projection map |
| `butterfly_gradient.webp` | Findings icon (used 3×) |

## Grasshopper (`pages/grasshopper.html`)

| File | Note |
|----|----|
| `bust.jpg` | Bust of Gordon Alexander |
| `2019-Niwot-Ridge.jpg` | Historical photo (orig. had space) |
| `2026-FrontRange.png` | Historical photo |
| `3006-Chautauqua-Mesa.jpg` | Historical photo (orig. had space) |
| `2676-J-Hilliard-Mrs-A.jpg` | Historical photo (orig. had spaces & `&`) |
| `field.jpg` | Field survey photo |
| `field2.jpg` | Field survey photo |
| `grasshopper.jpg` | Grasshopper field photo |
| `RoL.png` | Genomic clines / thermal specialization figure |
| `grasshopperphen.jpg` | Development index figure |
| `grasshopper_white.png` | Findings icon (used 3×) |

## Tools (`pages/tools.html`)

| File                             | Note                          |
|----------------------------------|-------------------------------|
| `TRENCH_Logo_Circle-TrenchR.png` | TrenchR logo                  |
| `vizualizations.gif`             | Visualizations                |
| `Laptop-scroll_5.gif`            | Laptop demo (orig. had space) |
| `tablet.png`                     | Tablet demo                   |
| `phone.gif`                      | Phone demo                    |

## About (`pages/about.html`)

| File                       | Note                                       |
|----------------------------|--------------------------------------------|
| `lauren-buckley.jpg`       | Team portrait (slug)                       |
| `issac-caruso.jpg`         | Team portrait (slug)                       |
| `yutaro-sakairi.jpg`       | Team portrait (slug)                       |
| `abby-meyer.jpg`           | Team portrait (slug)                       |
| `joel-kingsolver.jpg`      | Team portrait (slug)                       |
| `mike-kearney.jpg`         | Team portrait (slug)                       |
| `ray-huey.jpg`             | Team portrait (slug)                       |
| `tony-cannistra.jpg`       | Team portrait (slug)                       |
| `ofir-levy.jpg`            | Team portrait (slug)                       |
| `aji-john.jpg`             | Team portrait (slug)                       |
| `bryan-briones-ortiz.jpg`  | Team portrait (slug)                       |
| `ThermoNiche.jpg`          | Partner: NicheMapR                         |
| `thermimagesticker1-1.png` | Partner: Thermimage                        |
| `EFI_Logo-1.jpg`           | Partner: Ecological Forecasting Initiative |
| `PEcAn.jpg`                | Partner: PEcAn project                     |

## Latest News (`_posts/…`)

| File          | Note                                                 |
|---------------|------------------------------------------------------|
| `image_5.jpg` | Thumbnail for "New visualizations in TrEnCh-Ed" post |

------------------------------------------------------------------------

### Team portrait filenames

The original site served portraits with non-descriptive Squarespace filenames, so clean slugs were used here (`firstname-lastname.jpg`). Either name your portrait files to match, or edit the `file="…"` values in `pages/about.html`.
