# swap-space

[![Current Tag](https://img.shields.io/github/v/tag/actionhippie/swap-space?sort=semver)](https://github.com/actionhippie/swap-space) [![Testing Build](https://github.com/actionhippie/swap-space/workflows/testing/badge.svg)](https://github.com/actionhippie/swap-space/actions/workflows/testing.yml)

[GitHub Action](https://github.com/features/actions) to resize or create swap space.

## Usage

```yml
name: Example

on:
  - push
  - pull_request

jobs:
  test:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v2

      - uses: actionhippie/swap-space@v1
        with:
          size: 10G
```

## Inputs

### `size`

Swap size in fallocate format, defaults to `10G`

### `path`

Swap path if no swap exists, defaults to `/swapfile`

## Outputs

None

## Security

If you find a security issue please contact thomas@webhippie.de first.

## Contributing

Fork -> Patch -> Push -> Pull Request

## Authors

* [Thomas Boerger](https://github.com/tboerger)

## License

Apache-2.0

## Copyright

```console
Copyright (c) 2023 Thomas Boerger <thomas@webhippie.de>
```
