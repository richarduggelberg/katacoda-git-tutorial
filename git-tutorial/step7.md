# Make your changes 1
Branching is a way for you to work on different features in the code at the same without destroying the master branch. The basic idea is to create a feature branch, do some work, then integrate it into the master branch. You can see a branch as a clean slate where you can do whatever you want without ruining someone elses work.

Let's checkout the branches that exist, we can do that by running the command `git branch`. The only branch for now is the master branch, you can create a new branch by typing `git branch <new branch name>` and then `git checkout <new branch name>` OR we can just type `git checkout -b <new branch name>` to do the same thing. Go ahead and create a branch with the name 'new-feature'.

```git
git checkout -b new-feature
```{{execute}}

Which style do you think is the best? Let me know in the comment section below, be sure to like and subscribe while you're at it.