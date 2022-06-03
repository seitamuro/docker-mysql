# 概要

docker上でMySQLのコンテナを作成します｡

# 1. Docker-hubからMySQLのイメージをインストールする

```
$ docker pull mysql
```

# 2. インストールしたイメージからコンテナを起動・作成する


```
$ docker run -it --name test-world-mysql -e MYSQL_ROOT_PASSWORD=mysql -d mysql:latest
$ docker exec -it test-world-mysql bash -p
$ mysql -u root -p -h 127.0.0.1
> mysql
```


# 参考

https://qiita.com/TAMIYAN/items/ed9ec892d91e5af962c6
