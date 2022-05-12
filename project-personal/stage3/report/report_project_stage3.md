---
## Front matter
title: "Отчёт по 3 этапу Индивидуального проекта"
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

Добавление на персональный сайт научного работника список достижений.
(информация о навыках (Skills), информация об опыте (Experience), информация о достижениях (Accomplishments)), а также написание постов на сайт.

# Задание

Добавить к сайту достижения.

Список достижений.

Добавить информацию о навыках (Skills).

Добавить информацию об опыте (Experience).

Добавить информацию о достижениях (Accomplishments).

Сделать пост по прошедшей неделе.

Добавить пост на тему по выбору:

Легковесные языки разметки или Языки разметки. LaTeX. или Язык разметки Markdown.

# Теоретическое введение

Сайт  — это интернет-ресурс, состоящий из одной, нескольких или множества виртуальных страниц. Так как мы создаем  персональный сайт научного работника необходимо выгрузить на него информацию о достижениях, навыках и опыте работы, это нужно для того, чтобы посетитель сайта мог узнать о работнике больше.


# Выполнение лабораторной работы

Открываем папку с файлами, которые нужно отредактироватьдля добавления данных о навыках, опыте, достижениях. (рис. [-@fig:001])

![Название рисунка](image/1.png){ #fig:001 width=70% }

Редактируем информацию о навыках. (рис. [-@fig:002])

![Редактирование информации о навыках](image/2.png){ #fig:002 width=70% }

Редактируем информацию об опыте. (рис. [-@fig:003])

![Редактирование информации об опыте](image/3.png){ #fig:003 width=70% }

Редактируем информацию о достижениях. (рис. [-@fig:004])

![Редактирование информации о достижениях](image/4.png){ #fig:004 width=70% }

Создаем папки в которых будут необходимые файлы для постов. (рис. [-@fig:005])

![Папки для постов](image/6.png){ #fig:005 width=70% }

Выгружаем все на GitHub. (рис. [-@fig:006])

![Название рисунка](image/11.png){ #fig:006 width=70% }

Проверяем измения на сайте. (рис. [-@fig:007], [-@fig:008], [-@fig:009], [-@fig:010])

![Измененная информация о навыках на сайте](image/7.png){ #fig:007 width=70% }

![Измененная информация об опыте на сайте](image/8.png){ #fig:008 width=70% }

![Измененная информация о достижениях на сайте](image/9.png){ #fig:009 width=70% }

![Добавленные посты](image/10.png){ #fig:010 width=70% }


# Выводы

Мы добавили на персональный сайт научного работника список достижений.
(информация о навыках (Skills), информация об опыте (Experience), информация о достижениях (Accomplishments)), а также написали посты на сайт.(о прошлой неделе и о Языке разметки Markdown.)

