Git Branching - Remote Branches

Remote branches are references (pointers) to the state of branches in your remote repositories. They’re local branches that you can’t move; they’re moved automatically for you whenever you do any network communication. Remote branches act as bookmarks to remind you where the branches on your remote repositories were the last time you connected to them.


They take the form (remote)/(branch). For instance, if you wanted to see what the master branch on your origin remote looked like as of the last time you communicated with it, you would check the origin/master branch. If you were working on an issue with a partner and they pushed up an iss53 branch, you might have your own local iss53 branch; but the branch on the server would point to the commit at origin/iss53.

This may be a bit confusing, so let’s look at an example. Let’s say you have a Git server on your network at git.ourcompany.com. If you clone from this, Git’s clone command automatically names it origin for you, pulls down all its data, creates a pointer to where its master branch is, and names it origin/master locally. Git also gives you your own local master branch starting at the same place as origin’s master branch, so you have something to work from.

https://git-scm.com/book/en/v2/images/remote-branches-1.png

rest:
 https://git-scm.com/book/id/v2/Git-Branching-Remote-Branches

###How to make a new branch that tracks remote branches

```$ git checkout --track origin/dev
Branch dev set up to track remote branch dev from origin.
Switched to a new branch 'dev'```

I can also just edit the .git/config file, but it seems there should be an easier way.

### How do I make an existing branch track a remote branch?
Given a branch `foo` and a remote `upstream`:

**As of Git 1.8.0:**

    git branch -u upstream/foo

Or, if local branch `foo` is not the current branch:

    git branch -u upstream/foo foo

Or, if you like to type longer commands, these are equivalent to the above two:

    git branch --set-upstream-to=upstream/foo

    git branch --set-upstream-to=upstream/foo foo

**As of Git 1.7.0:**

    git branch --set-upstream foo upstream/foo

    

