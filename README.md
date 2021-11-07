# TerminalLinux
**[HW_Linux1.txt:](https://github.com/nlinky/TerminalLinux/blob/main/HW_Linux1.txt)**
==================================================================================
_Задание №1 - Linux terminal (GitBash) commands_
==================================================================================
1. Посмотреть где я - `pwd`
2. Создать папку - `mkdir Linux_commands`
3. Зайти в папку - `cd Linux_commands/`
4. Создать 3 папки - `mkdir one_papka two_papka three_papka`
5. Зайти в любоую папку - `cd one_papka/`
6. Создать 5 файлов (3 txt, 2 json) - `touch file1.txt file2.txt file3.txt file4.json file5.json`
7. Создать 3 папки - `mkdir one_one one_two one_three`
8. Вывести список содержимого папки - `ls -la`
9. + Открыть любой txt файл - `vim file1.txt`
10. + написать туда что-нибудь, любой текст - ```i + 
Унылая пора! Очей очарованье!
Приятна мне твоя прощальная краса —
Люблю я пышное природы увяданье,
В багрец и в золото одетые леса,
В их сенях ветра шум и свежее дыханье,
И мглой волнистою покрыты небеса,
И редкий солнца луч, и первые морозы,
И отдаленные седой зимы угрозы.```
11. + сохранить и выйти - `Esc + :wq`
12. Выйти из папки на уровень выше - `cd ..`
13. Переместить любые 2 файла, которые вы создали, в любую другую папку -  ```mv C:/Users/Cherv/git/course/Linux_commands/one_papka/file4.json C:/Users/Cherv/git/course/Linux_commands/one_papka/file5.json C:/Users/Cherv/git/course/Linux_commands/two_papka```
14. Cкопировать любые 2 файла, которые вы создали, в любую другую папку - ```cp C:/Users/Cherv/git/course/Linux_commands/one_papka/file2.txt C:/Users/Cherv/git/course/Linux_commands/one_papka/file3.txt C:/Users/Cherv/git/course/Linux_commands/three_papka```
15. Найти файл по имени - `find . -name file1.txt`
16. Просмотреть содержимое в реальном времени (команда grep) изучите как она работает - `grep 'лес' C:/Users/Cherv/git/course/Linux_commands/one_papka/file1.txt`
17. Вывести несколько первых строк из текстового файла - `head -2 C:/Users/Cherv/git/course/Linux_commands/one_papka/file1.txt`
18. Вывести несколько последних строк из текстового файла - `tail -2 C:/Users/Cherv/git/course/Linux_commands/one_papka/file1.txt`
19. Просмотреть содержимое длинного файла (команда less) изучите как она работает. - `less C:/Users/Cherv/git/course/Linux_commands/one_papka/file1.txt`
20. Вывести дату и время - `date`

==================================================================================
_*Задание №2 - Отправить http запрос на сервер._
==================================================================================
`curl 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000'`

```{"age":"32","family":{"children":[["Alex",24],["Kate",12]],"pets":{"cat":{"age":3,"name":"Sunny"},"dog":{"age":4,"name":"Luky"}},"u_salary_1_5_year":4000},"name":"Vadim","salary":1000}```
==================================================================================
_*Задание №3 - Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13_
==================================================================================
Файл - **[dz_Linux2.sh](https://github.com/nlinky/TerminalLinux/blob/main/HW_Linux2.sh)**
Комманда - ./dz_Linux2.sh

#!/bin/bash
cd Linux_commands/
mkdir one_papka two_papka three_papka
cd one_papka/
touch file1.txt file2.txt file3.txt file4.json file5.json
mkdir one_one one_two one_three
ls -la
mv C:/Users/Cherv/git/course/Linux_commands/one_papka/file4.json C:/Users/Cherv/git/course/Linux_commands/one_papka/file5.json C:/Users/Cherv/git/course/Linux_commands/two_papka
==================================================================================
**Задание по GIT - `[Git_HW_1.txt](https://github.com/nlinky/TerminalLinux/blob/main/Git_HW_1.txt)`**
==================================================================================
 1. Создайте текстовый файл как в первом ДЗ по Terminal.    - `Git_HW_1.txt`
 2. Сценарий перенесите в этот файл.
 3. На против каждого действия - напишите команду в GitBash
 4. Создать файл “new.json”.                                - `touch new.json`

 5. Добавить файл под гит.                                  - `git add new.json`

 6. Закоммитить файл.                                       - `git commit -m 'new.json'`

 7. Отправить файл на внешний GitHub репозиторий.           - `git push`

 8. Создать файлы new2.json, new2.xml, new2.txt             - `touch new2.json new2.xml new2.txt`

 9. Добавить файлы под гит.                                 - `git add .`

 10. Закоммитить файлы.                                     - `git commit -m '3 files'`

 11. Отправить файлы на внешний GitHub репозиторий.         - `git push`

 12. Отредактировать содержание файла “new2.txt” - написать 
информацию о себе (ФИО, возраст, количество домашних 
животных, будущая желаемая зарплата).                       - ```vim new2.txt
                                                            - нажать i
                                                            - ФИО - Червякова Надежда Александровна
                                                              возраст - 25 лет
                                                              количество домашних животных - 1
                                                              желаемая зарплата - 400 долларов
                                                            - нажать Esc
                                                            - ввести :wq```
     
 13. Отредактировать содержание файла “new2.json” - написать 
информацию о себе (ФИО, возраст, количество домашних 
животных, будущая желаемая зарплата). 
Всё написать в формате JSON. - vim new2.json                - ```vim new2.json
                                                            - нажать i
                                                            - {"FIO" : "Chervaykova Nadezhda Aleksandrovna",
                                                               "age" : 25,
                                                               "animal" : 1,
                                                               "salary" : 400}
                                                            - нажать Esc
                                                            - ввести :wq```

 14. Добавить и закоммитить “new2.txt” одной строчкой.      - `git commit new2.txt -m 'txt'`

 15. Добавить и закоммитить “new2.json” одной строчкой.     - `git commit new2.json -m 'json'`

 16. Отправить изменения на внешний репозиторий.            - `git push`

 17. Отредактировать содержание файла “new2.xml” - написать 
информацию о себе (ФИО, возраст, количество домашних 
животных, будущая желаемая зарплата). 
Всё написать в формате XML.                                 - ```vim new2.xml
                                                            - нажать i
                                                            - <info>
                                                              	<FIO>Chervaykova Nadezhda Aleksandrovna</FIO>
                                                                <age>25</age>
                                                                <animal>1</animal>
                                                                <salary>400</salary>
                                                              </info> 
                                                            - нажать Esc
                                                            - ввести :wq```

 18. Добавить и закоммитить “new2.xml” одной строчкой.      - `git commit new2.xml -m 'xml'`


 19. Отправить изменения на внешний репозиторий.            - `git push`

 20. Отправить предыдущее домашнее задание по GitBush       
Terminal на внешний репозиторий.                            - ```git add .
                                                            - git commit -m 'linux'
                                                            - git push```

 21. В веб интерфейсе GitHub создать файл new3.txt.         - ```Add file
							    - Create new file
							    - Commit new file```

 22. Отредактировать в веб интерфейсе содержание 
файла “new3.txt” - написать информацию о своих 
предпочтениях (Любимый фильм, любимый сериал, 
любимая еда, любимое время года, страна 
которую хотели бы посетить).				    - ```Нажать на new3.txt
							    - Edit this file
							    - Любимый фильм - "Гарри Поттер", 
							      любимый сериал - "Сверхъестественное", 
							      любимая еда - бутеры,
							      любимое время года - весна, 
							      страна которую хотели бы посетить - Австрия, Норвегия.```

 23. Сделать Commit changes (сохранить) изменения на 
веб интерфейсе.						    - `Commit changes`

 24. Синхронизировать внешний и локальный репозитории 
(слить изменения с внешнего репозитория).		    - `git pull`
 
 25. Отредактировать в веб интерфейсе содержание файла 
“new2.json” - добавить информацию о своих предпочтениях 
(Любимый фильм, любимый сериал, любимая еда, 
любимое время года, страна которую хотели бы посетить). 
Всё в формате JSON.					    - ```{
  								"FIO" : "Chervaykova Nadezhda Aleksandrovna",
 								"age" : 25,
  								"animal" : 1,
  								"salary" : 400,
  								"favorite movie" : "Harry Potter", 
  								"favorite TV series" : "Supernatural", 
  								"favorite food"  : "buters",
  								"favorite time of the year" : "spring", 
  								"the country you would like to visit" : ["Austria", "Norway"]
							      }```

 26. Сделать Commit changes (сохранить) изменения 
на веб интерфейсе.				            - `Commit changes`

 27. Синхронизировать внешний и локальный репозитории 	    - `git pull`

 28. Отредактировать в веб интерфейсе содержание файла 
“new2.xml” - добавить информацию о своих предпочтениях 
(Любимый фильм, любимый сериал, любимая еда, 
любимое время года, страна которую хотели бы посетить). 
Всё в формате XML.					    - ```<info>
								<FIO>Chervaykova Nadezhda Aleksandrovna</FIO>
        							<age>25</age>
        							<animal>1</animal>    
								<salary>400</salary>	
								<favorite_movie>Harry Potter</favorite_movie>
								<favorite_TV_series>Supernatural</favorite_TV_series>
								<favorite_food>buters</favorite_food>
								<favorite_time_of_the_year>spring</favorite_time_of_the_year> 
								<the_country_you_would_like_to_visit>Austria, Norway</the_country_you_would_like_to_visit>
							      </info>```

 29. Сделать Commit changes (сохранить) изменения 
на веб интерфейсе.	    			            - `Commit changes`

 30. Синхронизировать внешний и локальный репозитории.	    - `git pull`
==================================================================================
**Задание по GitHub - https://github.com/nlinky/Group_22**
==================================================================================
1. На локальном репозитории сделать ветки для:
- Postman
- Jmeter
- CheckLists
- Bag Reports
- SQL
- Charles
- Mobile testing

2. Запушить все ветки на внешний репозиторий
3. В ветке Bag Reports сделать текстовый документ со структурой баг репорта
4. Запушить структуру багрепорта на внешний репозиторий
5. Вмержить ветку Bag Reports в Main
6. Запушить main на внешний репозиторий.
7. В ветке CheckLists набросать структуру чек листа.
8. Запушить структуру на внешний репозиторий
9. На внешнем репозитории сделать Pull Request ветки CheckLists в main
10. Синхронизировать Внешнюю и Локальную ветки Main