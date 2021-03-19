# CLI-usage

`comtrya <manifest-directory> [FLAGS] [OPTIONS]`

## Flags

* `comtrya -h, --help` Prints help information

* `comtrya -V, --version` Prints help information

* `comtrya -v, --verbose` Debug & tracing mode (-v, -vv)

## Options

* `comtrya -m, --manifests <manifests>...` Run a subset of your manifests, comma separated list

## ARGS

* `comtrya <manifest-directory> ` Directory where manifests are locate

## Examples

```bash
# executes EXAMPLE manifest in current directory
comtrya . -m EXAMPLE
# executes EXAMPLE & TEST manifests in current directory
comtrya . -m EXAMPLE,TEST
# executes all manifestes in the apps directory
comtrya ./apps
``` 