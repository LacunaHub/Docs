# Глобальные переменные

## Command

Данный объект содержит в себе информацию о вызове текущей команды.

| Свойство  | Тип                                                                                             | Описание                     |
| --------- | ----------------------------------------------------------------------------------------------- | ---------------------------- |
| `id`      | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор команды        |
| `name`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Название команды             |
| `options` | array of [options](global-variables.md#undefined)                                               | Переданные аргументы команды |

### Option

| Свойство  | Тип                                                                                                                                                                                                                                                                                                   | Описание                                                 |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| `name`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                                                                                                                       | Название аргумента                                       |
| `value`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) or [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Значение аргумента                                       |
| `user`    | ?[user](global-variables.md#user)                                                                                                                                                                                                                                                                     | Упомянутый пользователь, если тип аргумента ПОЛЬЗОВАТЕЛЬ |
| `channel` | ?[channel](global-variables.md#channel)                                                                                                                                                                                                                                                               | Упомянутый канал, если тип аргумента КАНАЛ               |
| `role`    | ?[role](global-variables.md#role)                                                                                                                                                                                                                                                                     | Упомянутая роль, если тип аргумента РОЛЬ                 |

## Channel

Информация о канале в котором была вызвана команда.

| Свойство           | Тип                                                                                               | Описание                                    |
| ------------------ | ------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| `id`               | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Идентификатор канала                        |
| `name`             | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)   | Название канала                             |
| `type`             | [ChannelType](https://discord.com/developers/docs/resources/channel#channel-object-channel-types) | Тип канала                                  |
| `parentId`         | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Идентификатор категории канала              |
| `nsfw`             | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean) | Ограничение по возрасту                     |
| `position`         | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Позиция канала относительно других          |
| `topic`            | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Тема канала                                 |
| `lastMessageId`    | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)  | Идентификатор последнего сообщения в канале |
| `rateLimitPerUser` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Медленные режим в секундах                  |
| `createdTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)   | Временная метка создания канала             |

## Guild

Информация о текущем сервере

| Свойство                      | Тип                                                                                                                                                                                                | Описание                                    |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| `id`                          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Идентификатор сервера                       |
| `name`                        | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Название сервера                            |
| `nameAcronym`                 | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                    | Инициалы сервера                            |
| `icon`                        | ?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                                                                                                   | Ссылка на иконку сервера                    |
| `channels`                    | array of [channels](global-variables.md#obekt-channel)                                                                                                                                             | Каналы сервера                              |
| `roles`                       | array of [roles](global-variables.md#undefined)                                                                                                                                                    | Роли сервера                                |
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
| `economyCurrencies`           | array of [currencies](global-variables.md#undefined)                                                                                                                                               | Валюты экономики                            |

### Role

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

### Currency

| Свойство | Тип                                                                                             | Описание             |
| -------- | ----------------------------------------------------------------------------------------------- | -------------------- |
| `id`     | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор валюты |
| `name`   | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Название валюты      |
| `symbol` | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Символ валюты        |

## Member

| Свойство          | Тип                                                                                                                 | Описание                                |
| ----------------- | ------------------------------------------------------------------------------------------------------------------- | --------------------------------------- |
| `user`            | [user](global-variables.md#undefined)                                                                               | Информация о пользователе               |
| `avatar`          | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                     | Ссылка на серверный аватар              |
| `nickname`        | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)                     | Никнейм участника                       |
| `pending`         | [boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)                   | Прошел ли участник отбор                |
| `roles`           | array of [roles](global-variables.md#undefined)                                                                     | Роли участника                          |
| `permissions`     | array of [permissions](https://discord.com/developers/docs/topics/permissions#permissions-bitwise-permission-flags) | Разрешения участника                    |
| `joinedTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)                     | Временная метка присоединения к серверу |

### User

| Свойство           | Тип                                                                                             | Описание                          |
| ------------------ | ----------------------------------------------------------------------------------------------- | --------------------------------- |
| `id`               | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Идентификатор пользователя        |
| `username`         | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Имя пользователя                  |
| `discriminator`    | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Дискриминатор пользователя        |
| `avatar`           | [string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String) | Ссылка на аватар пользователя     |
| `createdTimestamp` | [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number) | Временная метка создания аккаунта |
