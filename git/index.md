# GIT

## Index

* [Rename a Local and Remote Git Branch](#Rename-a-Local-and-Remote-Git-Branch)
* [Specific User in Git Repository](#Specific-User-in-Git-Repository)

## Rename a Local and Remote Git Branch

```bash
git checkout <old_name>
git branch -m <new_name>
git push origin -u <new_name>
git push origin --delete <old_name>
```

## Specific User in Git Repository

```bash
cd <repository_folder>
git config user.name "<name>"
git config user.email "<email>"
```
