# Helm Repo
Repository with k8s Helm repo.
Basically it's a repository with helm repo.
Check out this example:
- https://github.com/kmzfs/helm-repo-in-github

## Update Helm Repo
```bash
cd helm
helm package postgres --destination charts #This will create tgz file with chart in charts directory
helm repo index ./charts #This will create index.yaml file which references postgres.yaml
git add *
git commit -m "postgres helm"
git push
```

## Use Helm Repo
```bash
helm repo add postgres 'https://raw.githubusercontent.com/hansehe/postgres-helm/master/helm/charts'
helm repo update
helm repo list
```
