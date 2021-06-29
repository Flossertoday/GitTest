# GitTest
**This is how I use Git**

## Initialize
First of all, clone a project. For example:

        git clone [url]
        git clone https://github.com/Flossertoday/GitTest
    
Optional: Put a customed name on it

        git clone [url] [name]


Move to its root path:

        cd [root_path]
        cd GitTest

'ls' shows everything under this path

        ls
    
Your workspace should have been initialized. Otherwise, 

        git init
        
to create local repository /.git


## Push and Pull
Save all edits to staging area. Commit then push. Meanwile, keep updated. 

Save

        git add .

Commit

        git commit -m [message]
        git commit -m 'update'

Push

        git push [remote_server] [branch]
        git push origin feat

If the local branch name is not the same as the remote one

        git push [remote_server] [local_branch]:[remote_branch]
        git push origin feat:main

Update by pulling

        git pull [remote_server] [branch]
        git pull [remote_server] [remote_branch]:[local_branch]


## Branches

Create a branch and switch to it

        git checkout -b [branch]
        git checkout -b feat

Switch to a branch

        git checkout [branch]
        git checkout feat

Merge branches

        git merge

Delete a branch

        git branch -d [branch]

List local branches

        git branch


## File Operations

Create a new file 

        touch [file]

Delete a file 

        rm [file]

Rename or move

        mv [file] [newfile]

Change path

        cd [path]

Make a new path

        mkdir [newpath]

## Remote

Show remotes

        git remote -v

Show more info about certain remote

        git remote show [remote]

Add remote

        git remote add [name] [link]
        git remote add origin https://github.com/Flossertoday/GitTest


## Others

Show changes

        git status

Show logs

        git log
        
