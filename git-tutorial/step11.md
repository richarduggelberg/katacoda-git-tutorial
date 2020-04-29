# Your first merge (conflict)

Merging and conflicts are a part of everyday life of a developer or anyone working with git. They can be a pain in the butt if you don't them, but pretty soon you will become proficient enough to handle them with ease.

##### When do they arise? 
A merge will fail to start when Git sees there are changes in either the working directory or staging area of the current project. Git fails to start the merge because these pending changes could be written over by the commits that are being merged in.

##### How do we fix them?
You will see conflict dividers that look like this

```
<<<<<<< HEAD

content 

=======

content 

>>>>>>> new-feature
```

Git is pretty good at automatically resolving merge conflicts, but sometimes you have to get into the fray and figure out what sticks and what doesn't.

To merge a different branch into your active branch: `git merge <branch>`

Let's try merging and see what happends: `git merge upstream/master`{{execute}}

BOOM 💥. A conflict appears. Thanks, Git for letting us know about this!

To gain more information about the merge conflict, go ahead and run `git status`{{execute}}

We can see that the conflict lies in `both modified:   merge.txt`. Let's investigate further `cat merge.txt`{{execute}}.

Alright, so now that we know where the conflict is, go ahead and remove the conflict dividers in the text edior, or just click here: `echo "totally different content" > merge.txt`{{execute}}.

Now we can add merge.txt `git add merge.txt`{{execute}} and continue with our merge`git merge --continue`{{execute}}!


#### Top tips

If you really mess up, don't freak out! You can always run `git merge --abort` which will return you to the state prior to merging. Phew!

We only had one file to work with, but when you have multiple merge conflicts you can run `git diff` to view them all.





