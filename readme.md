# Инструкция по работе с Git

## Что такое Git

Git - это одна из реализаций распределенных систем контроля версий, что позволяет иметь версионность как в локальном репозитории, так и в удаленном репозитории (общем для всех). Git является на данный момент самой популярной системой контроля версий.

## Подготовка репозитория

Для создания репозитория используется команда *git init*. В терминале в папке с будущим репозиторием достаточно написать *git init*, и эта папка станет репозиторием.

## Создание коммитов

### Просмотр состояния репозитория

Для просмотра состояния репозитория используется команда *git status*. Для этого необходимо в терминале папки-репозитория написать *git status*, после чего мы можем увидеть следующие возможные состояния:
1. *Nothing to commit* - это значит, что в репозитории нет абсоютно никаких изменений;
2. *Changes not staged for commit* - это значит, что в нашем файле есть изменения, которые еще не отслеживаются, а значит необходимо провести сохранение и добавить коммит.

### Добавление файла в коммит

Для добавления файла в текущий коммит используется команда *git add*. Для этого достаточно в терминале с папкой текущего репозитория написать *git add <название файла>*. 

### Сохранение коммита

Для сохранения коммита используется команда "git commit". Для этого в терминале с папкой репозитория необходимо написать команду *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***. 

## Журнал изменений

Для просмотра истории коммитов, то есть истории наших изменений, используется команда *git log*. Для этого необходимо в терминале с папкой-реаозиторием написать *git log*.

Для визуализации истории изменений в виде дерева достаточно в терминале папки-репозитория набрать команду *git log --graph*.

## Перемещение между коммитами

Для того, чтобы перемещаться между коммитами необходимо использовать команду *git checkout*. Для этого в терминале с папкой репозитория необходимо написать *git checkout <номер коммита>*. Номер коммита берется из истории изменений. После такого "перемещения" мы попадаем в состояние *Detached head*. Для возвращения в обычное состояние используется команда *git checkout master*. 



## Ветки в Git

## Слияние веток и решение конфликтов

## Удаление веток