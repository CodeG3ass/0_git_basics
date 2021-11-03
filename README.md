##  Работа с Git в терминале


### Цель работы

На основе уже полученных знаний о принципах работы СКВ получить более глубокое представление о работе Git  при помощи команд терминала.


### Задания для выполнения



1. Выберите тематику программы, которую собираетесь написать. Создайте для нее рабочую директорию
2. Инициализируйте в рабочей директории репозиторий при помощи команды git init.
3. Выполните в репозитории команду git status. Проинтерпретируйте полученное сообщение.
4. Создайте файл для исходного текста программы. Выполните команду git status.
5. Добавьте созданный файл под версионный контроль при помощи команды git add. Еще раз выполните git status.
6. Сделайте начальный коммит при помощи команды git commit с опцией -m.
7. Сделайте еще несколько коммитов. Выполните команду git log для просмотра истории коммитов.
8. Сделайте так, чтобы при коммите измененные файлы автоматически добавлялись в коммит.
9. Добавьте еще несколько файлов с исходным текстом программы. 
10.  Добавьте все новые файлы под версионный контроль одной командой. 
11. На всех стадиях работы пользуйтесь командой git status.
12. Инициализируйте в рабочей директории виртуальное окружение (Если вы пишите не на Python, то можете инициализировать какой-либо программный фреймворк, либо начать работать в IDE, которая создает скрытую папку с настройками в рабочем каталоге).
13. Добавьте созданную служебную папку в файл .gitignore. Проверьте, что они не добавляются в репозитории при добавлении новых файлов с исходным кодом. 
14. Создайте новую тематическую ветку git branch. Перейдите в нее с помощью git checkout. Выведите на экран список всех веток.
15. Сделайте несколько коммитов в основную и тематическую ветки. 
16. Слейте изменения в основную ветку с помощью git merge. Если произошел конфликт слияния, разрешите его и завершите слияние с помощью git commit.
17. При получении в процессе разработки программы в стабильно работающем состоянии, слейте это состояние в основную ветку и добавьте к коммиту слияния пометку с номером релиза.


### Методические указания

Для работы в терминале изучите шпаргалки по основным командам git.

Главные команды, которые вам понадобятся это:

git init - создает репозиторий системы контроля версий в данной директории;

git add - добавляет указанный файл под версионный контроль;

git add . - добавляет все файлы текущей директории под версионный контроль;

git status - показывает состояние рабочей директории по сравнению с последним сохраненным состоянием:

git commit -m "(message)" - сохраняет текущее состояние рабочей директории как новое состояние (создает новый коммит); новый коммит получает сообщение, переданное как параметр;

git commit -am "(message)" - создает новый коммит и автоматически включает в него все изменившиеся отслеживаемые файлы;

git log - выводит историю коммитов репозитория;

git branch - показывает список веток репозитория;

git branch <branchname> - создает новую ветку на основе текущего состояния с переданным названием;

git checkout -b <branchname> - создает новую ветку и автоматически делает ее текущей;

git merge <branchname> - сливает изменения, сделанные в ветке с переданным названием в текущую;

git branch -d <branchname> - удаляет ветку с переданным названием;

git clone (repo URL) - клонирует удаленный репозиторий, находящийся по переданному адресу в текущую директорию; доступ обычно осуществляется по протоколам HTTP либо SSH;

git fetch - считывает изменения в удаленном репозитории, отсутствующие в локальной копии;

git pull - считывает новые изменения в удаленном репозитории и сливает их в соответствующие локальные ветки;

git push –all - отправляет изменения, сделанные в локальном репозитории в удаленный;


### Контрольные вопросы



1. Что такое удаленный репозиторий?
2. Где нужно вводить команды git?
3. Для чего нужны ветки в системах контроля веток?
4. Как возникают конфликты слияни
5. Как разрешать конфликты слияния?


### Дополнительные задания



1. Ознакомьтесь с методологией разработки GitFlow.
2. Установите на свой компьютер инструментальное средство для работы с GitFlow.
3. Выполните основные задания лабораторной работы с использованием команд git-flow.


## 3. Работа с удаленными репозиториями и GitHub


### Цель работы

Освоить основные навыки работы с облачными и распределенными системами контроля версий, получить навыки работы с инструментальными средствами, обеспечивающими командную работу над разработкой ПО.


### Задания для выполнения



1. Зарегистрироваться на сайте github.com
2. Установить на компьютере программу Git
3. Форкнуть данный репозиторий в свой аккаунт
4. Склонировать созданный удаленный репозиторий в директорию ~/git/test
5. На локальной машине пишем скрипт ~/git/test/backup.sh, с произвольным содержанием
6. Фиксируем скрипт в репозитории (делаем коммит)
7. Обновляем удаленный репозиторий репозиторий (делаем пуш)
8. Через текстовый редактор добавить любую новую строку с комментарием
9. Сделать коммит
10. Вности синтаксическую ошибку в скрипт
11. Сделать коммит ошибочного скрипта
12. Откатываем до последней рабочей версии
13. Просмотреть историю коммитов
15. Добавить несколько коммитов произвольного содержимого
16. Создать пулл реквест в данный репозиторий


### Контрольные вопросы



1. Зачем нужен облачный хостинг репозиториев?
2. Какими основными функциями обладает сайт github.com?
3. Как организовать командную работу над открытым проектом?


### Дополнительные задания



1. Дополнительно оценивается, если студент продемонстрирует работу с ветками в процессе написания более-сложного программного проекта (не менее трех файлов, двух веток, десяти коммитов, как минимум одно объединение).
2. Дополнительно оценивается демонстрация командной работы. Для этого нужно склонировать репозиторий другому члену команды и коммитить от своего имени. При отправке истории на удаленный сервер (push) на сайте будет отображаться общая история. При скачивании истории с сервера (pull) общая история будет отображаться на локальном компьютере.
3. Настройте работу с git вашей интегрированной среды разработки по выбору. Для работы с python рекомендуется использовать PyCharm. Выполните задания лабораторной работы в IDE используя встроенные средства работы с системами контроля версий.

<!-- Docs to Markdown version 1.0β17 -->
