---
## Front matter
lang: ru-RU
title: Лабораторная работа №9
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

- Изучить возможности протокола STP и его модификаций по обеспечению
отказоустойчивости сети, агрегированию интерфейсов и перераспределению
нагрузки между ними.

# Основная часть

## Соединение

![Сформируем резервное соединение между коммутаторами msk-donskayasw-1 и msk-donskaya-sw-3](./image/1.png)

## Пинг

![С оконечного устройства dk-donskaya-1 пропингуем серверы mail и web](./image/2.png){#fig:002 width=40%}

## Просмотр протокола

![На коммутаторе msk-donskaya-sw-2 посмотрим состояние протокола STP для vlan 3](./image/3.png){#fig:003 width=20%}

## Настройка

![В качестве корневого коммутатора STP настроим коммутатор mskdonskaya-sw-1](./image/4.png){#fig:004 width=30%}

## Проверка
- Используя режим симуляции, убедимся, что пакеты ICMP пойдут от
хоста dk-donskaya-1 до mail через коммутаторы msk-donskaya-sw-1 и mskdonskaya-sw-3, а от хоста dk-donskaya-1 до web через коммутаторы
msk-donskaya-sw-1 и msk-donskaya-sw-2 

![](./image/5.png){#fig:005 width=30%}

## Настройка режима Portfast

![Настроим режим Portfast на тех интерфейсах коммутаторов, к которым подключены серверы](./image/6.png){#fig:006 width=25%}

## Изучение отказоустойчивости протокола STP

![Изучим отказоустойчивость протокола STP и время восстановления соединения при переключении на резервное соединение.](./image/7.png){#fig:007 width=30%}

## Перенастройка

![Переключим коммутаторы режим работы по протоколу Rapid PVST+](./image/8.png){#fig:008 width=30%}

## Изучение отказоустойчивости

![Изучим отказоустойчивость протокола Rapid PVST+ и время восстановления соединения при переключении на резервное соединение](./image/9.png){#fig:009 width=30%}

## Дополнительное соединение

![Сформируем агрегированное соединение интерфейсов Fa0/20 – Fa0/23 между коммутаторами msk-donskaya-sw-1 и msk-donskaya-sw-4](./image/10.png){#fig:010 width=30%}

## Настройка

![Настроим агрегирование каналов](./image/11.png){#fig:011 width=30%}
# Вывод

## Вывод

- Мы смогли изучить возможности протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.
