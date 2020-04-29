# Commit

Okay, so now we are at the last step, actually committing. (Well, that last that we can perform in this tutorial)

To commit, run this: `git commit -m "feature: use dynamic programming for fibonacci calculation"`{{execute}}

Alright, so now it's done.

Wait.

You know what.

Adding "//Also, whoever wrote this is bad at coding" is actually kind of mean. We shouldn't be mean. 

Let's take back that commit.

We do this with what's called a soft reset:

`git reset --soft HEAD^`{{execute}}

#### Soft?


