# Временные метки

_Автор: Aleх#0001_

Как вы знаете, заменители `created_at` участника сервера, сообщения, гильдии и `joined_at` участника сервера возвращают время в миллисекундах от 1 января 1970 года — Unix-время. Конвертировать эти числа в понятную для человека дату можно двумя способами: используя [временные метки Discord `<t:Unix-время>`](https://discord.com/developers/docs/reference#message-formatting-timestamp-styles) или [функцию-заменитель `DATE`](https://docs.lacunabot.com/useful/replacers/functions#date).

### **Временные метки Discord** <a href="#discord-timestamps" id="discord-timestamps"></a>

Для использования временных меток Discord вам потребуется лишь вставить `<t:{- MATH("ТРЕБУЕМЫЙ_ЗАМЕНИТЕЛЬ / 1000") -}:D>` в то место, где вы хотите использовать заменитель и заменить `ТРЕБУЕМЫЙ_ЗАМЕНИТЕЛЬ` на желаемый вами заменитель.

### **Функция-заменитель `DATE`** <a href="#date-function" id="date-function"></a>

Указание же даты через заменитель окажется куда проще — вам всего лишь требуется вставить `{- DATE("{ТРЕБУЕМЫЙ_ЗАМЕНИТЕЛЬ}") -}` и так же заменить `ТРЕБУЕМЫЙ_ЗАМЕНИТЕЛЬ` на тот заменитель, который вы хотите использовать.
