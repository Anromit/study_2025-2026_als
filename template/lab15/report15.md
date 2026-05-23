---
## Front matter
title: "Лабораторная работа 15"
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

Настроить динамическую маршрутизацию между территориями организации.

# Выполнение лаборатаорной работы

 Настройка маршрутизатора msk-donskaya-gw-1
(рис. [-@fig:001]).

![Настройка msk-donskaya-gw-1](image/1.png){#fig:001 width=40%}

Проверка состояния протокола OSPF на маршрутизаторе msk-donskaya-gw-1(рис. [-@fig:002]).

![Проверка msk-donskaya-gw-1](image/2.png){#fig:002 width=70%}

Настройка маршрутизатора msk-q42-gw-1
 (рис. [-@fig:003]).

![Настройка msk-q42-gw-1](image/3.png){#fig:003 width=70%}

Настройка маршрутизирующего коммутатора
msk-hostel-gw-1 (рис. [-@fig:004]).

![Настройка msk-hostel-gw-1](image/4.png){#fig:004 width=70%}

Настройка маршрутизатора sch-sochi-gw-1
(рис. [-@fig:005]).

![Настройка sch-sochi-gw-1](image/5.png){#fig:005 width=70%}

Настройка интерфейсов коммутатора provider-sw-1 (рис. [-@fig:006]).

![Настройка provider-sw-1](image/6.png){#fig:006 width=70%}

Настройка маршрутизатора msk-q42-gw-1
 (рис. [-@fig:007]).

![Настройка msk-q42-gw-1](image/7.png){#fig:007 width=70%}

Настройка коммутатора sch-sochi-sw-1 (рис.[-@fig:008]).

![Настройка sch-sochi-sw-1](image/8.png){#fig:008 width=70%}

Настройка маршрутизатора sch-sochi-gw-1
(рис. [-@fig:009]).

![Настройка sch-sochi-gw-1](image/9.png){#fig:009 width=70%}

Проверка
(рис. [-@fig:010]).

![Проверка](image/10.png){#fig:010 width=70%}

# Вывод

Мы смогли настроить динамическую маршрутизацию между территориями организации.

# Контрольные вопросы

1. Протоколы динамической маршрутизации:
RIP, OSPF, EIGRP (Cisco), IS-IS, BGP.

2. Принципы работы:
Маршрутизаторы автоматически обмениваются информацией о известных сетях, строят карту топологии, рассчитывают оптимальные маршруты на основе метрик (например, количество прыжков, пропускная способность) и обновляют таблицы маршрутизации при изменении сети.

3. Обращение устройства из одной подсети к устройству из другой:
Устройство-отправитель отправляет пакет на свой шлюз по умолчанию. Маршрутизатор получает пакет, смотрит в таблицу маршрутизации (заполненную динамически), находит подходящий маршрут до сети назначения и пересылает пакет следующему маршрутизатору, пока пакет не достигнет целевой подсети.

4. Выводимая информация при просмотре таблицы маршрутизации:

Сеть назначения (Destination)

Маска подсети (Netmask)

Адрес следующего шлюза (Gateway/Next-hop)

Интерфейс выхода (Interface)

Метрика (Metric)

Тип маршрута (статический, динамический, по умолчанию)

Источник протокола маршрутизации (например, OSPF, RIP).

# Список литературы{.unnumbered}

::: {#refs}
:::
