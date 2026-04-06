# Paperless-ngx Helm Chart

An unofficial Helm chart for deploying [paperless-ngx](https://github.com/paperless-ngx/paperless-ngx) on Kubernetes with PostgreSQL (CloudNativePG), Valkey, Apache Tika, and Gotenberg.

## Prerequisites

- Kubernetes 1.26+
- Helm 3.x
- [CloudNativePG operator](https://cloudnative-pg.io/) installed on the cluster

## Installation

```bash
git clone https://github.com/toby-st/paperless-ngx-helm.git
cd paperless-ngx
helm dependency update
helm install paperless . --namespace paperless-ngx --create-namespace
```


## Configuration

See [values.yaml](paperless-ngx/values.yaml) for the full list of configurable values.

## Upgrading

```bash
helm upgrade paperless paperless-ngx/ --namespace paperless-ngx
```

## Uninstalling

```bash
helm uninstall paperless --namespace paperless-ngx
```

## License

Apache-2.0
