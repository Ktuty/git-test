1.	Инициализировать версионный контроль Git в папке с проектом командой git init.
2.	Создать ветки master и develop командами git branch master и git branch develop.
3.	Переключиться на ветку develop командой git checkout develop.
4.	Доработать код приложения, чтобы echo сервер мог принимать произвольные данные, не только целые числа. При этом оставить текст "Введите целое число:" и "Вы ввели число:" из предыдущей версии.
5.	Зафиксить изменения в ветке develop командой git add . и git commit -m "Добавлена возможность принимать произвольные данные".
6.	Создать feature ветку из develop для нового функционала командой git checkout -b feature/correcting-text.
7.	Внести в feature ветке нужные изменения для исправления текстовых пояснений.
8.	Зафиксить изменения в feature ветке командой git add . и git commit -m "Исправлены текстовые пояснения".
9.	Переключиться на ветку develop командой git checkout develop.
10.	Слить feature ветку в develop командой git merge feature/correcting-text.
11.	Создать release ветку из develop командой git checkout -b release/add-tag.
12.	Создать новую метку (или тэг) с произвольным именем командой git tag echo-bot.v1
13.	Переключиться на ветку master командой git checkout master.
14.	Смержить release ветку с master командой git merge release/add-tag.
15.	Создать hotfix ветку из master командой git checkout -b hotfix/urgent-edits.
16.	Выполнить в hotfix ветке срочные правки.
17.	Зафиксить изменения в hotfix ветке командой git add . и git commit -m "Срочные правки".
18.	Переключиться на ветку master командой git checkout master.
19.	Смержить hotfix ветку с master командой git merge hotfix/urgent-edits.
20.	Переключиться на ветку develop командой git checkout develop.
21.	Смержить hotfix ветку с develop командой git merge hotfix/urgent-edits.
