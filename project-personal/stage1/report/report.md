---
## Front matter
title: "Индивидуальный проект. 1 этап"
subtitle: Операционные системы"
author: "Шулуужук Айраана Вячеславовна НПИбд-02-22"

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

Размещение на Github pages заготовки для персонального сайта.

# Задание

1. Установить необходимое программное обеспечение.

2. Скачать шаблон темы сайта.

3. Разместить его на хостинге git.

4. Установить параметр для URLs сайта.

5. Разместить заготовку сайта на Github pages.

# Выполнение лабораторной работы

1. Скачиваем архив hugo_extended_0.110.0linux-amd64.tar.gz. (рис. @fig:001)

![скачивание архива](image/1.png){#fig:001 width=70%}

В разделе Загрузки распакуем этот архив и скопируем исполняемый файл hugo. 

В домашнем каталоге создаем папку под названием bin и вставляем в эту папку файл hugo (рис. @fig:002)

![папка bin](image/2.png){#fig:002 width=70%}

2. Cоздаем репозиторий blog, используя шаблон (рис. @fig:003)

![репозитоий blog](image/3.png){#fig:003 width=70%}

В каталоге work клонируем созданный репозиторий blog  (рис. @fig:004)

![клонирование репозитория](image/4.jpg){#fig:004 width=70%}

Выполняем команду в каталоге blog (рис. @fig:005)
```
~/bin/hugo 
```
![команда ~/bin/hugo](image/5.jpg){#fig:005 width=70%}

Удаляем каталог public в каталоге blog (рис. @fig:006)

![удалеие public](image/6.jpg){#fig:006 width=70%}

Возвращаемся в терминал и проводим команду ~/bin/hugo server (рис. @fig:007), получаем ссылку на локальный сайт 

![ссылка на локальный сайт](image/7.png){#fig:007 width=70%}

Переходим на этот сайт через браузер (рис. @fig:008)

![локальный сайт](image/8.png){#fig:008 width=70%}

Для того, чтобы убрать синий блок с текстом нужно перейти в каталог blog-content-index.md (рис. @fig:009).

![файл _index.md](image/9.png){#fig:009 width=70%}

В данном файле следует редактировать текст. Удалаяем следующий набор текста (рис. @fig:010)

![редактирование _index.md](image/10.jpg){#fig:010 width=70%}

После удаления данного текста на сайте сразу исчезнет синий блок (рис. @fig:011)

![сайт после редактирования](image/11.png){#fig:011 width=70%}

3. На github создаем еще один новый репозиторий со специальным названием avshuluuzhuk.github.io (рис. @fig:012)

![новый репозиторий](image/12.jpg){#fig:012 width=70%}

Переходим в каталог work, клонируем новый репозиторий и перейдем в этот каталог  (рис. @fig:013)

![клонирование нового репозитория](image/13.jpg){#fig:013 width=70%}

В новом каталоге переключаемся на ветку main, создаем пустой файл README.md и отправляем его на github для активации репозитория (рис. @fig:014)

![создание пустого файла и добавление на github](image/14.png){#fig:014 width=70%}

Переходим в каталог blog и выполняем команду для подключения каталога public к созданному репозиторию (рис. @fig:015)

![подкючение public к репозиторию](image/15.png){#fig:015 width=70%}

Запускаем mc и редактируем .gitignore. Комментируем #public (рис. @fig:016)

![комментирование public](image/16.png){#fig:016 width=70%}

Командой "cat .gitignore" проверяем файл и после чего снова повторяем команду для подключения каталога к репозиторию  (рис. @fig:017)

![подключение каталога к новому репозиторию](image/17.jpg){#fig:017 width=70%}

С помощью команды "~/bin/hugo" генерируем автоматически файлы в папку public (рис. @fig:018)

![генерация файлов в public](image/18.jpg){#fig:018 width=70%}

Синхронизируем файлы в public с репозиторием. Переходим в public и проверим подключения каталога к репозиторию. После этого отправляем файлы нв сервер (рис. @fig:019)

![загрузка файлов на сервер](image/19.jpg){#fig:019 width=70%}

Обновляем репозиторий и проверяем добавление файлов  (рис. @fig:020)

![сайт с репозиторием](image/20.png){#fig:020 width=70%}

Копируем ссылку на новый сайт и переходим на него  (рис. @fig:021)

![переход на сайт](image/21.png){#fig:021 width=70%}

# Выводы

В ходе выполнения первого этапа индивидуального проекта я научилась размещать на github pages заготовки для персонального сайта 

