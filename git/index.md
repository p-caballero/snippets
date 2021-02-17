# GIT

## Index

* [Clone a Repository](#Clone-a-Repository)
  * [Bitbucket](#Bitbucket)
  * [GitHub](#GitHub)
* [Rename a Local and Remote Git Branch](#Rename-a-Local-and-Remote-Git-Branch)
* [Specific User in Git Repository](#Specific-User-in-Git-Repository)

---

## Clone a Repository

### Bitbucket

```bash
git clone https://<user-name>@bitbucket.org/<company-name>/<repository-name>.git
```

### GitHub

```bash
git clone https://<user-name>@github.com/<owner-github-user-name>/<repository-name>.git
```

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
