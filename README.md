# SalamanderDocker
一些Dockerfile

## 使用nginx镜像（Just for fun）
1. 构建镜像：docker build -t my_nginx:1.0 .
2. 运行容器：docker run -d -p 80:80 my_nginx:1.0


## 使用Docker-Compose
docker-compose使用docker-compose.yml文件来编排所有服务

1. 创建所有容器并启动：**docker-compose up**
2. 停止所有服务：**docker-compose stop**
3. 启动所有服务：**docker-compose start**