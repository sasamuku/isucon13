# isucon13

#### app.rb
ISUCON13_MYSQL_DIALCONFIG_ADDRESSを「db」に変更

#### 起動
docker-compose up -d

## DB
#### DB コンテナに入って行う
```
mysql -u root -p
source /app/initdb.d/00_create_database.sql
source /app/initdb.d/10_schema.sql
exit
mkdir /pdns
touch init_zone.sh
vim init_zone.sh
ローカルのinit_zone.shを書き込む
dos2unix /app/init.sh
bash /app/init.sh
```