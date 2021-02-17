# SQL Server

## Index

* [JOBS](#JOBS)
  * [Execute remotely](#Execute-remotely)

## JOBS

### Execute remotely

```sql
sqlcmd -S "<servername>" -Q "execute msdb.dbo.sp_start_job @job_name='<job name>'"
```
