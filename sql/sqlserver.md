# SQL Server

## Index

- [SQL Server](#sql-server)
  - [Index](#index)
  - [DOCKER](#docker)
    - [Run SQL Server 2017](#run-sql-server-2017)
  - [JOBS](#jobs)
    - [Execute remotely](#execute-remotely)
  - [SQL Server Express LocalDB](#sql-server-express-localdb)
    - [Database common name](#database-common-name)
    - [List instances](#list-instances)
    - [Stop instance](#stop-instance)
    - [Delete instance](#delete-instance)
    - [Recreate/Create new instance](#recreatecreate-new-instance)

---

## DOCKER

### Run SQL Server 2017

```bash
docker run --name sql-server-2017 -e 'ACCEPT_EULA=Y' -e 'SA_PASSWORD=P4$$w0rd12345' -p 1433:1433 -v /c/Temp/:/host/ -d microsoft/mssql-server-linux:2017-latest
```

## JOBS

### Execute remotely

```sql
sqlcmd -S "<servername>" -Q "execute msdb.dbo.sp_start_job @job_name='<job name>'"
```

## SQL Server Express LocalDB

### Database common name

```bash
(localdb)\MSSQLLocalDB
```

### List instances

```bash
sqllocaldb i
```

### Stop instance

```bash
sqllocaldb p <instance name>
```

### Delete instance

```bash
sqllocaldb d <instance name>
```

### Recreate/Create new instance

```bash
sqllocaldb c <instance name>
```
