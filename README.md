# Git and Github
Git and Github tutorial: https://youtu.be/tRZGeaHPoaw

### Configure Git
```
git config --global user.name "Muaaz Shoaib"
git config --global user.email muaazshoaib1670@gmail.com
git config --global init.default branch main
```

### Get help
```
git config -h
git help config
clear
```

### Initialize repository
```
cd c:/Users/muaaz/Desktop/Git
git init
```

### Git status
```
git status
```

### Track and untrack files
```
git add index.htm
git rm --cached index.htm
```

## Ignore files with .gitignore
```
# Step 1: Create a new file with the name .gitignore
# Step 2: Then ignores files you want to ignore

# ignore all .txt files
*.txt
```

### Track all files / add to staging
```
git add --all
git add -A
git add .
```

## Commit
```
git commit -m "first commit - committing all files to the repository"
```

## Change files and view differences
```
git diff
git add index.htm
git restore --staged index.htm
```

## Bypass staging and commit
```
git commit -a -m "updated text to free range"
```

## Delete / remove files
```
git rm "secret recipe.htm"
```

## Restore files
```
git restore --staged "secret recipe.htm"
git restore "secret recipe.htm"
```

## Rename files
```
git mv "KCC Logo.png" "Primary Logo.png"
git commit -m "changed the file name of image"
```

## View commit history with git log
```
git log
git log --oneline
```

## Amend commit
```
git commit -m "Changed file name to Primary Logo.png" --amend
```

## View changes in commits
```
git log -p
git help log
```

## Reset to previous commit
```
git reset 2139723
```

## Rebase git repository
```
git rebase -i --root
```

## Branches
```
git branch FixTemp
git branch
git switch FixTemp
git commit -a -m "updated temp for baking instruction"
git switch master
git switch -c UpdateText
```

## Merge branches
```
git merge -m "Merge fixtemp back to main" FixTemp
```
## Delete branch
```
git branch -d FixTemp
```

## Merge conflicts
```
git switch -c UpdateText
git commit -a -m "update index text"
git switch master
git commit -a -m "update index test"
git merge UpdateText # CONFLICT (content): Merge conflict in index.htm
git commit -a -m "update text on index"
```

## Typical Git flow
* Step 1: Create a new branch to create a new feature or remove a bug
* Step 2: Create a new feature or remove a bug
* Step 3: Merge a new branch with the main or master branch

## Set up GitHub account
https://github.com/signup

## Create new cloud repository
https://github.com/new

## Push local repo to GitHub
```
git remote add origin https://github.com/MuaazShoaib/learning-git-and-github.git
git branch -M main
git push -u origin main
git push --all
```

## Fetch and pull
```
git fetch
git merge
git pull
```
