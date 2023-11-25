# isucon13

## DB
```
# DB コンテナに入って行う
mysql -u root -p
source /app/initdb.d/00_create_database.sql
source /app/initdb.d/10_schema.sql
exit
yum install dos2unix
dos2unix /app/init.sh
bash /app/init.sh
```