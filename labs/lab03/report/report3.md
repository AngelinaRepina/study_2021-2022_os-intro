---
## Front matter
title: "Лабораторная работа №3"
subtitle: "Отчёт по лабораторной работе"
author: "Репина Ангелина Олеговна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bibwork
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
biblio-style: "gost-numeric"work
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

Ntcn
Здесь приводится формулировка цели лабораторной работы. Формулировки
цели для каждой лабораторной работы приведены в методических
указаниях.

Цель данной лабораторной работы ---  научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

– Сделать отчёт по предыдущей лабораторной работе (№2) в формате Markdown.
– В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве,
поскольку он должен содержать скриншоты, Makefile и т.д.)

# Теоретическое введение

Здесь описываются теоретические аспекты, связанные с выполнением работы.

Например, в табл. [-@tbl:std-dir] приведено краткое описание стандартных каталогов Unix.

: Описание некоторых каталогов файловой системы GNU Linux {#tbl:std-dir}

| Имя каталога | Описание каталога                                                                                                          |
|--------------|----------------------------------------------------------------------------------------------------------------------------|
| `/`          | Корневая директория, содержащая всю файловую                                                                               |
| `/bin `      | Основные системные утилиты, необхоfile:///afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/%D0%94%D0%BE%D0%BA%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B/%D0%9B%D0%B0%D0%B1%D0%BE%D1%80%D0%B0%D1%82%D0%BE%D1%80%D0%BD%D0%B0%D1%8F%202/github.png
димые как в однопользовательском режиме, так и при обычной работе всем пользователям     |
| `/etc`       | Общесистемные конфигурационные файлы и файлы конфигурации установленных программ                                           |
| `/home`      | Содержит домашние директории пользователей, которые, в свою очередь, содержат персональные настройки и данные пользователя |
| `/media`     | Точки монтирования для сменных носителей                                                                                   |
| `/root`      | Домашняя директория пользователя  `root`                                                                                   |
| `/tmp`       | Временные файлы                                                                                                            |
| `/usr`       | Вторичная иерархия для данных пользователя                                                                                 |

Более подробно об Unix см. в [@gnu-doc:bash;@newham:2005:bash;@zarrelli:2017:bash;@robbins:2013:bash;@tannenbaum:arch-pc:ru;@tannenbaum:modern-os:ru].

# Выполнение лабораторной работы

1) Создаём учетную запись на https://github.com (рис. [-@fig:001])

![Создание учетной записи ](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на github.png){ #fig:001 width=70% }

2) Настраиваем систему контроля версий git. Синхронизируем учетную запись github с компьютером.
git config --global user.name"Name Surname"
git config --global user.email"work@mail.ru"
После этого создаем новый ключ на github (команда ssh-keygen -C"Angelina Repina <angelinarepina997@gmail.com>") и привязываем его к компьютеру через консоль
![Создание ключа ssh](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на 2.png){ #fig:001 width=70% }

3) Создаём и настраиваем репозиторий на github и его подключение. В github заходим в "repository" и создаём новый репозиторий (имя laboratory)
Копируем ссылку в консоль на репозиторий для дальнейшей работы с файлами

![Добавление ключа в github ](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на 3.png){ #fig:001 width=70% }
![Копирование ключа ](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на 3.1.png){ #fig:001 width=70% }

4) В лабораторной работе описан алгоритм создания структуры каталога через консоль. Мы создаём репозиторий на github и после этого можем работать с каталогом и папками через консоль (перед этим мы копируем ссылку на репозиторий в консоль)
Перед тем, как создать файлы мы заходим в репозиторий

![Репозиторий ](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на Снимок экрана в 2022-04-22 14-22-17.png){ #fig:001 width=70% }
После этого можем создавать наши файлы

5) Настраиваем автоматические подписи комитов

![Настройкам комитов](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на 5.png){ #fig:001 width=70% }


6) Делаем и сохраняем комиты. Настраиваем каталог курса: удаляем лишние файлы и создаём необходимые каталоги.

![Настройка](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/Лабораторная 2/Ссылка на 6.png){ #fig:001 width=70% }


# Выводы

в ходе лабораторной работы я изучила идеологию и применение средств контроля версий и освоила умения по работе с github.

# Список литературы{.unnumbered}

::: {#refs}
:::
