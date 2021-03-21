# package.install

| Key          | Type   |  Optional   | Description |
| ------------ | ------ | ----------- | ----------- |
| `action`     | string | no          | Values: `package.install` |
| `name`       | string | no          | name of the target package to install |
| `list`       | string | yes         | list of multiple packages to install |
| `provider`   | string | yes         | OS specific package provider |
| `repository` | string | yes         | specific repository for a provider & package  |

## Examples

```yaml
actions:
  - action: package.install
    name: package_name
    provider: brew
    repository: EXAMPLE/tap
```