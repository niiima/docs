Deleting local branches in Git
$ git branch -d feature/login
Using the "-d" flag, you tell "git branch" which item you want to delete.

Note that you might also need the "-f" flag if you're trying to delete a branch that contains unmerged changes. Use this option with care because it makes losing data very easy.

Deleting remote branches in Git
To delete a remote branch, we do not use the "git branch" command - but instead "git push" with the "--delete" flag:

$ git push origin --delete feature/login

https://www.derekgourlay.com/blog/git-when-to-merge-vs-when-to-rebase/