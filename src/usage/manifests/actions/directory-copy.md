# Directories

| Key        | Type     |  Optional   | Description |
| ---------- | -------- | ----------- | ----------- |
| `action`   | string   | no          | Values: `directory.copy` |
| `from`     | string   | no          | source file |
| `to`       | string   | no          | destination file |

## Examples

```yaml
actions:
  - action: directory.copy
    from: SOURCE_DIR
    to: DESTINATION_DIR
```