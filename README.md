## 一、docker run
### `1、获取`
> docker pull ubuntu:18.04

### `2、运行`
> docker run -it --name ubuntu_18.04 -d -p 8000 -v /var/www:/var/www ubuntu:18.04

```
    -i:交互式操作
    -t:终端
    --name:容器名称
    -d:后台运行
    -p:端口映射
    -v:目录映射
    -rm:容器退出后删除
```

## 二、Dockerfile
### `1、Dockerfile 生成镜像`
> docker build -t php_7.1_fpm .
### `2、运行`
> docker run -it --name php_7.1_fpm -d -p 8000 -v /var/www:/var/www php_7.1_fpm

## 三、docker-compose
### `1、docker-compose生成镜像,并生成容器`
> docker-compose up --build


