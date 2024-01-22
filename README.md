https://practicum.yandex.ru/trainer/git-basics/lesson/c6b9607c-e8bc-4446-89f9-c74522c3492f/
<br>
Дополняем шпаргалку - https://practicum.yandex.ru/trainer/git-basics/lesson/5addb3b4-5171-426a-b753-b20ac48c1428/
<br>
Подсказка: как сделать mermaid-схему<br>
Чтобы получить mermaid-схему в README.md, нужно добавить блок кода типа mermaid.<br>

```markdown <br>
HEAD -- это голова.<br>
Коммит -- это всему голова.<br>
Статусы файлов: <br>
<тут пустая строка!><br>
```mermaid<br>%% описание схемы<br>```<и тут пустая строка!><br>

Блоки кода в маркдауне начинаются и заканчиваются тремя символами ```. После первых трёх ``` можно указать, какой именно код будет внутри блока. Например: ```mermaid , ```bash, ```python, ```javascript и так далее. Если ничего не указать, GitHub будет считать весь код простым текстом.

💡 Перед блоком и после него нужны пустые строки, иначе GitHub может не понять, что это блок кода.