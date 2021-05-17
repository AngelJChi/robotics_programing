# Command line of git.
## By Angel Chi 2C.

## git init 
git init is used to create a new local GIT repository.
The new repository will be create in the current directory

```sh
git init
```

As an alternative, you can create a repository inside of a new directory specifying the name of the project

```sh
git init [name of the project]
```



## git clone
git cloneis used to clone or copy a repository. If the repository is in a remote server use:

```sh
git clone nameoftheuser@host:/path/to/repository
```

Conversely, run the following basic command to copy a local repository:

```sh
git /path/to/repository
```



## git add
git add is used to add files to the preparation area

```sh
git add name.(format of the file: txt, md, rtf, etc.)
gti add example.md
```



## git commit
git commit will create a snapshot of the changes and save it in the git directory

```sh
git commit -m "name of the commit"
git commit -m "first commit"
```
Remember that the changes won't come to the remote repository


## git config
git config can be used to set specific user settings, such as email, user name and format type, etc. 

```sh
git config --global user.email "youremail@example.com"
git config --global user. name "2009039@upy.edu.mx"

git config --global user.name "yourname"
git config --global user.name "AngelJChi"
```

The -global option tells GIT that you are going to use that email for all local repositories. If you want to use different emails for different repositories, use the following command:

```sh
git config --global user.email "youremail@example.com"
git config --global user. name "2009039@upy.edu.mx"

git config --local user.name "yourname"
git config --local user.name "AngelJChi"
```



## git status
git status shows the list of the files that have been changed. Show the status of the work and branches

```sh
git status
```



## git push 
git push is used to send local commits to the master branch of the remote repository

```sh
git push -u origin main
```



## git checkout
git checkout is used to create branches

```sh
git checkout -b name
```
To switch from one branch to another, just use:
```sh
git checkout name
```



## git remote
git remote allows see all the remote repositories

```sh
git remote -v
```
to connect the local repository to a remote server use:

```sh
git remote add origin remoteURL
git remote add origin https://github.com/AngelJChi/robotics_programing.git
```
On the other hand, the following commmand will delete a connection to a specified remote repository

```sh
git remote nameoftherepository
```



## git branch
git branch is used to list, create or delete branches. If you want to see all the branches in the repository, use:

```sh
git branch -list
```

If you want to create a new branch, use:

```sh
git branch -M name
```

If you want to delete a branch, use:

```sh
git branch -D name
```
