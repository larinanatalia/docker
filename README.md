#  Команды для создания своего docker image с http сервером nginx + замена страницы приветсвия Nginx на своё

1. mkdir docker_nginx_test 
2. nano index.html
3. Копируем текст страницы, которую будем помиенть(файл index.html в репозитории) и сохраняем
4. docker run -d -p 80:80 -v ${PWD}:/usr/share/nginx/html --name=my_nginx nginx

