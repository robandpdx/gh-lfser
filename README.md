# gh-lfser

This GitHub CLI extension will migrate a repo to LFS. WARNING: This is destructive!! This will clone the repo, migrate it to LFS, then force push the repo back to it's origin.

## Install
`gh extension install robandpdx/gh-lfser`  

## Upgrade
`gh extension upgrade robandpdx/gh-lfser`  

## Usage
`gh lfser --extensions <extensions> --repo <repo>`  
`gh lfser --help`  

## Example
`gh lfser --extensions "*.dmg,*.png,*.jpg" --repo robandpdx/el-repo-mas-grande`  