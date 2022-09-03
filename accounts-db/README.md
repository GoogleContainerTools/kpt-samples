# accounts-db

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] accounts-db`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree accounts-db`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init accounts-db
kpt live apply accounts-db --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
