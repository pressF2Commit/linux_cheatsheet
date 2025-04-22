# to add the user.name and user.email from global git config;
git config --global --add user.name "your_username"
git config --global --add user.email "your_email"

# to remove the user.name and user.email from global git config;
git config --global --unset-all user.name
git config --global --unset-all user.email

# change Remote URL
git remote -v -> view current remote url
git remote ser-url origin <GIT_URL> -> set new git remote url
git remote -v -> confirm new url

# undo latest commit while keeping all staged commits staged and unstaged commits unstaged
# you can vary the number after ~ to vary how far back the commit you want to undo
git reset --mixed HEAD~1

# do not know what this is for.....(pray that you dont ever require this)
git reset --hard <commit_id>
