---
title: Установка
status: live
---

### Установка Сomposer

Cначала установите composer:

    curl -s https://getcomposer.org/installer | php

Создайте файл `composer.json` в корневой директории проекта:

    {
        "require": {
            "slim/slim": "2.*"
        }
    }

Установка с помощью Сomposer:

    php composer.phar install

Добавьте эту строчку в файл `index.php` приложения:

    <?php
    require 'vendor/autoload.php';

### Установка вручную

Скачайте и разархивируйте the Slim Framwork в директорию проекта и используйте `require` для его запроса в файле `index.php` приложения. 
Также вам необходимо инициализировать автозагрузчик Slim.

    <?php
    require 'Slim/Slim.php';
    \Slim\Slim::registerAutoloader();
