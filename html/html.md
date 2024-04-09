# Test

## Testing the CLI

### What is Important to Remember:

-`Do not add nested git repository into another git repository`

-`To  commit a message , Start with  a `**(Capital Letter)** `,and use` **(Present tense** `,` **imperative mode ..ex. Add , Update , fix etc...)**

-` To name a file or folder  use` **(lower case)** `and,` **(hypthens or underscores for spaces)**

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

## **Creating local repositories**

1- **git init** `To turn a folder into a repository`

2- **git status** `To check if the folder is initialized`

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

## **The files have two states:**

### **Untracked files** `The files which have been not added to git`

### **Tracked files** ` The files which have been added to git, and these have the following states:`

| `Modified: The file has been modified since the last commit.`

|| `Staged: The changes in the file have been staged to be included in the next commit.`

||| `Commited: The changes have been saved in git.`

|V `Unmodified : The file has not been changed since the last commit.`

V ` Rename, Recopy: The file has been renamed or copied.`

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

## **Committing in a local repository**

1 - **git status** `To list all files which have been changed`

2- **git add <filename>** `Add a file to the stage`

3- **git add .** `add all the files to the stage`

4- **git commit -m "your message"** ` To record the changes made to the repository and commit a message directly on the command line`

5- **git log** `To display all the commits made in the repository starting from thr recenr commit and going backwards `

6 - **git log --online** `To display more condensed version of the commit history`

 <div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

## **Backups**

1- **git restore .** `To restore all the files to their previous state in staging area, it will discard the changes made to tracked files [worth to mention that (git restore .) doesn't work for untracked files]`

2- **git restore <filename>** `To restore specific file`

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

## **Connecting the local repository to a remote repository**

1- ` In Github add a new repository`

2- `copy the commands from Github:`

git remote add origin git@github.com:GitHubUsername/repository-name.git
git branch -M main
git push -u origin main`

3- **git clone <url>**`To create copy of the remote repository locally`

4- **git push** `Upload content to the remote repository`

5-**git pull** `Download content from the remote repository`

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

# Git Branches and PRS

## some useful commands:

1- **git switch branch-name** `To add a new branch and switching to it.`

2- **git push -u origin branch-name** `To push the changes from our main branch to the remote repository.`

3- **git switch -** `To switch to the previously checked out branch.`

<div style="background-color:#FFFF78; padding:1px; color: black;">
</div>

**Important to remember**

`After we push our local repository, we should make pull and request in order for our colleagues to check our code. If the changes are approved, we can now merge them with our main remote repository. We can now delete the pull and request on Github`

`In our Terminal we should now use `**git pull** `command to download the content from our remote repository and update our local repository.`
`we can now delete our branch locally on our terminal ....using the commands:` **git branch -d branch-name** `but if the branch has unmerged changes,git won't let us deleted it unless we used this command.` **git branch -D branch-name**
