# Forking

Forking a repository is great! You can make all of the mistakes you want without affecting the original project, or you may want to take the project in a different direction.

What is forking generally used for? Most of the time, people fork projects to propose changes to someone else’s project.

That’s great! So how do I do this “fork” thing anyway? Forking is a simple process of finding the repository you want to fork on GitHub in the top right corner, click on Fork.

How to propose changes to a project. The workflow is something like this:

- Fork the repository
- Create a fix (commit changes)
- Submit a pull request to the original project

# Getting started

To get started with git, we have to do two things, first of all let's go ahead and configure git with our name and email. This is to identify who has done what on github.

`git config --global user.name "Sam Smith"`
`git config --global user.email sam@example.com`

Secondly, we need to create a local repository, we can do that by running the `git init` command.

Great! You're well on your way to become the person everyone asks for help with untangling their git-commit-hell at work. :)

# Remote

Alright, so we want to get the code from the remote repo to our local environment. We're going to have to, you've guessed it, setup something. The 'git remote -v' lists all currently configured remote repositories, which at this point is none.
To add our forked repo, go ahead and execute the following command:
```git
git remote add forked_repo https://github.com/richarduggelberg/katacoda-tutorial.git
```
Now if we run `git remote -v`, the output should be a little prettier. You're well on the way to actually look at some code now.

##### Syntax
Add: `git remote add <name> <url>`
Remove: `git remote rm <name>`
Rename: `git remote rename <old-name> <new-name>`

# Fetching

Alright! So now we're ready to get started on your super cool feature. Let’s take a look at how to get the repo from github to your local development environment. To do this, we’re going to use the `fetch` command which downloads objects and refs from a repo. This is the command you use when you want to see what everyone has worked on.
Go ahead and execute the following command to download the content of the repository:

```git
git fetch forked_repo
```
#### Syntax 

Fetch all branches and the whole shebang: `git fetch <remote>`
Fetch a specfic branch: `git fetch <remote> <branch>`
Get everything for all remotes: `git fetch --all`

# Cloning

The cloning command is awesome, not only does it get the repository, it also sets up the remote tracking for all of the branches. The syntax is:



git clone <repository url>

We are going to use the clone command to get our newly forked repo:

git clone https://github.com/richarduggelberg/katacoda-tutorial.git

Now what are some of the things that could go wrong? If you’re on a new machine and you haven’t authenticated yourself with github, you’re bound to get an error message stating:

“Fatal: Authentication Failed for: <repository url>”

Authentication is outside the scope of this tutorial, however, feel free to check out this awesome guide!
