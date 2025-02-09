# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
Git - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

## Создание коммитов

### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*

### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

## Ветки в Git

### Создание ветки

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

## Удаление веток
Для удаления ветки ввести команду "git branch -d 'name branch'"
# Работа с удалёнными репозиториями
**Инструкция по работе с удалёнными репозиториями включает следующие шаги:**
## 1. Подключение к удалённому репозиторию
* Для этого используется команда* **git remote add.** *К ней нужно добавить два параметра: имя удалённого репозитория и его адрес. Адрес можно найти на странице профиля во вкладке SSH.* 
## 2.	Просмотр удалённых репозиториев
*Для этого используется команда **git remote.** Можно посмотреть название связанных репозиториев и отсортировать все ненужные.*
## 3.	Отправка изменений в удалённый репозиторий. 
*Для этого используется команда* **git push.** *Во время первой загрузки нужно использовать команду с опцией* **-u.** *Это свяжет локальную и удалённую ветки и синхронизирует их для последующих операций. Для второй и всех последующих загрузок опция* **-u** *для связанных веток не понадобится*
## 4. Получение изменений из удалённого репозитория. 
*Для этого используется команда* **git pull.** *Она соединяется с удалённым репозиторием и запрашивает изменения. Если изменения присутствуют, Git скачает их.*