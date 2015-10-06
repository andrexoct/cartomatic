## О проекте

Автонастройка сервера для CS-Cart и Multi-Vendor 4.0+.

## Быстрый старт

Выполните сценарий с указанием доменного имени магазина:

    curl -sL http://cartoma.tk/installer | bash -s -- yourdomain.ltd

Если не установлен cURL:

    wget -qO - http://cartoma.tk/installer | bash -s -- yourdomain.ltd

Готово. Сервер настроен.

## Ручная установка

Выполните сценарий для установки зависимостей:

    curl -sL http://cartoma.tk/preconf | bash

Перейдите в каталог с конфигурациями и отредактируйте JSON-конфиг:

    cd /srv/cartomatic/<version>
    vim config/simple.json

Дополнительно можете указать настройки сервисов в файлах каталога group_vars/.

Запустите настройку сервера:

    ansible-playbook lamp.yml -c local -e @config/simple.json

Пароли будут автоматически сгенерированы и сохранены в каталоге credentials/.

## Поддерживаемые ОС

* Ubuntu 14.04 x86_64
* Ubuntu 14.10 x86_64
* Ubuntu 15.04 x86_64
* Debian 6 Squeeze x86_64
* Debian 7 Wheezy x86_64
* Debian 8 Jessie x86_64
* CentOS 6 x86_64
* CentOS 7 x86_64

## Ограничения

* Работает на чистых инсталляциях.
* Не работает с несколькими серверами.

## Благодарности

* [@jsjant](https://github.com/jsjant) за название проекта.
* [@hyrintalion](https://www.behance.net/hyrintalion) за логотип.

## Лицензия

GPLv3
