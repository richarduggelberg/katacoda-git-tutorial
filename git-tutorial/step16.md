# Commit a little bit with git

Alright, so we want to skip that mean part. How do we do that? 

##### Just edit the file?

Well yeah, we could do that. In this case that makes sense. However, some time, you might need to commit just part of a file. Maybe you're being bad and working on several things at once. It maybe then also happens that these two "things" occupy the same file. We fix that in the staging. 

First reset the staging:

`git reset HEAD fibonacci.js`{{execute}}

Then, do the magic with the patch flag "-p":

git add -p fibonacci.js

### But this is really complicated so we're not doing it

Just leave the comment in the code. I guess it applies to us now, great work. 

#### Just know this:

It is possible to do partial commits in a number of ways. However, exactly how depends on the context and is also outside the scope of this tutorial. 

You know, you could try to remove the comment with the patch tool. Maybe that'll get you to really avoid working on several things at once in the future since then you might actually have to use it. ;)