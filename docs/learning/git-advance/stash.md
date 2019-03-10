#git-stash why and when
Stash is just a convenience method. Since branches are so cheap and easy to manage in git, I personally almost always prefer creating a new temporary branch than stashing, but it's a matter of taste mostly.


The one place I do like stashing is if I discover I forgot something in my last commit and have already started working on the next one in the same branch:

# Assume the latest commit was already done
# start working on the next patch, and discovered I was missing something

# stash away the current mess I made
git stash save

# some changes in the working dir

# and now add them to the last commit:
git add -u
git commit --ammend

# back to work!
git stash pop

or If I work on branch A and suddenly need to work on branch B before being ready with a commit on branch A, I stash my changes on A, checkout B, do my work there, then checkout A and apply the stash.