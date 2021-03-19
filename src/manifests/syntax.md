# Syntax

```yaml
depends:
  - manifest_name

actions:
  - action: action_name
  
  - action: action_name

  - action: package.install
    name: package_name
    repository: homebrew/cask

  - action: package.install
    name: package_name
    provider: brew
    repository: EXAMPLE/tap
```