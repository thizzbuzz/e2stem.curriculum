* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 

## Git

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

Git is a version control system that will help us work collaboratively.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **GIT**

####  Installing git

Start by installing git:

https://gitforwindows.org/

And to check if git is installed run this command in a terminal:

`git --version`

Now configure git by adding your username:

`git config --global user.name "your_username"`

And your email address:

`git config --global user.email "your_email_address@example.com"`

To check the configuration:

`git config --global --list`

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **GITHUB**

#### Creating an account

Now create an account on github.com:

https://github.com

And create an access token:

https://github.com/settings/tokens/new

#### Creating a new repository on github.com

Create a new repository for the project under one of your accounts:

https://github.com/new


- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

🔷🔷🔷 **WORKFLOWS**

#### Cloning a repository

Cloning recreates a full local copy of a remote repository:

`git clone https://github.com/thizzbuzz/e2stem.full_site.git`

#### Creating a local repository 

For new project, navigate to an an empty folder or existing project root

Initialize a new local repository:

`git init`

Switch to the main branch:

`git branch -M main`

Optionally, add an origin to associate your local repository with a new remote repository:

`git remote add origin <your_project_url>`


#### Pushing an existing repository to a new repository

First create a new remote repository on github.com and clone an existing project

Then in a terminal navigate to the root of the project (e.g. the **e2stem.full_site** folder), and run these commands:

`git remote remove origin` 

`git remote add origin <your_new_repository_url>`

`git branch -M main`

`git push -u origin main`


#### Working on an project

Every time you work with `git` you'll start by pulling an up-to-date copy of the project:

`git pull origin <your_new_repository_url>`

In case you see an error, try this:

`git remote prune origin`
`git gc --prune=now`

After you make changes, add these changes to the staging area:

`git add .`

Then to commit these staged files:

`git commit -m "<your_commit_message>"`

And finally to push the changes to the remote repository:

`git push -u origin main`

And that's it! If two people have made changes to the same part of the project, `git` will attempt to merge those changes automatically.



