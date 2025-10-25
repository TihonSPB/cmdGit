
<h2 align="center" id="title1">Установка GIT</h2>

Скачать и установить https://git-scm.com/

$\color{rgb(255,132,61)}{\textsf{o}}$ Документация    
```
git
```  

<h2 align="center" id="title2">Настройка</h2>

$\color{rgb(255,132,61)}{\textsf{o}}$ Проверить версию GIT   
```
git --version
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Текущие настройки
```
git config --list
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Смена имени пользователя
```
git config --global user.name "Имя"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Проверка имени пользователя
```
git config --global user.name
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Смена почты пользователя
```
git config --global user.email "адрес@почта.ком"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Проверка почты пользователя
```
git config --global user.name
```

<h2 align="center" id="title3">Создание локального репозитория</h2>

Смена диска
```
D:
```

Посмотреть наличие файлов и папок в директории
```
dir
```

Смена директории
```
cd <Путь>
```

Создать папку в директории  
```
mkdir "Имя папки"

md "Имя папки"

mkdir "Папка1" "Папка2"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Инициализировать как локальную дирикторию
```
git init
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Добавить все папки и файлы в репозитории для commit
```
git add .
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Добавить файл в репозитории для commit
```
git add <файл>
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Создать commit с комментарием в репозитории
commit - точка сохранения/указания на версии
```
git commit -m "Комментарий"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Проверить статус файлов
```
git status
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Просмотр истории изменений
```
git log
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Переход к определенному коммиту
```
git checkout <branch name>
git checkout <commit hash>
```

<h2 align="center" id="title4">Создание удаленного репозитория</h2>

Зарегистрироваться на https://github.com/   
Создайте удаленный репозиторий Create repository (Имя удаленного должно совпадать с локальным)   

$\color{rgb(255,132,61)}{\textsf{o}}$ Связать локальный репозиторий с удаленным.   

во вновь созданный удаленный репозиторий и найдите следующий раздел:   
...or push an existing repository from the command line   
Выполнить поочередно все команды из раздела   
```
git remote add origin https://github.com/Имя_пользователя/Название_репозитория.git
git branch -M main
git push -u origin main
```

будет предложено подтвердить намерения связать Git и GitHub.   

$\color{rgb(255,132,61)}{\textsf{o}}$ Отправить изменения в удаленный репозиторий
```
git push
```

<h2 align="center" id="title5">Клонирование удаленного репозитория на локальный</h2>

Перейти в репозиторий который необходимо клонировать из https://github.com/   
Нажать кнопку "<> Code" и во вкладке Local скопировать адрес по https   

$\color{rgb(255,132,61)}{\textsf{o}}$  Клонировать репозиторий 
```
git clone https://github.com/Имя_пользователя/Название_репозитория.git
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Синхронизировать локальный репозиторий в соответствии с удаленным
```
git pull
```

<h2 align="center" id="title6">Работа с ветками</h2>

$\color{rgb(255,132,61)}{\textsf{o}}$ Просмотр всех веток
```
git branch
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Создать ветку
```
git branch "Имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Переключить ветку
```
git checkout "Имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Создать и переключить ветку
```
git checkout -b "Имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Переименовать текущую ветку
```
git branch -m "Новое имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Удалить ветку
```
git checkout -b "Имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Разместить локальную ветку на удаленном репозитории
```
git push -u origin "Имя ветки"
```

$\color{rgb(255,132,61)}{\textsf{o}}$ Слияние ветки с текущей (перейти в принимающую ветку и выполнить слияние) 
```
git merge "Имя ветки"
```