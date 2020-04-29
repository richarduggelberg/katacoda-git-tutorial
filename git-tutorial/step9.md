# Annoying coworker. Interrupted workflow.

So your coworker comes by and wants you to take a look at his code which has a bug and he needs help sorting it out.

Now if we want to switch to his branch, we need to run `git checkout coworker-branch`{{execute}}.

But wait! What is this?! Since we haven't pushed our code to the repo yet, we have to stash our changes.

You can go ahead and stash the changes in a dirty working directory away `git stash`. Now all the changes that were made are safe, and we can switch to his branch. `git checkout coworker-branch`{{execute}}

Take a look in fibonacci.js if you can spot the error?

#### Examples

To list all the stashed changes
`git stash -list`

Re-apply most recently stashed changes
`git stash pop`




