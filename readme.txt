### Step-By-Step GitHub Project ###
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:demwf/SmartLend.git
git push -u origin master

---=== Запуск агента для сохранения без запроса логина/пароля ===---

1. Запустить ssh-agent (в консоли git BASH)
eval "$(ssh-agent -s)"

2. Добавить сгенерированный ключ в ssh-agent
ssh-add ~/.ssh/id_rsa

3. Установить соединение с гитхаб
git remote add origin git@github.com:demwf/SmartLend.git

4. Изменить способ доступа для созданного репозитория. Без логин/пароль
git remote set-url origin git@github.com:demwf/SmartLend.git

5. установить username и email для подписи коммитов
git config --global user.name "demwf"
git config --global user.email "demwf@yandex.ru"

6. Проверить соединение локального репозитория с удаленным:
git remote -v

7. Коммиты
Локально
git add .
git commit -m "First"

затем Глобально
git push -u origin master
