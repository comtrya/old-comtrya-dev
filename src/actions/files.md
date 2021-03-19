# Files

| Key        | Type     | Description |
| ---------- | -------- | -------- |
| `action`   | string   | Values: `file.copy`    |
| `from`     | string   | source file   |
| `to`       | string   | destination file   |
| `template` | bool     | renderes files using [context providers](misc/context-provider.md), Values: `true` or `false`  |
| `chmod`    | int      | octal permissions   |

## Examples

```yaml
actions:
  - action: file.copy
    from: SOURCE_FILE
    to: DESTINATION_FILE
    template: false

  - action: file.copy
    from: config
    to: "{{ user.home_dir }}/.config/git/config"
    template: true
    chmod: 644
```