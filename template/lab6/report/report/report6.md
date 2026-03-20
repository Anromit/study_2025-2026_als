---
## Front matter
title: "Лабораторная работа 6"
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

Настроить статическую маршрутизацию VLAN в сети.

# Выполнение лаборатаорной работы

В логической области проекта разместим маршрутизатор Cisco 2811(рис. [-@fig:001]).

![Размещение маршрутизатора Cisco 2811 в логической области проекта](image/1.png){#fig:001 width=70%}

Общая схема сети (рис. [-@fig:002]).

![Общая схема](image/2.png){#fig:002 width=70%}

Подключим его к порту 24 коммутатора msk-donskaya-arromichina-sw-1 в
соответствии с таблицей портов(рис. [-@fig:003]).

![Подключение его к порту 24 коммутатора msk-donskaya-arromichina-sw-1.](image/3.png){#fig:003 width=70%}

Используя приведённую ниже последовательность команд по первоначальной настройке маршрутизатора, сконфигурируем маршрутизатор, задав на
нём имя, пароль для доступа к консоли, настроим удалённое подключение
к нему по ssh(рис. [-@fig:004]).

![Настройка добавленного устройства](image/4.png){#fig:004 width=70%}

 Настроим порт 24 коммутатора msk-donskaya-sw-1 как trunk-порт(рис. [-@fig:005]).

![Настройка порта коммутатора как trunk порт](image/5.png){#fig:005 width=70%}

На интерфейсе f0/0 маршрутизатора msk-donskaya-arromichina-gw-1 настроим виртуальные интерфейсы, соответствующие номерам VLAN. Согласно таблице IP-адресов (см. табл. 3.2 из раздела 3.3) зададим соответствующие IP-адреса на виртуальных интерфейсах. Для этого используем приведённую в лабораторной работе последовательность команд по конфигурации VLAN-интерфейсов маршрутизатора.(рис. [-@fig:006]).

![Настройка виртуальных интерфейсов, задание IP-адресов](image/6.png){#fig:006 width=70%}

Проверим доступность оконечных устройств из разных VLAN(рис. [-@fig:007]).

![Проверяем проделанную работу](image/7.png){#fig:007 width=70%}

Используя режим симуляции в Packet Tracer, изучим процесс передвижения пакета ICMP по сети. Изучим содержимое передаваемого пакета
и заголовки задействованных протоколов(рис. [-@fig:008]).

![Изучение процесса прердвижения пакета](image/8.png){#fig:008 width=70%}

# Вывод

Мы смогли настроить статическую маршрутизацию VLAN в сети.

# Контрольные вопросы

1 Охарактеризуйте стандарт IEEE 802.1Q - открытый стандарт,
который описывает процедуру тегирования трафика для передачи
информации о принадлежности к VLAN по сетям стандарта IEEE
802.3 Ethernet.

2 Опишите формат кадра IEEE 802.1Q - добавляет 32-битное поле
между MAC-адресом источника и полями EtherType исходного
кадра. В соответствии с 802.1Q минимальный размер кадра
остается 64 байта, но мост может увеличить минимальный размер
кадра с 64 до 68 байтов при передаче IEEE 802.1Q.

# Список литературы{.unnumbered}

::: {#refs}
:::
