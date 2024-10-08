# Dotnet webbapp

A Kustomize example.

## Sealed secrets

Creating a sealed secret allows you to commit it in git.

```sh
k config use-context <context>
kubeseal --scope strict --controller-name sealed-secrets --controller-namespace sealed-secrets --format yaml < secret-appsettings.yaml > sealed-secret-appsettings.yaml
```
