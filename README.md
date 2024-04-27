# GUI client for Databases

## Commands 

```
PostgreSQL
docker-compose -f docker-compose.pgsql.yml up -d

MySQL
docker-compose -f docker-compose.mysql.yml up -d
docker-compose -f docker-compose.mysql.workbench.yml up -d

MongoDB
docker-compose -f docker-compose.mongo.yml up -d 

SQLServer
docker-compose -f docker-compose.sqlserver.yml up -d

MariaDB
docker-compose -f docker-compose.maria.yml up -d

Oracle
docker-compose -f docker-compose.oracle.yml up -d
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
