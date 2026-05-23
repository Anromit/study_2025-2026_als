---
## Front matter
lang: ru-RU
title: Лабораторная работа №15
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

- Настроить динамическую маршрутизацию между территориями организации

# Основная часть

## Настройка msk-donskaya-gw-1

- Настройка маршрутизатора msk-donskaya-gw-1
![](./image/1.png)

## Проверка msk-donskaya-gw-1

![Проверка состояния протокола OSPF на маршрутизаторе msk-donskaya-gw-1](./image/2.png){#fig:002 width=40%}

## Настройка msk-q42-gw-1

- Настройка маршрутизатора msk-q42-gw-1

![](./image/3.png){#fig:003 width=20%}


## Настройка msk-hostel-gw-1

![Настройка маршрутизирующего коммутатора msk-hostel-gw-1](./image/4.png){#fig:004 width=35%}

## Настройка sch-sochi-gw-1

![Настройка маршрутизатора sch-sochi-gw-1](./image/5.png){#fig:005 width=30%}

## Настройка provider-sw-1

![Настройка интерфейсов коммутатора provider-sw-1](./image/6.png){#fig:006 width=30%}

## Настройка msk-q42-gw-1

![Настройка маршрутизатора msk-q42-gw-1](./image/7.png){#fig:007 width=30%}

## Настройка sch-sochi-sw-1

![Настройка коммутатора sch-sochi-sw-1 ](./image/8.png){#fig:008 width=30%}

## Настройка sch-sochi-gw-1

![Настройка маршрутизатора sch-sochi-gw-1](./image/9.png){#fig:009 width=30%}

## Настройка sch-sochi-gw-1

![Настройка маршрутизатора sch-sochi-gw-1](./image/10.png){#fig:010 width=30%}

# Вывод

## Вывод

- Мы смогли настроить динамическую маршрутизацию между территориями организации.
