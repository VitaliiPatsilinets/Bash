#  Bash

Я рад поделиться некоторыми командами bash, которые я использовал для выполнения задач во время обучения по курсу QA manager.

## Задание 1
                                 # Предварительно создайте файл bash1.txt, в который вы будете добавлять выполненные команды.
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
         
         
         
         
         
         
         #
                                   
* mkdir test1                    # Создать внутри этой папки каталог с именем test1
* cd test1                       # Перейти в папку test1
* touch 1.txt 2.txt 3.txt        #
* ls                             #
* cd ..                          #
* mkdir test2                    #
* rmdir test2                    #
* rm test1/2.txt                 #
* mkdir test3
* cd test3
* touch 1.txt 2.txt
* cd ..
* rm -r test3
* mkdir test4
* mv test1/1.txt test4
* mv test1/3.txt test4
* echo "line1" > test4/1.txt
* echo "line2" >> test4/1.txt
* echo "line3" >> test4/1.txt
* cat test4/1.txt
* echo "line1" > test4/3.txt
* echo "line2" >> test4/3.txt
* echo "line3" >> test4/3.txt
* cat test4/1.txt test4/3.txt
* nano test4/3.txt
 
```
## Task 2
##### Editing files, checking and killing proccesses, pinging websites
```bash
mkdir test3                                   # Create directory test3 
cd test3                                      # Open directory test3 
echo -e "row1\nrow2\nrow3\nrow4" > file4.txt  # Add 3 files to test3, each of which should contain 4 lines
echo -e "row1\nrow2\nrow3\nrow4" > file5.txt  
echo -e "row1\nrow2\nrow3\nrow4" > file6.txt 
grep "row2" file5.txt                         # Find the line "row2" in file5.txt 
grep -R "row" .                               # Find the line "row" in the test3 directory
grep -c "row" file6.txt                       # Count number of lines containing word "row" in file6.txt
find . -name "file5.txt"                      # Find file5.txt in test3 directory
find . -name "file5.txt" -delete              # Using find command delete file5.txt
echo test > file4.txt                         # Using the echo command, add the word "test" to file4.txt
sed 's/test/fail/g' file4.txt                 # Change the word "test" in file4.txt to "fail"
echo test >> file4.txt                        # Add the word "test" to file4.txt so that the content is preserved
ps aux                                        # View all processes in the system
kill 666                                      # Kill process 666 in console
ping artsiomrusau.com                         # Check the availability of the website artsiomrusau.com using ping
ping -c 5 artsiomrusau.com                    # Send 5 packages to artsiomrusau.com  
curl https://petstore.swagger.io/v2/pet/      # Using GET and cURL command, get info about registered pets at petstore.swagger.io
findByStatus?status=registered                
curl -X POST https://petstore.swagger.io/     # Using POST and cURL command, create a new user at petstore.swagger.io
v2/user --data "id=1" 
--data "username=Darrel_Volkman80" 
--data "firstName=Darrel" 
--data "lastName=Volkman" 
--data "email=Darrel_Volkman80@gmail.com" 
--data "password=g8kq2W1z_utLEBs" 
--data "phone=7442783865" 
--data "userStatus=0"
```
