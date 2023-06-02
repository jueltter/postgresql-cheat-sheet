# postgresql-cheat-sheet


## activities

* Activities associated with the database.

```sql
SELECT * FROM pg_stat_activity WHERE datname = '<database_name>';
```

* Terminate active connections.

```sql
SELECT	pg_terminate_backend (pid) FROM	pg_stat_activity WHERE	pg_stat_activity.datname = '<database_name>';
```