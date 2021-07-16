基于国内镜像的centos7+python+selenium完整运行环境 包含python依赖一站式全部解决 适合爬虫开发环境使用

### 已在服务器上构建成功 
### 已在服务器上构建成功 
### 已在服务器上构建成功 

## 构建方式
```
docker build -t centos7-python:3.8.10 -f Dockerfile . 
```
## 运行方式
```
docker run -itd --name python --restart always --privileged=true
```
## docker-compose 基本使用
```
docker-compose up -d 持久化运行
docker-compose restart 重启
docker-compose down 关闭
```

注意要点:

- yum安装完成后执行 yum clean all,进行过程文件清除
- 通过`docker history image` 查看每层的大小
- 编译安装后，删除源代码和整个编译目录


