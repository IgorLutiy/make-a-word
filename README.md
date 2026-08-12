# 🧩 Составь слово / Word Scramble v1.0

Интерактивная браузерная игра: составь слово из перемешанных букв.  
Поддерживает **русский**, **английский** и **украинский** языки.  
Работает на GitHub Pages без сервера.

[![Demo](https://img.shields.io/badge/demo-GitHub%20Pages-blue?style=flat-square)](https://igorlutiy.github.io/interactive/make_a_word/)
[![Languages](https://img.shields.io/badge/languages-RU%20%7C%20EN%20%7C%20UK-green?style=flat-square)](#)
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)

---

## 🎮 Возможности

- Выбор длины слова: **3 / 4 / 5 / 6 / 7 / 8** букв
- Сборка слова кликами по буквам или вводом с клавиатуры
- Перемешивание букв, пропуск слова, подсказка
- Счёт, таймер, количество угаданных слов
- Лучший результат сохраняется в `localStorage`
- Красивый адаптивный интерфейс (мобильные + десктоп)
- Легко добавлять новые языки

---

## 🚀 Как запустить

### Локально
Просто открой `index.html` в браузере  
или подними статический сервер:

```bash
npx serve .
# или
python -m http.server 8000
```

### На GitHub Pages
1. Создай репозиторий и загрузи все файлы
2. Перейди в **Settings → Pages**
3. Source: **Deploy from a branch** → `main` / `root`
4. Сайт будет доступен по адресу:  
   `https://<username>.github.io/<repo-name>/`

---

## 🌍 Добавление нового языка

Открой файл `words.js` и добавь язык по образцу:

```js
languages['de'] = {
  name: 'Deutsch',
  flag: '🇩🇪',
  words: {
    3: ['haus', 'baum', 'auto', ...],
    4: ['buch', 'tisch', 'spiel', ...],
    5: ['apfel', 'wasser', 'schule', ...],
    6: ['freund', 'familie', ...],
    7: ['lehrer', 'schüler', ...],
    8: ['computer', 'sprache', ...]
  }
};
```

После сохранения язык сразу появится в выпадающем списке игры.

---

## 📁 Структура проекта

```
word-game/
├── index.html      # Разметка
├── style.css       # Стили
├── game.js         # Логика игры
├── words.js        # Словари (RU / EN / UK)
└── README.md
```

---

## 📊 Словари

| Язык            | 3 | 4 | 5 | 6 | 7 | 8 |
|-----------------|---|---|---|---|---|---|
| 🇷🇺 Русский      | 49 | 64 | 58 | 30 | 20 | 13 |
| 🇬🇧 English     | 49 | 58 | 52 | 45 | 30 | 20 |
| 🇺🇦 Українська  | 47 | 52 | 41 | 17 | 20 | 5  |

Списки можно легко расширять в `words.js`.

---

## 🛠 Технологии

- Чистый **HTML / CSS / JavaScript** (без фреймворков)
- Работает офлайн
- Адаптивная вёрстка
- Поддержка кириллицы и латиницы

---

## 📄 Лицензия

GPL-3.0 license.

---

Приятной игры! 🎯
