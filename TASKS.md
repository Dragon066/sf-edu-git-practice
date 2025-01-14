# Tasks

## Часть 2: Add и Commit

1. Создайте новую ветку `task/2/add-commit` из ветки `develop` и переключитесь на нее.
2. Создайте простую программу на python, которая будет выводить в консоль строку "Hello, world!".
3. Добавьте файл с программой в индекс (команда `git add`).
4. Добавте в вашу программу новую строку, которая будет выводить в консоль строку "Hello, git!".
5. Сделайте коммит с сообщением "Add hello world".
6. Обратите внимание, какие изменения попали в коммит (команда `git show`).
7. Сделайте коммит, который добавит изменения из пункта 4.
8. Вмерджите ветку `task/2/add-commit` в ветку `develop`.
9. Вмерджите ветку `task/2/next` в ветку `develop`.

## Часть 3: Работа со стешем

1. **Сейчас вы должны находиться в ветке `develop`.**
2. Создайте новую ветку `task/3/stash` из ветки `develop` и переключитесь на нее.
3. Добавьте файл `mood.txt` с описанием вашего настроения в индекс (stage).
4. Создайте новый файл `todo.txt` с описанием того, что вы собираетесь сделать сегодня.
5. Удалите строку из вашей программы на пайтоне, которая выводит в консоль строку "Hello, git!".
6. Создайте стеш (stash).
7. Посмотрите, что попало в стеш, а что нет.
8. Добавте текущие изменения в коммит.
9. Вмерджите ветку `task/3/stash` в ветку `develop`.
10. Посмотрите список стешей.
11. Переключитесь на ветку `task/3/stash` и примените стеш.
12. Убедитесь, что список стешей пуст.
13. Вмерджите ветку `task/3/stash` в ветку `develop`.
14. Вмерджите ветку `task/3/next` в ветку `develop`.

## Часть 4: Работа с ветками, конфликты

1. **Сейчас вы должны находиться в ветке `develop`.**
2. Создайте новую ветку `task/4/branches` из ветки `develop` и переключитесь на нее.
3. Создайте файл `task4.txt` и добавьте в него следующий текст:

```
Привет!

1. Я попал сюда из ветки task/4/branches
```

4. Добавьте файл `task4.txt` в коммите.
5. Переключитесь на ветку **`develop`** и создайте новую ветку `task/4/branches-сonflict` из ветки **`develop`** и переключитесь на нее.
6. Создайте файл `task4.txt` и добавьте в него следующий текст:

```
Привет!

2. Когда этот файл будет сливаться с веткой task/4/branches, то возникнет конфликт, в котором нужно будет разрешить, что делать с этими строками.

3. В результате в файле должны остаться все строки по порядку. Но строка со словом "Привет!" должна быть только одна.
```

7. Закоммитьте изменения.
8. Вмерджите ветку `task/4/branches-сonflict` в ветку `develop`.
9. Вмерджите ветку `task/4/branches` в ветку `develop`.
10. В этом моменте должен возникнуть конфликт. Разрешите его так же, как в файле `task4.txt`.
11. Вмерджите ветку `task/4/next` в ветку `develop`.

## Часть 5: Revert

1. **Сейчас вы должны находиться в ветке `develop`.**
2. Создайте новую ветку `task/5/revert` из ветки `develop` и переключитесь на нее.
3. Измените файл с программой на пайтоне так, чтобы она выводила в консоль строку "Hello, I am EVIL BUG!" вместо строки "Hello, world!".
4. Сделайте коммит с изменениями в программе на пайтоне.
5. Создайте файл `task5.txt` и добавьте в него следующий текст:

```
Привет!

Я должен остаться здесь. Я не должен быть удален.
```

6. Сделайте коммит с `task5.txt`.
7. Отмените изменения в файле с программой на пайтоне.
8. Вмерджите ветку `task/5/revert` в ветку `develop`.
9. В ветке `develop` должны остаться только изменения в файле `task5.txt`.
10. Вмерджите ветку `task/5/next` в ветку `develop`.

## Часть 6: Rebasing

1. **Сейчас вы должны находиться в ветке `develop`.**
2. Создайте новую ветку `task/6/rebase` из ветки `develop` и переключитесь на нее.
3. Создайте еще один файл `grocieries.txt` и добавьте в него следующий текст:

```
Список покупок:

1. Хлеб
2. Молоко
3. Яйца
```

4. Сделайте коммит с `grocieries.txt`.
5. Создайте файл `task6.txt` и добавьте в него следующий текст:

```
Привет!

1. Сейчас я нахожусь во второс коммите в ветке task/6/rebase.
2. А по окончанию этого задания я должен оказаться в предпоследнем в ветке develop.
```

6. Сделайте коммит с `task6.txt`.
7. Измените файл `grocieries.txt` так, чтобы он выглядел следующим образом:

```
Список покупок:

1. Хлеб
2. Молоко
3. Яйца
4. Сыр
```

8. Сделайте коммит с изменениями в `grocieries.txt`.
9. Сделайте rebase в ветке `task/6/rebase` так, чтобы поменять порядок коммитов так, чтобы сначала был коммит с `task6.txt`, а потом **ОДИН** коммит с изменениями в `grocieries.txt`. Для этого вам нужно будет объединить два коммита с изменениями в `grocieries.txt` в один.
10. Сделайте rebase ветки `develop` на изменения в ветке `task/6/rebase`.
11. Прверьте историю коммитов в ветке `develop`. Проверьте что добавилось два новых коммита с изменениями в `grocieries.txt` и что коммит с `task6.txt` стал вторым по счету с конца.
12. Вмерджите ветку `task/6/next` в ветку `develop`.

## Часть 7: Cherry-pick

1. **Сейчас вы должны находиться в ветке `develop`.**
2. Создайте файл `task7.txt` и добавьте в него следующий текст:

```
Ой ой ой!

Я случайно попал в ветку develop, хотя мы не ведем разработку в прямо ней. Нужно меня перенести в ветку task/7/cherry-pick.
```

3. Сделайте коммит с `task7.txt`.
4. Давайте поможем исправить эту ошибку. Создайте новую ветку `task/7/cherry-pick` из ветки `develop` и переключитесь на нее.
5. Сделайте cherry-pick коммита с `task7.txt` из ветки `develop`.
6. Обновите файл `task7.txt` так, чтобы он выглядел следующим образом:

```
Фух!

Теперь я в ветке task/7/cherry-pick. Наш процесс работы с git спасен!
```

6. Вернитесь в ветку `develop`. И отмените последний коммит. В результате ветка develop должна вернуться в состояние, в котором она была до этого задания.
7. Вмерджите ветку `task/7/cherry-pick` в ветку `develop`. Если вы все сделали правильно, то в ветке `develop` должен появиться коммит с изменениями в файле `task7.txt` без конфликтов и с последней версией текста.
8. Вмерджите ветку `task/7/next` в ветку `develop`.

## Часть 8: PR

1. **Сейчас вы должны находиться в ветке `develop`. И в ней должны быть все изменения из прошлых заданий**
2. Создайте новую ветку `task/8/pr` из ветки `develop` и переключитесь на нее.
3. Создайте файл `task8.txt` и добавьте в него следующий текст:

```
Ура, я прошел все задания! Я - молодец!
```

4. Сделайте коммит с `task8.txt`.
5. Вмерджите ветку `task/8/pr` в ветку `develop`.
6. Создайте PR из ветки `develop` в ветку `main`.
7. Сделайте ревью PR, оставьте в нем комментарий о том, как вы постарались и все сделали правильно, сделайте approve PR, и rebase & merge.
8. После того, как PR будет замержен, сделайте pull ветки `main` в свой локальный репозиторий.
9. В ветке `main` должны появится все изменения из прошлых заданий.
10. Перейдите в ветку `develop` и вмерджите ветку `task/8/next` в ветку `develop`.
