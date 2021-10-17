# Simple-Database-querying
```sh
select
    u.id,
    u.username,
    (
        select u2.username
        from users u2
        where u2.id = u.parent
    ) parentUsername
from users u
```
