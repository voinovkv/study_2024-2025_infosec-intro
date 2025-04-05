---
## Front matter
title: "Отчет по лабораторной работе №4"
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

Получение практических навыков работы в консоли с расширенными атрибутами файлов

# Выполнение лабораторной работы

1. Определяю расширенные атрибуты файлa file1 (рис. 1).

![Определение атрибутов](image/1.png){#fig:001 width=70%}

2. Изменяю права доступа для файла file1 с помощью chmod 600 (рис. 2).

![Изменение прав доступа](image/2.png){#fig:002 width=70%}

3. Пробую установить на файл file1 расширенный атрибут, в ответ получаю отказ от выполнения операции (рис. 3).

![Попытка установки рассширенных атрибутов](image/3.png){#fig:003 width=70%}

4. Устанавливаю расширенные права уже от имени суперпользователя, теперь нет отказа от выполнения операции (рис. 4).

![Установка расширенных атрибутов](image/4.png){#fig:004 width=70%}

5. От пользователя guest проверяю правильность установки атрибута (рис. 5).

![Проверка атрибутов](image/5.png){#fig:005 width=70%}

6. Выполняю дозапись в файл с помощью echo 'test' >> file1, далее выполняю чтение файла, убеждаюсь, что дозапись была выполнена (рис. 6).

![Дозапись в файл](image/6.png){#fig:006 width=70%}

7. Пробую удалить файл, получаю отказ при попытке переименовать файл(рис. 7).

![Попытка переименовать файл](image/7.png){#fig:007 width=70%}

8. Добавляю расширенный атрибут i от имени суперпользователя, запись в файл, дозапись, переименовать или удалить, ничего из этого сделать нельзя.

# Выводы

В результате выполнения работы я повысил свои навыки использования интерфейса командой строки (CLI), познакомился на примерах с тем, как используются основные и расширенные атрибуты при разграничении доступа. Имел возможность связать теорию дискреционного разделения доступа (дискреционная политика безопасности) с её реализацией на практике в ОС Linux. Опробовали действие на практике расширенных атрибутов «а» и «i»
