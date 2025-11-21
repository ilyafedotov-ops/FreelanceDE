# FreelanceDE — навигатор (RU)

[Switch to English](README_EN.md)

Главная страница на русском: что в репозитории, как читать статьи и где найти ключевые разделы про бухгалтерию.

## О репозитории
Гайды и статьи о фрилансе в Германии. Все материалы в Markdown, лицензия — CC BY-NC 4.0.

## Текущая статья
- RU: [articles/2025/freelancer-gewerbe-guide.md](articles/2025/freelancer-gewerbe-guide.md)
- EN: [articles/2025/freelancer-gewerbe-guide-en.md](articles/2025/freelancer-gewerbe-guide-en.md) (пока в процессе перевода текста)
- Лицензия: CC BY-NC 4.0; на ваш риск.

## Кратко о статье
Практическое руководство по регистрации и работе как фрилансер или владелец Gewerbe в Германии: Elster и формы, быстрый/подробный сценарий регистрации, налоги (НДС, Kleinunternehmerregelung 2025, Europäische KUR), EÜR, выставление счетов и э‑счета, софт, банки, страховки, контракты, поиск клиентов.

## Что внутри (с учётом бухгалтерии)
- Регистрация: Elster, Freiberufler vs Gewerbe, быстрый и подробный сценарии.
- Налоги: НДС, Kleinunternehmerregelung (порог 25k с 2025), Europäische KUR, авансовые платежи, примеры расчётов.
- Бухгалтерия: EÜR (кассовый метод), что списывать, учёт расходов/амортизации, требования к счетам, электронные счета (этапы 2025–2027), reverse charge.
- Инструменты: бухгалт. софт (Lexoffice, SevDesk и др.), банки для фрилансеров, платёжные провайдеры (Stripe/Wise), шаблоны счетов.
- Риски/операционка: страховки, контракты, Scheinselbständigkeit, поиск клиентов и ставки.

## Ключевые заметки по учёту
- Ведите EÜR: доходы/расходы кассовым методом, храните подтверждения.
- Счёт должен включать реквизиты, дату/номер, описание услуги, суммы, VAT/основание освобождения, платежные условия.
- Kleinunternehmerregelung: оборот до 25 000 € (с 2025) — без НДС, но основание нужно указать на счёте.
- Э-счета: обязательное поэтапное введение с 2025; см. раздел про электронные счета для дат и форматов.

## Оглавление статьи
- [Предисловие](articles/2025/freelancer-gewerbe-guide.md#предисловие)
- [Об Авторе](articles/2025/freelancer-gewerbe-guide.md#об-авторе)
- [Список изменений](articles/2025/freelancer-gewerbe-guide.md#список-изменений)
- [Глава 1. Введение](articles/2025/freelancer-gewerbe-guide.md#глава-1-введение)
- [2. Про налоги](articles/2025/freelancer-gewerbe-guide.md#2-про-налоги)
- [3. Бухгалтерия и счета](articles/2025/freelancer-gewerbe-guide.md#3-бухгалтерия-и-счета)
- [4. ПО для Бухгалтерии](articles/2025/freelancer-gewerbe-guide.md#4-по-для-бухгалтерии)
- [5. Банки](articles/2025/freelancer-gewerbe-guide.md#5-банки)
- [6. Страховки](articles/2025/freelancer-gewerbe-guide.md#6-страховки)
- [7. Работа](articles/2025/freelancer-gewerbe-guide.md#7-работа)
- [8. Подработка как самозанятый](articles/2025/freelancer-gewerbe-guide.md#8-подработка-как-самозанятый)
- [9. Заключение](articles/2025/freelancer-gewerbe-guide.md#9-заключение)

## Структура репозитория
- `articles/` — статьи и ресурсы
- `articles/assets/<slug>/` — изображения статьи
- `articles/README.md` — индекс статей
- `sources/` — исходники и экспортированные версии (docx/html)
- `CONTRIBUTING.md`, `STYLEGUIDE.md`, `CODE_OF_CONDUCT.md`, `LICENSE`

## Как читать и обновлять
- Читайте статьи прямо на GitHub или через локальный редактор Markdown.
- Для обновлений: создайте ветку (`git checkout -b article/<slug>`), добавьте файл в `articles/<year>/<slug>.md`, обновите `articles/README.md`, коммит/пуш через SSH, откройте PR.

## Лицензия
CC BY-NC 4.0. Использование на ваш риск, без гарантий.
