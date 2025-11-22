# FreelanceDE

Multilingual, long-form guides about freelancing in Germany (Markdown, CC BY-NC 4.0). English first, Russian below.

## English
**Scope:** Practical guides for Freiberufler/Gewerbe: registration, taxes (ESt, USt/KUR, GewSt), EÜR, invoicing/e-invoicing, banks, insurance, contracts, finding clients. Markdown + images; no build/site. Not tax/legal advice.

**Navigation:**  
- EN hub: [README_EN.md](README_EN.md)  
- RU hub: [README_RU.md](README_RU.md)

**Current articles:**  
- EN: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md)  
- RU: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)

**Latest release:** `2025.Q4` — notes: <https://github.com/ilyafedotov-ops/FreelanceDE/releases/tag/2025.Q4>

**Repo layout:**  
- `articles/` — articles and assets  
- `articles/assets/<slug>/` — images per article  
- `articles/README.md` — article index  
- `sources/` — source/exports (docx/html)  
- `CONTRIBUTING.md`, `STYLEGUIDE.md`, `CODE_OF_CONDUCT.md`, `LICENSE`

**Contributing (SSH):**  
1) `ssh -T git@github.com`  
2) `git clone git@github.com:ilyafedotov-ops/FreelanceDE.git`  
3) `git checkout -b article/<slug>`  
4) Edit `articles/<year>/<slug>.md`; assets under `articles/assets/<slug>/`  
5) Update `articles/README.md` (title/date/status)  
6) Commit/push; open PR.

**TOC regeneration:**  
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide.md`  
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide-en.md`

## По-русски
**О чём:** Практические гайды для Freiberufler/Gewerbe: регистрация, налоги (ESt, USt/KUR, GewSt), EÜR, счёта/e-Rechnung, банки, страховки, контракты и поиск клиентов. Формат: Markdown + картинки; это не налоговая/юрд консультация.

**Навигация:**  
- Английский: [README_EN.md](README_EN.md)  
- Русский: [README_RU.md](README_RU.md)

**Текущие статьи:**  
- RU: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)  
- EN: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md)

**Последний релиз:** `2025.Q4` — заметки: <https://github.com/ilyafedotov-ops/FreelanceDE/releases/tag/2025.Q4>

**Структура:**  
- `articles/` — статьи и ассеты  
- `articles/assets/<slug>/` — изображения статьи  
- `articles/README.md` — индекс статей  
- `sources/` — исходники/экспорт (docx/html)  
- `CONTRIBUTING.md`, `STYLEGUIDE.md`, `CODE_OF_CONDUCT.md`, `LICENSE`

**Как внести вклад (SSH):**  
1) `ssh -T git@github.com`  
2) `git clone git@github.com:ilyafedotov-ops/FreelanceDE.git`  
3) `git checkout -b article/<slug>`  
4) Правьте `articles/<year>/<slug>.md`, ассеты — в `articles/assets/<slug>/`  
5) Обновите `articles/README.md` (название/дата/статус)  
6) Commit/push; создайте PR.

**Перегенерация оглавления:**  
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide.md`  
- `npx markdown-toc -i articles/2025/freelancer-gewerbe-guide-en.md`

## License / Лицензия
CC BY-NC 4.0. Use at your own risk; no warranty. / Использование на свой страх и риск, без гарантий.
