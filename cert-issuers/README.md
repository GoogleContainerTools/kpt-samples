# cert-issuers

## Description
Package contains manifests for certificate issuers.

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] cert-issuers`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree cert-issuers`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init cert-issuers
kpt live apply cert-issuers --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
