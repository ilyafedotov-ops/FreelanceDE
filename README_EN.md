# FreelanceDE — English README

[Русская версия](README_RU.md) | [Home](README.md)

FreelanceDE is a practical content project about freelancing and Gewerbe in Germany. The main format is Markdown articles with images, plus HTML/DOCX exports for publishing and migration.

There is no application and no build step. This repository stores articles, assets, sources, exports, and related media.

## Start Here

- Main English guide: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md)
- Russian version: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)
- Article index: [articles/README.md](articles/README.md)
- Blog/WordPress HTML version: [blog/freelance-guide.ru.html](blog/freelance-guide.ru.html)

## What the Main Guide Covers

- Freiberufler vs Gewerbe;
- registration with Finanzamt, ELSTER, and Gewerbeamt;
- Einkommensteuer, Umsatzsteuer, Kleinunternehmerregelung, Gewerbesteuer;
- EÜR and annual tax filing;
- filing forms by status: Freiberufler, Gewerbe, Kleinunternehmer, employment plus side gig;
- invoices, e-Rechnung, Reverse Charge, and international clients;
- business bank accounts, payment providers, and accounting tools;
- health, pension, professional liability, and other insurance topics;
- contracts, Scheinselbständigkeit, client acquisition, and rate calculation;
- self-employed side gigs;
- freelance visa basics and official resources.

## Current Status

The main guide was refreshed on `02.05.2026`. The latest update checked and refreshed:

- 2026 Grundfreibetrag and Einkommensteuer brackets;
- Kinderfreibetrag;
- Kleinunternehmerregelung limits;
- Umsatzsteuer-Voranmeldung thresholds;
- annual filing deadlines;
- GKV, Pflegeversicherung, Rentenversicherung, and JAEG figures;
- sections on insurance for foreigners, freelance visas, resources, and communities.

Older release notes may still reference `2025.Q4`; for content accuracy, use the article changelog as the closest source of truth.

## Important

The content is educational and practical. It is not tax, legal, accounting, or immigration advice.

Before filing documents or making decisions, verify current requirements with official sources, Finanzamt, Ausländerbehörde, Krankenkasse, or a qualified Steuerberater.

## Repository Layout

```text
articles/
  2025/
    freelancer-gewerbe-guide.md       Russian Markdown guide
    freelancer-gewerbe-guide-en.md    English Markdown guide
  assets/
    freelancer-gewerbe-guide/         Images used by the guide
  README.md                           Article index

blog/
  freelance-guide.ru.html             WordPress-style HTML version of the Russian guide

sources/
  freelanceguide.html                 Source/export copy
  freelancer_gewerbe_guide_v0.5.docx  DOCX source/export

podcasts/
  FreelancerDE-Podcast-*.mp4          Related podcast/video files
```

## Editing Workflow

For normal content updates:

1. Update [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md) first.
2. If the topic exists in both languages, mirror the change in [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md).
3. Update the changelog near the top of the relevant article.
4. If the public HTML page must match, update [blog/freelance-guide.ru.html](blog/freelance-guide.ru.html).
5. Update files in [sources/](sources/) only when intentionally refreshing source/export versions.

For tax, insurance, and visa updates, check official sources first: BMF, ELSTER, BMG, DRV, Bundesagentur für Arbeit, Make it in Germany, Berlin LEA, IHK, BZSt, and current law texts.

## Useful Checks

```bash
# Find old or suspicious values
rg -n "2024|2025|12 096|10 096|450 евро|€450|bmf-steuerrechner.de/ekst" articles/2025 blog

# Check HTML internal anchors
node - <<'NODE'
const fs = require('fs');
const html = fs.readFileSync('blog/freelance-guide.ru.html', 'utf8');
const ids = new Set([...html.matchAll(/\bid=["']([^"']+)["']/g)].map(m => m[1]));
const hrefs = [...html.matchAll(/href=["']#([^"']+)["']/g)].map(m => m[1]);
const missing = [...new Set(hrefs.filter(h => !ids.has(h)))];
console.log({ internalLinks: hrefs.length, missing: missing.length });
if (missing.length) console.log(missing.join('\n'));
NODE

# Check HTML warnings
tidy -utf8 -qe blog/freelance-guide.ru.html
```

`tidy` may report legacy warnings from WordPress/Word HTML: missing doctype, old generated IDs, missing image alt text, or nested emphasis. Treat malformed links, broken anchors, and new structural issues as problems.

## Contributing

```bash
git clone git@github.com:ilyafedotov-ops/FreelanceDE.git
cd FreelanceDE
git checkout -b article/<slug>
```

Then edit the relevant files, check links/anchors, commit/push, and open a pull request.

## License

CC BY-NC 4.0. Use at your own risk; no warranty.
