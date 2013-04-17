Turboloader
=========

Turboloader - это скрипт на php, который позволяет скачивать серии с сайта turbofilm.tv
> Был написан на коленке, как средство борьбы с неверной html разметкой на данном сайте, из-за которой, в один момент пропала возможность заходить на турбофильм через Apple TV и PlayStation 3.

Предполагает использование на маломощных серверах с примитивным линуксом: роутеры, nas. Не требует базы данных.

## Важно
Пожалуйста, не начинайте сразу выкачивать весь турбофильм и не ставьте в крон чаще чем раз в час. Вас могут забанить за сильную активность.

## Возможности
+ Скачивание новых серий
+ Скачивание всех "ваших" сериалов
+ Правильные названия файлов
+ Почтовые уведомления
+ Почтовые уведомления через smtp

## Установка

+ Загрузите файлы на ваш сервер
+ Создайте config.php на основе config.sample.php
+ Добавьте в крон

## config.php

```
login       - Ваш логин
password    - Ваш пароль
watch       - Отмечать серию как просмотренную после скачивания
language    - Язык на котором скачивать серию
tasks       - Максимальное кол-во серий скачиваемых за раз
email       - email для уведомлений

use_smtp    - использовать smtp отправку писем.
smtp
    - server - smtp server
    - port   - port smtp
    - login  - Логин для авторизации ( test@gmail.com )
    - password

download_dir- Путь к папке для загрузок

cookie_file - путь к cookie файлу, лучше не трогайте
tools       - масив с путями к бинарникам
only_hq     - Скачивать только в высоком качестве
        по умолчанию всегда выбирается наивысшее качество.
        если установить в TRUE, то серии не в HQ скачиваться не будут
owner       - пользователь:группа в линукс системе
        которые будут установленны владельцами файлов
```

## ToDo
Не знаю. Субтитры? Фиксы? У меня все работает и меня все устраивает.