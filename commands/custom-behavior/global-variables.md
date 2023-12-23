---
layout:
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# Глобальные переменные

## channel

Канал события

[Channel](data-types/channel.md)

## guild

Объект сервера.

[Guild](data-types/guild.md)

## member

Участник, который инициировал событие.

[Member](data-types/member.md)

## interaction

Объект взаимодействия. Доступно только в автоматизации для триггеров `INTERACTION_BUTTON`, `INTERACTION_SELECT_MENU` и `INTERACTION_MODAL_SUBMIT`.

Interaction

## message

Объект сообщения. Доступно только в автоматизации для триггеров `MESSAGE_CREATE`, `MESSAGE_DELETE` и `MESSAGE_UPDATE`.

Message

## voiceState

Объект голосового состояния. Доступно только в автоматизации для триггеров `VOICE_CONNECT` и `VOICE_DISCONNECT`.

VoiceState
