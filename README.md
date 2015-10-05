## О проекте

Сценарий автоматической настройки сервера для CS-Cart и Multi-Vendor 4.0+.

## Установка

    curl -sL http://cartoma.tk/installer | bash

## Использование

Укажите доменное имя магазина в config/simple.json и запустите команду:

    ansible-playbook lamp.yml -e @config/simple.json
