# Политика конфиденциальности — расширение Zeno

**Дата последнего обновления:** 21 апреля 2026 г.

**Оператор / разработчик:** nikel303
**Контакт по вопросам конфиденциальности:** nikel303@gmail.com

---

## Единственное назначение

**Zeno** служит одной цели: заменить стандартную страницу новой вкладки на минималистичный экран (дата, сетка ярлыков из **одной** папки закладок Chrome, выбранной пользователем). Ярлыки — обычные закладки браузера; расширение **не** предназначено для блокировки рекламы, слежения за сайтами или изменения содержимого веб-страниц, кроме подмены новой вкладки.

---

## Кратко

- Расширение **не собирает**, **не продаёт** и **не передаёт** ваши закладки, настройки или историю просмотров на серверы разработчика.
- Закладки и их синхронизация — это стандартные функции **Chrome** (в том числе синхронизация через аккаунт Google, если вы её включили). Zeno только **читает и изменяет** закладки через официальный API браузера в выбранной вами папке.
- Настройки интерфейса и служебные данные (например, время обновления кэша иконок) хранятся **локально** в профиле Chrome (`chrome.storage.local` и локальные хранилища расширения).
- Для показа иконок сайтов расширение может **запрашивать изображения по сети** у самих сайтов (например, `favicon.ico`) и у публичного сервиса Google favicon (`https://www.google.com/s2/favicons`). Эти запросы идут **напрямую из вашего браузера**, не через сервер разработчика.

---

## Какие данные задействованы

### Закладки (`bookmarks`)

- Используются для отображения ярлыков на новой вкладке, изменения порядка, добавления и редактирования записей в **папке, которую вы выбрали** в настройках Zeno, а также для пункта контекстного меню «Добавить на главный экран (Zeno)».
- Содержимое закладок **не выгружается** разработчиком; оно остаётся в Chrome так же, как и для обычных закладок.

### Локальное хранилище (`storage`)

- Сохраняется идентификатор выбранной папки закладок, параметры отображения (стратегии иконок, заливки, подписей и т.п.), переопределения внешнего вида отдельных ярлыков, а также служебные метаданные кэша иконок (например, время последнего обновления по хосту).
- Данные хранятся **только на устройстве** в рамках профиля браузера.

### Кэш иконок (Cache API и связанные метаданные)

- Загруженные изображения favicon могут кэшироваться локально для ускорения работы. Кэш не передаётся разработчику.

### Сетевые запросы

- При отображении ярлыков расширение может запрашивать иконки по URL сайтов и через сервис Google favicon. Удалённые серверы видят такой запрос так же, как при обычном обращении к ресурсу (типично — только запрос файла изображения, без передачи списка ваших закладок от имени Zeno).

---

## Контекстное меню (`contextMenus`)

- Нужно только для добавления текущей страницы или ссылки в выбранную папку закладок. Данные меню не отправляются разработчику.

---

## Дети

Расширение не ориентировано на сбор данных о детях младше 13 лет (или возраста, установленного в вашей юрисдикции) и не запрашивает такие данные целенаправленно.

---

## Изменения политики

При существенных изменениях в обработке данных мы обновим этот документ и дату «последнего обновления». Актуальная версия доступна по тому же адресу, который вы указали в Chrome Web Store.

---

## Контакт

По вопросам конфиденциальности: **nikel303@gmail.com**.

---

# Privacy Policy — Zeno browser extension (English summary)

**Last updated:** April 21, 2026.

**Developer:** nikel303
**Privacy contact:** nikel303@gmail.com

## Single purpose

**Zeno** has one purpose: replace Chrome’s default new tab page with a minimal dashboard (the date, a grid of shortcuts from **one** bookmark folder you select). Shortcuts are normal browser bookmarks; the extension is **not** for ad blocking, cross-site tracking, or modifying web page content except the new tab override.

---

**Zeno** is a Chrome extension (Manifest V3) that replaces the new tab page with a speed-dial backed by your **Chrome bookmarks** in a folder you choose.

- We **do not** collect, sell, or transmit your bookmarks, settings, or browsing history to our servers. **We do not operate a backend** for this extension.
- Bookmarks are read and updated through Chrome’s **bookmarks API**; sync behavior follows your **Chrome / Google account** settings.
- UI preferences and related metadata are stored **locally** in `chrome.storage.local` (and local extension storage). Favicons may be cached locally.
- To show site icons, the extension may **fetch images** from the **same sites** as your shortcuts (e.g. `favicon.ico`) and from **Google’s public favicon service** (`https://www.google.com/s2/favicons`). Those requests go **from your browser** to those hosts, not through us.
For questions: **nikel303@gmail.com**.
