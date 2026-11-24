# praxor-brand-assets

Логотипы, цвета и шрифты Праксора. Исходник — дизайн-система «Праксор» (снята с [praxor.ru](https://praxor.ru)). Значения всех токенов — в [tokens.json](tokens.json).

## Логотипы

Все SVG в кривых, цвета вшиты. Название шрифтом не набирать — брать готовый файл.

| Логотип | Файлы | Где использовать |
| ------- | ----- | ---------------- |
| <img src="images/png/praxor-logo.png?raw=true" width="240"> | [svg](images/svg/praxor-logo.svg), [png](images/png/praxor-logo.png) | Основная версия: на `brand-paper` и любом светлом фоне |
| <img src="images/png/praxor-logo-inverse.png?raw=true" width="240"> | [svg](images/svg/praxor-logo-inverse.svg), [png](images/png/praxor-logo-inverse.png) | На `brand-ink` и тёмных фото: рамка и буквы `brand-paper`, ядро `brand-blue-night` |
| <img src="images/png/praxor-logo-mono.png?raw=true" width="240"> | [svg](images/svg/praxor-logo-mono.svg), [png](images/png/praxor-logo-mono.png) | Одна краска: печать, гравировка, ч/б документы. Ядро цвета рамки |
| <img src="images/png/praxor-logo-latin.png?raw=true" width="200"> | [svg](images/svg/praxor-logo-latin.svg), [png](images/png/praxor-logo-latin.png) | Англоязычные материалы, домены, международные конференции |
| <img src="images/png/praxor-logo-latin-inverse.png?raw=true" width="200"> | [svg](images/svg/praxor-logo-latin-inverse.svg), [png](images/png/praxor-logo-latin-inverse.png) | То же, для тёмных фонов |

| Знак | Знак inverse | App icon | Favicon |
| ---- | ------------ | -------- | ------- |
| <img src="images/png/praxor-mark.png?raw=true" width="80"> | <img src="images/png/praxor-mark-inverse.png?raw=true" width="80"> | <img src="images/png/praxor-app-icon.png?raw=true" width="80"> | <img src="images/png/praxor-favicon.png?raw=true" width="32"> |
| [svg](images/svg/praxor-mark.svg), [png](images/png/praxor-mark.png) | [svg](images/svg/praxor-mark-inverse.svg), [png](images/png/praxor-mark-inverse.png) | [svg](images/svg/praxor-app-icon.svg), [png](images/png/praxor-app-icon.png) | [svg](images/svg/praxor-favicon.svg), [png](images/png/praxor-favicon.png) |
| Там, где название уже стоит рядом или места мало | То же, для тёмных фонов | Аватар в Telegram, LinkedIn, иконка приложения | 16px: обводка 2, ядро 6 — иначе рамка рассыпается |

Инверсные версии светлые и на белом фоне GitHub не видны — это нормально.

### Построение

Знак — квадратная рамка с синим ядром. Рамка — это Harness, среда с правилами и проверками; ядро — работа агента внутри этих рамок.

| Элемент | Размер | Положение |
| ------- | ------ | --------- |
| Рамка | 14 × 14, обводка 1.5 | по краю сетки, обводка внутрь |
| Ядро | 5 × 5, заливка | точно по центру (4.5 от каждого края) |
| Просвет | 3 | одинаковый со всех сторон |

Словесный знак — «Праксор» / «Praxor», Geist Medium (500), трекинг −0.019em, в кривых. Горизонтальная композиция одна: знак 14, пробел 10, словесный знак кеглем 16; знак выровнен по центру высоты прописной.

### Использование

- Охранное поле — ширина ядра (5 единиц сетки знака) со всех сторон.
- Минимальная высота знака: 14px на экране (меньше — только фавикон), 4 мм в печати.
- Минимальная ширина горизонтальной версии: 80px на экране, 20 мм в печати.
- На светлом фоне: рамка и буквы `brand-ink`, ядро `brand-blue`.
- На тёмном фоне: рамка и буквы `brand-paper`, ядро `brand-blue-night`. Синий `brand-blue` на `brand-ink` даёт только 2.9:1 и проваливается.
- На фото — только на спокойном участке; иначе версия на плашке `praxor-app-icon.svg`.
- Ядро только синее или цвета рамки (монохром). Янтарный, градиенты и другие цвета запрещены.

### Как нельзя

- Скруглять рамку или делать ядро кругом.
- Сдвигать ядро из центра, менять толщину рамки.
- Ставить знак без ядра (пустая рамка — устаревший вариант).
- Набирать «Праксор» шрифтом рядом со знаком.
- Растягивать, поворачивать, добавлять тени и обводки.
- Писать название капсом («ПРАКСОР») или разрывать композицию на две строки.

## Типографика

### Текст и заголовки

Geist — [шрифт](https://fonts.google.com/specimen/Geist). Заголовки — Regular 400 с отрицательным трекингом (жирные не используем), лид и тезисы — Light 300, заголовки пунктов — Medium 500, основной текст — Regular 400.

### Служебный слой

JetBrains Mono Regular — [шрифт](https://fonts.google.com/specimen/JetBrains+Mono). Eyebrow, коды, кнопки, навигация, подписи полей. Всегда в верхнем регистре с разрядкой 0.08–0.09em.

```html
<link href="https://fonts.googleapis.com/css2?family=Geist:wght@300;400;500&family=JetBrains+Mono:wght@400&display=swap" rel="stylesheet">
```

## Цвета

Палитра — бумага, чернила и один синий. Остальные цвета служебные.

<img src="images/png/praxor-brand-palette.png?raw=true" width="600">

[svg](images/svg/praxor-brand-palette.svg), [png](images/png/praxor-brand-palette.png)

### Основные

| Токен | RGB | HEX | CMYK | Где |
| ----- | --- | --- | ---- | --- |
| `brand-paper` | `251 250 248` | `FBFAF8` | `0 0 1 2` | Фон страницы, светлые панели |
| `brand-ink` | `14 17 22` | `0E1116` | `36 23 0 91` | Текст, тёмные полосы, рамка знака |
| `brand-blue` | `27 77 228` | `1B4DE4` | `88 66 0 11` | Ядро знака, ссылки, выделение. На `brand-ink` не использовать |

### Дополнительные

| Токен | RGB | HEX | CMYK | Где |
| ----- | --- | --- | ---- | --- |
| `brand-blue-night` | `110 143 247` | `6E8FF7` | `55 42 0 3` | Синий для тёмного фона: ядро знака на `brand-ink` |
| `brand-amber` | `180 83 9` | `B45309` | `0 54 95 29` | Только человек в контуре (gate) и ошибка формы |
| `brand-amber-night` | `232 161 85` | `E8A155` | `0 31 63 9` | Янтарь для тёмного фона |
| `brand-graphite` | `58 65 73` | `3A4149` | `21 11 0 71` | Вторичный текст, навигация |
| `brand-slate` | `91 100 110` | `5B646E` | `17 9 0 57` | Примечания, подписи под формой |
| `brand-steel` | `139 147 156` | `8B939C` | `11 6 0 39` | Моно-лейблы и номера. На светлом фоне 3.0:1 — не нести им важный смысл |
| `brand-sand` | `226 223 218` | `E2DFDA` | `0 1 4 11` | Волосяные линии, рельсы, заглушка фото |

CMYK рассчитан из RGB без цветового профиля. Для печати сверяйте с типографией.

Синий — всегда «цель» или «действие»; большими площадями не заливать. Янтарь — никогда не декоративный цвет.
