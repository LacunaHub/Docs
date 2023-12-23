# MessageMentions

## .channels

Список упоминаний каналов.

```
// замените <index> на порядковый номер упоминания
{ message.mentions.channels.<index>.name }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)<[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [Channel](channel.md)>

## .members

Список упоминаний участников.

```
// замените <index> на порядковый номер упоминания
{ message.mentions.members.<index>.display_name }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)<[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [Partial](https://www.typescriptlang.org/docs/handbook/utility-types.html#partialtype)<[Member](member.md)>>

## .roles

Список упоминаний ролей.

```
// замените <index> на порядковый номер упоминания
{ message.mentions.roles.<index>.name }
```

[Record](https://www.typescriptlang.org/docs/handbook/utility-types.html#recordkeys-type)<[string](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global\_Objects/String), [Role](role.md)>
