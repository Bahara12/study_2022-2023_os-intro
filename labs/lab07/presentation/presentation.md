---
## Front matter
lang: ru-RU
title: " Лабораторной работе 7 "
author:
  - "Абдуллахи Бахара"
institute:
  
  - Объединённый институт ядерных исследований, Дубна, Россия
date: 23 Мар 2024

## i18n babel
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

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---




## Цель работы:
- Ознакомление с файловой системой Linux, её структурой, именами и содержанием
каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке исполь-
зования диска и обслуживанию файловой системы.

## Последовательность выполнения работы:

1. Выполните все примеры, приведённые в первой части описания лабораторной работы.

# Копирование файлов и каталогов:
- Команда cp используется для копирования файлов и каталогов.
Формат команды:
- Примеры:
- 1) Копирование файла в текущем каталоге. Скопировать файл ~/abc1 в файл april и в файл may:

![](./image/1.png)


- 2) Копирование нескольких файлов в каталог. Скопировать файлы april и may в каталог monthly:

![](./image/2.png)

![](./image/2,2.png)

- 3) Копирование файлов в произвольном каталоге. Скопировать файл monthly/may в файл с именем june:

![](./image/3.png)

## Опция i в команде cp выведет на экран запрос подтверждения о перезаписи файла.Для рекурсивного копирования каталогов, содержащих файлы, используется команда cp с опцией r.

- Примеры:
- 1) Копирование каталогов в текущем каталоге. Скопировать каталог monthly в каталог monthly.00:

![](./image/4.png)

- 2) Копирование каталогов в произвольном каталоге. Скопировать каталог monthly.00 в каталог /tmp

![](./image/5.png)

## Перемещение и переименование файлов и каталогов:
# Команды mv и mvdir предназначены для перемещения переименования файлов и каталогов. 

- Формат команды mv:
- Примеры:

- 1) Переименование файлов в текущем каталоге. Изменить название файла april на july в домашнем каталоге:

![](./image/6.png)

- 2) Перемещение файлов в другой каталог. Переместить файл july в каталог monthly.00:

![](./image/7.png)

- 3) Переименование каталогов в текущем каталоге. Переименовать каталог monthly.00 в monthly.01

![](./image/8.png)

- 4) Перемещение каталога в другой каталог. Переместить каталог monthly.01в каталог reports:

![](./image/9.png)

- 5) Переименование каталога, не являющегося текущим. Переименовать каталог reports/monthly.01 в reports/monthly:

![](./image/10.png)


## Изменение прав доступа:

- Права доступа к файлу или каталогу можно изменить, воспользовавшись командой chmod. Сделать это может владелец файла (или каталога) или пользователь с правами
администратора.

- Примеры:
- 1) Требуется создать файл ~/may с правом выполнения для владельца:

![](./image/11.png)

- 2) Требуется лишить владельца файла ~/may права на выполнение:

![](./image/12.png)

- 3) Требуется создать каталог monthly с запретом на чтение для членов группы и всех остальных пользователей:

![](./image/13.png)

![](./image/14.png)

![](./image/15.png)

- 4) Требуется создать файл ~/abc1 с правом записи для членов группы:

![](./image/16.png)


## 2. Выполните следующие действия, зафиксировав в отчёте по лабораторной работе используемые при этом команды и результаты их выполнения:

- Скопируйте файл /usr/include/sys/io.h в домашний каталог и назовите его equipment. Если файла io.h нет, то используйте любой другой файл в каталоге /usr/include/sys/ вместо него.

![](./image/17.png)

- В домашнем каталоге создайте директорию ~/ski.plases.
- Переместите файл equipment в каталог ~/ski.plases.

![](./image/18.png)

- Переименуйте файл ~/ski.plases/equipment в ~/ski.plases/equiplist.
![](./image/19.png)

- Создайте в домашнем каталоге файл abc1 и скопируйте его в каталог ~/ski.plases, назовите его equiplist2.

![](./image/20.png)

![](./image/21.png)

- Создайте каталог с именем equipment в каталоге ~ ski.plases.
- Переместите файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment.

![](./image/22.png)
- Создайте и переместите каталог ~/newdir в каталог ~/ski.plases и назовите его plans.

![](./image/23.png)

## 3. Определите опции команды chmod, необходимые для того, чтобы присвоить перечис- ленным ниже файлам выделенные права доступа, считая, что в начале таких правнет:
- 3.1)  drwxr--r-- ... australia 
- 3.2)  drwx--x--x ... play 
- 3.3)  -r-xr--r-- ... my_os 
- 3.4)  -rw-rw-r-- ... feathers
- При необходимости создайте нужные файлы.

![](./image/24.png)

![](./image/25.png)

![](./image/26.png)

## 4. Проделайте приведённые ниже упражнения, записывая в отчёт по лабораторной работе используемые при этом команды:

- Просмотрите содержимое файла /etc/password.

![cat/etc/passwd](./image/27.png)

- Скопируйте файл ~/feathers в файл ~/file.old.
- Переместите файл ~/file.old в каталог ~/play.

![](./image/28.png)

- Скопируйте каталог ~/play в каталог ~/fun.
- Переместите каталог ~/fun в каталог ~/play и назовите его games.

![](./image/29.png)

-  Лишите владельца файла ~/feathers права на чтение.
- Что произойдёт, если вы попытаетесь просмотреть файл ~/feathers командой cat?
- Что произойдёт, если вы попытаетесь скопировать файл ~/feathers?

![](./image/30.png)

-  Дайте владельцу файла ~/feathers право на чтение.
-  Лишите владельца каталога ~/play права на выполнение.

![](./image/31.png)

-  Перейдите в каталог ~/play. Что произошло?
-  Перейдите в каталог ~/play. Что произошло?

![](./image/32.png)

## 5. Прочитайте man по командам mount, fsck, mkfs, kill и кратко их охарактеризуйте, приведя примеры.

![ man mount](./image/33.png)

![man fsck](./image/34.png)

![man mkfs](./image/35.png)

![man kill](./image/36.png)


# Спасибо за винимание!




  
