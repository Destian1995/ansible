Самоконтроль выполненения задания

* Где расположен файл с some_fact из второго пункта задания?
```
ansible\group_vars\all
```
* Какая команда нужна для запуска вашего playbook на окружении test.yml?
```
ansible-playbook -i inventory/test.yml site.yml
```
* Какой командой можно зашифровать файл?
```
ansible-vault encrypt group_vars/all/examp.yml
```
* Какой командой можно расшифровать файл?
```
ansible-vault decrypt --ask-vault-password group_vars/all/*
```
* Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
```
ansible-vault view group_vars/all/examp.yml
```
* Как выглядит команда запуска playbook, если переменные зашифрованы?
```
ansible-playbook -i inventory/test.yml site.yml --ask-vault-pass
```
* Как называется модуль подключения к host на windows?
```
winrm
```
* Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
```
ansible-doc -t connection ssh
```
* Какой параметр из модуля подключения ssh необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
```
   - remote_user
```