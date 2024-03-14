

docker run -d -p 3306:3306 --privileged=true
-v / :/var/log/mysql
-v / :/var/lib/mysql
-v /:/etc/mysql/conf.d
-e MYSQL_ROOT_PASSWORD=root
-name mysql 