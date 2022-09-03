# ledger-db

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] ledger-db`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree ledger-db`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init ledger-db
kpt live apply ledger-db --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
