# Member

## .avatar

Ссылка на аватар участника.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .bot

Является ли участник ботом.

[boolean](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Boolean)

## .created\_at

Дата создания аккаунта участника.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .display\_name

Отображаемое имя участника.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .id

Идентификатор участника.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .joined\_at

Дата присоединения к серверу.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .level

Уровень участника.

[MemberLevel](memberlevel.md)

## .mention

Упоминание участника.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .nickname

Никнейм участника.

?[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .premium\_since

Дата начала подписки Discord Nitro.

[number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)

## .roles

Роли участника

```javascript
// замените <role_id> на идентификатор нужной роли
{ member.roles.<role_id>.name }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)<[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [Role](role.md)>

## .username

Имя пользователя участника.

[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String)

## .voice

Голосовой канал участника.

?[MemberVoice](membervoice.md)

## .wallet

Кошелёк участника.

```
// замените <currency_id> на идентификатор нужной валюты
{ member.wallet.<currency_id> }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)<[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [number](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/Number)>
