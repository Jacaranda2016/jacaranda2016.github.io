## About Myself

I just graduated with a Master degree in IT at the end of 2018 and started my career in the IT industry of Australia from Febrary of 2019. I found myself the beginner of the beginner of coding but I did not lose confidence. 

The purpose of this blog is to track the practices I performed on my way of self-evolution and record the progress I gained during this journey. I would appreciate it if you would like to give me some suggestions and advice. 

### Achievements
- setup personal tech blog using Github Pages. **done**
- Basics of Git. **doing**


## How to setup your personal blog using Github Pages?

* Create a new repository named {your_username}.github.io and that's all. This URL will be the default Github Page URL for you.
* If you create the repository using other name, it would be just a normal project not a Github Page.


## Basics of Git

### 1. What is Git?
- Git is designed for SCM (hence Source Code Management)
- Git is the most widely used modern Version Control System. 
- Git is actively maintained open source system. 
- Git is distributed. Having a distributed architecture, Git is an example of a DVCS (hence Distributed Version Control System). Rather than have only one single place for the full version history of the software as is common in once-popular version control systems like CVS or Subversion (also known as SVN), in Git, every developer's working copy of the code is also a repository that can contain the full history of all changes.

#### 1.1 Key features of Git: 
* Performance:
* Security: Secure Hash Algorithms; protections against secret alteration. 
* Flexibility:

### 2. Required Vocabulary
(The following contents is copied from the Tutorial)

#### 2.1 Repository:
Often referred to as a repo. A repository is the collection of files and folders that you’re using git to track. The repository consists of the entire history of your team’s changes to the project. It’s the big ole box you and your team throw your code into.

#### 2.2 Github:
The most popular remote storage solution for git repos. It also allows you to set access permissions for projects, track and submit bugs, accept feature requests, subscribe to repository notifications, and utilize a graphic interface, rather than use the command line. Repos default to public, but paid accounts can have private ones.

Other remote storage solutions or git platforms: Bitbucket、Google Code

#### 2.3 Commit:
Think of this as saving your work. When you commit to a repository, it’s like you’re gathering up the files as they exist at that moment and putting them in a time capsule. The commit will only exist on your local machine until it is pushed to a remote repository.

#### 2.4 Push:
Pushing is the bread to committing’s butter. Committing throws your files into the timecapsule, and pushing is what launches the capsule into space. Pushing is essentially syncing your commits to the cloud (again, probably Github). You can push multiple commits at once, too. You can work offline, commit lots of work, and then push it all up to Github when you’re back in civilization with that sweet, sweet wifi.

#### 2.5 Branch:
You can think of your git repo as a tree. The trunk of the tree, the software that goes live, is called the Master Branch. That’s the one that goes live. The branches of that tree are, well, called branches. These are separate instances of the code that offshoots from the main codebase. You might branch off for a single feature or an experimental patch. By branching, you can preserve the integrity of the software and have a way to revert if you do something totally bonkers. It also allows you to work on your task without stumbling into your team’s way (or they into yours).

how to create a branch?

#### 2.6 Merge:
When a branch is polished up, free of bugs (as far as you can tell, at least), and ready to become part of the primary codebase, it will get merged into the master branch. Merging is just what it sounds like: integrating two branches together. Any new or updated code will become an official part of the codebase. Anyone who branches off from the point of merging will have this code in their branch as well.

#### 2.7 Clone:
Cloning a repo is pretty much exactly what it sounds like. It takes the entire online repository and makes an exact copy of it on your local machine. You will need to do this for any number of reasons, not the least of which are starting in the middle of a project with a new team, swapping workstations, or starting over from a corrupted repo.

#### 2.8 Fork:
Forking is a lot like cloning, only instead of making a duplicate of an existing repo on your local machine, you get an entirely new repo of that code under your own name. This feature is mainly used for taking an existing codebase and going an entirely new direction with it, which happens a lot in open-source software; developers see a base idea that works, but want to go a different way with it. Forking allows that to happen. You can also play in another developer’s repository like it’s your own personal sandbox. And if you do something that you think they may like, you can make a pull request for it to be merged in.

#### ?? 2.9 Pull Request:??
A pull request is when you submit a request for the changes you have made (either on a branch or a fork) to be pulled (or merged) into the Master Branch of the repository. This is the big time. This is where the magic happens. If the pull request is approved, you will have officially contributed to the software, and Github will forever show exactly what you did. However, if the pull request is denied for any reason, the denier will be able to give feedback on why the request was turned down and what you can do to get it accepted.

### 3. How to interact with Git?
- Command line
- Graphical Git Clients ( e.g. Github website)
    * Examples of Graphical Git Clients: Source Tree, [Github Desktop](https://git-scm.com/downloads/guis)

### 4. How to install and config Git?
- Download Git from its official website:https://git-scm.com/downloads 
- Configuration via command line

This would be your identification.
$ git config --global user.name " your username"
$ git config --global user. email "your email address"

- Create repository locally or remotely (on Github)
$ git init project1
$ git cd project1

- Add files to repository
$ git add filename  #add to the staging area
$ git commit   -m "some message"  # commit to the local repository

- Push to the remote 
$ git push

### Other Git commands
$ git clone 
$ git pull  ??

