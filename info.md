# Инструкция по работе с git

![](pic.jpg)

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

## Отслеживание состояние репозитория
> git status

показывает изменненые файлы и файлы готовые для комита
> git log

для визуализации веток добавляйте тег 
> git log --graph

показывает все комиты
> git diff

показывает разницу между текущей версией и зафиксированной

## Переход между коммитами
> git checkout commit_code

Переходит к комиту с кодом commit_code(его можно подсмотреть по git log)

> git checkout master

Вернуться к актуальному состоянию

## Ветки в git
Чтобы посмотреть все ветки:
> git branch

Для создания ветки branch_name:
> git branch branch_name

Переместиться к ветке branch_name:
> git checkout branch_name

## Удаление веток

Удалить ветку с именем branch_name можно командой:
> git branch -d branch_name

Для удаления ветки игнорируя все ошибки:
> git branch -D branch_name

## Слияние веток и решение конфликтов

Команда для выкачивания информации из ветки branch_name в текущую ветку:
> git merge branch_name

**Для того чтобы решить мердж конфлик, нужно убрать лишние строки и отредактировать текст**

## Справка
Чтобы вызвать справку для какой-то команды, нужно добавить тег:
> --help

Примеры:
>git add --help

>git commit --help

>git branch --help