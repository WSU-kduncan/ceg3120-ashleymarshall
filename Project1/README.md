# Project 1

Our goal in project 1 was to create a git server of our own on our AWS instance. In the process, we practiced with ssh keys, markdown for this readme, and background actions involved with git.

## Setup

How to initialize a brand new repo:

Use 'git init' then add the name before hitting enter. This creates a new repo, workspace, and .git folder.

Can also use the 'git init --bare name.git' to create just a bare repo aka just the .git folder.

Users, permissions:

Different users can be assigned permissions.
rw- = user can read and write
r-- = groupe can read
r-- = anyone on system can read

Keys setup:
.ssh/authorized_keys holds a list of public keys that can authenticate to the system for a given user.
To create new keys, use the command ssh-keygen.

## Usage

Guides below on git commands from a given system to the repo hosted on the AWS instance.

How to clone:
'git clone username@AWS_IP:project_creator/repo_name.git'
Using git clone is a way for users to obtain a copy of the target repo.

How to init:
'git init name' creates an empty repository (also explained in the Setup section above.)

Clone vs. init: both are used to initialize a new git repo, but clone relies on init to create a new repository before copying an existing repository to it.

How to add:
'git add' adds a change in the working directory to a staging area. Doing this action tells Git you'd like to include this change in the next commit.

How to commit:
'git commit' commits the staged changes to the git repo. Can think of these as 'snapshots' from previous versions. Can roll back to previous commits if needed. Can use git diff to compare files to see the changes.

How to push:
'git push' is used to upload the local repo contents to the remote repo. This is the actual transfer of changes from your local copy to the remote repo.

## Proof
Clone to AWS Ubuntu System:
![Clone to AWS Ubuntu system](clone-to-system.png)

Clone to Personal System:
![Clone to personal system](clone-to-personal.png)