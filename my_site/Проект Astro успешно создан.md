# Проект Astro успешно создан

```
user@debian01:~/my_site$ npm create astro@latest

> npx
> create-astro


 astro   Launch sequence initiated.

   dir   Where should we create your new project?
         ./mechanical-mercury

  tmpl   How would you like to start your new project?
         A basic, helpful starter project

  deps   Install dependencies?
         Yes

   git   Initialize a new git repository?
         Yes

      ✔  Project initialized!
         ■ Template copied
         ■ Dependencies installed
         ■ Git initialized

  next   Liftoff confirmed. Explore your project!

         Enter your project directory using cd ./mechanical-mercury 
         Run npm run dev to start the dev server. q + ENTER to stop.
         Add frameworks like react or tailwind using astro add.

         Stuck? Join us at https://astro.build/chat

╭─────╮  Houston:
│ ◠ ◡ ◠  Good luck out there, astronaut! 🚀╰─────╯
user@debian01:~/my_site$ 
```

Отлично! Проект Astro успешно создан. Разберу дальнейшие шаги подробно.

## Статус проекта

Все этапы выполнены успешно:

- ✓ Создана папка `mechanical-mercury` в `~/my_site`;
- ✓ Скопирован базовый шаблон Astro;
- ✓ Установлены все зависимости через `npm install`;
- ✓ Инициализирован Git‑репозиторий.

------

## Пошаговое руководство по запуску

**Шаг 1. Перейдите в папку проекта**

Выполните команду:

bash

```bash
cd mechanical-mercury
```

**Шаг 2. Проверьте содержимое папки**

Убедитесь, что структура проекта создана корректно:

bash

```bash
ls -la
```

Вы должны увидеть ключевые файлы и папки:

- `package.json` — описание проекта и список зависимостей;
- `astro.config.mjs` — конфигурация Astro;
- `src/` — исходные файлы проекта (страницы, компоненты, стили);
- `public/` — статические файлы (изображения, шрифты);
- `.gitignore` — файлы, игнорируемые Git.

**Шаг 3. Запустите сервер разработки**

Выполните:

bash

```bash
npm run dev
```

Что произойдёт:

- запустится локальный сервер;
- откроется браузер с адресом `http://localhost:3000`;
- включится «горячая перезагрузка» (Hot Reload) — изменения в коде будут сразу отображаться в браузере.

**Шаг 4. Проверьте работу Git**

Убедитесь, что репозиторий инициализирован:

bash

```bash
git status
```

Ожидаемый результат — сообщение о том, что все файлы отслеживаются и нет неотслеживаемых изменений.

------

## Основные команды для работы с проектом

| Команда                     | Действие                                                     |
| --------------------------- | ------------------------------------------------------------ |
| `npm run dev`               | Запуск сервера разработки (локальный режим)                  |
| `npm run build`             | Сборка проекта для продакшена (файлы помещаются в папку `dist/`) |
| `npm run preview`           | Предпросмотр собранного проекта локально                     |
| `git status`                | Проверка статуса Git‑репозитория                             |
| `git add .`                 | Добавление файлов в индекс Git                               |
| `git commit -m "Сообщение"` | Создание коммита в Git                                       |

------

## Что делать дальше: первые шаги в проекте

1. **Откройте проект в редакторе кода** (VS Code, WebStorm и т. д.):

   - найдите файл `src/pages/index.astro` — это главная страница сайта;
   - измените текст внутри тега `<h1>` и сохраните файл;
   - в браузере автоматически отобразится обновлённая страница (благодаря Hot Reload).

2. **Добавьте новый маршрут**:

   - создайте файл `src/pages/about.astro`;
   - вставьте базовый HTML‑код (например, `<h1>О нас</h1>`);
   - откройте в браузере `http://localhost:3000/about` — новая страница будет доступна.

3. **Установите дополнительные фреймворки** (по желанию):

   - React: `npx astro add react`;
   - Tailwind CSS: `npx astro add tailwind`.

4. **Соберите проект для продакшена**:

   bash

1. ```bash
   npm run build
   ```

   Статические файлы появятся в папке `dist/`. Их можно загрузить на хостинг (Netlify, Vercel, GitHub Pages и т. д.).

------

## Возможные проблемы и решения

- **«Порт 3000 занят»**:
  - сервер уже запущен в другом терминале;
  - используйте другой порт: `npm run dev -- --port 5000`.
- **«Страница в браузере не загружается»**:
  - проверьте, что в терминале нет ошибок после запуска `npm run dev`;
  - откройте `http://localhost:3000` вручную в браузере.
- **«Git не отслеживает файлы»**:
  - убедитесь, что вы находитесь в папке проекта (`cd mechanical-mercury`);
  - выполните `git status` для проверки статуса.
- **«Ошибка при сборке (`npm run build`)»**:
  - очистите кэш: `npm cache clean --force`;
  - переустановите зависимости: `rm -rf node_modules && npm install`.

------

## Краткий итог действий

1. Перейдите в папку проекта: `cd mechanical-mercury`.
2. Запустите сервер: `npm run dev`.
3. Откройте `http://localhost:3000` в браузере.
4. Редактируйте файлы в `src/pages/` и наблюдайте за изменениями в реальном времени.
5. Соберите проект: `npm run build`.
6. (Опционально) Работайте с Git: `git add .`, `git commit`.

Если у вас возникнут вопросы по какому‑либо этапу или появятся ошибки — напишите, я помогу разобраться!



```
user@debian01:~/my_site$ cd mechanical-mercury
user@debian01:~/my_site/mechanical-mercury$ ls -la
итого 224
drwxr-xr-x   7 user user   4096 апр 14 11:23 .
drwxr-xr-x   3 user user   4096 апр 14 11:27 ..
-rw-r--r--   1 user user    122 апр 14 01:21 astro.config.mjs
drwxr-xr-x   7 user user   4096 апр 14 11:23 .git
-rw-r--r--   1 user user    264 апр 14 01:21 .gitignore
drwxr-xr-x 227 user user  12288 апр 14 11:23 node_modules
-rw-r--r--   1 user user    292 апр 14 11:22 package.json
-rw-r--r--   1 user user 169345 апр 14 11:23 package-lock.json
drwxr-xr-x   2 user user   4096 апр 14 11:22 public
-rw-r--r--   1 user user   1657 апр 14 11:22 README.md
drwxr-xr-x   6 user user   4096 апр 14 11:22 src
-rw-r--r--   1 user user    109 апр 14 01:21 tsconfig.json
drwxr-xr-x   2 user user   4096 апр 14 11:22 .vscode
user@debian01:~/my_site/mechanical-mercury$ npm run dev

> mechanical-mercury@0.0.1 dev
> astro dev

▶ Astro collects anonymous usage data.
  This information helps us improve Astro.
  Run "astro telemetry disable" to opt-out.
  https://astro.build/telemetry

[vite] connected.
11:32:55 [types] Generated 0ms
11:32:55 [WARN] [content] Content config not loaded
 astro  v6.1.6 ready in 890 ms
┃ Local    http://localhost:4321/
┃ Network  use --host to expose
11:32:55 watching for file changes...
11:33:25 [200] / 46ms
11:33:25 [vite] ✨ new dependencies optimized: astro/runtime/client/dev-toolbar/entrypoint.js
11:33:25 [vite] ✨ optimized dependencies changed. reloading
11:33:25 [200] / 3ms
```

Отлично! Проект успешно запущен. Разберу вывод терминала и дам дальнейшие инструкции.

## Анализ вывода терминала

Вы выполнили команду `npm run dev`, и система сообщила:

- **Astro v6.1.6 ready in 890 ms** — проект успешно инициализирован за 890 мс;
- **Local:**  — локальный адрес для просмотра проекта в браузере;

- **Network: use --host to expose** — чтобы открыть доступ к проекту с других устройств в сети, нужно добавить флаг `--host`;
- **watching for file changes…** — включён режим наблюдения за изменениями файлов (Hot Reload);
- **Content config not loaded** — предупреждение о том, что конфигурация контента не загружена (это нормально для базового шаблона, не является ошибкой).

## Что делать дальше

**1. Откройте проект в браузере**

Перейдите по адресу: `http://localhost:4321/`

Вы должны увидеть стартовую страницу Astro с приветствием и базовой навигацией.

**2. Протестируйте Hot Reload (горячую перезагрузку)**

1. Откройте файл `src/pages/index.astro` в текстовом редакторе.
2. Найдите тег `<h1>` с текстом «Welcome to Astro».
3. Измените текст, например, на «Мой первый Astro‑сайт».
4. Сохраните файл.
5. Обновите страницу в браузере или дождитесь автоматического обновления — новый текст появится мгновенно.

**3. Изучите структуру проекта**

Ключевые папки и файлы:

- `src/pages/` — здесь создаются страницы сайта (каждая `.astro`‑файл становится отдельной страницей);
- `src/components/` — папка для повторно используемых компонентов;
- `public/` — статические файлы (изображения, шрифты, favicon);
- `astro.config.mjs` — основная конфигурация Astro;
- `package.json` — зависимости и скрипты проекта;
- `.git/` — папка Git‑репозитория.

**4. Создайте новую страницу**

1. Создайте файл `src/pages/about.astro`.
2. Вставьте следующий код:

astro

```astro
---
---
<html>
  <head>
    <title>О нас</title>
  </head>
  <body>
    <h1>Страница «О нас»</h1>
    <p>Это новая страница, созданная вручную.</p>
  </body>
</html>
```

1. Сохраните файл и откройте в браузере `http://localhost:4321/about` — новая страница будет доступна.

**5. Добавьте навигацию**

В `src/pages/index.astro` добавьте ссылку на новую страницу:

astro

```astro
<a href="/about">О нас</a>
```

Теперь с главной страницы можно перейти на страницу «О нас».

------

## Основные команды для работы

| Команда                   | Действие                                              |
| ------------------------- | ----------------------------------------------------- |
| `npm run dev`             | Запуск сервера разработки (порт 4321)                 |
| `npm run build`           | Сборка проекта для продакшена (файлы в `dist/`)       |
| `npm run preview`         | Предпросмотр собранного проекта локально              |
| `astro add <framework>`   | Добавление фреймворков (React, Vue, Tailwind и т. д.) |
| `astro telemetry disable` | Отключение сбора анонимных данных Astro               |

------

## Полезные советы

- **Изменение порта**: если порт 4321 занят, запустите сервер на другом порту:

bash

```bash
npm run dev -- --port 5000
```

- **Доступ по сети**: чтобы открыть проект для других устройств в локальной сети:

bash

```bash
npm run dev -- --host
```

- **Остановка сервера**: нажмите `Ctrl+C` в терминале.
- **Обновление зависимостей**: проверяйте обновления Astro:

bash

```bash
npm outdated
```

------

## Проверка работоспособности

Убедитесь, что:

- браузер открывает `http://localhost:4321/` без ошибок;
- изменения в `.astro`‑файлах автоматически отображаются в браузере;
- команда `npm run build` выполняется без ошибок и создаёт папку `dist/`;
- `git status` показывает чистые изменения (если планируете использовать Git).

------

## Краткий итог действий

1. Откройте `http://localhost:4321/` в браузере.
2. Редактируйте файлы в `src/pages/` и наблюдайте за изменениями в реальном времени.
3. Создайте новую страницу (`about.astro`) и добавьте на неё контент.
4. Добавьте ссылку на новую страницу в `index.astro`.
5. Соберите проект: `npm run build`.
6. Остановите сервер: `Ctrl+C`.

Если у вас возникнут вопросы по какому‑либо этапу или появятся ошибки — напишите, я помогу разобраться!



# Как перенести этот проект на Гитхаб

```
Как перенести этот проект на Гитхаб
```

Разберу процесс переноса проекта на GitHub пошагово.

## Шаг 1. Создайте репозиторий на GitHub

1. Зайдите на 

1.  и войдите в свой аккаунт.
2. Нажмите кнопку `New` (зелёная кнопка «New repository») в верхнем правом углу.
3. Заполните поля:
   - **Repository name**: `mechanical-mercury` (или любое другое название);
   - **Description**: краткое описание проекта (опционально);
   - **Visibility**: выберите `Public` (доступно всем) или `Private` (только для вас и приглашённых);
   - **Initialize this repository with**: **не ставьте галочки** — у вас уже есть локальный репозиторий.
4. Нажмите `Create repository`.

## Шаг 2. Подготовьте локальный репозиторий

Убедитесь, что вы в папке проекта:

bash

```bash
cd ~/my_site/mechanical-mercury
```

Проверьте статус Git:

bash

```bash
git status
```

Вы должны увидеть, что все файлы отслеживаются и нет неотслеживаемых изменений.

## Шаг 3. Добавьте удалённый репозиторий

Скопируйте URL нового репозитория с GitHub (в формате `https://github.com/username/repository-name.git`).

Добавьте его как удалённый репозиторий (`origin`):

bash

```bash
git remote add origin https://github.com/ваш-логин/mechanical-mercury.git
```

Замените `ваш-логин` на ваш логин GitHub и `mechanical-mercury` на реальное название репозитория, если выбрали другое.

Проверьте, что удалённый репозиторий добавлен:

bash

```bash
git remote -v
```

Вы должны увидеть URL в строках `fetch` и `push`.

## Шаг 4. Отправьте код на GitHub

**Вариант 1. Если у вас стандартная ветка `main`**

Выполните команды:

bash

```bash
git branch -M main
git push -u origin main
```

- `git branch -M main` — переименовывает текущую ветку в `main` (стандарт для новых репозиториев GitHub);
- `git push -u origin main` — отправляет ветку `main` на GitHub и связывает её с удалённой веткой.

**Вариант 2. Если у вас ветка `master`**

Если локальная ветка называется `master`, используйте:

bash

```bash
git push -u origin master
```

## Шаг 5. Проверьте результат

1. Перейдите на страницу вашего репозитория на GitHub.
2. Убедитесь, что:
   - все файлы проекта загружены;
   - история коммитов видна;
   - нет ошибок.

------

## Что попадёт на GitHub (и что нет)

**Будет загружено:**

- исходный код проекта (файлы `.astro`, `.js`, `.css` и т. д.);
- конфигурация Astro (`astro.config.mjs`);
- файл `package.json` (описание зависимостей);
- папка `public/` (статические файлы);
- документация (`README.md`);
- настройки Git (`.gitignore`, история коммитов).

**Не будет загружено:**

- папка `node_modules/` (исключается через `.gitignore`);
- файлы логов;
- временные файлы сборки (папка `dist/`).

------

## Дополнительные настройки (опционально)

**1. Обновите `README.md`**

Отредактируйте файл `README.md` в корне проекта, чтобы добавить:

- описание проекта;
- инструкции по запуску (`npm run dev`);
- список используемых технологий;
- скриншоты (если есть).

После изменений зафиксируйте их:

bash

```bash
git add README.md
git commit -m "Update README with project description"
git push
```

**2. Добавьте `.gitignore` (если нужно)**

Убедитесь, что в `.gitignore` есть строки:

```
node_modules/
dist/
.cache/
```

Это предотвратит загрузку временных и служебных файлов.

**3. Создайте ветки для функций**

Для разработки новых функций создавайте отдельные ветки:

bash

```bash
git checkout -b feature/new-page
```

После завершения работы сливайте их с `main`.

**4. Используйте теги для релизов**

Помечайте стабильные версии тегами:

bash

```bash
git tag v1.0.0
git push --tags
```

На GitHub это создаст релиз.

------

## Частые проблемы и решения

- **«Authentication failed»** (ошибка аутентификации):
  - используйте **Personal Access Token** вместо пароля;
  - создайте токен в настройках GitHub: `Settings → Developer settings → Personal access tokens`;
  - при пуше введите токен вместо пароля.
- **«Everything up-to-date»** (ничего не загружается):
  - проверьте, что есть коммиты: `git log`;
  - если коммитов нет, создайте первый:

bash

```bash
git add .
git commit -m "Initial commit"
```

- **«Remote rejected»** (удаленный репозиторий отклонил пуш):
  - возможно, в удалённом репозитории есть конфликтующие файлы (например, `README.md`);
  - выполните `git pull origin main`, разрешите конфликты, затем `git push`.
- **«Large files»** (слишком большие файлы):
  - удалите большие файлы из истории Git или используйте **Git LFS**;
  - добавьте их в `.gitignore`.

------

## Краткий итог команд

1. Переход в папку проекта:

bash

```bash
cd ~/my_site/mechanical-mercury
```

1. Добавление удалённого репозитория:

bash

```bash
git remote add origin https://github.com/ваш-логин/mechanical-mercury.git
```

1. Отправка кода на GitHub:

bash

```bash
git branch -M main
git push -u origin main
```

1. (Опционально) Обновление `README` и отправка изменений:

bash

```bash
git add README.md
git commit -m "Update README"
git push
```

------

## Проверка успешного переноса

После выполнения команд убедитесь, что:

- на странице GitHub репозитория видны все файлы проекта;
- `README.md` отображается корректно;
- нет ошибок в терминале после `git push`;
- команда `git status` показывает чистую рабочую директорию.

Если у вас возникнут вопросы по какому‑либо этапу или появятся ошибки — напишите, я помогу разобраться!