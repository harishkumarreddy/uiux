# Github setup
## Create SSH key and add to github
    command: ssh-keygen -t rsa -b 4096 -C "your_email@example.com"

1. follow the ref section **Generating a new SSH key**: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key
2. Add SSH to github: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account#adding-a-new-ssh-key-to-your-account
3. Test SSH connection: https://docs.github.com/en/authentication/connecting-to-github-with-ssh/testing-your-ssh-connection#testing-your-ssh-connection
4. Create a new repo
5. Clone the repo
```
git clone <repo_shh_url>
```

## git config
```
git config --global user.name "<Your Name>"
git config --global user.email "<Your Email>"
``` 

## git commands
```
git init  # initialize git repo
git remote add origin <repo_ssh_url>  # add remote repo
git add .  # add all files to staging area
git add <full/file/path> # add specific file to staging area
git status # check status of git repo
git commit -m "first commit" # commit changes to local repo
git branch -M main # rename branch
git push -u origin main # push changes to remote repo
git pull # pull changes from remote repo
git clone <repo_ssh_url> # clone repo

git checkout -b <branch_name> # create and checkout to new branch
git checkout <branch_name> # checkout to existing branch
git branch # list all branches
git branch -d <branch_name> # delete branch

git merge <branch_name> # merge branch to current branch
git rebase <branch_name> # rebase branch to current branch
git reset --hard <commit_hash> # reset to specific commit
git reset --hard HEAD~1 # reset to previous commit
git reset --hard HEAD~2 # reset to previous to previous commit

git log # list all commits

git stash # stash changes
git stash list # list all stashes
git stash apply # apply last stash
git stall drop # drop last stash
git stash pop # apply and drop last stash
git stash apply stash@{1} # apply specific stash
git stash drop stash@{1} # drop specific stash
git stash clear # drop all stashes

```