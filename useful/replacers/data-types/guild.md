# Guild

## .afk\_channel\_id

Идентификатор голосового канала, в который перемещаются AFK участники.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .banner

Ссылка на баннер сервера.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .boost\_tier

Уровень буста сервера.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .booster\_count

Количество бустеров на сервере.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .channels

Список каналов на сервере.

```javascript
// замените <channel_id> на идентификатор нужного канала
{ guild.channels.<channel_id>.name }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)\<string, [Channel](channel.md)>

## .created\_at

Дата создания сервера.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .description

Описание сервера.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .discovery\_splash

Ссылка на заставку сервера в путешествии.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .icon

Ссылка на иконку сервера.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .id

Идентификатор сервера.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .member\_count

Количество участников на сервере.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .name

Название сервера.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .name\_acronym

Акроним названия сервера.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .owner

Владелец сервера.

[GuildOwner](guildowner.md)

## .presence\_count

Количество участников на сервере, которые имеют статус в сети.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .public\_updates\_channel\_id

Идентификатор канала для публичных обновлений.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .rules\_channel\_id

Идентификатор канала с правилами.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .safety\_alerts\_channel\_id

Идентификатор канала для уведомлений о безопасности.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .splash

Ссылка на заставку для приглашений.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .system\_channel\_id

Идентификатор системного канала.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .vanity\_url

Ссылка на пользовательское приглашение.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .voice\_connection\_count

Количество участников на сервере, которые находятся в голосовом канале.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)
