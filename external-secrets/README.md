# external-secrets

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] external-secrets`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree external-secrets`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init external-secrets
kpt live apply external-secrets --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/

