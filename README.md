# k8s-home-test

## ArgoCD

Add an app either via the web-ui, or via cmd line.

Helm v3 requires the cmd line for some reason:

```
argocd app create nginx-test2 --repo https://github.com/dsschult/k8s-home-test --path nginx-test2 --dest-server https://kubernetes.default.svc --dest-namespace default --helm-version v3 --auto-prune --sync-policy auto
```