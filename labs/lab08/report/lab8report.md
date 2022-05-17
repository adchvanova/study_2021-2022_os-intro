---
## Front matter
title: "Отчёта по лабораторной работе 8"
subtitle: "Текстовой редактор vi"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

Задание 1. Создание нового файла с использованием vi

1. Создайте каталог с именем ~/work/os/lab06.

2. Перейдите во вновь созданный каталог.

3. Вызовите vi и создайте файл hello.sh

4. Нажмите клавишу i и вводите текст.

5. Нажмите клавишу Esc для перехода в командный режим после завершения ввода
текста.

6. Нажмите : для перехода в режим последней строки и внизу вашего экрана появится приглашение в виде двоеточия.

7. Нажмите w (записать) и q (выйти), а затем нажмите клавишу Enter для сохранения вашего текста и завершения работы.

8. Сделайте файл исполняемым


Задание 2. Редактирование существующего файла

1. Вызовите vi на редактирование файла

2. Установите курсор в конец слова HELL второй строки.

3. Перейдите в режим вставки и замените на HELLO. Нажмите Esc для возврата в командный режим.

4. Установите курсор на четвертую строку и сотрите слово LOCAL.

5. Перейдите в режим вставки и наберите следующий текст: local, нажмите Esc для возврата в командный режим.

6. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую следующий текст: echo $HELLO.

7. Нажмите Esc для перехода в командный режим.

8. Удалите последнюю строку.

9. Введите команду отмены изменений u для отмены последней команды.

10. Введите символ : для перехода в режим последней строки. Запишите произведённые изменения и выйдите из vi.

# Теоретическое введение

В большинстве дистрибутивов Linux в качестве текстового редактора по умолчанию устанавливается интерактивный экранный редактор vi (Visual display editor).

Редактор vi имеет три режима работы:

– командный режим — предназначен для ввода команд редактирования и навигации по редактируемому файлу;

– режим вставки — предназначен для ввода содержания редактируемого файла;

– режим последней (или командной) строки — используется для записи изменений в файл и выхода из редактора.

Для вызова редактора vi необходимо указать команду vi и имя редактируемого файла:

vi <имя_файла>
При этом в случае отсутствия файла с указанным именем будет создан такой файл. Переход в командный режим осуществляется нажатием клавиши Esc . Для выхода из редактора vi необходимо перейти в режим последней строки: находясь в командном режиме, нажать Shift-; (по сути символ : — двоеточие), затем:

– набрать символы wq, если перед выходом из редактора требуется записать изменения в файл;

– набрать символ q (или q!), если требуется выйти из редактора без сохранения.

# Выполнение лабораторной работы

Задание 1. Создание нового файла с использованием vi

1. Создайте каталог с именем ~/work/os/lab06.Перейдите во вновь созданный каталог.(рис. [-@fig:001])

![Создание каталога с именем ~/work/os/lab06 и переход в него](image/n1.1-2.png){ #fig:001 width=70% }

2. Вызовите vi и создайте файл hello.sh (рис. [-@fig:002])

vi hello.sh 


![ Вызов vi и создание файла hello.sh](image/n1.3.png){ #fig:002 width=70% }

3. Нажмите клавишу i и вводите текст. Нажмите клавишу Esc для перехода в командный режим после завершения ввода текста. Нажмите : для перехода в режим последней строки и внизу вашего экрана появится приглашение в виде двоеточия.(рис. [-@fig:003])

![Редактирование файла hello.sh](image/4.png){ #fig:003 width=70% }

4. Нажмите w (записать) и q (выйти), а затем нажмите клавишу Enter для сохранения вашего текста и завершения работы.(рис. [-@fig:004])

![Запись файла и выход из него ](image/n1.7.png){ #fig:004 width=70% }

5. Сделайте файл исполняемым(рис. [-@fig:005])

![Делаем файл исполняемым](image/n1.8.png){ #fig:005 width=70% }

Задание 2. Редактирование существующего файла

1. Вызовите vi на редактирование файла(рис. [-@fig:006])

vi ~/work/os/lab06/hello.sh

![Делаем файл исполняемым](image/n2.1.png){ #fig:006 width=70% }


2. Установите курсор в конец слова HELL второй строки. Перейдите в режим вставки и замените на HELLO. Нажмите Esc для возврата в командный режим. Установите курсор на четвертую строку и сотрите слово LOCAL.
Перейдите в режим вставки и наберите следующий текст: local, нажмите Esc для возврата в командный режим. Установите курсор на последней строке файла. Вставьте после неё строку, содержащую следующий текст: echo $HELLO. Нажмите Esc для перехода в командный режим. Удалите последнюю строку.
Введите команду отмены изменений u для отмены последней команды.
Введите символ : для перехода в режим последней строки. Запишите произведённые изменения и выйдите из vi.(рис. [-@fig:007])

![Файл после всех изменений](image/n2.png){ #fig:007 width=70% }

# Выводы

Мы познакомились с операционной системой Linux. Получили практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Контрольные вопросы

1. Дайте краткую характеристику режимам работы редактора vi.

- командный режим − предназначен для ввода команд редактирования и навигации по редактируемому файлу;

-	режим вставки − предназначен для ввода содержания редактируемого файла;

-	режим последней (или командной) строки − используется для записи изменений в файл и выхода из редактора.

2. Как выйти из редактора, не сохраняя произведённые изменения?

нужно в режиме командной строки нажать клавиши «:» «q» «!»

3. Назовите и дайте краткую характеристику командам позиционирования.

-	«0»(ноль) − переход в начало строки;

-	«$» − переход в конец строки;

-	«G» − переход в конец файла;

-	n«G» − переход на строку с номером n.



4. Что для редактора vi является словом?

При использовании прописных W и B под разделителями понимаются только пробел, табуляция и возврат каретки. При использовании строчных w и b под разделителями понимаются также любые знаки пунктуации.

5. Каким образом из любого места редактируемого файла перейти в начало(конец) файла?

Для того чтобы перейти из любого места редактируемого файла в начало (конец) файла, нужно в режиме командной строки нажать клавиши «1» «G» («G»).

6. Назовите и дайте краткую характеристику основным группам команд редактирования.

	Вставка текста

-	«а» − вставить текст после курсора;

-	«А» − вставить текст в конец строки;

-	«i» − вставить текст перед курсором;

-	n «i» − вставить текст n раз;

-	«I» − вставить текст в начало строки.

	Вставка строки

-	«о» − вставить строку под курсором;

-	«О» − вставить строку над курсором.

	Удаление текста

-	«x» − удалить один символ в буфер;

-	«d» «w» − удалить одно слово в буфер;

-	«d» «$» − удалить в буфер текст от курсора до конца строки;

-	«d» «0» − удалить в буфер текст от начала строки до позиции курсора;

-	«d» «d» − удалить в буфер одну строку;

-	n «d» «d» − удалить в буфер n строк.

	Отмена и повтор произведённых изменений

-	«u» − отменить последнее изменение;

-	«.» − повторить последнее изменение.

	Копирование текста в буфер

-	«Y» − скопировать строку в буфер;

-	n «Y» − скопировать n строк в буфер;

-	«y» «w» − скопировать слово в буфер.

	Вставка текста из буфера

-	«p» − вставить текст из буфера после курсора;

-	«P» − вставить текст из буфера перед курсором.

	Замена текста

-	«c» «w» − заменить слово;

-	n «c» «w» − заменить nслов;

-	«c» «$» − заменить текст от курсора до конца строки;

-	«r» − заменить слово;

-	«R» − заменить текст.

	Поиск текста

-	«/» текст − произвести поиск вперёд по тексту указанной строки символов текст;

-	«?» текст − произвести поиск назад по тексту указанной строки символов текст.

	Копирование и перемещение текста

-	«:» n,m «d» – удалить строки с n по m;

-	«:» i,j «m» k – переместить строки с i по j, начиная со строки k;

-	«:» i,j «t» k – копировать строки с i по j в строку k;

-	«:» i,j «w» имя-файла – записать строки с i по j в файл с именем имя-файла.

7. Необходимо заполнить строку символами $. Каковы ваши действия?

необходимо для начала перейти на эту строку,нажав клавиши n«G»,где n–номер строки, далее нажать«0» для перехода в начало строки.Теперь необходимо нажать «c»«», чтобы заменить текст от курсора до конца строки, и ввести символы $.

8. Как отменить некорректное действие, связанное с процессом редактирования?

Чтобы отменить по одному предыдущему действию последовательно, необходимо нажать «u». Чтобы отменить все изменения, произведённые со времени последней записи, нужно нажать «:» «e» «!».

9. Назовите и дайте характеристику основным группам команд режима последней строки.

	Копирование и перемещение текста

-	«:»n,m «d» − удалить строки с n по m;

-	«:»i,j «m» k − переместить строки с i по j, начиная со строки k;

-	«:»i,j «t» k − копировать строки с i по j в строку k;

-	«:»i,j «w» имя-файла − записать строки с i по j в файл с именем имя-файла.

	Запись в файл и выход из редактора

-	«:» «w» − записать изменённый текст в файл, не выходя из vi;

-	«:» «w» имя-файла − записать изменённый текст в новый файл с именем имя-файла;

-	«:» «w» «!» имя-файла − записать изменённый текст в файл с именем имя-файла;

-	«:» «w» «q» − записать изменения в файл и выйти из vi;

-	«:» «q» − выйти из редактора vi;

-	«:» «q» «!» − выйти из редактора без записи;

-	«:» «e» «!» − вернуться в командный режим, отменив все изменения, 
произведённые со времени последней записи.

10. Как определить, не перемещая курсора, позицию, в которой заканчивается строка?

Чтобы определить, не перемещая курсора, позицию, в которой заканчивается строка, нужно в командном режиме находясь на нужной строке нажать «$»и посмотреть на число после запятой в правом нижнем углу экрана 

11. Выполните анализ опций редактора vi (сколько их, как узнать их назначение и т.д.).

Опции редактора vi позволяют настроить рабочую среду. Для задания опций используется команда set (в режиме командной строки). Если вы хотите отказаться от использования опции, то в команде set перед именем опции надо поставить no. Чтобы просмотреть опции редактора vi, необходимо нажать «:» set all 

12. Как определить режим работы редактора vi?

В редакторе vi есть два основных режима: командный режим и режим вставки. По умолчанию работа начинается в командном режиме. В режиме вставки клавиатура используется для набора текста. Для выхода в командный режим используется клавиша Esc или комбинация Ctrl + c. В командном режиме алфавитные клавиши соответствуют командам перемещения и изменения текста.
