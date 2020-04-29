# Remote

Alright, so we want to get the code from the remote repo to our local environment. We're going to have to, you've guessed it, setup something. The 'git remote -v' lists all currently configured remote repositories, which at this point is none.
To add our forked repo, go ahead and execute the following command:

`git remote add forked_repo https://github.com/richarduggelberg/katacoda-tutorial.git`{{execute}}

Now if we run `git remote -v`{{execute}}, the output should be a little prettier. You're well on the way to actually look at some code now.