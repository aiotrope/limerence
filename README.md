# limerence

DBSWA assignment: Redis Cache for TODO API. 

Using redis cache. All database queries are cached for the sake of this exercise, but it is not recommended,
only expensive queries should be cache.

## CLI Commands

```bash
# build todo-api
$ cd todo-api && docker build -t todo-api .

# start container at the root directory; application running on port 7800
$ cd limerence && docker compose up

# stop running container
$ docker compose down

# run K6 performance measuring
$ k6 run performance-test-get-todos.js
```
