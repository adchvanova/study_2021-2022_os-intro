---
## Front matter
title: "Отчёт по 5 этапу Индивидуального проекта"
subtitle: "Персональный сайт научного работника"
author: "Ангелина Чванова Дмитриевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Добавление к сайту записей для персональных проектов и двух постов( по по прошедшей неделе, пост на тему языки научного программирования.)

# Задание

Добавить с сайту все остальные элементы.

Сделать записи для персональных проектов.

Сделать пост по прошедшей неделе.

Добавить пост на тему по выбору. (Языки научного программирования.)

# Теоретическое введение

Сайт  — это интернет-ресурс, состоящий из одной, нескольких или множества виртуальных страниц. Так как мы создаем  персональный сайт научного работника необходимо выгрузить на него персональные проекты, это нужно для того, чтобы посетитель сайта мог посмотреть наши работы.

# Выполнение лабораторной работы


Создаем папки для персональных проектов. (рис. [-@fig:001])

![папки для персональных проектов](image/1.png){ #fig:001 width=70% }

Меняем файл, вставляя информацию о проекте. (рис. [-@fig:002])

![отредактированный файл проекта](image/2.png){ #fig:002 width=70% }

Создаем папки в которых будут необходимые файлы для постов. (рис. [-@fig:003])

![Папки для постов](image/3.png){ #fig:003 width=70% }

Пишем посты. Пост о прошлой неделе и о языках научного программирования.(рис. [-@fig:004])

![Написанипе поста](image/4.png){ #fig:004 width=70% }

Выгружаем все на GitHub. (рис. [-@fig:005])

![Выгрузка на GitHub ](image/7.png){ #fig:005 width=70% }

Проверяем измения на сайте. (рис. [-@fig:006], [-@fig:007])

![измения на сайте ](image/5.png){ #fig:006 width=70% }

![измения на сайте](image/6.png){ #fig:007 width=70% }

# Выводы

Мы добавили к сайту записи для персональных проектов и два поста (по по прошедшей неделе, пост на тему языки научного программирования.)
