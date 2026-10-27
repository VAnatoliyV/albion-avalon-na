# Карта Дорог Авалона — сервер Америки

Отдельный статический сайт с одной картой Дорог Авалона для сервера Albion Online **Americas**.
Будет опубликован как GitHub Pages: https://vanatoliyv.github.io/albion-avalon-na/

Связи присылают игроки из приложения Albion Journal. Сайт опрашивает живой сервер
`https://129-80-180-213.sslip.io/roads.json?server=americas` (тот же, что у европейской
карты на основном сайте), раскладку и поиск пути считает `avalon-core.js`, названия зон — `zones.json`.
Приложения открывают карту с зоной игрока: `#here=<код зоны>`. Ключ админа — `#key=…`, хранится в localStorage (`aan_mapkey`).

Тесты ядра: `node --test test/*.test.js`. Локально: `python3 -m http.server 8080`.
