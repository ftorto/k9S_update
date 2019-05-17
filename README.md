# k9s_update

Simple Updater for [k9s](https://k9ss.io/) (github repo [here](https://github.com/derailed/k9s))

## Description

This script updates k9s binary by comparing current release with the latest available release in github releases
You can provide a specific version to fetch using the first parameter

The new version of k9s binary will be placed at `${HOME}/.local/bin`. Make sure this path is available in `$PATH`

## Installation

Create a link or copy `k9s_update` bash script to a location pointed by `$PATH` variable then you can call the script from anywhere.

Example:

```sh
cd k9s_update
ln -fs $(pwd)/k9s_update ${HOME}/.local/bin/k9s_update
```

## Usage

```sh
# Update to latest version
k9s_update

# Update to specific version
k9s_update 0.5.0
```
