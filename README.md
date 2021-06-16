# Git - Github

git, created by Torvalds in 2005. It helps to track the progress of the project.

## Difference between Git, GitHub, Gitlab??

git is a version control system whereas Github is a code library and includes git. You can storage your projects private or public in GitHub. Also GitLab is like a GitHub and you can use it on your own server. So generally companies use GitLab.

## Some Git Defines

- repository : This is storage
- master : This is most stable version of project but you can change this name.
- branch : GIT works like tree mechanism. When created a new project, master branch will create automatically. Making changes on master branch is so dangerous. If you don't want to distrupt anything while developing the project, you can create new branch and work on. After the developing you can send changes to the master branch.
- merge : If you want send changes to the master or any branch you must use this command. This command merges branches.
- push : This works for sending the changes to the server.
- pull : This works for getting the changes from the server.
- .gitignore : If you don't want to send some things you can add this things to the .gitignore file.

## Git Codes

- git init : for starting git.
- git status : shows current status.
- git add file.ext : add file to the git
- git add .  : add all files to the git
- git rm —cached file.ext : remove track from git.
- git commit : for applying changes and take snapshot
- git commit -m "initial commit" : commit with message
- git diff : shows all changes after last snapshot
- git branch <branch_name> : for adding new branch to the project
- git branch -a : list all branches.
- git branch -d <branch_name> : for deleting branch by name
- git checkout <branch_name or commit id> : change branch
- git merge <branch name> : it merges the changes in branch to the branch you are in.
- git clone <project url> : for copying the project in your local.
- git push origin master : origin is remote repository and constant but "master" is changable.
- git push : same as the upward. Also you can use this.
- git pull : for getting changes.

## What is the .gitignore and how it works?

As I mentioned above, if you don't want to add something to git you can use .gitignore. I understand to the here but when should i use .gitignore? Let me show you:

- Downloaded dependencies from package manager.
- image and videos files
- IDE extensions
- Secret files (maybe apk signature, some configurations)
- API keys
- Temporary files in work directory.
- Log files.
- Or anything don't you want.

### How is it created?

```java
echo some-text or nothing > .gitignore
```

### Some rules:

- You can add file name :

```java
.env
```

- You can add folders with using '/' :

```java
node-modules/
dist/
logs/
src/temp/
```

- If you don't want to track anything you can add '!' to the head of line :

```java
!files/example.txt
```

- If you want to create comments you can use '#' :

```java
# this is a comment
```

- You can ignore all choosed extension of files with using '*'  :

```java
*.dll
```