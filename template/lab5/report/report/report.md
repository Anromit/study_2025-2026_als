---
## Front matter
title: "Лабораторная работа 5"
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

Получить основные навыки по настройке VLAN на коммутаторах 

# Выполнение лаборатаорной работы

Настройка VLAN-портов на коммутаторе msk-donskaya-arromichina-sw-1  (рис. [-@fig:001]).

![VLAN-порт msk-donskaya-arromichina-sw-1](image/1.png){#fig:001 width=70%}

Настройка VLAN-портов на коммутаторе msk-donskaya-arromichina-sw-2 (рис. [-@fig:002]).

![VLAN-порт msk-donskaya-arromichina-sw-2](image/2.png){#fig:002 width=70%}

Настройка VLAN-портов на коммутаторе msk-donskaya-arromichina-sw-3 (рис. [-@fig:003]).

![VLAN-порт msk-donskaya-arromichina-sw-3](image/3.png){#fig:003 width=70%}

Настройка VLAN-портов на коммутаторе msk-donskaya-arromichina-sw-4 (рис. [-@fig:004]).

![VLAN-порт msk-donskaya-arromichina-sw-4](image/4.png){#fig:004 width=70%}

Настройка VLAN-портов на коммутаторе msk-pavlovskaya-arromichina-sw-1(рис. [-@fig:005]).

![VLAN-порт msk-pavlovskaya-arromichina-sw-1](image/5.png){#fig:005 width=70%}

Настройка коммутатора msk-donskaya-arromichina-sw-1 как VTP-сервера, добавление номеров и назвний VLAN(рис. [-@fig:006]).

![VTP-сервер](image/6.png){#fig:006 width=70%}

Настройка коммутатора msk-donskaya-arromichina-sw-2 как VTP-сервера, добавление номеров и назвний VLAN(рис. [-@fig:007]).

![VTP-сервер](image/7.png){#fig:007 width=70%}

Настройка коммутатора msk-donskaya-arromichina-sw-4 как VTP-сервера, добавление номеров и назвний VLAN(рис. [-@fig:008]).

![VTP-сервер](image/8.png){#fig:008 width=70%}

Настройка коммутатора msk-donskaya-arromichina-sw-3 как VTP-сервера, добавление номеров и назвний VLAN(рис. [-@fig:009]).

![VTP-сервер](image/9.png){#fig:009 width=40%}

Настройка коммутатора msk-pavlovskaya-arromichina-sw-1 как VTP-сервера, добавление номеров и назвний VLAN(рис. [-@fig:010]).

![VTP-сервер](image/10.png){#fig:010 width=40%}

Проверка статуса msk-donskaya-arromichina-sw-3 (рис. [-@fig:011]).

![Проверка статуса](image/11.png){#fig:011 width=40%}

Проверка статуса msk-donskaya-arromichina-sw-4 (рис. [-@fig:012]).

![Проверка статуса](image/12.png){#fig:012 width=40%}

Проверка статуса msk-pavlovskaya-arromichina-sw-1(рис. [-@fig:013]).

![Проверка статуса](image/13.png){#fig:013 width=40%}

Настройка IP адреса web(рис. [-@fig:014]).

![Настройка IP](image/14.png){#fig:014 width=40%}

Настройка IP адреса file(рис. [-@fig:015]).

![Настройка IP](image/15.png){#fig:015 width=40%}

Настройка IP адреса mail(рис. [-@fig:016]).

![Настройка IP](image/16.png){#fig:016 width=40%}

Настройка IP адреса dns(рис. [-@fig:017]).

![Настройка IP](image/17.png){#fig:017 width=40%}

Настройка IP адреса dk-pc-1(рис. [-@fig:018]).

![Настройка IP](image/18.png){#fig:018 width=40%}

Настройка IP адреса dep-pc-1(рис. [-@fig:019]).

![Настройка IP](image/19.png){#fig:019 width=40%}

Настройка IP адреса adm-pc-1(рис. [-@fig:020]).

![Настройка IP](image/20.png){#fig:020 width=70%}

Настройка IP адреса other-pc-1(рис. [-@fig:021]).

![Настройка IP](image/21.png){#fig:021 width=70%}

Настройка IP адреса dk-pavlovskaya-pc-1(рис. [-@fig:022]).

![Настройка IP](image/22.png){#fig:022 width=70%}

Настройка IP адреса other-pavlovskaya-pc-1(рис. [-@fig:023]).

![Настройка IP](image/23.png){#fig:023 width=70%}

Проверка соединения(рис. [-@fig:024]).

![Проверка](image/24.png){#fig:024 width=70%}

# Вывод

Мы смогли получить основные навыки по настройке VLAN на коммутаторах 

# Контрольные вопросы

1. Какая команда используется для просмотра списка VLAN на сетевом устройстве? show vlan brief (или show vlan).

2. Охарактеризуйте VLAN Trunking Protocol (VTP). Приведите перечень команд с пояснениями для настройки и просмотра информации о VLAN. VTP — протокол Cisco для централизованного управления VLAN (создание, удаление, переименование) в рамках одного домена. Команды настройки: vtp domain <имя> (задание домена), vtp mode {server | client | transparent} (режим работы), vtp password <пароль> (аутентификация), vtp version {1 | 2 | 3} (версия). Команды просмотра: show vtp status (статус и параметры VTP), show vtp password (пароль), show vlan (информация о VLAN).

3. Охарактеризуйте Internet Control Message Protocol (ICMP). Опишите формат пакета ICMP. ICMP — протокол сетевого уровня для передачи сообщений об ошибках и диагностики (ping, traceroute). Формат пакета: IP-заголовок (20 байт) + ICMP-заголовок (4 байта: Тип (1 байт), Код (1 байт), Контрольная сумма (2 байта)) + Данные (переменной длины, обычно часть исходного IP-пакета).

4. Охарактеризуйте Address Resolution Protocol (ARP). Опишите формат пакета ARP. ARP — протокол канального/сетевого уровня для определения MAC-адреса по известному IP-адресу в локальной сети. Формат пакета: Hardware Type (2 байта, тип сети, обычно Ethernet), Protocol Type (2 байта, тип протокола, обычно IP), Hardware Length (1 байт, длина MAC-адреса), Protocol Length (1 байт, длина IP-адреса), Operation (2 байта, код операции: 1=запрос, 2=ответ), MAC отправителя (6 байт), IP отправителя (4 байта), MAC получателя (6 байт), IP получателя (4 байта).

5. Что такое MAC-адрес? Какова его структура? MAC-адрес (Media Access Control) — это уникальный физический адрес, "прошитый" в сетевой интерфейс на заводе. Структура (48 бит / 6 байт): Первые 3 байта (24 бита) — OUI (идентификатор организации-производителя), последующие 3 байта — уникальный номер устройства, назначаемый производителем. Записывается обычно в шестнадцатеричном формате (например, AA:BB:CC:11:22:33).

# Список литературы{.unnumbered}

::: {#refs}
:::
