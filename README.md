# sample-argocd-deploy

An example of how a k8s cluster could be provisioned

Hook up your ArgoCD instance to this repo so that it can scan for kustomize and helm manifests.

* Kustomize: */overlays/<env>
* Helm: */values/<env>.yaml

## Apps

argo-workflows

```
helm chart update
helm search repo argo/argo-workflows --versions
NAME               	CHART VERSION	APP VERSION	DESCRIPTION
argo/argo-workflows	0.42.5       	v3.5.11    	A Helm chart for Argo Workflows
...
```
