# Роль Lighthouse

Ansible роль для установки и настройки Lighthouse — веб-интерфейса для управления ClickHouse.

## Требования
- Ansible версии 2.10 или выше
- Ubuntu 20.04/22.04 (для других ОС可能需要 адаптация)

## Переменные роли
- `lighthouse_repo` - репозиторий Lighthouse (по умолчанию: "https://github.com/VKCOM/lighthouse.git")
- `lighthouse_version` - версия/ветка (по умолчанию: "master")
- `lighthouse_dir` - директория установки (по умолчанию: "/var/www/lighthouse")
- `nginx_user` - пользователь nginx (по умолчанию: "www-data")

## Зависимости
- nginx (устанавливается автоматически)

## Пример playbook
hosts: lighthouse
roles:

lighthouse-role
## Лицензия
MIT

## Информация об авторе
Создано в учебных целях
