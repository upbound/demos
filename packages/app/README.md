## Publish To Upbound

```bash
export VERSION=v0.2.8

# Replace `[...]` with the Upbound Cloud account
export UP_ACCOUNT=[...]

up login

up xpkg build --name app.xpkg

up xpkg push \
    --package app.xpkg \
    xpkg.upbound.io/$UP_ACCOUNT/kubecon-demo-app:$VERSION
```
