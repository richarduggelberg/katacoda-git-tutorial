# Fetching

Alright! So now we're ready to get started on your super cool feature. Let’s take a look at how to get the repo from github to your local development environment. To do this, we’re going to use the `fetch` command which downloads objects and refs from a repo. This is the command you use when you want to see what everyone has worked on.
Go ahead and execute the following command to download the content of the repository:

`git fetch forked_repo`{{execute}}

#### Syntax 

Fetch all branches and the whole shebang: `git fetch <remote>`
Fetch a specfic branch: `git fetch <remote> <branch>`
Get everything for all remotes: `git fetch --all`