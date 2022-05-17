## Publish To Upbound

```bash
export VERSION=v0.3.3

# Replace `[...]` with the Upbound Cloud account
export UP_ACCOUNT=[...]

up login

up xpkg build --name sql.xpkg

up xpkg push \
    --package sql.xpkg \
    xpkg.upbound.io/$UP_ACCOUNT/kubecon-demo-sql:$VERSION
```