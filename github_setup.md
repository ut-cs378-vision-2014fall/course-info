GitHub account setup
====================

GitHub is a git repository hosting service that we'll use to publish projects and collect your finished submissions. You'll be assigned your own private repository for you to work on your code.

## Step 0: How do I... git?

If you're new to git, you may find it a bit overwhelming at first. But don't fear! There are many resources available online to help you learn. A list of recommended resources from GitHub is [here](https://help.github.com/articles/what-are-other-good-resources-for-learning-git-and-github). 

My favorite conceptual overview of git, which is tailored to computer scientists, is [here](http://eagain.net/articles/git-for-computer-scientists/). 

## Step 1: Install git

### Mac OS X

I recommend installing the GitHub Mac application, which provides the [option to install the command-line git program](https://github.com/blog/1510-installing-git-from-github-for-mac).

### Linux

Your Linux distribution almost certainly has a git package available. For example, to install git on Ubuntu, just use:

```bash
$sudo apt-get install git-core
```

### Windows

Windows is a bit trickier, because it's native command-line environment is not UNIX-like. You can install the [GUI GitHub for Windows](https://windows.github.com/) app and probably accomplish all of the below using its user interface, but I haven't tried.

## Step 1: Create a GitHub account

If you don't already have a GitHub account, get one [here](https://github.com/join).

## Step 2: Notify us of your EID -> GitHub mapping

Once you've created your GitHub account, send an email to Pengxiang (pxcheng at cs dot utexas dot edu) with your GitHub account name and EID. He'll create a new private repository called `projects-[EID]` for you and grant you access to the `projects` private repository where project code will be posted. He'll send confirmation when that's done, and then you can proceed.

## Step 3: Set up your projects repository

We will publish project descriptions, starter code, and unit tests to the 'projects' class repository. You will clone this repository to your private repo and push your changes there. We will collect your assignment by cloning your private repository.

### Clone the class projects repository

From the command line of the computer where you installed git, clone the class-wide projects repository:

```bash
$ git clone https://github.com/ut-cs378-vision-2014fall/projects.git
```

You will need to enter your GitHub username and password when prompted.

This creates a local "clone" of the projects repository on your local machine.

Next, change your working directory to the newly created projects repo:

```bash
$ cd projects/
```

### Configure pushes to your private repository

You'll complete your projects by making changes in `projects` and pushing them to your private repo. To make this work, we need to set up your private repo as a [remote](http://git-scm.com/book/en/Git-Basics-Working-with-Remotes).

Initially, your clone will be configured with the master projects repo as its only remote:

```bash
$ git remote -v
origin	https://github.com/ut-cs378-vision-2014fall/projects.git (fetch)
origin	https://github.com/ut-cs378-vision-2014fall/projects.git (push)
```

You'll reconfigure the remotes so you can push your changes to your private projects repo. First, rename the master projects remote `upstream`:

```bash
$ git remote rename origin upstream
```

You can see the effect this has by listing your remotes again:

```bash
$ git remote -v
upstream	https://github.com/ut-cs378-vision-2014fall/projects.git (fetch)
upstream	https://github.com/ut-cs378-vision-2014fall/projects.git (push)
```

Now, replace `origin` with your private repository:

```bash
$ git remote add origin https://github.com/ut-cs378-vision-2014fall/projects-[EID].git
```

You can now see the new remote:

```bash
$ git remote -v
origin	https://github.com/ut-cs378-vision-2014fall/projects-[EID].git (fetch)
origin	https://github.com/ut-cs378-vision-2014fall/projects-[EID].git (push)
upstream	https://github.com/ut-cs378-vision-2014fall/projects.git (fetch)
upstream	https://github.com/ut-cs378-vision-2014fall/projects.git (push)
```

Finally, push the contents of your clone to your private repository:

```bash
$ git push -u origin master
```

You should see output that's something like:

```bash
Counting objects: 19, done.
Delta compression using up to 8 threads.
Compressing objects: 100% (10/10), done.
Writing objects: 100% (19/19), 1.86 KiB | 0 bytes/s, done.
Total 19 (delta 1), reused 0 (delta 0)
To https://github.com/ut-cs378-vision-2014fall/projects-[EID].git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
```

Now, any pushes you make from your local repo will go to your private projects repo on GitHub by default with a mere `git push`:

```bash
$ git push
Everything up-to-date
```

### Getting updated `projects` content

During the class, new project content will be published to the master `projects` repo. You can fetch this updated content using `git pull`:

```bash
$ git pull upstream master
```

As long as you didn't edit any of the master files (e.g. unit tests) as described in the project instructions, you shouldn't face any merge conflicts.

### Submitting your work

When you've complete a project, you need to push your finished work to your private repository on GitHub for grading.

Remember that git is a distributed version control system, so `git commit` on your local machine has no effect on your GitHub repository. For changes to show up there, you need to `git push`. Check that the code reflected on the GitHub website reflects what you want graded before the project submission deadline.

###### These instructions are heavily inspired by [this guide](https://raw.githubusercontent.com/ComS342-ISU/course-info/master/guides/course-setup.md).
