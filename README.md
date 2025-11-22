# Setup Uiua action

[![Stand With Ukraine](https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/badges/StandWithUkraine.svg)](https://stand-with-ukraine.pp.ua)
![Release](https://img.shields.io/github/v/release/fabasoad/setup-uiua-action?include_prereleases)
![functional-tests](https://github.com/fabasoad/setup-uiua-action/actions/workflows/functional-tests.yml/badge.svg)
![security](https://github.com/fabasoad/setup-uiua-action/actions/workflows/security.yml/badge.svg)
![linting](https://github.com/fabasoad/setup-uiua-action/actions/workflows/linting.yml/badge.svg)

This action installs [Uiua](https://www.uiua.org/) language interpreter.

## Supported OS

<!-- prettier-ignore-start -->
| OS      |                    |
|---------|--------------------|
| Windows | :white_check_mark: |
| Linux   | :white_check_mark: |
| macOS   | :white_check_mark: |
<!-- prettier-ignore-end -->

## Prerequisites

None.

## Inputs

```yaml
- uses: fabasoad/setup-uiua-action@v0
  with:
    # (Optional) Uiua version. Defaults to "latest".
    version: "0.17.3"
    # (Optional) If "false" skips installation if Uiua is already installed.
    # If "true" installs Uiua in any case. Defaults to "false".
    force: "false"
    # (Optional) GitHub token that is used to send requests to GitHub API such
    # as downloading asset. Defaults to the token provided by GitHub Actions
    # environment.
    github-token: "${{ github.token }}"
```

## Outputs

<!-- prettier-ignore-start -->
| Name      | Description                       | Example |
|-----------|-----------------------------------|---------|
| installed | Whether Uiua was installed or not | `true`  |
<!-- prettier-ignore-end -->

## Contributions

![Alt](https://repobeats.axiom.co/api/embed/d84692b9fb0ec9a6f1b0a28d840e66fb7361e0b1.svg "Repobeats analytics image")
