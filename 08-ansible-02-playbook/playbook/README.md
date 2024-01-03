# Playbook для установки ClickHouse и Vector на VM c CentOS7

## Описание

Playbook устанавливает на managed хосты ClickHouse и Vector

## Артефакты

Источники rpm

- https://packages.clickhouse.com/rpm/stable 
- https://packages.timber.io/vector/

### Версии

- clickhouse_version: "22.3.3.44"
- vector_version: "0.33.0"

## Запуск

- Заполнить в inventory/prod.yml ip адреса хостов, на которые нобходимо установить ClickHouse и Vector
- Команда запуска:
  
```sh
ansible-playbook -i /inventory/prod.yml /site.yml
```

## Теги

- `clickhouse` - для установки Clickhouse 
- `vector` - соотвественно Vector
