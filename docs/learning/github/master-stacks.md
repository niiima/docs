moving committed (but not pushed) changes to a new branch after pull
Asked Question

I've done a fair bit of work ("Your branch is ahead of 'origin/master' by 37 commits.") which really should have gone into its own branch rather than into `master`.  These commits only exist on my local machine and have not been pushed to `origin`, but the situation is complicated somewhat in that other devs have been pushing to `origin/master` and I've pulled those changes.

How do I retroactively move my 37 local commits onto a new branch?  Based on the docs, it appears that `git rebase --onto my-new-branch master` or `...origin/master` should do this, but both just give me the error "fatal: Needed a single revision".  `man git-rebase` says nothing about providing a revision to `rebase` and its examples do not do so, so I have no idea how to resolve this error.

(Note that this is **not** a duplicate of https://stackoverflow.com/questions/1394797/git-how-to-move-existing-work-to-new-branch or https://stackoverflow.com/questions/556923/git-how-to-merge-my-local-working-changes-into-another-branch as those questions deal with uncommitted changes in the local working tree, not changes which have been committed locally.)

###Answer
This should be fine, since you haven't pushed your commits anywhere else yet, and you're free to rewrite the history of your branch after `origin/master`.  First I would run a `git fetch origin` to make sure that `origin/master` is up to date.  Assuming that you're currently on `master`, you should be able to do:

    git rebase origin/master

... which will replay all of your commits that aren't in `origin/master` onto `origin/master`.  The default action of rebase is to ignore merge commits (e.g. those that your `git pull`s probably introduced) and it'll just try to apply the patch introduced by each of your commits onto `origin/master`.  (You may have to resolve some conflicts along the way.)  Then you can create your new branch based on the result:

    git branch new-work

... and then reset your `master` back to `origin/master`:

    # Use with care - make sure "git status" is clean and you're still on master:
    git reset --hard origin/master

When doing this kind of manipulating branches with `git branch`, `git reset`, etc. I find it useful to frequently look at the commit graph with `gitk --all` or a similar tool, just to check that I understand where all the different refs are pointing.

Alternatively, you could have just created a topic branch based on where your master is at in the first place (`git branch new-work-including-merges`) and then reset `master` as above.  However, since your topic branch will include merges from `origin/master` and you've not pushed your changes yet, I'd suggest doing a rebase so that the history is tidier.  (Also, when you eventually merge your topic branch back to master, the changes will be more obvious.)