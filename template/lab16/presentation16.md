---
## Front matter
lang: ru-RU
title: Лабораторная работа №16
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

# Вводная часть

## Цель работы

- Получение навыков настройки VPN-туннеля через незащищённое Интернетсоединение.

# Основная часть

## Размещение объектов

- Разместим в рабочей области проекта оборудование для сети Университета г. Пиза
![](./image/1.png)

## Размещение объектов

![В физической рабочей области проекта создадим город Пиза, здание Университета г. Пиза](./image/2.png){#fig:002 width=40%}

## Перемещение оборудования

- Переместим туда соответствующее оборудование

![](./image/3.png){#fig:003 width=20%}

## Первоначальная настройка

![Первоначальная настройка маршрутизатора pisa-unipi-gw-1](./image/4.png){#fig:004 width=35%}

## Первоначальная настройка коммутатора pisa-unipi-sw-1

![Первоначальная настройка коммутатора pisa-unipi-sw-1](./image/5.png){#fig:005 width=30%}

## Настройка интерфейсов маршрутизатора pisa-unipi-gw-1

![Настройка интерфейсов маршрутизатора pisa-unipi-gw-1](./image/6.png){#fig:006 width=30%}

## Настройка интерфейсов коммутатора pisa-unipi-sw-1

![Настройка интерфейсов коммутатора pisa-unipi-sw-1](./image/7.png){#fig:007 width=30%}

## Настройка маршрутизатора msk-donskaya-gw-1

![Настройка маршрутизатора msk-donskaya-gw-1 ](./image/8.png){#fig:008 width=30%}

## Настройка интерфейсов маршрутизатора pisa-unipi-gw-1

![Настройка интерфейсов маршрутизатора pisa-unipi-gw-1](./image/9.png){#fig:009 width=30%}

## Проверка

![Проверка](./image/10.png){#fig:010 width=30%}

# Вывод

## Вывод

- Мы смогли получить навыки настройки VPN-туннеля через незащищённое Интернетсоединение.
