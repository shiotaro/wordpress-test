# wordpress-test
Herokuで動かす

# Herokuで動かす
https://qiita.com/k_shiota/items/73073d1476d64135eff0

# Dockerで動かす
Dockerで動かすには下記の作業が必要です

## .envを追加する

```
WORDPRESS_DB_NAME=wordpress
WORDPRESS_DB_USER=wp_user
WORDPRESS_DB_PASSWORD=hogehoge

MYSQL_RANDOM_ROOT_PASSWORD=yes
MYSQL_DATABASE=wordpress
MYSQL_USER=wp_user
MYSQL_PASSWORD=hogehoge
```

## docker-compose

```
docker-compose up -d -buil
```
その後
```
docker ps
```
で立ち上がったことを確認する
