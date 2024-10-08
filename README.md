# Sample Argocd deploy repo

An example of how a k8s cluster could be provisioned

Hook up your ArgoCD instance to this repo so that it can scan for kustomize and helm manifests.

* Kustomize: */overlays/<env>
* Helm: */values/<env>.yaml

Building apps could trigger a new image tag to be committed in this repo.
