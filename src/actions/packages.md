# Packages

| Key          | Type   |  Optional   | Description |
| ------------ | ------ | ----------- | ----------- |
| `action`     | string | no          | Values: `package.install`    |
| `name`       | string | no          |
| `list`       | string | yes         |
| `provider`   | string | yes         | renderes files using [context providers](misc/context-provider.md), Values: `true` or `false`  |
| `repository` | string | yes         | octal permissions   |

## Examples

```yaml
# Single package
actions:
  - action: package.install
    name: package_name
# Single Package from a specific provider
actions:
  - action: package.install
    name: package_name
    provider: aptitude
# Multiple packages in a list
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
# Multiple packages from a specific repository
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
    repository: homebrew/cask
# Multiple packages
actions:
  - action: package.install
    name: package_name
    repository: homebrew/cask

  - action: package.install
    name: package_name#
    provider: brew
    repository: EXAMPLE/tap

    - action: package.install
    name: package_name
    provider: winget
```
