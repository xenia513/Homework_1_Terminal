# Homework_1_Terminal

## Homework to the first Terminal lesson - Vadim Ksendzov's course


#### 1. Посмотреть, в какой папке находишься:

`$ pwd`

#### 2. Создать папку:

`$ mkdir test`

#### 3. Зайти в папку:

`$ cd test`

#### 4. Создать 3 папки одной командой:

`$ mkdir 1 2 3`
или
`$ mkdir {1,2,3}`

#### 5. Зайти в одну из созданнных папок:

`$ cd 1`

#### 6. Создать 5 файлов одной командой (3 файла в формате *txt* и 2 в формате *json*):

`$ touch 1.txt 2.txt 3.txt json1.json json2.json`

#### 7. Создать ещё 3 папки:

`$ mkdir test1 test2 test3`

#### 8. Вывести список содержимого папки:

`$ ls`

`$ ls -l # команда с этим параметром предоставит список содержимого текущей директории с разрешением, количеством индексных дескрипторов, указанием владельца и группы, размера файла, даты последнего доступа и времени и имени файла`

`$ ls -la  # параметр 'a' позволит отобразить скрыте файлы и папки`

#### 9. Открыть созданный файл:

`$ vim 1.txt`

#### 10. Отредактировать файл, добавить текст:

`i`

#### 11. Сохранить файл и завершить редактирование:

`esc`
`:wq`

#### 12. Переместиться в папку на уровень выше: 

`$ cd ..`

#### 13. Переместить 2 созданных файла в другую папку:

`$ mv {1/1.txt,1/2.txt} 2`

#### 14. Скопировать 2 созданных файла в другую папку:

`$ cp {1/1.txt,1/2.txt} 2`

#### 15. Найти файл по имени:

`$ find . -f -name 1.txt`

#### 16. Посмотреть содержимое файла в реальном времени:

`$ tail -F 1.txt`

#### 17. Вывести несколько первых строк текстового файла:

`$ head -n 3 1.txt`
или
`$ head -3 1.txt`

#### 18. Вывести несколько последних строк текстового файла:

`$ tail -n 3 1.txt`
или
`$ tail -3 1.txt`

#### 19. Посмотреть содержимое длинного файла:

`$ less 1.txt`

Чтобы увидеть построчную нумерацию в файле нужно воспользоваться командой с параметром *-N*:

`$ less -N 1.txt`

#### 20. Вывести текущие дату и время:

`$ date`

### Задание со звёздочкой *

#### 1. Отправить запрос на сервер:

`curl http://162.55.220.72:5005/terminal-hw-request`

или можно воспользоваться командой lwp-request, которая по умолчанию отправляет на сервер GET-запрос:

`lwp-request http://162.55.220.72:5005/terminal-hw-request`

#### 2. Скрипт, который автоматически выполняет п.3, 4, 5, 6, 7, 8, 13 текущего задания:

`#!/bin/bash`
`/c/Users/User/desktop`

`cd homework_1 # Зайти в папку`

`mkdir test1 test2 test3 # Создать 3 папки`

`cd test1 # Зайти в любую папку`

`touch tst1.txt tst2.txt tst3.txt json1.json json2.json # Создать 5 файлов `

`mkdir test_1 test_2 test_3 # Создать 3 папки`

`ls -la # вывести список содержимого папки`

`mv {tst1.txt,tst2.txt} test_2 # переместить 2 файла в другую папку`
