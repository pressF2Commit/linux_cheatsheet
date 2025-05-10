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

## change Remote URL

```bash
# view current remote url
git remote -v
# set new git remote url
git remote set-url origin <GIT_URL>
# confirm new url
git remote -v
```

## undo latest commit

```bash
git reset --mixed HEAD~1
```

this keeps all staged commits staged and unstaged commits unstaged  
you can vary the number after ~ to vary how far back the commit you want to undo

## do not know what this is for.....(pray that you dont ever require this)

```bash
git reset --hard <commit_id>
```
