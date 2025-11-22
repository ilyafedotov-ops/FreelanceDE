# FreelanceDE

Multilingual, long-form guides about freelancing in Germany (Markdown, CC BY-NC 4.0).

## Navigation
- English hub: [README_EN.md](README_EN.md)
- Русский: [README_RU.md](README_RU.md)

## What this project covers
- Практические гайды по регистрации Freiberufler/Gewerbe, налоги (ESt, USt/KUR, GewSt), EÜR, счёта/e-Rechnung, банки, страхование, контракты и поиск клиентов.
- Формат: чистый Markdown + изображения; без сайта/билда.
- Лицензия: CC BY-NC 4.0; не является налоговой/юридической консультацией.

## Current articles
- RU: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)
- EN: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md) (синхронизирована по структуре/содержанию).

## Latest release
- Tag: `2025.Q4`
- Notes: <https://github.com/ilyafedotov-ops/FreelanceDE/releases/tag/2025.Q4>

## Repository layout
- `articles/` — статьи и ассеты
- `articles/assets/<slug>/` — изображения статьи
- `articles/README.md` — индекс статей
- `sources/` — исходники/экспорт (docx/html)
- `CONTRIBUTING.md`, `STYLEGUIDE.md`, `CODE_OF_CONDUCT.md`, `LICENSE`

## Contributing (SSH)
1) `ssh -T git@github.com`  
2) `git clone git@github.com:ilyafedotov-ops/FreelanceDE.git`  
3) `git checkout -b article/<slug>`  
4) Добавьте/правьте Markdown в `articles/<year>/<slug>.md`, ассеты — в `articles/assets/<slug>/`.  
5) Обновите `articles/README.md` (название/дата/статус).  
6) Commit/push, откройте PR.

### TOC regeneration
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide.md`
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide-en.md`

## License
CC BY-NC 4.0. Use at your own risk; no warranty.
