# Аргумент длительности

## Формат

`<число><буква>`

Число – это количество минут/часов/дней и т.д. Число необязательно должно быть целым - можно использовать `0.5h` для указания 30 минут (полчаса).

Буква влияет непосредственно на то, в чём будет измеряться время — в секундах, минутах, часах и т.п.

Число и букву писать нужно слитно.

#### Доступные величины

| Тип                                                                                                                                    | Величина     |
| -------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| <p><code>ms</code></p><p><code>msec</code></p><p><code>msecs</code></p><p><code>millisecond</code></p><p><code>milliseconds</code></p> | Миллисекунды |
| <p><code>s</code></p><p><code>sec</code></p><p><code>secs</code></p><p><code>second</code></p><p><code>seconds</code></p>              | Секунды      |
| <p><code>m</code></p><p><code>min</code></p><p><code>mins</code></p><p><code>minute</code></p><p><code>minutes</code></p>              | Минуты       |
| <p><code>h</code></p><p><code>hr</code></p><p><code>hrs</code></p><p><code>hour</code></p><p><code>hours</code></p>                    | Часы         |
| <p><code>d</code></p><p><code>day</code></p><p><code>days</code></p>                                                                   | Дни          |
| <p><code>w</code></p><p><code>week</code></p><p><code>weeks</code></p>                                                                 | Недели       |
| <p><code>y</code></p><p><code>yr</code></p><p><code>yrs</code></p><p><code>year</code></p><p><code>years</code></p>                    | Годы         |

#### Примеры

`30s` — 30 секунд\
`15m` — 15 минут\
`0.25d` — 6 часов\
`12h` — 12 часов\
`2w` — 2 недели
