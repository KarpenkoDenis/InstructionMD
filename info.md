# Инструкция по работе с git

## Начало работы с репозиторием
 > git init

 * создает локальный репозиторий

 Если не было здано имя пользователя ранее, то:
> git config --global user.name "name"

> git config --global user.email "mail@mail.com"

## Добавление файлов в репозиторий
> git add file_name

Добавляет файл file_name для отслеживания

> git commit -m "some message"

Фиксирует все файлы, которые были добавлены для отслеживания