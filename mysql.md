
## 启动mysql镜像
sudo docker run --name mysql  -v /usr/workspace/docker/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql

## 启动mongo镜像
docker run -d --name mongo -v /usr/workspace/docker/mongodb:/data/db -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=admin  mongo


