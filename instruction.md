## Инструкция для работы с GIT

## Начальные настройки и установки

*git config --global user.name «Ваше имя английскими буквами» например: Konstantin*

*git config --global user.email ваша почта@example.com*

*git init* – **инициализация локального репозитория**

*git status* – **получить информацию от git о его текущем состоянии**

*git add* – **добавить файл или файлы к следующему коммиту**

*git commit -m “message”* – **создание коммита**.

*git log* – **вывод на экран истории всех коммитов с их хеш-кодами**

*git checkout* – **переход от одного коммита к другому**

*git checkout* master – **вернуться к актуальному состоянию и продолжить работу**

*git diff* – **увидеть разницу между текущим файлом и закоммиченным файлом**

## Работа с ветками

*git branch* – **посмотреть список веток в репозитории**

*git branch <название ветки>* – **создать новую ветку**

*git checkout <название ветки>* – **переход к другой ветке**

*git checkout -b <название ветки>* – **переход к новой созданной ветке**

*git branch -d <название ветки>* – **удалить ветку**

*git merge <branch_name>* - **слияние веток**

## Цитата

*Дочерние ветки создаются из ветки master. Дочерние ветки никогда не сздаются из других дочерних веток* - **ОБЯЗАТЕЛЬНО ЗАПОМНИТЬ**

## Клонирование репозитория

*$ git clone https://github.com/UserName/UpRemote.git* - **Клонирование удаленного репозитория в локальный каталог с именем по умолчанию**

*$ git clone https://github.com/UserName/UpRemote.git LocalBranches* - **Клонирование удаленного репозитория в правильном каталоге с описанием имени**
*git status* - **Постоянно запускать git status - хорошая привычка**

*Сохранять актуальную версию програмного кода у себя*

*Использование стрелок в терминале вместо ввода руками всех комманд - удобно и быстро =DD*

*Полезное наименование, чтоб быстрее можно было разобраться*

*Не забывайте сохранять файл после внесения измененний*

*git mergetool* - **вызывает внешнюю программу слияний, в случае если у вас возникли проблемы слияния**

*git stash* - **используется для временного сохранения всех незакоммиченных изменений для очистки рабочей директории без необходимости коммитить незавершённую работу в новую ветку**

*git tag* - **используется для задания постоянной метки на какой-либо момент в истории проекта, обычно она используется для релизов**

## Работа с удаленным репозиторием

*git clone* – **клонирование удаленного репозитория на локальный компьютер**

*git push* – **выгрузить изменения удаленный репозиторий**

*git pull* - **стянуть изменения из удаленного репозитория**

## Шпаргалка по отладке

В Git есть несколько команд, используемых для нахождения проблем в коде. Это команды для поиска места в истории, где проблема впервые проявилась и собственно виновника этой проблемы.

*git bisect* - **Команда git bisect — это чрезвычайно полезная утилита для поиска коммита в котором впервые проявился баг или проблема с помощью автоматического бинарного поиска.**

*git blame* - **Команда git blame выводит перед каждой строкой файла SHA-1 коммита, последний раз менявшего эту строку и автора этого коммита. Это помогает в поисках человека, которому нужно задавать вопросы о проблемном куске кода.**

*git grep* - **Команда git grep используется для поиска любой строки или регулярного выражения в любом из файлов вашего проекта, даже в более ранних его версиях.**