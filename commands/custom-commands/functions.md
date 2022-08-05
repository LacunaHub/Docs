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

## getValue(_key_): _any_

Возвращает данные на основе указанного ключа.

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ getValue('data.balance') }} // 500
{{ getValue('data.name') }} // Hello World!
{{ getValue('data') }} // { balance: 500, name: 'Hello World!' }
```

## deleteValue(_key_): _void_

Удаляет данные на основе указанного ключа.

<table><thead><tr><th>Параметр</th><th>Тип</th><th data-type="checkbox">Обязательный</th><th>Описание</th></tr></thead><tbody><tr><td><code>key</code></td><td><a href="https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/String">string</a></td><td>true</td><td>Ключ значения</td></tr></tbody></table>

```javascript
{{ setValue('data', { balance: 500, name: 'Hello World!' }) }}

{{ deleteValue('data.balance') }}
{{ deleteValue('data') }}
```
