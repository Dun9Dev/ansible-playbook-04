# Playbook для установки ClickHouse, Vector и Lighthouse

## Описание
Этот playbook устанавливает и настраивает три компонента:
- **ClickHouse** — колоночная БД для аналитики
- **Vector** — сборщик и обработчик логов
- **Lighthouse** — веб-интерфейс для ClickHouse

## Требования
- Ansible 2.10 или выше
- Docker (для тестирования) или реальные хосты с Ubuntu/CentOS

## Переменные
Переменные для каждой роли находятся в соответствующих репозиториях:
- [vector-role](https://github.com/Dun9Dev/ansible-vector-role)
- [lighthouse-role](https://github.com/Dun9Dev/ansible-lighthouse-role)

## Использование

1. Установите зависимости:
```bash
ansible-galaxy install -r requirements.yml

2. Запустите playbook:
```bash
ansible-playbook -i inventory/prod.yml site.yml

