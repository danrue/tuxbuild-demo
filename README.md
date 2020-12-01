# Building Linux with Clang, GitHub Actions, and TuxBuild

[![Actions Status](https://github.com/danrue/tuxbuild-demo/workflows/Clang%20Linux%20Builds/badge.svg)](https://github.com/danrue/tuxbuild-demo/actions)

This repository demonstrates basic usage of tuxbuild integration with github
actions to build the Linux kernel with several versions of clang.

## Contents of this Repo

- [tuxbuild.yml](tuxbuilds.yml): TuxBuild Build Set Definition (list of build
  combinations, read by tuxbuild's cli)
- [.github/workflows/builds.yml](.github/workflows/builds.yml): GitHub Actions
  Job Definition (how to call tuxbuild to perform all the builds)

## Set Up

Fork this repo.

In the fork, navigate to "Settings->Secrets" and add a variable named
`TUXBUILD_TOKEN` with the contents of your tuxbuild token from
tuxbuild@linaro.org.

Modify the path in the build badge link at the top of this file.

## Usage

To manually trigger a run, nagivate to "Actions", click on "Clang Linux Builds"
under "All workflows", and click "Run workflow".

The workflow will also run automatically per the cron schedule in
[.github/workflows/builds.yml](.github/workflows/builds.yml).
