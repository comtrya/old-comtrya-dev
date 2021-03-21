# file.copy

| Key        | Type     |  Optional   | Description |
| ---------- | -------- | ----------- | -------- |
| `action`   | string   | no          | Values: `file.copy` |
| `from`     | string   | no          | source file |
| `to`       | string   | no          | destination file |
| `template` | bool     | yes         | renderes files using [context providers](misc/context-provider.md), Default: `false` |
| `chmod`    | string   | yes         | octal permissions |

## Examples

```yaml
actions:
  - action: file.copy
    from: config
    to: "{{ user.home_dir }}/.config/git/config"
    template: true
    chmod: 644
```