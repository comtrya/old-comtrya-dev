# Styleguide

This is the official styleguide for `Comtrya`.

## Use yaml instead of yml for manifests

[YAML.org - FAQ](https://yaml.org/faq.html)

## Use the correct order of keywords

- `actions:`
- `depends:`

## Add spaces between tasks

```yaml
actions:
  - action: package.install
    name: package1_name

  - action: package.install
    name: package2_name
```

## Use 2 spaces for indentation

```yaml
actions:
  - name: firefox-developer-edition
    action: package.install
    variant:
      ubuntu:
        name: firefox
        repository: ppa:mozillateam/firefox-next
```

## Wrap vars in spaces

```yaml
actions:
  - action: file.copy
    from: default.yaml
    to: "{{ user.home_dir }}/default.yaml"
    template: false
```

