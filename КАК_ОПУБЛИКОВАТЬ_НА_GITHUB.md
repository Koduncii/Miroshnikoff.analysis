# Как выложить отчёт на GitHub Pages

## Вариант без командной строки

1. Войди на https://github.com
2. Нажми `+` справа сверху → `New repository`.
3. В поле `Repository name` напиши: `miroshnikov-analytics`.
4. Выбери `Public`.
5. Нажми `Create repository`.
6. На странице репозитория нажми `uploading an existing file`
   или `Add file` → `Upload files`.
7. Распакуй архив `miroshnikov_github_pages.zip`.
8. Перетащи в окно GitHub ВСЕ файлы ИЗ распакованной папки.
   Важно: `index.html` должен лежать в корне репозитория,
   а не внутри ещё одной папки.
9. Внизу нажми `Commit changes`.
10. Открой `Settings` репозитория.
11. Слева нажми `Pages`.
12. В блоке `Build and deployment`:
    - Source: `Deploy from a branch`
    - Branch: `main`
    - Folder: `/ (root)`
13. Нажми `Save`.

Ссылка будет такой:

https://ТВОЙ-ЛОГИН.github.io/miroshnikov-analytics/

Например, при логине `ivan`:

https://ivan.github.io/miroshnikov-analytics/

## Как обновить отчёт

1. Открой репозиторий.
2. `Add file` → `Upload files`.
3. Перетащи обновлённые файлы.
4. Подтверди замену.
5. Нажми `Commit changes`.

GitHub Pages обновит ту же ссылку.

## Частая ошибка

Неправильно:

miroshnikov-analytics/
└── miroshnikov_github_pages/
    └── index.html

Правильно:

miroshnikov-analytics/
├── index.html
├── .nojekyll
├── analysis_explorer.csv
└── остальные файлы
