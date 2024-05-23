---
## Front matter
lang: ru-RU
title: Упражнение
subtitle: Моделирование в xcos
author:
  - Демидова Е. А.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 3 мая 2024

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

## Цели 

Построить с помощью xcos фигуры Лиссажу.

## Задачи

Построить с помощью xcos фигуры Лиссажу со следующими параметрами:

1) $A = B = 1$, $a = 2$, $b = 2$, $\delta = 0$; 
                $\pi/4$; $\pi/2$; $3 \pi/4$; $\pi$;
2) $A = B = 1$, $a = 2$, $b = 4$, $\delta = 0$; 
                $\pi/4$; $\pi/2$; $3 \pi/4$; $\pi$;
3) $A = B = 1$, $a = 2$, $b = 6$, $\delta = 0$; 
                $\pi/4$; $\pi/2$; $3 \pi/4$; $\pi$;
4) $A = B = 1$, $a = 2$, $b = 3$, $\delta = 0$; 
                $\pi/4$; $\pi/2$; $3 \pi/4$; $\pi$;

# Выполнение лабораторной работы

## Математическая модель

$$
\begin{cases}
	x(t) = A sin(at+\delta), \\
	y(t) = B sin(bt),
\end{cases}
$$

где $A$, $B$ -- амплитуды колебаний, $a$, $b$ -- частоты, $\delta$ -- сдвиг фаз.

## Реализация модели в xcos

![Модель фигуры Лиссажу в xcos](image/1.png){#fig:001 width=50%}

## Реализация модели в xcos

![Параметры генератора синусоидального сигнала](image/2.png){#fig:002 width=70%}

## Реализация модели в xcos

![Задать параметры устройства для построения графика](image/3.png){#fig:003 width=50%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 2$, $\delta = 0$](image/4.png){#fig:004 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 2$, $\delta = \pi/4$](image/5.png){#fig:005 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 2$, $\delta = \pi/2$](image/6.png){#fig:006 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 2$, $\delta = 3*\pi/4$](image/7.png){#fig:007 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 2$, $\delta = \pi$](image/8.png){#fig:008 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 4$, $\delta = 0$](image/9.png){#fig:009 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 4$, $\delta = \pi/4$](image/10.png){#fig:010 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 4$, $\delta = \pi/2$](image/11.png){#fig:011 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 4$, $\delta = 3*\pi/4$](image/12.png){#fig:012 width=65%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 4$, $\delta = \pi$](image/13.png){#fig:013 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 6$, $\delta = 0$](image/14.png){#fig:014 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 6$, $\delta = \pi/4$](image/15.png){#fig:015 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 6$, $\delta = \pi/2$](image/16.png){#fig:016 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 6$, $\delta = 3*\pi/4$](image/17.png){#fig:017 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 6$, $\delta = \pi$](image/18.png){#fig:018 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 3$, $\delta = 0$](image/19.png){#fig:019 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 3$, $\delta = \pi/4$](image/20.png){#fig:020 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 3$, $\delta = \pi/2$](image/21.png){#fig:021 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 3$, $\delta = 3*\pi/4$](image/22.png){#fig:022 width=70%}

## Реализация модели в xcos

![Фигура Лиссажу при $A = B = 1$, $a = 2$, $b = 3$, $\delta = \pi$](image/23.png){#fig:023 width=70%}

# Выводы

В результате выполнения работы были построены с помощью xcos фигуры Лиссажу.

