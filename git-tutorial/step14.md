# Commit

Okay, so now we are at the last step, actually committing. (Well, that last that we can perform in this tutorial)

To commit, run this: `git commit -m "feature: use dynamic programming for fibonacci calculation"`{{execute}}

Alright, so now it's done.

Wait.

You know what.

Adding "//Also, whoever wrote this is bad at coding" is actually kind of mean. We shouldn't be mean. 

Let's take back that commit.

We do this with what's called a soft reset:

`git reset --soft HEAD~1`{{execute}}

#### Soft?

"Soft" here means that we only revert the commit. All changes are still there and staged. Running "git status" would show that. If our reset was "--hard", then all the changes would be sent straight to the trash. Be careful with that. There is also the default, --mixed. Simply put that removes the "commit" and the "add".

#### HEAD?

The "HEAD~1" means that we go back 1 commit from the current head.
