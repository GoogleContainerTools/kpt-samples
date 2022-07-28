# How was this package created

```sh

#The original manifests were generated from the helm chart as documented in the `getting started` guide on external-secrets website.
helm template external-secrets external-secrets/external-secrets -n external-secrets --create-namespace --set installCRDs=true > external-secrets.yaml

# Used `kubectl-slice` to split the uber manifests into individual files.
kubectl-slice -f external-secrets.yaml --template '{{.kind | lower}}-{{.metadata.name|dottodash}}.yaml' -o external-secrets

# Had to manually add the `external-secrets` namespace.

# Removed the `managed-by` helm label using a starlark function. The function is part of the package.
kpt fn eval -i starlark:v0.4.3 --fn-config fn-config-remove-labels.yaml

## Manually organized the files in three different components `controller`, `cert-controller` and `webhook`.
```
