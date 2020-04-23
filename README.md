# moodle_test

## Инструкция

1. Зайти в `deploy` и ввести команду `sudo ./build_and_run_docker.sh`
2. Ввести команду `sudo docker exec -it <container_id> bash`
3. Ввести команду `mysql -u root -p`, пароль: `devel@`
4. Ввести команду `CREATE USER 'test_user'@'%' IDENTIFIED BY 'password';`
5. Ввести команду `GRANT ALL PRIVILEGES ON * . * TO 'test_user'@'%';`
6. `\q`
7. В браузере перейти по http:localhost:1010/install.php 
8. Выбрать ru, потом 2 раза "далее"
9. В пользователе написать `test_user` и пароль `password`
