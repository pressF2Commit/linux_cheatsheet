# User Configuration

## to add the user.name and user.email from global git config;

```bash
git config --global --add user.name <username>
git config --global --add user.email <email>
```

## to remove the user.name and user.email from global git config;

```bash
git config --global --unset-all user.name
git config --global --unset-all user.email
```

# Git URL Configuration

## change Remote URL

```bash
# view current remote url
git remote -v
# set new git remote url
git remote set-url origin <GIT_URL>
# confirm new url
git remote -v
```

# Git Reset

## undo latest commit

```bash
git reset --mixed HEAD~<number_of_commits_to_roll_back>
# this keeps all staged commits staged and unstaged commits unstaged.
```

```bash
git reset --hard <commit_id>
# do not know what this is for.....(pray that you dont ever require this)
```

# Git Log

## visual diff summary

```bash
git log -n <number> --stat
# shows summary of total additions and removals in the previous <number> number of commits
```
