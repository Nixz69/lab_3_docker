### Лабаратораня работа 3 

## Задача 1
---
Выполение первого задания связанного с докером создание 2х файлов
![alt text](2файла.png)
```html

- Создайте Dockerfile и реализуйте в нем замену дефолтной индекс-страницы(/usr/share/nginx/html/index.html), на файл index.html с содержимым:

<html>
    <head>
        Hey, ZGU!
</head>
<body>
    <p>I will be IT Engineer!</p>
</body>
</html>

```
![alt text](докер.png)

-Ссылка на DockerHub
https://hub.docker.com/repository/docker/nixz69/custom-nginx/general

## Задача 2
- Запустите ваш образ custom-nginx:1.0.0 командой docker run в соответвии с требованиями:
![alt text](имя.png)
- Далее требовалось перименовать custom-nginx

![alt text](переименовал.png)

- Убедитесь с помощью curl или веб браузера, что индекс-страница доступна.

![alt text](ПРУФ2.png)


## Задача 3

 Выполните ```docker ps -a``` и объясните своими словами почему контейнер остановился.

 - Контейнер остановился, потому что сигнал Ctrl-C отправил команду прерывание главному процессу контейнера

Уставил текстовый редакто Nano

![alt text](nano.png)

Сделал reload и прописал ```curl http://127.0.0.1:8080```
Благодаря Nano были изменены версии порты на 81
![alt text](ПРУФ3.png)

## Задача 4

- Запустите первый контейнер из образа ***centos*** c любым тегом в фоновом режиме, подключив папку  текущий рабочий каталог ```$(pwd)``` на хостовой машине в ```/data``` контейнера, используя ключ -v.

- Запустите второй контейнер из образа ***debian*** в фоновом режиме, подключив текущий рабочий каталог ```$(pwd)``` в ```/data``` контейнера. 

![alt text](контейнеры.png)

- Добавьте ещё один файл в текущий каталог ```$(pwd)``` на хостовой машине.
![alt text](4хост.png)

Добавил все необозодимые файлы что были по заданию
![alt text](конец4.png)


## Задача 5
    Создал файлы как просиловсь в задании compose.yaml и docker-compose.yaml.

![alt text](пруф5.png)

    Также было задание где надо было отредактировать файл, успешно был выполнен

![alt text](пруф.png)

    Также произвел запуск обоих контейнеров
![alt text](зап2.png)

    Пруф авторизации
![alt text](port.png)

 - Откройте страницу "http://127.0.0.1:9000/#!/home", выберите ваше local  окружение. Перейдите на вкладку "stacks" и в "web editor" задеплойте следующий компоуз:

![alt text](код.png)

    Далее на сайте 

![alt text](5здание.png)

Также по заданию нужно было удалить compose.yaml и решить конфликт
![alt text](удаление.png)

И скрин исправления ошибки - ошибка была связанна с тем что при удалении compose.yaml в docker-compose.yaml вызывалсь старая версии нужно было удалить строчку version: "3"

![alt text](ошибка.png)

Послдений скрин
![alt text](финал.png)
