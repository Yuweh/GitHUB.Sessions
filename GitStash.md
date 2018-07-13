## GIT STASH

Here are some of the useful tricks I learned about Git stash last week.

---
#### Git stash save
---

git stash save “Your stash message”.

-OR-
stash untracked files.

git stash save -u

git stash save --include-untracked

---
#### Git stash list
---

git stash list

---
#### Git stash apply
---
//This command takes the top most stash in the stack and applies it to the repo. 

git stash apply stash@{1}

---
#### Git stash pop
---
//This command is very similar to stash apply but it deletes the stash from the stack after it is applied.


---
#### Git stash show
---
This command shows the summary of the stash diffs. The above command considers only the latest stash.

git stash show -p // see the full diff

git stash show stash@{1}

---
#### Git stash branch <name>
---

git stash branch <name> stash@{1}

---
#### Git stash clear
---

git stash clear

---
#### Git stash drop
---

git stash drop stash@{1}


