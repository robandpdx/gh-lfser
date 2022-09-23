# gh-lfser

This GitHub CLI extension will migrate a repo to LFS. WARNING: This is destructive!! The repo pull requests will be outdated after this operation because the commit shas will change as a result of the history being rewritten.

This will:
1. Clone the repo
1. Migrate files with the provided extension to LFS
1. Commit lfs-mapping.csv file on default branch showing old sha to new sha mapping
1. Force push all repo branches back to the origin
1. Forge push all tags

## Permissions
You need write access to the repo. The repo needs to allow force pushes to all branches. It's probably best to disable any branch protection rules that may be in place before running this.

## Install
`gh extension install robandpdx/gh-lfser`  

## Upgrade
`gh extension upgrade robandpdx/gh-lfser`  

## Usage
`gh lfser --extensions <extensions> --repo <repo>`  
`gh lfser --help`  

## Example
`gh lfser --extensions "*.dmg,*.png,*.jpg" --repo robandpdx/el-repo-mas-grande`  