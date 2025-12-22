---
## Front matter
title: "Лабораторная работа №7"
subtitle: "Введение в работу с данными"
author: "Доберштейн А. С."

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib

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
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Основная цель работы — освоить специализированные пакеты Julia для обработки данных.

# Выполнение лабораторной работы

Повторим примеры из лабораторной работы. (рис. [-@fig:001] - [-@fig:039]). 

![Считывание данных](image/1.png){#fig:001 width=70%}

![Считывание данных](image/2.png){#fig:002 width=70%}

![Считывание данных](image/3.png){#fig:003 width=70%}

![Считывание данных](image/4.png){#fig:004 width=70%}

![Считывание данных](image/5.png){#fig:005 width=70%}

![Запись данных в CSV-файл](image/6.png){#fig:006 width=70%}

![Словари](image/7.png){#fig:007 width=70%}

![Словари](image/8.png){#fig:008 width=70%}

![DataFrames](image/9.png){#fig:009 width=70%}

![DataFrames](image/10.png){#fig:010 width=70%}

![DataFrames](image/11.png){#fig:011 width=70%}

![RDatasets](image/12.png){#fig:012 width=70%}

![RDatasets](image/13.png){#fig:013 width=70%}

![Работа с переменными отсутствующего типа (Missing Values)](image/14.png){#fig:014 width=70%}

![Работа с переменными отсутствующего типа (Missing Values)](image/15.png){#fig:015 width=70%}

![Работа с переменными отсутствующего типа (Missing Values)](image/16.png){#fig:016 width=70%}

![Работа с переменными отсутствующего типа (Missing Values)](image/17.png){#fig:017 width=70%}

![FileIO](image/18.png){#fig:018 width=70%}

![FileIO](image/19.png){#fig:019 width=70%}

![Кластеризация данных. Метод k-средних](image/20.png){#fig:020 width=70%}

![Кластеризация данных. Метод k-средних](image/21.png){#fig:021 width=70%}

![Кластеризация данных. Метод k-средних](image/22.png){#fig:022 width=70%}

![Кластеризация данных. Метод k-средних](image/23.png){#fig:023 width=70%}

![Кластеризация данных. Метод k-средних](image/24.png){#fig:024 width=70%}

![Кластеризация данных. Метод k-средних](image/25.png){#fig:025 width=70%}

![Кластеризация данных. Метод k-средних](image/26.png){#fig:026 width=70%}

![Кластеризация данных. Метод k-средних](image/27.png){#fig:027 width=70%}

![Кластеризация данных. Метод k-средних](image/28.png){#fig:028 width=70%}

![Кластеризация данных. Метод k-средних](image/29.png){#fig:029 width=70%}

![Кластеризация данных. Метод k ближайших соседей](image/30.png){#fig:030 width=70%}

![Кластеризация данных. Метод k ближайших соседей](image/31.png){#fig:031 width=70%}

![Кластеризация данных. Метод k ближайших соседей](image/32.png){#fig:032 width=70%}

![Обработка данных. Метод главных компонент](image/33.png){#fig:033 width=70%}

![Обработка данных. Метод главных компонент](image/34.png){#fig:034 width=70%}

![Обработка данных. Метод главных компонент](image/35.png){#fig:035 width=70%}

![Обработка данных. Линейная регрессия](image/36.png){#fig:036 width=70%}

![Обработка данных. Линейная регрессия](image/37.png){#fig:037 width=70%}

![Обработка данных. Линейная регрессия](image/38.png){#fig:038 width=70%}

![Обработка данных. Линейная регрессия](image/39.png){#fig:039 width=70%}

Выполним задания для самостоятельного выполнения: (рис. [-@fig:040] - [-@fig:057]). 

Используем Clustering.jl для кластеризации на основе k-средних. Сделаем точечную диаграмму полученных кластеров. Для этого проиндексируем фрейм данных, преобразуем его в массив и транспонируем.

![Задание для самостоятельного выполнения №1](image/40.png){#fig:040 width=70%}

![Задание для самостоятельного выполнения №1](image/41.png){#fig:041 width=70%}

![Задание для самостоятельного выполнения №1](image/42.png){#fig:042 width=70%}

![Задание для самостоятельного выполнения №1](image/43.png){#fig:043 width=70%}

Cоздадим матрицу данных 𝑋2, которая добавляет столбец единиц в начало матрицы данных, и решим систему линейных уравнений.

![Задание для самостоятельного выполнения №2](image/44.png){#fig:044 width=70%}

![Задание для самостоятельного выполнения №2](image/45.png){#fig:045 width=70%}

![Задание для самостоятельного выполнения №2](image/46.png){#fig:046 width=70%}

![Задание для самостоятельного выполнения №2](image/47.png){#fig:047 width=70%}

![Задание для самостоятельного выполнения №2](image/48.png){#fig:048 width=70%}

![Задание для самостоятельного выполнения №2](image/49.png){#fig:049 width=70%}

![Задание для самостоятельного выполнения №3](image/50.png){#fig:050 width=70%}

Пусть $S = 100, \, T = 1, \, n = 10000, \, \sigma = 0.3$ и $r = 0.08$. Попробуем  построить траекторию курса акций. 

![Задание для самостоятельного выполнения №3](image/51.png){#fig:051 width=70%}

![Задание для самостоятельного выполнения №3](image/52.png){#fig:052 width=70%}

![Задание для самостоятельного выполнения №3](image/53.png){#fig:053 width=70%}

Создадим функцию `createPath (S ::Float64, r ::Float64, sigma ::Float64, T ::Float64, n ::Int64)`, которая создает траекторию цены акции с учетом начальных параметров. Используем `createPath`, чтобы создать 10 разных траекторий и построим их все на одном графике

![Задание для самостоятельного выполнения №3](image/54.png){#fig:054 width=70%}

![Задание для самостоятельного выполнения №3](image/55.png){#fig:055 width=70%}

Распараллелим генерацию траектории. Можем использовать `Threads.@threads`, `pmap` и `@parallel`

![Задание для самостоятельного выполнения №3](image/56.png){#fig:056 width=70%}

![Задание для самостоятельного выполнения №3](image/57.png){#fig:057 width=70%}

# Выводы

В результате выполнения работы были освоены специализированные пакеты Julia для обработки данных.