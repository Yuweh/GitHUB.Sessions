### GitHUB.Sessions

#TERMINAL SESSIONS

Areas:
Working Directory (git add)
Staging Area      (git commit)
Local Repository  (git checkout) 


——-
## GIT Sessions

git init - create git for the chosen project or directory

git status - to check status of files if they are tracked or not / check items that are in or not in the staging area

git add - then add name //
git add . (Dot will add all items in the working directory)

git commit -m “Insert message here”

git log (check the commits that are made)

REMOTE
//create remote repository add HTTPs at url
usage: git remote add [<options>] <name> <url>
  
 //push create repository to remote
 git push -u origin master
 
———
## Navigating in the Terminal

cd = change directory
mkdir = make or create directory
touch = create a file and name  ex. Touch READMe.md
ls = list down contents on the chosen folder

touch - to create file (ex. chapter.text or file.html
open - open file (ex. Open chapter.text
vim = take you to the chosen file and open to create content

——
VIM
**inside vim, to create and insert content; press “ i “
**to exit vim press; esc then shift + colon : + x then enter

——-
## GIT Merge or Pull Request

Differences:

Ability to approve or reject request

Ability to provide add a descriptive message with the request


### Pull Request

<img src="https://i.stack.imgur.com/iUcsn.jpg" width="900">


### Merge Request

#### What is the difference between `git merge` and `git merge --no-ff`?

The --no-ff flag prevents git merge from executing a "fast-forward" if it detects that your current HEAD is an ancestor of the commit you're trying to merge. 

A fast-forward is when, instead of constructing a merge commit, git just moves your branch pointer to point at the incoming commit. 

This commonly occurs when doing a git pull without any local changes.


However, occasionally you want to prevent this behavior from happening, typically because you want to maintain a specific branch topology (e.g. you're merging in a topic branch and you want to ensure it looks that way when reading history). 

In order to do that, you can pass the --no-ff flag and git merge will always construct a merge instead of fast-forwarding.

Similarly, if you want to execute a git pull or use git merge in order to explicitly fast-forward, and you want to bail out if it can't fast-forward, then you can use the --ff-only flag. 

This way you can regularly do something like git pull --ff-only without thinking, and then if it errors out you can go back and decide if you want to merge or rebase.


<img src="https://i.stack.imgur.com/GGkZc.png" width="900">

REF: https://stackoverflow.com/questions/9069061/what-is-the-difference-between-git-merge-and-git-merge-no-ff



