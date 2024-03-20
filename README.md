# public-repo
Git — это система контроля версий. Именно этот инструмент поможет нам решить задачу сохранения разных версий кода для себя и переменчивых заказчиков.
Для начала нам понадобится программа Терминал. Вы можете найти его в списке приложений Finder > Программы > Утилиты > Терминал или же нажать Cmd+Space, затем ввести terminal. 
В командной строке вы тоже всегда находитесь в какой-то папке, только этого не видно. Узнать, где вы сейчас, позволяет команда pwd. Расшифровывается как Print Working Directory – покажи рабочую папку. Введите pwd в командную строку и нажмите Enter:
pwd
/Users/practicum
Командная строка вывела ответ — это путь к папке, в которой мы сейчас находимся. У вас вместо practicum будет имя вашего пользователя. Это домашняя директория — каталог с пользовательскими файлами. Когда вы открываете командную строку, вы сразу оказываетесь в ней.
В графическом интерфейсе вы просто видите содержимое открытой папки. Чтобы сделать это в командной строке, есть команда ls.
Чтобы переместиться из одной папки в другую, пользуйтесь командой cd. Это сокращение от change directory (сменить
каталог). Синтаксис у команды такой: cd имя_папки:
cd Desktop # переходим на рабочий стол
pwd
/Users/practicum/Desktop # теперь мы здесь
Команда mkdir создаёт папку. Команде нужно передать имя новой папки.
Создайте в домашней директории папку dev — она станет местом для ваших учебных проектов:
mkdir dev # создаст папку dev в текущем каталоге 
Переместитесь в папку dev, создайте в ней папку first-project и переместитесь в неё:
cd dev
mkdir first-project
cd first-project
Создадим нужные файлы. Это делают командой touch, от английского слова touch — прикоснуться, и вы будто создаёте файл прикосновением, передавая ей имя файла.
Например:
touch hello-world.txt # создаст файл hello-world.txt в текущей папке
У разработчиков и разработчиц часто бывает — создал новый файл, а потом заметил, что в названии допустил ошибку! Такой файл обязательно хочется исправить. В командной строке для такой задачи у нас есть команда mv, от английского move — двигать.
Давайте переименуем hello-world.txt в HelloWorld.txt:
mv hello-world.txt HelloWorld.txt
Файл как бы переместится со старого названия в новое HelloWorld.txt. Если на втором месте написать не новое имя, а название папки, то файл переместится в неё. Давайте создадим временную папку и переместим туда файл HelloWorld.txt:
mkdir temp
mv HelloWorld.txt temp
Для удаления файлов используют команду rm, от английского remove — удалять:
rm bad-emotions.txt # удалит bad-emotions.txt из текущей папки
Удалить папку можно командой rmdir:
rmdir images # удалит папку images из текущей папки
Мы научились создавать файлы, но не умеем в них записывать текст. Тут нам пригодится команда echo. Сама команда не записывает данные в файл, она их лишь выводит.
Для записи в файл следует использовать символ перенаправления вывода — >>. Этот символ перемещает всё, что выводиться в командную строку, внутрь файла.
Прямо сейчас, чтобы посмотреть содержимое файлов, нам приходится выходить из командной строки. Однако есть ещё одна команда, чтобы выводить содержимое файла прямо в командную строку:
cat output.txt
Итоги работы с командами командной строки:
команды перемещения и просмотра директорий: cd, pwd, ls;
управления файлами и папками: mkdir, touch, rm;
чтения и записи данных: cat, echo.
