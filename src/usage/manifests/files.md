# Files

| Key        | Type     | Description |
| ---------- | -------- | -------- |
| `action`   | string   | Values: `file.copy`    |
| `from`     | string   | source file   |
| `to`       | string   | destination file   |
| `template` | bool     | renderes files using [context providers](misc/context-provider.md), Values: `true` or `false`  |
| `chmod`    | string   | octal permissions   |

## Examples

```yaml
actions:
  - action: file.copy
    from: config
    to: "{{ user.home_dir }}/.config/git/config"
    template: true
    chmod: 644
```