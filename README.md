# Overview
Kustomize for K3s clusters  
Current apps running on cluster  
- unbound
- blocky

## Commands
Apply everything
```shell
kubectl apply -k overlays/seattle
```

## cilium-envoy
For raspberry pi with TCMALLOC error

```shell
kubectl -n kube-system set env daemonset/cilium-envoy TCMALLOC_DISABLE=1
```

```shell
kubectl -n kube-system set env daemonset/cilium-envoy TCMALLOC_DISABLE-
```

```shell
kubectl -n kube-system rollout status daemonset cilium-envoy
```
