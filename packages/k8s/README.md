## Publish To Upbound

```bash
export VERSION=v0.0.6

up login

up xpkg build --name k8s.xpkg

up xpkg push \
    --package k8s.xpkg \
    xpkg.upbound.io/upbound/kubecon-demo-k8s:$VERSION
```