# GUI client for Databases

## Commands 

```
PostgreSQL
docker-compose -f postgresql/pgadmin.yaml up -d

MySQL
docker-compose -f mysql/phpmyadmin.yaml up -d
docker-compose -f mysql/mysql-workbench.yaml up -d

MongoDB
docker-compose -f mongodb/mongoclient.yaml up -d 

SQLServer
docker-compose -f sqlserver/cloudbeaver.yaml up -d

MariaDB
docker-compose -f mariadb/phpmyadmin.yaml up -d
docker-compose -f mariadb/cloudbeaver.yaml up -d

Oracle
docker-compose -f oracle/cloudbeaver.yaml up -d
```

## Ports

```
5010, 5011           pgsql
5012, 5013, 5014     mysql
5015, 5016           mongo
5017                 sqlserver
5018                 maria
5019, 5020, 5021     oracle
```

## Check Database Version

Here are a few SQL queries to check our working database versions:

```sql
SELECT @@VERSION;            /*sql server*/       /*also works with mysql*/
SELECT * FROM V$VERSION;     /*oracle*/
SELECT VERSION();            /*mysql*/            /*also works with postgre*/
SELECT VERSION();            /*mariadb*/
SELECT VERSION();            /*postgre sql*/      /*also works with mysql*/
```
