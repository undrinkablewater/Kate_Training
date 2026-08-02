# The Long Emergency

**Jihadist terrorism in Australia, 2001–2026 — a reader's guide.**

A single-file HTML long read in eleven modules plus a reference appendix, written for
readers starting from zero. Roughly 26,000 words; 12–17 minutes per module.

## Contents

| # | Module | Read |
|---|--------|------|
| 01 | Before the Beginning — Australia, Islam, and the world before 2001 | 15 min |
| 02 | The First Wave, 2001–2006 — Brigitte, Lodhi, Operation Pendennis | 12 min |
| 03 | The Milieu, Part One — suburbs, mosques, bookshops, preachers | 12 min |
| 04 | The Quiet Years, 2007–2013 — Holsworthy, prison, the road to Syria | 13 min |
| 05 | Exodus — Australians in the Islamic State | 12 min |
| 06 | The Home Front, 2014–2015 — Haider, the Lindt Café, Curtis Cheng | 13 min |
| 07 | The Grind, 2016–2019 — Minto, Melbourne, Brighton, the plane plot | 12 min |
| 08 | The Milieu, Part Two — after the caliphate | 13 min |
| 09 | Fracture, 2023–2026 — Wakeley, the synagogue fires, Bondi Beach | 17 min |
| 10 | The Ideas, in Brief — a short primer | 9 min |
| 11 | Patterns and Arguments | 13 min |
| ★ | Reference — timeline, glossary, cast, further reading | look-up |

## Publishing

`index.html` is fully self-contained. No build step, no dependencies, no external
requests of any kind — no CDNs, no web fonts, no analytics, no trackers. Drop the
repository on any static host and it works.

**GitHub Pages:** push to a repository, then *Settings → Pages → Source: Deploy from
a branch → `main` / `(root)`*. The page will be served at
`https://<user>.github.io/<repo>/`.

`.nojekyll` is included so GitHub serves the files verbatim.

### Before you publish

Two fields in `<head>` are intentionally left blank. Fill them in or delete them:

```html
<meta name="author" content="">
<link rel="canonical" href="">
```

For rich link previews on social platforms, add a 1200×630 image and reference it:

```html
<meta property="og:image" content="https://example.com/preview.png">
<meta property="og:url" content="https://example.com/">
```

## Technical notes

- Mobile-first; one module displayed at a time with previous/next navigation.
- Light and dark themes, following the system preference by default, with a manual
  toggle. Browser chrome colour tracks the theme.
- Reading position is remembered in `localStorage` and offered as "Resume" on the
  cover. Degrades silently if storage is unavailable.
- Keyboard navigation: `←` / `→` between modules, `Esc` closes the contents drawer.
- Four original inline SVG figures. No photographs — see below.
- Prints as a single continuous document (all modules expand, chrome hidden).
- System font stacks only, so it renders offline and instantly.

## Sourcing and editorial standards

Compiled from open sources: court judgments and sentencing remarks, coronial
inquests, ASIO and AFP public statements, parliamentary material, and reporting by
the ABC, the *Sydney Morning Herald*, *The Age*, *The Australian*, the *Guardian*,
SBS and the BBC, together with academic and think-tank analysis.

Editorial rules applied throughout:

- Every individual is tagged by legal status — **convicted**, **acquitted**,
  **killed**, **never charged**, or **before the courts**.
- People who have never been charged with an offence are explicitly identified as
  such, every time they appear.
- Civil findings are distinguished from criminal convictions.
- Matters currently before the courts carry an express statement that no finding of
  guilt should be inferred.
- Contested questions are described as disputes rather than resolved.

Modules 3, 8 and 9 open with content or legal cautions.

## Images

The piece contains no photographs. It uses original inline SVG artwork and
typographic profile cards instead. This keeps the file self-contained, portable and
free of third-party licensing risk. If you want to add photographs, the profile card
markup (`.person` / `.mono`) is straightforward to extend with an `<img>`.

## Corrections

This is a compilation from open sources covering twenty-five years and several
hundred people. It will contain errors. Corrections are welcome via issues.

## Licence

Not yet specified. Add a `LICENSE` file before publishing if you want to set terms
for reuse.

---

*Last updated: August 2026.*
