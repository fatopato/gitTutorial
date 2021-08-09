# Introduction to Git

Basics for git

## Initialize the git
You need to specify a folder or workspace for git to track. After initialization git can detect the changes.

In order to initialize the git in a workspace:
``` shell
git init 
```
a file named '.git' is created after initialization process. 

## Add files to git
You need to add files to track.
You can add single file by:
``` shell
git add [filename]
```
or you can add all files on workspace:
``` shell
git add . 
```
After modify any file you need to add it again.

## Commit changes
Adding is not enough to save the changes to the local repository. After you add files to staging you need to commit changes to save.

In order to commit the changes:

``` shell
git commit -m "[commit message]" 
```

You can add commit message after -m parameter. For example:

``` shell
git commit -m "All files added to the workspace" 
```

## Push to Remote Repository (Optional)

If you have a remote repository, you can push your local changes.
First you need to specify the remote repo address:

``` shell
git remote add origin [repository address]
```

The remote repository address should be placed such as:
``` shell
git remote add origin https://github.com/fatopato/gitTutorial.git
```

**origin** is the remote repo name. You can give any name but origin is the common name for it.

After adding the remote repo now you can push the local code to the remote by:
``` shell
git push origin [branch_name]
```
You can specify the remote branch by changing the branch name but the common branch name for first commit is **master**
For example in order to the push local branch to remote master branch:

``` shell
git push origin master
```
