# Forking

Forking a repository is great! You can make all of the mistakes you want without affecting the original project, or you may want to take the project in a different direction.

What is forking generally used for? Most of the time, people fork projects to propose changes to someone else’s project.

That’s great! So how do I do this “fork” thing anyway? Forking is a simple process of finding the repository you want to fork on GitHub in the top right corner, click on Fork.

How to propose changes to a project. The workflow is something like this:

- Fork the repository
- Create a fix (commit changes)
- Submit a pull request to the original project


# Fetching

Alright! So now you’ve created your fork and you're ready to get started on your super cool feature. Let’s take a look at how to get the repo from github to your local development environment. To do this, we’re going to use the `fetch` command which downloads objects and refs from a repo.

This is the command that we are going to execute to get the forked repo:

Syntax: `git fetch <remote>`
Example: `git fetch https://github.com/richarduggelberg/katacoda-tutorial.git`

##### Top tip
If you only want to fetch a specific branch, you can do so `git fetch <remote> <branch>`

# Remote
So what is this remote thing anyway? I keep getting these errors whenever I try to push my code, why isn't this working?!
When you fetch a repo, it does not set up the link to the remote repo, it only downloads the objects and refs. We want to set up the upstream link for our local copy of the forked repo to the original repo, so that every time there is a change in the original repo, we can get the latest commits. 
Did you follow that? Don't worry, here is how we are going to proceed:

Go ahead and enter the command `git remote -v` which should list the links to other repositories



# Cloning

The cloning command is awesome, not only does it get the repository, it also sets up the remote tracking for all of the branches. Trust, me, you’ll learn to appreciate this later on. The syntax is:

git clone <repository url>

We are going to use the clone command to get our newly forked repo:

git clone https://github.com/richarduggelberg/katacoda-tutorial.git

Now what are some of the things that could go wrong? If you’re on a new machine and you haven’t authenticated yourself with github, you’re bound to get an error message stating:

“Fatal: Authentication Failed for: <repository url>”

Authentication is outside the scope of this tutorial, however, feel free to check out this awesome guide!
