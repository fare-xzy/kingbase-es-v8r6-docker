# 人大金仓数据库Docker镜像制作

License 到期时间

```shell

docker build -t kingbase:v8r6 ./

docker run -d --name kingbasev8r6 -p 54321:54321 -e SYSTEM_USER=SYSTEM  -e SYSTEM_PWD=1111111111   kingbase:v8r6

```