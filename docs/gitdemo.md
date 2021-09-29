## Terms

1. Directory -> Folder
1. Terminal or command line -> Interface for text commands
1. CLI - command line interface
1. cd -> change directory
1. Code Editor - Word Processor for writing code
1. Repository -> Project, or the folder/place where your project is kept

1. Git -> Its a tool that tracks the changes in your code over time
1. Github -> A website where you host all of your Git repositories online. Being online it makes to work in groups with other people, and organize your projects into a portfolio for you to show potential employer.

## Git Commands

* clone -> Bring a repository that is hosted somewhere like Github into a folder on your local machine.
``` git clone 
* add -> Track your files and changes in Git
* commit -> Save your files in Git
* push -> Upload Git commits to a remote repo, like Github
* pull -> Download changes from remote repo to your local machine, the opposite of push.
* status -> it will show all of the command that has been created or modified or deleted.

create a new repository on the command line </br>
echo "# demo-repo" >> README.md </br>
git init </br>
git add README.md  </br>
git commit -m "first commit" </br>
git branch -M main </br>
git remote add origin https://github.com/SundarBishnoi/demo-repo.git  </br>
git push -u origin main </br>

or push an existing repository from the command line </br>
git remote add origin https://github.com/SundarBishnoi/demo-repo.git  </br>
git branch -M main  </br>
git push -u origin main </br>



## SSH Keys.

In order to push your code to github repo, you are going to approve that you are the owner of account.
```
SSh-keygen -t rsa -b 4096 -C "sundarlal2929@gmail.com" 
testkey


ls | grep testkey

```


## Git WorkFlow
![Git workflow](../img/git-workflow.JPG)



## Git Branching
![Git branching](../img/git-branching.JPG)

## Commands
```
git checkout -b branch-name // for creating new branch.

git checkout branch-name // for switching branch

git status // to know the status

git branch // to know all of the branches

git diff name-of-branch // will show what are all chanes are made

git merge branch-name

```

when you make changes to code, first thing you do is to save those changes and then commit them to branch. then push those changes to github.

```
git add 

git commit 

git push --set-upstream origin feature-readme-instructions


```

What is a pull request?
Its basically a request to have your code pulled into another branch.  for eg. we are using here feature branch and we want to have our code pulled into the master branch. So we make a PR from the feature branch to the master branch. Now once we have made a PR, anyone can 
review our code, comment on it, ask us to make changes or update the code. Now after you make a PR, you can also update the code just by making additional commits and pushing them up to Github, as long as Its on same branch that you are making the PR with. Once the PR is merged, you will generally delete your feature or source branch. And switch back to the master/main branch. 
Then when you want to make additional coding changes, you will create another new branch and start the process over make your commits, make your PR and then merge again. 

git pull origin master

```

git branch -d name-of-branch // this is to delete the branch once PR is merged.


