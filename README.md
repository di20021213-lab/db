Задание 1
1.1. Поднимите чистый инстанс MySQL версии 8.0+. Можно использовать локальный сервер или контейнер Docker.
<img width="814" height="582" alt="1 задание нетология" src="https://github.com/user-attachments/assets/c934d35a-aeae-4826-a79f-a7c70a4349c3" />

1.2. Создайте учётную запись sys_temp.
<img width="284" height="146" alt="image" src="https://github.com/user-attachments/assets/4574e003-2e83-4457-926d-6b778abc5712" />
1.3. Выполните запрос на получение списка пользователей в базе данных. (скриншот)
все в 1.2
1.4. Дайте все права для пользователя sys_temp.
скрин ушёл к сожалению, воспользовался командой GRANT SELECT,UPDATE,INSERT ON db1 . * TO 'sys_temp'@'localhost';
1.5. Выполните запрос на получение списка прав для пользователя sys_temp. (скриншот)

1.6. Переподключитесь к базе данных от имени sys_temp.
<img width="952" height="642" alt="1 задание нетологии" src="https://github.com/user-attachments/assets/fbd6baec-9361-4872-bf29-ae40843a7e42" />

Для смены типа аутентификации с sha2 используйте запрос:
ALTER USER 'sys_test'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
1.6. По ссылке https://downloads.mysql.com/docs/sakila-db.zip скачайте дамп базы данных.
<img width="909" height="646" alt="image" src="https://github.com/user-attachments/assets/88c49ce1-1b5e-4881-9992-064f9238c0e9" />

1.7. Восстановите дамп в базу данных.
<img width="1132" height="760" alt="image" src="https://github.com/user-attachments/assets/64c6ceaf-8fd1-4484-ab7d-3193e690b9b0" />

1.8. При работе в IDE сформируйте ER-диаграмму получившейся базы данных. При работе в командной строке используйте команду для получения всех таблиц базы данных. (скриншот)
<img width="300" height="595" alt="image" src="https://github.com/user-attachments/assets/feb3f783-1393-4a59-90f8-40cb09ccf3be" />

Результатом работы должны быть скриншоты обозначенных заданий, а также простыня со всеми запросами.

Задание 2
Составьте таблицу, используя любой текстовый редактор или Excel, в которой должно быть два столбца: в первом должны быть названия таблиц восстановленной базы, во втором названия первичных ключей этих таблиц. Пример: (скриншот/текст)
