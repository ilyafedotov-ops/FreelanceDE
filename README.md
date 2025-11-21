# FreelanceDE

Articles and guides about freelancing in Germany. All content lives in Markdown and is licensed under CC BY-NC 4.0.

## Current article: Freelancer Gewerbe Guide
- File: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)
- License: CC BY-NC 4.0; use at your own risk.

### Summary (EN)
Practical guide to registering and working as a freelancer or small Gewerbe in Germany: covers Elster setup, quick and detailed registration, tax basics (VAT, Kleinunternehmerregelung 2025), EÜR and invoicing, software, banks, insurance, contracts, and job-search tips.

### Кратко (RU)
Практическое руководство по регистрации и работе как фрилансер или владелец Gewerbe в Германии: Elster, быстрая и подробная регистрация, налоги и Kleinunternehmerregelung 2025, EÜR и выставление счетов, софт, банки, страховки, контракты и поиск заказов.

### Table of contents
- [Предисловие](articles/2025/freelancer-gewerbe-guide.md#предисловие)
- [Об Авторе](articles/2025/freelancer-gewerbe-guide.md#об-авторе)
- [Список изменений](articles/2025/freelancer-gewerbe-guide.md#список-изменений)
- [Глава 1. Введение](articles/2025/freelancer-gewerbe-guide.md#глава-1-введение)
- [2. Про налоги](articles/2025/freelancer-gewerbe-guide.md#2-про-налоги)
- [3. Бухгалтерия и счета](articles/2025/freelancer-gewerbe-guide.md#3-бухгалтерия-и-счета)
- [ПО для Бухгалтерии](articles/2025/freelancer-gewerbe-guide.md#по-для-бухгалтерии)
- [Банки](articles/2025/freelancer-gewerbe-guide.md#банки)
- [Страховки](articles/2025/freelancer-gewerbe-guide.md#страховки)
- [Работа](articles/2025/freelancer-gewerbe-guide.md#работа)
- [Подработка как самозанятый](articles/2025/freelancer-gewerbe-guide.md#подработка-как-самозанятый)
- [Заключение](articles/2025/freelancer-gewerbe-guide.md#заключение)

## Repository layout
- `articles/` — articles and assets
- `articles/README.md` — article index
- `articles/assets/<slug>/` — per-article images
- `freelancer_gewerbe_guide_v0.5.docx` — source draft
- `freelanceguide.html` — exported guide

## Writing and publishing
1. Confirm SSH access to GitHub: `ssh -T git@github.com`.
2. Clone via SSH: `git clone git@github.com:ilyafedotov-ops/FreelanceDE.git`.
3. Create a branch: `git checkout -b article/<slug>`.
4. Add Markdown under `articles/<year>/<slug>.md` with the front matter below. Place images in `articles/assets/<slug>/` and link them relatively (for example, `![alt](./assets/<slug>/image.png)`).
5. Update `articles/README.md` with the title, date, and status.
6. Commit and push: `git add . && git commit -m "Add article <slug>" && git push -u origin article/<slug>`.
7. Open a pull request and merge to `main`.

### Front matter template
```markdown
---
title: "Title here"
date: "2024-03-01"
tags: ["freelance", "germany"]
summary: "One- or two-sentence abstract."
---
```

## Documentation
- `CONTRIBUTING.md` — contribution workflow.
- `STYLEGUIDE.md` — Markdown conventions.
- `CODE_OF_CONDUCT.md` — community standards.
- `LICENSE` — CC BY-NC 4.0.

## License
Creative Commons Attribution-NonCommercial 4.0 International. Use at your own risk; no warranty is provided.
