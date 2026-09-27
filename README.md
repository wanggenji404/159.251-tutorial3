# tutorial3

[![Java CI with Maven](https://github.com/wanggenji404/159.251-tutorial3/actions/workflows/build.yml/badge.svg)](https://github.com/wanggenji404/159.251-tutorial3/actions/workflows/build.yml)

159.251 Software Design and Construction — Tutorial 3: Continuous Integration (CI) using GitHub Actions.

A small Maven project used to practise wiring a local repository, a remote GitHub repository and a
CI service together. `Calc` provides `add` and `subtract`; `CalcTest` verifies them with JUnit 5.

## Build and test locally

```bash
mvn clean test
```

## Continuous integration

`.github/workflows/build.yml` runs `mvn clean test` on every push, so each commit shows up in the
repository's **Actions** tab with a red or green status.
