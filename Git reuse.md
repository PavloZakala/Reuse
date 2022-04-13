Для встановлення імені користувача:
```
git config --global user.email "user@example.com"
git config --global user.name "user"
```
Поточні дані про користувача:
```
git config -l
```
Генерація SSH ключа
```
ssh-keygen -t rsa -C "user@example.com"

cat ~/.ssh/id_rsa  # приватний ключ
cat ~/.ssh/id_rsa.pub  # публічний ключ
```
Створення нового alias:
```
git config --global alias.graph "log --all --oneline --graph"
```
Завантажити один файл з GitHub репозиторію:
```
wget https://github.com/ZPavlo/Tutorials/raw/master/Git_cookbook.ipynb
```

Для того щоб пушити на remote non-bare репозиторій:
```
git config receive.denyCurrentBranch updateInstead
```

Клонувати через ssh
```
git clone ssh://git@mydomain.com:[port]/gitolite-admin
```
