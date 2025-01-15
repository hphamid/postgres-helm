# Pgbouncer Helm Chart

## Introduction

A lightweight pgbouncer helm chart for development purposes, check out:
- https://www.pgbouncerql.org/

## Installing the Chart

To install the chart with the release name `pgbouncer` run:

```bash
$ helm repo add pgbouncer https://raw.githubusercontent.com/hansehe/pgbouncer-helm/master/helm/charts
$ helm install pgbouncer pgbouncer/pgbouncer
```

Alternatively, a YAML file that specifies the values for the parameters can be provided while installing the chart. For example,

```bash
$ helm install pgbouncer -f values.yaml pgbouncer/pgbouncer
```

## Configuration

Find all possible configuration values here:
- https://github.com/hansehe/pgbouncer-helm/blob/master/helm/pgbouncer/values.yaml
