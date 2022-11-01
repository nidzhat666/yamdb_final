![Yamdb Workflow Status](https://github.com/nidzhat666/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg?branch=master&event=push)

###### http://nzmaslo.ru:3000

ApiYamdb
===

---

## Инструкция по разворачиванию локального сервера

## Установка

#### 1. Установка docker и docker-compose

Если у вас уже установлены docker и docker-compose, этот шаг можно пропустить, иначе можно воспользоваться официальной [инструкцией](https://docs.docker.com/engine/install/).

#### 2. Запуск контейнера
```bash
docker-compose up
```
### 3. Выключение контейнера
```bash
docker-compose down
```


## Использование
#### Создание суперпользователя Django
```bash
docker-compose run web python manage.py createsuperuser
```

#### Пример инициализации стартовых данных:
```bash
docker-compose run web python manage.py loaddata fixtures.json
```


#### Работа с api
Документация ко всем ручкам описана в redoc


#### Переменные окружения
Для дефолтного набора переменных в энвике нужно скопировать .env.template и переименовать в .env




## Developer
#### Nidzhat Agalarov - Python Backend Developer
