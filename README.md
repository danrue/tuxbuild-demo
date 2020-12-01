# Building Linux with Clang, GitHub Actions, and TuxBuild

This repository demonstrates basic usage of tuxbuild integration with github
actions to build the Linux kernel with several versions of clang.

## Set Up

Fork this repo.

In the fork, navigate to "Settings->Secrets" and add a variable named
`TUXBUILD_TOKEN` with the contents of your tuxbuild token from
tuxbuild@linaro.org.

## Usage

To manually trigger a run, nagivate to "Actions", click on "Clang Linux Builds"
under "All workflows", and click "Run workflow".

The workflow will also run automatically per the cron schedule in
[.github/workflows/builds.yml](.github/workflows/builds.yml].
