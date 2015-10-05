## О проекте

Автонастройка сервера для CS-Cart и Multi-Vendor 4.0+.

## Установка

    curl -sL http://cartoma.tk/installer | bash

## Использование

Укажите доменное имя в config/simple.json и запустите настройку:

    ansible-playbook lamp.yml -e @config/simple.json

Пароли генерируются автоматически и сохраняются в каталоге credentials.

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
