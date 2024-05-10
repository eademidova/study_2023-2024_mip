---
## Front matter
lang: ru-RU
title: Лабораторная работа № 5
subtitle: Модель эпидемии
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

Исследование модели эпидемии (SIR) с помощью xcos и OpenModelica.

## Задачи

- Реализовать классическую модель SIR с помощью xcos(в том числе с помощью блока Modelica) и OpenModelica.
- Реализовать модель SIR с учетом демографических признаков с помощью xcos(в том числе с помощью блока Modelica) и OpenModelica.
- Исследовать модель SIR с учетом демографических признаков, изменяя параметры.

# Выполнение лабораторной работы

## Теоретическое введение

$$
\begin{cases}
\frac{dS}{dt} = - \frac{\beta I S}{N}, \\
\frac{dI}{dt} = \frac{\beta I S}{N} - \gamma I, \\
\frac{dR}{dt} = \gamma I,
\end{cases}
$$

где $S$ -- численность восприимчивой популяции, $I$ -- численность инфицированных, $R$ -- численность удаленной популяции (в результате смерти или выздоровления), и $N$ — это сумма этих трёх, а $\beta$ и $\gamma$ - это коэффициенты заболеваемости и выздоровления соответственное


## Реализация модели в xcos

![Задать переменные окружения в xcos](image/1.png){#fig:001 width=60%}

## Реализация модели в xcos

![Модель SIR в xcos](image/2.png){#fig:002 width=70%}

## Реализация модели в xcos

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Задать начальные значение в блоке интегрирования для S](image/3.png){#fig:003 width=70%}

:::
::: {.column width="50%"}

![Задать начальные значение в блоке интегрирования для I](image/4.png){#fig:004 width=70%}

:::
::::::::::::::

## Реализация модели в xcos

![Задать конечное время интегрирования в xcos](image/5.png){#fig:005 width=70%}

## Реализация модели в xcos

![График решения модели SIR при $\beta = 1$, $\nu = 0.3$](image/6.png){#fig:006 width=70%}

## Реализация модели с помощью блока Modelica в xcos

![Модель SIR в xcos с применением блока Modelica](image/7.png){#fig:007 width=70%}

## Реализация модели с помощью блока Modelica в xcos

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Ввод значений входных параметров блока Modelica для модели](image/8.png){#fig:008 width=70%}

:::
::: {.column width="50%"}

![Ввод функции блока Modelica для модели](image/9.png){#fig:009 width=70%}

:::
::::::::::::::

## Реализация модели с помощью блока Modelica в xcos

![График решения модели SIR при $\beta = 1$, $\nu = 0.3$. Блок Modelica](image/10.png){#fig:010 width=70%}

## Реализация модели в OpenModelica

![Модель в OpenModelica](image/11.png){#fig:011 width=70%}

## Реализация модели в OpenModelica

![Параметры модели в OpenModelica](image/12.png){#fig:012 width=65%}

## Реализация модели в OpenModelica

![График решения модели SIR при $\beta = 1$, $\nu = 0.3$. OpenModelica](image/13.png){#fig:013 width=70%}

# Задание для самостоятельного выполнения

## Модель SIR с учетом демографии

$$
\begin{cases}
\frac{dS}{dt} = - \beta I S + \mu (N - S), \\
\frac{dI}{dt} = \beta I S - \gamma I - \mu I, \\
\frac{dR}{dt} = \gamma I - \mu R,
\end{cases}
$$

где $\nu$ -- константа, которая равна коэффициенту смертности и рождаемости.

## Задание

- реализовать модель SIR с учётом процесса рождения гибели особей в xcos (в том числе и с использованием блока Modelica), а также в OpenModelica;
- построить графики эпидемического порога при различных значениях параметров модели (в частности изменяя параметр μ);
- сделать анализ полученных графиков в зависимости от выбранных значений параметров модели

## Реализация модели в xcos

![Задать переменные окружения в xcos](image/14.png){#fig:014 width=55%}

## Реализация модели в xcos

![Модель SIR с учетом демографии в xcos](image/15.png){#fig:015 width=70%}

## Реализация модели в xcos

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.3$, $\mu = 0.1$](image/16.png){#fig:016 width=60%}

## Реализация модели с помощью блока Modelica в xcos

![Модель SIR с учетом демографии в xcos с применением блока Modelica](image/17.png){#fig:017 width=60%}

## Реализация модели с помощью блока Modelica в xcos

:::::::::::::: {.columns align=center}
::: {.column width="50%"}

![Ввод значений входных параметров блока Modelica для модели](image/18.png){#fig:018 width=70%}

:::
::: {.column width="50%"}

![Ввод функции блока Modelica для модели](image/19.png){#fig:019 width=70%}

:::
::::::::::::::

## Реализация модели с помощью блока Modelica в xcos

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.3$, $\mu = 0.1$. Блок Modelica](image/20.png){#fig:020 width=55%}

## Реализация модели в OpenModelica

![Модель SIR с учетом демографии в OpenModelica](image/21.png){#fig:021 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.3$, $\mu = 0.1$. OpenModelica](image/sir_0.1.png){#fig:022 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.3$, $\mu = 0.3$. OpenModelica](image/sir_0.3.png){#fig:023 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.3$, $\mu = 0.7$. OpenModelica](image/sir_0.7.png){#fig:024 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1.5$, $\nu = 0.3$, $\mu = 0.1$. OpenModelica](image/sir_b1.5.png){#fig:025 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 2$, $\nu = 0.3$, $\mu = 0.1$. OpenModelica](image/sir_b2.png){#fig:026 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 10$, $\nu = 0.3$, $\mu = 0.1$. OpenModelica](image/sir_b10.png){#fig:027 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.5$, $\mu = 0.1$. OpenModelica](image/sir_nu0.5.png){#fig:028 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.8$, $\mu = 0.1$. OpenModelica](image/sir_nu0.8.png){#fig:029 width=70%}

## Анализ графиков при разных параметрах модели

![График решения модели SIR с учетом демографии при $\beta = 1$, $\nu = 0.9$, $\mu = 0.1$. OpenModelica](image/sir_nu0.9.png){#fig:030 width=70%}

# Выводы

В результате выполнения работы была исследована модель SIR при помощи xcos и OpenModelica.

