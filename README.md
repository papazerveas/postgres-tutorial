## 
see https://www.postgresqltutorial.com/postgresql-getting-started/postgresql-sample-database/

## init
.\pgsql\bin\initdb.exe -D .\data

## start

.\pgsql\bin\pg_ctl.exe -D .\data start
.\pgsql\bin\pg_ctl.exe -D .\data stop
.\pgsql\bin\pg_ctl.exe -D .\data restart


## superuser
.\pgsql\bin\createuser.exe --superuser postgres

## pgadmin
.\pgsql\bin\pgAdmin3.exe


## sql
.\pgsql\bin\psql.exe -U postgres -c 'create database dvdrental'
.\pgsql\bin\psql.exe -U postgres

##
.\pgsql\bin\pg_restore.exe -U postgres -d dvdrental  .\dvdrental.tar


### sql cmd
```sql
-- change default schema
ALTER DATABASE dvdrental SET search_path TO test_schema;

```