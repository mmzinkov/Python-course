# Что делать, если сделал Merge pull request до проверки

> Допустим есть PR, который уже залит в main

![Merged-pr.png](images_reset-pr/Merged-pr.png)

1. В PyCharm перейдите на ветку `main`, обновите её. Откатите изменения с помощью метода `Hard`
до того момента, 
когда была создана ветка, влитая в main.

> В примере коммит `Add task3.txt` был сделан уже на ветке `hw4`. Поэтому
> нужно откатиться на один коммит ниже. 

![Main-commit.png](images_reset-pr/Main-commit.png)

2. Отправьте изменения с локальной ветки main в удалённую с помощью форсированного пуша.

> Форсированный пуш может быть не доступен в ветку `main` из-за правил безопасности.
> Отключите их на время.
> 
> Зайдите в настройки `Settings -> Version Control -> Git`, сохраните текст из поля 
`Protected branches` и очистите его.

![Disable-protected-branch.png](images_reset-pr/Disable-protected-branch.png)

![Push-main.png](images_reset-pr/Push-main.png)

![Force-push.png](images_reset-pr/Force-push.png)

![Force-push-warning.png](images_reset-pr/Force-push-warning.png)

3. Отправьте нужную ветку в удалённый репозиторий для возможности создания PR.

> В примере ветку `hw4` нужно отправить на удалённый репозиторий.

![Push-hw4.png](images_reset-pr/Push-hw4.png)

![Push-hw4-settings.png](images_reset-pr/Push-hw4-settings.png)

4. Создайте новый PR из ветки `hw4` в `main`

![New-pr.png](images_reset-pr/New-pr.png)

![Settings-new-pr.png](images_reset-pr/Settings-new-pr.png)

5. Укажите преподавателей для проверки RP.

![Open-new-pr.png](images_reset-pr/Open-new-pr.png)

> Задайте правила безопасности для веток.
> Зайдите в настройки `Settings -> Version Control -> Git`, заполните поле
`Protected branches` теми значениями, которые в нём были.