# oc - simple Docker container with OpenShift CLI utility

1. Build

```
    docker build -t quay.io/ebbe_jonsson/ebxoc .
```

2. Set up alias:

```
alias oc='docker run --rm -ti -v /etc/hosts:/etc/hosts:ro -v $(pwd):/files -v $(pwd)/.kube:/root/.kube quay.io/ebbe_jonsson/ebxoc'
```
