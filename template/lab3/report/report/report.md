---
## Front matter
title: "Лабораторная работа 3"
subtitle: "Планирование локальной сети организации"
author: "Ромицына Анасасия Романовна"

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

# Цель работы

Познакомиться с принципами планирования локальной сети организации

# Выполнение лабораторной работы

Повторяем схемы из лабораторной работы(рис. [-@fig:001]).

![Рабочая область](image/1.png){#fig:001 width=50%}


Начальная настройка msk-donskaya-arromichina-sw-1(рис. [-@fig:002]).

![Настройка msk-donskaya-arromichina-sw-1](image/2.png){#fig:002 width=50%}


Начальная настройка msk-donskaya-arromichina-sw-2(рис. [-@fig:003]).

![Настройка msk-donskaya-arromichina-sw-2](image/3.png){#fig:003 width=50%}


Начальная настройка msk-donskaya-arromichina-sw-4(рис. [-@fig:004]).

![Настройка msk-donskaya-arromichina-sw-4](image/4.png){#fig:004 width=50%}


Начальная настройка msk-donskaya-arromichina-sw-3(рис. [-@fig:005]).

![Настройка msk-donskaya-arromichina-sw-3](image/5.png){#fig:005 width=50%}


Настройка msk-donskaya-arromichina-sw-1(рис. [-@fig:006]).

![msk-donskaya-arromichina-sw-1](image/6.png){#fig:006 width=70%}


Начальная настройка msk-donskaya-arromichina-sw-3(рис. [-@fig:007]).

![Настройка msk-donskaya-arromichina-sw-3](image/7.png){#fig:007 width=70%}


Настройка msk-donskaya-arromichina-sw-4(рис. [-@fig:008]).

![Настройка msk-donskaya-arromichina-sw-4](image/8.png){#fig:008 width=70%}


Настройка msk-donskaya-arromichina-sw-1(рис. [-@fig:009]).

![Настройка msk-donskaya-arromichina-sw-1](image/9.png){#fig:009 width=70%}


настройка msk-donskaya-arromichina-gw-1(рис. [-@fig:010]).

![Настройка msk-donskaya-arromichina-gw-1](image/10.png){#fig:010 width=70%}


настройка web-arromichina 10.128.0.0.16 (рис. [-@fig:011]).

![Настройка web-arromichina 10.128.0.0.16](image/11.png){#fig:011 width=70%}


Настройка file-arromichina 10.128.0.0.16 (рис. [-@fig:012]).

![Настройка file-arromichina 10.128.0.0.16](image/12.png){#fig:012 width=70%}


Настройка mail-arromichina 10.128.0.0.16 (рис. [-@fig:013]).

![Настройка mail-arromichina 10.128.0.0.16](image/13.png){#fig:013 width=70%}


Настройка дк1-arromichina 10.128.0.0.16 (рис. [-@fig:014]).

![Настройка дк1-arromichina 10.128.0.0.16](image/14.png){#fig:014 width=70%}


Настройка дк-arromichina 10.128.0.0.16 (рис. [-@fig:015]).

![Настройка дк-arromichina 10.128.0.0.16](image/15.png){#fig:015 width=70%}


Настройка deportaments-arromichina 10.128.0.0.16 (рис. [-@fig:016]).

![Настройка deportaments-arromichina 10.128.0.0.16](image/16.png){#fig:016 width=70%}


Настройка adm-arromichina 10.128.0.0.16 (рис. [-@fig:017]).

![Настройка adm-arromichina 10.128.0.0.16](image/17.png){#fig:017 width=70%}


Настройка other-arromichina 10.128.0.0.16 (рис. [-@fig:018]).

![Настройка other-arromichina 10.128.0.0.16](image/18.png){#fig:018 width=70%}


настройка dk-arromichina 10.128.0.0.16 (рис. [-@fig:019]).

![Настройка dr-arromichina 10.128.0.0.16](image/19.png){#fig:019 width=70%}


Настройка other-arromichina 10.128.0.0.16 (рис. [-@fig:020]).

![Настройка other-arromichina 10.128.0.0.16](image/20.png){#fig:020 width=70%}


Настройка dns-arromichina 10.128.0.0.16 (рис. [-@fig:021]).

![Настройка dns-arromichina 10.128.0.0.16](image/21.png){#fig:021 width=70%}


Настроили все, зпускаем на проверку (рис. [-@fig:022]).

![Запускаем](image/22.png){#fig:022 width=70%}


Настройка msk-donskaya-arromichina-gw-1 (рис. [-@fig:023]).

![настройка msk-donskaya-arromichina-gw-1](image/23.png){#fig:023 width=70%}


Настройка file-arromichina 172.16.0.3 (рис. [-@fig:024]).

![Настройка file-arromichina 172.16.0.3](image/24.png){#fig:024 width=70%}


Настройка other1-arromichina 172.16.0.3 (рис. [-@fig:025]).

![Настройка other1-arromichina 172.16.0.3 аналогично настраиваем все нужные устройства](image/25.png){#fig:025 width=70%}


Запускаем на проверку(рис. [-@fig:026]).

![Запускаем на проверку на этом этапе](image/26.png){#fig:026 width=70%}


Настраиваем все устройства на новый адрес 192.168.0.0(рис. [-@fig:027]).

![Настройка всех умтройств на адрес 192.168.0.0](image/27.png){#fig:027 width=70%}


Запускаем на проверку(рис. [-@fig:028]).

![Запускаем на проверку на этом этапе](image/28.png){#fig:028 width=70%}

# Выводы

Мы смогли познакомиться с принципами планирования локальной сети организации

# Контрольные вопросы

1. Модель OSI (Open Systems Interconnection) — это эталонная модель, определяющая уровни взаимодействия в сети. Выделяют 7 уровней: физический (передача битов), канальный (формирование кадров, MAC-адреса), сетевой (маршрутизация, IP-адреса), транспортный (обеспечение надежности, сегменты), сеансовый (управление сеансами), представления (преобразование данных) и прикладной (взаимодействие с приложениями).

2. Коммутатор (switch) функционирует на канальном уровне (L2), он соединяет устройства в сети, используя их MAC-адреса для коммутации кадров, и используется для создания VLAN.

3. Маршрутизатор (router) работает на сетевом уровне (L3), обеспечивает связь между разными сетями (подсетями) и VLAN, принимая решения о маршрутизации на основе IP-адресов.

4. Коммутатор второго уровня (L2) работает только с MAC-адресами и не выполняет маршрутизацию, в отличие от коммутатора третьего уровня (L3), который также способен выполнять функции маршрутизации между VLAN, совмещая функции коммутатора и маршрутизатора.

5. Сетевой интерфейс — это точка подключения устройства к сети (например, сетевая плата), имеющая собственный MAC-адрес.

6. Сетевой порт — это физический разъем на сетевом устройстве (коммутаторе, маршрутизаторе), через который осуществляется подключение.

7. Ethernet — базовая технология локальных сетей. Fast Ethernet — стандарт со скоростью передачи 100 Мбит/с. Gigabit Ethernet обеспечивает скорость 1000 Мбит/с, используется для магистралей и серверов.

8. IPv4-адрес — это 32-битный адрес, идентифицирующий устройство в сети (например, 10.128.3.1). Сеть — это совокупность устройств, имеющих общую часть IP-адреса. Подсеть — это логическое разделение одной большой сети на более мелкие части для упрощения управления. Маска подсети определяет, какая часть IP-адреса относится к сети, а какая — к узлу (например, /24 или 255.255.255.0). Служебные адреса: адрес сети (младший, все биты хоста =0) и широковещательный адрес (старший, все биты хоста =1). Пример разбиения: сеть 10.128.0.0/16 (одна большая) разбита на подсети /24: 10.128.1.0/24 (управление), 10.128.3.0/24 (ДК) и другие, каждая поддерживает до 254 узлов.

9. VLAN (Virtual Local Area Network) — это технология, позволяющая логически разделить единую физическую сеть на несколько изолированных широковещательных доменов. Применяется для разделения трафика разных групп пользователей, повышения безопасности и упрощения управления. Преимущества: трафик отделяется, повышается производительность, упрощается добавление новых устройств. Примеры: отдельная сеть для Администрации (VLAN 103) и отдельная для Дисплейных классов (VLAN 101) на разных территориях.

10. Access Port (порт доступа) принадлежит одному конкретному VLAN и используется для подключения конечных устройств (компьютеров, принтеров). Trunk Port (магистральный порт) передает трафик сразу нескольких VLAN между коммутаторами и маршрутизаторами.


# Список литературы{.unnumbered}

::: {#refs}
:::
