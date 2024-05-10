---
## Front matter
lang: ru-RU
title: Лабораторная работа № 7
subtitle: Модель СМО
author:
  - Демидова Е. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 10 мая 2024

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
---

# Вводная часть

## Цели и задачи

**Цель работы**

Реализовать модель $M|M|1|\infty$ с помощью xcos.

**Задание**

- Реализовать в xcos модель системы массового обслуживания типа $M|M|1|\infty$.
- Построить график, описывающий динамику размера очереди 
- Построить график, описывающий поступление и обработку заявок.

# Выполнение лабораторной работы

## Реализация модели в xcos

![Переменное окружение](image/1.png){#fig:001 width=70%}

## Реализация модели в xcos

![Суперблок, моделирующий поступление заявок](image/2.png){#fig:002 width=50%}

## Реализация модели в xcos

![Суперблок, моделирующий обработку заявок](image/3.png){#fig:003 width=50%}

## Реализация модели в xcos

![Модель $M|M|1|\infty$ в xcos](image/4.png){#fig:004 width=50%}

## Реализация модели в xcos

![Поступление(зеленым) и обработка(черным) заявок](image/5.png){#fig:005 width=70%}

## Реализация модели в xcos

![Динамика размера очереди](image/6.png){#fig:006 width=70%}

# Выводы

В результате выполнения работы была реализована модель $M|M|1|\infty$ с помощью xcos.