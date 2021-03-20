# Examples

This is WIP.


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

actions:
  - action: file.copy
    from: SOURCE_FILE
    to: DESTINATION_FILE
    template: false
```
