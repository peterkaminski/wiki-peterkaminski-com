# Git Snippets

## Stop Tracking A File

Source:
- [How to make Git “forget” about a file that was tracked but is now in .gitignore](https://stackoverflow.com/a/1274447)

Remove the file from the index:

```shell
git rm --cached <file>
```

Remove a whole directory:

```shell
git rm -r --cached <folder>
```

WARNING: While this will not remove the physical file from your local machines, it will remove the files from other developers machines on next `git pull`.

## Change Upstream URL

Perhaps to change from https: to SSH or vice versa.

```shell
git remote set-url origin <url>
```