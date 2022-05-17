## Publish To Upbound

```bash
export VERSION=v0.0.1

# Replace `[...]` with the Upbound Cloud account
export UP_ACCOUNT=[...]

up login

up xpkg build --name app.xpkg

up xpkg push \
    --package app.xpkg \
    xpkg.upbound.io/$UP_ACCOUNT/kubecon-demo-k8s:$VERSION
```