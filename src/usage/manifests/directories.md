# Directories

| Key        | Type     | Description |
| ---------- | -------- | -------- |
| `action`   | string   | Values: `directory.copy`    |
| `from`     | string   | source file   |
| `to`       | string   | destination file   |

## Examples

```yaml
actions:
  - action: directory.copy
    from: SOURCE_DIR
    to: DESTINATION_DIR
```