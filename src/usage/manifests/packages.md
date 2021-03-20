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
actions:
  - action: package.install
    name: package_name#
    provider: brew
    repository: EXAMPLE/tap
```