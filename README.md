1. Устанавливаете docker https://docs.docker.com/v17.09/engine/installation/linux/docker-ce/ubuntu/#install-using-the-repository
2. Устанавливаете docker-compose https://docs.docker.com/compose/install/
3. В папке с проектами git clone https://github.com/siqel/gDocker.git
4. Копируете docker-compose.yml.example в свой проект и переминовываете в docker-compose.yml
5. В директории своего проекта docker-compose up -d --build первый раз, потом можно без --build
6. Для переключения между проектами docker-compose down для завершения текущего проекта и docker-compose up -d в новом проекте

xdebug на порту docker-compose up -d --build

Troubleshout 
Проверяйте не заблокированны ли порты 80,443,3306 
Если проект не запускается пробуйте docker-compose up -d --build

Доступ в контейнер docker exec -it localhost-php-fpm bash
