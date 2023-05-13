# Функции

## setValue(_key, value_): _void_

Устанавливает данные на основе ключа. Если ключа не существует, то он будет создан, в ином случае перезапишет данные ключа.

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ</td></tr><tr><td><code>value</code></td><td>any</td><td>true</td><td>Значение</td></tr></tbody></table>

```javascript
{{ setValue('data.balance', 500) }}
{{ setValue('data.name', 'Hello World!') }}
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}
```

{% hint style="warning" %}
Данную функцию можно вызвать только 5 раз в одной пользовательской команде.
{% endhint %}

## getValue(_key_): _Promise\<any>_

Возвращает данные на основе указанного ключа.

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ getValue('data.balance').then(value => { /* do something */ }) }}
{{ getValue('data.name').then(value => { /* do something */ }) }}
{{ getValue('data').then(value => { /* do something */ }) }}
```

## deleteValue(_key_): _void_

Удаляет данные на основе указанного ключа.

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ deleteValue('data.balance') }}
{{ deleteValue('data') }}
```

## deferReply(options): _Promise\<void>_

Откладывает ответ на команду

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td>partial <a href="https://discord.com/developers/docs/resources/channel#create-message-jsonform-params">ReplyOptions</a></td><td>false</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 1 раз в одной пользовательской команде.
{% endhint %}

## deleteReply(): _Promise\<void>_

Удаляет ответ на команду

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 1 раз в одной пользовательской команде.
{% endhint %}

## editReply(options): _Promise\<void>_

Редактирует ответ на команду

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="https://discord.com/developers/docs/resources/channel#create-message-jsonform-params">ReplyOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 3 раза в одной пользовательской команде.
{% endhint %}

## followUpReply(options): _Promise\<void>_

Отправляет последующий ответ на команду

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="https://discord.com/developers/docs/resources/channel#create-message-jsonform-params">ReplyOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 3 раза в одной пользовательской команде.
{% endhint %}

## getUserActivity(userId): _Promise<_[_UserActivity_](data-types.md#useractivity)_>_

Получает активность пользователя

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 3 раза в одной пользовательской команде.
{% endhint %}

## reply(options): _Promise\<void>_

Отправляет ответ на команду

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="https://discord.com/developers/docs/resources/channel#create-message-jsonform-params">ReplyOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 1 раз в одной пользовательской команде.
{% endhint %}

## modifyUserRoles(userId, roles, mode): _Promise\<void>_

Редактирует роли пользователя

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя, которому будут изменены роли</td></tr><tr><td><code>roles</code></td><td>array of <a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">strings</a></td><td>true</td><td>Роли, которые будут добавлены/убраны/установлены</td></tr><tr><td><code>mode</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>false</td><td>Режим функции. <code>add</code> - добавить, <code>remove</code> - убрать, <code>set</code> - установить. По умолчанию <code>add</code></td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 1 раз в одной пользовательской команде.
{% endhint %}

## modifyUserWallet(userId, amount, currencyId): _Promise\<void>_

Добавляет/отнимает валюту у пользователя

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя, которому будет изменен кошелёк</td></tr><tr><td><code>amount</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Number">number</a></td><td>true</td><td>Количество валюты, которое будет добавлено или убрано. Негативное число отнимает валюту</td></tr><tr><td><code>currencyId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>false</td><td>Идентификатор валюты. По умолчанию <code>DEFAULT</code></td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 2 раза в одной пользовательской команде.
{% endhint %}

## sendMessage(channelId, options): _Promise<_[_Message_](data-types.md#message)_>_

Отправляет сообщение в указанный канал

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>channelId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор канала, в который будет отправлено сообщение</td></tr><tr><td><code>options</code></td><td><a href="https://discord.com/developers/docs/resources/channel#create-message-jsonform-params">MessageOptions</a></td><td>true</td><td>Опции для сообщения</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

{% hint style="warning" %}
Данную функцию можно вызвать только 2 раза в одной пользовательской команде.
{% endhint %}
