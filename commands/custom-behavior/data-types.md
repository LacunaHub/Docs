# Типы данных

## Guild

| Свойство                      | Тип                                                                                                                                                                                                | Описание                                    |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| `id`                          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Идентификатор сервера                       |
| `name`                        | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Название сервера                            |
| `nameAcronym`                 | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Инициалы сервера                            |
| `icon`                        | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Ссылка на иконку сервера                    |
| `channels`                    | array of [channels](data-types.md#channel)                                                                                                                                                         | Каналы сервера                              |
| `roles`                       | array of [roles](data-types.md#guildrole)                                                                                                                                                          | Роли сервера                                |
| `splash`                      | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Ссылка на баннер приглашений                |
| `banner`                      | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Ссылка на баннер                            |
| `description`                 | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Описание сервера                            |
| `discoverySplash`             | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Ссылка на баннер в каталоге серверов        |
| `vanityURLCode`               | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Код установленного приглашения              |
| `verificationLevel`           | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Уровень проверки сервера                    |
| `afkTimeout`                  | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Тайм-аут простоя                            |
| `afkChannelId`                | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Идентификатор канала простоя                |
| `rulesChannelId`              | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Идентификатор канала правил                 |
| `systemChannelId`             | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Идентификатор системного канала             |
| `publicUpdatesChannelId`      | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Идентификатор канала публичных обновлений   |
| `premiumTier`                 | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Уровень буста сервера                       |
| `premiumSubscriptionCount`    | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Количество пользователей забустивших сервер |
| `explicitContentFilter`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Фильтр фильтрации нежелательного контента   |
| `defaultMessageNotifications` | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) or [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Стандартные уведомления о сообщениях        |
| `ownerId`                     | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Идентификатор владельца сервера             |
| `createdTimestamp`            | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Временная метка создания сервера            |
| `economyCurrencies`           | array of [currencies](data-types.md#guildcurrency)                                                                                                                                                 | Валюты экономики                            |

### GuildRole

| Свойство      | Тип                                                                                               | Описание                                                    |
| ------------- | ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| `id`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор роли                                          |
| `name`        | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Название роли                                               |
| `color`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Цвет роли                                                   |
| `icon`        | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Иконка роли                                                 |
| `hoist`       | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Включено ли отдельное отображение участников с данной ролью |
| `managed`     | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Является ли роль управляемой                                |
| `mentionable` | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Можно ли упомянуть роль                                     |
| `position`    | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Позиция роли                                                |

### GuildCurrency

| Свойство | Тип                                                                                             | Описание             |
| -------- | ----------------------------------------------------------------------------------------------- | -------------------- |
| `id`     | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор валюты |
| `name`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Название валюты      |
| `symbol` | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Символ валюты        |

## Member

| Свойство          | Тип                                                                                                                 | Описание                                |
| ----------------- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `user`            | [user](data-types.md#user)                                                                                          | Информация о пользователе               |
| `avatar`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                     | Ссылка на серверный аватар              |
| `nickname`        | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                     | Никнейм участника                       |
| `pending`         | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)                   | Прошел ли участник отбор                |
| `roles`           | array of [roles](data-types.md#guildrole)                                                                           | Роли участника                          |
| `permissions`     | array of [permissions](https://discord.com/developers/docs/topics/permissions#permissions-bitwise-permission-flags) | Разрешения участника                    |
| `joinedTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                     | Временная метка присоединения к серверу |
| `voice`           | [VoiceState](data-types.md#voicestate)                                                                              | Голосовое состояние                     |

## Channel

| Свойство           | Тип                                                                                                | Описание                                    |
| ------------------ | -------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| `createdTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)    | Временная метка создания канала             |
| `full`             | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Заполнен ли голосовой канал                 |
| `id`               | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Идентификатор канала                        |
| `lastMessageId`    | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор последнего сообщения в канале |
| `name`             | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Название канала                             |
| `nsfw`             | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)  | Ограничение по возрасту                     |
| `type`             | [ChannelType](https://discord.com/developers/docs/resources/channel#channel-object-channel-types)  | Тип канала                                  |
| `parentId`         | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор категории канала              |
| `position`         | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)    | Позиция канала относительно других          |
| `rateLimitPerUser` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)    | Медленные режим в секундах                  |
| `topic`            | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Тема канала                                 |

## Thread

| Свойство            | Тип                                                                                               | Описание                           |
| ------------------- | ------------------------------------------------------------------------------------------------- | ---------------------------------- |
| `archived`          | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Архивирована ли ветка              |
| `archivedTimestamp` | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)  | Временная метка архивирования      |
| `createdTimestamp`  | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Временная метка создания ветки     |
| `id`                | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор ветки                |
| `ownerId`           | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Автор ветки                        |
| `parentId`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Канал ветки                        |
| `rateLimitPerUser`  | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)  | Слоумод                            |
| `totalMessageSent`  | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)  | Всего отправлено сообщений в ветке |

## Command

| Свойство  | Тип                                                                                             | Описание                     |
| --------- | ----------------------------------------------------------------------------------------------- | ---------------------------- |
| `id`      | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор команды        |
| `name`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Название команды             |
| `options` | array of [options](data-types.md#commandoption)                                                 | Переданные аргументы команды |

### CommandOption

| Свойство  | Тип                                                                                                                                                                                                                                                                                                   | Описание                                                 |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| `name`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                                                                                                                       | Название аргумента                                       |
| `value`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) or [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Значение аргумента                                       |
| `user`    | ?[user](data-types.md#user)                                                                                                                                                                                                                                                                           | Упомянутый пользователь, если тип аргумента ПОЛЬЗОВАТЕЛЬ |
| `channel` | ?[channel](data-types.md#channel)                                                                                                                                                                                                                                                                     | Упомянутый канал, если тип аргумента КАНАЛ               |
| `role`    | ?[role](data-types.md#role)                                                                                                                                                                                                                                                                           | Упомянутая роль, если тип аргумента РОЛЬ                 |

## Interaction

| Свойство      | Тип                                                                                                                                                                                                 | Описание                                      |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------- |
| `customId`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                     | Пользовательский идентификатор взаимодействия |
| `fields`      | array of [InteractionField](data-types.md#interactionfield)                                                                                                                                         | Значения полей модального окна                |
| `guildLocale` | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)                                                                                                   | Локализация на сервере                        |
| `id`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                     | Идентификатор взаимодействия                  |
| `locale`      | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                     | Локализация пользователя                      |
| `values`      | ?array of [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)[s](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Выбранные значения выпадающего списка         |

### InteractionField

| Свойство   | Тип                                                                                             | Описание           |
| ---------- | ----------------------------------------------------------------------------------------------- | ------------------ |
| `customId` | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор поля |
| `value`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Значения поля      |

## Message

| Свойство           | Тип                                                                                                                                                                                                | Описание                                |
| ------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `cleanContent`     | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Содержание сообщения без форматирования |
| `content`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Содержание сообщения                    |
| `createdTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Дата создания сообщения                 |
| `crosspostable`    | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)                                                                                                  | Является ли сообщение публикуемым       |
| `editedTimestamp`  | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Дата изменения сообщения                |
| `embeds`           | array of [MessageEmbed](data-types.md#messageembed)                                                                                                                                                | Массив встроенных сообщений             |
| `flags`            | array of [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)[s](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Список флагов сообщения                 |
| `id`               | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Идентификатор сообщения                 |
| `mentions`         | array of [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)[s](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Упоминания сообщения                    |
| `pinnable`         | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)                                                                                                  | Является ли сообщение закрепляемым      |
| `type`             | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                                                                                                    | Тип сообщения                           |
| `url`              | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Ссылка на сообщение                     |

### MessageEmbed

| Свойство      | Тип                                                                                              | Описание                              |
| ------------- | ------------------------------------------------------------------------------------------------ | ------------------------------------- |
| `author`      | ?[MessageEmbedAuthor](data-types.md#messageembedauthor)                                          | Автор встроенного сообщения           |
| `color`       | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Цвет встроенного сообщения            |
| `description` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Описание встроенного сообщения        |
| `fields`      | ?array of  [MessageEmbedField](data-types.md#messageembedfield)                                  | Поля встроенного сообщения            |
| `footer`      | ?[MessageEmbedFooter](data-types.md#messageembedfooter)                                          | Футер встроенного сообщения           |
| `image`       | ?[MessageEmbedImage](data-types.md#messageembedimage)                                            | Изображение встроенного сообщения     |
| `thumbnail`   | ?[MessageEmbedImage](data-types.md#messageembedimage)                                            | Миниатюра встроенного сообщения       |
| `timestamp`   | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Временная метка встроенного сообщения |
| `title`       | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Заголовок встроенного сообщения       |
| `url`         | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка встроенного сообщения          |

#### MessageEmbedAuthor

| Свойство   | Тип                                                                                              | Описание              |
| ---------- | ------------------------------------------------------------------------------------------------ | --------------------- |
| `icon_url` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка на изображение |
| `name`     | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Имя автора            |
| `url`      | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка                |

#### MessageEmbedField

| Свойство | Тип                                                                                              | Описание                                 |
| -------- | ------------------------------------------------------------------------------------------------ | ---------------------------------------- |
| `inline` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Должно ли это поле отображаться в строке |
| `name`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Заголовок поля                           |
| `value`  | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Значение поля                            |

#### MessageEmbedFooter

| Свойство   | Тип                                                                                              | Описание              |
| ---------- | ------------------------------------------------------------------------------------------------ | --------------------- |
| `icon_url` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка на изображение |
| `text`     | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Текст футера          |

#### MessageEmbedImage

| Свойство | Тип                                                                                             | Описание              |
| -------- | ----------------------------------------------------------------------------------------------- | --------------------- |
| `url`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка на изображение |

## User

| Свойство           | Тип                                                                                             | Описание                          |
| ------------------ | ----------------------------------------------------------------------------------------------- | --------------------------------- |
| `id`               | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор пользователя        |
| `username`         | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Имя пользователя                  |
| `discriminator`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Дискриминатор пользователя        |
| `avatar`           | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка на аватар пользователя     |
| `createdTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Временная метка создания аккаунта |

## UserActivity

| Свойство | Тип                                                                                                       | Описание                     |
| -------- | --------------------------------------------------------------------------------------------------------- | ---------------------------- |
| `level`  | [UserLevel](data-types.md#userlevel)                                                                      | Уровень пользователя         |
| `wallet` | array of [numbers](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Баланс кошелька пользователя |

### UserLevel

| Свойство         | Тип                                                                                             | Описание                                                          |
| ---------------- | ----------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| `rank`           | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Текущий уровень пользователя                                      |
| `current_xp`     | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Текущее количество опыта                                          |
| `total_xp`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Общее количество опыта                                            |
| `total_messages` | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Общее количество отправленных сообщений                           |
| `voice_time`     | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Количество времени, проведенного в голосовых каналах (в секундах) |

## VoiceState

| Свойство     | Тип                                                                                                | Описание                                  |
| ------------ | -------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| `channelId`  | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор канала голосового состояния |
| `deaf`       | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли звук                          |
| `id`         | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор участника                   |
| `mute`       | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли микрофон                      |
| `selfDeaf`   | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли звук локально                 |
| `selfMute`   | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли микрофон локально             |
| `selfVideo`  | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Включено ли видео                         |
| `serverDeaf` | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли звук глобально                |
| `serverMute` | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Отключён ли микрофон глобально            |
| `streaming`  | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Запущен ли стрим                          |

## MessageOptions

| Свойство     | Тип                                                                                                                          | Описание                    |
| ------------ | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------- |
| `content`    | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                             | Содержание сообщения        |
| `embeds`     | ?array of [MessageEmbed](data-types.md#messageembed)                                                                         | Массив встроенных сообщений |
| `components` | ?array of [ComponentButton](data-types.md#componentbutton)\[] or [ComponentSelectMenu](data-types.md#componentselectmenu)\[] | Компоненты сообщения        |

## ReplyOptions

расширяет [MessageOptions](data-types.md#messageoptions)

| Свойство    | Тип                                                                                                | Описание            |
| ----------- | -------------------------------------------------------------------------------------------------- | ------------------- |
| `tts`       | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Text-to-speech      |
| `ephemeral` | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Эфемерное сообщение |

## CreateChannelOptions

| Свойство           | Тип                                                                                                | Описание                                                                                                     |
| ------------------ | -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| `name`             | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Название канала                                                                                              |
| `type`             | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Тип канала. 0 - текстовый, 2 - голосовой, 4 - категория, 5 - новостной, 13 - трибуна, 15 - форум, 16 - медиа |
| `topic`            | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Заголовок канала                                                                                             |
| `nsfw`             | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Ограничение по возрасту                                                                                      |
| `bitrate`          | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Битрейт канала                                                                                               |
| `userLimit`        | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Лимит пользователей                                                                                          |
| `position`         | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Позиция канала                                                                                               |
| `rateLimitPerUser` | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Слоумод                                                                                                      |
| `parent`           | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Категория канала                                                                                             |

## CreateThreadOptions

| Свойство    | Тип                                                                                              | Описание                                                                                           |
| ----------- | ------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------- |
| `name`      | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Название канала                                                                                    |
| `message`   | ?[MessageOptions](data-types.md#messageoptions)                                                  | Объект сообщения. В случае создания ветки в форуме. Взаимозаменяемые со свойством `messageId`      |
| `messageId` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор сообщения, для которого будет создана ветка. Взаимозаменяемые со свойством `message` |

## DeferReplyOptions

| Свойство    | Тип                                                                                                | Описание            |
| ----------- | -------------------------------------------------------------------------------------------------- | ------------------- |
| `ephemeral` | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Эфемерное сообщение |

## ShowModalOptions

| Свойство     | Тип                                                                                             | Описание                      |
| ------------ | ----------------------------------------------------------------------------------------------- | ----------------------------- |
| `title`      | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Заголовок модального окна     |
| `customId`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор модального окна |
| `components` | array of [ComponentTextInput](data-types.md#componenttextinput)\[]                              | Компоненты модального окна    |

## ComponentButton

| Свойство   | Тип                                                                                                | Описание                                  |
| ---------- | -------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| `type`     | `'Button'`                                                                                         | Тип компонента                            |
| `customId` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Пользовательский идентификатор компонента |
| `disabled` | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Состояние компонента                      |
| `emoji`    |                                                                                                    | Эмодзи компонента                         |
| `label`    | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Название компонента                       |
| `style`    | `'Danger'` or `'Link'` or `'Primary'` or `'Secondary'` or `'Success'`                              | Стиль кнопки                              |
| `url`      | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Ссылка кнопки                             |

## ComponentSelectMenu

| Свойство      | Тип                                                                                                | Описание                                  |
| ------------- | -------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| `type`        | `'SelectMenu'`                                                                                     | Тип компонента                            |
| `customId`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Пользовательский идентификатор компонента |
| `disabled`    | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Состояние компонента                      |
| `maxValues`   | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Максимум выбранных опций                  |
| `minValues`   | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Минимум выбранных опций                   |
| `options`     | array of [SelectMenuOption](data-types.md#selectmenuoption)                                        | Опции выпадающего списка                  |
| `placeholder` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Заполнитель выпадающего списка            |

### SelectMenuOption

| Свойство      | Тип                                                                                                | Описание           |
| ------------- | -------------------------------------------------------------------------------------------------- | ------------------ |
| `default`     | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Опция по умолчанию |
| `description` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Описание опции     |
| `emoji`       | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Эмодзи опции       |
| `label`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Название опции     |
| `value`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Значение опции     |

## ComponentTextInput

| Свойство      | Тип                                                                                                | Описание                                  |
| ------------- | -------------------------------------------------------------------------------------------------- | ----------------------------------------- |
| `type`        | `'TextInput'`                                                                                      | Тип компонента                            |
| `customId`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Пользовательский идентификатор компонента |
| `label`       | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)    | Название поля                             |
| `maxLength`   | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Максимальное количество символов          |
| `minLength`   | ?[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Минимальное количество символов           |
| `placeholder` | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Заполнитель поля                          |
| `required`    | ?[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Обязательное поле                         |
| `style`       | `'Short'` or `'Paragraph'`                                                                         | Стиль поля                                |
| `value`       | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Значение поля                             |
