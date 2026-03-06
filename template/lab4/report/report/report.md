---
## Front matter
title: "Лабораторная работа 4"
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

Провести подготовительную работу по первоначальной настройке коммутатора сети.

# Выполнение лаборатаорной работы

В логической области размещаем коммутаоры и оконечные устройства согласно схеме сети L1(рис. [-@fig:001]).

![размещаем коммутаоры и устройства](image/1.png){#fig:001 width=70%}

Настраиваем устройство msk-donskaya-arromichina-sw-1 согласно лабораторной работе(рис. [-@fig:002]).

![Настройка устройства 1](image/2.png){#fig:002 width=70%}

Настраиваем устройство msk-donskaya-arromichina-sw-2 согласно лабораторной работе(рис. [-@fig:003]).

![Настройка устройства 2](image/3.png){#fig:003 width=70%}

Настраиваем устройство msk-donskaya-arromichina-sw-3 согласно лабораторной работе(рис. [-@fig:004]).

![Настройка устройства 3](image/4.png){#fig:004 width=70%}

Настраиваем устройство msk-donskaya-arromichina-sw-4 согласно лабораторной работе(рис. [-@fig:005]).

![Настройка устройства 4](image/5.png){#fig:005 width=70%}

Настраиваем устройство msk-pavlovskaya-arromichina-sw-1 согласно лабораторной работе(рис. [-@fig:006]).

![Настройка устройства msk-pavlovskaya-arromichina-sw-1](image/6.png){#fig:006 width=70%}

Проверяем(рис. [-@fig:007]).

![Проверяем проделанную работу](image/7.png){#fig:007 width=70%}

# Вывод

Мы смогли провести подготовительную работу по первоначальной настройке коммутатора сети.

# Контрольные вопросы

1. При помощи каких команд можно посмотреть конфигурацию сетевого оборудования?
Для просмотра текущей (активной) конфигурации сетевого оборудования (коммутатора или маршрутизатора) в Cisco IOS используются следующие команды в привилегированном режиме (enable):

show running-config (или сокращённо show run) — отображает конфигурацию, которая в данный момент загружена в оперативную память (RAM) устройства и активна. Именно эта конфигурация управляет работой оборудования в настоящий момент.

show startup-config — показывает конфигурацию, которая сохранена в энергонезависимой памяти (NVRAM) и будет загружена при следующей перезагрузке устройства.

2. При помощи каких команд можно посмотреть стартовый конфигурационный файл оборудования?
Для просмотра стартового конфигурационного файла (который используется при загрузке) служит команда:

show startup-config

Чтобы увидеть содержимое этого файла, необходимо находиться в привилегированном режиме (режим enable, приглашение заканчивается символом #).

3. При помощи каких команд можно экспортировать конфигурационный файл оборудования?
Под экспортом конфигурационного файла обычно понимают его сохранение (копирование) на внешнее хранилище, например, на TFTP-сервер. Основная команда для этого:

copy running-config tftp: или copy startup-config tftp:

После ввода этой команды устройство запросит IP-адрес TFTP-сервера и имя файла, под которым сохранить конфигурацию.

Также экспортом можно считать сохранение текущей конфигурации в стартовый файл (чтобы она не потерялась после перезагрузки), хотя технически это скорее "сохранение", а не экспорт:

copy running-config startup-config (или write memory / wr)

4. При помощи каких команд можно импортировать конфигурационный файл оборудования?
Импорт (загрузка) конфигурации выполняется обратной операцией — копированием файла с внешнего носителя (сервера) в память устройства:

copy tftp: running-config — загружает конфигурацию с TFTP-сервера в оперативную память, объединяя её с текущей конфигурацией (команды добавляются к уже существующим).

copy tftp: startup-config — загружает конфигурацию с сервера прямо в стартовый файл (NVRAM).

# Список литературы{.unnumbered}

::: {#refs}
:::
