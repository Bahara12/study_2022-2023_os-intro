---
## Front matter
title: "Шаблон отчёта по лабораторной работе 1 "
subtitle: "Простейший вариант"
author: "Абдуллахи Бахара"

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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание
 Я уже установила виртуальный Virtualbox в прошлом семестре, поэтому мне не нода было.
Следующим шагом будет загрузка Linux Feedora Sway.
 
![Название рисунка](image/0.jpg){#fig:001 width=100%}

-Далее вам необходимо установить Linux Fedora Sway на виртуальную машину.
![Название рвисунка](image/1.jpg){#fig:001 width=100%}

![Название рвисунка](image/2.jpg){#fig:001 width=100%}

-нужно указать объем памяти и я указала 8192 мб

![Название рвисунка](image/3.jpg){#fig:001 width=100%}

-Измените размер виртуального жесткого диска на 80 ГБ.

![Название рвисунка](image/4.jpg){#fig:001 width=100%}

-Теперь вам нужно открыть настройку, изменить настройку дисплея и выбрать 3D.

![Название рвисунка](image/5.jpg){#fig:001 width=100%}

![Название рвисунка](image/6.jpg){#fig:001 width=710%}

-Теперь все готово и вам нужно запустить виртуальную машину.

![Название рвисунка](image/7.jpg){#fig:001 width=100%}

-Я запустила виртуальную машину через Troubleshooting:

![Название рвисунка](image/8.jpg){#fig:001 width=100%}

-машина запустилась:

![Название рвисунка](image/29.jpg){#fig:001 width=100%}

-Чтобы начать установку Fedora, вам нужно нажать клавишу Ctrl+d, откроется экран и вам нужно написать Liveinst.

![Название рвисунка](image/9.jpg){#fig:001 width=100%}

-Я выбрала русский язык для установки:

![Название рвисунка](image/10.jpg){#fig:001 width=100%}

Настройка клавиатуры (английская и русская)

![Название рвисунка](image/11t.jpg){#fig:001 width=100%}

-При выборе места установки оставим все как есть.

![Название рвисунка](image/13.jpg){#fig:001 width=100%}

-Теперь вам нужно создать имя пользователя и пароль.

![Название рвисунка](image/14.jpg){#fig:001 width=100%}

-Теперь все готово и можно приступать к установке.

![Название рвисунка](image/18.jpg){#fig:001 width=100%}

-установка окончена

![Название рвисунка](image/17.jpg){#fig:001 width=100%}

-После завершения установки необходимо завершить работу.

![Название рвисунка](image/33.jpg){#fig:001 width=100%}

-Теперь в разделе «носители» нужно извлечь диск из привода.

![Название рвисунка](image/21.jpg){#fig:001 width=100%}

-перезагрузите машину

![Название рвисунка](image/31.jpg){#fig:001 width=100%}

-и все работает нормально.

![Название рвисунка](image/32.jpg){#fig:001 width=100%}

![Название рвисунка](image/30.jpg){#fig:001 width=100%}


# домашнее задание:

1: Версия ядра Linux
можно посмотреть командой dmsg | grep-i "Linux version"

![Название рвисунка](image/22.jpg){#fig:001 width=100%}

2:частота процессора (обнаруженный Mhz процессор)
можно посмотреть командой dmsg |grep-i "Mhz"

![Название рвисунка](image/23.jpg){#fig:001 width=100%}

3: модель процессора(CPU0)
можно посмотреть командой cat/proc/cpuinfo|grep "model name"

![Название рвисунка](image/24.jpg){#fig:001 width=100%}

4:Доступная сумма RAM (Memory available)
можно посмотреть командой free-m

![Название рвисунка](image/25.jpg){#fig:001 width=100%}

5:Тип обнаруженного гипервизора,можно посмотреть командой dmsg|grep-i "hypervisor detected"

![Название рвисунка](image/26.jpg){#fig:001 width=100%}

6: Тип файловой системы корневого раздела,ожно посмотреть командой findmnt

![Название рвисунка](image/27.jpg){#fig:001 width=100%}


7: Последовательность монтирования файловой системы:можно посмотреть командой dmsg|grep-i "mount"

![Название рвисунка](image/28.jpg){#fig:001 width=100%}

![Название рвисунка](image/.jpg){#fig:001 width=70%}

Описываются проведённые действия, в качестве иллюстрации даётся ссылка на иллюстрацию (рис. [-@fig:001]).

![Название рвисунка](image/.jpg){#fig:001 width=70%}
`ё``
# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
