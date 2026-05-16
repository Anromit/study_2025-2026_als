---
## Front matter
title: "Лабораторная работа 14"
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

Настроить взаимодействие через сеть провайдера посредством статической
маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного
в г. Сочи

# Выполнение лаборатаорной работы

Настройка интерфейсов коммутатора provider-sw-1
(рис. [-@fig:001]).

![Настройка provider-sw-1](image/1.png){#fig:001 width=40%}

Настройка интерфейсов маршрутизатора msk-donskaya-gw-1(рис. [-@fig:002]).

![Настройка msk-donskaya-gw-1](image/2.png){#fig:002 width=70%}

Настройка интерфейсов маршрутизатора msk-q42-gw-1
 (рис. [-@fig:003]).

![Настройка msk-q42-gw-1](image/3.png){#fig:003 width=70%}

Настройка интерфейсов коммутатора sch-sochi-sw-1 (рис. [-@fig:004]).

![Настройка sch-sochi-sw-1](image/4.png){#fig:004 width=70%}

Настройка интерфейсов маршрутизатора sch-sochi-gw-1 (рис. [-@fig:005]).

![Настройка sch-sochi-gw-1](image/5.png){#fig:005 width=70%}

Настройка интерфейсов маршрутизатора msk-q42-gw-1
(рис. [-@fig:006]).

![Настройка msk-q42-gw-1](image/6.png){#fig:006 width=70%}

Настройка интерфейсов коммутатора msk-q42-sw-1 (рис. [-@fig:007]).

![Настройка msk-q42-sw-1](image/7.png){#fig:007 width=70%}

Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1
 (рис. [-@fig:008]).

![Настройка msk-hostel-gw-1](image/8.png){#fig:008 width=70%}

Настройка интерфейсов коммутатора msk-hostel-sw-1 (рис.[-@fig:009]).

![Настройка msk-hostel-sw-1](image/9.png){#fig:009 width=70%}

Настройка интерфейсов маршрутизатора sch-sochi-gw-1
(рис. [-@fig:010]).

![Настройка sch-sochi-gw-1](image/10.png){#fig:010 width=70%}

Настройка интерфейсов коммутатора sch-sochi-sw-1
(рис. [-@fig:011]).

![Настройка sch-sochi-sw-1](image/11.png){#fig:011 width=70%}

Настройка маршрутизатора msk-donskaya-gw-1
(рис. [-@fig:012]).

![Настройка msk-donskaya-gw-1](image/12.png){#fig:012 width=70%}

Настройка маршрутизатора msk-q42-gw-1
(рис. [-@fig:013]).

![Настройка msk-q42-gw-1](image/13.png){#fig:013 width=70%}

Настройка маршрутизатора sch-sochi-gw-1
(рис. [-@fig:014]).

![Настройка sch-sochi-gw-1](image/14.png){#fig:014 width=70%}

Настройка маршрутизатора msk-q42-gw-1 (рис. [-@fig:015]).

![Настройка msk-q42-gw-1](image/15.png){#fig:015 width=70%}

Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1
(рис. [-@fig:016]).

![Настройка msk-hostel-gw-1](image/16.png){#fig:016 width=70%}

Настройка NAT на маршрутизаторе msk-donskaya-gw-1 (рис. [-@fig:017]).

![Настройка msk-donskaya-gw-1](image/17.png){#fig:017 width=70%}

# Вывод

Мы смогли настроить взаимодействие через сеть провайдера посредством статической
маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного
в г. Сочи

# Контрольные вопросы

1. Пример из файла (раздел 14.3.4.3) — настройка маршрута по умолчанию на маршрутизаторе sch-sochi-gw-1:

text
sch-sochi-gw-1>enable
sch-sochi-gw-1#configure terminal
sch-sochi-gw-1(config)#ip route 0.0.0.0 0.0.0.0 10.128.255.5
Пояснение:

0.0.0.0 0.0.0.0 — сеть назначения и маска (маршрут по умолчанию).

10.128.255.5 — IP-адрес следующего шлюза (в данном случае msk-donskaya-gw-1).

Другой пример (гипотетический, между двумя подсетями организации, например, между VLAN 201 и VLAN 202):
На маршрутизаторе msk-q42-gw-1:

text
msk-q42-gw-1(config)#ip route 10.129.1.0 255.255.255.0 10.129.0.2
Это означает, что для достижения подсети 10.129.1.0/24 трафик направляется на шлюз 10.129.0.2.

2. Опишите процесс обращения устройства из одного VLAN к устройству из другого VLAN.
Отправка запроса:
Устройство в VLAN A (IP: 10.129.0.10) пытается связаться с устройством в VLAN B (IP: 10.129.1.20).
Поскольку IP-адреса находятся в разных подсетях, отправитель понимает, что цель находится не в его локальной сети.

ARP-запрос на шлюз по умолчанию:
Отправитель отправляет ARP-запрос для MAC-адреса своего шлюза по умолчанию (например, 10.129.0.1 — это msk-q42-gw-1).

Передача пакета на маршрутизатор:
Пакет (с исходным MAC отправителя и MAC шлюза) отправляется на маршрутизатор.

Маршрутизация между VLAN:
Маршрутизатор (или многоуровневый коммутатор) получает пакет на субинтерфейсе .201 (VLAN 201), смотрит в таблицу маршрутизации и определяет, что сеть VLAN 202 доступна через субинфейс .202 (или другой интерфейс).

ARP со стороны маршрутизатора:
Маршрутизатор выполняет ARP-запрос в VLAN 202 для определения MAC-адреса целевого устройства (10.129.1.20).

Пересылка пакета:
Маршрутизатор заменяет исходный MAC на свой MAC в VLAN 202, MAC назначения — на MAC целевого устройства, и отправляет пакет в VLAN 202.

Ответ:
Устройство в VLAN B получает пакет и отвечает аналогичным образом через маршрутизатор.

Важно: Без маршрутизатора (L3-устройства) устройства из разных VLAN не могут общаться напрямую, даже если они физически подключены к одному коммутатору.

3. Как проверить работоспособность маршрута?
Основные способы:

Команда ping — проверка связности с удалённым устройством:

text
ping 10.130.0.1
Успешные ответы (!!!!!) означают, что маршрут работает.

Команда traceroute (или tracert) — показывает путь следования пакетов:

text
traceroute 10.130.0.1
Позволяет увидеть, через какие шлюзы проходит трафик, и где возможен обрыв.

Extended ping (в Cisco) с указанием источника:

text
ping 10.130.0.1 source 10.129.0.1
Проверяет маршрут от конкретного интерфейса.

Проверка таблицы маршрутизации — убедиться, что маршрут внесён и имеет правильный next-hop (см. следующий вопрос).

4. Как посмотреть таблицу маршрутизации?
На оборудовании Cisco (маршрутизаторы, многоуровневые коммутаторы):

Основная команда:

text
show ip route
Пример вывода (гипотетический):

text
Codes: C - connected, S - static, O - OSPF, ...
S    10.130.0.0/24 [1/0] via 10.128.255.6
C    10.128.255.4/30 is directly connected, FastEthernet0/1.6
S*   0.0.0.0/0 [1/0] via 10.128.255.5
S — статический маршрут

C — подключённая сеть

S* — маршрут по умолчанию

Другие полезные команды:

show ip route static — только статические маршруты

show ip route connected — только подключённые сети

show ip route 10.130.0.0 — детали конкретного маршрута

На компьютере (Windows):

text
route print
или

text
netstat -r
На Linux:

text
ip route show
или

text
route -n

# Список литературы{.unnumbered}

::: {#refs}
:::
