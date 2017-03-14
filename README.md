这是一个利用Maven和Docker方便构建部署多个项目的好东东，当使用命令行到这里的时候，你可以，

mvn clean package	：	编译，打包

mvn clean install	：	编译，打包，创建镜像

docker-compose up 	:	创建容器并启用服务
docker-compose stop	：	停止容器服务
docker-compose rm	：	删除容器服务

docker images		:	镜像列表
docker rmi -f $(docker images | grep "teligen" | awk "{print \$3}")		:		删除镜像名有"teligen"的所有镜像