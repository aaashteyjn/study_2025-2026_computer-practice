---
## Front matter
title: "Лабораторная работа №2"
subtitle: "Структуры данных"
author: "Доберштейн Алина Сергеевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
# csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: false # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: FreeSerif
romanfont: FreeSerif
sansfont: FreeSerif
monofont: FreeSerif

mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{unicode-math}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Изучить несколько структур данных, реализованных в Julia, научиться применять их и операции над ними для решения заадач.

# Задание

 1. Используя Jupyter Lab,повторите примеры из раздела 2.2.
 2. Выполните заданиядля самостоятельной работы.

# Теоретическое введение

Рассмотрим несколько структур данных, реализованных в Julia.
Несколько функций (методов), общих для всех структур данных:
– isempty()— проверяет, пуста ли структура данных;
– length() — возвращает длину структуры данных;
– in() — проверяет принадлежность элемента к структуре;
– unique() — возвращает коллекцию уникальных элементов структуры,– reduce() — свёртывает структуру данных в соответствии с заданным бинарным оператором;
– maximum() (или minimum()) — возвращает наибольший (или наименьший) результат вызова функциидля каждого элемента структуры данных.

# Выполнение лабораторной работы

# Кортежи

Кортеж(Tuple) — структура данных (контейнер) в виде неизменяемой индексируемой последовательности элементов какого-либо типа (элементы индексируются с единицы).

Повторила примеры из лабораторной работы с кортежами: (рис. [-@fig:001]-[-@fig:002])

![Кортежи](image/1.png){#fig:001 width=70%}

![Кортежи](image/2.png){#fig:002 width=70%}

# Словари

Словарь — неупорядоченный набор связанных между собой по ключу данных.

Повторила примеры из лабораторной работы со словарями: (рис. [-@fig:003]-[-@fig:004])

![Словари](image/3.png){#fig:003 width=70%}

![Словари](image/4.png){#fig:004 width=70%}

# Множества

Множество,как структураданных в Julia,соответствуетмножеству,как математическому объекту,то есть является неупорядоченной совокупностью элементов какого-либо типа.

Повторила примеры из лабораторной работы с множествами: (рис. [-@fig:005]-[-@fig:007])

![Множества](image/5.png){#fig:005 width=70%}

![Множества](image/6.png){#fig:006 width=70%}

![Множества](image/7.png){#fig:007 width=70%}

# Массивы

Массив — коллекция упорядоченных элементов, размещённая в многомерной сетке. Векторы и матрицы являются частными случаями массивов.

Повторила примеры из лабораторной работы с массивами: (рис. [-@fig:008]-[-@fig:016])

![Массивы](image/8.png){#fig:008 width=70%}

![Массивы](image/9.png){#fig:009 width=70%}

![Массивы](image/10.png){#fig:010 width=70%}

![Массивы](image/11.png){#fig:011 width=70%}

![Массивы](image/12.png){#fig:012 width=70%}

![Массивы](image/13.png){#fig:013 width=70%}

![Массивы](image/14.png){#fig:014 width=70%}

![Массивы](image/15.png){#fig:015 width=70%}

![Массивы](image/16.png){#fig:016 width=70%}

# Задание 1

Выполнила задание для самостоятельной работы №1 (рис. [-@fig:017])

![Задание 1](image/17.png){#fig:017 width=70%}

# Задание 2

Выполнила задание для самостоятельной работы №2 (рис. [-@fig:018]-[-@fig:019])

![Задание 2](image/18.png){#fig:018 width=70%}

![Задание 2](image/19.png){#fig:019 width=70%}

# Задание 3

Выполнила задание для самостоятельной работы №3 (рис. [-@fig:020]-[-@fig:042])

![Задание 3.1](image/20.png){#fig:020 width=70%}

![Задание 3.2](image/21.png){#fig:021 width=70%}

![Задание 3.3](image/22.png){#fig:022 width=70%}

![Задание 3.4](image/23.png){#fig:023 width=70%}

![Задание 3.5](image/24.png){#fig:024 width=70%}

![Задание 3.6](image/25.png){#fig:025 width=70%}

![Задания 3.7, 3.8](image/26.png){#fig:026 width=70%}

![Задание 3.9](image/27.png){#fig:027 width=70%}

![Задание 3.10](image/28.png){#fig:028 width=70%}

![Задание 3.11](image/29.png){#fig:029 width=70%}

![Задание 3.12](image/30.png){#fig:030 width=70%}

![Задание 3.13](image/31.png){#fig:031 width=70%}

![Задание 3.14](image/32.png){#fig:032 width=70%}

![Задание 3.14](image/33.png){#fig:033 width=70%}

![Задание 3.14](image/34.png){#fig:034 width=70%}

![Задание 3.14](image/35.png){#fig:035 width=70%}

![Задание 3.14](image/36.png){#fig:036 width=70%}

![Задание 3.14](image/37.png){#fig:037 width=70%}

![Задание 3.14](image/38.png){#fig:038 width=70%}

![Задание 3.14](image/39.png){#fig:039 width=70%}

![Задание 3.14](image/40.png){#fig:040 width=70%}

![Задание 3.14](image/41.png){#fig:041 width=70%}

![Задание 3.14](image/42.png){#fig:042 width=70%}

# Задание 4

Выполнила задание для самостоятельной работы №4 (рис. [-@fig:043])

![Задание 4](image/43.png){#fig:043 width=70%}

# Задание 5

Выполнила задание для самостоятельной работы №5 (рис. [-@fig:044]-[-@fig:045])

![Задание 5](image/44.png){#fig:044 width=70%}

![Задание 5](image/45.png){#fig:045 width=70%}

# Задание 6

Выполнила задание для самостоятельной работы №6 (рис. [-@fig:046]-[-@fig:048])

![Задание 6](image/46.png){#fig:046 width=70%}

![Задание 6](image/47.png){#fig:047 width=70%}

![Задание 6](image/48.png){#fig:048 width=70%}

# Выводы

В результате выполнения данной лабораторной работы я изучила несколько структур данных, реализованных в Julia, научилась применять их и операции над ними для решения заадач.

# Список литературы{.unnumbered}

::: {#refs}
:::
