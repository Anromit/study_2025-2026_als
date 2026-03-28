---
## Front matter
lang: ru-RU
title: Лабораторная работа №7
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

- Получить навыки работы с физической рабочей областью Packet Tracer,
а также учесть физические параметры сети

# Основная часть

## Открытие проекта

![Откроем проект предыдущей лабораторной работы](./image/1.png)

## Название города

![Перейдем в физическую рабочую область Packet Tracer. Присвоим название городу — Moscow](./image/2.png){#fig:002 width=40%}

## Название города

![Щёлкнув на изображении города, мы видим изображение здания.Присвоим ему название Donskaya.](./image/3.png){#fig:003 width=20%}

## Новое здвние

![Щёлкнув на изображении здания Donskaya, переместим изображение, обозначающее серверное помещение, в него](./image/4.png){#fig:004 width=30%}

## Серверные стойки

![ Щёлкнув на изображении серверной, Мы увидим отображение серверныхстоек.](./image/5.png){#fig:005 width=30%}

## Перемещение коммутаторов

- Вернувшись в логическую рабочую область Packet Tracer, пропингуем с коммутатора msk-donskaya-arromichina-sw-1 коммутатор msk-pavlovskaya-arromichina-sw-1.
Убедимся в работоспособности соединения

![](./image/6.png){#fig:006 width=25%}

## Пинг соединения

![Вернувшись в логическую рабочую область Packet Tracer, пропингуем с коммутатора msk-donskaya-arromichina-sw-1 коммутатор msk-pavlovskaya-arromichina-sw-1. Убедимся в работоспособности соединения](./image/7.png){#fig:007 width=30%}

## Настройки

![В меню Options , Preferences во вкладке Interface активируем разрешение на учёт физических характеристик среды передачи (Enable Cable Length Effects)](./image/8.png){#fig:008 width=30%}

## Большое расстояние

![В физической рабочей области Packet Tracer разместим две территории на расстоянии более 100 м друг от друга (рекомендуемое расстояние — около 1000 м или более).](./image/9.png){#fig:009 width=30%}

## Пинг на большом расстоянии

![Вернувшись в логическую рабочую область Packet Tracer, пропингуем с коммутатора msk-donskaya-arromichina-sw-1 коммутатор msk-pavlovskaya-arromichina--sw-1. Убедимся в неработоспособности соединения.](./image/10.png){#fig:010 width=30%}

## Добавление двух повторителей

- Удалим соединение между msk-donskaya-arromichina-sw-1 и msk-pavlovskaya--arromichina-sw-1.
Добавим в логическую рабочую область два повторителя (RepeaterPT). Присвоим им соответствующие названия msk-donskaya-arromichina-mc-1
и msk-pavlovskaya-arromichina-mc-1. Заменим имеющиеся модули на PT-REPEATERNM-1FFE и PT-REPEATER-NM-1CFE для подключения оптоволокна
и витой пары по технологии Fast Ethernet 

![](./image/11.png){#fig:011 width=30%}

## Перемещение

![Переместим msk-pavlovskaya-arromichina-mc-1 на территорию Pavlovskaya (в физической рабочей области Packet Tracer).](./image/12.png){#fig:012 width=30%}

## Подключение
- Подключим коммутатор msk-donskaya-arromichina-sw-1 к msk-donskaya-arromichina-mc-1 по витой паре, msk-donskaya-arromichina-mc-1 и msk-pavlovskaya-arromichina-mc-1 — по оптоволокну,msk-pavlovskaya-arromichina-sw-1 к msk-pavlovskaya-arromichina-mc-1 — по витой парерис.

![](./image/13.png){#fig:013 width=30%}

## Проверка соединения

![Убедимся в работоспособности соединения между msk-donskaya-arromichina-sw-1 и msk-pavlovskaya-arromichina-sw-1.](./image/10.png){#fig:010 width=30%}

# Вывод

## Вывод

- Мы смогли получить навыки работы с физической рабочей областью Packet Tracer,а также учесть физические параметры сети
