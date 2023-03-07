# Terminal #

![](https://help.apple.com/assets/61E89D604694F96BA04E7D79/61E89D614694F96BA04E7D80/tr_TR/d94aa1c4979b25e9ffbda97fcbae219a.png)

## HW_terminal_1 ##

###### Первая часть первого  ДЗ. Linux terminal (GitBash) commands ######

1) Посмотреть где я: 
```bash
КОМАНДА pwd 
```
2) Создать папку:
```bash
КОМАНДА mkdir название папки
```
3) Зайти в папку: 
```bash
КОМАНДА cd название папки
```
4) Создать 3 папки:
```bash
КОМАНДА mkdir название папки название папки название папки
```
5) Зайти в любоую папку:
```bash
КОМАНДА cd название папки
```
6) Создать 5 файлов (3 txt, 2 json):
```bash
КОМАНДА touch название файла.расширение - просто создать файл
cat >> название файла.расширение - создать файл и сразу войти в режим его редактирования 
Enter, затем ctrl+C - выход из режима редактирования
```
7) Создать 3 папки:
```bash
КОМАНДА mkdir название папки название папки название папки
```
8) Вывести список содержимого папки:
```bash
КОМАНДА ls - посмотреть содержимое папки
```
9) Открыть любой txt файл:
```bash
vim название файла.расширение - это редактор файла в терминале
или cat >> название файла.расширение 
```
10) Написать туда что-нибудь, любой текст:
```bash
Чтобы начать редактировать в vim - команда I, перемещение курсора с помощью стрелок на клавиатуре
```
11) Сохранить и выйти:
```bash
Чтобы выйти из vim - esc, затем : , затем wq и enter
```
12) Выйти из папки на уровень выше:
```bash
КОМАНДА cd .. - переход на предыдущую родительскую папку
```
13) Переместить любые 2 файла, которые вы создали, в любую другую папку:
```bash
КОМАНДА mv fail1.txt ../2/fail1.txt - переместить такой-то файл в такую-то папку (и в конце еще раз указать этот файл)
```
14) Скопировать любые 2 файла, которые вы создали, в любую другую папку:
```bash
КОМАНДА cp fail1.txt ../2/f1.txt - скопировать файл в такую-то папку и назвать новый файл так-то
КОМАНДА - mv f1.txt d1.txt - переименовать (старое название файла и новое название файла)
КОМАНДА cp fail1.txt fail2.txt - скопировать содержимое одного файла в дрогой файл
КОМАНДА cat d1.txt > fail1.txt -заместить во втором указанном файле информацией из первого
```
15) Найти файл по имени:
```bash
КОМАНДА find  . -name "название файла"
```
16) Просмотреть содержимое в реальном времени:
```bash
КОМАНДА tail -f название файла (показывает последние 10 строк) или less +f название файла
```
17) Вывести несколько первых строк из текстового файла:
```bash
КОМАНДА head -(количество строк) название файла
```
18) Вывести несколько последних строк из текстового файла: 
```bash
КОМАНДА tail -n(количество строк) -f название файла
```
19) Просмотреть содержимое длинного файла:
```bash
КОМАНДА less название файла
```
20) Вывести дату и время:
```bash
КОМАНДА dat
```
21) Готово!

## HW_terminal_2 ##

1. Создать папку dir_1:
```bash
mkdir dir_1
```
 2. Зайти в папку dir_1:
 ```bash
 cd dir_1
 ```
 3. Создать папку inner_dir_1:
 ```bash
 mkdir inner_dir_1
 ```
 4. Посмотреть, где ты находишься: 
 ```bash
pwd  - /Users/aleksandrasoloshenko/terminal_1/dir_1
```
 5. Находясь в папке dir_1, создать пустой текстовый файл tf_1.txt:
 ```bash
dir_1 % touch tf_1.txt
```
 6. Находясь в папке dir_1, через команду cat создать текстовый файл tf_2.txt со следующими строками:
- the first 1
- the second 2
- the third 3
```bash
cat >> tf_2.txt
the first 1
the second 2
the third 3
```
 7. Зайти в папку inner_dir_1:
 ```bash
cd inner_dir_1
```
 8. Через cat сделать текстовый файл tf_3.txt  c любыми строками:
 ```bash
 inner_dir_1 % cat >> tf_3.txt
line 1
line 2
line 3
line 4
line_5
```
 9. Через cat добавить в текстовый файл tf_3.txt строку “the second 2”
 10. Через cat добавить в текстовый файл tf_3.txt строку “the sec 2”
 ```bash
inner_dir_1 % cat >> tf_3.txt
the second 2
the sec 2
```
 11.  Через cat добавить в текстовый файл tf_3.txt строку “the SeCoNd 2”
 ```bash
inner_dir_1 % cat >> tf_3.txt
the SeCoNd 2
```
 12. Через cat добавить в текстовый файл tf_2.txt строку “the sec 3”
 13. Через cat добавить в текстовый файл tf_2.txt строку “the seConD 2”
 ```bash
 inner_dir_1 % cat >> tf_2.txt
the sec 3
the seConD 2
```
 14. Сделать текстовый файл tf_4.txt в котором будет 15 строк:
 ```bash
 inner_dir_1 % cat >> tf_4.txt
 ```
 15. Сделать текстовый файл tF_5.txt в котором будет 13 строк:
 ```bash
 inner_dir_1 % cat >> tF_5.txt
 ```
 16. Вывести список всех файлов в папке:
 ```bash
 inner_dir_1 % ls
tF_5.txt	tf_2.txt	tf_3.txt	tf_4.txt
```
 17. Выйти из папки inner_dir_1:
 ```bash
inner_dir_1 % cd ..
```
 18. Вывести содержимое файла tf_3.txt в терминал:
 ```bash
 dir_1 % cat inner_dir_1/tf_3.txt
 ```
 19. Найти путь к файлу tf_4.txt:
 ```bash
 terminal_1 % find . -name "tf_4.txt"
Путь - ./dir_1/inner_dir_1/tf_4.txt
```
 20. Очистить файл tf_4.txt от содержимого без удаления самого файла:
 ```bash
terminal_1 % echo > ./dir_1/inner_dir_1/tf_4.txt
```
 21. Найти путь к файлам, у которых есть  “tf” в названии:
 ```bash
terminal_1 % find . -name "*tf*"

Результат:
./dir_1/tf_1.txt
./dir_1/tf_2.txt
./dir_1/inner_dir_1/tf_3.txt
./dir_1/inner_dir_1/tf_2.txt
./dir_1/inner_dir_1/tf_4.txt
```
 22. Найти путь к файлам, у которых есть  “tf” в названии и буквы в любом регистре:
 ```bash
 terminal_1 % find . -iname "*tf*"
 
Результат:
./dir_1/tf_1.txt
./dir_1/tf_2.txt
./dir_1/inner_dir_1/tf_3.txt
./dir_1/inner_dir_1/tf_2.txt
./dir_1/inner_dir_1/tF_5.txt
./dir_1/inner_dir_1/tf_4.txt
```
 23. Найти строки в файлах, где есть комбинация букв “sec” в текущей папке:
```bash
dir_1 % grep -r sec .

Результат:
./tf_2.txt:the second 2
./tf_2.txt:the sec 3
./inner_dir_1/tf_3.txt:the second 2
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_2.txt:the second 2
./inner_dir_1/tf_2.txt:the sec 3
```
 24. Найти строки в файлах, где есть комбинация букв “sec” в любом регистре в текущей папке:
```bash
dir_1 % grep -r -i sec .

Результат:
./tf_2.txt:the second 2
./tf_2.txt:the sec 3
./tf_2.txt:the seConD 2
./inner_dir_1/tf_3.txt:the second 2
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_3.txt:the SeCoNd 2
./inner_dir_1/tf_2.txt:the second 2
./inner_dir_1/tf_2.txt:the sec 3
./inner_dir_1/tf_2.txt:the seConD 2
```
 25. Найти строки в файлах, где есть только комбинация букв “sec” в текущей папке:
```bash
 dir_1 % grep -r -w sec .
 
Результат:
./tf_2.txt:the sec 3
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_2.txt:the sec 3
```
 26. Найти строки в файлах, где есть только комбинация букв “sec” в любом регистре в текущей папке:
```bash
 dir_1 % grep -r -w -i sec .
 
Результат:
./tf_2.txt:the sec 3
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_2.txt:the sec 3
```
27. Найти строки в файлах, где есть комбинация букв “second” в текущей папке:
```bash
dir_1 % grep -r second .   

Результат:
./tf_2.txt:the second 2
./inner_dir_1/tf_3.txt:the second 2
./inner_dir_1/tf_2.txt:the second 2
```
 28. Найти строки в файлах, где есть комбинация букв “second” в любом регистре в текущей папке:
```bash
dir_1 % grep -r -i second .

Результат:
./tf_2.txt:the second 2
./tf_2.txt:the seConD 2
./inner_dir_1/tf_3.txt:the second 2
./inner_dir_1/tf_3.txt:the SeCoNd 2
./inner_dir_1/tf_2.txt:the second 2
./inner_dir_1/tf_2.txt:the seConD 2
```
 29. Найти строки в файлах, где есть комбинация букв “second” во всех папках ниже уровнем
 
 30. Найти только путь и название файла в строках, в которых есть комбинация букв “second” в текущей папке:
 ```bash
 dir_1 % grep -r -l second .  
 
Результат:
./tf_2.txt
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_2.txt
```
 31. Найти все строки во всех файлах, где нет комбинации “second”:
```bash
 dir_1 % grep -r -v second .
 
Результат:
Binary file ./.DS_Store matches
./tf_2.txt:the first 1
./tf_2.txt:the third 3
./tf_2.txt:the sec 3
./tf_2.txt:the seConD 2
./inner_dir_1/tf_3.txt:line 1
./inner_dir_1/tf_3.txt:line 2
./inner_dir_1/tf_3.txt:line 3
./inner_dir_1/tf_3.txt:line 4
./inner_dir_1/tf_3.txt:line_5
./inner_dir_1/tf_3.txt:the sec 2
./inner_dir_1/tf_3.txt:the SeCoNd 2
./inner_dir_1/tf_2.txt:the first 1
./inner_dir_1/tf_2.txt:the third 3
./inner_dir_1/tf_2.txt:the sec 3
./inner_dir_1/tf_2.txt:the seConD 2
./inner_dir_1/tF_5.txt:line_1
./inner_dir_1/tF_5.txt:line_2
./inner_dir_1/tF_5.txt:line_3
./inner_dir_1/tF_5.txt:line_4
./inner_dir_1/tF_5.txt:line_5
./inner_dir_1/tF_5.txt:line_6
./inner_dir_1/tF_5.txt:line_7
./inner_dir_1/tF_5.txt:line_8
./inner_dir_1/tF_5.txt:line_9
./inner_dir_1/tF_5.txt:line_10
./inner_dir_1/tF_5.txt:line_11
./inner_dir_1/tF_5.txt:line_12
./inner_dir_1/tF_5.txt:line_13
./inner_dir_1/tF_5.txt:line_14
./inner_dir_1/tF_5.txt:lane_15
./inner_dir_1/tf_4.txt:
```
 32. Найти только название и путь к файлам, где нет комбинации “second”:
```bash
dir_1 % grep -r -v -l second .

Результат:
./.DS_Store
./tf_2.txt
./inner_dir_1/tf_3.txt
./inner_dir_1/tf_2.txt
./inner_dir_1/tF_5.txt
./inner_dir_1/tf_4.txt
```
 33. Вывести в терминал 4 последних строки любого текстового файла:
```bash
tail -n4 -f tF_5.txt

Результат:
line_12
line_13
line_14
lane_15
```
 34. Вывести в терминал 4 первые строки любого текстового файла:
```bash
head -4 tF_5.txt

Результат:
line_1
line_2
line_3
line_4
```
 35. Команда в одну строку. Создать папку и создать текстовый файл с содержимым:
```bash
 mkdir название папки | echo содержимое > название файла
```
