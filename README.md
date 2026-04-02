#  Bash

Я рад поделиться некоторыми командами bash, которые я использовал для выполнения задач во время обучения по курсу QA manager.

## Задание 1
                                         Предварительно создайте файл bash1.txt, в который вы будете добавлять выполненные команды.
                                         Открыть домашнюю директорию через терминал
                                         Определить имя папки, в которой вы находитесь
         * mkdir test1                  # Создать внутри этой папки каталог с именем test1
         * cd test1                     # Перейти в папку test1
         * touch 1.txt 2.txt 3.txt      # Создать файл 1,2 и 3 внутри каталога test1
         * ls                           # Проверить содержимое каталога test1
         * cd ..                        # Перейти в домашнюю директорию
         * mkdir test2                  # Создать папку test2 внутри домашней директории
         * rmdir test2                  # Удалить папку test2
         * rm test1/2.txt               # Удалить файл 2 из папки test1
         * mkdir test3                  # Создать папку в домашней директории test3 и добавить в нее два файла
         * touch 1.txt 2.txt            # 
         * cd ..                        # 
         * rm -r test3                  # Удалить папку test3
         * mkdir test4                  # Создать папку test4 в домашней директории
         * mv test1/3.txt test4         # Переместить файлы 1 и 3 из папки test1 в папку test4
         * echo "line1" > test4/1.txt   # Добавить в файл 1 три строки со словами line
         * echo "line2" >> test4/1.txt  #
         * echo "line3" >> test4/1.txt  #
         * cat test4/1.txt              # Посмотреть содержимое файла 1
         * echo "line1" > test4/3.txt   # Добавьте в файл 3 три строки со словами line
         * echo "line2" >> test4/3.txt  #
         * echo "line3" >> test4/3.txt  #
         * cat test4/1.txt test4/3.txt  # Просмотрите содержимое двух файлов (1 и 3) сразу
         * nano test4/3.txt             # Используя один из редакторов замените все строки в файле 1
         
         
         
         
         
   
## Задание 2
```bash


                                               Предварительно создайте файл bash2.txt, в который вы будете добавлять выполненные команды.
                                               Зайти в домашнюю директорию через терминал.

mkdir test3                                   # Создать папку test 3 
cd test3                                      # Открыть папку test3 
echo -e "row1\nrow2\nrow3\nrow4" > file4.txt  # Добавить в папку test 3 три файла 4, 5 и 6, в каждом из которых должно быть по 4 строки row1, row2, row3, row4
echo -e "row1\nrow2\nrow3\nrow4" > file5.txt  
echo -e "row1\nrow2\nrow3\nrow4" > file6.txt 
grep "row2" file5.txt                         # Найдите строку row2 в файле 5 
grep -R "row" .                               # Найдите строку row в папке test3
grep -c "row" file6.txt                       # Посчитайте сколько строк с содержимым row в файле 6
find . -name "file5.txt"                      # Найдите файл 5 внутри папки test3
find . -name "file5.txt" -delete              # Используя команду find, удалите файл 5
echo test > file4.txt                         # Используя команду echo, добавьте слово test в файл 4
sed 's/test/fail/g' file4.txt                 # Замените слово "test" в файле 4 на "fail"
echo test >> file4.txt                        # Добавьте в файл 4 слово "test" так, чтобы сохранилось содержимое
ps aux                                        # Просмотрите все процессы для юзеров не только в консоли, которые происходят в системе
kill 666                                      # Убейте любой неважный процесс в консоли. Если боитесь удалить что-то лишнее,
                                                то можете просто прислать сам запрос без его запуска.
ping artsiomrusau.com                         # Узнайте доступность ресурса rusau.net, используя ping
ping -c 5 artsiomrusau.com                    # Отправьте 5 пакетов на сайт rusau.net  
curl https://petstore.swagger.io/v2/pet/      # Используя GET и команду curl, получите информацию о зарегистрированных питомцах с любым статусом
findByStatus?status=registered                  на https://petstore.swagger.io/              
curl -X POST https://petstore.swagger.io/     # Используя POST и команду curl, создайте нового пользователя на https://petstore.swagger.io/
v2/user --data "id=1" 
--data "username=Darrel_Volkman80" 
--data "firstName=Darrel" 
--data "lastName=Volkman" 
--data "email=Darrel_Volkman80@gmail.com" 
--data "password=g8kq2W1z_utLEBs" 
--data "phone=7442783865" 
--data "userStatus=0"
```
