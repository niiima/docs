git remote add origin <remote_repo_url>
git push --all origin
If you want to set all of your branches to automatically use this remote repo when you use git pull, add --set-upstream to the push:

git push --all --set-upstream origin