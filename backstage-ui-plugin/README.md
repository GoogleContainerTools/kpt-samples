# backstage-ui-plugin

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get REPO_URI[.git]/PKG_PATH[@VERSION] backstage-ui-plugin`
Details: https://kpt.dev/reference/cli/pkg/get/

### View package content
`kpt pkg tree backstage-ui-plugin`
Details: https://kpt.dev/reference/cli/pkg/tree/

### Apply the package
```
kpt live init backstage-ui-plugin
kpt live apply backstage-ui-plugin --reconcile-timeout=2m --output=table
```
Details: https://kpt.dev/reference/cli/live/
