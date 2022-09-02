# anthos-app

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] anthos-app`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree anthos-app`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init anthos-app
kpt live apply anthos-app --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
