https://practicum.yandex.ru/trainer/git-basics/lesson/c6b9607c-e8bc-4446-89f9-c74522c3492f/
<br>
<h1>Дополняем шпаргалку</h1> - https://practicum.yandex.ru/trainer/git-basics/lesson/5addb3b4-5171-426a-b753-b20ac48c1428/
<br>
Подсказка: как сделать mermaid-схему<br>
Чтобы получить mermaid-схему в README.md, нужно добавить блок кода типа mermaid.<br>

```markdown <br>
HEAD -- это голова.
Коммит -- это всему голова.
Статусы файлов: 
<тут пустая строка!>
```mermaid
%% описание схемы
```
<и тут пустая строка!>

Блоки кода в маркдауне начинаются и заканчиваются тремя символами ```. После первых трёх ``` можно указать, какой именно код будет внутри блока. Например: ```mermaid , ```bash, ```python, ```javascript и так далее. Если ничего не указать, GitHub будет считать весь код простым текстом.

💡 Перед блоком и после него нужны пустые строки, иначе GitHub может не понять, что это блок кода.

<h2>Дополнить коммит новыми файлами можно с помощью</h2>
git add . или touch index.html style.css dock.md
 
git commit --amend --no-edit
<p>Благодаря опции --no-edit сообщение к коммиту останется таким, каким и было.</p>

<h2>Точно так же можно добавить не новый файл, а дополнительные изменения в уже добавленном в коммит файле.</h2>

# Ещё раз отредактировали main.html

$ git add main.html # добавили в список на коммит<br>
$ git commit --amend --no-edit 

<h2>Как изменить сообщение последнего коммита?</h2>
git commit --amend -m "новое сообщение"

Если забыли указать один из флагов --no-edit или -m, Git предложит отредактировать сообщение вручную.

<h2>Чтобы убрать только один файл в пример credentials и при этом оставить файл в пример app.js в списке на коммит.</h2>

git restore --staged credentials

<h2>Как откатить изменения в файле app.js, но при этом оставить файл styles.css как есть.</h2>
git restore app.js

Она откатит файл до состояния последней сохранённой в коммите версии. По сути, это удалит все текущие изменения в файле.

<h2>Какую команду нужно использовать, чтобы коммит в пример aaa2508 исчез?</h2>

git reset --hard 96aa6ee

Он  96aa6ee предпоследний комит.

<h2>Как выяснить детали изменения внутри файла?</h2>

git diff

Команда git diff сравнит последнюю закоммиченную версию файла с той, что находится в состоянии modified.<br>
Команда git diff --staged покажет изменения в staged-файлах относительно последних закоммиченных версий.
