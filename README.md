# k8s-home-test

## ArgoCD

Add an app either via the web-ui, or via cmd line.

Example of cmd line:

```
argocd app create ingress-helm --repo https://github.com/dsschult/k8s-home-test --path ingress-helm --dest-server https://kubernetes.default.svc --dest-namespace default --helm-version v3 --auto-prune --sync-policy auto
```
