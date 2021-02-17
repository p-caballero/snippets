# SQL Server

## Index

* [DOCKER](#DOCKER)
  * [Run SQL Server 2017](#Run-SQL-Server-2017)
* [JOBS](#JOBS)
  * [Execute remotely](#Execute-remotely)

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
