# Домашнее задание 2

Домашнее задание состоит из 4 частей:
1. Настройка git
2. Создание проекта в PyCharm
3. Настройка .gitignore
4. Работа с файлами

---

### Часть 1: Настройка git

1. Откройте консоль git.

![Open-cmd.png](images/Open-cmd.png)

2. Измените имя пользователя в консоли с помощью команды:
```commandline
git config --global user.name "Здесь имя пользователя"
```

![Update-name.png](images/Update-name.png)

3. Измените почту пользователя на ту, которая указана в GitHub с помощью команды:
```commandline
git config --global user.email почта
```

![Update-email.png](images/Update-email.png)

4. Проверьте установленные параметры с помощью команды:
```commandline
git config --list --show-origin
```

---

### Часть 2: Создание проекта в PyCharm

1. Откройте PyCharm.
2. Создайте новый проект.

![New-project.png](images/New-project.png)

3. Введите название проекта `TestProject`, выберите существующую виртуальную среду.
После завершения всех настроек нажмите `Create`

![Project-settings.png](images/Project-settings.png)

4. Проект должен выглядеть примерно как на изображении ниже.

![Project-done.png](images/Project-done.png)

---

### Часть 3: Настройка .gitignore

1. Откройте консоль и проинициализируйте репозиторий командой `git init`

![Git-init.png](images/Git-init.png)

2. Нажмите правой кнопкой мыши на название проекта -> New -> File.

![Create-file-gitignore.png](images/Create-file-gitignore.png)

3. Введите название файла `.gitignore` и нажмите Enter.

![name-file-gitignore.png](images/name-file-gitignore.png)

4. Появится окно с вопросом - нужно ли добавить файлик в stage git. Нажмите `Add`

![Add-file-to-git.png](images/Add-file-to-git.png)

5. Введите в файле текст `.idea/`, чтобы убрать папку из отслеживаемых.

![Gitignore-idea.png](images/Gitignore-idea.png)

6. Откройте меню `Commit`

![Git-menu.png](images/Git-menu.png)

> Если меню нет - нажмите 3 точки и выберите его в списке.

![Open-git-menu.png](images/Open-git-menu.png)

7. Перейдите в меню `Commit`, выделите все файлики, введите название коммита
`Add gitignore` и нажмите на кнопку `Commit`

![Commit-gitignore.png](images/Commit-gitignore.png)

---

### Часть 4: Работа с файлами

1. Создайте новый файлик под названием `task1.txt`
Для этого нажмите правой кнопкой мыши на название папки и введите название.
2. Появится окно с вопросом - нужно ли добавить файлик в stage git. Нажмите `Add`

![Git-add-window.png](images/Git-add-window.png)

3. Перейдите в меню `Commit`, выделите файлик, введите название коммита `Add task1.txt`
и нажмите `Commit`.

![Initial-commit.png](images/Initial-commit.png)

4. Теперь внесите изменения в файл `task1.txt` с текстом
`Начинается дорожка, но прошел я лишь немножко.`

    В меню `Commit` файлик подсветился синим - теперь он изменённый.
5. Выделите файлик и сделайте коммит с описанием `Add text in task1.txt`

![Git-commit-1.png](images/Git-commit-1.png)

6. Перейдите в меню `Git` (значок подсвечен на изображении внизу слева). Здесь отражена вся информация о ваших коммитах.

![Git-icon.png](images/Git-icon.png)

7. Вернитесь на коммит назад с помощью команды `Reset` и режима `Mixed`.
Состояние файла станет "изменённый".

![Reset-current-branch.png](images/Reset-current-branch.png)

![Reset-current-branch-mixed.png](images/Reset-current-branch-mixed.png)

8. Сделайте коммит с файликом task1.txt с описанием `Update task1.txt`
9. Вернитесь на коммит назад с помощью команды `Reset` и режима `Hard` - в таком случае все изменения и новые файлы будут утеряны.

   Это может помочь, если код полностью сломался и вы не знаете, где ошибка. **Применяйте с крайней осторожностью!**
10. Скопируйте в файлик `task1.txt` следующий текст: `Продолжается дорожка и прошел я уже "множко".`
11. Сделайте коммит с описанием `Add text in task1.txt`
11. Создайте файл `task2.txt`, добавьте его в stage git и внесите в него строку `Параллельная дорожка начинается немножко.`
12. Удалите текст из файла `task1.txt`
12. Перейдите в меню `Commit`, там вы увидете 2 файлика - изменённый и только что добавленный.
Сделайте коммит с описанием `Fix task1.txt and Add task2.txt`

![Update-files.png](images/Update-files.png)

13. Измените содержимое файла `task2.txt` на `Параллельная дорожка продолжается ...`
14. Теперь верните файл `task2.txt` в исходное состояние с помощью Rollback.

![Rollback-file.png](images/Rollback-file.png)

15. Удалите файл `task2.txt`. Сделайте коммит с описанием `Delete task2.txt`

![Delete-task2.png](images/Delete-task2.png)

16. Измените содержимое файла `task1.txt` на `Вот закончилась дорожка, изучил я git немножко.`
Сделайте коммит с описанием `Update text in task1.txt`

![Git-commit-final.png](images/Git-commit-final.png)

17. Приложите в iSpring скриншот PyCharm с меню `Git` и файловой структурой. Пример:

![Screenshot-window.png](images/Screenshot-window.png)

---

### Полезные материалы

- Руководство по работе с Git и GitHub через интерфейс PyCharm: https://teletype.in/@kurilkv/CodimGitHub#H084