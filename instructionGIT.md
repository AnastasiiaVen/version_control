# Инструкция по GIT

## Что такое GIT

Это система для контроля версионности. 
[Википедия](https://ru.wikipedia.org/wiki/Git)

## Подготовка репозитория

Для инициализации репозитория необходимо выполнить команду
```sh
git init
```

## Создание и сохранение
Посмотреть статус репозитория
```sh
git status
```
Добавить измененный файл к индексации
```sh
git add filename.md
```
Зафиксировать изменения
```sh
git commit -m "Message"
```

## Перемещение между сохранениями
Переход к указанному сохранению
```sh
git checkout 'commit_number'
```
Вернуться к последнему сохранению
```sh
git checkout master
```

## Журнал изменений
Журнал изменений показывает все действия, которые мы произвели с рабочим файлом. 
Существует несколько способов выведения этого списка изменений.

Отобразить все сохраненнные изменения:
```sh
git log
```
Укороченное отображение журнала действий:
```sh
git log --oneline
```
Показать подробно, что было сделано в указанном коммите:
```sh
git show 'хеш_коммита'
```
Показать изменения в разрезе веток:
```sh
git log --oneline --graph
```
Показать изменения между коммитами:
```sh
git diff
```

## Ветки в GIT 
Просмотр всех веток:
```sh 
git branch
```
Создание новой ветки:
```sh
git branch 'namebranch'
```
Переход на нужную ветку:
```sh
git checkout 'namebranch'
```
Создание новой ветки и автоматический переход на нее:
```sh
git checkout -b 'namebranch'
```

### Слияние веток
```sh
git merge 'namebranch, которую хотим добавить'
```
... *вызываем из той ветки, в которую хотим добавить*

### Удаление веток
```sh
git branch -d 'namebranch'
```

## Заметки

Для того, чтобы очистить терминал, наберите
```sh
clear
```