# Curriculum Vitae — Francesco Tosoni, PhD

Source for the academic CV of **Francesco Tosoni** (Scuola Superiore Sant'Anna /
University of Pisa). Typeset in LaTeX on top of the
[AltaCV](https://github.com/liantze/AltaCV) class.

- 🌐 Website: <https://www.francescotosoni.it>
- 📄 Latest PDFs (built by CI): <https://github.com/ftosoni/cv/releases/latest>
- 🔗 ORCID [`0000-0001-8457-3866`](https://orcid.org/0000-0001-8457-3866) ·
  [DBLP](https://dblp.org/pid/317/5120-1.html) ·
  [Google Scholar](https://scholar.google.com/citations?user=8-0w_KAAAAAJ)

## Build variants

The CV is generated in **four variants** from a single source (`main.tex`),
controlled by two flags:

| Flag | `1` | `0` (default) |
| --- | --- | --- |
| `\BUILDSHORT` | condensed CV | full CV |
| `\BUILDPHOTO` | with photo | no photo |

The `short` variant drops the more encyclopaedic sections (code artefacts,
professional internships, conference attendance, coursework lists). The
`no-photo` variant suits the anglosphere/international market where CV photos are
discouraged; the photo variant suits EU academia. Only the photo (EU) variant
ends with the self-certification under Italian DPR 445/2000 and the signature,
as needed for Italian procedures.

Four thin wrappers select the combinations:

| Wrapper | Variant |
| --- | --- |
| [`cv-full-eu.tex`](cv-full-eu.tex) | full, with photo |
| [`cv-full-intl.tex`](cv-full-intl.tex) | full, no photo |
| [`cv-short-eu.tex`](cv-short-eu.tex) | short, with photo |
| [`cv-short-intl.tex`](cv-short-intl.tex) | short, no photo |

## Building the PDF

The document **must** be compiled with **XeLaTeX** (or LuaLaTeX): it uses
`fontspec` with the Lato font and the `fontawesome5` / `academicons` icon
packages, which require a Unicode engine.

Build the default (full, with photo):

```bash
latexmk -xelatex main.tex
```

Build a specific variant via its wrapper:

```bash
latexmk -xelatex cv-short-intl.tex
```

`latexmk` runs Biber automatically. To compile by hand, run
`xelatex → biber → xelatex → xelatex` on the chosen root file.

### Requirements

- A recent TeX distribution (TeX Live 2020+ or MiKTeX) with:
  `altacv` dependencies, `fontspec`, `paracol`, `enumitem`, `fontawesome5`,
  `academicons`, `tikz`, `wrapfig`, `adjustbox`, `hyperref`, `eurosym`,
  `biblatex` + `biber`.
- The **Lato** font (TeX Live `lato` package).
- A Devanagari font for the one Hindi label: **Mangal** (bundled with Windows)
  or **Noto Sans Devanagari**. The preamble auto-detects these and degrades
  gracefully to a no-op if neither is present, so the build never fails on this.

MiKTeX offers to install any missing packages on first compilation.

## Repository layout

| Path | Purpose |
| --- | --- |
| [`main.tex`](main.tex) | The CV source (the file you edit). |
| `cv-{full,short}-{eu,intl}.tex` | One-line wrappers selecting a build variant. |
| `altacv.cls` | The AltaCV document class (upstream). |
| `sample.bib` | Bibliography database loaded via `biblatex`. |
| `photo.jpeg`, `signature.pdf`, `unipi-logo.png`, … | Images used in the CV. |
| `old.tex` | A previous draft, kept for reference. |
| `.github/workflows/build-cv.yml` | CI that builds all four variants (see below). |

No PDF is version-controlled: `main.pdf` and the variant PDFs are git-ignored
and produced by CI (see below).

## Continuous integration

[`.github/workflows/build-cv.yml`](.github/workflows/build-cv.yml) recompiles the
CV on every push/PR that touches the sources (and on demand via *Run workflow*).
A build **matrix** compiles all four variants in parallel on a full TeX Live
image; a broken source fails the check. Each variant's PDF is uploaded as an
artifact, and on `main` all four are attached to a rolling **`latest`** GitHub
Release, e.g.:

```
https://github.com/ftosoni/cv/releases/latest/download/cv-full-eu.pdf
https://github.com/ftosoni/cv/releases/latest/download/cv-short-intl.pdf
```

## Publications & talks

Publication and talk entries mirror the canonical lists maintained on
<https://www.francescotosoni.it> (`publications.html`, `talks.html`). Each entry
carries the full set of links (DOI, arXiv, author PDF, Wikidata, code, data,
SWHID, erratum, licence) as compact icon "pills"; a legend under *Publications*
explains the icons. Publications use DBLP-style keys — `jN` journal, `cN`
conference, `wN` working paper — consistent with the website.

## Colours & accessibility

The palette uses a deep-crimson accent (`#A6172D`, ~7.5:1 contrast on white,
WCAG 2.1 AAA for normal text). Hyperlinks share the accent colour, and the
"Research Focus" skill tags use solid accent fills with white text for a legible
contrast ratio.

## Credits & licence

Built on **AltaCV** v1.2 by Lian Tze Lim, distributed under the
[LaTeX Project Public License (LPPL) v1.3c](http://www.latex-project.org/lppl.txt).
The AltaCV class file retains its original licence.

The CV **content** (text, images, and personal data in `main.tex` and the bundled
images) is © Francesco Tosoni and is not covered by the LPPL.
