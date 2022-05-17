## Publish To Upbound

```bash
export VERSION=v0.0.4

up login

up xpkg build --name app.xpkg

up xpkg push \
    --package app.xpkg \
    xpkg.upbound.io/upbound/kubecon-demo-app:$VERSION
```
