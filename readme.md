# Git guide for me
---
## Работа в Git Bash
---
_&&_ - позволяет задать несколько команд в ондой строке  
_cd_ - смена директории  
* ~ - домашняя директория
* .. - на уровень вверх
* / - корневая директория  

_pwd_ - узнать текущую директорию  
_ls_ - вывести содержимое директории
* -а - выведет также скрытые папки и файлы, начинающиеся с .  
_cat_ - вывод содержимого файла на экран  
_cp_ (что_копируем)*n куда_копируем  - копируем выбранные файлы/папки в указанную дерикторию
_mv_ (что_копируем)*n куда_копируем  - перемещаем выбранные файлы/папки в указанную дерикторию
_touch_ - создать файл  
_mkdir_ - создать папку
* -p - позволяет создать сразу ряд вложенных папок
_rm_ - удаляет файл
* -r - позволяет удалить папку со всеми вложенными в нее папками и файлами
_rmdir_ - удаляет папку 
_clip <_ - копируем содержимое файла, указанного после <, в буфер обмена
---
## Работа с репозиториями
---
_git add_ - собираем файлы/папки для дальнейшего коммита
* --all - позволяет подготовить к сохранению все файлы в репозитории
* . - позволяет добавить всю текущую папку
* имя_конкретного_файла.разрешение - прямое указание файла для сохранения
_git status_ - проверить статус репозитория  
_git commit_ - делает коммит
* -m - позволяет добавить комментарий в '' к коммиту  
_git log_ - показывает историю коммитов  
_git init_ - инициализирует новый репозиторий  
_git remote add origin SHH-link на репозиторий_ - привязываем удаленный репозиторий к локальному по SSH  
_git push_ - отправляем изменения на удаленный репозиторий
* -u origin master - для первого вызова этой команды надо добавлять. Флаг -u свяжет локальную ветку с одноименной удаленной
---
## Создание и синхронизация локального и удаленного репозиториев
---
1. создаем локальную папку
2. переходим в нее в консоли при помощи _cd_
3. в консоли прописываем _git init_, чтобы инициализировать новый репозиторий и начать отслеживание существующего каталога
4. создаем на гитхабе новый репозиторий
5. в консоли прописываем _git remote add origin SHH-link на репозиторий_ 
6. можем проверить успешность синхронизации командой _git remote -v_
