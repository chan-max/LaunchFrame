
## 启动mysql镜像
sudo docker run --name mysql  -v /usr/workspace/docker/mysql:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d --restart=always mysql

## 启动mongo镜像
docker run -d --name mongo -v /usr/workspace/docker/mongodb:/data/db -p 27017:27017 -e MONGO_INITDB_ROOT_USERNAME=admin -e MONGO_INITDB_ROOT_PASSWORD=admin --restart=always mongo

# postgressql
docker run --name postgres -e POSTGRES_PASSWORD=666666 -v /usr/workspace/docker/postgres:/var/lib/postgresql/data -p 5432:5432 -d postgres

# redis
docker run --name redis -v /usr/workspace/docker/redis:/data -p 6379:6379 -d redis redis-server --appendonly yes