GitHub account setup
====================

GitHub is a git repository hosting service that we'll use to publish projects and collect your finished submissions. You'll be assigned your own private repository for you to work on your code.

## Step 0: How do I... git?

If you're new to git, you may find it a bit overwhelming at first. But don't fear! There are many resources available online to help you learn. A list of recommended resources from GitHub is [here](https://help.github.com/articles/what-are-other-good-resources-for-learning-git-and-github). 

My favorite conceptual overview of git, which is tailored to computer scientists, is [here](http://eagain.net/articles/git-for-computer-scientists/). 

## Step 1: Create a GitHub account

If you don't already have a GitHub account, get one [here](https://github.com/join).

## Step 2: Notify us of your EID -> GitHub mapping

Once you've created your GitHub account, send an email to Pengxiang (pxcheng at cs dot utexas dot edu) with your GitHub account name and EID. He'll create a new private repository called `projects-[EID]` for you and grant you access to the `projects` private repository where project code will be posted.

## Step 3: Set up your projects repository

We will publish project descriptions, starter code, and unit tests to the 'projects' private repository. You will clone this repository to your private repo and push your changes there. We will collect your assignment by cloning your private repository.

### Clone the class projects repository into your repository.

From the command line of the computer where you installed git, clone the class-wide projects repository:

```bash
$ git clone https://github.com/ut-cs378-vision-2014fall/projects.git
```

You will need to enter your GitHub username and password when prompted.

This creates a local "clone" of the projects repository on your local machine. Next, we'll point this clone at your personal repository we set up for you in step 2, so your changes can be pushed there.

Next, change your working directory to the newly created projects repo:

```bash
$ cd homework/
```