---
## Front matter
lang: ru-RU
title: Лабораторная работа 2
subtitle: Предварительная настройка оборудования Cisco
author:
  - Ромицына А.Р.
institute:
  - Российский университет дружбы народов, Москва, Россия


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
  * Российский университет дружбы народов
  * [1132236132@rudn.ru](mailto:1132236132@rudn.ru)


:::
::: {.column width="30%"}


:::
::::::::::::::

## Цель работы

Получить основные навыки по начальному конфигурированию оборудования
Cisco.



# Выполнение лабораторной работы



## Рабочая область

![В логической рабочей области Packet Tracer разместим коммутатор, маршрутизатор и 2 оконечных устройства типа PC, соединим один PC с маршрутизатором, другой PC — с коммутатором. Настроим PC как в лабораторной работе](image/1.png){#fig:001 width=30%}

## Настройка маршрутизатора

![Проведем настройку маршрутизатора в соответствии с заданием, ориентируясь на приведённую ниже часть конфигурации маршрутизатора](image/2.png){#fig:002 width=30%}

## Настройка коммутатора

![Проведем настройку коммутатора в соответствии с заданием, ориентируясь на приведённую ниже часть конфигурации коммутатора](image/3.png){#fig:003 width=30%}

## ping маршрутизатора

![Проверим работоспособность соединений с помощью команды ping для маршрутизатора.](image/4.png){#fig:004 width=70%}

## ping коммутатора

![Проверим работоспособность соединений с помощью команды ping для коммутатора.](image/5.png){#fig:005 width=70%}

## Проверка подключения разными способами к маршрутизатору

![Попробуем подключиться к маршрутизатору разными способами: с помощью консольного кабеля, по протоколу удалённого доступа (telnet, ssh)](image/6.png){#fig:006 width=70%}

## Проверка подключения разными способами к коммутатору

![Попробуем подключиться к коммутатору разными способами: с помощью консольного кабеля, по протоколу удалённого доступа (telnet, ssh)](image/7.png){#fig:007 width=70%}
# Выводы
Мы смогли получить основные навыки по начальному конфигурированию оборудования
Cisco.
:::

