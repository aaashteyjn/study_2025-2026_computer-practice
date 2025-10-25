---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Линейная алгебра"
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

Основной целью работы является изучение возможностей специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной алгебры.

# Задание

1. Используя Jupyter Lab, повторить примеры из раздела 4.2.
2. Выполнить задания для самостоятельной работы.

# Теоретическое введение

Julia – высокоуровневый свободный язык программирования с динамической типизацией, созданный для математических вычислений [1]. Эффективен также и для написания программ общего назначения. Синтаксис языка схож с синтаксисом других математических языков, однако имеет некоторые существенные отличия.
Для выполнения заданий была использована официальная документация Julia.

# Выполнение лабораторной работы

## Поэлементные операции над многомерными массивами

Повторила примеры из лабораторной работы: (рис. [-@fig:001]-[-@fig:002])

![Поэлементные операции над многомерными массивами](image/1.png){#fig:001 width=70%}

![Поэлементные операции над многомерными массивами](image/2.png){#fig:002 width=70%}

## Транспонирование, след, ранг, определитель и инверсия матрицы

Повторила примеры из лабораторной работы: (рис. [-@fig:003]-[-@fig:005])

![Транспонирование, след, ранг, определитель и инверсия матрицы](image/3.png){#fig:003 width=70%}

![Транспонирование, след, ранг, определитель и инверсия матрицы](image/4.png){#fig:004 width=70%}

![Транспонирование, след, ранг, определитель и инверсия матрицы](image/5.png){#fig:005 width=70%}

## Вычисление нормы векторов и матриц, повороты, вращения

Повторила примеры из лабораторной работы: (рис. [-@fig:006]-[-@fig:008])

![Вычисление нормы векторов и матриц, повороты, вращения](image/6.png){#fig:006 width=70%}

![Вычисление нормы векторов и матриц, повороты, вращения](image/7.png){#fig:007 width=70%}

![Вычисление нормы векторов и матриц, повороты, вращения](image/8.png){#fig:008 width=70%}

## Матричное умножение, единичная матрица, скалярное произведение

Повторила примеры из лабораторной работы: (рис. [-@fig:009])

![Матричное умножение, единичная матрица, скалярное произведение](image/9.png){#fig:009 width=70%}

## Факторизация. Специальные матричные структуры

Повторила примеры из лабораторной работы: (рис. [-@fig:010]-[-@fig:008])

![Факторизация. Специальные матричные структуры](image/10.png){#fig:010 width=70%}

![Факторизация. Специальные матричные структуры](image/11.png){#fig:011 width=70%}

![Факторизация. Специальные матричные структуры](image/12.png){#fig:012 width=70%}

![Факторизация. Специальные матричные структуры](image/13.png){#fig:013 width=70%}

![Факторизация. Специальные матричные структуры](image/14.png){#fig:014 width=70%}

![Факторизация. Специальные матричные структуры](image/15.png){#fig:015 width=70%}

![Факторизация. Специальные матричные структуры](image/16.png){#fig:016 width=70%}

![Факторизация. Специальные матричные структуры](image/17.png){#fig:017 width=70%}

![Факторизация. Специальные матричные структуры](image/18.png){#fig:018 width=70%}

![Факторизация. Специальные матричные структуры](image/19.png){#fig:019 width=70%}

![Факторизация. Специальные матричные структуры](image/20.png){#fig:020 width=70%}

## Общая линейная алгебра

Повторила примеры из лабораторной работы: (рис. [-@fig:021]-[-@fig:022])

![Общая линейная алгебра](image/21.png){#fig:021 width=70%}

![Общая линейная алгебра](image/22.png){#fig:022 width=70%}

## Задания для самостоятельной работы

### №1 Произведение векторов

Выполнила задания с произведением векторов: (рис. [-@fig:023]-[-@fig:024])

![Задание 1.1](image/23.png){#fig:023 width=70%}

![Задание 1.2](image/24.png){#fig:024 width=70%}

### №2 Системы линейных уравнений

Определила функцию для решения СЛАУ: (рис. [-@fig:025])

![Задание 2.1](image/25.png){#fig:025 width=70%}

Решила первую СЛАУ разными методами, сравнила результаты: (рис. [-@fig:026]-[-@fig:029])

![Задание 2.1](image/26.png){#fig:026 width=70%}

![Задание 2.1](image/27.png){#fig:027 width=70%}

![Задание 2.1](image/28.png){#fig:028 width=70%}

![Задание 2.1](image/29.png){#fig:029 width=70%}

Решила СЛАУ с тремя неизвестными: (рис. [-@fig:030]-[-@fig:031])

![Задание 2.2](image/30.png){#fig:030 width=70%}

![Задание 2.2](image/31.png){#fig:031 width=70%}

### №3 Операции с матрицами

Выполнила задания с матрицами: (рис. [-@fig:032]-[-@fig:037])

![Задание 3.1](image/32.png){#fig:032 width=70%}

![Задание 3.1](image/33.png){#fig:033 width=70%}

![Задание 3.2](image/34.png){#fig:034 width=70%}

![Задание 3.2](image/35.png){#fig:035 width=70%}

![Задание 3.3](image/36.png){#fig:036 width=70%}

![Задание 3.3](image/37.png){#fig:037 width=70%}

### №4 Линейные модели экономики

Выполнила задания с линейными моделями экономики: (рис. [-@fig:038]-[-@fig:043])

![Задание 4.1](image/38.png){#fig:038 width=70%}

![Задание 4.1](image/39.png){#fig:039 width=70%}

![Задание 4.2](image/40.png){#fig:040 width=70%}

![Задание 4.2](image/41.png){#fig:041 width=70%}

![Задание 4.3](image/42.png){#fig:042 width=70%}

![Задание 4.3](image/43.png){#fig:043 width=70%}

# Выводы

В результате выполнения данной лабораторной работы я изучила возможности специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной алгебры.