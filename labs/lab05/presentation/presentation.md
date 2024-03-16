---
## Front matter
lang: ru-RU
title: " Лабораторной работе 5 "

author:
  - Абдуллахи Бахара
institute:
  - Российский университет дружбы народов, Москва, Россия
  
date: 15 Мар 2024

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


---


## Выполнение лабораторной работы
## Менеджер паролей pass:
- Установка
- pass  ,   dnf install pass pass-otp
- gopass     ,  dnf install gopass

![](./image/1.jpg)

![](./image/2.jpg)

## Настройка:
- Ключи GPG 

![Просмотр списка ключей](./image/3.jpg)

## Инициализация хранилища: 

![](./image/2.jpg)

- Инициализируем хранилище: pass init <gpg-id or email>

## Синхронизация с git:
- Создадим структуру git:

![](./image/5.jpg)

![](./image/6.jpg)

- pass git init:

![](./image/7.jpg)

![](./image/8.jpg)

- Для синхронизации выполняется следующая команда:

![](./image/10.jpg)

![pass git pull](./image/11.jpg)

![](./image/12.jpg)

![pass git push](./image/13.jpg)

## Прямые изменения: 
 - Следует заметить, что отслеживаются только изменения, сделанные через сам gopass (или pass).
 
 ![](./image/14.jpg)
 
 ![](./image/15.jpg)
 
## Настройка интерфейса с броузером:
- Для взаимодействия с броузером используется интерфейс native messaging.

- Плагин browserpass: Плагин для Firefox: https://addons.mozilla.org/en-US/firefox/addon/browserpass-ce/.

 ![](./image/18.jpg)
 
 ![](./image/19.jpg)
 
## Fedora: 
- dnf copr enable maximbaz/browserpass
- dnf install browserpass
![](./image/16.jpg)

![](./image/17.jpg)
 
## Сохранение пароля:
- Добавить новый файла; 
- touch pass.txt

 ![](./image/20.jpg)

- pass insert [OPTIONAL DIR]/[FILENAME]

![написала пароля](./image/21.jpg)
 ![](./image/22.jpg)
 
 ![](./image/24.jpg)
 
## Управление файлами конфигурации:

- Дополнительное программное обеспечение;
- Установите дополнительное программное обеспечение:

![](./image/25.jpg)

## установите шрифты:
- sudo dnf copr enable peterwu/iosevka

![](./image/26.jpg)
![](./image/27.jpg)

## Установка:
- Установка бинарного файла. Скрипт определяет архитектуру процессора и операционную систему и скачивает необходимый файл:

![ с помощью wget: ](./image/29.jpg)

## Создание собственного репозитория с помощью утилит:

- Будем использовать утилиты командной строки для работы с github.

![](./image/30.jpg)

## Подключение репозитория к своей системе:
- копиравала chezmoi с помощью этого команда :
- sudo cp ./bin/chezmoi /usr/local/bin

![](./image/31.jpg)

## Инициализируйте chezmoi с вашим репозиторием dotfiles:
![](./image/32.jpg)

![](./image/33.jpg)

![](./image/34.jpg)

- Проверьте, какие изменения внесёт chezmoi в домашний каталог, запустив:
![](./image/35.jpg)

![](./image/36.jpg)

## Использование chezmoi на нескольких машинах:
- Установка;
- Установка бинарного файла. Скрипт определяет архитектуру процессора и операционную систему и скачивает необходимый файл:
- с помощью wget:   sh -c "$(wget -qO- chezmoi.io/get)"

![](./image/37.jpg)

![](./image/38.jpg)

- копиравала chezmoi с помощью этого команда в ubuntu :

- sudo cp ./bin/chezmoi /usr/local/bin
![](./image/39.jpg)

![](./image/40.jpg)

![](./image/41.jpg)

## Настройка новой машины с помощью одной команды:
- Ежедневные операции c chezmoi:

 - Извлеките последние изменения из репозитория и примените их
 - Можно извлечь изменения из репозитория и применить их одной командой:
 ![](./image/42.jpg)
 
 - Извлеките последние изменения из своего репозитория и посмотрите, что изменится, фактически не применяя изменения:
 ![](./image/43.jpg)
 
 ![](./image/44.jpg)
 
- Это запускается git pull --autostash --rebase в вашем исходном каталоге, а chezmoi diff затем показывает разницу между целевым состоянием, вычисленным из вашего исходного каталога, и фактическим состоянием.

- Если вы довольны изменениями, вы можете применить их:

 ![](./image/45.jpg)
 
## Автоматически фиксируйте и отправляйте изменения в репозиторий:

- Можно автоматически фиксировать и отправлять изменения в исходный каталог в репозиторий.
 
- Чтобы включить её, добавьте в файл конфигурации ~/.config/chezmoi/chezmoi.toml следующее:
- ~/.config/chezmoi/chezmoi.toml следующее:

 ![](./image/46.jpg)
 
 ![](./image/47.jpg)
  
  

#  Спасибо за винимание!

