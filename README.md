## rdkit_pgsql_cartridge
Dockerfile for PostgreSQL + RDKit PostgreSQL cartridge

This container is derived from [postgres:9.5](https://github.com/docker-library/postgres/tree/d7accc9c8c7d740ad756b887225fe31286d98f64/9.5).
See descriptions at [postgres official repository](https://hub.docker.com/r/library/postgres/) for more details.

### Versions
- [PostgreSQL](https://www.postgresql.org) 9.5
- [RDKit](https://github.com/rdkit/rdkit) [Release_2016.09.4](https://github.com/rdkit/rdkit/releases/tag/Release_2016_09_4)

### Getting started

```
docker run -d -p 5432:5432 dsatoh/rdkit_pgsql_cartridge
docker exec -it <container_id> psql -h localhost -U postgres -c 'CREATE DATABASE test_db'
docker exec -it <container_id> psql -h localhost -U postgres -c 'CREATE EXTENSION rdkit' test_db
```
