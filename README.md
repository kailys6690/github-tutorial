# GitHub Tutorial

_by Kaily Sanchez_

---
## Git vs. GitHub
What is **Git**?


What is **GitHub**?


What is the difference between **Git** and **GitHub**?

Git runs locally, unlike GitHub which runs in the clouds. Git doesn't require GitHub, but GitHub does require Git.
  

---
## Initial Setup



---
## Repository Setup
How do you set up your own repo(sitory)?




---
## Workflow & Commands
These are *the most* important steps to remember because you will **ALWAYS** be using these commands:

1. `git status`
2. `git add`
3. `git status` *(optional)*
4. `git commit -m ""` 
5. `git push` (only _if_ you have )

The commands above are in workflow order. You *__cannot__* use these commands randomly or you will run into many errors. 

`git status` is used to check any changes/ edits made in the working directory. This command can be used as many times as you want and it very helpful.  
Use `git status` often! It can help you if you run into a probelm when you are using the workflow.  
_hint_: to know if your recent edits have been made, they will be in **_red_**!

`git add` is used to add file(s) to the staging area. This doesnt mean it's been fully saved! It has to be commited so the file is pushed to the staging area, waiting to be fully commited.

`git status` is completely optional to use again, but I totally recommend it because you can never underetimate `git status`!  
This is especially helpful to use after adding file(s) because you may never know if you fully added the file to the staging area. This can also check what file(s) you have added to the staging area.  
_hint_: to know if your files are staged for the commit, they will be in **_green_**!

`git commit -m""` is the last step of the workflow and the most important. This command takes a 'snapshot' of the file(s) you have added and fully commits them into the . Otherwords, it is saving the changes you have made **permantely**.

`git push` is used after git commit.

---
### Error Handlings