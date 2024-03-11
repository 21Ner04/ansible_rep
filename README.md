# Ansible-rep
___

Данный репозиторий создан для выполнения практической работы по предмету "Внедрение и поддержка компьютерных систем".

## Задачи
___

1. Создать пользователя ansible-worker

2.  Установить Git. (ВАЖНО! на своей машине для тестирования положите ключи в папку ssh_keys (имена id_rsa и id_rsa.pub) в корне проекта и добавьте ее в .gitignore,  при проверка я буду использовать свои ssh ключи. Ключи нужны для того, чтобы работать с гитом, при проверке я добавлю такую же папку, но со своими ключами. Реализуйте механизм копированию ключей) 

3. [Склонировать репозиторий](https://github.com/iphilka/stud-template]) в директорию /home/ansible-worker/www/

4. В вашем проекте заранее должен быть определен файл index.html. [Шаблон тут](https://github.com/iphilka/stud-template/blob/main/index.html). Измените данные на свои.

5. Установка и настройка nginx. Копирование конфигурационного файла в sites-available и создание ссылки в sites-enabled.

**Конфигурационный файл**:

- Имя файла ansible.iphilka.ru.conf
- Доменное имя, по которому мы будем слушать порт 80 - ansible.iphilka.ru

-  Файл который мы отдаем при обращении по этому доменному имени /home/ansible-worker/www/stud-template/index.html

- Нужно самостоятельно разрешить все возможный проблемы с доступом. Проверка осуществляется автоматически и править разрешения к          файлам/папкам, если необходимо вы должны самостоятельно.

Теперь немного о структуре проекта в корне разместите файл  hosts.ini, во всех командах ansible ссылайтесь на него. Можете располагать файлы в любом удобном для вас виде. 
В корне проекта должен быть файл(run.txt), где будут написаны команды для ansible. Одна команда, одна стройка. *На основе команд записанных в этом файле будет осуществляться проверка.*
