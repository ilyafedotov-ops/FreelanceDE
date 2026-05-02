# FreelanceDE — русский README

[English version](README_EN.md) | [Главная](README.md)

Практический контентный проект о фрилансе и Gewerbe в Германии. Основной формат — Markdown-статьи с изображениями, плюс HTML/DOCX-экспорты для публикации и переноса.

В проекте нет приложения и отдельного build-step: это репозиторий для статей, источников, экспортов и сопутствующих материалов.

## Быстрый старт

- Основной русский гайд: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)
- Английская версия: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md)
- Индекс статей: [articles/README.md](articles/README.md)
- HTML-версия для blog/WordPress: [blog/freelance-guide.ru.html](blog/freelance-guide.ru.html)

## Что покрывает основной гайд

- разница между Freiberufler и Gewerbe;
- регистрация через Finanzamt, ELSTER и Gewerbeamt;
- Einkommensteuer, Umsatzsteuer, Kleinunternehmerregelung, Gewerbesteuer;
- EÜR и годовая налоговая декларация;
- формы декларации по статусам: Freiberufler, Gewerbe, Kleinunternehmer, работа по найму плюс подработка;
- счета, e-Rechnung, Reverse Charge и международные клиенты;
- банковские счета, платежные сервисы и бухгалтерский софт;
- медицинское, пенсионное и профессиональное страхование;
- контракты, Scheinselbständigkeit, поиск клиентов и расчет ставки;
- подработка как самозанятый;
- основы freelance-визы и полезные официальные ресурсы.

## Актуальность

Основной гайд обновлен `02.05.2026`. В последнем обновлении проверены и обновлены:

- Grundfreibetrag и зоны Einkommensteuer на 2026 год;
- Kinderfreibetrag;
- лимиты Kleinunternehmerregelung;
- пороги Umsatzsteuer-Voranmeldung;
- сроки подачи годовой декларации;
- GKV, Pflegeversicherung, Rentenversicherung и JAEG;
- разделы про страховки для иностранцев, freelance-визы, ресурсы и сообщества.

Старые release notes могут ссылаться на `2025.Q4`; для содержания статьи главным ориентиром является changelog внутри самой статьи.

## Важно

Материалы носят образовательный и практический характер. Это не налоговая, юридическая, бухгалтерская или миграционная консультация.

Перед подачей документов или принятием решений проверяйте актуальные требования в официальных источниках, Finanzamt, Ausländerbehörde, Krankenkasse или у квалифицированного Steuerberater.

## Структура репозитория

```text
articles/
  2025/
    freelancer-gewerbe-guide.md       русский Markdown-гайд
    freelancer-gewerbe-guide-en.md    английский Markdown-гайд
  assets/
    freelancer-gewerbe-guide/         изображения основного гайда
  README.md                           индекс статей

blog/
  freelance-guide.ru.html             WordPress-style HTML-версия русского гайда

sources/
  freelanceguide.html                 source/export copy
  freelancer_gewerbe_guide_v0.5.docx  DOCX source/export

podcasts/
  FreelancerDE-Podcast-*.mp4          связанные podcast/video-файлы
```

## Как обновлять материалы

Для обычных текстовых изменений:

1. Сначала обновите [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md).
2. Если тема есть в обеих версиях, зеркально обновите [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md).
3. Обновите changelog в начале соответствующей статьи.
4. Если публичная HTML-страница должна совпадать, обновите [blog/freelance-guide.ru.html](blog/freelance-guide.ru.html).
5. Файлы в [sources/](sources/) обновляйте только при сознательном обновлении source/export-версий.

Для налоговых, страховых и визовых изменений сначала сверяйтесь с официальными источниками: BMF, ELSTER, BMG, DRV, Bundesagentur für Arbeit, Make it in Germany, Berlin LEA, IHK, BZSt и актуальными текстами законов.

## Полезные проверки

```bash
# Найти старые или подозрительные значения
rg -n "2024|2025|12 096|10 096|450 евро|€450|bmf-steuerrechner.de/ekst" articles/2025 blog

# Проверить внутренние якоря HTML
node - <<'NODE'
const fs = require('fs');
const html = fs.readFileSync('blog/freelance-guide.ru.html', 'utf8');
const ids = new Set([...html.matchAll(/\bid=["']([^"']+)["']/g)].map(m => m[1]));
const hrefs = [...html.matchAll(/href=["']#([^"']+)["']/g)].map(m => m[1]);
const missing = [...new Set(hrefs.filter(h => !ids.has(h)))];
console.log({ internalLinks: hrefs.length, missing: missing.length });
if (missing.length) console.log(missing.join('\n'));
NODE

# Проверить HTML warnings
tidy -utf8 -qe blog/freelance-guide.ru.html
```

`tidy` может показывать legacy warnings из WordPress/Word HTML: missing doctype, старые generated IDs, missing image alt или nested emphasis. Проблемой считаются malformed links, broken anchors и новые структурные ошибки.

## Как внести вклад

```bash
git clone git@github.com:ilyafedotov-ops/FreelanceDE.git
cd FreelanceDE
git checkout -b article/<slug>
```

Дальше внесите изменения, проверьте ссылки/якоря, сделайте commit/push и откройте pull request.

## Лицензия

CC BY-NC 4.0. Использование на свой страх и риск, без гарантий.
