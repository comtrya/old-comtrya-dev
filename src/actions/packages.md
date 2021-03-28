# Packages

## Single Package

```yaml
actions:
  - action: package.install
    name: package_name
```

## Single Package from a specific repository

```yaml
actions:
  - action: package.install
    name: package_name
    provider: aptitude
    repository: ppa://
```

## Package List

```yaml
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
```

## Package List from a specific provider & repository

```yaml
actions:
  - action: package.install
    list:
      - package_name_1
      - package_name_2
    provider: brew
    repository: homebrew/cask
```

## Multi Action

```yaml
actions:
  - action: package.install
    name: package_name
    repository: homebrew/cask

  - action: package.install
    name: package_name
    repository: EXAMPLE/tap
```
