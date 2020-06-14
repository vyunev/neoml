# Класс CConcatChannelsLayer

<!-- TOC -->

- [Класс CConcatChannelsLayer](#класс-cconcatchannelslayer)
    - [Настройки](#настройки)
    - [Обучаемые параметры](#обучаемые-параметры)
    - [Входы](#входы)
    - [Выходы](#выходы)

<!-- /TOC -->

Класс реализует слой, объединяющий блобы своих входов по оси `Channels`.

## Настройки

Слой не имеет настроек.

## Обучаемые параметры

Слой не имеет обучаемых параметров.

## Входы

На входы слоя подаются блобы размеров:

- `BatchLength`, `BatchWidth`, `ListSize`, `Height`, `Width`, `Depth` должны быть равны у блобов всех входов;
- `Channels` могут различаться.

## Выходы

Единственный выход будет содержать блоб размера:

- `BatchLength`, `BatchWidth`, `ListSize`, `Height`, `Width`, `Depth` равны аналогичным у входов;
- `Channels` равен сумме `Channels` всех входов.