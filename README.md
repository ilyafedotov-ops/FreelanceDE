# FreelanceDE

Multilingual guides about freelancing in Germany (Markdown, CC BY-NC 4.0).

## Choose your navigator
- English: [README_EN.md](README_EN.md)
- Русский: [README_RU.md](README_RU.md)

## Current article
- [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md) — freelancer/Gewerbe guide with registration, taxes, accounting (EÜR), invoicing (incl. e-invoices), tooling, banks, insurance, and contracts.

## Repository layout
- `articles/` — articles and assets
- `articles/assets/<slug>/` — per-article images
- `articles/README.md` — article index
- `sources/` — source and exported files (docx/html)
- `CONTRIBUTING.md`, `STYLEGUIDE.md`, `CODE_OF_CONDUCT.md`, `LICENSE`

## Contributing (SSH)
1. Confirm SSH access: `ssh -T git@github.com`.
2. Clone: `git clone git@github.com:ilyafedotov-ops/FreelanceDE.git`.
3. Branch: `git checkout -b article/<slug>`.
4. Add Markdown in `articles/<year>/<slug>.md`; assets under `articles/assets/<slug>/`.
5. Update `articles/README.md` with title/date/status; commit/push; open PR.

## License
CC BY-NC 4.0. Use at your own risk; no warranty.
