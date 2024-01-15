tags: #docker

# Docker

links: [[dev/000_Index|Index]]

---

## Connecting to the filesystem of a container

For images without bash

```
docker exec -it CONTAINER /bin/sh --login
```

For images with bash

```
docker exec -it CONTAINER /bin/bash
```

## Interacting with MariaDB

Connecting to the database

```
docker exec -it CONTAINER mysql -u USER -pPASSWORD --default-character-set=utf8 DATABASE
```

Executing a SQL script

```
docker exec -i CONTAINER mysql -u USER -pPASSWORD DATABASE < ./xyz.sql
```

---
links: [[dev/000_Index|Index]]