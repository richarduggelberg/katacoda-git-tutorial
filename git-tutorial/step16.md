# Commit a little bit with git

Alright, so we want to skip that mean part. How do we do that? 

##### Just edit the file?

Well yeah, we could do that. In this case that makes sense. However, some time, you might need to commit just part of a file. Maybe you're being bad and working on several things at once. It maybe then also happens that these two "things" occupy the same file. We fix that in the staging. 

First reset the staging:

`git reset HEAD <filename>`{{execute}}

Then, do the magic with the patch flag "-p":

`git add -p <filename>`{{execute}}

Now, it all might seem a bit complicated since you have a lot of options (see list, down below). What git does here is that it divides the code into "hunks". If we wanted to stage the current hunk we'd type "y", if not then "n". However, we want to only remove a small part of the current hunk so we'll have to do this manually. Type "e" for edit to manually edit the staging. The interactive guide should tell you to just erase the line that we don't want to stage. 

After that, exit the interative mode and commit the changes ???? TODO