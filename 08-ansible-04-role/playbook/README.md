# Playbook для установки LightHouse, ClickHouse и Vector на VM c CentOS7

## Описание

Playbook устанавливает на managed хосты LightHouse, ClickHouse и Vector

## Роли

Источники:

- https://github.com/AlexeySetevoi/ansible-clickhouse
- https://github.com/zemlyachev/vector-role
- https://github.com/zemlyachev/lighthouse-role

## Запуск

- Заполнить в inventory/prod.yml ip адреса хостов, на которые необходимо установить LightHouse, ClickHouse и Vector
- Команда запуска:
  
```sh
ansible-playbook -i /inventory/prod.yml /site.yml
```
