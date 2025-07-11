# Домашнее задание 3

Домашнее задание состоит из 3 частей:
1. Создание репозитория в GitHub
2. Клонирование репозитория
3. Отработка взаимодействия

---

### Часть 1: Создание репозитория в GitHub

1. Перейдите в GitHub: https://github.com/
2. Нажмите на кнопку `New` для создания репозитория.

![New-repository.png](images/New-repository.png)

3. Настройте новый репозиторий:
    - Введите имя репозитория: `TestRepository`
    - Выберите `Private`
    - Добавьте файлик `.gitignore` для Python
    - Нажмите кнопку `Create repository`

![Settings-repository.png](images/Settings-repository.png)

Поздравляем! Репозиторий создан!

---

### Часть 2: Клонирование репозитория

1. В новом репозитории нажмите кнопку `Code` и скопируйте HTTPS-ссылку.

![Copy-url-repository.png](images/Copy-url-repository.png)

2. Откройте PyCharm и в меню `File` выберите `Project from Version Control...`

![Open-menu.png](images/Open-menu.png)

![Project-from-vc.png](images/Project-from-vc.png)

3. Вставьте скопированный URL и нажмите `Clone`

![Add-git-reposirory.png](images/Add-git-reposirory.png)

4. При первом подключении из PyCharm потребуется авторизация в GitHub.
5. Для авторизации можно использовать токен или вход через github.
Выбираем вход через GitHub.

![login-via-github.png](images/login-via-github.png)

6. Данная кнопка перенаправляет на web-страницу с авторизацией.
На странице нужно нажать кнопку `Authorize in GitHub`

![Authorize-in-github.png](images/Authorize-in-github.png)

7. После должно появиться сообщение об успешной авторизации.

![Successfully-authorized.png](images/Successfully-authorized.png)

8. Теперь можно перейти в PyCharm и открыть проект.

![open-this-window.png](images/open-this-window.png)

9. В открытом проекте должен лежать 1 файлик - `.gitignore`

![open-test-repository.png](images/open-test-repository.png)

10. Теперь GitHub и PyCharm связаны.

>Добавить или удалить аккаунт можно в пункте меню `Settings` -> `Version Control` -> `GitHub`

---

### Часть 3: Отработка взаимодействия

1. Откройте файл `.gitignore`. Найдите пункт `PyCharm`. В данном пункте раскомментируйте строку `.idea/`.
Готовый вариант должен выглядеть как на изображении ниже.

![Settings-gitignore.png](images/Settings-gitignore.png)

2. Сделайте коммит с описанием `Update .gitignore`
3. Создайте файл `task1.txt` и добавьте его в отслеживаемые.
4. Добавьте в файл `task1.txt` содержимое: `Это было бы мученье, но я настроил подключение`
5. Сделайте коммит с описанием `Add task1.txt`
6. Теперь при помощи команды Push отправьте изменения в локальной ветке main на удаленный репозиторий, также в ветку main.

![Push1.png](images/Push1.png)

![Settings-push1.png](images/Settings-push1.png)

7. Перейдите в GitHub, обновите страницу и проверьте изменения.

> Запомните! Отправлять коммиты сразу в ветку main - плохая практика!
> В дальнейшем, в процессе выполнения домашних заданий на курсе так делать запрещено!
> 
> Если в ходе выполнения домашних работ вы случайно зальете изменения сразу в ветку main,
> нужно будет откатить изменения и сделать корректный Pull Request.

8. Перед тем, как создавать новую ветку, нужно загрузить обновленную ветку main из удаленного репозитория.
Для этого нажмите на ветку main и выберите `Update Project...`

![Update-project-1.png](images/Update-project-1.png)

![Update-project-1-settings.png](images/Update-project-1-settings.png)

9. Создайте ветку `hw3` от ветки `main`

![Create-new-branch.png](images/Create-new-branch.png)

![Create-new-branch-name.png](images/Create-new-branch-name.png)

10. Проверьте, что вы находитесь на ветке `hw3`

![Hw3-branch.png](images/Hw3-branch.png)

11. Создайте файл `task2.txt` со следующим содержимым: `Изучаю, познаю, до конца точно дойду` и добавьте его в stage git.
12. Сделайте коммит с описанием `Add task2.txt` и отправьте изменения на удаленный репозиторий в GitHub.
Данные действия можно сделать одной кнопкой - `Commit and Push...`

![Push2.png](images/Push2.png)

13. Убедитесь, что на удаленном репозитории будет создана новая ветка `hw3`

![Settings-push2.png](images/Settings-push2.png)

14. Перейдите в GitHub и откройте Pull Request (PR).

![New-pr-1.png](images/New-pr-1.png)

15. Настройте PR. Убедитесь, что изменения будут отправляться из ветки `hw3` в ветку `main`.
Введите название `HW 3`. В меню `Reviewers` вы в будущем будете выбирать ваших преподавателей.
Пока что оставьте это поле без изменений. Нажмите кнопку `Create pull request`

![New-pr-settings-1.png](images/New-pr-settings-1.png)

16. В последующих домашних заданиях кнопку `Merge pull request` можно будет нажимать **только после того, как преподаватели одобрят PR!**

> Если вы случайно (хотя нужно нажать 2 кнопки) смержите ветки до одобрения преподавателей, то
> можно будет откатить PR путем создания нового.
> 
> Подробнее см. [Reset_PR.md](Reset_PR.md)

![Merge-pr.png](images/Merge-pr.png)

17. В данном домашнем задании PR не проверяется, поэтому нажмите на кнопку `Merge Pull Request`.
После можете ввести сообщение к коммиту, описание и нажать кнопку `Confirm merge`

![Confirm-merge.png](images/Confirm-merge.png)

18. Теперь можно безопасно удалить ветку `hw3`  и на Github, и в локальном репозитории.

![Delete-branch.png](images/Delete-branch.png)

19. Перейдите в PyCharm и переключитесь на ветку main

![Checkout-main.png](images/Checkout-main.png)

20. Файлик `task2.txt` пропал, так как в локальной ветке main еще нет изменений из ветки main на Github.
21. Обновите локальную ветку main с помощью `Update Project...`

![Update-project-2.png](images/Update-project-2.png)

22. Приложите в iSpring скриншот PyCharm с меню `Git` и файловой структурой.
Пример:

![PyCharm-final.png](images/PyCharm-final.png)

23. Также приложите скриншот с GitHub.
Пример:

![GitHub-final.png](images/GitHub-final.png)

---

### Полезные материалы:

- Интерактивный курс по git: https://learngitbranching.js.org/?locale=ru_RU.
- Руководство по работе с Git и GitHub через интерфейс PyCharm: https://teletype.in/@kurilkv/CodimGitHub#H084
- [Что делать если отправил изменения сразу в ветку main](Reset_commit.md)
- [Что делать если сделал Merge pull request до проверки](Reset_PR.md)