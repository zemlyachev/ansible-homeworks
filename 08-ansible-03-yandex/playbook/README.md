# Playbook для установки LightHouse, ClickHouse и Vector на VM c CentOS7

## Описание

Playbook устанавливает на managed хосты LightHouse, ClickHouse и Vector

## Артефакты

Источники:

- https://github.com/VKCOM/lighthouse.git
- https://packages.clickhouse.com/rpm/stable 
- https://packages.timber.io/vector/

### Версии

- lighthouse: master
- clickhouse_version: "22.3.3.44"
- vector_version: "0.33.0"

Для настройки версий используются соответствующие параметры в group_vars

## Запуск

- Заполнить в inventory/prod.yml ip адреса хостов, на которые необходимо установить LightHouse, ClickHouse и Vector
- Команда запуска:
  
```sh
ansible-playbook -i /inventory/prod.yml /site.yml
```
