---
## Front matter
lang: ru-RU
title: Лабораторная работа №6
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

- Настроить статическую маршрутизацию VLAN в сети.

# Основная часть

## Размещение маршрутизатора Cisco 2811 в логической области проекта

![В логической области проекта разместим маршрутизатор Cisco 2811](./image/1.png)

## Общая схема

![Общая схема сети](./image/2.png){#fig:002 width=40%}

## Подключение его к порту 24 коммутатора msk-donskaya-arromichina-sw-1.

![Подключим его к порту 24 коммутатора msk-donskaya-arromichina-sw-1 в соответствии с таблицей портов](./image/3.png){#fig:003 width=20%}

## Настройка добавленного устройства

![Используя приведённую ниже последовательность команд по первоначальной настройке маршрутизатора, сконфигурируем маршрутизатор, задав на нём имя, пароль для доступа к консоли, настроим удалённое подключение к нему по ssh](./image/4.png){#fig:004 width=30%}

## Настройка порта коммутатора как trunk порт

![ Настроим порт 24 коммутатора msk-donskaya-sw-1 как trunk-порт](./image/5.png){#fig:005 width=30%}

## Настройка виртуальных интерфейсов, задание IP-адресов

- На интерфейсе f0/0 маршрутизатора msk-donskaya-arromichina-gw-1 настроим виртуальные интерфейсы, соответствующие номерам VLAN. Согласно таблице IP-адресов (см. табл. 3.2 из раздела 3.3) зададим соответствующие IP-адреса на виртуальных интерфейсах. Для этого используем приведённую в лабораторной работе последовательность команд по конфигурации VLAN-интерфейсов маршрутизатора

![](./image/6.png){#fig:006 width=25%}

## Проверяем проделанную работу

![Проверим доступность оконечных устройств из разных VLAN](./image/7.png){#fig:007 width=30%}

## Изучение процесса прердвижения пакета

![Используя режим симуляции в Packet Tracer, изучим процесс передвижения пакета ICMP по сети. Изучим содержимое передаваемого пакета и заголовки задействованных протоколов](./image/8.png){#fig:008 width=30%}


# Вывод

## Вывод

- Мы смогли настроить статическую маршрутизацию VLAN в сети.
