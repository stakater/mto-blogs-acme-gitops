# mto-blogs-acme-gitops

The GitOps repository of tenant `acme`, for the tutorial
[Hands-on: tenants on OpenShift, carried into Argo CD](https://github.com/stakater/mto-blogs/tree/main/06-try-it-tenants-and-argocd).

- `hello.yaml`: a small web server. The Applications `hello` and
  `hello-prod` sync it into `acme-dev` and `acme-prod`.
- `quota/`: a ResourceQuota. Argo CD refuses it, because Multi-Tenant
  Operator owns the quotas in tenant namespaces.
