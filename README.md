# intro-git

Tasks
=====

1. Fork this repository
2. Clone the fork (not the main repository)
3. Add a remote "upstream" to point to this repository

Start addressing some [issues](https://github.com/jasmainak/intro-git/issues)!

6. Make a Branch
7. Make a commit on your branch
8. Push to origin
9. Make your first pull request!

Cheatsheet
==========

Setting up
----------

Configure your set up using the following commands:

	$ git config --global user.name "Your Name"
	$ git config --global user.email youremail@example.com
	$ git config --global color.ui auto

Remember to use the same email address that you use for github.

Branching
---------

To check the branch you are on:

	$ git branch -v

To make a new branch from current branch:

	$ git branch cool-feature

To change to ``cool-feature`` branch:

	$ git checkout cool-feature

Deleting the branch ``cool-feature``:

	$ git checkout master (or any branch other than cool-feature)
	$ git branch -D cool-feature

Making a commit
---------------

To check the changes since last commit:

	$ git diff

To add a file to the staging area:

	$ git add <filename>

To check which files are staged, tracked, or untracked:

	$ git status

To make a commit:

	$ git commit -m "My new feature"

To check history of commits:

	$ git log

Working collaboratively
-----------------------

Get list of remotes:

	$ git remote -v

Set up "origin" (your fork) and "upstream" remotes:

	$ git remote add upstream https://github.com/whynhow/intro-git.git

Push a branch ``cool-feature`` to your fork:

	$ git push origin cool-feature

Fetching branch ``master`` from "upstream":

	$ git fetch upstream master:master
