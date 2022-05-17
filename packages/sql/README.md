## Publish To Upbound

```bash
export VERSION=v0.0.5

up login

up xpkg build --name sql.xpkg

up xpkg push \
    --package sql.xpkg \
    xpkg.upbound.io/upbound/kubecon-demo-sql:$VERSION
```