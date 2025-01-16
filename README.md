# Postgres Light

[![Artifact HUB](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/postgres)](https://artifacthub.io/packages/search?repo=postgres)

## Run With Docker
```bash
pip install DockerBuildManagement
dbm -swarm -start
```

Access pgadmin at (username/password: admin@admin.no/admin): 
- http://localhost:8080/


## Use Helm Repo
```bash
helm repo add postgres https://raw.githubusercontent.com/hansehe/postgres-helm/master/helm/charts/postgres
helm repo add pgbouncer https://raw.githubusercontent.com/hansehe/postgres-helm/master/helm/charts/pgbouncer
helm repo update
```
```bash
helm install postgres postgres/postgres
helm install pgbouncer pgbouncer/pgbouncer
```
