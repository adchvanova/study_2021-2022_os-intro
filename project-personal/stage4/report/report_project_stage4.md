---
## Front matter
title: "Отчёт по 4 этапу Индивидуального проекта"
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

Добавление к сайту ссылок на научные и библиометрические ресурсы. Написание двух постов.

# Задание

Добавить к сайту ссылки на научные и библиометрические ресурсы.

Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:

Google Scholar : https://scholar.google.com/;

ORCID : https://orcid.org/;

ResearchGate : https://www.researchgate.net/;

Academia.edu : https://www.academia.edu/;

arXiv : https://arxiv.org/;

github : https://github.com/.

Сделать пост по прошедшей неделе.

Добавить пост на тему по выбору:

Оформление отчёта. или Создание презентаций. или Работа с библиографией.

# Теоретическое введение

Сайт  — это интернет-ресурс, состоящий из одной, нескольких или множества виртуальных страниц. Так как мы создаем  персональный сайт научного работника необходимо выгрузить на него информацию м ссылки на научные и библиометрические ресурсы, это нужно для того, чтобы посетитель сайта мог найти наши рабы и публикации на других научных ресурсах.

# Выполнение лабораторной работы

Открываем папку с файлом, который нужно отредактировать и пеходим в пунк social . (рис. [-@fig:001])

![Добавление научных и библиометрических ресурсов в md файл](image/1.png){ #fig:001 width=70% }

Подбираем иконки для научных и библиометрических ресурсов. (рис. [-@fig:002])

![Подбор иконок для научных и библиометрических ресурсов ](image/2.png){ #fig:002 width=70% }

Создаем папки в которых будут необходимые файлы для постов. (рис. [-@fig:003])

![Папки для постов](image/3.png){ #fig:003 width=70% }

Пишем посты. Пост о прошлой неделе и о работе с библиографией.(рис. [-@fig:004])

![Написание поста](image/4.png){ #fig:004 width=70% }

Выгружаем все на GitHub. (рис. [-@fig:005])

![Выгрузка на GitHub ](image/7.png){ #fig:005 width=70% }

Проверяем изменения на сайте. (рис. [-@fig:006], [-@fig:007])

![Научные и библиометрические ресурсы, которые появились на сайте ](image/5.png){ #fig:006 width=70% }

![Написанные посты, которые загрузились на сайте ](image/6.png){ #fig:007 width=70% }


# Выводы

Мы добавили на персональный сайт научного работника научные и библиометрические ресурсы,а также написали посты на сайт.(о прошлой неделе и о работе с библиографией.)
