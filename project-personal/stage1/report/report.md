---
## Front matter
title: "Отчет по первому этапу индивидуального проекта"
author: "Воинов Кирилл, НКАбд-02-23"

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

Приобретение практических навыков по установке операционной системы Linux на виртуальную машину.

# Задание

1. Установить дистрибутив Kali Linux на виртуальную машину VirtualBox.

# Выполнение лабораторной работы

Открываю VirtualBox, нажимаю `создать`, в появившемся окне выбираю тип операционной системы Linux, версия - Debian, задаю имя машины (рис. 1).

![Выбор имени и операционной системы](image/1.png){#fig:001 width=70%}

Настраиваю основную память и количество выделяемых процессоров, необходимое для работы без помех (рис. 2).

![Настройка оборудования виртуальной машины](image/2.png){#fig:002 width=70%}

Подключаю ранее скачанный образ диска (рис. 3).

![Подключение образа диска](image/3.png){#fig:003 width=70%}

В окне установки Kali выбираю установку (рис. 4).

![Начало становки](image/4.png){#fig:004 width=70%}

Выбираю язык, на котором будет установка (рис. 5).

![Выбор языка установки](image/5.png){#fig:005 width=70%}

Ввожу имя компьютера (рис. 6).

![Ввод имени компьютера](image/6.png){#fig:006 width=70%}

Ввожу имя домена (рис. 7).

![Ввод имени домена.](image/7.png){#fig:007 width=70%}

Ввожу имя пользователя, у которой будут права суперпользователя (рис. 8).

![Настройка учетной записи](image/8.png){#fig:008 width=70%}

Ввожу пароль для созданного пользователя (рис. 9).

![Настройка пароля](image/9.png){#fig:009 width=70%}

Выбираю часовой пояс (рис. 10).

![Настройка времени](image/10.png){#fig:010 width=70%}

Теперь установщик проверяет диски и предлагает различные варианты, в зависимости от настроек. Созданный виртуальный диск чистый, поэтому я выбираю «весь диск» (рис. 11).

![Разметка дисков](image/11.png){#fig:011 width=70%}

Завершаю установку (рис. 12).

![Завершение установки](image/12.png){#fig:012 width=70%}

Проверяю, что в носителях теперь пусто (рис. 13).

![Проверка носителей](image/13.png){#fig:013 width=70%}

Вход в систему выполнен успешно, как и ее загрузка (рис. 14).

![Успешная загрузка системы](image/14.png){#fig:014 width=70%}

# Выводы

Приобрёл практические навыки по установке операционной системы Linux на виртуальную машину. Установил дистрибутив Kali LInux на VirtualBox.

# Список литературы. Библиография.
