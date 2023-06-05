# Функции

## setValue(key, value): _void_ <a href="#setvalue" id="setvalue"></a>

Устанавливает данные на основе ключа. Если ключа не существует, то он будет создан, в ином случае перезапишет данные ключа.

<table><thead><tr><th width="193.7142857142857">Параметр</th><th width="150">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ</td></tr><tr><td><code>value</code></td><td>any</td><td>true</td><td>Значение</td></tr></tbody></table>

```javascript
{{ setValue('data.balance', 500) }}
{{ setValue('data.name', 'Hello World!') }}
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}
```

## getValue(key): _Promise\<any>_ <a href="#getvalue" id="getvalue"></a>

Возвращает данные на основе указанного ключа.

<table><thead><tr><th width="193.7142857142857">Параметр</th><th width="150">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ getValue('data.balance').then(value => { /* do something */ }) }}
{{ getValue('data.name').then(value => { /* do something */ }) }}
{{ getValue('data').then(value => { /* do something */ }) }}
```

## deleteValue(key): _void_ <a href="#deletevalue" id="deletevalue"></a>

Удаляет данные на основе указанного ключа.

<table><thead><tr><th width="193.7142857142857">Параметр</th><th width="150">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ deleteValue('data.balance') }}
{{ deleteValue('data') }}
```

## deferReply(options): _Promise\<void>_ <a href="#deferreply" id="deferreply"></a>

Откладывает ответ на команду

<table><thead><tr><th width="208">Параметр</th><th width="192">Тип</th><th width="153" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="data-types.md#deferreplyoptions">DeferReplyOptions</a></td><td>false</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## deferUpdate(): _Promise\<void>_ <a href="#deferupdate" id="deferupdate"></a>

Откладывает обновление сообщения, к которому был привязан компонент

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## deleteReply(): _Promise\<void>_

Удаляет ответ на команду

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## editReply(options): _Promise\<void>_ <a href="#editreply" id="editreply"></a>

Редактирует ответ на команду

<table><thead><tr><th>Параметр</th><th width="164">Тип</th><th width="153" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="data-types.md#messageoptions">MessageOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## followUpReply(options): _Promise\<void>_ <a href="#followupreply" id="followupreply"></a>

Отправляет последующий ответ на команду

<table><thead><tr><th>Параметр</th><th width="135">Тип</th><th width="153" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="data-types.md#replyoptions">ReplyOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## getUserActivity(userId): _Promise<_[_UserActivity_](data-types.md#useractivity)_>_ <a href="#getuseractivity" id="getuseractivity"></a>

Получает активность пользователя

<table><thead><tr><th>Параметр</th><th width="163">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## reply(options): _Promise\<void>_ <a href="#reply" id="reply"></a>

Отправляет ответ на команду

<table><thead><tr><th>Параметр</th><th width="135">Тип</th><th width="153" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="data-types.md#replyoptions">ReplyOptions</a></td><td>true</td><td>Опции для ответа</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## showModal(options): _Promise\<void>_ <a href="#showmodal" id="showmodal"></a>

Отображает модальный компонент

<table><thead><tr><th>Параметр</th><th width="181">Тип</th><th width="153" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>options</code></td><td><a href="data-types.md#showmodaloptions">ShowModalOptions</a></td><td>true</td><td>Опции модального окна</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## modifyUserRoles(userId, roles, mode): _Promise\<void>_ <a href="#modifyuserroles" id="modifyuserroles"></a>

Редактирует роли пользователя

<table><thead><tr><th>Параметр</th><th width="163">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя, которому будут изменены роли</td></tr><tr><td><code>roles</code></td><td>array of <a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">strings</a></td><td>true</td><td>Роли, которые будут добавлены/убраны/установлены</td></tr><tr><td><code>mode</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>false</td><td>Режим функции. <code>add</code> - добавить, <code>remove</code> - убрать, <code>set</code> - установить. По умолчанию <code>add</code></td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## modifyUserWallet(userId, amount, currencyId): _Promise\<void>_ <a href="#modifyuserwallet" id="modifyuserwallet"></a>

Добавляет/отнимает валюту у пользователя

<table><thead><tr><th>Параметр</th><th width="163">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>userId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор пользователя, которому будет изменен кошелёк</td></tr><tr><td><code>amount</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Number">number</a></td><td>true</td><td>Количество валюты, которое будет добавлено или убрано. Негативное число отнимает валюту</td></tr><tr><td><code>currencyId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>false</td><td>Идентификатор валюты. По умолчанию <code>DEFAULT</code></td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## sendMessage(channelId, options): _Promise<_[_Message_](data-types.md#message)_>_ <a href="#sendmessage" id="sendmessage"></a>

Отправляет сообщение в указанный канал

<table><thead><tr><th>Параметр</th><th width="163">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>channelId</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор канала, в который будет отправлено сообщение</td></tr><tr><td><code>options</code></td><td><a href="data-types.md#messageoptions">MessageOptions</a></td><td>true</td><td>Опции для сообщения</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}

## overwriteChannelPermissions(channelIds, permissions, userOrRole): _Promise\<void>_ <a href="#overwritechannelpermissions" id="overwritechannelpermissions"></a>

Переопределяет права выбранного канала для выбранного пользователя или роли

<table><thead><tr><th width="168">Параметр</th><th width="169">Тип</th><th width="150" data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>channelIds</code></td><td>array of <a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификаторы каналов для которых будут переопределены права</td></tr><tr><td><code>permissions</code></td><td><a href="https://discord.com/developers/docs/topics/permissions#permissions-bitwise-permission-flags">PermissionsFlags</a></td><td>true</td><td>Список прав, пример: <code>{VIEW_CHANNEL: false}</code></td></tr><tr><td><code>userOrRole</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Идентификатор роли или пользователя</td></tr></tbody></table>

{% hint style="info" %}
Данная функция доступна только для действия "Выполнить код".
{% endhint %}
