# **Инструкция по введению контроля версий Git**

![Эмблема Гит](git.png)

## что такое Git

программа Git - это программа для контроля версий

## Инициализация репозитория

чтобы инициализировать (создать) новый репозиторий, нужно ввести в терминале команду:

    git init

## Проверка состояния репозитория

чтобы проверить состояние репозитория, нужно ввести команду

    git status

## Добавление изменений в индекс

чтобы добавить изменения в индекс для следующего коммита, нужно ввести команду:

    git add <file name>

## Сохранение текущей версии

Команда

    git commit

берёт все данные, добавленные в индекс с помощью *git add*, и сохраняет их слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок.

## Обращение к журналу изменений

Обратиться к журналу изменений можно с помощью команды

    git log

## Сохранение текущей версии с описанием

Чтобы добавить описание в сохранение текущей версии, необходимо использовать команду

    git commit -m "message"

## Индексация файлов перед фиксацией

чтобы индексировать файлы перед фиксацией, минуя git add, необходимо ввести команду

    git commit -a

## Индексация файлов перед фиксацией с комментарием

Чтобы добавить комментарий к фиксации версии, минуя git add, необходимо ввести команду 

    git commit -a -m "message"

## Обращение к журналу изменений с сокращенными записями

Вывод журнала изменений с сокращенными кодами версий и выводом только комментариев, без остальной информации, осуществляет команда

    git log --oneline

## Вывод всех веток коммитов

Осуществляется командой

    git log --all

## Вывод всех веток коммитов списком с сокращенными кодами версий и комментариями к ним

    git log --oneline --all

## Разница между сохраненными файлами

Посмотреть разницу между текущим файлом и сохраненным можно с помощью команды 

    git diff

## Переключение между версиями

Переключиться между версиями программы можно с помощью команды 

    git checkout <hash>

## Ветвление

Ветки в гит нужны для параллельного редактирования проекта

### Создание новой ветки

Чтобы создать новую ветку, нужно использовать команду

    git branch <название ветки>

### Переход между ветками

Чтобы перейти на другую ветку, нужно использовать команду

    git checkout <название ветки>.

### Слияние

Чтобы влить изменение из одной ветки в другую, используется команда:

    git merge <имя ветки, которую сливаем>

обязательно находиться в ветке, в которую сливаем изменения!

#### Конфликты слияний

Если при слиянии двух версий файлов одна и та же строка напечатана по-разному, происходит конфликт слияния и необходимо выбрать версию, оставить обе или отказаться от всех изменений.

### Удаление веток

Если ветка нам больше не нужна, мы можем ее удалить. Для этого используется команда:

    git branch -d <имя ветки>

## Удаленные репозитории

Удаленные репозитории - это очень полезная штука
