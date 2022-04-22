---
## Front matter
title: "Лабораторная работа №4"
subtitle: "Отчет по лабораторной работе 4"
author: "Репина Ангелина Олеговна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

 
# Цель работы

Цель данной лабораторной работы -- Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

1. Сделать отчет по лабораторной работе №4 в формате Markdown
2. Приобрести практические навыки взаимодействия пользователя с системой

# Выполнение лабораторной работы

1. Определила полное имя домашнего каталога  с помощью команды pwd

![Определение имени домашнего каталога](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на дом каталог.png){ #fig:001 width=70% }

2.
2.1 Перешла в катлог tmp (cd /tmp)

![TMP](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на tmp.png){ #fig:001 width=70% }

2.2 . Вывела на экран содержимое каталога /tmp. Для этого использовала команду ls
с различными опциями. 

![Содержимое](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на ls.png) { #fig:001 width=70% }

1) "ls" используется для просмотра содержимого каталога. 
2) Для того, чтобы отобразить имена скрытых файлов, необходимо использовать команду ls
с опцией a: " ls -a "
3) "ls -F" - Можно также получить информацию о типах файлов (каталог, исполняемый файл,
ссылка), для чего используется опция F. При использовании этой опции в поле имени
выводится символ, который определяет тип файла
Символ, который определяет тип файла
Каталог - символ "/"
Исполняемый файл - "*"
Ссылка - "@"
4) "ls -l" Чтобы вывести на экран подробную информацию о файлах и каталогах, необходимо
использовать опцию l. При этом о каждом файле и каталоге будет выведена следующая
информация:
– тип файла,
– право доступа,
– число ссылок,
– владелец,
– размер,
– дата последней ревизии,
– имя файла или каталога.

2.3 Определила, есть ли в каталоге /var/spool подкаталог с именем cron. Чтобы это определить необходимо перейти в указанный каталог с помощью команды cd/var/spool. Теперь нужно посмотреть его содержимое командой ls. Видим, что такой каталог действительно существует в /var/spool.

![cron](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на cron.png){ #fig:001 width=70% }

2.4 Перешла в домашний каталог и вывела на экран его содержимое. Определила, кто является владельцем файлов и подкаталогов. Владельцем файлов и подкаталогов является aorepina studsci.

![owner](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на owner.png){ #fig:001 width=70% }

3.
3.1 В домашнем каталоге создала новый каталог с именем newdir командой mkdir.

![newdir](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на newdir.png){ #fig:001 width=70% }

3.2 В каталоге ~/newdir создаю новый каталог с именем morefun командой mkdir.

![morefun](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на morefun.png){ #fig:001 width=70% }

3.3 В домашнем каталоге создала одной командой три новых каталога с именами
letters, memos, misk (mkdir letters memos misk). Затем удалила эти каталоги одной командой (rm -r letters memos misk).

![lmm](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на lmm.png){ #fig:001 width=70% }

3.4 Попробовала удалить ранее созданный каталог ~/newdir командой rm. Проверила,
был ли каталог удалён. Видим, что каталог удалить этой командой невозможно.

![rmnewdir](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на rmnewdir.png){ #fig:001 width=70% }

3.5 Удалила каталог ~/newdir/morefun из домашнего каталога. Проверила, был ли
каталог удалён.

![rm](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на rm.png){ #fig:001 width=70% }

4. С помощью команды man определила, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него. (man ls)

![manls](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на lsls.png){ #fig:001 width=70% }

5. С помощью команды man определила набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов. (history команда)

![history](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на history.png){ #fig:001 width=70% }

6. Использовала команду man для просмотра описания следующих команд: cd, pwd, mkdir,
rmdir, rm.  

![cd](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на cd.png){ #fig:001 width=70% }
![pwd](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на pwd.png) { #fig:001 width=70% }
![mkdir](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на mkdir.png){ #fig:001 width=70% }
![rmdir](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на rmdir.png){ #fig:001 width=70% }
![rm](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Другая ссылка на rm.png){ #fig:001 width=70% }

1) Команда cd используется для перемещения по файловой системе операционной системы типа Linux.
2)  Для определения абсолютного пути к текущему каталогу используется
команда pwd (print working directory).
3)Команда mkdir используется для создания каталогов.
4) Команда rm используется для удаления файлов и/или каталогов.

7. Используя информацию, полученную при помощи команды history, выполнила модификацию и исполнение нескольких команд из буфера команд. (командой !+номер строки из истории, полученной с помощью команды history)

![!](/afs/.dk.sci.pfu.edu.ru/home/a/o/aorepina/Документы/ЛР4/Ссылка на 7.png){ #fig:001 width=70% }
# Выводы

Вывод: приобрела навыки взаимодействия пользователя с системой посредством командной строки в ходе лабораторной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::