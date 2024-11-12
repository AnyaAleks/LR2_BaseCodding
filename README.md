# Лабораторная работа №2. Система контроля версий
## Цель лабораторной работы
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и удаленным репозиторием. 
## Модель решения

1. Копирование в личное хранилище из https://github.com/Kurtyanik/LR6/ с помощью Fork.

Переход в репозиторий преподавателя (рис. 1).
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture1.png">
</p>
<p align="center">Рисунок 1 – Переход в репозиторий</p> </br>

Создание нового fork с названием LR2_BasicCodding (рис. 2).
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture2.png">
</p>
<p align="center">Рисунок 2 – Создание fork</p> </br>

Демонстрация созданного репозитория представлена на рисунке 3.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture3.png">
</p>
<p align="center">Рисунок 3 – Созданный репозиторий</p> </br>


2. Настройка клиента git с вводом имени пользователя (Группа Фамилия И.О.) и email.
   
Настройка имени автора и email представлена на рисунке 4. Для того, чтобы имя пользователя применялось ко всем проектам, в команду config добавлена опция --global. Для просмотра полного списка настроек используется команда git config --list. С помощью нее осуществляется проверка установки настроек имени автора и email.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture4.png">
</p>
<p align="center">Рисунок 4 – Настройка имени и email</p> </br>


3. Клонирование своего личного удалённого репозитория на компьютер.
   
Для клонирования своего личного удалённого репозитория на компьютер, используется команда git clone с указанием ссылки на репозиторий (рис. 5). 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture5.png">
</p>
<p align="center">Рисунок 5 – Клонирование репозитория</p> </br>


4. Добавление файла через интерфейс GitHub. Подтягивание изменений в локальный репозиторий.
   
С помощью «Add file» происходит добавление файла через GitHub (рис. 6). Затем необходимо назвать файл (название создаваемого файла createdFile) и внести текстовые данные (рис. 7). Затем производится сохранение внесенных изменений «Commit changes…». На ветке мастер отображается только что созданный файл, что представлено на рисунке 8.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture6.png">
</p>
<p align="center">Рисунок 6 – Начало добавления нового файла</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture7.png">
</p>
<p align="center">Рисунок 7 – Создание нового файла</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture8.png">
</p>
<p align="center">Рисунок 8 – Созданный файл</p> </br>

Перед тем как подтягивать изменения в локальный репозиторий, необходимо перейти в него с помощью команды cd (изменения текущей рабочей директории). Только после этого используется команда pull, которая получает изменения из удалённого репозитория и обновляет рабочую копию в соответствии с удалённым репозиторием. На рисунке 9 представлено подтягивание изменений в локальных репозиторий.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture9.png">
</p>
<p align="center">Рисунок 9 – Подтягивание изменений</p> </br>


5. Получение истории операций для каждой из веток.

Команда git branch с опцией -a выводит список локальных и удалённых веток. Для получения истории операций для каждой из веток можно воспользоваться командой git log, которая отображает истории коммитов в репозитории. На рисунке 10 представлена история коммитов ветки master, а на рисунке 11 - история коммитов ветки branch1.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture10.png">
</p>
<p align="center">Рисунок 10 – Истории операций для master</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture11.png">
</p>
<p align="center">Рисунок 11 – Истории операций для branch1</p> </br>


6. Просмотр последних изменений.

Для просмотра последнего изменения используется команда git log --all --graph --oneline (рис. 12). Команда git log показывает список всех коммитов в текущей ветке. Параметр --all показывает коммиты из всех веток. Параметр --graph добавляет визуальное представление структуры коммитов в виде ASCII-графа. Параметр --oneline показывает каждый коммит в одной строке. 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture12.png">
</p>
<p align="center">Рисунок 12 – Просмотр последних изменений</p> </br>


7. Выполнение слияния в ветку master, разрешив конфликт.

Выполнения слияния в ветку master производится с помощью команды git merge (рис. 13). Возник конфликт между файлами с одинаковым названием mergefile.txt и разным содержанием, который можно посмотреть через команду git diff (сравнение содержимого файлов и фиксация его как результата слияния) (рис. 14). 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture13_1.png">
</p>
<p align="center">Рисунок 13 – Выполнения слияния</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture13.png">
</p>
<p align="center">Рисунок 14 – Отображение конфликта</p> </br>

С помощью Notepad можно увидить конфликт (рис.15) и решить его (рис. 16). В данной ситуации было принято сохранить обе версии файла, ничего не удаляя.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture14.png">
</p>
<p align="center">Рисунок 15 – Просмотр конфликта</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture15.png">
</p>
<p align="center">Рисунок 16 – Решение конфликта</p> </br>

После решение конфликта заново добавляем файл mergefile.txt в индекс в Git с помощью команды git add. Проверяем статус репозитория через git status. Делаем коммит и фиксируем изменения в репозитории (рис. 17). Команда git commit с опцией -m позволяет указать сообщение коммита прямо из командной строки. 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture16.png">
</p>
<p align="center">Рисунок 17 – Решенный конфликт</p> </br>


8. Удаление побочной ветки после успешного слияния.
   
Для того, чтобы удалить побочную ветку branch1 после успешного слияния локально используется команда git branch -d (рис. 18).
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture17.png">
</p>
<p align="center">Рисунок 18 – Удаление branch1</p> </br>


9. Внесение изменений, их фиксация и добавление комментариев.

С помощью команды echo создаются новые файлы (file1.txt и file1.txt) и c текстом в нем. "Стрелочки" применяются для добавления содержимого в файл (>>) или перезаписи его (>). Добавляются в Git, проверяются через ls и коммитятся. Выше описанные команды и результаты их выполнения представлены последовательно на рисунке 19.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture18.png">
</p>
<p align="center">Рисунок 19 – Создание файлов</p> </br>


10. Откат коммита.

Выводим историю операций для ветки master (рис. 20). Затем вызываем команду git reset HEAD~1, которая откатывает историю на один коммит назад, оставляя рабочую директорию и индекс неизменными, и после снова выводим историю ветки (рис. 21). 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture19.png">
</p>
<p align="center">Рисунок 20 – История коммитов до отката</p> </br>

<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture20.png">
</p>
<p align="center">Рисунок 21 – Откат коммита и история коммитов после отката</p> </br>


11. Создание ветки для отчёта.
    
Создается новая ветка branch_report с помощью команды git branch. На рисунке 22 представлено создание ветки для отчета.
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture21.png">
</p>
<p align="center">Рисунок 22 – Создание ветки для отчета</p> </br>

Затем с помощью команды git push (изменения с ветки master) и git push origin (новая ветка) отправляем изменения в удалённый репозиторий (рис. 23). 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture22.png">
</p>
<p align="center">Рисунок 23 – Отправка изменений в удаленный репозиторий</p> </br>

## Лог команд
$ git config --global user.name "4315 Алексеева А.С." </br>
$ git config --global user.email "aalekseeva.volt@mail.ru" </br>
$ git --list </br>
$ git clone https://github.com/AnyaAleks/LR2_BasicCoding </br>
$ git pull </br>
$ git log </br>
$ git branch -a </br>
$ git switch branch1 </br>
$ git log </br>
$ git log --all --graph --oneline </br>
$ git diff </br>
$ git add mergefile.txt </br>
$ git status </br>
$ git commit -m "Конфликт решен" </br>
$ git branch -d branch1 </br>
$ echo "Добавление информации в файл 1" > file1.txt </br>
$ git add file1.txt </br>
$ git commit -m "Добавлен 1 файл" </br>
$ echo "Добавление информации в файл 2" > file2.txt </br>
$ git add file2.txt </br>
$ git commit -m "Добавлен 2 файл" </br>
$ git log </br>
$ git reset HEAD~1 </br>
$ git log </br>
$ git branch branch_report </br>
$ git branch </br>
$ git push </br>
$ git push origin branch_report </br>

## История операций в форматированном виде 
<p align="center">
  <img src="https://github.com/AnyaAleks/LR2_BaseCodding/blob/branch_report/pictures_report/Picture23_2.png">
</p>
<p align="center">Рисунок 23 – Форматированный вывод истории операций</p> </br>

## Вывод
В ходе выполнения лабораторной работы были изучены базовые возможности системы управления версиями, получен опыт работы с Git и GitHub. Также был изучен функционал Git API и получен опыт работы с локальным и удаленным репозиторием.</br>
Был создан аккаунт на GitHub и освоен процесс fork существующего репозитория, что позволило создать собственную копию для дальнейшей работы. После установки и настройки клиента Git, было произведено клонирование удалённого репозитория на локальный компьютер.</br>
Работа с GitHub включала добавление файлов через интерфейс платформы, а также синхронизацию изменений между локальным и удалённым репозиториями. Получен опыт роботы в оформлении файла README с помощью markdown синтаксиса.</br>
В Git было изучено получение истории операций для каждой ветки, анализ последних изменений в репозитории. Была произведена работа с ветками и файлами. Также освоено разрешение конфликтов при слиянии веток в Git и работа с коммитами. </br>
Полученные знания и навыки будут полезны в дальнейшей практике разработки программного обеспечения, особенно в условиях командной работы и совместного редактирования кода.
