---
## Front matter
title: "Лабораторная работа № 3."
subtitle: "Операционные системы"
author: "Шулуужук Айраана Вячеславовна"

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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

1. Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.

2. В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве,
поскольку он должен содержать скриншоты, Makefile и т.д)

# Выполнение лабораторной работы

1. Для обработки файлов в формате markdown, необходимо установить pandoc, pandoc-crossref, texlive

2. Открываем в текстовом редакторе отчет лабораторной работы 2 и редактируем шаблон (рис. @fig:001) (рис. @fig:002).

![редактирование шаблона](image/1.png){#fig:001 width=70%}

![редактирование шаблона](image/2.png){#fig:002 width=70%}

3. Далее конвертируем файл в формате markdown в pdf и docx, используя команду make (в папке, где находится файл для компиляции)

4. Проверяем выполнение команды (создание файлов) (рис. @fig:003)

![проверка созданных файлов](image/3.png){#fig:003 width=70%}

# Выводы

В ходе выполнения лабораторной рвботы мы научились оформлять отчеты с помощью легковесного языка markdown, оформили отчеты лабораторной работы № 2 и № 3.

