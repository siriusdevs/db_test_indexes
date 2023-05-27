Дана таблица `tasks` со свойствами `name`, `status`, `priority`, `created` (дата создания).

Составить бинарные деревья поиска, которые могут соответствовать следующим индексам:

1:
```sql
create index tasks_created on tasks using btree(created)
```
2:
```sql
create index tasks_priority_created on tasks using btree(priority, created)
```
3:
```sql
create index tasks_status_priority_created on tasks using btree(status, priority, created)
```

Для каждого индекса написать запросы, которые могут использовать этот индекс.
