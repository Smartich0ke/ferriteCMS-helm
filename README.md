# FerriteCMS-helm
Helm chart for FerriteCMS

## Usage

```bash
helm repo add ferritecms https://ferritecms.github.io/helm
helm repo update
helm install ferritecms ferritecms/ferritecms
```

## Database and Cache

FerriteCMS requires a database and cache to be configured. The default values
will use a Postgres database and Redis cache. The chart does not provide these
services, so you will need to provide your own. I recommend using cloudnative-pg
and ot-operator redis.