---
## Front matter
lang: ru-RU
title: Лабораторная работа №12
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

- Приобретение практических навыков по настройке доступа локальной сети
к внешней сети посредством NAT


# Основная часть

## Настройка маршрутизатора provider-gw-1

- Первоначально настроим маршрутизатор provider-gw-1
![](./image/1.png)

## Настройка коммутатора provider-sw-1

![Первоначально настрорм коммутатор provider-sw-1](./image/2.png){#fig:002 width=40%}

## Интерфейсы маршрутизатора

- Настроим интерфейсы маршрутизатора provider-gw-1

![](./image/3.png){#fig:003 width=40%}

## Интерфейсы коммутатора

- Настроим интерфейсы коммутатора provider-sw-1

![](./image/4.png){#fig:004 width=30%}

## Интерфейсы маршрутизатора

![Настроим интерфейсы маршрутизатора msk-donskaya-gw-1](./image/5.png){#fig:005 width=25%}

## Настройка

![Настройка пула адресов для NAT, настройка списка доступа для NAT, сеть дисплейных классов, сеть администрации, доступ для компьютера администратора](./image/6.png){#fig:006 width=30%}

## Настройка

![Настроим NAT](./image/7.png){#fig:007 width=30%}

## Настройка доступа

![Настроим доступа из Интернета](./image/8.png){#fig:008 width=30%}

## Пинг

![Проверим работоспособности](./image/9.png){#fig:009 width=30%}



# Вывод

## Вывод

- Мы смогли приобрести практические навыки по настройке доступа локальной сети
к внешней сети посредством NAT
