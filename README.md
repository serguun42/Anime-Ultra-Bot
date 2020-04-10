# Anime Ultra Bot
#### Что умеет?

* Скрывать спойлеры командой /spoiler.
* Приветствовать новых пользователей.
* Обрабатывать ссылки на ресурсы.

#### Обработка ссылок на ресурсы

Если сообщение пользователя состоит из одной только ссылки на
* Твит (изображения, гифки и видео)
* Иллюстрацию или мангу в Pixiv (изображения)
* Пост в Instagram (изображения и видео)
* Пост на Reddit (изображения и гифки)
* Пост на Danbooru (изображения)
* Пост на Gelbooru (изображения)
* Пост на Konachan (изображения)
* Пост на Yande.re (изображения)
* Пост на Sankaku Channel (изображения)
* Пост на Zerochan (изображения)
* Пост на Anime-Pictures.net (изображения)
* Пост на Anime Joyreactor (изображения)
* На файл изображения в Твиттере
то бот отправит в чат все картинки из поста в лучшем качестве, даст ссылки на пост, автора (при наличии), на файлы картинок/гифок/видео, сделает красивые кнопки для перехода (в зависимости от платформы) к автору и/или посту и/или исходнику, а также рабочую кнопку лайка.


#### Команда /spoiler

Если пользователь
* напишет спойлер через инлайн,
* напишет команду /spoiler в реплае к тексту или картинке,
* напишет команду /spoiler в описании к картинку при её отправке (после команды можешь указать описание, и оно будет видно при отправке через ЛС бота),
* напишет команду /spoiler, а после неё текст спойлера,
то бот скроет текст и/или изображения спойлера.


#### Команда /khaleesi

*Кхалиси*фицирует текст – работает на текст сообщения, на которое ответили командой `/khaleesi`.


## Конфигурация

Всё указывается и настраивается в файле `animeultrabot.config.json` – токены для Telegram и Twitter, список чатов с id, white-list для команд, данные админа, картинки для взаимодействия с пользователем в inline-режиме и т.п.

## Использующиеся модули


Модули, которые использует `animeultrabot.js` (можете установить их через `npm`, `yarn`, etc.):
* Telegraf
* Twitter-lite
* node-fetch
* proxy-agent – используется на локалке (винде) для обхода ограничений Рыбнадзора. Указать параметр `PROXY_URL` в конфигурации.
* [Khaleesi.JS](https://github.com/serguun42/Khaleesi-JS) – ровно такой же модуль есть и в этом репозитории (нет в npm/yarn)

#### Полезные ссылки
* [Telegraf Module for Node.jS](https://telegraf.js.org/)
* [Telegram Bots API](https://core.telegram.org/bots/api)
* [Twitter API page for getting status](https://developer.twitter.com/en/docs/tweets/post-and-engage/api-reference/get-statuses-show-id)