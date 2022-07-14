# Инструкция по работе с Git

## Что такое Git

Git - это одна из реализаций распределенных систем контроля версий, что позволяет иметь версионность как в локальном репозитории, так и в удаленном репозитории (общем для всех). Git является на данный момент самой популярной системой контроля версий.

## Подготовка репозитория

Для создания репозитория используется команда *git init*. В терминале в папке с будущим репозиторием достаточно написать *git init*, и эта папка станет репозиторием.

## Создание коммитов

### Добавление файла в коммит

Для добавления файла в текущий коммит используется команда *git add*. Для этого достаточно в терминале с папкой текущего репозитория написать *git add <название файла>*. 

### Сохранение коммита

Для сохранения коммита используется команда "git commit". Для этого в терминале с папкой репозитория необходимо написать команду *git commit -m "<сообщение к коммиту>"*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***. 

## Журнал изменений

Для просмотра истории коммитов, т.е. истории наших изменений используется команда *git log*. Для этого необходимо в терминале с папкой-репозиторием написать *git log*.


## Перемещение между коммитами

Для того, чтобы перемещаться между коммитами необходимо использовать команду *git checkout*. Для этого в терминале с папкой репозитория необходимо написать *git checkout <номер коммита>*. Номер коммита берется из истории изменений. После такого "перемещения" мы попадаем в состояние *Detached head*. Для возвращения в обычное состояние используется команда *git checkout master*. 



## Ветки в Git

## Слияние веток и решение конфликтов

### Слияние веток

В случае, когда создаваемый черновик в какой-либо ветке нас полностью устраивает, мы можем все изменения из этой ветки перенести в ветку с чистовиком. Для такого слияния необходимо в терминале папки-репозитория, находясь в ветке с чистовиком, набрать команду *git merge <имя ветки для слияния с текущей>*. 

### Решение конфликтов

При работе может возникнуть ситуация, когда в сливаемых ветках окажется, что один и тот же блок текста был изменен по-разному. В этом случае Git сообщит о конфликте и предложит выбрать, какие изменения записать:
1. Accept Current Change;
2. Accept Incomming Change;
3. Accept Both Change;
4. Compare Changes.

Мы можем выбрать из этих вариантов решения конфликта или отредактировать все вручную. Всегда надо помнить, что после решения
конфликтов необходимо провести сохранение ветки с чистовиком и запись нового коммита по схеме:
 *git add <название файла>* -> *git commit -m "<сообщение коммиту>"*.  


## Удаление веток