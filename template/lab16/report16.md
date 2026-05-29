---
## Front matter
title: "Лабораторная работа 16"
subtitle: "Администрирование локальных сетей"
author: "Ромицына Анастасия Романовна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Введение

Получение навыков настройки VPN-туннеля через незащищённое Интернетсоединение.

# Выполнение лаборатаорной работы

Разместим в рабочей области проекта оборудование для сети Университета г. Пиза
(рис. [-@fig:001]).

![Размещение объектов](image/1.png){#fig:001 width=40%}

В физической рабочей области проекта создадим город Пиза, здание Университета г. Пиза.(рис. [-@fig:002]).

![Размещение объектов](image/2.png){#fig:002 width=70%}

Переместим туда соответствующее оборудование
 (рис. [-@fig:003]).

![Перемещение оборудования](image/3.png){#fig:003 width=70%}

Первоначальная настройка маршрутизатора pisa-unipi-gw-1 (рис. [-@fig:004]).

![Первоначальная настройка](image/4.png){#fig:004 width=70%}

Первоначальная настройка коммутатора pisa-unipi-sw-1
(рис. [-@fig:005]).

![Первоначальная настройка коммутатора pisa-unipi-sw-1](image/5.png){#fig:005 width=70%}

Настройка интерфейсов маршрутизатора pisa-unipi-gw-1 (рис. [-@fig:006]).

![Настройка интерфейсов маршрутизатора pisa-unipi-gw-1](image/6.png){#fig:006 width=70%}

Настройка интерфейсов коммутатора pisa-unipi-sw-1 (рис. [-@fig:007]).

![Настройка интерфейсов коммутатора pisa-unipi-sw-1](image/7.png){#fig:007 width=70%}

Настройка маршрутизатора msk-donskaya-gw-1 (рис.[-@fig:008]).

![Настройка маршрутизатора msk-donskaya-gw-1](image/8.png){#fig:008 width=70%}

Настройка интерфейсов маршрутизатора pisa-unipi-gw-1
(рис. [-@fig:009]).

![Настройка интерфейсов маршрутизатора pisa-unipi-gw-1](image/009.png){#fig:009 width=70%}

Проверка
(рис. [-@fig:010]).

![Проверка](image/010.png){#fig:010 width=70%}

# Вывод

Мы смогли получить навыки настройки VPN-туннеля через незащищённое Интернетсоединение.

# Контрольные вопросы

1. Что такое VPN?
   VPN (Virtual Private Network) — это технология для создания защищённого (зашифрованного) соединения между устройством и сетью через интернет.

2. В каких случаях следует использовать VPN?
   Для защиты данных в публичных Wi-Fi, обхода блокировок, скрытия реального IP-адреса и безопасного доступа к корпоративной сети.

3. Как с помощью VPN обойти NAT?
   VPN-клиент устанавливает исходящее соединение с VPN-сервером, которое не блокируется NAT (т.к. идёт «наружу»). Сервер присваивает устройству внутренний IP и перенаправляет обратный трафик через уже открытый канал, минуя ограничения NAT на входящие подключения.

# Список литературы{.unnumbered}

::: {#refs}
:::
