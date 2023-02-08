---
## Front matter
title: "Отчёт по лабораторной работе"
subtitle: "Лабораторная работа № 1"
author: "Живцова Анна"

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

Подготовить рабочее пространство для выполнения последующих работ. 
Повторить основы markdown разметки. Настроить работу с удаленным Git репозиторием на Windows.  

# Задание

Создать унифицированное рабочее пространство для выполнения лабораторных работ по дисциплине "Математическое моделирование". 
Оформить отчет о проделанной работе в соответствии с имеющимся шаблоном выполнения работ.

# Теоретическое введение

> **Markdown** — облегчённый язык разметки, созданный с целью обозначения форматирования в простом тексте, с максимальным сохранением его читаемости человеком.     
> **GitHub** — крупнейший веб-сервис для хостинга IT-проектов и их совместной разработки.
Веб-сервис основан на системе контроля версий Git и разработан на Ruby on Rails и Erlang компанией GitHub, Inc (ранее Logical Awesome), принадлежит компании Microsoft.    
![Логотип github](image/github.png){#fig:001 width=70%}

Для комфортной работы с удаленным репозиторием на github, компьютер должен быть связан с системой контроля версий по SSH (протокол Secure Shell). При подключении через SSH проверка подлинности выполняется с помощью файла закрытого ключа на локальном компьютере.      
Для конвертации markdown отчета в форматы pdf и docx на компьютере должен быть установлен pandoc. На входе система pandoc может получать форматы: markdown, reStructuredText, HTML, LaTeX, OPML, Org-mode, DocBook, и Office Open XML (Microsoft Word .docx). И конвертировать их в:
- форматы на основе HTML: XHTML, HTML5, HTML-слайды презентаций (S5, Slidy, Slideous, DZSlides).    
- форматы текстовых процессоров: Microsoft Word docx, OpenOffice/LibreOffice ODT, OpenDocument XML    
- электронные книги: EPUB версии 2 или 3, FictionBook2    
- форматы технической документации: DocBook, GNU TexInfo, groff    
- форматы системы tex: LaTeX, ConTeXt, слайды LaTeX Beamer    
- PDF (с помощью LaTeX)    
- текстовые форматы с облегчённой разметкой: Markdown, reStructuredText, AsciiDoc, MediaWiki, Emacs Org-Mode, Textile     


# Выполнение лабораторной работы

1. Создан репозиторий с шаблонами. 
![Шаблон репозитория курса](image/git.png){#fig:002 width=70%}
2. Создана структура рабочего пространства. 
![Рабочее пространство](image/files.png){#fig:003 width=70%} 
3. Клонирован репозиторий. 
![Клонирование репозитория](image/clone.png){#fig:004 width=70%} 
3. Записан markdown отчет. 
![Markdown](image/markdown.png){#fig:005 width=70%} 
3. Итоговые файлы помещены в репозиторий. 
![commit](image/commit.png){#fig:006 width=70%} 

# Выводы

Настроено рабочее пространство. Оформлен репозиторий. Освежены в памяти основные команды Git и синтаксис markdown.  

# Список литературы{.unnumbered}

1. [Wikipedia GitHub](https://ru.wikipedia.org/wiki/GitHub){#refs:git}    
2. [Wikipedia Markdown](https://ru.wikipedia.org/wiki/Markdown){#refs:markdown}    
