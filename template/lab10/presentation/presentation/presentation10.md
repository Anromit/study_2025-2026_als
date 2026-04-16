---
## Front matter
lang: ru-RU
title: Лабораторная работа №10
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

- Освоить настройку прав доступа пользователей к ресурсам сети


# Основная часть

## Добавление устройства

- В рабочей области проекта подключим ноутбук администратора с именем
admin к сети к other-donskaya-1 с тем, чтобы разрешить ему потом любые
действия, связанные с управлением сетью
Для этого подсоединим ноутбук к порту 24 коммутатора msk-donskaya-sw-4 и присвоим ему статический адрес 10.128.6.200, указав в качестве gateway-адреса 10.128.6.1 и адреса DNS-сервера 10.128.0.5 
![](./image/1.png){#fig:001 width=40%}

## Настройка доступа

![Настроим доступ к web-серверу по порту tcp 80](./image/2.png){#fig:002 width=40%}

## Добавление списка

![Добавим список управления доступом к интерфейсу](./image/3.png){#fig:003 width=20%}

## Настройка

![Настроим дополнительный доступ для администратора по протоколам Telnet и FTP](./image/4.png){#fig:004 width=30%}

## Проверка

- Убедитесь, что с узла с ip-адресом 10.128.6.200 есть доступ по протоколу
FTP.

![](./image/5.png){#fig:005 width=30%}

## Настройка доступа

![Настроим доступ к файловому серверу](./image/6.png){#fig:006 width=25%}

## Настройка доступа

![Настроим доступ к почтовому серверу](./image/7.png){#fig:007 width=30%}

## Настройка доступа DNS

![Настроим доступ к DNS-серверу](./image/8.png){#fig:008 width=30%}

## icmp-запросы

![Разрешим icmp-запросы](./image/9.png){#fig:009 width=30%}

## Настройка доступа

![Настроим доступ для сети Other](./image/10.png){#fig:010 width=30%}

## Настройка доступа

![Настроим доступ администратора к сети сетевого оборудования](./image/11.png){#fig:011 width=30%}

# Сомостятельная работа


## Проверка коректности

![Проверим корректность установленных правил доступа, попытавшись получить доступ по различным протоколам с разных устройств сети к подсети серверов и подсети сетевого оборудования](./image/12.png){#fig:012 width=30%}

## Разрешение действий

![Разрешим администратору из сети Other на Павловской действия, аналогичные действиям администратора сети Other на Донской.](./image/13.png){#fig:013 width=30%}


# Вывод

## Вывод

- Мы смогли освоить настройку прав доступа пользователей к ресурсам сети
