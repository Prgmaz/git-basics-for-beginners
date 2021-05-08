# Git basics for beginners

![alt text](https://programmer101n.com/assets/images/2021/05/08/0.png)

What we need.
1. A Computer
2. Git CLI
3. Some Basic Terminal commands

## How to Install Git CLI

First go to `http://git-scm.com/` and download latest git cli.

![GIT CLI DOWNLOAD](https://programmer101n.com/assets/images/2021/05/08/1.png)

Now double click it and install it default.

![GIT CLI INSTALLATION](https://programmer101n.com/assets/images/2021/05/08/2.png)

Now we have installed git cli on our pc. Now let's create a repository.

## What is Git?
Git is a version control system, Which can keep track of every modification to the code in some special kind of database. If developer made a mistake, they can reverse the changes to the previous commit.

## How to use git.
First you need a project that will you work on.

In my case, I will create a project. Now open terminal or cmd in that project folder and type `git init`.

![GIT CLI INIT](https://programmer101n.com/assets/images/2021/05/08/3.png)

So now we just initialized a repository in that project folder. Now we have the version control system of that project. But first we need to create a commit.

## What is a git commit?
You can say it as a restore point for your code. Which you can go to, if you have messed up your code or something else.

## How to create a git commit?
1. You need to stage the files for commit. We want to commit all the files so I will type `git add .`, Here `.` represents all files. You can give file names instead of `.`. You can see status of the files by typing `git status`. You can also remove files by typing `git rm <FILE NAME>`. (THIS WILL DELETE THE FILE)
2. Now, we have all the files staged and ready to commit. Type `git commit -m "YOUR MESSAGE"`, `-m` represents the message, You can type any message you want.
3. To see all the commits, You can type `git log`.

![GIT CLI ADD](https://programmer101n.com/assets/images/2021/05/08/4.png)

![GIT CLI LOG](https://programmer101n.com/assets/images/2021/05/08/5.png)

## How to ignore a file or folder from `git add .`?
To ignore a file or folder, you need to create a special file called `.gitignore`. Whatever you will type in this file, Git will ignore them.

### FOR EXAMPLE

I want to ignore `node_modules` folder. So I created a file named `.gitignore` in my project level directory and typed `node_modules` in `.gitignore` file. Now if you stage all the files with `git add .` and see the status with `git status`. You will see that my `node_modules` directory isn't staged, It is now ignored by git.

![GIT CLI IGNORE](https://programmer101n.com/assets/images/2021/05/08/6.png)

![GIT CLI IGNORE](https://programmer101n.com/assets/images/2021/05/08/7.png)

## How to revert back to a commit?
First you need the commit id, You can get it by typing `git log`. You can see all the commits you have in your project.

![GIT CLI LOG](https://programmer101n.com/assets/images/2021/05/08/8.png)

Now type `git reset <ID>` if you want to keep the changes you made but restore the commit. If you want to purge the changes you need to give `git reset --hard <ID>`, It will purge all the changes you did. NOTE: Your commit ID will be in place of `<ID>`.

![GIT CLI RESET](https://programmer101n.com/assets/images/2021/05/08/9.png)

![GIT CLI RESET](https://programmer101n.com/assets/images/2021/05/08/10.png)
