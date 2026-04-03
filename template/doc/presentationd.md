---
## Front matter
lang: ru-RU
title: Использование протокола STP. Агрегирование каналов.
subtitle: Администрирование локальных сетей
author:
  - Ромицына А. Р.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 30 марта 2026

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'

## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Ромицына Анастасия Романовна
  * НПИбд-02-23 Студ. билет: 1132236132
  * Российский университет дружбы народов
  * [1132236132@pfur.ru](mailto:1132236132@pfur.ru)

:::
::: {.column width="30%"}
:::
::::::::::::::

## Проблема: что будет без STP?

Широковещательный шторм — парализует сеть

Нестабильность MAC-таблицы

Резервные связи = риск петель

## Решение: STP (Spanning Tree Protocol)

Оставляет активным один путь

Остальные — блокирует (горячий резерв)

Автоматическое восстановление при обрыве

![Spanning Tree Protocol](./image/1.jpg)

## Роли портов и состояния

Роль	      -   Назначение
Root Port	-     путь к корневому мосту
Designated	-   пересылает в сегменте
Alternate	-   заблокирован (запасной)

## Эволюция STP (какую версию брать?)

Версия	Время перестройки
STP (802.1D)	до 50 сек 
RSTP (802.1w)	1–6 сек 
MSTP (802.1s)	группы VLAN
В современных сетях используем RSTP (быстро) или MSTP (экономит CPU)

## Защита от ошибок STP

BPDU Guard — блокирует порт с чужим коммутатором (для портов к ПК)

Root Guard — запрещает захват корневого моста

Loop Guard — защита при пропаже BPDU

## Агрегирование каналов (Link Aggregation)

Скорость = сумма портов (2 × 1 Гбит/с = 2 Гбит/с)

При отказе одного порта — остальные работают

Балансировка нагрузки по хэшу

![Link Aggregation](./image/2.jpg)

##  LACP (802.3ad) — открытый стандарт

LACP — протокол переговоров

Устройства сами создают группу

Альтернатива: статический LAG (ручной)

## Балансировка нагрузки в LAG

Хэш от	Когда использовать
src-ip	много клиентов
dst-ip	один сервер
src-dst-ip	универсально 
src-dst-port	максимальная детализация

##  Взаимодействие STP и LAG

STP блокирует / переводит весь LAG целиком

Добавление/удаление физического порта — без перестройки дерева

Резервный LAG можно держать заблокированным через STP

# Итоги
## Итоги

STP (RSTP/MSTP) — обязателен при резервных связях, иначе петли и коллапс сети.

Защитные механизмы (BPDU Guard, Root Guard) — стандарт безопасности.

LACP — увеличивает пропускную способность без изменения топологии.

STP + LAG работают вместе: LAG ускоряет, STP страхует от петель.


