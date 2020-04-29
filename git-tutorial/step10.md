# Get latests changes from original repository.

Before we were interrupted by our colleague, we were in the process of making some changes. Let's go back and finish our work!

`git checkout new-feature`{{execute}}

Now there may have been some changes that are of interest in the original repository that we've forked from, let's take a look and get them.

Specify a new remote upstream repository that will be synced with the fork `git remote add upstream https://github.com/pojans/katacoda-tutorial.git`{{execute}}

Verify the new upstream repository you've specified for your fork. `git remote -v`{{execute}}

Fetch the branches and their respective commits from the upstream repository. Commits to master will be stored in a local branch, upstream/master. `git fetch upstream`{{execute}}

Awesome! You should be ready for your first merge conflict now! :)