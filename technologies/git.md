* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 

# Git

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

Git is a version control system that will help us work collaboratively. Our code will be stored in a repository, which we can host remotely on a site like github.com or gitlab.com.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

## Installing

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

## Creating an account

Now create an account on github.com:

https://github.com

And create an access token:

https://github.com/settings/tokens/new

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - 

## Creating a new repository

Create a new remote repository:

https://github.com/new

Initialize a new local repository:

`git init`

Switch to the main branch:

`git branch -M main`

Adding an origin associates a remote repository with your local one:

`git remote add origin <your_project_url>`

Or clone an existing remote repository:

`git clone https://github.com/thizzbuzz/e2stem.full_site.git`


## Pushing an existing repository to a new repository

Create a new repository for the project under one of your accounts:

https://github.com/new

Assuming you've cloned it already, navigate to the *e2stem.full_site* folder and run these commands:

`git remote remove origin` 
`git remote add origin <your_new_repository_url>`
`git branch -M main`
`git push -u origin main`


## Working on an existing project

Every time you work with `git` you'll start by pulling an up-to-date copy of the project:

`git pull origin <your_new_repository_url>`

After you make changes, add these changes to the staging area:

`git add .`

Then to commit these staged files:

`git commit -m "<your_commit_message>"`

And finally to push the changes to the remote repository:

`git push -u origin main`

And that's it! If two people have made changes to the same part of the project, `git` will attempt to merge those changes automatically.



