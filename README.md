# FreelanceDE

Multilingual, long-form guides about freelancing in Germany (Markdown, CC BY-NC 4.0). English first, Russian below.

## English
**Scope:** Practical guides for Freiberufler/Gewerbe: registration, taxes (ESt, USt/KUR, GewSt), EÜR, invoicing/e-invoicing, banks, insurance, contracts, finding clients. Markdown + images; no build/site. Not tax/legal advice.

**Who/why:** Written for newcomers and practicing freelancers in Germany who want a single, printable, reference-style guide (no SaaS). Emphasis on norms/§ references where helpful and plain-language explanations.

**Freshness:** Current release `2025.Q4`. Tax thresholds/links are kept in the article changelog; always verify against primary sources (BMF, UStG/EStG, GewStG, IHK/BZSt).

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

**How to use:**  
- Read directly in GitHub or Markdown viewer; export from `sources/` if you need docx/html.  
- Copy/paste snippets for checklists/templates; adapt to your case and confirm locally relevant rules (Finanzamt/IHK/Gemeinde).  
- Track changes via `articles/*/Список изменений` / `Changelog` tables and release notes.

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

**Кому и зачем:** Для новичков и практикующих фрилансеров в Германии, которым нужен один референс без веб-сервиса. Делается упор на понятные объяснения и ссылки на нормы там, где это полезно.

**Актуальность:** Текущий релиз `2025.Q4`. Пороговые значения и ссылки фиксируются в changelog статьи; при сомнениях сверяйтесь с первоисточниками (BMF, UStG/EStG, GewStG, IHK/BZSt).

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

**Как использовать:**  
- Читайте прямо на GitHub или в Markdown-ридере; docx/html — в `sources/`.  
- Копируйте чек-листы/шаблоны под свою ситуацию и сверяйте с локальными правилами (Finanzamt/IHK/Gemeinde).  
- Отслеживайте изменения через `Список изменений` в статье и релизные заметки.

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
