---
## Front matter
title: "Шаблон отчёта по лабораторной работе 4 "
subtitle: "Продвинутое использование git"
author: "Абдуллахи Бахара"

---
}


# Цель работы
- Получение навыков правильной работы с репозиториями git.

# Задание

- Выполнить работу для тестового репозитория.

- Преобразовать рабочий репозиторий в репозиторий с git-flow и conventional commits.

# Выполнение лабораторной работы:

## Установка программного обеспечения

- Установка git-flow:
- Linux
- Fedora
- Установка из коллекции репозиториев Copr (https://copr.fedorainfracloud.org/coprs/elegos/gitflow/):

 # Enable the copr repository
 dnf copr enable elegos/gitflow
 # Install gitflow
 dnf install gitflow

![](image/1.jpg){#fig:001 width=100%}

![](image/2.jpg){#fig:001 width=100%}

![](image/3.jpg){#fig:001 width=100%}

Установка Node.js :

![](image/4.jpg){#fig:001 width=100%}

- Чтобы установить apt-get install pnpm, нужно установить apt с помощью этого камнда dnf install apt:


![](image/5.jpg){#fig:001 width=100%}

![](image/6.jpg){#fig:001 width=100%}

# Настройка Node.js:

- Для работы с Node.js добавим каталог с исполняемыми файлами, устанавливаемыми yarn, в переменную PATH.

![](image/7.jpg){#fig:001 width=100%}

- Запустите:
- Перелогиньтесь, или выполните:

![](image/8.jpg){#fig:001 width=100%}

# Общепринятые коммиты: 
- commitizen:

- Данная программа используется для помощи в форматировании коммитов.

![](image/9.jpg){#fig:001 width=100%}

- При этом устанавливается скрипт git-cz, который мы и будем использовать для коммитов.

- standard-changelog:

- Данная программа используется для помощи в создании логов.

![](image/10.jpg){#fig:001 width=100%}

- Практический сценарий использования git:

1) Подключение репозитория к github

- Создайте репозиторий на GitHub. Для примера назовём его git-extended.

![](image/11.jpg){#fig:001 width=100%}
![](image/12.jpg){#fig:001 width=100%}
![](image/13.jpg){#fig:001 width=100%}
![](image/14.jpg){#fig:001 width=100%}

# Делаем первый коммит и выкладываем на github:

- Сначала мы входим в файл git-extended, затем создадим файл README.md, открываем там README.md, потом с помощью nano там напишим README.md после этого начинаем коммитить на github:

![](image/15.jpg){#fig:001 width=100%}

# Конфигурация общепринятых коммитов:
- Конфигурация для пакетов Node.js

![](image/16.jpg){#fig:001 width=100%}

- Сконфигурим формат коммитов. Для этого добавим в файл package.json команду для формирования коммитов:

![](image/17.jpg){#fig:001 width=100%}

- добавим новые файлы, зафиксируем их и отправим на Gthub:


![](image/18.jpg){#fig:001 width=100%}

# Конфигурация git-flow: 

- мы инициализируем git-flow  и устанавливаем префикс для ярлыков v.

![](image/19.jpg){#fig:001 width=100%}

- Проверьте, что Вы на ветке develop:
- Загрузите весь репозиторий в хранилище:

![](image/20.jpg){#fig:001 width=100%}


- Установите внешнюю ветку как вышестоящую для этой ветки:


![](image/21.jpg){#fig:001 width=100%}

- Создадим релиз с версией 1.0.0

![](image/22.jpg){#fig:001 width=100%}

- Создадим журнал изменений

![](image/23.jpg){#fig:001 width=100%}

- Добавим журнал изменений в индекс:

![](image/24.jpg){#fig:001 width=100%}
![](image/25.jpg){#fig:001 width=100%}
![](image/26.jpg){#fig:001 width=100%}

- Зальём релизную ветку в основную ветку:

![](image/27.jpg){#fig:001 width=100%}

- Отправим данные на github:

![](image/28.jpg){#fig:001 width=100%}

- Создадим релиз на github. Для этого будем использовать утилиты работы с github:

![](image/29.jpg){#fig:001 width=100%}

# Работа с репозиторием git:

-  Разработка новой функциональности:

- Создадим ветку для новой функциональности:

![](image/31.jpg){#fig:001 width=100%}

- следует объединить ветку:

![](image/32.jpg){#fig:001 width=100%}

- Создание релиза git-flow:
- Создадим релиз с версией 1.2.3:

![](image/33.jpg){#fig:001 width=100%}

- Обновите номер версии в файле package.json.


![](image/34.jpg){#fig:001 width=100%}

- Создадим журнал изменений

![](image/35.jpg){#fig:001 width=100%}

- Добавим журнал изменений в индекс
- Зальём релизную ветку в основную ветку

 ![](image/36.jpg){#fig:001 width=100%}
 
 ![](image/37.jpg){#fig:001 width=100%}
 
 - Отправим данные на github 
 
 - Создадим релиз на github с комментарием из журнала изменений: 
  
  ![](image/38.jpg){#fig:001 width=100%}
  

# Выводы:

- Получение навыков правильной работы с репозиториями git.


