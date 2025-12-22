---
## Front matter
title: "Лабораторная работа №6"
subtitle: "Решение моделей в непрерывном и дискретном времени"
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

Основной целью работы является освоение специализированных пакетов для решения задач в непрерывном и дискретном времени.

# Выполнение лабораторной работы

Повторим примеры из лабораторной работы. (рис. [-@fig:001] - [-@fig:010]). 

![Решение обыкновенных дифференциальных уравнений](image/1.png){#fig:001 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/2.png){#fig:002 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/3.png){#fig:003 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/4.png){#fig:004 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/5.png){#fig:005 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/6.png){#fig:006 width=70%}

![Решение обыкновенных дифференциальных уравнений](image/7.png){#fig:007 width=70%}

![Модель Лотки–Вольтерры](image/8.png){#fig:008 width=70%}

![Модель Лотки–Вольтерры](image/9.png){#fig:009 width=70%}

![Модель Лотки–Вольтерры](image/10.png){#fig:010 width=70%}

Выполним задания для самостоятельного выполнения: (рис. [-@fig:011] - [-@fig:034]).

![Задание для самостоятельного выполнения №1](image/11.png){#fig:011 width=70%}

![Задание для самостоятельного выполнения №1](image/12.png){#fig:012 width=70%}

![Задание для самостоятельного выполнения №1](image/13.png){#fig:013 width=70%}

![Задание для самостоятельного выполнения №2](image/14.png){#fig:014 width=70%}

![Задание для самостоятельного выполнения №2](image/15.png){#fig:015 width=70%}

![Задание для самостоятельного выполнения №2](image/16.png){#fig:016 width=70%}

![Задание для самостоятельного выполнения №3](image/17.png){#fig:017 width=70%}

![Задание для самостоятельного выполнения №3](image/18.png){#fig:018 width=70%}

![Задание для самостоятельного выполнения №4](image/19.png){#fig:019 width=70%}

![Задание для самостоятельного выполнения №4](image/20.png){#fig:020 width=70%}

![Задание для самостоятельного выполнения №5](image/21.png){#fig:021 width=70%}

![Задание для самостоятельного выполнения №5](image/22.png){#fig:022 width=70%}

![Задание для самостоятельного выполнения №5](image/23.png){#fig:023 width=70%}

![Задание для самостоятельного выполнения №6](image/24.png){#fig:024 width=70%}

![Задание для самостоятельного выполнения №6](image/25.png){#fig:025 width=70%}

![Задание для самостоятельного выполнения №6](image/26.png){#fig:026 width=70%}

![Задание для самостоятельного выполнения №7](image/27.png){#fig:027 width=70%}

![Задание для самостоятельного выполнения №7](image/28.png){#fig:028 width=70%}

![Задание для самостоятельного выполнения №7](image/29.png){#fig:029 width=70%}

![Задание для самостоятельного выполнения №7](image/30.png){#fig:030 width=70%}

![Задание для самостоятельного выполнения №8](image/31.png){#fig:031 width=70%}

![Задание для самостоятельного выполнения №8](image/32.png){#fig:032 width=70%}

![Задание для самостоятельного выполнения №8](image/33.png){#fig:033 width=70%}

![Задание для самостоятельного выполнения №8](image/34.png){#fig:034 width=70%}

# Выводы

В результате выполнения работы были освоены пакеты для решения задач в непрерывном и дискретном времени.