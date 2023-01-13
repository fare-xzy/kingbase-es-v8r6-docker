# 人大金仓数据库Docker镜像制作

## 使用前说明

license版本为专业版本，90天有效期

kingbase版本为V008R006C005B0013

## 使用

### 制作镜像

将安装好的数据库Server文件夹打包放置于工程内 重命名为kingbase.tar.gz ，执行如下命令。

```shell
docker build -t kingbase:v8r6 ./
```

### 导入镜像

```shell
docker load --input ${name} 
```

### 创建并运行容器

```shell
docker run -d --name kingbasev8r6 -p 54321:54321 -e SYSTEM_USER=SYSTEM  -e SYSTEM_PWD=1111111111   kingbase:v8r6
```